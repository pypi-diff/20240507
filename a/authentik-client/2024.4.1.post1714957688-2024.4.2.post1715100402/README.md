# Comparing `tmp/authentik_client-2024.4.1.post1714957688.tar.gz` & `tmp/authentik_client-2024.4.2.post1715100402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authentik_client-2024.4.1.post1714957688.tar", max compression
+gzip compressed data, was "authentik_client-2024.4.2.post1715100402.tar", max compression
```

## Comparing `authentik_client-2024.4.1.post1714957688.tar` & `authentik_client-2024.4.2.post1715100402.tar`

### file list

```diff
@@ -1,596 +1,596 @@
--rw-r--r--   0        0        0   143973 2024-05-06 01:08:21.852086 authentik_client-2024.4.1.post1714957688/README.md
--rw-r--r--   0        0        0    48535 2024-05-06 01:08:21.860086 authentik_client-2024.4.1.post1714957688/authentik_client/__init__.py
--rw-r--r--   0        0        0     1170 2024-05-06 01:08:21.860086 authentik_client-2024.4.1.post1714957688/authentik_client/api/__init__.py
--rw-r--r--   0        0        0    97518 2024-05-06 01:08:21.564083 authentik_client-2024.4.1.post1714957688/authentik_client/api/admin_api.py
--rw-r--r--   0        0        0   700271 2024-05-06 01:08:21.588084 authentik_client-2024.4.1.post1714957688/authentik_client/api/authenticators_api.py
--rw-r--r--   0        0        0   701197 2024-05-06 01:08:21.612084 authentik_client-2024.4.1.post1714957688/authentik_client/api/core_api.py
--rw-r--r--   0        0        0   116805 2024-05-06 01:08:21.628084 authentik_client-2024.4.1.post1714957688/authentik_client/api/crypto_api.py
--rw-r--r--   0        0        0   107946 2024-05-06 01:08:21.636084 authentik_client-2024.4.1.post1714957688/authentik_client/api/enterprise_api.py
--rw-r--r--   0        0        0   408008 2024-05-06 01:08:21.648084 authentik_client-2024.4.1.post1714957688/authentik_client/api/events_api.py
--rw-r--r--   0        0        0   280806 2024-05-06 01:08:21.664085 authentik_client-2024.4.1.post1714957688/authentik_client/api/flows_api.py
--rw-r--r--   0        0        0   101134 2024-05-06 01:08:21.676085 authentik_client-2024.4.1.post1714957688/authentik_client/api/managed_api.py
--rw-r--r--   0        0        0   135649 2024-05-06 01:08:21.684085 authentik_client-2024.4.1.post1714957688/authentik_client/api/oauth2_api.py
--rw-r--r--   0        0        0   413301 2024-05-06 01:08:21.696085 authentik_client-2024.4.1.post1714957688/authentik_client/api/outposts_api.py
--rw-r--r--   0        0        0   725201 2024-05-06 01:08:21.708085 authentik_client-2024.4.1.post1714957688/authentik_client/api/policies_api.py
--rw-r--r--   0        0        0   552586 2024-05-06 01:08:21.720085 authentik_client-2024.4.1.post1714957688/authentik_client/api/propertymappings_api.py
--rw-r--r--   0        0        0   718066 2024-05-06 01:08:21.732085 authentik_client-2024.4.1.post1714957688/authentik_client/api/providers_api.py
--rw-r--r--   0        0        0   150485 2024-05-06 01:08:21.744085 authentik_client-2024.4.1.post1714957688/authentik_client/api/rac_api.py
--rw-r--r--   0        0        0   207550 2024-05-06 01:08:21.752085 authentik_client-2024.4.1.post1714957688/authentik_client/api/rbac_api.py
--rw-r--r--   0        0        0    10391 2024-05-06 01:08:21.760085 authentik_client-2024.4.1.post1714957688/authentik_client/api/root_api.py
--rw-r--r--   0        0        0    11845 2024-05-06 01:08:21.764085 authentik_client-2024.4.1.post1714957688/authentik_client/api/schema_api.py
--rw-r--r--   0        0        0  1037225 2024-05-06 01:08:21.784086 authentik_client-2024.4.1.post1714957688/authentik_client/api/sources_api.py
--rw-r--r--   0        0        0  1945986 2024-05-06 01:08:21.824086 authentik_client-2024.4.1.post1714957688/authentik_client/api/stages_api.py
--rw-r--r--   0        0        0   157909 2024-05-06 01:08:21.844086 authentik_client-2024.4.1.post1714957688/authentik_client/api/tenants_api.py
--rw-r--r--   0        0        0    25779 2024-05-06 01:08:21.864086 authentik_client-2024.4.1.post1714957688/authentik_client/api_client.py
--rw-r--r--   0        0        0      652 2024-05-06 01:08:21.864086 authentik_client-2024.4.1.post1714957688/authentik_client/api_response.py
--rw-r--r--   0        0        0    14724 2024-05-06 01:08:21.856086 authentik_client-2024.4.1.post1714957688/authentik_client/configuration.py
--rw-r--r--   0        0        0     5934 2024-05-06 01:08:21.860086 authentik_client-2024.4.1.post1714957688/authentik_client/exceptions.py
--rw-r--r--   0        0        0    46837 2024-05-06 01:08:21.860086 authentik_client-2024.4.1.post1714957688/authentik_client/models/__init__.py
--rw-r--r--   0        0        0     4513 2024-05-06 01:08:18.596056 authentik_client-2024.4.1.post1714957688/authentik_client/models/access_denied_challenge.py
--rw-r--r--   0        0        0      688 2024-05-06 01:08:18.604056 authentik_client-2024.4.1.post1714957688/authentik_client/models/alg_enum.py
--rw-r--r--   0        0        0     2482 2024-05-06 01:08:18.616056 authentik_client-2024.4.1.post1714957688/authentik_client/models/app.py
--rw-r--r--   0        0        0     4230 2024-05-06 01:08:18.624056 authentik_client-2024.4.1.post1714957688/authentik_client/models/app_enum.py
--rw-r--r--   0        0        0     2702 2024-05-06 01:08:18.632056 authentik_client-2024.4.1.post1714957688/authentik_client/models/apple_challenge_response_request.py
--rw-r--r--   0        0        0     4508 2024-05-06 01:08:18.644056 authentik_client-2024.4.1.post1714957688/authentik_client/models/apple_login_challenge.py
--rw-r--r--   0        0        0     6686 2024-05-06 01:08:18.656057 authentik_client-2024.4.1.post1714957688/authentik_client/models/application.py
--rw-r--r--   0        0        0     4473 2024-05-06 01:08:18.664057 authentik_client-2024.4.1.post1714957688/authentik_client/models/application_request.py
--rw-r--r--   0        0        0      711 2024-05-06 01:08:18.668057 authentik_client-2024.4.1.post1714957688/authentik_client/models/auth_mode_enum.py
--rw-r--r--   0        0        0      709 2024-05-06 01:08:18.676057 authentik_client-2024.4.1.post1714957688/authentik_client/models/auth_type_enum.py
--rw-r--r--   0        0        0     5195 2024-05-06 01:08:18.680057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session.py
--rw-r--r--   0        0        0     3064 2024-05-06 01:08:18.688057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session_asn.py
--rw-r--r--   0        0        0     2826 2024-05-06 01:08:18.696057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session_geo_ip.py
--rw-r--r--   0        0        0     3865 2024-05-06 01:08:18.700057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session_user_agent.py
--rw-r--r--   0        0        0     2646 2024-05-06 01:08:18.708057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session_user_agent_device.py
--rw-r--r--   0        0        0     2792 2024-05-06 01:08:18.716057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session_user_agent_os.py
--rw-r--r--   0        0        0     2725 2024-05-06 01:08:18.720057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session_user_agent_user_agent.py
--rw-r--r--   0        0        0      895 2024-05-06 01:08:18.724057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authentication_enum.py
--rw-r--r--   0        0        0      782 2024-05-06 01:08:18.728057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_attachment_enum.py
--rw-r--r--   0        0        0     4686 2024-05-06 01:08:18.736057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_duo_challenge.py
--rw-r--r--   0        0        0     2743 2024-05-06 01:08:18.740057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_duo_challenge_response_request.py
--rw-r--r--   0        0        0     5327 2024-05-06 01:08:18.748057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_duo_stage.py
--rw-r--r--   0        0        0     2768 2024-05-06 01:08:18.764057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_duo_stage_device_import_response.py
--rw-r--r--   0        0        0     2785 2024-05-06 01:08:18.768057 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
--rw-r--r--   0        0        0     4744 2024-05-06 01:08:18.776058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     4594 2024-05-06 01:08:18.784058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_sms_challenge.py
--rw-r--r--   0        0        0     3022 2024-05-06 01:08:18.788058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_sms_challenge_response_request.py
--rw-r--r--   0        0        0     6409 2024-05-06 01:08:18.796058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_sms_stage.py
--rw-r--r--   0        0        0     5595 2024-05-06 01:08:18.800058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4474 2024-05-06 01:08:18.808058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_static_challenge.py
--rw-r--r--   0        0        0     2761 2024-05-06 01:08:18.816058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_static_challenge_response_request.py
--rw-r--r--   0        0        0     5363 2024-05-06 01:08:18.820058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_static_stage.py
--rw-r--r--   0        0        0     4392 2024-05-06 01:08:18.828058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4468 2024-05-06 01:08:18.832058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_totp_challenge.py
--rw-r--r--   0        0        0     2858 2024-05-06 01:08:18.836058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_totp_challenge_response_request.py
--rw-r--r--   0        0        0     5132 2024-05-06 01:08:18.844058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_totp_stage.py
--rw-r--r--   0        0        0     4201 2024-05-06 01:08:18.848058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     6722 2024-05-06 01:08:18.856058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_validate_stage.py
--rw-r--r--   0        0        0     4893 2024-05-06 01:08:18.860058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5717 2024-05-06 01:08:18.864058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_validation_challenge.py
--rw-r--r--   0        0        0     3805 2024-05-06 01:08:18.872058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_validation_challenge_response_request.py
--rw-r--r--   0        0        0     4499 2024-05-06 01:08:18.876058 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_web_authn_challenge.py
--rw-r--r--   0        0        0     2852 2024-05-06 01:08:18.880059 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_web_authn_challenge_response_request.py
--rw-r--r--   0        0        0     7081 2024-05-06 01:08:18.884059 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_web_authn_stage.py
--rw-r--r--   0        0        0     5302 2024-05-06 01:08:18.892059 authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     2718 2024-05-06 01:08:18.896059 authentik_client-2024.4.1.post1714957688/authentik_client/models/auto_submit_challenge_response_request.py
--rw-r--r--   0        0        0     4388 2024-05-06 01:08:18.900059 authentik_client-2024.4.1.post1714957688/authentik_client/models/autosubmit_challenge.py
--rw-r--r--   0        0        0      950 2024-05-06 01:08:18.904059 authentik_client-2024.4.1.post1714957688/authentik_client/models/backends_enum.py
--rw-r--r--   0        0        0      748 2024-05-06 01:08:18.908059 authentik_client-2024.4.1.post1714957688/authentik_client/models/binding_type_enum.py
--rw-r--r--   0        0        0     2995 2024-05-06 01:08:18.912059 authentik_client-2024.4.1.post1714957688/authentik_client/models/blueprint_file.py
--rw-r--r--   0        0        0     4453 2024-05-06 01:08:18.916059 authentik_client-2024.4.1.post1714957688/authentik_client/models/blueprint_instance.py
--rw-r--r--   0        0        0     3208 2024-05-06 01:08:18.920059 authentik_client-2024.4.1.post1714957688/authentik_client/models/blueprint_instance_request.py
--rw-r--r--   0        0        0      836 2024-05-06 01:08:18.924059 authentik_client-2024.4.1.post1714957688/authentik_client/models/blueprint_instance_status_enum.py
--rw-r--r--   0        0        0     6255 2024-05-06 01:08:18.928059 authentik_client-2024.4.1.post1714957688/authentik_client/models/brand.py
--rw-r--r--   0        0        0     6307 2024-05-06 01:08:18.932059 authentik_client-2024.4.1.post1714957688/authentik_client/models/brand_request.py
--rw-r--r--   0        0        0     2501 2024-05-06 01:08:18.936059 authentik_client-2024.4.1.post1714957688/authentik_client/models/cache.py
--rw-r--r--   0        0        0      875 2024-05-06 01:08:18.936059 authentik_client-2024.4.1.post1714957688/authentik_client/models/capabilities_enum.py
--rw-r--r--   0        0        0     4476 2024-05-06 01:08:18.940059 authentik_client-2024.4.1.post1714957688/authentik_client/models/captcha_challenge.py
--rw-r--r--   0        0        0     2797 2024-05-06 01:08:18.944059 authentik_client-2024.4.1.post1714957688/authentik_client/models/captcha_challenge_response_request.py
--rw-r--r--   0        0        0     4438 2024-05-06 01:08:18.948059 authentik_client-2024.4.1.post1714957688/authentik_client/models/captcha_stage.py
--rw-r--r--   0        0        0     3774 2024-05-06 01:08:18.952059 authentik_client-2024.4.1.post1714957688/authentik_client/models/captcha_stage_request.py
--rw-r--r--   0        0        0     2522 2024-05-06 01:08:18.956059 authentik_client-2024.4.1.post1714957688/authentik_client/models/certificate_data.py
--rw-r--r--   0        0        0     2990 2024-05-06 01:08:18.964059 authentik_client-2024.4.1.post1714957688/authentik_client/models/certificate_generation_request.py
--rw-r--r--   0        0        0     6655 2024-05-06 01:08:18.968059 authentik_client-2024.4.1.post1714957688/authentik_client/models/certificate_key_pair.py
--rw-r--r--   0        0        0     2989 2024-05-06 01:08:18.972059 authentik_client-2024.4.1.post1714957688/authentik_client/models/certificate_key_pair_request.py
--rw-r--r--   0        0        0      747 2024-05-06 01:08:18.976060 authentik_client-2024.4.1.post1714957688/authentik_client/models/challenge_choices.py
--rw-r--r--   0        0        0    24236 2024-05-06 01:08:18.984059 authentik_client-2024.4.1.post1714957688/authentik_client/models/challenge_types.py
--rw-r--r--   0        0        0      729 2024-05-06 01:08:18.984059 authentik_client-2024.4.1.post1714957688/authentik_client/models/client_type_enum.py
--rw-r--r--   0        0        0     3539 2024-05-06 01:08:18.988060 authentik_client-2024.4.1.post1714957688/authentik_client/models/config.py
--rw-r--r--   0        0        0     4021 2024-05-06 01:08:18.992060 authentik_client-2024.4.1.post1714957688/authentik_client/models/connection_token.py
--rw-r--r--   0        0        0     2662 2024-05-06 01:08:18.996060 authentik_client-2024.4.1.post1714957688/authentik_client/models/connection_token_request.py
--rw-r--r--   0        0        0     5736 2024-05-06 01:08:19.004060 authentik_client-2024.4.1.post1714957688/authentik_client/models/consent_challenge.py
--rw-r--r--   0        0        0     2838 2024-05-06 01:08:19.008060 authentik_client-2024.4.1.post1714957688/authentik_client/models/consent_challenge_response_request.py
--rw-r--r--   0        0        0     2513 2024-05-06 01:08:19.012060 authentik_client-2024.4.1.post1714957688/authentik_client/models/consent_permission.py
--rw-r--r--   0        0        0     4511 2024-05-06 01:08:19.016060 authentik_client-2024.4.1.post1714957688/authentik_client/models/consent_stage.py
--rw-r--r--   0        0        0      783 2024-05-06 01:08:19.016060 authentik_client-2024.4.1.post1714957688/authentik_client/models/consent_stage_mode_enum.py
--rw-r--r--   0        0        0     3569 2024-05-06 01:08:19.024060 authentik_client-2024.4.1.post1714957688/authentik_client/models/consent_stage_request.py
--rw-r--r--   0        0        0     2891 2024-05-06 01:08:19.028060 authentik_client-2024.4.1.post1714957688/authentik_client/models/contextual_flow_info.py
--rw-r--r--   0        0        0      879 2024-05-06 01:08:19.032060 authentik_client-2024.4.1.post1714957688/authentik_client/models/contextual_flow_info_layout_enum.py
--rw-r--r--   0        0        0     2657 2024-05-06 01:08:19.032060 authentik_client-2024.4.1.post1714957688/authentik_client/models/coordinate.py
--rw-r--r--   0        0        0     4704 2024-05-06 01:08:19.036060 authentik_client-2024.4.1.post1714957688/authentik_client/models/current_brand.py
--rw-r--r--   0        0        0      771 2024-05-06 01:08:19.040060 authentik_client-2024.4.1.post1714957688/authentik_client/models/denied_action_enum.py
--rw-r--r--   0        0        0     4200 2024-05-06 01:08:19.044060 authentik_client-2024.4.1.post1714957688/authentik_client/models/deny_stage.py
--rw-r--r--   0        0        0     3230 2024-05-06 01:08:19.048060 authentik_client-2024.4.1.post1714957688/authentik_client/models/deny_stage_request.py
--rw-r--r--   0        0        0     3522 2024-05-06 01:08:19.060060 authentik_client-2024.4.1.post1714957688/authentik_client/models/device.py
--rw-r--r--   0        0        0     2657 2024-05-06 01:08:19.064060 authentik_client-2024.4.1.post1714957688/authentik_client/models/device_challenge.py
--rw-r--r--   0        0        0     2792 2024-05-06 01:08:19.072060 authentik_client-2024.4.1.post1714957688/authentik_client/models/device_challenge_request.py
--rw-r--r--   0        0        0      780 2024-05-06 01:08:19.076060 authentik_client-2024.4.1.post1714957688/authentik_client/models/device_classes_enum.py
--rw-r--r--   0        0        0     1244 2024-05-06 01:08:19.080060 authentik_client-2024.4.1.post1714957688/authentik_client/models/digest_algorithm_enum.py
--rw-r--r--   0        0        0      695 2024-05-06 01:08:19.080060 authentik_client-2024.4.1.post1714957688/authentik_client/models/digits_enum.py
--rw-r--r--   0        0        0     4969 2024-05-06 01:08:19.084061 authentik_client-2024.4.1.post1714957688/authentik_client/models/docker_service_connection.py
--rw-r--r--   0        0        0     4087 2024-05-06 01:08:19.092060 authentik_client-2024.4.1.post1714957688/authentik_client/models/docker_service_connection_request.py
--rw-r--r--   0        0        0     2847 2024-05-06 01:08:19.096061 authentik_client-2024.4.1.post1714957688/authentik_client/models/domain.py
--rw-r--r--   0        0        0     2746 2024-05-06 01:08:19.100061 authentik_client-2024.4.1.post1714957688/authentik_client/models/domain_request.py
--rw-r--r--   0        0        0     4155 2024-05-06 01:08:19.104061 authentik_client-2024.4.1.post1714957688/authentik_client/models/dummy_challenge.py
--rw-r--r--   0        0        0     2681 2024-05-06 01:08:19.108061 authentik_client-2024.4.1.post1714957688/authentik_client/models/dummy_challenge_response_request.py
--rw-r--r--   0        0        0     4515 2024-05-06 01:08:19.112061 authentik_client-2024.4.1.post1714957688/authentik_client/models/dummy_policy.py
--rw-r--r--   0        0        0     3237 2024-05-06 01:08:19.120061 authentik_client-2024.4.1.post1714957688/authentik_client/models/dummy_policy_request.py
--rw-r--r--   0        0        0     4213 2024-05-06 01:08:19.124061 authentik_client-2024.4.1.post1714957688/authentik_client/models/dummy_stage.py
--rw-r--r--   0        0        0     3232 2024-05-06 01:08:19.128061 authentik_client-2024.4.1.post1714957688/authentik_client/models/dummy_stage_request.py
--rw-r--r--   0        0        0     2720 2024-05-06 01:08:19.132061 authentik_client-2024.4.1.post1714957688/authentik_client/models/duo_device.py
--rw-r--r--   0        0        0     2575 2024-05-06 01:08:19.136061 authentik_client-2024.4.1.post1714957688/authentik_client/models/duo_device_enrollment_status.py
--rw-r--r--   0        0        0     2619 2024-05-06 01:08:19.140061 authentik_client-2024.4.1.post1714957688/authentik_client/models/duo_device_request.py
--rw-r--r--   0        0        0      748 2024-05-06 01:08:19.144061 authentik_client-2024.4.1.post1714957688/authentik_client/models/duo_response_enum.py
--rw-r--r--   0        0        0     4090 2024-05-06 01:08:19.148061 authentik_client-2024.4.1.post1714957688/authentik_client/models/email_challenge.py
--rw-r--r--   0        0        0     2770 2024-05-06 01:08:19.152061 authentik_client-2024.4.1.post1714957688/authentik_client/models/email_challenge_response_request.py
--rw-r--r--   0        0        0     5902 2024-05-06 01:08:19.160061 authentik_client-2024.4.1.post1714957688/authentik_client/models/email_stage.py
--rw-r--r--   0        0        0     5121 2024-05-06 01:08:19.164061 authentik_client-2024.4.1.post1714957688/authentik_client/models/email_stage_request.py
--rw-r--r--   0        0        0     4707 2024-05-06 01:08:19.168061 authentik_client-2024.4.1.post1714957688/authentik_client/models/endpoint.py
--rw-r--r--   0        0        0     3678 2024-05-06 01:08:19.176061 authentik_client-2024.4.1.post1714957688/authentik_client/models/endpoint_request.py
--rw-r--r--   0        0        0     2530 2024-05-06 01:08:19.180061 authentik_client-2024.4.1.post1714957688/authentik_client/models/error_detail.py
--rw-r--r--   0        0        0     3309 2024-05-06 01:08:19.184061 authentik_client-2024.4.1.post1714957688/authentik_client/models/error_reporting_config.py
--rw-r--r--   0        0        0     4129 2024-05-06 01:08:19.188061 authentik_client-2024.4.1.post1714957688/authentik_client/models/event.py
--rw-r--r--   0        0        0     1730 2024-05-06 01:08:19.192062 authentik_client-2024.4.1.post1714957688/authentik_client/models/event_actions.py
--rw-r--r--   0        0        0     6006 2024-05-06 01:08:19.196061 authentik_client-2024.4.1.post1714957688/authentik_client/models/event_matcher_policy.py
--rw-r--r--   0        0        0     4807 2024-05-06 01:08:19.204062 authentik_client-2024.4.1.post1714957688/authentik_client/models/event_matcher_policy_request.py
--rw-r--r--   0        0        0     3990 2024-05-06 01:08:19.212062 authentik_client-2024.4.1.post1714957688/authentik_client/models/event_request.py
--rw-r--r--   0        0        0     2697 2024-05-06 01:08:19.220062 authentik_client-2024.4.1.post1714957688/authentik_client/models/event_top_per_user.py
--rw-r--r--   0        0        0     3926 2024-05-06 01:08:19.224062 authentik_client-2024.4.1.post1714957688/authentik_client/models/expiring_base_grant_model.py
--rw-r--r--   0        0        0     4191 2024-05-06 01:08:19.232062 authentik_client-2024.4.1.post1714957688/authentik_client/models/expression_policy.py
--rw-r--r--   0        0        0     2992 2024-05-06 01:08:19.240062 authentik_client-2024.4.1.post1714957688/authentik_client/models/expression_policy_request.py
--rw-r--r--   0        0        0     4524 2024-05-06 01:08:19.248062 authentik_client-2024.4.1.post1714957688/authentik_client/models/extra_role_object_permission.py
--rw-r--r--   0        0        0     4524 2024-05-06 01:08:19.252062 authentik_client-2024.4.1.post1714957688/authentik_client/models/extra_user_object_permission.py
--rw-r--r--   0        0        0     2519 2024-05-06 01:08:19.260062 authentik_client-2024.4.1.post1714957688/authentik_client/models/file_path_request.py
--rw-r--r--   0        0        0     6047 2024-05-06 01:08:19.268062 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow.py
--rw-r--r--   0        0        0    25850 2024-05-06 01:08:19.276062 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_challenge_response_request.py
--rw-r--r--   0        0        0      934 2024-05-06 01:08:19.280062 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_designation_enum.py
--rw-r--r--   0        0        0     2533 2024-05-06 01:08:19.288062 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_diagram.py
--rw-r--r--   0        0        0     4505 2024-05-06 01:08:19.296062 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_error_challenge.py
--rw-r--r--   0        0        0     3111 2024-05-06 01:08:19.300063 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_import_result.py
--rw-r--r--   0        0        0     3418 2024-05-06 01:08:19.308063 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_inspection.py
--rw-r--r--   0        0        0     3875 2024-05-06 01:08:19.316063 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_inspector_plan.py
--rw-r--r--   0        0        0      837 2024-05-06 01:08:19.320063 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_layout_enum.py
--rw-r--r--   0        0        0     4741 2024-05-06 01:08:19.324063 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_request.py
--rw-r--r--   0        0        0     5223 2024-05-06 01:08:19.332063 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_set.py
--rw-r--r--   0        0        0     4459 2024-05-06 01:08:19.340063 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_set_request.py
--rw-r--r--   0        0        0     4763 2024-05-06 01:08:19.344063 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_stage_binding.py
--rw-r--r--   0        0        0     3983 2024-05-06 01:08:19.352063 authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_stage_binding_request.py
--rw-r--r--   0        0        0     2641 2024-05-06 01:08:19.356063 authentik_client-2024.4.1.post1714957688/authentik_client/models/footer_link.py
--rw-r--r--   0        0        0     2531 2024-05-06 01:08:19.360063 authentik_client-2024.4.1.post1714957688/authentik_client/models/generic_error.py
--rw-r--r--   0        0        0      865 2024-05-06 01:08:19.364063 authentik_client-2024.4.1.post1714957688/authentik_client/models/geoip_binding_enum.py
--rw-r--r--   0        0        0     5445 2024-05-06 01:08:19.368063 authentik_client-2024.4.1.post1714957688/authentik_client/models/group.py
--rw-r--r--   0        0        0     4209 2024-05-06 01:08:19.376063 authentik_client-2024.4.1.post1714957688/authentik_client/models/group_member.py
--rw-r--r--   0        0        0     4006 2024-05-06 01:08:19.380063 authentik_client-2024.4.1.post1714957688/authentik_client/models/group_member_request.py
--rw-r--r--   0        0        0     3347 2024-05-06 01:08:19.384063 authentik_client-2024.4.1.post1714957688/authentik_client/models/group_request.py
--rw-r--r--   0        0        0     6080 2024-05-06 01:08:19.392063 authentik_client-2024.4.1.post1714957688/authentik_client/models/identification_challenge.py
--rw-r--r--   0        0        0     3174 2024-05-06 01:08:19.396063 authentik_client-2024.4.1.post1714957688/authentik_client/models/identification_challenge_response_request.py
--rw-r--r--   0        0        0     7503 2024-05-06 01:08:19.404063 authentik_client-2024.4.1.post1714957688/authentik_client/models/identification_stage.py
--rw-r--r--   0        0        0     6533 2024-05-06 01:08:19.412063 authentik_client-2024.4.1.post1714957688/authentik_client/models/identification_stage_request.py
--rw-r--r--   0        0        0     2438 2024-05-06 01:08:19.416064 authentik_client-2024.4.1.post1714957688/authentik_client/models/install_id.py
--rw-r--r--   0        0        0      771 2024-05-06 01:08:19.420064 authentik_client-2024.4.1.post1714957688/authentik_client/models/intent_enum.py
--rw-r--r--   0        0        0      800 2024-05-06 01:08:19.420064 authentik_client-2024.4.1.post1714957688/authentik_client/models/invalid_response_action_enum.py
--rw-r--r--   0        0        0     4878 2024-05-06 01:08:19.428064 authentik_client-2024.4.1.post1714957688/authentik_client/models/invitation.py
--rw-r--r--   0        0        0     3895 2024-05-06 01:08:19.436064 authentik_client-2024.4.1.post1714957688/authentik_client/models/invitation_request.py
--rw-r--r--   0        0        0     4508 2024-05-06 01:08:19.444064 authentik_client-2024.4.1.post1714957688/authentik_client/models/invitation_stage.py
--rw-r--r--   0        0        0     3527 2024-05-06 01:08:19.448064 authentik_client-2024.4.1.post1714957688/authentik_client/models/invitation_stage_request.py
--rw-r--r--   0        0        0      729 2024-05-06 01:08:19.452064 authentik_client-2024.4.1.post1714957688/authentik_client/models/issuer_mode_enum.py
--rw-r--r--   0        0        0     4386 2024-05-06 01:08:19.456064 authentik_client-2024.4.1.post1714957688/authentik_client/models/kubernetes_service_connection.py
--rw-r--r--   0        0        0     3454 2024-05-06 01:08:19.464064 authentik_client-2024.4.1.post1714957688/authentik_client/models/kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     2811 2024-05-06 01:08:19.472064 authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_debug.py
--rw-r--r--   0        0        0     5765 2024-05-06 01:08:19.476064 authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_outpost_config.py
--rw-r--r--   0        0        0     4378 2024-05-06 01:08:19.480064 authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_property_mapping.py
--rw-r--r--   0        0        0     3478 2024-05-06 01:08:19.480064 authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_property_mapping_request.py
--rw-r--r--   0        0        0     8694 2024-05-06 01:08:19.484064 authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_provider.py
--rw-r--r--   0        0        0     6192 2024-05-06 01:08:19.488064 authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_provider_request.py
--rw-r--r--   0        0        0    11791 2024-05-06 01:08:19.492064 authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_source.py
--rw-r--r--   0        0        0     9542 2024-05-06 01:08:19.500064 authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_source_request.py
--rw-r--r--   0        0        0     3129 2024-05-06 01:08:19.504064 authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_sync_status.py
--rw-r--r--   0        0        0      726 2024-05-06 01:08:19.468064 authentik_client-2024.4.1.post1714957688/authentik_client/models/ldapapi_access_mode.py
--rw-r--r--   0        0        0     3278 2024-05-06 01:08:19.504064 authentik_client-2024.4.1.post1714957688/authentik_client/models/license.py
--rw-r--r--   0        0        0     2897 2024-05-06 01:08:19.512065 authentik_client-2024.4.1.post1714957688/authentik_client/models/license_forecast.py
--rw-r--r--   0        0        0     2509 2024-05-06 01:08:19.516065 authentik_client-2024.4.1.post1714957688/authentik_client/models/license_request.py
--rw-r--r--   0        0        0     3222 2024-05-06 01:08:19.520064 authentik_client-2024.4.1.post1714957688/authentik_client/models/license_summary.py
--rw-r--r--   0        0        0     2411 2024-05-06 01:08:19.528065 authentik_client-2024.4.1.post1714957688/authentik_client/models/link.py
--rw-r--r--   0        0        0     2882 2024-05-06 01:08:19.532065 authentik_client-2024.4.1.post1714957688/authentik_client/models/log_event.py
--rw-r--r--   0        0        0      843 2024-05-06 01:08:19.532065 authentik_client-2024.4.1.post1714957688/authentik_client/models/log_level_enum.py
--rw-r--r--   0        0        0     6520 2024-05-06 01:08:19.540065 authentik_client-2024.4.1.post1714957688/authentik_client/models/login_challenge_types.py
--rw-r--r--   0        0        0     4171 2024-05-06 01:08:19.544065 authentik_client-2024.4.1.post1714957688/authentik_client/models/login_metrics.py
--rw-r--r--   0        0        0     3192 2024-05-06 01:08:19.544065 authentik_client-2024.4.1.post1714957688/authentik_client/models/login_source.py
--rw-r--r--   0        0        0     2513 2024-05-06 01:08:19.552065 authentik_client-2024.4.1.post1714957688/authentik_client/models/metadata.py
--rw-r--r--   0        0        0     7604 2024-05-06 01:08:19.552065 authentik_client-2024.4.1.post1714957688/authentik_client/models/model_enum.py
--rw-r--r--   0        0        0     9828 2024-05-06 01:08:19.556065 authentik_client-2024.4.1.post1714957688/authentik_client/models/model_request.py
--rw-r--r--   0        0        0     1559 2024-05-06 01:08:19.560065 authentik_client-2024.4.1.post1714957688/authentik_client/models/name_id_policy_enum.py
--rw-r--r--   0        0        0      831 2024-05-06 01:08:19.564065 authentik_client-2024.4.1.post1714957688/authentik_client/models/network_binding_enum.py
--rw-r--r--   0        0        0      764 2024-05-06 01:08:19.568065 authentik_client-2024.4.1.post1714957688/authentik_client/models/not_configured_action_enum.py
--rw-r--r--   0        0        0     3479 2024-05-06 01:08:19.572065 authentik_client-2024.4.1.post1714957688/authentik_client/models/notification.py
--rw-r--r--   0        0        0     2858 2024-05-06 01:08:19.576065 authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_request.py
--rw-r--r--   0        0        0     4010 2024-05-06 01:08:19.580065 authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_rule.py
--rw-r--r--   0        0        0     3549 2024-05-06 01:08:19.584065 authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_rule_request.py
--rw-r--r--   0        0        0     3760 2024-05-06 01:08:19.584065 authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_transport.py
--rw-r--r--   0        0        0      818 2024-05-06 01:08:19.588065 authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_transport_mode_enum.py
--rw-r--r--   0        0        0     3500 2024-05-06 01:08:19.592065 authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_transport_request.py
--rw-r--r--   0        0        0     2503 2024-05-06 01:08:19.596065 authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_transport_test.py
--rw-r--r--   0        0        0     2707 2024-05-06 01:08:19.600065 authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_webhook_mapping.py
--rw-r--r--   0        0        0     2717 2024-05-06 01:08:19.600065 authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     8888 2024-05-06 01:08:19.604065 authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth2_provider.py
--rw-r--r--   0        0        0     6654 2024-05-06 01:08:19.608065 authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth2_provider_request.py
--rw-r--r--   0        0        0     3482 2024-05-06 01:08:19.612065 authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth2_provider_setup_urls.py
--rw-r--r--   0        0        0     4164 2024-05-06 01:08:19.616065 authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth_device_code_challenge.py
--rw-r--r--   0        0        0     2846 2024-05-06 01:08:19.620066 authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth_device_code_challenge_response_request.py
--rw-r--r--   0        0        0     4213 2024-05-06 01:08:19.624065 authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth_device_code_finish_challenge.py
--rw-r--r--   0        0        0     2816 2024-05-06 01:08:19.628065 authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
--rw-r--r--   0        0        0    10563 2024-05-06 01:08:19.632066 authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth_source.py
--rw-r--r--   0        0        0     8013 2024-05-06 01:08:19.636066 authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth_source_request.py
--rw-r--r--   0        0        0     3922 2024-05-06 01:08:19.640066 authentik_client-2024.4.1.post1714957688/authentik_client/models/open_id_connect_configuration.py
--rw-r--r--   0        0        0     5545 2024-05-06 01:08:19.644066 authentik_client-2024.4.1.post1714957688/authentik_client/models/outpost.py
--rw-r--r--   0        0        0     2541 2024-05-06 01:08:19.648066 authentik_client-2024.4.1.post1714957688/authentik_client/models/outpost_default_config.py
--rw-r--r--   0        0        0     3755 2024-05-06 01:08:19.652066 authentik_client-2024.4.1.post1714957688/authentik_client/models/outpost_health.py
--rw-r--r--   0        0        0     4050 2024-05-06 01:08:19.656066 authentik_client-2024.4.1.post1714957688/authentik_client/models/outpost_request.py
--rw-r--r--   0        0        0      752 2024-05-06 01:08:19.660066 authentik_client-2024.4.1.post1714957688/authentik_client/models/outpost_type_enum.py
--rw-r--r--   0        0        0     3322 2024-05-06 01:08:19.664066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_application_list.py
--rw-r--r--   0        0        0     3395 2024-05-06 01:08:19.664066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticated_session_list.py
--rw-r--r--   0        0        0     3404 2024-05-06 01:08:19.668066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticator_duo_stage_list.py
--rw-r--r--   0        0        0     3404 2024-05-06 01:08:19.672066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticator_sms_stage_list.py
--rw-r--r--   0        0        0     3428 2024-05-06 01:08:19.676066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticator_static_stage_list.py
--rw-r--r--   0        0        0     3412 2024-05-06 01:08:19.680066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticator_totp_stage_list.py
--rw-r--r--   0        0        0     3444 2024-05-06 01:08:19.684066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticator_validate_stage_list.py
--rw-r--r--   0        0        0     3445 2024-05-06 01:08:19.688066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
--rw-r--r--   0        0        0     3371 2024-05-06 01:08:19.692066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_blueprint_instance_list.py
--rw-r--r--   0        0        0     3274 2024-05-06 01:08:19.696066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_brand_list.py
--rw-r--r--   0        0        0     3331 2024-05-06 01:08:19.700066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_captcha_stage_list.py
--rw-r--r--   0        0        0     3380 2024-05-06 01:08:19.700066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_certificate_key_pair_list.py
--rw-r--r--   0        0        0     3355 2024-05-06 01:08:19.704066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_connection_token_list.py
--rw-r--r--   0        0        0     3331 2024-05-06 01:08:19.708066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_consent_stage_list.py
--rw-r--r--   0        0        0     3307 2024-05-06 01:08:19.712066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_deny_stage_list.py
--rw-r--r--   0        0        0     3420 2024-05-06 01:08:19.716066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_docker_service_connection_list.py
--rw-r--r--   0        0        0     3282 2024-05-06 01:08:19.720066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_domain_list.py
--rw-r--r--   0        0        0     3323 2024-05-06 01:08:19.724066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_dummy_policy_list.py
--rw-r--r--   0        0        0     3315 2024-05-06 01:08:19.728067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_dummy_stage_list.py
--rw-r--r--   0        0        0     3307 2024-05-06 01:08:19.732066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_duo_device_list.py
--rw-r--r--   0        0        0     3315 2024-05-06 01:08:19.732066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_email_stage_list.py
--rw-r--r--   0        0        0     3298 2024-05-06 01:08:19.736066 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_endpoint_list.py
--rw-r--r--   0        0        0     3274 2024-05-06 01:08:19.740067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_event_list.py
--rw-r--r--   0        0        0     3380 2024-05-06 01:08:19.744067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_event_matcher_policy_list.py
--rw-r--r--   0        0        0     3413 2024-05-06 01:08:19.748067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_expiring_base_grant_model_list.py
--rw-r--r--   0        0        0     3363 2024-05-06 01:08:19.752067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_expression_policy_list.py
--rw-r--r--   0        0        0     3437 2024-05-06 01:08:19.756067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_extra_role_object_permission_list.py
--rw-r--r--   0        0        0     3437 2024-05-06 01:08:19.760067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_extra_user_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-05-06 01:08:19.764067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_flow_list.py
--rw-r--r--   0        0        0     3364 2024-05-06 01:08:19.764067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_flow_stage_binding_list.py
--rw-r--r--   0        0        0     3274 2024-05-06 01:08:19.768067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_group_list.py
--rw-r--r--   0        0        0     3387 2024-05-06 01:08:19.772067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_identification_stage_list.py
--rw-r--r--   0        0        0     3314 2024-05-06 01:08:19.776067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_invitation_list.py
--rw-r--r--   0        0        0     3355 2024-05-06 01:08:19.780067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_invitation_stage_list.py
--rw-r--r--   0        0        0     3452 2024-05-06 01:08:19.784067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_kubernetes_service_connection_list.py
--rw-r--r--   0        0        0     3372 2024-05-06 01:08:19.788067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_ldap_outpost_config_list.py
--rw-r--r--   0        0        0     3388 2024-05-06 01:08:19.792067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_ldap_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-05-06 01:08:19.796067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_ldap_provider_list.py
--rw-r--r--   0        0        0     3315 2024-05-06 01:08:19.800067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_ldap_source_list.py
--rw-r--r--   0        0        0     3290 2024-05-06 01:08:19.804067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_license_list.py
--rw-r--r--   0        0        0     3330 2024-05-06 01:08:19.808067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_notification_list.py
--rw-r--r--   0        0        0     3363 2024-05-06 01:08:19.812067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_notification_rule_list.py
--rw-r--r--   0        0        0     3403 2024-05-06 01:08:19.812067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_notification_transport_list.py
--rw-r--r--   0        0        0     3444 2024-05-06 01:08:19.816067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_notification_webhook_mapping_list.py
--rw-r--r--   0        0        0     3348 2024-05-06 01:08:19.820067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_o_auth2_provider_list.py
--rw-r--r--   0        0        0     3324 2024-05-06 01:08:19.824067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_o_auth_source_list.py
--rw-r--r--   0        0        0     3290 2024-05-06 01:08:19.828067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_outpost_list.py
--rw-r--r--   0        0        0     3396 2024-05-06 01:08:19.832067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_password_expiry_policy_list.py
--rw-r--r--   0        0        0     3347 2024-05-06 01:08:19.836068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_password_policy_list.py
--rw-r--r--   0        0        0     3339 2024-05-06 01:08:19.840067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_password_stage_list.py
--rw-r--r--   0        0        0     3314 2024-05-06 01:08:19.844067 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_permission_list.py
--rw-r--r--   0        0        0     3396 2024-05-06 01:08:19.848068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_plex_source_connection_list.py
--rw-r--r--   0        0        0     3315 2024-05-06 01:08:19.848068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_plex_source_list.py
--rw-r--r--   0        0        0     3339 2024-05-06 01:08:19.852068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_policy_binding_list.py
--rw-r--r--   0        0        0     3282 2024-05-06 01:08:19.856068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_policy_list.py
--rw-r--r--   0        0        0     3282 2024-05-06 01:08:19.864068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_prompt_list.py
--rw-r--r--   0        0        0     3323 2024-05-06 01:08:19.868068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_prompt_stage_list.py
--rw-r--r--   0        0        0     3355 2024-05-06 01:08:19.872068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_property_mapping_list.py
--rw-r--r--   0        0        0     3298 2024-05-06 01:08:19.876068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_provider_list.py
--rw-r--r--   0        0        0     3380 2024-05-06 01:08:19.876068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_proxy_outpost_config_list.py
--rw-r--r--   0        0        0     3339 2024-05-06 01:08:19.880068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_proxy_provider_list.py
--rw-r--r--   0        0        0     3380 2024-05-06 01:08:19.884068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_rac_property_mapping_list.py
--rw-r--r--   0        0        0     3323 2024-05-06 01:08:19.888068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_rac_provider_list.py
--rw-r--r--   0        0        0     3388 2024-05-06 01:08:19.892068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_radius_outpost_config_list.py
--rw-r--r--   0        0        0     3347 2024-05-06 01:08:19.896068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_radius_provider_list.py
--rw-r--r--   0        0        0     3314 2024-05-06 01:08:19.900068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_reputation_list.py
--rw-r--r--   0        0        0     3363 2024-05-06 01:08:19.900068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_reputation_policy_list.py
--rw-r--r--   0        0        0     3461 2024-05-06 01:08:19.904068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_role_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3266 2024-05-06 01:08:19.908068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_role_list.py
--rw-r--r--   0        0        0     3388 2024-05-06 01:08:19.912068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_saml_property_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-05-06 01:08:19.916068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_saml_provider_list.py
--rw-r--r--   0        0        0     3315 2024-05-06 01:08:19.916068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_saml_source_list.py
--rw-r--r--   0        0        0     3323 2024-05-06 01:08:19.920068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_scim_mapping_list.py
--rw-r--r--   0        0        0     3331 2024-05-06 01:08:19.924068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_scim_provider_list.py
--rw-r--r--   0        0        0     3356 2024-05-06 01:08:19.924068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_scim_source_group_list.py
--rw-r--r--   0        0        0     3315 2024-05-06 01:08:19.928068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_scim_source_list.py
--rw-r--r--   0        0        0     3348 2024-05-06 01:08:19.932068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_scim_source_user_list.py
--rw-r--r--   0        0        0     3331 2024-05-06 01:08:19.936068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_scope_mapping_list.py
--rw-r--r--   0        0        0     3371 2024-05-06 01:08:19.940068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_service_connection_list.py
--rw-r--r--   0        0        0     3307 2024-05-06 01:08:19.932068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_sms_device_list.py
--rw-r--r--   0        0        0     3282 2024-05-06 01:08:19.940068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_source_list.py
--rw-r--r--   0        0        0     3323 2024-05-06 01:08:19.944069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_source_stage_list.py
--rw-r--r--   0        0        0     3274 2024-05-06 01:08:19.948068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_stage_list.py
--rw-r--r--   0        0        0     3331 2024-05-06 01:08:19.952068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_static_device_list.py
--rw-r--r--   0        0        0     3315 2024-05-06 01:08:19.952068 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_system_task_list.py
--rw-r--r--   0        0        0     3282 2024-05-06 01:08:19.960069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_tenant_list.py
--rw-r--r--   0        0        0     3274 2024-05-06 01:08:19.960069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_token_list.py
--rw-r--r--   0        0        0     3315 2024-05-06 01:08:19.964069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_token_model_list.py
--rw-r--r--   0        0        0     3315 2024-05-06 01:08:19.956069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_totp_device_list.py
--rw-r--r--   0        0        0     3461 2024-05-06 01:08:19.968069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_assigned_object_permission_list.py
--rw-r--r--   0        0        0     3323 2024-05-06 01:08:19.968069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_consent_list.py
--rw-r--r--   0        0        0     3356 2024-05-06 01:08:19.972069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_delete_stage_list.py
--rw-r--r--   0        0        0     3266 2024-05-06 01:08:19.976069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_list.py
--rw-r--r--   0        0        0     3348 2024-05-06 01:08:19.976069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_login_stage_list.py
--rw-r--r--   0        0        0     3356 2024-05-06 01:08:19.980069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_logout_stage_list.py
--rw-r--r--   0        0        0     3438 2024-05-06 01:08:19.984069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_o_auth_source_connection_list.py
--rw-r--r--   0        0        0     3429 2024-05-06 01:08:19.984069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_saml_source_connection_list.py
--rw-r--r--   0        0        0     3396 2024-05-06 01:08:19.988069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_source_connection_list.py
--rw-r--r--   0        0        0     3348 2024-05-06 01:08:19.992069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_write_stage_list.py
--rw-r--r--   0        0        0     3348 2024-05-06 01:08:19.992069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_web_authn_device_list.py
--rw-r--r--   0        0        0     3381 2024-05-06 01:08:19.996069 authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_web_authn_device_type_list.py
--rw-r--r--   0        0        0     3076 2024-05-06 01:08:20.000069 authentik_client-2024.4.1.post1714957688/authentik_client/models/pagination.py
--rw-r--r--   0        0        0     4454 2024-05-06 01:08:20.000069 authentik_client-2024.4.1.post1714957688/authentik_client/models/password_challenge.py
--rw-r--r--   0        0        0     2819 2024-05-06 01:08:20.004069 authentik_client-2024.4.1.post1714957688/authentik_client/models/password_challenge_response_request.py
--rw-r--r--   0        0        0     4377 2024-05-06 01:08:20.008069 authentik_client-2024.4.1.post1714957688/authentik_client/models/password_expiry_policy.py
--rw-r--r--   0        0        0     3099 2024-05-06 01:08:20.008069 authentik_client-2024.4.1.post1714957688/authentik_client/models/password_expiry_policy_request.py
--rw-r--r--   0        0        0     6428 2024-05-06 01:08:20.012069 authentik_client-2024.4.1.post1714957688/authentik_client/models/password_policy.py
--rw-r--r--   0        0        0     5239 2024-05-06 01:08:20.016069 authentik_client-2024.4.1.post1714957688/authentik_client/models/password_policy_request.py
--rw-r--r--   0        0        0     5274 2024-05-06 01:08:20.020069 authentik_client-2024.4.1.post1714957688/authentik_client/models/password_stage.py
--rw-r--r--   0        0        0     4264 2024-05-06 01:08:20.024069 authentik_client-2024.4.1.post1714957688/authentik_client/models/password_stage_request.py
--rw-r--r--   0        0        0     4594 2024-05-06 01:08:20.028069 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_application_request.py
--rw-r--r--   0        0        0     4833 2024-05-06 01:08:20.032069 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_authenticator_duo_stage_request.py
--rw-r--r--   0        0        0     5701 2024-05-06 01:08:20.032069 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_authenticator_sms_stage_request.py
--rw-r--r--   0        0        0     4430 2024-05-06 01:08:20.036069 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_authenticator_static_stage_request.py
--rw-r--r--   0        0        0     4256 2024-05-06 01:08:20.040069 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_authenticator_totp_stage_request.py
--rw-r--r--   0        0        0     4931 2024-05-06 01:08:20.044069 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_authenticator_validate_stage_request.py
--rw-r--r--   0        0        0     5340 2024-05-06 01:08:20.048069 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_authenticator_web_authn_stage_request.py
--rw-r--r--   0        0        0     3246 2024-05-06 01:08:20.052070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_blueprint_instance_request.py
--rw-r--r--   0        0        0     6352 2024-05-06 01:08:20.056069 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_brand_request.py
--rw-r--r--   0        0        0     3860 2024-05-06 01:08:20.060070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_captcha_stage_request.py
--rw-r--r--   0        0        0     3051 2024-05-06 01:08:20.060070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_certificate_key_pair_request.py
--rw-r--r--   0        0        0     2717 2024-05-06 01:08:20.064070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_connection_token_request.py
--rw-r--r--   0        0        0     3607 2024-05-06 01:08:20.068070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_consent_stage_request.py
--rw-r--r--   0        0        0     3268 2024-05-06 01:08:20.072070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_deny_stage_request.py
--rw-r--r--   0        0        0     4149 2024-05-06 01:08:20.076070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_docker_service_connection_request.py
--rw-r--r--   0        0        0     2801 2024-05-06 01:08:20.076070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_domain_request.py
--rw-r--r--   0        0        0     3275 2024-05-06 01:08:20.080070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_dummy_policy_request.py
--rw-r--r--   0        0        0     3270 2024-05-06 01:08:20.084070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_dummy_stage_request.py
--rw-r--r--   0        0        0     2674 2024-05-06 01:08:20.088070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_duo_device_request.py
--rw-r--r--   0        0        0     5159 2024-05-06 01:08:20.092070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_email_stage_request.py
--rw-r--r--   0        0        0     3784 2024-05-06 01:08:20.096070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_endpoint_request.py
--rw-r--r--   0        0        0     4845 2024-05-06 01:08:20.100070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_event_matcher_policy_request.py
--rw-r--r--   0        0        0     4045 2024-05-06 01:08:20.104070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_event_request.py
--rw-r--r--   0        0        0     3047 2024-05-06 01:08:20.108070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_expression_policy_request.py
--rw-r--r--   0        0        0     4903 2024-05-06 01:08:20.112070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_flow_request.py
--rw-r--r--   0        0        0     4055 2024-05-06 01:08:20.116070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_flow_stage_binding_request.py
--rw-r--r--   0        0        0     3385 2024-05-06 01:08:20.120070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_group_request.py
--rw-r--r--   0        0        0     6571 2024-05-06 01:08:20.124070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_identification_stage_request.py
--rw-r--r--   0        0        0     3985 2024-05-06 01:08:20.124070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_invitation_request.py
--rw-r--r--   0        0        0     3565 2024-05-06 01:08:20.128070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_invitation_stage_request.py
--rw-r--r--   0        0        0     3492 2024-05-06 01:08:20.132070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_kubernetes_service_connection_request.py
--rw-r--r--   0        0        0     3550 2024-05-06 01:08:20.136070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_ldap_property_mapping_request.py
--rw-r--r--   0        0        0     6254 2024-05-06 01:08:20.136070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_ldap_provider_request.py
--rw-r--r--   0        0        0     9697 2024-05-06 01:08:20.140070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_ldap_source_request.py
--rw-r--r--   0        0        0     2557 2024-05-06 01:08:20.144070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_license_request.py
--rw-r--r--   0        0        0     2879 2024-05-06 01:08:20.144070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_notification_request.py
--rw-r--r--   0        0        0     3587 2024-05-06 01:08:20.148070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_notification_rule_request.py
--rw-r--r--   0        0        0     3538 2024-05-06 01:08:20.152070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_notification_transport_request.py
--rw-r--r--   0        0        0     2782 2024-05-06 01:08:20.156070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_notification_webhook_mapping_request.py
--rw-r--r--   0        0        0     6716 2024-05-06 01:08:20.160071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_o_auth2_provider_request.py
--rw-r--r--   0        0        0     8185 2024-05-06 01:08:20.160071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_o_auth_source_request.py
--rw-r--r--   0        0        0     4139 2024-05-06 01:08:20.164070 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_outpost_request.py
--rw-r--r--   0        0        0     3154 2024-05-06 01:08:20.168071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_password_expiry_policy_request.py
--rw-r--r--   0        0        0     5277 2024-05-06 01:08:20.172071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_password_policy_request.py
--rw-r--r--   0        0        0     4326 2024-05-06 01:08:20.176071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_password_stage_request.py
--rw-r--r--   0        0        0     2922 2024-05-06 01:08:20.180071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_permission_assign_request.py
--rw-r--r--   0        0        0     2784 2024-05-06 01:08:20.184071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_plex_source_connection_request.py
--rw-r--r--   0        0        0     5905 2024-05-06 01:08:20.188071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_plex_source_request.py
--rw-r--r--   0        0        0     4286 2024-05-06 01:08:20.192071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_policy_binding_request.py
--rw-r--r--   0        0        0     5023 2024-05-06 01:08:20.196071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_prompt_request.py
--rw-r--r--   0        0        0     3406 2024-05-06 01:08:20.200071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_prompt_stage_request.py
--rw-r--r--   0        0        0     6907 2024-05-06 01:08:20.204071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_proxy_provider_request.py
--rw-r--r--   0        0        0     3495 2024-05-06 01:08:20.208071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_rac_property_mapping_request.py
--rw-r--r--   0        0        0     4413 2024-05-06 01:08:20.208071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_rac_provider_request.py
--rw-r--r--   0        0        0     4563 2024-05-06 01:08:20.212071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_radius_provider_request.py
--rw-r--r--   0        0        0     3276 2024-05-06 01:08:20.212071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_reputation_policy_request.py
--rw-r--r--   0        0        0     2565 2024-05-06 01:08:20.216071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_role_request.py
--rw-r--r--   0        0        0     3901 2024-05-06 01:08:20.220071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_saml_property_mapping_request.py
--rw-r--r--   0        0        0     7539 2024-05-06 01:08:20.224071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_saml_provider_request.py
--rw-r--r--   0        0        0     8676 2024-05-06 01:08:20.228071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_saml_source_request.py
--rw-r--r--   0        0        0     3364 2024-05-06 01:08:20.232071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_scim_mapping_request.py
--rw-r--r--   0        0        0     3888 2024-05-06 01:08:20.232071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_scim_provider_request.py
--rw-r--r--   0        0        0     3095 2024-05-06 01:08:20.236071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_scim_source_group_request.py
--rw-r--r--   0        0        0     3829 2024-05-06 01:08:20.240071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_scim_source_request.py
--rw-r--r--   0        0        0     3098 2024-05-06 01:08:20.244071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_scim_source_user_request.py
--rw-r--r--   0        0        0     3819 2024-05-06 01:08:20.248071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_scope_mapping_request.py
--rw-r--r--   0        0        0     5079 2024-05-06 01:08:20.252071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_settings_request.py
--rw-r--r--   0        0        0     2674 2024-05-06 01:08:20.244071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_sms_device_request.py
--rw-r--r--   0        0        0     3562 2024-05-06 01:08:20.256071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_source_stage_request.py
--rw-r--r--   0        0        0     2686 2024-05-06 01:08:20.256071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_static_device_request.py
--rw-r--r--   0        0        0     2820 2024-05-06 01:08:20.264071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_tenant_request.py
--rw-r--r--   0        0        0     4419 2024-05-06 01:08:20.268072 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_token_request.py
--rw-r--r--   0        0        0     2678 2024-05-06 01:08:20.260071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_totp_device_request.py
--rw-r--r--   0        0        0     3167 2024-05-06 01:08:20.268072 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_delete_stage_request.py
--rw-r--r--   0        0        0     4766 2024-05-06 01:08:20.272071 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_login_stage_request.py
--rw-r--r--   0        0        0     3167 2024-05-06 01:08:20.276072 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_logout_stage_request.py
--rw-r--r--   0        0        0     3109 2024-05-06 01:08:20.280072 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3934 2024-05-06 01:08:20.284072 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_request.py
--rw-r--r--   0        0        0     2733 2024-05-06 01:08:20.284072 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_saml_source_connection_request.py
--rw-r--r--   0        0        0     4450 2024-05-06 01:08:20.288072 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_write_stage_request.py
--rw-r--r--   0        0        0     2625 2024-05-06 01:08:20.292072 authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_web_authn_device_request.py
--rw-r--r--   0        0        0     3548 2024-05-06 01:08:20.292072 authentik_client-2024.4.1.post1714957688/authentik_client/models/permission.py
--rw-r--r--   0        0        0     2884 2024-05-06 01:08:20.296072 authentik_client-2024.4.1.post1714957688/authentik_client/models/permission_assign_request.py
--rw-r--r--   0        0        0     4315 2024-05-06 01:08:20.300072 authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_authentication_challenge.py
--rw-r--r--   0        0        0     2726 2024-05-06 01:08:20.304072 authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_authentication_challenge_response_request.py
--rw-r--r--   0        0        0     7752 2024-05-06 01:08:20.308072 authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_source.py
--rw-r--r--   0        0        0     3265 2024-05-06 01:08:20.312072 authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_source_connection.py
--rw-r--r--   0        0        0     2719 2024-05-06 01:08:20.316072 authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_source_connection_request.py
--rw-r--r--   0        0        0     5760 2024-05-06 01:08:20.320072 authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_source_request.py
--rw-r--r--   0        0        0     2576 2024-05-06 01:08:20.320072 authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_token_redeem_request.py
--rw-r--r--   0        0        0     4055 2024-05-06 01:08:20.324072 authentik_client-2024.4.1.post1714957688/authentik_client/models/policy.py
--rw-r--r--   0        0        0     5643 2024-05-06 01:08:20.324072 authentik_client-2024.4.1.post1714957688/authentik_client/models/policy_binding.py
--rw-r--r--   0        0        0     4231 2024-05-06 01:08:20.328072 authentik_client-2024.4.1.post1714957688/authentik_client/models/policy_binding_request.py
--rw-r--r--   0        0        0      711 2024-05-06 01:08:20.328072 authentik_client-2024.4.1.post1714957688/authentik_client/models/policy_engine_mode.py
--rw-r--r--   0        0        0     2817 2024-05-06 01:08:20.332072 authentik_client-2024.4.1.post1714957688/authentik_client/models/policy_request.py
--rw-r--r--   0        0        0     2583 2024-05-06 01:08:20.332072 authentik_client-2024.4.1.post1714957688/authentik_client/models/policy_test_request.py
--rw-r--r--   0        0        0     3281 2024-05-06 01:08:20.336072 authentik_client-2024.4.1.post1714957688/authentik_client/models/policy_test_result.py
--rw-r--r--   0        0        0     4885 2024-05-06 01:08:20.336072 authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt.py
--rw-r--r--   0        0        0     4649 2024-05-06 01:08:20.340072 authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt_challenge.py
--rw-r--r--   0        0        0     3325 2024-05-06 01:08:20.344072 authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt_challenge_response_request.py
--rw-r--r--   0        0        0     4927 2024-05-06 01:08:20.348072 authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt_request.py
--rw-r--r--   0        0        0     4321 2024-05-06 01:08:20.352072 authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt_stage.py
--rw-r--r--   0        0        0     3351 2024-05-06 01:08:20.352072 authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt_stage_request.py
--rw-r--r--   0        0        0     1185 2024-05-06 01:08:20.356072 authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt_type_enum.py
--rw-r--r--   0        0        0     4264 2024-05-06 01:08:20.356072 authentik_client-2024.4.1.post1714957688/authentik_client/models/property_mapping.py
--rw-r--r--   0        0        0     2610 2024-05-06 01:08:20.360072 authentik_client-2024.4.1.post1714957688/authentik_client/models/property_mapping_preview.py
--rw-r--r--   0        0        0     2744 2024-05-06 01:08:20.364072 authentik_client-2024.4.1.post1714957688/authentik_client/models/property_mapping_test_result.py
--rw-r--r--   0        0        0      715 2024-05-06 01:08:20.364072 authentik_client-2024.4.1.post1714957688/authentik_client/models/protocol_enum.py
--rw-r--r--   0        0        0     5722 2024-05-06 01:08:20.368072 authentik_client-2024.4.1.post1714957688/authentik_client/models/provider.py
--rw-r--r--   0        0        0      713 2024-05-06 01:08:20.368072 authentik_client-2024.4.1.post1714957688/authentik_client/models/provider_enum.py
--rw-r--r--   0        0        0     1314 2024-05-06 01:08:20.368072 authentik_client-2024.4.1.post1714957688/authentik_client/models/provider_model_enum.py
--rw-r--r--   0        0        0     3397 2024-05-06 01:08:20.372073 authentik_client-2024.4.1.post1714957688/authentik_client/models/provider_request.py
--rw-r--r--   0        0        0     1009 2024-05-06 01:08:20.372073 authentik_client-2024.4.1.post1714957688/authentik_client/models/provider_type_enum.py
--rw-r--r--   0        0        0      754 2024-05-06 01:08:20.376073 authentik_client-2024.4.1.post1714957688/authentik_client/models/proxy_mode.py
--rw-r--r--   0        0        0     7819 2024-05-06 01:08:20.376073 authentik_client-2024.4.1.post1714957688/authentik_client/models/proxy_outpost_config.py
--rw-r--r--   0        0        0     9552 2024-05-06 01:08:20.380072 authentik_client-2024.4.1.post1714957688/authentik_client/models/proxy_provider.py
--rw-r--r--   0        0        0     6828 2024-05-06 01:08:20.384073 authentik_client-2024.4.1.post1714957688/authentik_client/models/proxy_provider_request.py
--rw-r--r--   0        0        0     4407 2024-05-06 01:08:20.384073 authentik_client-2024.4.1.post1714957688/authentik_client/models/rac_property_mapping.py
--rw-r--r--   0        0        0     3440 2024-05-06 01:08:20.388073 authentik_client-2024.4.1.post1714957688/authentik_client/models/rac_property_mapping_request.py
--rw-r--r--   0        0        0     6813 2024-05-06 01:08:20.392073 authentik_client-2024.4.1.post1714957688/authentik_client/models/rac_provider.py
--rw-r--r--   0        0        0     4351 2024-05-06 01:08:20.392073 authentik_client-2024.4.1.post1714957688/authentik_client/models/rac_provider_request.py
--rw-r--r--   0        0        0     3833 2024-05-06 01:08:20.396073 authentik_client-2024.4.1.post1714957688/authentik_client/models/radius_outpost_config.py
--rw-r--r--   0        0        0     6924 2024-05-06 01:08:20.400073 authentik_client-2024.4.1.post1714957688/authentik_client/models/radius_provider.py
--rw-r--r--   0        0        0     4501 2024-05-06 01:08:20.400073 authentik_client-2024.4.1.post1714957688/authentik_client/models/radius_provider_request.py
--rw-r--r--   0        0        0     4184 2024-05-06 01:08:20.404073 authentik_client-2024.4.1.post1714957688/authentik_client/models/redirect_challenge.py
--rw-r--r--   0        0        0     3642 2024-05-06 01:08:20.408073 authentik_client-2024.4.1.post1714957688/authentik_client/models/reputation.py
--rw-r--r--   0        0        0     4516 2024-05-06 01:08:20.408073 authentik_client-2024.4.1.post1714957688/authentik_client/models/reputation_policy.py
--rw-r--r--   0        0        0     3238 2024-05-06 01:08:20.412073 authentik_client-2024.4.1.post1714957688/authentik_client/models/reputation_policy_request.py
--rw-r--r--   0        0        0      795 2024-05-06 01:08:20.412073 authentik_client-2024.4.1.post1714957688/authentik_client/models/resident_key_requirement_enum.py
--rw-r--r--   0        0        0     2618 2024-05-06 01:08:20.416073 authentik_client-2024.4.1.post1714957688/authentik_client/models/role.py
--rw-r--r--   0        0        0     3333 2024-05-06 01:08:20.420073 authentik_client-2024.4.1.post1714957688/authentik_client/models/role_assigned_object_permission.py
--rw-r--r--   0        0        0     3293 2024-05-06 01:08:20.420073 authentik_client-2024.4.1.post1714957688/authentik_client/models/role_object_permission.py
--rw-r--r--   0        0        0     2517 2024-05-06 01:08:20.424073 authentik_client-2024.4.1.post1714957688/authentik_client/models/role_request.py
--rw-r--r--   0        0        0     2712 2024-05-06 01:08:20.424073 authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_metadata.py
--rw-r--r--   0        0        0     4718 2024-05-06 01:08:20.428073 authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_property_mapping.py
--rw-r--r--   0        0        0     3829 2024-05-06 01:08:20.432073 authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_property_mapping_request.py
--rw-r--r--   0        0        0    11056 2024-05-06 01:08:20.432073 authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_provider.py
--rw-r--r--   0        0        0     7460 2024-05-06 01:08:20.436073 authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_provider_request.py
--rw-r--r--   0        0        0    10563 2024-05-06 01:08:20.436073 authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_source.py
--rw-r--r--   0        0        0     8507 2024-05-06 01:08:20.440073 authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_source_request.py
--rw-r--r--   0        0        0     4248 2024-05-06 01:08:20.448073 authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_mapping.py
--rw-r--r--   0        0        0     3309 2024-05-06 01:08:20.448073 authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_mapping_request.py
--rw-r--r--   0        0        0     5454 2024-05-06 01:08:20.452073 authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_provider.py
--rw-r--r--   0        0        0     3802 2024-05-06 01:08:20.452073 authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_provider_request.py
--rw-r--r--   0        0        0     5999 2024-05-06 01:08:20.456073 authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_source.py
--rw-r--r--   0        0        0     3369 2024-05-06 01:08:20.460073 authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_source_group.py
--rw-r--r--   0        0        0     3023 2024-05-06 01:08:20.460073 authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_source_group_request.py
--rw-r--r--   0        0        0     3708 2024-05-06 01:08:20.464073 authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_source_request.py
--rw-r--r--   0        0        0     3370 2024-05-06 01:08:20.468073 authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_source_user.py
--rw-r--r--   0        0        0     3026 2024-05-06 01:08:20.472073 authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_source_user_request.py
--rw-r--r--   0        0        0     3131 2024-05-06 01:08:20.472073 authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_sync_status.py
--rw-r--r--   0        0        0     4629 2024-05-06 01:08:20.484073 authentik_client-2024.4.1.post1714957688/authentik_client/models/scope_mapping.py
--rw-r--r--   0        0        0     3740 2024-05-06 01:08:20.484073 authentik_client-2024.4.1.post1714957688/authentik_client/models/scope_mapping_request.py
--rw-r--r--   0        0        0     2738 2024-05-06 01:08:20.488073 authentik_client-2024.4.1.post1714957688/authentik_client/models/selectable_stage.py
--rw-r--r--   0        0        0     3773 2024-05-06 01:08:20.492074 authentik_client-2024.4.1.post1714957688/authentik_client/models/service_connection.py
--rw-r--r--   0        0        0     2776 2024-05-06 01:08:20.492074 authentik_client-2024.4.1.post1714957688/authentik_client/models/service_connection_request.py
--rw-r--r--   0        0        0     2731 2024-05-06 01:08:20.496074 authentik_client-2024.4.1.post1714957688/authentik_client/models/service_connection_state.py
--rw-r--r--   0        0        0     3178 2024-05-06 01:08:20.500074 authentik_client-2024.4.1.post1714957688/authentik_client/models/session_user.py
--rw-r--r--   0        0        0     4931 2024-05-06 01:08:20.504074 authentik_client-2024.4.1.post1714957688/authentik_client/models/settings.py
--rw-r--r--   0        0        0     5058 2024-05-06 01:08:20.504074 authentik_client-2024.4.1.post1714957688/authentik_client/models/settings_request.py
--rw-r--r--   0        0        0      733 2024-05-06 01:08:20.508074 authentik_client-2024.4.1.post1714957688/authentik_client/models/severity_enum.py
--rw-r--r--   0        0        0     4175 2024-05-06 01:08:20.512074 authentik_client-2024.4.1.post1714957688/authentik_client/models/shell_challenge.py
--rw-r--r--   0        0        0     2172 2024-05-06 01:08:20.512074 authentik_client-2024.4.1.post1714957688/authentik_client/models/signature_algorithm_enum.py
--rw-r--r--   0        0        0     2906 2024-05-06 01:08:20.476073 authentik_client-2024.4.1.post1714957688/authentik_client/models/sms_device.py
--rw-r--r--   0        0        0     2619 2024-05-06 01:08:20.480074 authentik_client-2024.4.1.post1714957688/authentik_client/models/sms_device_request.py
--rw-r--r--   0        0        0     6945 2024-05-06 01:08:20.516074 authentik_client-2024.4.1.post1714957688/authentik_client/models/source.py
--rw-r--r--   0        0        0     4836 2024-05-06 01:08:20.520074 authentik_client-2024.4.1.post1714957688/authentik_client/models/source_request.py
--rw-r--r--   0        0        0     4438 2024-05-06 01:08:20.524074 authentik_client-2024.4.1.post1714957688/authentik_client/models/source_stage.py
--rw-r--r--   0        0        0     3507 2024-05-06 01:08:20.528074 authentik_client-2024.4.1.post1714957688/authentik_client/models/source_stage_request.py
--rw-r--r--   0        0        0     5355 2024-05-06 01:08:20.528074 authentik_client-2024.4.1.post1714957688/authentik_client/models/source_type.py
--rw-r--r--   0        0        0      714 2024-05-06 01:08:20.532074 authentik_client-2024.4.1.post1714957688/authentik_client/models/sp_binding_enum.py
--rw-r--r--   0        0        0     4070 2024-05-06 01:08:20.536074 authentik_client-2024.4.1.post1714957688/authentik_client/models/stage.py
--rw-r--r--   0        0        0     3437 2024-05-06 01:08:20.536074 authentik_client-2024.4.1.post1714957688/authentik_client/models/stage_prompt.py
--rw-r--r--   0        0        0     3089 2024-05-06 01:08:20.540074 authentik_client-2024.4.1.post1714957688/authentik_client/models/stage_request.py
--rw-r--r--   0        0        0     3385 2024-05-06 01:08:20.544074 authentik_client-2024.4.1.post1714957688/authentik_client/models/static_device.py
--rw-r--r--   0        0        0     2631 2024-05-06 01:08:20.548074 authentik_client-2024.4.1.post1714957688/authentik_client/models/static_device_request.py
--rw-r--r--   0        0        0     2546 2024-05-06 01:08:20.548074 authentik_client-2024.4.1.post1714957688/authentik_client/models/static_device_token.py
--rw-r--r--   0        0        0     2581 2024-05-06 01:08:20.552074 authentik_client-2024.4.1.post1714957688/authentik_client/models/static_device_token_request.py
--rw-r--r--   0        0        0      846 2024-05-06 01:08:20.556074 authentik_client-2024.4.1.post1714957688/authentik_client/models/sub_mode_enum.py
--rw-r--r--   0        0        0     4463 2024-05-06 01:08:20.556074 authentik_client-2024.4.1.post1714957688/authentik_client/models/system_info.py
--rw-r--r--   0        0        0     2934 2024-05-06 01:08:20.560074 authentik_client-2024.4.1.post1714957688/authentik_client/models/system_info_runtime.py
--rw-r--r--   0        0        0     4701 2024-05-06 01:08:20.564074 authentik_client-2024.4.1.post1714957688/authentik_client/models/system_task.py
--rw-r--r--   0        0        0      789 2024-05-06 01:08:20.564074 authentik_client-2024.4.1.post1714957688/authentik_client/models/system_task_status_enum.py
--rw-r--r--   0        0        0     2872 2024-05-06 01:08:20.572074 authentik_client-2024.4.1.post1714957688/authentik_client/models/tenant.py
--rw-r--r--   0        0        0     2589 2024-05-06 01:08:20.576074 authentik_client-2024.4.1.post1714957688/authentik_client/models/tenant_admin_group_request_request.py
--rw-r--r--   0        0        0     2705 2024-05-06 01:08:20.580074 authentik_client-2024.4.1.post1714957688/authentik_client/models/tenant_recovery_key_request_request.py
--rw-r--r--   0        0        0     2599 2024-05-06 01:08:20.584074 authentik_client-2024.4.1.post1714957688/authentik_client/models/tenant_recovery_key_response.py
--rw-r--r--   0        0        0     2765 2024-05-06 01:08:20.584074 authentik_client-2024.4.1.post1714957688/authentik_client/models/tenant_request.py
--rw-r--r--   0        0        0     4802 2024-05-06 01:08:20.588075 authentik_client-2024.4.1.post1714957688/authentik_client/models/token.py
--rw-r--r--   0        0        0     4198 2024-05-06 01:08:20.592074 authentik_client-2024.4.1.post1714957688/authentik_client/models/token_model.py
--rw-r--r--   0        0        0     4329 2024-05-06 01:08:20.592074 authentik_client-2024.4.1.post1714957688/authentik_client/models/token_request.py
--rw-r--r--   0        0        0     2521 2024-05-06 01:08:20.596074 authentik_client-2024.4.1.post1714957688/authentik_client/models/token_set_key_request.py
--rw-r--r--   0        0        0     2494 2024-05-06 01:08:20.600075 authentik_client-2024.4.1.post1714957688/authentik_client/models/token_view.py
--rw-r--r--   0        0        0     2724 2024-05-06 01:08:20.568074 authentik_client-2024.4.1.post1714957688/authentik_client/models/totp_device.py
--rw-r--r--   0        0        0     2623 2024-05-06 01:08:20.572074 authentik_client-2024.4.1.post1714957688/authentik_client/models/totp_device_request.py
--rw-r--r--   0        0        0     3389 2024-05-06 01:08:20.600075 authentik_client-2024.4.1.post1714957688/authentik_client/models/transaction_application_request.py
--rw-r--r--   0        0        0     2595 2024-05-06 01:08:20.604075 authentik_client-2024.4.1.post1714957688/authentik_client/models/transaction_application_response.py
--rw-r--r--   0        0        0     2936 2024-05-06 01:08:20.608075 authentik_client-2024.4.1.post1714957688/authentik_client/models/type_create.py
--rw-r--r--   0        0        0      730 2024-05-06 01:08:20.608075 authentik_client-2024.4.1.post1714957688/authentik_client/models/ui_theme_enum.py
--rw-r--r--   0        0        0     2808 2024-05-06 01:08:20.612075 authentik_client-2024.4.1.post1714957688/authentik_client/models/used_by.py
--rw-r--r--   0        0        0      795 2024-05-06 01:08:20.612075 authentik_client-2024.4.1.post1714957688/authentik_client/models/used_by_action_enum.py
--rw-r--r--   0        0        0     5459 2024-05-06 01:08:20.616075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user.py
--rw-r--r--   0        0        0     2458 2024-05-06 01:08:20.620075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_account_request.py
--rw-r--r--   0        0        0     4946 2024-05-06 01:08:20.624075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_assigned_object_permission.py
--rw-r--r--   0        0        0     3828 2024-05-06 01:08:20.628075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_consent.py
--rw-r--r--   0        0        0      811 2024-05-06 01:08:20.628075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_creation_mode_enum.py
--rw-r--r--   0        0        0     4110 2024-05-06 01:08:20.632075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_delete_stage.py
--rw-r--r--   0        0        0     3129 2024-05-06 01:08:20.636075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_delete_stage_request.py
--rw-r--r--   0        0        0      735 2024-05-06 01:08:20.636075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_fields_enum.py
--rw-r--r--   0        0        0     3909 2024-05-06 01:08:20.640075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_group.py
--rw-r--r--   0        0        0     3193 2024-05-06 01:08:20.640075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_group_request.py
--rw-r--r--   0        0        0     4334 2024-05-06 01:08:20.644075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_login_challenge.py
--rw-r--r--   0        0        0     2805 2024-05-06 01:08:20.644075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_login_challenge_response_request.py
--rw-r--r--   0        0        0     5631 2024-05-06 01:08:20.644075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_login_stage.py
--rw-r--r--   0        0        0     4728 2024-05-06 01:08:20.648075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_login_stage_request.py
--rw-r--r--   0        0        0     4110 2024-05-06 01:08:20.648075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_logout_stage.py
--rw-r--r--   0        0        0     3129 2024-05-06 01:08:20.652075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_logout_stage_request.py
--rw-r--r--   0        0        0      853 2024-05-06 01:08:20.652075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_matching_mode_enum.py
--rw-r--r--   0        0        0     4160 2024-05-06 01:08:20.656075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_metrics.py
--rw-r--r--   0        0        0     3188 2024-05-06 01:08:20.656075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_o_auth_source_connection.py
--rw-r--r--   0        0        0     3054 2024-05-06 01:08:20.660075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_o_auth_source_connection_request.py
--rw-r--r--   0        0        0     3293 2024-05-06 01:08:20.660075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_object_permission.py
--rw-r--r--   0        0        0     2557 2024-05-06 01:08:20.664075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_password_set_request.py
--rw-r--r--   0        0        0     2491 2024-05-06 01:08:20.668075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_path.py
--rw-r--r--   0        0        0     3872 2024-05-06 01:08:20.668075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_request.py
--rw-r--r--   0        0        0     3107 2024-05-06 01:08:20.672075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_saml_source_connection.py
--rw-r--r--   0        0        0     2668 2024-05-06 01:08:20.676075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_saml_source_connection_request.py
--rw-r--r--   0        0        0     5465 2024-05-06 01:08:20.676075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_self.py
--rw-r--r--   0        0        0     2629 2024-05-06 01:08:20.680075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_self_groups.py
--rw-r--r--   0        0        0     3074 2024-05-06 01:08:20.684075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_service_account_request.py
--rw-r--r--   0        0        0     2844 2024-05-06 01:08:20.684075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_service_account_response.py
--rw-r--r--   0        0        0     2866 2024-05-06 01:08:20.688075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_setting.py
--rw-r--r--   0        0        0     3245 2024-05-06 01:08:20.688075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_source_connection.py
--rw-r--r--   0        0        0      817 2024-05-06 01:08:20.692075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_type_enum.py
--rw-r--r--   0        0        0      777 2024-05-06 01:08:20.692075 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_verification_enum.py
--rw-r--r--   0        0        0     5382 2024-05-06 01:08:20.696076 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_write_stage.py
--rw-r--r--   0        0        0     4412 2024-05-06 01:08:20.696076 authentik_client-2024.4.1.post1714957688/authentik_client/models/user_write_stage_request.py
--rw-r--r--   0        0        0     3197 2024-05-06 01:08:20.700075 authentik_client-2024.4.1.post1714957688/authentik_client/models/validation_error.py
--rw-r--r--   0        0        0     3589 2024-05-06 01:08:20.704075 authentik_client-2024.4.1.post1714957688/authentik_client/models/version.py
--rw-r--r--   0        0        0     3786 2024-05-06 01:08:20.704075 authentik_client-2024.4.1.post1714957688/authentik_client/models/web_authn_device.py
--rw-r--r--   0        0        0     2577 2024-05-06 01:08:20.708076 authentik_client-2024.4.1.post1714957688/authentik_client/models/web_authn_device_request.py
--rw-r--r--   0        0        0     2562 2024-05-06 01:08:20.712076 authentik_client-2024.4.1.post1714957688/authentik_client/models/web_authn_device_type.py
--rw-r--r--   0        0        0     2669 2024-05-06 01:08:20.712076 authentik_client-2024.4.1.post1714957688/authentik_client/models/web_authn_device_type_request.py
--rw-r--r--   0        0        0     2410 2024-05-06 01:08:20.716076 authentik_client-2024.4.1.post1714957688/authentik_client/models/workers.py
--rw-r--r--   0        0        0        0 2024-05-06 01:08:21.856086 authentik_client-2024.4.1.post1714957688/authentik_client/py.typed
--rw-r--r--   0        0        0     9196 2024-05-06 01:08:21.864086 authentik_client-2024.4.1.post1714957688/authentik_client/rest.py
--rw-r--r--   0        0        0     1936 2024-05-06 01:08:21.856086 authentik_client-2024.4.1.post1714957688/pyproject.toml
--rw-r--r--   0        0        0   144925 1970-01-01 00:00:00.000000 authentik_client-2024.4.1.post1714957688/PKG-INFO
+-rw-r--r--   0        0        0   143973 2024-05-07 16:46:56.723042 authentik_client-2024.4.2.post1715100402/README.md
+-rw-r--r--   0        0        0    48535 2024-05-07 16:46:56.735042 authentik_client-2024.4.2.post1715100402/authentik_client/__init__.py
+-rw-r--r--   0        0        0     1170 2024-05-07 16:46:56.739042 authentik_client-2024.4.2.post1715100402/authentik_client/api/__init__.py
+-rw-r--r--   0        0        0    97518 2024-05-07 16:46:56.459042 authentik_client-2024.4.2.post1715100402/authentik_client/api/admin_api.py
+-rw-r--r--   0        0        0   700271 2024-05-07 16:46:56.479042 authentik_client-2024.4.2.post1715100402/authentik_client/api/authenticators_api.py
+-rw-r--r--   0        0        0   701197 2024-05-07 16:46:56.503042 authentik_client-2024.4.2.post1715100402/authentik_client/api/core_api.py
+-rw-r--r--   0        0        0   116805 2024-05-07 16:46:56.515042 authentik_client-2024.4.2.post1715100402/authentik_client/api/crypto_api.py
+-rw-r--r--   0        0        0   107946 2024-05-07 16:46:56.519042 authentik_client-2024.4.2.post1715100402/authentik_client/api/enterprise_api.py
+-rw-r--r--   0        0        0   408008 2024-05-07 16:46:56.531042 authentik_client-2024.4.2.post1715100402/authentik_client/api/events_api.py
+-rw-r--r--   0        0        0   280806 2024-05-07 16:46:56.543042 authentik_client-2024.4.2.post1715100402/authentik_client/api/flows_api.py
+-rw-r--r--   0        0        0   101134 2024-05-07 16:46:56.551042 authentik_client-2024.4.2.post1715100402/authentik_client/api/managed_api.py
+-rw-r--r--   0        0        0   135649 2024-05-07 16:46:56.555042 authentik_client-2024.4.2.post1715100402/authentik_client/api/oauth2_api.py
+-rw-r--r--   0        0        0   413301 2024-05-07 16:46:56.567042 authentik_client-2024.4.2.post1715100402/authentik_client/api/outposts_api.py
+-rw-r--r--   0        0        0   725201 2024-05-07 16:46:56.583042 authentik_client-2024.4.2.post1715100402/authentik_client/api/policies_api.py
+-rw-r--r--   0        0        0   552586 2024-05-07 16:46:56.595042 authentik_client-2024.4.2.post1715100402/authentik_client/api/propertymappings_api.py
+-rw-r--r--   0        0        0   718066 2024-05-07 16:46:56.611042 authentik_client-2024.4.2.post1715100402/authentik_client/api/providers_api.py
+-rw-r--r--   0        0        0   150485 2024-05-07 16:46:56.623042 authentik_client-2024.4.2.post1715100402/authentik_client/api/rac_api.py
+-rw-r--r--   0        0        0   207550 2024-05-07 16:46:56.627042 authentik_client-2024.4.2.post1715100402/authentik_client/api/rbac_api.py
+-rw-r--r--   0        0        0    10391 2024-05-07 16:46:56.635042 authentik_client-2024.4.2.post1715100402/authentik_client/api/root_api.py
+-rw-r--r--   0        0        0    11845 2024-05-07 16:46:56.639042 authentik_client-2024.4.2.post1715100402/authentik_client/api/schema_api.py
+-rw-r--r--   0        0        0  1037225 2024-05-07 16:46:56.655042 authentik_client-2024.4.2.post1715100402/authentik_client/api/sources_api.py
+-rw-r--r--   0        0        0  1945986 2024-05-07 16:46:56.691042 authentik_client-2024.4.2.post1715100402/authentik_client/api/stages_api.py
+-rw-r--r--   0        0        0   157909 2024-05-07 16:46:56.711042 authentik_client-2024.4.2.post1715100402/authentik_client/api/tenants_api.py
+-rw-r--r--   0        0        0    25779 2024-05-07 16:46:56.739042 authentik_client-2024.4.2.post1715100402/authentik_client/api_client.py
+-rw-r--r--   0        0        0      652 2024-05-07 16:46:56.743042 authentik_client-2024.4.2.post1715100402/authentik_client/api_response.py
+-rw-r--r--   0        0        0    14724 2024-05-07 16:46:56.731042 authentik_client-2024.4.2.post1715100402/authentik_client/configuration.py
+-rw-r--r--   0        0        0     5934 2024-05-07 16:46:56.739042 authentik_client-2024.4.2.post1715100402/authentik_client/exceptions.py
+-rw-r--r--   0        0        0    46837 2024-05-07 16:46:56.735042 authentik_client-2024.4.2.post1715100402/authentik_client/models/__init__.py
+-rw-r--r--   0        0        0     4513 2024-05-07 16:46:53.519043 authentik_client-2024.4.2.post1715100402/authentik_client/models/access_denied_challenge.py
+-rw-r--r--   0        0        0      688 2024-05-07 16:46:53.527043 authentik_client-2024.4.2.post1715100402/authentik_client/models/alg_enum.py
+-rw-r--r--   0        0        0     2482 2024-05-07 16:46:53.539043 authentik_client-2024.4.2.post1715100402/authentik_client/models/app.py
+-rw-r--r--   0        0        0     4230 2024-05-07 16:46:53.547043 authentik_client-2024.4.2.post1715100402/authentik_client/models/app_enum.py
+-rw-r--r--   0        0        0     2702 2024-05-07 16:46:53.555043 authentik_client-2024.4.2.post1715100402/authentik_client/models/apple_challenge_response_request.py
+-rw-r--r--   0        0        0     4508 2024-05-07 16:46:53.567043 authentik_client-2024.4.2.post1715100402/authentik_client/models/apple_login_challenge.py
+-rw-r--r--   0        0        0     6686 2024-05-07 16:46:53.579043 authentik_client-2024.4.2.post1715100402/authentik_client/models/application.py
+-rw-r--r--   0        0        0     4473 2024-05-07 16:46:53.587043 authentik_client-2024.4.2.post1715100402/authentik_client/models/application_request.py
+-rw-r--r--   0        0        0      711 2024-05-07 16:46:53.591043 authentik_client-2024.4.2.post1715100402/authentik_client/models/auth_mode_enum.py
+-rw-r--r--   0        0        0      709 2024-05-07 16:46:53.595043 authentik_client-2024.4.2.post1715100402/authentik_client/models/auth_type_enum.py
+-rw-r--r--   0        0        0     5195 2024-05-07 16:46:53.599043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session.py
+-rw-r--r--   0        0        0     3064 2024-05-07 16:46:53.607043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session_asn.py
+-rw-r--r--   0        0        0     2826 2024-05-07 16:46:53.615043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session_geo_ip.py
+-rw-r--r--   0        0        0     3865 2024-05-07 16:46:53.619043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session_user_agent.py
+-rw-r--r--   0        0        0     2646 2024-05-07 16:46:53.627043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session_user_agent_device.py
+-rw-r--r--   0        0        0     2792 2024-05-07 16:46:53.631043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session_user_agent_os.py
+-rw-r--r--   0        0        0     2725 2024-05-07 16:46:53.639043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session_user_agent_user_agent.py
+-rw-r--r--   0        0        0      895 2024-05-07 16:46:53.643043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authentication_enum.py
+-rw-r--r--   0        0        0      782 2024-05-07 16:46:53.643043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_attachment_enum.py
+-rw-r--r--   0        0        0     4686 2024-05-07 16:46:53.651043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_duo_challenge.py
+-rw-r--r--   0        0        0     2743 2024-05-07 16:46:53.659043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_duo_challenge_response_request.py
+-rw-r--r--   0        0        0     5327 2024-05-07 16:46:53.667043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_duo_stage.py
+-rw-r--r--   0        0        0     2768 2024-05-07 16:46:53.671043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_duo_stage_device_import_response.py
+-rw-r--r--   0        0        0     2785 2024-05-07 16:46:53.679043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py
+-rw-r--r--   0        0        0     4744 2024-05-07 16:46:53.683043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-05-07 16:46:53.691043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_sms_challenge.py
+-rw-r--r--   0        0        0     3022 2024-05-07 16:46:53.695043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_sms_challenge_response_request.py
+-rw-r--r--   0        0        0     6409 2024-05-07 16:46:53.703043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_sms_stage.py
+-rw-r--r--   0        0        0     5595 2024-05-07 16:46:53.707043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4474 2024-05-07 16:46:53.715043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_static_challenge.py
+-rw-r--r--   0        0        0     2761 2024-05-07 16:46:53.723043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_static_challenge_response_request.py
+-rw-r--r--   0        0        0     5363 2024-05-07 16:46:53.727043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_static_stage.py
+-rw-r--r--   0        0        0     4392 2024-05-07 16:46:53.735043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4468 2024-05-07 16:46:53.739043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_totp_challenge.py
+-rw-r--r--   0        0        0     2858 2024-05-07 16:46:53.743043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_totp_challenge_response_request.py
+-rw-r--r--   0        0        0     5132 2024-05-07 16:46:53.747043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_totp_stage.py
+-rw-r--r--   0        0        0     4201 2024-05-07 16:46:53.755043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     6722 2024-05-07 16:46:53.759043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_validate_stage.py
+-rw-r--r--   0        0        0     4893 2024-05-07 16:46:53.763043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5717 2024-05-07 16:46:53.771043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_validation_challenge.py
+-rw-r--r--   0        0        0     3805 2024-05-07 16:46:53.775043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_validation_challenge_response_request.py
+-rw-r--r--   0        0        0     4499 2024-05-07 16:46:53.783043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_web_authn_challenge.py
+-rw-r--r--   0        0        0     2852 2024-05-07 16:46:53.787043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_web_authn_challenge_response_request.py
+-rw-r--r--   0        0        0     7081 2024-05-07 16:46:53.791043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_web_authn_stage.py
+-rw-r--r--   0        0        0     5302 2024-05-07 16:46:53.795043 authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     2718 2024-05-07 16:46:53.799043 authentik_client-2024.4.2.post1715100402/authentik_client/models/auto_submit_challenge_response_request.py
+-rw-r--r--   0        0        0     4388 2024-05-07 16:46:53.807043 authentik_client-2024.4.2.post1715100402/authentik_client/models/autosubmit_challenge.py
+-rw-r--r--   0        0        0      950 2024-05-07 16:46:53.807043 authentik_client-2024.4.2.post1715100402/authentik_client/models/backends_enum.py
+-rw-r--r--   0        0        0      748 2024-05-07 16:46:53.811043 authentik_client-2024.4.2.post1715100402/authentik_client/models/binding_type_enum.py
+-rw-r--r--   0        0        0     2995 2024-05-07 16:46:53.815043 authentik_client-2024.4.2.post1715100402/authentik_client/models/blueprint_file.py
+-rw-r--r--   0        0        0     4453 2024-05-07 16:46:53.819043 authentik_client-2024.4.2.post1715100402/authentik_client/models/blueprint_instance.py
+-rw-r--r--   0        0        0     3208 2024-05-07 16:46:53.823043 authentik_client-2024.4.2.post1715100402/authentik_client/models/blueprint_instance_request.py
+-rw-r--r--   0        0        0      836 2024-05-07 16:46:53.827043 authentik_client-2024.4.2.post1715100402/authentik_client/models/blueprint_instance_status_enum.py
+-rw-r--r--   0        0        0     6255 2024-05-07 16:46:53.827043 authentik_client-2024.4.2.post1715100402/authentik_client/models/brand.py
+-rw-r--r--   0        0        0     6307 2024-05-07 16:46:53.831043 authentik_client-2024.4.2.post1715100402/authentik_client/models/brand_request.py
+-rw-r--r--   0        0        0     2501 2024-05-07 16:46:53.835043 authentik_client-2024.4.2.post1715100402/authentik_client/models/cache.py
+-rw-r--r--   0        0        0      875 2024-05-07 16:46:53.839043 authentik_client-2024.4.2.post1715100402/authentik_client/models/capabilities_enum.py
+-rw-r--r--   0        0        0     4476 2024-05-07 16:46:53.851043 authentik_client-2024.4.2.post1715100402/authentik_client/models/captcha_challenge.py
+-rw-r--r--   0        0        0     2797 2024-05-07 16:46:53.855043 authentik_client-2024.4.2.post1715100402/authentik_client/models/captcha_challenge_response_request.py
+-rw-r--r--   0        0        0     4438 2024-05-07 16:46:53.859043 authentik_client-2024.4.2.post1715100402/authentik_client/models/captcha_stage.py
+-rw-r--r--   0        0        0     3774 2024-05-07 16:46:53.863043 authentik_client-2024.4.2.post1715100402/authentik_client/models/captcha_stage_request.py
+-rw-r--r--   0        0        0     2522 2024-05-07 16:46:53.867043 authentik_client-2024.4.2.post1715100402/authentik_client/models/certificate_data.py
+-rw-r--r--   0        0        0     2990 2024-05-07 16:46:53.871043 authentik_client-2024.4.2.post1715100402/authentik_client/models/certificate_generation_request.py
+-rw-r--r--   0        0        0     6655 2024-05-07 16:46:53.875043 authentik_client-2024.4.2.post1715100402/authentik_client/models/certificate_key_pair.py
+-rw-r--r--   0        0        0     2989 2024-05-07 16:46:53.879043 authentik_client-2024.4.2.post1715100402/authentik_client/models/certificate_key_pair_request.py
+-rw-r--r--   0        0        0      747 2024-05-07 16:46:53.883043 authentik_client-2024.4.2.post1715100402/authentik_client/models/challenge_choices.py
+-rw-r--r--   0        0        0    24236 2024-05-07 16:46:53.891043 authentik_client-2024.4.2.post1715100402/authentik_client/models/challenge_types.py
+-rw-r--r--   0        0        0      729 2024-05-07 16:46:53.895043 authentik_client-2024.4.2.post1715100402/authentik_client/models/client_type_enum.py
+-rw-r--r--   0        0        0     3539 2024-05-07 16:46:53.899043 authentik_client-2024.4.2.post1715100402/authentik_client/models/config.py
+-rw-r--r--   0        0        0     4021 2024-05-07 16:46:53.907043 authentik_client-2024.4.2.post1715100402/authentik_client/models/connection_token.py
+-rw-r--r--   0        0        0     2662 2024-05-07 16:46:53.911043 authentik_client-2024.4.2.post1715100402/authentik_client/models/connection_token_request.py
+-rw-r--r--   0        0        0     5736 2024-05-07 16:46:53.919043 authentik_client-2024.4.2.post1715100402/authentik_client/models/consent_challenge.py
+-rw-r--r--   0        0        0     2838 2024-05-07 16:46:53.923043 authentik_client-2024.4.2.post1715100402/authentik_client/models/consent_challenge_response_request.py
+-rw-r--r--   0        0        0     2513 2024-05-07 16:46:53.927043 authentik_client-2024.4.2.post1715100402/authentik_client/models/consent_permission.py
+-rw-r--r--   0        0        0     4511 2024-05-07 16:46:53.931043 authentik_client-2024.4.2.post1715100402/authentik_client/models/consent_stage.py
+-rw-r--r--   0        0        0      783 2024-05-07 16:46:53.935043 authentik_client-2024.4.2.post1715100402/authentik_client/models/consent_stage_mode_enum.py
+-rw-r--r--   0        0        0     3569 2024-05-07 16:46:53.939043 authentik_client-2024.4.2.post1715100402/authentik_client/models/consent_stage_request.py
+-rw-r--r--   0        0        0     2891 2024-05-07 16:46:53.943043 authentik_client-2024.4.2.post1715100402/authentik_client/models/contextual_flow_info.py
+-rw-r--r--   0        0        0      879 2024-05-07 16:46:53.947043 authentik_client-2024.4.2.post1715100402/authentik_client/models/contextual_flow_info_layout_enum.py
+-rw-r--r--   0        0        0     2657 2024-05-07 16:46:53.947043 authentik_client-2024.4.2.post1715100402/authentik_client/models/coordinate.py
+-rw-r--r--   0        0        0     4704 2024-05-07 16:46:53.951043 authentik_client-2024.4.2.post1715100402/authentik_client/models/current_brand.py
+-rw-r--r--   0        0        0      771 2024-05-07 16:46:53.955043 authentik_client-2024.4.2.post1715100402/authentik_client/models/denied_action_enum.py
+-rw-r--r--   0        0        0     4200 2024-05-07 16:46:53.959043 authentik_client-2024.4.2.post1715100402/authentik_client/models/deny_stage.py
+-rw-r--r--   0        0        0     3230 2024-05-07 16:46:53.963043 authentik_client-2024.4.2.post1715100402/authentik_client/models/deny_stage_request.py
+-rw-r--r--   0        0        0     3522 2024-05-07 16:46:53.967043 authentik_client-2024.4.2.post1715100402/authentik_client/models/device.py
+-rw-r--r--   0        0        0     2657 2024-05-07 16:46:53.975043 authentik_client-2024.4.2.post1715100402/authentik_client/models/device_challenge.py
+-rw-r--r--   0        0        0     2792 2024-05-07 16:46:53.979043 authentik_client-2024.4.2.post1715100402/authentik_client/models/device_challenge_request.py
+-rw-r--r--   0        0        0      780 2024-05-07 16:46:53.979043 authentik_client-2024.4.2.post1715100402/authentik_client/models/device_classes_enum.py
+-rw-r--r--   0        0        0     1244 2024-05-07 16:46:53.983043 authentik_client-2024.4.2.post1715100402/authentik_client/models/digest_algorithm_enum.py
+-rw-r--r--   0        0        0      695 2024-05-07 16:46:53.987043 authentik_client-2024.4.2.post1715100402/authentik_client/models/digits_enum.py
+-rw-r--r--   0        0        0     4969 2024-05-07 16:46:53.987043 authentik_client-2024.4.2.post1715100402/authentik_client/models/docker_service_connection.py
+-rw-r--r--   0        0        0     4087 2024-05-07 16:46:53.995043 authentik_client-2024.4.2.post1715100402/authentik_client/models/docker_service_connection_request.py
+-rw-r--r--   0        0        0     2847 2024-05-07 16:46:53.999043 authentik_client-2024.4.2.post1715100402/authentik_client/models/domain.py
+-rw-r--r--   0        0        0     2746 2024-05-07 16:46:54.003043 authentik_client-2024.4.2.post1715100402/authentik_client/models/domain_request.py
+-rw-r--r--   0        0        0     4155 2024-05-07 16:46:54.007043 authentik_client-2024.4.2.post1715100402/authentik_client/models/dummy_challenge.py
+-rw-r--r--   0        0        0     2681 2024-05-07 16:46:54.011043 authentik_client-2024.4.2.post1715100402/authentik_client/models/dummy_challenge_response_request.py
+-rw-r--r--   0        0        0     4515 2024-05-07 16:46:54.019043 authentik_client-2024.4.2.post1715100402/authentik_client/models/dummy_policy.py
+-rw-r--r--   0        0        0     3237 2024-05-07 16:46:54.023043 authentik_client-2024.4.2.post1715100402/authentik_client/models/dummy_policy_request.py
+-rw-r--r--   0        0        0     4213 2024-05-07 16:46:54.027043 authentik_client-2024.4.2.post1715100402/authentik_client/models/dummy_stage.py
+-rw-r--r--   0        0        0     3232 2024-05-07 16:46:54.031043 authentik_client-2024.4.2.post1715100402/authentik_client/models/dummy_stage_request.py
+-rw-r--r--   0        0        0     2720 2024-05-07 16:46:54.035043 authentik_client-2024.4.2.post1715100402/authentik_client/models/duo_device.py
+-rw-r--r--   0        0        0     2575 2024-05-07 16:46:54.039043 authentik_client-2024.4.2.post1715100402/authentik_client/models/duo_device_enrollment_status.py
+-rw-r--r--   0        0        0     2619 2024-05-07 16:46:54.043043 authentik_client-2024.4.2.post1715100402/authentik_client/models/duo_device_request.py
+-rw-r--r--   0        0        0      748 2024-05-07 16:46:54.047043 authentik_client-2024.4.2.post1715100402/authentik_client/models/duo_response_enum.py
+-rw-r--r--   0        0        0     4090 2024-05-07 16:46:54.055043 authentik_client-2024.4.2.post1715100402/authentik_client/models/email_challenge.py
+-rw-r--r--   0        0        0     2770 2024-05-07 16:46:54.059043 authentik_client-2024.4.2.post1715100402/authentik_client/models/email_challenge_response_request.py
+-rw-r--r--   0        0        0     5902 2024-05-07 16:46:54.067043 authentik_client-2024.4.2.post1715100402/authentik_client/models/email_stage.py
+-rw-r--r--   0        0        0     5121 2024-05-07 16:46:54.079043 authentik_client-2024.4.2.post1715100402/authentik_client/models/email_stage_request.py
+-rw-r--r--   0        0        0     4707 2024-05-07 16:46:54.087043 authentik_client-2024.4.2.post1715100402/authentik_client/models/endpoint.py
+-rw-r--r--   0        0        0     3678 2024-05-07 16:46:54.091043 authentik_client-2024.4.2.post1715100402/authentik_client/models/endpoint_request.py
+-rw-r--r--   0        0        0     2530 2024-05-07 16:46:54.095043 authentik_client-2024.4.2.post1715100402/authentik_client/models/error_detail.py
+-rw-r--r--   0        0        0     3309 2024-05-07 16:46:54.103043 authentik_client-2024.4.2.post1715100402/authentik_client/models/error_reporting_config.py
+-rw-r--r--   0        0        0     4129 2024-05-07 16:46:54.107043 authentik_client-2024.4.2.post1715100402/authentik_client/models/event.py
+-rw-r--r--   0        0        0     1730 2024-05-07 16:46:54.111043 authentik_client-2024.4.2.post1715100402/authentik_client/models/event_actions.py
+-rw-r--r--   0        0        0     6006 2024-05-07 16:46:54.115043 authentik_client-2024.4.2.post1715100402/authentik_client/models/event_matcher_policy.py
+-rw-r--r--   0        0        0     4807 2024-05-07 16:46:54.119043 authentik_client-2024.4.2.post1715100402/authentik_client/models/event_matcher_policy_request.py
+-rw-r--r--   0        0        0     3990 2024-05-07 16:46:54.123043 authentik_client-2024.4.2.post1715100402/authentik_client/models/event_request.py
+-rw-r--r--   0        0        0     2697 2024-05-07 16:46:54.127043 authentik_client-2024.4.2.post1715100402/authentik_client/models/event_top_per_user.py
+-rw-r--r--   0        0        0     3926 2024-05-07 16:46:54.131043 authentik_client-2024.4.2.post1715100402/authentik_client/models/expiring_base_grant_model.py
+-rw-r--r--   0        0        0     4191 2024-05-07 16:46:54.139043 authentik_client-2024.4.2.post1715100402/authentik_client/models/expression_policy.py
+-rw-r--r--   0        0        0     2992 2024-05-07 16:46:54.147043 authentik_client-2024.4.2.post1715100402/authentik_client/models/expression_policy_request.py
+-rw-r--r--   0        0        0     4524 2024-05-07 16:46:54.151043 authentik_client-2024.4.2.post1715100402/authentik_client/models/extra_role_object_permission.py
+-rw-r--r--   0        0        0     4524 2024-05-07 16:46:54.155043 authentik_client-2024.4.2.post1715100402/authentik_client/models/extra_user_object_permission.py
+-rw-r--r--   0        0        0     2519 2024-05-07 16:46:54.159043 authentik_client-2024.4.2.post1715100402/authentik_client/models/file_path_request.py
+-rw-r--r--   0        0        0     6047 2024-05-07 16:46:54.167043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow.py
+-rw-r--r--   0        0        0    25850 2024-05-07 16:46:54.171043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_challenge_response_request.py
+-rw-r--r--   0        0        0      934 2024-05-07 16:46:54.175043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_designation_enum.py
+-rw-r--r--   0        0        0     2533 2024-05-07 16:46:54.179043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_diagram.py
+-rw-r--r--   0        0        0     4505 2024-05-07 16:46:54.187043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_error_challenge.py
+-rw-r--r--   0        0        0     3111 2024-05-07 16:46:54.191043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_import_result.py
+-rw-r--r--   0        0        0     3418 2024-05-07 16:46:54.195043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_inspection.py
+-rw-r--r--   0        0        0     3875 2024-05-07 16:46:54.199043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_inspector_plan.py
+-rw-r--r--   0        0        0      837 2024-05-07 16:46:54.203043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_layout_enum.py
+-rw-r--r--   0        0        0     4741 2024-05-07 16:46:54.211043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_request.py
+-rw-r--r--   0        0        0     5223 2024-05-07 16:46:54.215043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_set.py
+-rw-r--r--   0        0        0     4459 2024-05-07 16:46:54.219043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_set_request.py
+-rw-r--r--   0        0        0     4763 2024-05-07 16:46:54.223043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_stage_binding.py
+-rw-r--r--   0        0        0     3983 2024-05-07 16:46:54.231043 authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_stage_binding_request.py
+-rw-r--r--   0        0        0     2641 2024-05-07 16:46:54.235043 authentik_client-2024.4.2.post1715100402/authentik_client/models/footer_link.py
+-rw-r--r--   0        0        0     2531 2024-05-07 16:46:54.239043 authentik_client-2024.4.2.post1715100402/authentik_client/models/generic_error.py
+-rw-r--r--   0        0        0      865 2024-05-07 16:46:54.243043 authentik_client-2024.4.2.post1715100402/authentik_client/models/geoip_binding_enum.py
+-rw-r--r--   0        0        0     5445 2024-05-07 16:46:54.251043 authentik_client-2024.4.2.post1715100402/authentik_client/models/group.py
+-rw-r--r--   0        0        0     4209 2024-05-07 16:46:54.259043 authentik_client-2024.4.2.post1715100402/authentik_client/models/group_member.py
+-rw-r--r--   0        0        0     4006 2024-05-07 16:46:54.263043 authentik_client-2024.4.2.post1715100402/authentik_client/models/group_member_request.py
+-rw-r--r--   0        0        0     3347 2024-05-07 16:46:54.267043 authentik_client-2024.4.2.post1715100402/authentik_client/models/group_request.py
+-rw-r--r--   0        0        0     6080 2024-05-07 16:46:54.271043 authentik_client-2024.4.2.post1715100402/authentik_client/models/identification_challenge.py
+-rw-r--r--   0        0        0     3174 2024-05-07 16:46:54.279043 authentik_client-2024.4.2.post1715100402/authentik_client/models/identification_challenge_response_request.py
+-rw-r--r--   0        0        0     7503 2024-05-07 16:46:54.287043 authentik_client-2024.4.2.post1715100402/authentik_client/models/identification_stage.py
+-rw-r--r--   0        0        0     6533 2024-05-07 16:46:54.295043 authentik_client-2024.4.2.post1715100402/authentik_client/models/identification_stage_request.py
+-rw-r--r--   0        0        0     2438 2024-05-07 16:46:54.299043 authentik_client-2024.4.2.post1715100402/authentik_client/models/install_id.py
+-rw-r--r--   0        0        0      771 2024-05-07 16:46:54.303043 authentik_client-2024.4.2.post1715100402/authentik_client/models/intent_enum.py
+-rw-r--r--   0        0        0      800 2024-05-07 16:46:54.307043 authentik_client-2024.4.2.post1715100402/authentik_client/models/invalid_response_action_enum.py
+-rw-r--r--   0        0        0     4878 2024-05-07 16:46:54.311043 authentik_client-2024.4.2.post1715100402/authentik_client/models/invitation.py
+-rw-r--r--   0        0        0     3895 2024-05-07 16:46:54.319043 authentik_client-2024.4.2.post1715100402/authentik_client/models/invitation_request.py
+-rw-r--r--   0        0        0     4508 2024-05-07 16:46:54.327043 authentik_client-2024.4.2.post1715100402/authentik_client/models/invitation_stage.py
+-rw-r--r--   0        0        0     3527 2024-05-07 16:46:54.335043 authentik_client-2024.4.2.post1715100402/authentik_client/models/invitation_stage_request.py
+-rw-r--r--   0        0        0      729 2024-05-07 16:46:54.339043 authentik_client-2024.4.2.post1715100402/authentik_client/models/issuer_mode_enum.py
+-rw-r--r--   0        0        0     4386 2024-05-07 16:46:54.343043 authentik_client-2024.4.2.post1715100402/authentik_client/models/kubernetes_service_connection.py
+-rw-r--r--   0        0        0     3454 2024-05-07 16:46:54.351043 authentik_client-2024.4.2.post1715100402/authentik_client/models/kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     2811 2024-05-07 16:46:54.359043 authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_debug.py
+-rw-r--r--   0        0        0     5765 2024-05-07 16:46:54.363043 authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_outpost_config.py
+-rw-r--r--   0        0        0     4378 2024-05-07 16:46:54.371043 authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_property_mapping.py
+-rw-r--r--   0        0        0     3478 2024-05-07 16:46:54.375043 authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     8694 2024-05-07 16:46:54.383043 authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_provider.py
+-rw-r--r--   0        0        0     6192 2024-05-07 16:46:54.391043 authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_provider_request.py
+-rw-r--r--   0        0        0    11791 2024-05-07 16:46:54.399043 authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_source.py
+-rw-r--r--   0        0        0     9542 2024-05-07 16:46:54.407043 authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_source_request.py
+-rw-r--r--   0        0        0     3129 2024-05-07 16:46:54.415043 authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_sync_status.py
+-rw-r--r--   0        0        0      726 2024-05-07 16:46:54.351043 authentik_client-2024.4.2.post1715100402/authentik_client/models/ldapapi_access_mode.py
+-rw-r--r--   0        0        0     3278 2024-05-07 16:46:54.419043 authentik_client-2024.4.2.post1715100402/authentik_client/models/license.py
+-rw-r--r--   0        0        0     2897 2024-05-07 16:46:54.427043 authentik_client-2024.4.2.post1715100402/authentik_client/models/license_forecast.py
+-rw-r--r--   0        0        0     2509 2024-05-07 16:46:54.431043 authentik_client-2024.4.2.post1715100402/authentik_client/models/license_request.py
+-rw-r--r--   0        0        0     3222 2024-05-07 16:46:54.439043 authentik_client-2024.4.2.post1715100402/authentik_client/models/license_summary.py
+-rw-r--r--   0        0        0     2411 2024-05-07 16:46:54.443043 authentik_client-2024.4.2.post1715100402/authentik_client/models/link.py
+-rw-r--r--   0        0        0     2882 2024-05-07 16:46:54.451043 authentik_client-2024.4.2.post1715100402/authentik_client/models/log_event.py
+-rw-r--r--   0        0        0      843 2024-05-07 16:46:54.455043 authentik_client-2024.4.2.post1715100402/authentik_client/models/log_level_enum.py
+-rw-r--r--   0        0        0     6520 2024-05-07 16:46:54.459043 authentik_client-2024.4.2.post1715100402/authentik_client/models/login_challenge_types.py
+-rw-r--r--   0        0        0     4171 2024-05-07 16:46:54.467043 authentik_client-2024.4.2.post1715100402/authentik_client/models/login_metrics.py
+-rw-r--r--   0        0        0     3192 2024-05-07 16:46:54.471043 authentik_client-2024.4.2.post1715100402/authentik_client/models/login_source.py
+-rw-r--r--   0        0        0     2513 2024-05-07 16:46:54.479043 authentik_client-2024.4.2.post1715100402/authentik_client/models/metadata.py
+-rw-r--r--   0        0        0     7604 2024-05-07 16:46:54.483043 authentik_client-2024.4.2.post1715100402/authentik_client/models/model_enum.py
+-rw-r--r--   0        0        0     9828 2024-05-07 16:46:54.487043 authentik_client-2024.4.2.post1715100402/authentik_client/models/model_request.py
+-rw-r--r--   0        0        0     1559 2024-05-07 16:46:54.491043 authentik_client-2024.4.2.post1715100402/authentik_client/models/name_id_policy_enum.py
+-rw-r--r--   0        0        0      831 2024-05-07 16:46:54.495043 authentik_client-2024.4.2.post1715100402/authentik_client/models/network_binding_enum.py
+-rw-r--r--   0        0        0      764 2024-05-07 16:46:54.495043 authentik_client-2024.4.2.post1715100402/authentik_client/models/not_configured_action_enum.py
+-rw-r--r--   0        0        0     3479 2024-05-07 16:46:54.499043 authentik_client-2024.4.2.post1715100402/authentik_client/models/notification.py
+-rw-r--r--   0        0        0     2858 2024-05-07 16:46:54.503043 authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_request.py
+-rw-r--r--   0        0        0     4010 2024-05-07 16:46:54.507043 authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_rule.py
+-rw-r--r--   0        0        0     3549 2024-05-07 16:46:54.511043 authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_rule_request.py
+-rw-r--r--   0        0        0     3760 2024-05-07 16:46:54.515043 authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_transport.py
+-rw-r--r--   0        0        0      818 2024-05-07 16:46:54.515043 authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_transport_mode_enum.py
+-rw-r--r--   0        0        0     3500 2024-05-07 16:46:54.519043 authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_transport_request.py
+-rw-r--r--   0        0        0     2503 2024-05-07 16:46:54.523043 authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_transport_test.py
+-rw-r--r--   0        0        0     2707 2024-05-07 16:46:54.527043 authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_webhook_mapping.py
+-rw-r--r--   0        0        0     2717 2024-05-07 16:46:54.531043 authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     8888 2024-05-07 16:46:54.535043 authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth2_provider.py
+-rw-r--r--   0        0        0     6654 2024-05-07 16:46:54.539043 authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth2_provider_request.py
+-rw-r--r--   0        0        0     3482 2024-05-07 16:46:54.543043 authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth2_provider_setup_urls.py
+-rw-r--r--   0        0        0     4164 2024-05-07 16:46:54.547043 authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth_device_code_challenge.py
+-rw-r--r--   0        0        0     2846 2024-05-07 16:46:54.551043 authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth_device_code_challenge_response_request.py
+-rw-r--r--   0        0        0     4213 2024-05-07 16:46:54.555043 authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth_device_code_finish_challenge.py
+-rw-r--r--   0        0        0     2816 2024-05-07 16:46:54.559043 authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py
+-rw-r--r--   0        0        0    10563 2024-05-07 16:46:54.563043 authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth_source.py
+-rw-r--r--   0        0        0     8013 2024-05-07 16:46:54.567043 authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth_source_request.py
+-rw-r--r--   0        0        0     3922 2024-05-07 16:46:54.571043 authentik_client-2024.4.2.post1715100402/authentik_client/models/open_id_connect_configuration.py
+-rw-r--r--   0        0        0     5545 2024-05-07 16:46:54.575043 authentik_client-2024.4.2.post1715100402/authentik_client/models/outpost.py
+-rw-r--r--   0        0        0     2541 2024-05-07 16:46:54.579043 authentik_client-2024.4.2.post1715100402/authentik_client/models/outpost_default_config.py
+-rw-r--r--   0        0        0     3755 2024-05-07 16:46:54.583043 authentik_client-2024.4.2.post1715100402/authentik_client/models/outpost_health.py
+-rw-r--r--   0        0        0     4050 2024-05-07 16:46:54.587043 authentik_client-2024.4.2.post1715100402/authentik_client/models/outpost_request.py
+-rw-r--r--   0        0        0      752 2024-05-07 16:46:54.587043 authentik_client-2024.4.2.post1715100402/authentik_client/models/outpost_type_enum.py
+-rw-r--r--   0        0        0     3322 2024-05-07 16:46:54.591043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_application_list.py
+-rw-r--r--   0        0        0     3395 2024-05-07 16:46:54.595043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticated_session_list.py
+-rw-r--r--   0        0        0     3404 2024-05-07 16:46:54.599043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticator_duo_stage_list.py
+-rw-r--r--   0        0        0     3404 2024-05-07 16:46:54.599043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticator_sms_stage_list.py
+-rw-r--r--   0        0        0     3428 2024-05-07 16:46:54.603043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticator_static_stage_list.py
+-rw-r--r--   0        0        0     3412 2024-05-07 16:46:54.607043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticator_totp_stage_list.py
+-rw-r--r--   0        0        0     3444 2024-05-07 16:46:54.611043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticator_validate_stage_list.py
+-rw-r--r--   0        0        0     3445 2024-05-07 16:46:54.615043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticator_web_authn_stage_list.py
+-rw-r--r--   0        0        0     3371 2024-05-07 16:46:54.619043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_blueprint_instance_list.py
+-rw-r--r--   0        0        0     3274 2024-05-07 16:46:54.619043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_brand_list.py
+-rw-r--r--   0        0        0     3331 2024-05-07 16:46:54.623043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_captcha_stage_list.py
+-rw-r--r--   0        0        0     3380 2024-05-07 16:46:54.627043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_certificate_key_pair_list.py
+-rw-r--r--   0        0        0     3355 2024-05-07 16:46:54.631043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_connection_token_list.py
+-rw-r--r--   0        0        0     3331 2024-05-07 16:46:54.635043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_consent_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-05-07 16:46:54.639043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_deny_stage_list.py
+-rw-r--r--   0        0        0     3420 2024-05-07 16:46:54.643043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_docker_service_connection_list.py
+-rw-r--r--   0        0        0     3282 2024-05-07 16:46:54.643043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_domain_list.py
+-rw-r--r--   0        0        0     3323 2024-05-07 16:46:54.651043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_dummy_policy_list.py
+-rw-r--r--   0        0        0     3315 2024-05-07 16:46:54.655043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_dummy_stage_list.py
+-rw-r--r--   0        0        0     3307 2024-05-07 16:46:54.659043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_duo_device_list.py
+-rw-r--r--   0        0        0     3315 2024-05-07 16:46:54.659043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_email_stage_list.py
+-rw-r--r--   0        0        0     3298 2024-05-07 16:46:54.663043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_endpoint_list.py
+-rw-r--r--   0        0        0     3274 2024-05-07 16:46:54.667043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_event_list.py
+-rw-r--r--   0        0        0     3380 2024-05-07 16:46:54.671043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_event_matcher_policy_list.py
+-rw-r--r--   0        0        0     3413 2024-05-07 16:46:54.675043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_expiring_base_grant_model_list.py
+-rw-r--r--   0        0        0     3363 2024-05-07 16:46:54.679043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_expression_policy_list.py
+-rw-r--r--   0        0        0     3437 2024-05-07 16:46:54.683043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_extra_role_object_permission_list.py
+-rw-r--r--   0        0        0     3437 2024-05-07 16:46:54.687043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_extra_user_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-05-07 16:46:54.687043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_flow_list.py
+-rw-r--r--   0        0        0     3364 2024-05-07 16:46:54.695043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_flow_stage_binding_list.py
+-rw-r--r--   0        0        0     3274 2024-05-07 16:46:54.703043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_group_list.py
+-rw-r--r--   0        0        0     3387 2024-05-07 16:46:54.707043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_identification_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-05-07 16:46:54.711043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_invitation_list.py
+-rw-r--r--   0        0        0     3355 2024-05-07 16:46:54.715043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_invitation_stage_list.py
+-rw-r--r--   0        0        0     3452 2024-05-07 16:46:54.719043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_kubernetes_service_connection_list.py
+-rw-r--r--   0        0        0     3372 2024-05-07 16:46:54.727043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_ldap_outpost_config_list.py
+-rw-r--r--   0        0        0     3388 2024-05-07 16:46:54.731043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_ldap_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-05-07 16:46:54.735043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_ldap_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-05-07 16:46:54.739043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_ldap_source_list.py
+-rw-r--r--   0        0        0     3290 2024-05-07 16:46:54.747043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_license_list.py
+-rw-r--r--   0        0        0     3330 2024-05-07 16:46:54.751043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_notification_list.py
+-rw-r--r--   0        0        0     3363 2024-05-07 16:46:54.755043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_notification_rule_list.py
+-rw-r--r--   0        0        0     3403 2024-05-07 16:46:54.759043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_notification_transport_list.py
+-rw-r--r--   0        0        0     3444 2024-05-07 16:46:54.767043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_notification_webhook_mapping_list.py
+-rw-r--r--   0        0        0     3348 2024-05-07 16:46:54.771043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_o_auth2_provider_list.py
+-rw-r--r--   0        0        0     3324 2024-05-07 16:46:54.775043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_o_auth_source_list.py
+-rw-r--r--   0        0        0     3290 2024-05-07 16:46:54.779043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_outpost_list.py
+-rw-r--r--   0        0        0     3396 2024-05-07 16:46:54.783043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_password_expiry_policy_list.py
+-rw-r--r--   0        0        0     3347 2024-05-07 16:46:54.791043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_password_policy_list.py
+-rw-r--r--   0        0        0     3339 2024-05-07 16:46:54.795043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_password_stage_list.py
+-rw-r--r--   0        0        0     3314 2024-05-07 16:46:54.799043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_permission_list.py
+-rw-r--r--   0        0        0     3396 2024-05-07 16:46:54.803043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_plex_source_connection_list.py
+-rw-r--r--   0        0        0     3315 2024-05-07 16:46:54.807043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_plex_source_list.py
+-rw-r--r--   0        0        0     3339 2024-05-07 16:46:54.811043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_policy_binding_list.py
+-rw-r--r--   0        0        0     3282 2024-05-07 16:46:54.815043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_policy_list.py
+-rw-r--r--   0        0        0     3282 2024-05-07 16:46:54.819043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_prompt_list.py
+-rw-r--r--   0        0        0     3323 2024-05-07 16:46:54.823043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_prompt_stage_list.py
+-rw-r--r--   0        0        0     3355 2024-05-07 16:46:54.823043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_property_mapping_list.py
+-rw-r--r--   0        0        0     3298 2024-05-07 16:46:54.827043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-05-07 16:46:54.831043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_proxy_outpost_config_list.py
+-rw-r--r--   0        0        0     3339 2024-05-07 16:46:54.835043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_proxy_provider_list.py
+-rw-r--r--   0        0        0     3380 2024-05-07 16:46:54.839043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_rac_property_mapping_list.py
+-rw-r--r--   0        0        0     3323 2024-05-07 16:46:54.843043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_rac_provider_list.py
+-rw-r--r--   0        0        0     3388 2024-05-07 16:46:54.847043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_radius_outpost_config_list.py
+-rw-r--r--   0        0        0     3347 2024-05-07 16:46:54.847043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_radius_provider_list.py
+-rw-r--r--   0        0        0     3314 2024-05-07 16:46:54.851043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_reputation_list.py
+-rw-r--r--   0        0        0     3363 2024-05-07 16:46:54.855043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_reputation_policy_list.py
+-rw-r--r--   0        0        0     3461 2024-05-07 16:46:54.859043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_role_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3266 2024-05-07 16:46:54.863043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_role_list.py
+-rw-r--r--   0        0        0     3388 2024-05-07 16:46:54.863043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_saml_property_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-05-07 16:46:54.867043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_saml_provider_list.py
+-rw-r--r--   0        0        0     3315 2024-05-07 16:46:54.871043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_saml_source_list.py
+-rw-r--r--   0        0        0     3323 2024-05-07 16:46:54.875043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_scim_mapping_list.py
+-rw-r--r--   0        0        0     3331 2024-05-07 16:46:54.879043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_scim_provider_list.py
+-rw-r--r--   0        0        0     3356 2024-05-07 16:46:54.879043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_scim_source_group_list.py
+-rw-r--r--   0        0        0     3315 2024-05-07 16:46:54.883043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_scim_source_list.py
+-rw-r--r--   0        0        0     3348 2024-05-07 16:46:54.887043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_scim_source_user_list.py
+-rw-r--r--   0        0        0     3331 2024-05-07 16:46:54.895043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_scope_mapping_list.py
+-rw-r--r--   0        0        0     3371 2024-05-07 16:46:54.895043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_service_connection_list.py
+-rw-r--r--   0        0        0     3307 2024-05-07 16:46:54.891043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_sms_device_list.py
+-rw-r--r--   0        0        0     3282 2024-05-07 16:46:54.899043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_source_list.py
+-rw-r--r--   0        0        0     3323 2024-05-07 16:46:54.903043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_source_stage_list.py
+-rw-r--r--   0        0        0     3274 2024-05-07 16:46:54.907043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_stage_list.py
+-rw-r--r--   0        0        0     3331 2024-05-07 16:46:54.911043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_static_device_list.py
+-rw-r--r--   0        0        0     3315 2024-05-07 16:46:54.911043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_system_task_list.py
+-rw-r--r--   0        0        0     3282 2024-05-07 16:46:54.919043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_tenant_list.py
+-rw-r--r--   0        0        0     3274 2024-05-07 16:46:54.923043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_token_list.py
+-rw-r--r--   0        0        0     3315 2024-05-07 16:46:54.923043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_token_model_list.py
+-rw-r--r--   0        0        0     3315 2024-05-07 16:46:54.915043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_totp_device_list.py
+-rw-r--r--   0        0        0     3461 2024-05-07 16:46:54.927043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_assigned_object_permission_list.py
+-rw-r--r--   0        0        0     3323 2024-05-07 16:46:54.931043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_consent_list.py
+-rw-r--r--   0        0        0     3356 2024-05-07 16:46:54.935043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_delete_stage_list.py
+-rw-r--r--   0        0        0     3266 2024-05-07 16:46:54.939043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_list.py
+-rw-r--r--   0        0        0     3348 2024-05-07 16:46:54.939043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_login_stage_list.py
+-rw-r--r--   0        0        0     3356 2024-05-07 16:46:54.943043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_logout_stage_list.py
+-rw-r--r--   0        0        0     3438 2024-05-07 16:46:54.947043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_o_auth_source_connection_list.py
+-rw-r--r--   0        0        0     3429 2024-05-07 16:46:54.951043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_saml_source_connection_list.py
+-rw-r--r--   0        0        0     3396 2024-05-07 16:46:54.955043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_source_connection_list.py
+-rw-r--r--   0        0        0     3348 2024-05-07 16:46:54.959043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_write_stage_list.py
+-rw-r--r--   0        0        0     3348 2024-05-07 16:46:54.959043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_web_authn_device_list.py
+-rw-r--r--   0        0        0     3381 2024-05-07 16:46:54.963043 authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_web_authn_device_type_list.py
+-rw-r--r--   0        0        0     3076 2024-05-07 16:46:54.967043 authentik_client-2024.4.2.post1715100402/authentik_client/models/pagination.py
+-rw-r--r--   0        0        0     4454 2024-05-07 16:46:54.971043 authentik_client-2024.4.2.post1715100402/authentik_client/models/password_challenge.py
+-rw-r--r--   0        0        0     2819 2024-05-07 16:46:54.975043 authentik_client-2024.4.2.post1715100402/authentik_client/models/password_challenge_response_request.py
+-rw-r--r--   0        0        0     4377 2024-05-07 16:46:54.979043 authentik_client-2024.4.2.post1715100402/authentik_client/models/password_expiry_policy.py
+-rw-r--r--   0        0        0     3099 2024-05-07 16:46:54.983043 authentik_client-2024.4.2.post1715100402/authentik_client/models/password_expiry_policy_request.py
+-rw-r--r--   0        0        0     6428 2024-05-07 16:46:54.983043 authentik_client-2024.4.2.post1715100402/authentik_client/models/password_policy.py
+-rw-r--r--   0        0        0     5239 2024-05-07 16:46:54.987043 authentik_client-2024.4.2.post1715100402/authentik_client/models/password_policy_request.py
+-rw-r--r--   0        0        0     5274 2024-05-07 16:46:54.991043 authentik_client-2024.4.2.post1715100402/authentik_client/models/password_stage.py
+-rw-r--r--   0        0        0     4264 2024-05-07 16:46:54.995043 authentik_client-2024.4.2.post1715100402/authentik_client/models/password_stage_request.py
+-rw-r--r--   0        0        0     4594 2024-05-07 16:46:54.999043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_application_request.py
+-rw-r--r--   0        0        0     4833 2024-05-07 16:46:55.003043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_authenticator_duo_stage_request.py
+-rw-r--r--   0        0        0     5701 2024-05-07 16:46:55.003043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_authenticator_sms_stage_request.py
+-rw-r--r--   0        0        0     4430 2024-05-07 16:46:55.007043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_authenticator_static_stage_request.py
+-rw-r--r--   0        0        0     4256 2024-05-07 16:46:55.011043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_authenticator_totp_stage_request.py
+-rw-r--r--   0        0        0     4931 2024-05-07 16:46:55.015043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_authenticator_validate_stage_request.py
+-rw-r--r--   0        0        0     5340 2024-05-07 16:46:55.015043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_authenticator_web_authn_stage_request.py
+-rw-r--r--   0        0        0     3246 2024-05-07 16:46:55.019043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_blueprint_instance_request.py
+-rw-r--r--   0        0        0     6352 2024-05-07 16:46:55.023043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_brand_request.py
+-rw-r--r--   0        0        0     3860 2024-05-07 16:46:55.027043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_captcha_stage_request.py
+-rw-r--r--   0        0        0     3051 2024-05-07 16:46:55.031043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_certificate_key_pair_request.py
+-rw-r--r--   0        0        0     2717 2024-05-07 16:46:55.031043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_connection_token_request.py
+-rw-r--r--   0        0        0     3607 2024-05-07 16:46:55.035043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_consent_stage_request.py
+-rw-r--r--   0        0        0     3268 2024-05-07 16:46:55.039043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_deny_stage_request.py
+-rw-r--r--   0        0        0     4149 2024-05-07 16:46:55.043043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_docker_service_connection_request.py
+-rw-r--r--   0        0        0     2801 2024-05-07 16:46:55.047043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_domain_request.py
+-rw-r--r--   0        0        0     3275 2024-05-07 16:46:55.047043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_dummy_policy_request.py
+-rw-r--r--   0        0        0     3270 2024-05-07 16:46:55.051043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_dummy_stage_request.py
+-rw-r--r--   0        0        0     2674 2024-05-07 16:46:55.055043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_duo_device_request.py
+-rw-r--r--   0        0        0     5159 2024-05-07 16:46:55.059043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_email_stage_request.py
+-rw-r--r--   0        0        0     3784 2024-05-07 16:46:55.059043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_endpoint_request.py
+-rw-r--r--   0        0        0     4845 2024-05-07 16:46:55.063043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_event_matcher_policy_request.py
+-rw-r--r--   0        0        0     4045 2024-05-07 16:46:55.067043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_event_request.py
+-rw-r--r--   0        0        0     3047 2024-05-07 16:46:55.071043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_expression_policy_request.py
+-rw-r--r--   0        0        0     4903 2024-05-07 16:46:55.075043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_flow_request.py
+-rw-r--r--   0        0        0     4055 2024-05-07 16:46:55.075043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_flow_stage_binding_request.py
+-rw-r--r--   0        0        0     3385 2024-05-07 16:46:55.079043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_group_request.py
+-rw-r--r--   0        0        0     6571 2024-05-07 16:46:55.083043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_identification_stage_request.py
+-rw-r--r--   0        0        0     3985 2024-05-07 16:46:55.087043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_invitation_request.py
+-rw-r--r--   0        0        0     3565 2024-05-07 16:46:55.091043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_invitation_stage_request.py
+-rw-r--r--   0        0        0     3492 2024-05-07 16:46:55.091043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_kubernetes_service_connection_request.py
+-rw-r--r--   0        0        0     3550 2024-05-07 16:46:55.095043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_ldap_property_mapping_request.py
+-rw-r--r--   0        0        0     6254 2024-05-07 16:46:55.099043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_ldap_provider_request.py
+-rw-r--r--   0        0        0     9697 2024-05-07 16:46:55.103043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_ldap_source_request.py
+-rw-r--r--   0        0        0     2557 2024-05-07 16:46:55.107043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_license_request.py
+-rw-r--r--   0        0        0     2879 2024-05-07 16:46:55.107043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_notification_request.py
+-rw-r--r--   0        0        0     3587 2024-05-07 16:46:55.111043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_notification_rule_request.py
+-rw-r--r--   0        0        0     3538 2024-05-07 16:46:55.115043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_notification_transport_request.py
+-rw-r--r--   0        0        0     2782 2024-05-07 16:46:55.115043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_notification_webhook_mapping_request.py
+-rw-r--r--   0        0        0     6716 2024-05-07 16:46:55.119043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_o_auth2_provider_request.py
+-rw-r--r--   0        0        0     8185 2024-05-07 16:46:55.123043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_o_auth_source_request.py
+-rw-r--r--   0        0        0     4139 2024-05-07 16:46:55.127043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_outpost_request.py
+-rw-r--r--   0        0        0     3154 2024-05-07 16:46:55.127043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_password_expiry_policy_request.py
+-rw-r--r--   0        0        0     5277 2024-05-07 16:46:55.131043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_password_policy_request.py
+-rw-r--r--   0        0        0     4326 2024-05-07 16:46:55.135043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_password_stage_request.py
+-rw-r--r--   0        0        0     2922 2024-05-07 16:46:55.139043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_permission_assign_request.py
+-rw-r--r--   0        0        0     2784 2024-05-07 16:46:55.143043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_plex_source_connection_request.py
+-rw-r--r--   0        0        0     5905 2024-05-07 16:46:55.147043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_plex_source_request.py
+-rw-r--r--   0        0        0     4286 2024-05-07 16:46:55.147043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_policy_binding_request.py
+-rw-r--r--   0        0        0     5023 2024-05-07 16:46:55.151043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_prompt_request.py
+-rw-r--r--   0        0        0     3406 2024-05-07 16:46:55.151043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_prompt_stage_request.py
+-rw-r--r--   0        0        0     6907 2024-05-07 16:46:55.155043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_proxy_provider_request.py
+-rw-r--r--   0        0        0     3495 2024-05-07 16:46:55.159043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_rac_property_mapping_request.py
+-rw-r--r--   0        0        0     4413 2024-05-07 16:46:55.159043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_rac_provider_request.py
+-rw-r--r--   0        0        0     4563 2024-05-07 16:46:55.163043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_radius_provider_request.py
+-rw-r--r--   0        0        0     3276 2024-05-07 16:46:55.167043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_reputation_policy_request.py
+-rw-r--r--   0        0        0     2565 2024-05-07 16:46:55.167043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_role_request.py
+-rw-r--r--   0        0        0     3901 2024-05-07 16:46:55.171043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_saml_property_mapping_request.py
+-rw-r--r--   0        0        0     7539 2024-05-07 16:46:55.175043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_saml_provider_request.py
+-rw-r--r--   0        0        0     8676 2024-05-07 16:46:55.179043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_saml_source_request.py
+-rw-r--r--   0        0        0     3364 2024-05-07 16:46:55.179043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_scim_mapping_request.py
+-rw-r--r--   0        0        0     3888 2024-05-07 16:46:55.183043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_scim_provider_request.py
+-rw-r--r--   0        0        0     3095 2024-05-07 16:46:55.183043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_scim_source_group_request.py
+-rw-r--r--   0        0        0     3829 2024-05-07 16:46:55.187043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_scim_source_request.py
+-rw-r--r--   0        0        0     3098 2024-05-07 16:46:55.191043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_scim_source_user_request.py
+-rw-r--r--   0        0        0     3819 2024-05-07 16:46:55.195043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_scope_mapping_request.py
+-rw-r--r--   0        0        0     5079 2024-05-07 16:46:55.199043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_settings_request.py
+-rw-r--r--   0        0        0     2674 2024-05-07 16:46:55.191043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_sms_device_request.py
+-rw-r--r--   0        0        0     3562 2024-05-07 16:46:55.203043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_source_stage_request.py
+-rw-r--r--   0        0        0     2686 2024-05-07 16:46:55.203043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_static_device_request.py
+-rw-r--r--   0        0        0     2820 2024-05-07 16:46:55.211043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_tenant_request.py
+-rw-r--r--   0        0        0     4419 2024-05-07 16:46:55.211043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_token_request.py
+-rw-r--r--   0        0        0     2678 2024-05-07 16:46:55.207043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_totp_device_request.py
+-rw-r--r--   0        0        0     3167 2024-05-07 16:46:55.215043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_delete_stage_request.py
+-rw-r--r--   0        0        0     4766 2024-05-07 16:46:55.219043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_login_stage_request.py
+-rw-r--r--   0        0        0     3167 2024-05-07 16:46:55.223043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_logout_stage_request.py
+-rw-r--r--   0        0        0     3109 2024-05-07 16:46:55.223043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3934 2024-05-07 16:46:55.227043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_request.py
+-rw-r--r--   0        0        0     2733 2024-05-07 16:46:55.231043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     4450 2024-05-07 16:46:55.231043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_write_stage_request.py
+-rw-r--r--   0        0        0     2625 2024-05-07 16:46:55.239043 authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_web_authn_device_request.py
+-rw-r--r--   0        0        0     3548 2024-05-07 16:46:55.239043 authentik_client-2024.4.2.post1715100402/authentik_client/models/permission.py
+-rw-r--r--   0        0        0     2884 2024-05-07 16:46:55.243043 authentik_client-2024.4.2.post1715100402/authentik_client/models/permission_assign_request.py
+-rw-r--r--   0        0        0     4315 2024-05-07 16:46:55.247043 authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_authentication_challenge.py
+-rw-r--r--   0        0        0     2726 2024-05-07 16:46:55.247043 authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_authentication_challenge_response_request.py
+-rw-r--r--   0        0        0     7752 2024-05-07 16:46:55.251043 authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_source.py
+-rw-r--r--   0        0        0     3265 2024-05-07 16:46:55.251043 authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_source_connection.py
+-rw-r--r--   0        0        0     2719 2024-05-07 16:46:55.255043 authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_source_connection_request.py
+-rw-r--r--   0        0        0     5760 2024-05-07 16:46:55.259043 authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_source_request.py
+-rw-r--r--   0        0        0     2576 2024-05-07 16:46:55.259043 authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_token_redeem_request.py
+-rw-r--r--   0        0        0     4055 2024-05-07 16:46:55.263043 authentik_client-2024.4.2.post1715100402/authentik_client/models/policy.py
+-rw-r--r--   0        0        0     5643 2024-05-07 16:46:55.263043 authentik_client-2024.4.2.post1715100402/authentik_client/models/policy_binding.py
+-rw-r--r--   0        0        0     4231 2024-05-07 16:46:55.267042 authentik_client-2024.4.2.post1715100402/authentik_client/models/policy_binding_request.py
+-rw-r--r--   0        0        0      711 2024-05-07 16:46:55.267042 authentik_client-2024.4.2.post1715100402/authentik_client/models/policy_engine_mode.py
+-rw-r--r--   0        0        0     2817 2024-05-07 16:46:55.271043 authentik_client-2024.4.2.post1715100402/authentik_client/models/policy_request.py
+-rw-r--r--   0        0        0     2583 2024-05-07 16:46:55.271043 authentik_client-2024.4.2.post1715100402/authentik_client/models/policy_test_request.py
+-rw-r--r--   0        0        0     3281 2024-05-07 16:46:55.271043 authentik_client-2024.4.2.post1715100402/authentik_client/models/policy_test_result.py
+-rw-r--r--   0        0        0     4885 2024-05-07 16:46:55.275043 authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt.py
+-rw-r--r--   0        0        0     4649 2024-05-07 16:46:55.279043 authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt_challenge.py
+-rw-r--r--   0        0        0     3325 2024-05-07 16:46:55.279043 authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt_challenge_response_request.py
+-rw-r--r--   0        0        0     4927 2024-05-07 16:46:55.279043 authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt_request.py
+-rw-r--r--   0        0        0     4321 2024-05-07 16:46:55.283043 authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt_stage.py
+-rw-r--r--   0        0        0     3351 2024-05-07 16:46:55.283043 authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt_stage_request.py
+-rw-r--r--   0        0        0     1185 2024-05-07 16:46:55.287043 authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt_type_enum.py
+-rw-r--r--   0        0        0     4264 2024-05-07 16:46:55.287043 authentik_client-2024.4.2.post1715100402/authentik_client/models/property_mapping.py
+-rw-r--r--   0        0        0     2610 2024-05-07 16:46:55.291043 authentik_client-2024.4.2.post1715100402/authentik_client/models/property_mapping_preview.py
+-rw-r--r--   0        0        0     2744 2024-05-07 16:46:55.291043 authentik_client-2024.4.2.post1715100402/authentik_client/models/property_mapping_test_result.py
+-rw-r--r--   0        0        0      715 2024-05-07 16:46:55.291043 authentik_client-2024.4.2.post1715100402/authentik_client/models/protocol_enum.py
+-rw-r--r--   0        0        0     5722 2024-05-07 16:46:55.295043 authentik_client-2024.4.2.post1715100402/authentik_client/models/provider.py
+-rw-r--r--   0        0        0      713 2024-05-07 16:46:55.295043 authentik_client-2024.4.2.post1715100402/authentik_client/models/provider_enum.py
+-rw-r--r--   0        0        0     1314 2024-05-07 16:46:55.295043 authentik_client-2024.4.2.post1715100402/authentik_client/models/provider_model_enum.py
+-rw-r--r--   0        0        0     3397 2024-05-07 16:46:55.299043 authentik_client-2024.4.2.post1715100402/authentik_client/models/provider_request.py
+-rw-r--r--   0        0        0     1009 2024-05-07 16:46:55.299043 authentik_client-2024.4.2.post1715100402/authentik_client/models/provider_type_enum.py
+-rw-r--r--   0        0        0      754 2024-05-07 16:46:55.303043 authentik_client-2024.4.2.post1715100402/authentik_client/models/proxy_mode.py
+-rw-r--r--   0        0        0     7819 2024-05-07 16:46:55.303043 authentik_client-2024.4.2.post1715100402/authentik_client/models/proxy_outpost_config.py
+-rw-r--r--   0        0        0     9552 2024-05-07 16:46:55.307043 authentik_client-2024.4.2.post1715100402/authentik_client/models/proxy_provider.py
+-rw-r--r--   0        0        0     6828 2024-05-07 16:46:55.307043 authentik_client-2024.4.2.post1715100402/authentik_client/models/proxy_provider_request.py
+-rw-r--r--   0        0        0     4407 2024-05-07 16:46:55.311043 authentik_client-2024.4.2.post1715100402/authentik_client/models/rac_property_mapping.py
+-rw-r--r--   0        0        0     3440 2024-05-07 16:46:55.311043 authentik_client-2024.4.2.post1715100402/authentik_client/models/rac_property_mapping_request.py
+-rw-r--r--   0        0        0     6813 2024-05-07 16:46:55.315043 authentik_client-2024.4.2.post1715100402/authentik_client/models/rac_provider.py
+-rw-r--r--   0        0        0     4351 2024-05-07 16:46:55.315043 authentik_client-2024.4.2.post1715100402/authentik_client/models/rac_provider_request.py
+-rw-r--r--   0        0        0     3833 2024-05-07 16:46:55.319043 authentik_client-2024.4.2.post1715100402/authentik_client/models/radius_outpost_config.py
+-rw-r--r--   0        0        0     6924 2024-05-07 16:46:55.319043 authentik_client-2024.4.2.post1715100402/authentik_client/models/radius_provider.py
+-rw-r--r--   0        0        0     4501 2024-05-07 16:46:55.323042 authentik_client-2024.4.2.post1715100402/authentik_client/models/radius_provider_request.py
+-rw-r--r--   0        0        0     4184 2024-05-07 16:46:55.323042 authentik_client-2024.4.2.post1715100402/authentik_client/models/redirect_challenge.py
+-rw-r--r--   0        0        0     3642 2024-05-07 16:46:55.327043 authentik_client-2024.4.2.post1715100402/authentik_client/models/reputation.py
+-rw-r--r--   0        0        0     4516 2024-05-07 16:46:55.331043 authentik_client-2024.4.2.post1715100402/authentik_client/models/reputation_policy.py
+-rw-r--r--   0        0        0     3238 2024-05-07 16:46:55.331043 authentik_client-2024.4.2.post1715100402/authentik_client/models/reputation_policy_request.py
+-rw-r--r--   0        0        0      795 2024-05-07 16:46:55.335043 authentik_client-2024.4.2.post1715100402/authentik_client/models/resident_key_requirement_enum.py
+-rw-r--r--   0        0        0     2618 2024-05-07 16:46:55.335043 authentik_client-2024.4.2.post1715100402/authentik_client/models/role.py
+-rw-r--r--   0        0        0     3333 2024-05-07 16:46:55.339043 authentik_client-2024.4.2.post1715100402/authentik_client/models/role_assigned_object_permission.py
+-rw-r--r--   0        0        0     3293 2024-05-07 16:46:55.339043 authentik_client-2024.4.2.post1715100402/authentik_client/models/role_object_permission.py
+-rw-r--r--   0        0        0     2517 2024-05-07 16:46:55.343043 authentik_client-2024.4.2.post1715100402/authentik_client/models/role_request.py
+-rw-r--r--   0        0        0     2712 2024-05-07 16:46:55.343043 authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_metadata.py
+-rw-r--r--   0        0        0     4718 2024-05-07 16:46:55.347043 authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_property_mapping.py
+-rw-r--r--   0        0        0     3829 2024-05-07 16:46:55.351043 authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_property_mapping_request.py
+-rw-r--r--   0        0        0    11056 2024-05-07 16:46:55.351043 authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_provider.py
+-rw-r--r--   0        0        0     7460 2024-05-07 16:46:55.355043 authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_provider_request.py
+-rw-r--r--   0        0        0    10563 2024-05-07 16:46:55.355043 authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_source.py
+-rw-r--r--   0        0        0     8507 2024-05-07 16:46:55.359043 authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_source_request.py
+-rw-r--r--   0        0        0     4248 2024-05-07 16:46:55.363043 authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_mapping.py
+-rw-r--r--   0        0        0     3309 2024-05-07 16:46:55.363043 authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_mapping_request.py
+-rw-r--r--   0        0        0     5454 2024-05-07 16:46:55.367043 authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_provider.py
+-rw-r--r--   0        0        0     3802 2024-05-07 16:46:55.367043 authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_provider_request.py
+-rw-r--r--   0        0        0     5999 2024-05-07 16:46:55.371043 authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_source.py
+-rw-r--r--   0        0        0     3369 2024-05-07 16:46:55.375043 authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_source_group.py
+-rw-r--r--   0        0        0     3023 2024-05-07 16:46:55.375043 authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_source_group_request.py
+-rw-r--r--   0        0        0     3708 2024-05-07 16:46:55.379042 authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_source_request.py
+-rw-r--r--   0        0        0     3370 2024-05-07 16:46:55.379042 authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_source_user.py
+-rw-r--r--   0        0        0     3026 2024-05-07 16:46:55.383043 authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_source_user_request.py
+-rw-r--r--   0        0        0     3131 2024-05-07 16:46:55.387043 authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_sync_status.py
+-rw-r--r--   0        0        0     4629 2024-05-07 16:46:55.391043 authentik_client-2024.4.2.post1715100402/authentik_client/models/scope_mapping.py
+-rw-r--r--   0        0        0     3740 2024-05-07 16:46:55.395043 authentik_client-2024.4.2.post1715100402/authentik_client/models/scope_mapping_request.py
+-rw-r--r--   0        0        0     2738 2024-05-07 16:46:55.399043 authentik_client-2024.4.2.post1715100402/authentik_client/models/selectable_stage.py
+-rw-r--r--   0        0        0     3773 2024-05-07 16:46:55.399043 authentik_client-2024.4.2.post1715100402/authentik_client/models/service_connection.py
+-rw-r--r--   0        0        0     2776 2024-05-07 16:46:55.403043 authentik_client-2024.4.2.post1715100402/authentik_client/models/service_connection_request.py
+-rw-r--r--   0        0        0     2731 2024-05-07 16:46:55.407043 authentik_client-2024.4.2.post1715100402/authentik_client/models/service_connection_state.py
+-rw-r--r--   0        0        0     3178 2024-05-07 16:46:55.407043 authentik_client-2024.4.2.post1715100402/authentik_client/models/session_user.py
+-rw-r--r--   0        0        0     4931 2024-05-07 16:46:55.411043 authentik_client-2024.4.2.post1715100402/authentik_client/models/settings.py
+-rw-r--r--   0        0        0     5058 2024-05-07 16:46:55.411043 authentik_client-2024.4.2.post1715100402/authentik_client/models/settings_request.py
+-rw-r--r--   0        0        0      733 2024-05-07 16:46:55.415042 authentik_client-2024.4.2.post1715100402/authentik_client/models/severity_enum.py
+-rw-r--r--   0        0        0     4175 2024-05-07 16:46:55.415042 authentik_client-2024.4.2.post1715100402/authentik_client/models/shell_challenge.py
+-rw-r--r--   0        0        0     2172 2024-05-07 16:46:55.419043 authentik_client-2024.4.2.post1715100402/authentik_client/models/signature_algorithm_enum.py
+-rw-r--r--   0        0        0     2906 2024-05-07 16:46:55.387043 authentik_client-2024.4.2.post1715100402/authentik_client/models/sms_device.py
+-rw-r--r--   0        0        0     2619 2024-05-07 16:46:55.391043 authentik_client-2024.4.2.post1715100402/authentik_client/models/sms_device_request.py
+-rw-r--r--   0        0        0     6945 2024-05-07 16:46:55.423043 authentik_client-2024.4.2.post1715100402/authentik_client/models/source.py
+-rw-r--r--   0        0        0     4836 2024-05-07 16:46:55.423043 authentik_client-2024.4.2.post1715100402/authentik_client/models/source_request.py
+-rw-r--r--   0        0        0     4438 2024-05-07 16:46:55.427043 authentik_client-2024.4.2.post1715100402/authentik_client/models/source_stage.py
+-rw-r--r--   0        0        0     3507 2024-05-07 16:46:55.431043 authentik_client-2024.4.2.post1715100402/authentik_client/models/source_stage_request.py
+-rw-r--r--   0        0        0     5355 2024-05-07 16:46:55.431043 authentik_client-2024.4.2.post1715100402/authentik_client/models/source_type.py
+-rw-r--r--   0        0        0      714 2024-05-07 16:46:55.435042 authentik_client-2024.4.2.post1715100402/authentik_client/models/sp_binding_enum.py
+-rw-r--r--   0        0        0     4070 2024-05-07 16:46:55.435042 authentik_client-2024.4.2.post1715100402/authentik_client/models/stage.py
+-rw-r--r--   0        0        0     3437 2024-05-07 16:46:55.439043 authentik_client-2024.4.2.post1715100402/authentik_client/models/stage_prompt.py
+-rw-r--r--   0        0        0     3089 2024-05-07 16:46:55.439043 authentik_client-2024.4.2.post1715100402/authentik_client/models/stage_request.py
+-rw-r--r--   0        0        0     3385 2024-05-07 16:46:55.443043 authentik_client-2024.4.2.post1715100402/authentik_client/models/static_device.py
+-rw-r--r--   0        0        0     2631 2024-05-07 16:46:55.447043 authentik_client-2024.4.2.post1715100402/authentik_client/models/static_device_request.py
+-rw-r--r--   0        0        0     2546 2024-05-07 16:46:55.447043 authentik_client-2024.4.2.post1715100402/authentik_client/models/static_device_token.py
+-rw-r--r--   0        0        0     2581 2024-05-07 16:46:55.451043 authentik_client-2024.4.2.post1715100402/authentik_client/models/static_device_token_request.py
+-rw-r--r--   0        0        0      846 2024-05-07 16:46:55.451043 authentik_client-2024.4.2.post1715100402/authentik_client/models/sub_mode_enum.py
+-rw-r--r--   0        0        0     4463 2024-05-07 16:46:55.455043 authentik_client-2024.4.2.post1715100402/authentik_client/models/system_info.py
+-rw-r--r--   0        0        0     2934 2024-05-07 16:46:55.459043 authentik_client-2024.4.2.post1715100402/authentik_client/models/system_info_runtime.py
+-rw-r--r--   0        0        0     4701 2024-05-07 16:46:55.463043 authentik_client-2024.4.2.post1715100402/authentik_client/models/system_task.py
+-rw-r--r--   0        0        0      789 2024-05-07 16:46:55.467043 authentik_client-2024.4.2.post1715100402/authentik_client/models/system_task_status_enum.py
+-rw-r--r--   0        0        0     2872 2024-05-07 16:46:55.475043 authentik_client-2024.4.2.post1715100402/authentik_client/models/tenant.py
+-rw-r--r--   0        0        0     2589 2024-05-07 16:46:55.479043 authentik_client-2024.4.2.post1715100402/authentik_client/models/tenant_admin_group_request_request.py
+-rw-r--r--   0        0        0     2705 2024-05-07 16:46:55.479043 authentik_client-2024.4.2.post1715100402/authentik_client/models/tenant_recovery_key_request_request.py
+-rw-r--r--   0        0        0     2599 2024-05-07 16:46:55.483043 authentik_client-2024.4.2.post1715100402/authentik_client/models/tenant_recovery_key_response.py
+-rw-r--r--   0        0        0     2765 2024-05-07 16:46:55.483043 authentik_client-2024.4.2.post1715100402/authentik_client/models/tenant_request.py
+-rw-r--r--   0        0        0     4802 2024-05-07 16:46:55.487043 authentik_client-2024.4.2.post1715100402/authentik_client/models/token.py
+-rw-r--r--   0        0        0     4198 2024-05-07 16:46:55.491042 authentik_client-2024.4.2.post1715100402/authentik_client/models/token_model.py
+-rw-r--r--   0        0        0     4329 2024-05-07 16:46:55.491042 authentik_client-2024.4.2.post1715100402/authentik_client/models/token_request.py
+-rw-r--r--   0        0        0     2521 2024-05-07 16:46:55.495043 authentik_client-2024.4.2.post1715100402/authentik_client/models/token_set_key_request.py
+-rw-r--r--   0        0        0     2494 2024-05-07 16:46:55.499043 authentik_client-2024.4.2.post1715100402/authentik_client/models/token_view.py
+-rw-r--r--   0        0        0     2724 2024-05-07 16:46:55.471042 authentik_client-2024.4.2.post1715100402/authentik_client/models/totp_device.py
+-rw-r--r--   0        0        0     2623 2024-05-07 16:46:55.471042 authentik_client-2024.4.2.post1715100402/authentik_client/models/totp_device_request.py
+-rw-r--r--   0        0        0     3389 2024-05-07 16:46:55.499043 authentik_client-2024.4.2.post1715100402/authentik_client/models/transaction_application_request.py
+-rw-r--r--   0        0        0     2595 2024-05-07 16:46:55.503043 authentik_client-2024.4.2.post1715100402/authentik_client/models/transaction_application_response.py
+-rw-r--r--   0        0        0     2936 2024-05-07 16:46:55.507043 authentik_client-2024.4.2.post1715100402/authentik_client/models/type_create.py
+-rw-r--r--   0        0        0      730 2024-05-07 16:46:55.507043 authentik_client-2024.4.2.post1715100402/authentik_client/models/ui_theme_enum.py
+-rw-r--r--   0        0        0     2808 2024-05-07 16:46:55.511042 authentik_client-2024.4.2.post1715100402/authentik_client/models/used_by.py
+-rw-r--r--   0        0        0      795 2024-05-07 16:46:55.511042 authentik_client-2024.4.2.post1715100402/authentik_client/models/used_by_action_enum.py
+-rw-r--r--   0        0        0     5459 2024-05-07 16:46:55.515043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user.py
+-rw-r--r--   0        0        0     2458 2024-05-07 16:46:55.519043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_account_request.py
+-rw-r--r--   0        0        0     4946 2024-05-07 16:46:55.523043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_assigned_object_permission.py
+-rw-r--r--   0        0        0     3828 2024-05-07 16:46:55.523043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_consent.py
+-rw-r--r--   0        0        0      811 2024-05-07 16:46:55.527042 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_creation_mode_enum.py
+-rw-r--r--   0        0        0     4110 2024-05-07 16:46:55.531043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_delete_stage.py
+-rw-r--r--   0        0        0     3129 2024-05-07 16:46:55.531043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_delete_stage_request.py
+-rw-r--r--   0        0        0      735 2024-05-07 16:46:55.535043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_fields_enum.py
+-rw-r--r--   0        0        0     3909 2024-05-07 16:46:55.535043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_group.py
+-rw-r--r--   0        0        0     3193 2024-05-07 16:46:55.539043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_group_request.py
+-rw-r--r--   0        0        0     4334 2024-05-07 16:46:55.539043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_login_challenge.py
+-rw-r--r--   0        0        0     2805 2024-05-07 16:46:55.543043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_login_challenge_response_request.py
+-rw-r--r--   0        0        0     5631 2024-05-07 16:46:55.543043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_login_stage.py
+-rw-r--r--   0        0        0     4728 2024-05-07 16:46:55.547042 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_login_stage_request.py
+-rw-r--r--   0        0        0     4110 2024-05-07 16:46:55.547042 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_logout_stage.py
+-rw-r--r--   0        0        0     3129 2024-05-07 16:46:55.551043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_logout_stage_request.py
+-rw-r--r--   0        0        0      853 2024-05-07 16:46:55.551043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_matching_mode_enum.py
+-rw-r--r--   0        0        0     4160 2024-05-07 16:46:55.555043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_metrics.py
+-rw-r--r--   0        0        0     3188 2024-05-07 16:46:55.555043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_o_auth_source_connection.py
+-rw-r--r--   0        0        0     3054 2024-05-07 16:46:55.559043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_o_auth_source_connection_request.py
+-rw-r--r--   0        0        0     3293 2024-05-07 16:46:55.563042 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_object_permission.py
+-rw-r--r--   0        0        0     2557 2024-05-07 16:46:55.567042 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_password_set_request.py
+-rw-r--r--   0        0        0     2491 2024-05-07 16:46:55.567042 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_path.py
+-rw-r--r--   0        0        0     3872 2024-05-07 16:46:55.571043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_request.py
+-rw-r--r--   0        0        0     3107 2024-05-07 16:46:55.575043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_saml_source_connection.py
+-rw-r--r--   0        0        0     2668 2024-05-07 16:46:55.579043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_saml_source_connection_request.py
+-rw-r--r--   0        0        0     5465 2024-05-07 16:46:55.583042 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_self.py
+-rw-r--r--   0        0        0     2629 2024-05-07 16:46:55.587043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_self_groups.py
+-rw-r--r--   0        0        0     3074 2024-05-07 16:46:55.587043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_service_account_request.py
+-rw-r--r--   0        0        0     2844 2024-05-07 16:46:55.591043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_service_account_response.py
+-rw-r--r--   0        0        0     2866 2024-05-07 16:46:55.591043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_setting.py
+-rw-r--r--   0        0        0     3245 2024-05-07 16:46:55.595043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_source_connection.py
+-rw-r--r--   0        0        0      817 2024-05-07 16:46:55.595043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_type_enum.py
+-rw-r--r--   0        0        0      777 2024-05-07 16:46:55.599043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_verification_enum.py
+-rw-r--r--   0        0        0     5382 2024-05-07 16:46:55.599043 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_write_stage.py
+-rw-r--r--   0        0        0     4412 2024-05-07 16:46:55.603042 authentik_client-2024.4.2.post1715100402/authentik_client/models/user_write_stage_request.py
+-rw-r--r--   0        0        0     3197 2024-05-07 16:46:55.603042 authentik_client-2024.4.2.post1715100402/authentik_client/models/validation_error.py
+-rw-r--r--   0        0        0     3589 2024-05-07 16:46:55.607043 authentik_client-2024.4.2.post1715100402/authentik_client/models/version.py
+-rw-r--r--   0        0        0     3786 2024-05-07 16:46:55.607043 authentik_client-2024.4.2.post1715100402/authentik_client/models/web_authn_device.py
+-rw-r--r--   0        0        0     2577 2024-05-07 16:46:55.611043 authentik_client-2024.4.2.post1715100402/authentik_client/models/web_authn_device_request.py
+-rw-r--r--   0        0        0     2562 2024-05-07 16:46:55.611043 authentik_client-2024.4.2.post1715100402/authentik_client/models/web_authn_device_type.py
+-rw-r--r--   0        0        0     2669 2024-05-07 16:46:55.615043 authentik_client-2024.4.2.post1715100402/authentik_client/models/web_authn_device_type_request.py
+-rw-r--r--   0        0        0     2410 2024-05-07 16:46:55.615043 authentik_client-2024.4.2.post1715100402/authentik_client/models/workers.py
+-rw-r--r--   0        0        0        0 2024-05-07 16:46:56.731042 authentik_client-2024.4.2.post1715100402/authentik_client/py.typed
+-rw-r--r--   0        0        0     9196 2024-05-07 16:46:56.743042 authentik_client-2024.4.2.post1715100402/authentik_client/rest.py
+-rw-r--r--   0        0        0     1936 2024-05-07 16:46:56.731042 authentik_client-2024.4.2.post1715100402/pyproject.toml
+-rw-r--r--   0        0        0   144925 1970-01-01 00:00:00.000000 authentik_client-2024.4.2.post1715100402/PKG-INFO
```

### Comparing `authentik_client-2024.4.1.post1714957688/README.md` & `authentik_client-2024.4.2.post1715100402/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2024.4.1
-- Package version: 2024.4.1-1714957688
+- API version: 2024.4.2
+- Package version: 2024.4.2-1715100402
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/__init__.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2024.4.1-1714957688"
+__version__ = "2024.4.2-1715100402"
 
 # import apis into sdk package
 from authentik_client.api.admin_api import AdminApi
 from authentik_client.api.authenticators_api import AuthenticatorsApi
 from authentik_client.api.core_api import CoreApi
 from authentik_client.api.crypto_api import CryptoApi
 from authentik_client.api.enterprise_api import EnterpriseApi
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/__init__.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/admin_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/admin_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/authenticators_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/authenticators_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/core_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/core_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/crypto_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/crypto_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/enterprise_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/enterprise_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/events_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/events_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/flows_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/flows_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/managed_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/managed_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/oauth2_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/oauth2_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/outposts_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/outposts_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/policies_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/policies_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/propertymappings_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/propertymappings_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/providers_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/providers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/rac_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/rac_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/rbac_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/rbac_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/root_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/root_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/schema_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/schema_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/sources_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/sources_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/stages_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/stages_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api/tenants_api.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api/tenants_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 import warnings
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api_client.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -84,15 +84,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2024.4.1-1714957688/python'
+        self.user_agent = 'OpenAPI-Generator/2024.4.2-1715100402/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/api_response.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/api_response.py`

 * *Files identical despite different names*

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/configuration.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -374,16 +374,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2024.4.1\n"\
-               "SDK Package Version: 2024.4.1-1714957688".\
+               "Version of the API: 2024.4.2\n"\
+               "SDK Package Version: 2024.4.2-1715100402".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/exceptions.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 from typing import Any, Optional
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/__init__.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/access_denied_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/access_denied_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/alg_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/alg_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/app.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/app_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/app_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/apple_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/apple_challenge_response_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/apple_login_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/apple_login_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/application.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/application_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/application_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/auth_mode_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/auth_mode_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/auth_type_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/auth_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session_asn.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session_asn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session_geo_ip.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session_geo_ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session_user_agent.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session_user_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session_user_agent_device.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session_user_agent_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session_user_agent_os.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session_user_agent_os.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticated_session_user_agent_user_agent.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticated_session_user_agent_user_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authentication_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authentication_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_attachment_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_attachment_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_duo_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_duo_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_duo_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_duo_challenge_response_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_duo_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_duo_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_duo_stage_device_import_response.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_duo_stage_device_import_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_duo_stage_manual_device_import_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_duo_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_duo_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_sms_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_sms_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_sms_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_sms_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_sms_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_sms_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_sms_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_sms_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_static_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_static_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_static_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_static_challenge_response_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_static_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_static_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_static_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_static_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_totp_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_totp_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_totp_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_totp_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_totp_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_totp_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_totp_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_totp_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_validate_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_validate_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_validate_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_validate_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_validation_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_validation_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_validation_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_validation_challenge_response_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_web_authn_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_web_authn_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_web_authn_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_web_authn_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_web_authn_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_web_authn_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/authenticator_web_authn_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/authenticator_web_authn_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/auto_submit_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/auto_submit_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/autosubmit_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/autosubmit_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/backends_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/backends_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/binding_type_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/binding_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/blueprint_file.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/blueprint_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/blueprint_instance.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/blueprint_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/blueprint_instance_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/blueprint_instance_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/blueprint_instance_status_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/blueprint_instance_status_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/brand.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/brand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/brand_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/brand_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/cache.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/capabilities_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/capabilities_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/captcha_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/captcha_challenge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/captcha_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/captcha_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/captcha_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/captcha_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/captcha_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/captcha_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/certificate_data.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/certificate_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/certificate_generation_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/certificate_generation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/certificate_key_pair.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/certificate_key_pair.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/certificate_key_pair_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/certificate_key_pair_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/challenge_choices.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/challenge_choices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/challenge_types.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/challenge_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/client_type_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/client_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/config.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/connection_token.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/connection_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/connection_token_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/connection_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/consent_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/consent_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/consent_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/consent_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/consent_permission.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/consent_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/consent_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/consent_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/consent_stage_mode_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/consent_stage_mode_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/consent_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/consent_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/contextual_flow_info.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/contextual_flow_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/contextual_flow_info_layout_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/contextual_flow_info_layout_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/coordinate.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/coordinate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/current_brand.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/current_brand.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/denied_action_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/denied_action_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/deny_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/deny_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/deny_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/deny_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/device.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/device_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/device_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/device_challenge_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/device_challenge_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/device_classes_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/device_classes_enum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/digest_algorithm_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/digest_algorithm_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/digits_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/digits_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/docker_service_connection.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/docker_service_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/docker_service_connection_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/docker_service_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/domain.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/domain_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/domain_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/dummy_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/dummy_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/dummy_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/dummy_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/dummy_policy.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/dummy_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/dummy_policy_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/dummy_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/dummy_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/dummy_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/dummy_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/dummy_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/duo_device.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/duo_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/duo_device_enrollment_status.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/duo_device_enrollment_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/duo_device_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/duo_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/duo_response_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/duo_response_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/email_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/email_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/email_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/email_challenge_response_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/email_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/email_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/email_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/email_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/endpoint.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/endpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/endpoint_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/endpoint_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/error_detail.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/error_detail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/error_reporting_config.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/error_reporting_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/event.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/event_actions.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/event_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/event_matcher_policy.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/event_matcher_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/event_matcher_policy_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/event_matcher_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/event_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/event_top_per_user.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/event_top_per_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/expiring_base_grant_model.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/expiring_base_grant_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/expression_policy.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/expression_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/expression_policy_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/expression_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/extra_role_object_permission.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/extra_role_object_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/extra_user_object_permission.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/extra_user_object_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/file_path_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/file_path_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_designation_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_designation_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_diagram.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_diagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_error_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_error_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_import_result.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_import_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_inspection.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_inspection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_inspector_plan.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_inspector_plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_layout_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_layout_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_set.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_set_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_set_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_stage_binding.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_stage_binding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/flow_stage_binding_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/flow_stage_binding_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/footer_link.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/footer_link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/generic_error.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/generic_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/geoip_binding_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/geoip_binding_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/group.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/group_member.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/group_member.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/group_member_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/group_member_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/group_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/identification_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/identification_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/identification_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/identification_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/identification_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/identification_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/identification_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/identification_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/install_id.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/install_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/intent_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/intent_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/invalid_response_action_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/invalid_response_action_enum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/invitation.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/invitation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/invitation_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/invitation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/invitation_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/invitation_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/invitation_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/invitation_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/issuer_mode_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/issuer_mode_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/kubernetes_service_connection.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/kubernetes_service_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/kubernetes_service_connection_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/kubernetes_service_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_debug.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_outpost_config.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_outpost_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_property_mapping.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_property_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_property_mapping_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_property_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_provider.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_source.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_source_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/ldap_sync_status.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/ldap_sync_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/ldapapi_access_mode.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/ldapapi_access_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/license.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/license.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/license_forecast.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/license_forecast.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/license_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/license_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/license_summary.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/license_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/link.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/link.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/log_event.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/log_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/log_level_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/log_level_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/login_challenge_types.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/login_challenge_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/login_metrics.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/login_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/login_source.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/login_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/metadata.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/model_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/model_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/model_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/model_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/name_id_policy_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/name_id_policy_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/network_binding_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/network_binding_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/not_configured_action_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/severity_enum.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class NotConfiguredActionEnum(str, Enum):
+class SeverityEnum(str, Enum):
     """
-    NotConfiguredActionEnum
+    SeverityEnum
     """
 
     """
     allowed enum values
     """
-    SKIP = 'skip'
-    DENY = 'deny'
-    CONFIGURE = 'configure'
+    NOTICE = 'notice'
+    WARNING = 'warning'
+    ALERT = 'alert'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of NotConfiguredActionEnum from a JSON string"""
+        """Create an instance of SeverityEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/notification.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_rule.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_rule_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_rule_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_transport.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_transport_mode_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_transport_mode_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_transport_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_transport_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_transport_test.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_transport_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_webhook_mapping.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_webhook_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/notification_webhook_mapping_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/notification_webhook_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth2_provider.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth2_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth2_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth2_provider_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth2_provider_setup_urls.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth2_provider_setup_urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth_device_code_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth_device_code_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth_device_code_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth_device_code_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth_device_code_finish_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth_device_code_finish_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth_device_code_finish_challenge_response_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth_source.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/o_auth_source_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/o_auth_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/open_id_connect_configuration.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/open_id_connect_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/outpost.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/outpost.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/outpost_default_config.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/outpost_default_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/outpost_health.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/outpost_health.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/outpost_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/outpost_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/outpost_type_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/not_configured_action_enum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class OutpostTypeEnum(str, Enum):
+class NotConfiguredActionEnum(str, Enum):
     """
-    OutpostTypeEnum
+    NotConfiguredActionEnum
     """
 
     """
     allowed enum values
     """
-    PROXY = 'proxy'
-    LDAP = 'ldap'
-    RADIUS = 'radius'
-    RAC = 'rac'
+    SKIP = 'skip'
+    DENY = 'deny'
+    CONFIGURE = 'configure'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of OutpostTypeEnum from a JSON string"""
+        """Create an instance of NotConfiguredActionEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_application_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_application_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticated_session_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticated_session_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticator_duo_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticator_duo_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticator_sms_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticator_sms_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticator_static_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticator_static_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticator_totp_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticator_totp_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticator_validate_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticator_validate_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_authenticator_web_authn_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_authenticator_web_authn_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_blueprint_instance_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_blueprint_instance_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_brand_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_brand_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_captcha_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_captcha_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_certificate_key_pair_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_certificate_key_pair_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_connection_token_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_connection_token_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_consent_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_consent_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_deny_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_deny_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_docker_service_connection_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_docker_service_connection_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_domain_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_domain_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_dummy_policy_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_dummy_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_dummy_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_dummy_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_duo_device_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_duo_device_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_email_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_email_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_endpoint_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_endpoint_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_event_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_event_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_event_matcher_policy_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_event_matcher_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_expiring_base_grant_model_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_expiring_base_grant_model_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_expression_policy_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_expression_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_extra_role_object_permission_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_extra_role_object_permission_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_extra_user_object_permission_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_extra_user_object_permission_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_flow_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_flow_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_flow_stage_binding_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_flow_stage_binding_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_group_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_group_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_identification_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_identification_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_invitation_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_invitation_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_invitation_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_invitation_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_kubernetes_service_connection_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_kubernetes_service_connection_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_ldap_outpost_config_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_ldap_outpost_config_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_ldap_property_mapping_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_ldap_property_mapping_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_ldap_provider_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_ldap_provider_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_ldap_source_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_ldap_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_license_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_license_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_notification_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_notification_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_notification_rule_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_system_task_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
-from authentik_client.models.notification_rule import NotificationRule
 from authentik_client.models.pagination import Pagination
+from authentik_client.models.system_task import SystemTask
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedNotificationRuleList(BaseModel):
+class PaginatedSystemTaskList(BaseModel):
     """
-    PaginatedNotificationRuleList
+    PaginatedSystemTaskList
     """ # noqa: E501
     pagination: Pagination
-    results: List[NotificationRule]
+    results: List[SystemTask]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedNotificationRuleList from a JSON string"""
+        """Create an instance of PaginatedSystemTaskList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedNotificationRuleList from a dict"""
+        """Create an instance of PaginatedSystemTaskList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [NotificationRule.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [SystemTask.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_notification_transport_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_notification_transport_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_notification_webhook_mapping_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_notification_webhook_mapping_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_o_auth2_provider_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_o_auth2_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_o_auth_source_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_o_auth_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_outpost_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_outpost_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_password_expiry_policy_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_password_expiry_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_password_policy_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_password_policy_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_password_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_password_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_permission_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_permission_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_plex_source_connection_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_plex_source_connection_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_plex_source_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_plex_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_policy_binding_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_policy_binding_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_policy_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_policy_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_prompt_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_prompt_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_prompt_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_prompt_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_property_mapping_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_property_mapping_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_provider_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_provider_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_proxy_outpost_config_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_proxy_outpost_config_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_proxy_provider_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_proxy_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_rac_property_mapping_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_rac_property_mapping_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_rac_provider_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_rac_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_radius_outpost_config_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_radius_outpost_config_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_radius_provider_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_radius_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_reputation_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_reputation_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_reputation_policy_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_reputation_policy_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_role_assigned_object_permission_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_role_assigned_object_permission_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_role_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_role_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_saml_property_mapping_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_saml_property_mapping_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_saml_provider_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_saml_provider_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_saml_source_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_saml_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_scim_mapping_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_scim_mapping_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_scim_provider_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_scim_provider_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_scim_source_group_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_scim_source_group_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_scim_source_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_scim_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_scim_source_user_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_scim_source_user_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_scope_mapping_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_scope_mapping_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_service_connection_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_service_connection_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_sms_device_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_sms_device_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_source_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_source_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_source_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_source_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_stage_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_static_device_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_static_device_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_system_task_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,24 +17,24 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
 from authentik_client.models.pagination import Pagination
-from authentik_client.models.system_task import SystemTask
+from authentik_client.models.user import User
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedSystemTaskList(BaseModel):
+class PaginatedUserList(BaseModel):
     """
-    PaginatedSystemTaskList
+    PaginatedUserList
     """ # noqa: E501
     pagination: Pagination
-    results: List[SystemTask]
+    results: List[User]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedSystemTaskList from a JSON string"""
+        """Create an instance of PaginatedUserList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedSystemTaskList from a dict"""
+        """Create an instance of PaginatedUserList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [SystemTask.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [User.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_tenant_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_tenant_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_token_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_token_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_token_model_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_token_model_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_totp_device_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_totp_device_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_assigned_object_permission_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_assigned_object_permission_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_consent_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_consent_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_delete_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_delete_stage_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_write_stage_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,24 +17,24 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
 from authentik_client.models.pagination import Pagination
-from authentik_client.models.user import User
+from authentik_client.models.user_write_stage import UserWriteStage
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedUserList(BaseModel):
+class PaginatedUserWriteStageList(BaseModel):
     """
-    PaginatedUserList
+    PaginatedUserWriteStageList
     """ # noqa: E501
     pagination: Pagination
-    results: List[User]
+    results: List[UserWriteStage]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedUserList from a JSON string"""
+        """Create an instance of PaginatedUserWriteStageList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedUserList from a dict"""
+        """Create an instance of PaginatedUserWriteStageList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [User.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [UserWriteStage.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_login_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_login_stage_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_logout_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_logout_stage_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_o_auth_source_connection_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_o_auth_source_connection_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_saml_source_connection_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_saml_source_connection_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_source_connection_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_user_source_connection_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_user_write_stage_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_web_authn_device_type_list.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -17,24 +17,24 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
 from authentik_client.models.pagination import Pagination
-from authentik_client.models.user_write_stage import UserWriteStage
+from authentik_client.models.web_authn_device_type import WebAuthnDeviceType
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedUserWriteStageList(BaseModel):
+class PaginatedWebAuthnDeviceTypeList(BaseModel):
     """
-    PaginatedUserWriteStageList
+    PaginatedWebAuthnDeviceTypeList
     """ # noqa: E501
     pagination: Pagination
-    results: List[UserWriteStage]
+    results: List[WebAuthnDeviceType]
     __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
@@ -47,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedUserWriteStageList from a JSON string"""
+        """Create an instance of PaginatedWebAuthnDeviceTypeList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -82,21 +82,21 @@
                 if _item:
                     _items.append(_item.to_dict())
             _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedUserWriteStageList from a dict"""
+        """Create an instance of PaginatedWebAuthnDeviceTypeList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [UserWriteStage.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "results": [WebAuthnDeviceType.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_web_authn_device_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_web_authn_device_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/paginated_web_authn_device_type_list.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/transaction_application_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
 from typing import Any, ClassVar, Dict, List
-from authentik_client.models.pagination import Pagination
-from authentik_client.models.web_authn_device_type import WebAuthnDeviceType
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PaginatedWebAuthnDeviceTypeList(BaseModel):
+class TransactionApplicationResponse(BaseModel):
     """
-    PaginatedWebAuthnDeviceTypeList
+    Transactional creation response
     """ # noqa: E501
-    pagination: Pagination
-    results: List[WebAuthnDeviceType]
-    __properties: ClassVar[List[str]] = ["pagination", "results"]
+    applied: StrictBool
+    logs: List[StrictStr]
+    __properties: ClassVar[List[str]] = ["applied", "logs"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PaginatedWebAuthnDeviceTypeList from a JSON string"""
+        """Create an instance of TransactionApplicationResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -68,35 +66,25 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of pagination
-        if self.pagination:
-            _dict['pagination'] = self.pagination.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in results (list)
-        _items = []
-        if self.results:
-            for _item in self.results:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PaginatedWebAuthnDeviceTypeList from a dict"""
+        """Create an instance of TransactionApplicationResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
-            "results": [WebAuthnDeviceType.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
+            "applied": obj.get("applied"),
+            "logs": obj.get("logs")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/pagination.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/pagination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/password_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/password_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/password_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/password_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/password_expiry_policy.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/password_expiry_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/password_expiry_policy_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/password_expiry_policy_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/password_policy.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/password_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/password_policy_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/password_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/password_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/password_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/password_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/password_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_application_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_application_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_authenticator_duo_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_authenticator_duo_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_authenticator_sms_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_authenticator_sms_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_authenticator_static_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_authenticator_static_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_authenticator_totp_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_authenticator_totp_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_authenticator_validate_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_authenticator_validate_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_authenticator_web_authn_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_authenticator_web_authn_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_blueprint_instance_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_blueprint_instance_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_brand_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_brand_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_captcha_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_captcha_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_certificate_key_pair_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_certificate_key_pair_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_connection_token_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_connection_token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_consent_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_consent_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_deny_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_deny_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_docker_service_connection_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_docker_service_connection_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_domain_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_domain_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_dummy_policy_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_dummy_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_dummy_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_dummy_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_duo_device_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_duo_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_email_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_email_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_endpoint_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_endpoint_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_event_matcher_policy_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_event_matcher_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_event_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_event_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_expression_policy_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_expression_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_flow_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_flow_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_flow_stage_binding_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_flow_stage_binding_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_group_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_identification_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_identification_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_invitation_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_invitation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_invitation_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_invitation_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_kubernetes_service_connection_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_kubernetes_service_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_ldap_property_mapping_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_ldap_property_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_ldap_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_ldap_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_ldap_source_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_ldap_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_license_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_license_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_notification_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_notification_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_notification_rule_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_notification_rule_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_notification_transport_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_notification_transport_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_notification_webhook_mapping_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_notification_webhook_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_o_auth2_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_o_auth2_provider_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_o_auth_source_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_o_auth_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_outpost_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_outpost_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_password_expiry_policy_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_password_expiry_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_password_policy_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_password_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_password_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_password_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_permission_assign_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_permission_assign_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_plex_source_connection_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_plex_source_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_plex_source_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_plex_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_policy_binding_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_policy_binding_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_prompt_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_prompt_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_prompt_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_prompt_stage_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_proxy_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_proxy_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_rac_property_mapping_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_rac_property_mapping_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_rac_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_rac_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_radius_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_radius_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_reputation_policy_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_reputation_policy_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_role_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_role_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_saml_property_mapping_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_saml_property_mapping_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_saml_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_saml_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_saml_source_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_saml_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_scim_mapping_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_scim_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_scim_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_scim_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_scim_source_group_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_scim_source_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_scim_source_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_scim_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_scim_source_user_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_scim_source_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_scope_mapping_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/scope_mapping_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -20,22 +20,22 @@
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class PatchedScopeMappingRequest(BaseModel):
+class ScopeMappingRequest(BaseModel):
     """
     ScopeMapping Serializer
     """ # noqa: E501
     managed: Optional[Annotated[str, Field(min_length=1, strict=True)]] = Field(default=None, description="Objects that are managed by authentik. These objects are created and updated automatically. This flag only indicates that an object can be overwritten by migrations. You can still modify the objects via the API, but expect changes to be overwritten in a later update.")
-    name: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
-    expression: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
-    scope_name: Optional[Annotated[str, Field(min_length=1, strict=True)]] = Field(default=None, description="Scope name requested by the client")
+    name: Annotated[str, Field(min_length=1, strict=True)]
+    expression: Annotated[str, Field(min_length=1, strict=True)]
+    scope_name: Annotated[str, Field(min_length=1, strict=True)] = Field(description="Scope name requested by the client")
     description: Optional[StrictStr] = Field(default=None, description="Description shown to the user when consenting. If left empty, the user won't be informed.")
     __properties: ClassVar[List[str]] = ["managed", "name", "expression", "scope_name", "description"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -49,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of PatchedScopeMappingRequest from a JSON string"""
+        """Create an instance of ScopeMappingRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -79,15 +79,15 @@
         if self.managed is None and "managed" in self.model_fields_set:
             _dict['managed'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of PatchedScopeMappingRequest from a dict"""
+        """Create an instance of ScopeMappingRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_settings_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_sms_device_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_sms_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_source_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_source_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_static_device_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_static_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_tenant_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_tenant_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_token_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_token_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_totp_device_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_totp_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_delete_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_delete_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_login_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_login_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_logout_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_logout_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_o_auth_source_connection_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_o_auth_source_connection_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_saml_source_connection_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_saml_source_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_user_write_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_user_write_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/patched_web_authn_device_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_web_authn_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/permission.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/permission_assign_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/permission_assign_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_authentication_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_authentication_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_authentication_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_authentication_challenge_response_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_source.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_source_connection.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_source_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_source_connection_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_source_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_source_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/plex_token_redeem_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/plex_token_redeem_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/policy.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/policy_binding.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/policy_binding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/policy_binding_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/policy_binding_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/policy_engine_mode.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/policy_engine_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/policy_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/policy_test_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/policy_test_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/policy_test_result.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/policy_test_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/prompt_type_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/prompt_type_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/property_mapping.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/property_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/property_mapping_preview.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/property_mapping_preview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/property_mapping_test_result.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/property_mapping_test_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/protocol_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/protocol_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/provider.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/provider_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/provider_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/provider_model_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/provider_model_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/provider_type_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/provider_type_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/proxy_mode.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/proxy_mode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/proxy_outpost_config.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/proxy_outpost_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/proxy_provider.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/proxy_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/proxy_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/proxy_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/rac_property_mapping.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/rac_property_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/rac_property_mapping_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/rac_property_mapping_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/rac_provider.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/rac_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/rac_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/rac_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/radius_outpost_config.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/radius_outpost_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/radius_provider.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/radius_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/radius_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/radius_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/redirect_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/redirect_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/reputation.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/reputation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/reputation_policy.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/reputation_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/reputation_policy_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/reputation_policy_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/resident_key_requirement_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/resident_key_requirement_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/role.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/role_assigned_object_permission.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/role_assigned_object_permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/role_object_permission.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/role_object_permission.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/role_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/role_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_metadata.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_property_mapping.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_property_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_property_mapping_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_property_mapping_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_provider.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_source.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/saml_source_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/saml_source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_mapping.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_mapping_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_mapping_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_provider.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_provider_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_provider_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_source.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_source_group.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_source_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_source_group_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_source_group_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_source_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_source_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_source_user.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_source_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_source_user_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_source_user_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/scim_sync_status.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/scim_sync_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/scope_mapping.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/scope_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/scope_mapping_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/patched_scope_mapping_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -20,22 +20,22 @@
 
 from pydantic import BaseModel, ConfigDict, Field, StrictStr
 from typing import Any, ClassVar, Dict, List, Optional
 from typing_extensions import Annotated
 from typing import Optional, Set
 from typing_extensions import Self
 
-class ScopeMappingRequest(BaseModel):
+class PatchedScopeMappingRequest(BaseModel):
     """
     ScopeMapping Serializer
     """ # noqa: E501
     managed: Optional[Annotated[str, Field(min_length=1, strict=True)]] = Field(default=None, description="Objects that are managed by authentik. These objects are created and updated automatically. This flag only indicates that an object can be overwritten by migrations. You can still modify the objects via the API, but expect changes to be overwritten in a later update.")
-    name: Annotated[str, Field(min_length=1, strict=True)]
-    expression: Annotated[str, Field(min_length=1, strict=True)]
-    scope_name: Annotated[str, Field(min_length=1, strict=True)] = Field(description="Scope name requested by the client")
+    name: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
+    expression: Optional[Annotated[str, Field(min_length=1, strict=True)]] = None
+    scope_name: Optional[Annotated[str, Field(min_length=1, strict=True)]] = Field(default=None, description="Scope name requested by the client")
     description: Optional[StrictStr] = Field(default=None, description="Description shown to the user when consenting. If left empty, the user won't be informed.")
     __properties: ClassVar[List[str]] = ["managed", "name", "expression", "scope_name", "description"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
@@ -49,15 +49,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of ScopeMappingRequest from a JSON string"""
+        """Create an instance of PatchedScopeMappingRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -79,15 +79,15 @@
         if self.managed is None and "managed" in self.model_fields_set:
             _dict['managed'] = None
 
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of ScopeMappingRequest from a dict"""
+        """Create an instance of PatchedScopeMappingRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/selectable_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/selectable_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/service_connection.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/service_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/service_connection_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/service_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/service_connection_state.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/service_connection_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/session_user.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/session_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/settings.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/settings_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/settings_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/severity_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/ui_theme_enum.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class SeverityEnum(str, Enum):
+class UiThemeEnum(str, Enum):
     """
-    SeverityEnum
+    UiThemeEnum
     """
 
     """
     allowed enum values
     """
-    NOTICE = 'notice'
-    WARNING = 'warning'
-    ALERT = 'alert'
+    AUTOMATIC = 'automatic'
+    LIGHT = 'light'
+    DARK = 'dark'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of SeverityEnum from a JSON string"""
+        """Create an instance of UiThemeEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/shell_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/shell_challenge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/signature_algorithm_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/signature_algorithm_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/sms_device.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/sms_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/sms_device_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/sms_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/source.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/source_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/source_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/source_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/source_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/source_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/source_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/source_type.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/source_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/sp_binding_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/sp_binding_enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/stage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/stage_prompt.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/stage_prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/static_device.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/static_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/static_device_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/static_device_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/static_device_token.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/static_device_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/static_device_token_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/static_device_token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/sub_mode_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/sub_mode_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/system_info.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/system_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/system_info_runtime.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/system_info_runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/system_task.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/system_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/system_task_status_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/system_task_status_enum.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/tenant.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/tenant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/tenant_admin_group_request_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/tenant_admin_group_request_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/tenant_recovery_key_request_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/tenant_recovery_key_request_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/tenant_recovery_key_response.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/tenant_recovery_key_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/tenant_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/tenant_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/token.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/token_model.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/token_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/token_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/token_set_key_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/token_set_key_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/token_view.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/token_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/totp_device.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/totp_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/totp_device_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/totp_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/transaction_application_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/transaction_application_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/transaction_application_response.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_path.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictBool, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictStr
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class TransactionApplicationResponse(BaseModel):
+class UserPath(BaseModel):
     """
-    Transactional creation response
+    UserPath
     """ # noqa: E501
-    applied: StrictBool
-    logs: List[StrictStr]
-    __properties: ClassVar[List[str]] = ["applied", "logs"]
+    paths: List[StrictStr]
+    __properties: ClassVar[List[str]] = ["paths"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -45,46 +44,47 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of TransactionApplicationResponse from a JSON string"""
+        """Create an instance of UserPath from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
+        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
+            "paths",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of TransactionApplicationResponse from a dict"""
+        """Create an instance of UserPath from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "applied": obj.get("applied"),
-            "logs": obj.get("logs")
+            "paths": obj.get("paths")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/type_create.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/type_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/ui_theme_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_type_enum.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class UiThemeEnum(str, Enum):
+class UserTypeEnum(str, Enum):
     """
-    UiThemeEnum
+    UserTypeEnum
     """
 
     """
     allowed enum values
     """
-    AUTOMATIC = 'automatic'
-    LIGHT = 'light'
-    DARK = 'dark'
+    INTERNAL = 'internal'
+    EXTERNAL = 'external'
+    SERVICE_ACCOUNT = 'service_account'
+    INTERNAL_SERVICE_ACCOUNT = 'internal_service_account'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of UiThemeEnum from a JSON string"""
+        """Create an instance of UserTypeEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/used_by.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/used_by.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/used_by_action_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/used_by_action_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_account_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_account_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_assigned_object_permission.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_assigned_object_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_consent.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_consent.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_creation_mode_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_creation_mode_enum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_delete_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_delete_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_delete_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_delete_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_fields_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_fields_enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_group.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_group_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_group_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_login_challenge.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_login_challenge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_login_challenge_response_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_login_challenge_response_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_login_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_login_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_login_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_login_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_logout_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_logout_stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_logout_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_logout_stage_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_matching_mode_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_matching_mode_enum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_metrics.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_o_auth_source_connection.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_o_auth_source_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_o_auth_source_connection_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_o_auth_source_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_object_permission.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_object_permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_password_set_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_password_set_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_path.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/workers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictStr
+from pydantic import BaseModel, ConfigDict, StrictInt
 from typing import Any, ClassVar, Dict, List
 from typing import Optional, Set
 from typing_extensions import Self
 
-class UserPath(BaseModel):
+class Workers(BaseModel):
     """
-    UserPath
+    Workers
     """ # noqa: E501
-    paths: List[StrictStr]
-    __properties: ClassVar[List[str]] = ["paths"]
+    count: StrictInt
+    __properties: ClassVar[List[str]] = ["count"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,47 +44,45 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of UserPath from a JSON string"""
+        """Create an instance of Workers from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
 
         * `None` is only added to the output dict for nullable fields that
           were set at model initialization. Other fields with value `None`
           are ignored.
-        * OpenAPI `readOnly` fields are excluded.
         """
         excluded_fields: Set[str] = set([
-            "paths",
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of UserPath from a dict"""
+        """Create an instance of Workers from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "paths": obj.get("paths")
+            "count": obj.get("count")
         })
         return _obj
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_saml_source_connection.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_saml_source_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_saml_source_connection_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_saml_source_connection_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_self.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_self.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_self_groups.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_self_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_service_account_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_service_account_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_service_account_response.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_service_account_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_setting.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_setting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_source_connection.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_source_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_type_enum.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_verification_enum.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import json
 from enum import Enum
 from typing_extensions import Self
 
 
-class UserTypeEnum(str, Enum):
+class UserVerificationEnum(str, Enum):
     """
-    UserTypeEnum
+    UserVerificationEnum
     """
 
     """
     allowed enum values
     """
-    INTERNAL = 'internal'
-    EXTERNAL = 'external'
-    SERVICE_ACCOUNT = 'service_account'
-    INTERNAL_SERVICE_ACCOUNT = 'internal_service_account'
+    REQUIRED = 'required'
+    PREFERRED = 'preferred'
+    DISCOURAGED = 'discouraged'
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of UserTypeEnum from a JSON string"""
+        """Create an instance of UserVerificationEnum from a JSON string"""
         return cls(json.loads(json_str))
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_write_stage.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_write_stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/user_write_stage_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/user_write_stage_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/validation_error.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/version.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/web_authn_device.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/web_authn_device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/web_authn_device_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/web_authn_device_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/web_authn_device_type.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/web_authn_device_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/web_authn_device_type_request.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/web_authn_device_type_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/models/workers.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/models/paginated_notification_rule_list.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, StrictInt
+from pydantic import BaseModel, ConfigDict
 from typing import Any, ClassVar, Dict, List
+from authentik_client.models.notification_rule import NotificationRule
+from authentik_client.models.pagination import Pagination
 from typing import Optional, Set
 from typing_extensions import Self
 
-class Workers(BaseModel):
+class PaginatedNotificationRuleList(BaseModel):
     """
-    Workers
+    PaginatedNotificationRuleList
     """ # noqa: E501
-    count: StrictInt
-    __properties: ClassVar[List[str]] = ["count"]
+    pagination: Pagination
+    results: List[NotificationRule]
+    __properties: ClassVar[List[str]] = ["pagination", "results"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -44,15 +47,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of Workers from a JSON string"""
+        """Create an instance of PaginatedNotificationRuleList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -65,24 +68,35 @@
         ])
 
         _dict = self.model_dump(
             by_alias=True,
             exclude=excluded_fields,
             exclude_none=True,
         )
+        # override the default output from pydantic by calling `to_dict()` of pagination
+        if self.pagination:
+            _dict['pagination'] = self.pagination.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in results (list)
+        _items = []
+        if self.results:
+            for _item in self.results:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['results'] = _items
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of Workers from a dict"""
+        """Create an instance of PaginatedNotificationRuleList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "count": obj.get("count")
+            "pagination": Pagination.from_dict(obj["pagination"]) if obj.get("pagination") is not None else None,
+            "results": [NotificationRule.from_dict(_item) for _item in obj["results"]] if obj.get("results") is not None else None
         })
         return _obj
```

### Comparing `authentik_client-2024.4.1.post1714957688/authentik_client/rest.py` & `authentik_client-2024.4.2.post1715100402/authentik_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     authentik
 
     Making authentication simple.
 
-    The version of the OpenAPI document: 2024.4.1
+    The version of the OpenAPI document: 2024.4.2
     Contact: hello@goauthentik.io
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `authentik_client-2024.4.1.post1714957688/pyproject.toml` & `authentik_client-2024.4.2.post1715100402/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "authentik_client"
-version = "2024.4.1-1714957688"
+version = "2024.4.2-1715100402"
 description = "authentik"
 authors = ["authentik Team <hello@goauthentik.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/goauthentik/authentik"
 keywords = ["OpenAPI", "OpenAPI-Generator", "authentik"]
 include = ["authentik_client/py.typed"]
```

### Comparing `authentik_client-2024.4.1.post1714957688/PKG-INFO` & `authentik_client-2024.4.2.post1715100402/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authentik_client
-Version: 2024.4.1.post1714957688
+Version: 2024.4.2.post1715100402
 Summary: authentik
 Home-page: https://github.com/goauthentik/authentik
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,authentik
 Author: authentik Team
 Author-email: hello@goauthentik.io
 Requires-Python: >=3.7,<4.0
@@ -24,16 +24,16 @@
 Description-Content-Type: text/markdown
 
 # authentik-client
 Making authentication simple.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2024.4.1
-- Package version: 2024.4.1-1714957688
+- API version: 2024.4.2
+- Package version: 2024.4.2-1715100402
 - Generator version: 7.4.0
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 
 ## Requirements.
 
 Python 3.7+
```

