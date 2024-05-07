# Comparing `tmp/ofscraper-3.9.4.tar.gz` & `tmp/ofscraper-3.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-3.9.4.tar", max compression
+gzip compressed data, was "ofscraper-3.9.5.tar", max compression
```

## Comparing `ofscraper-3.9.4.tar` & `ofscraper-3.9.5.tar`

### file list

```diff
@@ -1,188 +1,205 @@
--rw-r--r--   0        0        0     1067 2024-04-27 15:37:09.008659 ofscraper-3.9.4/LICENSE
--rw-r--r--   0        0        0     4213 2024-04-27 15:37:09.008659 ofscraper-3.9.4/README.md
--rwxr-xr-x   0        0        0      283 2024-04-27 15:37:09.012659 ofscraper-3.9.4/ofscraper/__main__.py
--rw-r--r--   0        0        0     1064 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/__version__.pye
--rw-r--r--   0        0        0        1 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/actions/__init__.py
--rw-r--r--   0        0        0     8505 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/actions/like.py
--rw-r--r--   0        0        0    10057 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/actions/process.py
--rw-r--r--   0        0        0    21651 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/actions/scraper.py
--rw-r--r--   0        0        0    15624 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/archive.py
--rw-r--r--   0        0        0      274 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/common/logs.py
--rw-r--r--   0        0        0    14646 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1479 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/init.py
--rw-r--r--   0        0        0    14203 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/labels.py
--rw-r--r--   0        0        0     2912 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/me.py
--rw-r--r--   0        0        0    18946 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/messages.py
--rw-r--r--   0        0        0    13861 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/paid.py
--rw-r--r--   0        0        0     8091 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     6180 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/profile.py
--rw-r--r--   0        0        0     1718 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/subscriptions/helpers.py
--rw-r--r--   0        0        0     3275 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/subscriptions/individual.py
--rw-r--r--   0        0        0    12660 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/subscriptions/lists.py
--rw-r--r--   0        0        0     8171 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/subscriptions/subscriptions.py
--rw-r--r--   0        0        0    16613 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     1460 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/base.py
--rw-r--r--   0        0        0      876 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/labels.py
--rw-r--r--   0        0        0    15560 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/media.py
--rw-r--r--   0        0        0     6005 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/models.py
--rw-r--r--   0        0        0     1771 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/multiprocessprogress.py
--rw-r--r--   0        0        0    20557 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     5156 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/posts.py
--rw-r--r--   0        0        0    18324 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/sessionmanager.py
--rw-r--r--   0        0        0    31979 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/classes/table.py
--rw-r--r--   0        0        0    26079 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/commands/check.py
--rw-r--r--   0        0        0    11014 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/commands/manual.py
--rw-r--r--   0        0        0      430 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/commands/picker.py
--rwxr-xr-x   0        0        0     3810 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0       53 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/binary.py
--rw-r--r--   0        0        0     1655 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/config.py
--rw-r--r--   0        0        0      966 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/constants.py
--rw-r--r--   0        0        0       74 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/date.py
--rw-r--r--   0        0        0      190 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/download.py
--rw-r--r--   0        0        0      204 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/files.py
--rw-r--r--   0        0        0     1333 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/general.py
--rw-r--r--   0        0        0       93 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/logger.py
--rw-r--r--   0        0        0       69 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/metadata.py
--rw-r--r--   0        0        0      862 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/other_url.py
--rw-r--r--   0        0        0     1908 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/prompts.py
--rw-r--r--   0        0        0     1804 2024-04-27 15:37:09.016659 ofscraper-3.9.4/ofscraper/const/req.py
--rw-r--r--   0        0        0   265533 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/const/test_constants.py
--rw-r--r--   0        0        0      248 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/const/time.py
--rw-r--r--   0        0        0     3594 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/const/url.py
--rw-r--r--   0        0        0        1 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    15585 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations.py
--rw-r--r--   0        0        0      206 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/helpers.py
--rw-r--r--   0        0        0     8568 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/labels.py
--rw-r--r--   0        0        0    19112 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/media.py
--rw-r--r--   0        0        0    11270 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/merge.py
--rw-r--r--   0        0        0     8504 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/messages.py
--rw-r--r--   0        0        0     8928 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/others.py
--rw-r--r--   0        0        0    10366 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/posts.py
--rw-r--r--   0        0        0     6725 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/profile.py
--rw-r--r--   0        0        0     7485 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/stories.py
--rw-r--r--   0        0        0     4810 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/db/operations_/wrapper.py
--rw-r--r--   0        0        0    10881 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/alt_download.py
--rw-r--r--   0        0        0    10682 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/alt_downloadbatch.py
--rw-r--r--   0        0        0     4930 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/download.py
--rw-r--r--   0        0        0    17167 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/downloadbatch.py
--rw-r--r--   0        0        0     9077 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/downloadnormal.py
--rw-r--r--   0        0        0    10787 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/main_download.py
--rw-r--r--   0        0        0    11235 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/main_downloadbatch.py
--rw-r--r--   0        0        0     1414 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/classes/retries.py
--rw-r--r--   0        0        0     1356 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/classes/session.py
--rw-r--r--   0        0        0     3796 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/common/alt_common.py
--rw-r--r--   0        0        0     6372 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/common/general.py
--rw-r--r--   0        0        0     2063 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/common/main_common.py
--rw-r--r--   0        0        0     2341 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/globals.py
--rw-r--r--   0        0        0     9440 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/keyhelpers.py
--rw-r--r--   0        0        0     3431 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/log.py
--rw-r--r--   0        0        0      317 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/media.py
--rw-r--r--   0        0        0      790 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/message.py
--rw-r--r--   0        0        0     3927 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/metadata.py
--rw-r--r--   0        0        0     2590 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/paths.py
--rw-r--r--   0        0        0      453 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/progress.py
--rw-r--r--   0        0        0     1155 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/download/shared/utils/text.py
--rw-r--r--   0        0        0     8075 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/media/helpers.py
--rw-r--r--   0        0        0     5019 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/media/main.py
--rw-r--r--   0        0        0     3136 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/date.py
--rw-r--r--   0        0        0     3143 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/flags.py
--rw-r--r--   0        0        0      957 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/helpers.py
--rw-r--r--   0        0        0      726 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/other.py
--rw-r--r--   0        0        0     7561 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/price.py
--rw-r--r--   0        0        0     1538 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/sort.py
--rw-r--r--   0        0        0     1454 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/filters/models/subtype.py
--rw-r--r--   0        0        0     3457 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/models/retriver.py
--rw-r--r--   0        0        0     8011 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/models/selector.py
--rw-r--r--   0        0        0     2466 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/helpers/model_helpers.py
--rw-r--r--   0        0        0    15219 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/helpers/prompt_helpers.py
--rw-r--r--   0        0        0      846 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     7747 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0      917 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/actions.py
--rw-r--r--   0        0        0     6595 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/area.py
--rw-r--r--   0        0        0     8257 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/auth.py
--rw-r--r--   0        0        0     4438 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/binary.py
--rw-r--r--   0        0        0    27915 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/config.py
--rw-r--r--   0        0        0     1879 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/menu.py
--rw-r--r--   0        0        0     2740 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/merge.py
--rw-r--r--   0        0        0    16090 2024-04-27 15:37:09.020659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/model.py
--rw-r--r--   0        0        0     4135 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/prompts/prompt_groups/profile.py
--rw-r--r--   0        0        0     7609 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    10346 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0     1342 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      567 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/runner/exit.py
--rw-r--r--   0        0        0     1578 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/runner/load.py
--rw-r--r--   0        0        0     2743 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/runner/run.py
--rw-r--r--   0        0        0        1 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     3803 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/actions.py
--rw-r--r--   0        0        0     1838 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/areas.py
--rw-r--r--   0        0        0       12 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/globals.py
--rw-r--r--   0        0        0     7512 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/common_args.py
--rw-r--r--   0        0        0    20038 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/main_args.py
--rw-r--r--   0        0        0     1318 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/manual_args.py
--rw-r--r--   0        0        0     1587 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/message_args.py
--rw-r--r--   0        0        0     1588 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/paid_args.py
--rw-r--r--   0        0        0     1955 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/post_args.py
--rw-r--r--   0        0        0     1641 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/groups/story_args.py
--rw-r--r--   0        0        0     5571 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/helpers.py
--rw-r--r--   0        0        0     1928 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/parse.py
--rw-r--r--   0        0        0      395 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/quality.py
--rw-r--r--   0        0        0      863 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/read.py
--rw-r--r--   0        0        0      721 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/user.py
--rw-r--r--   0        0        0      261 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/args/write.py
--rw-r--r--   0        0        0     2148 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/context.py
--rw-r--r--   0        0        0     1680 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/data.py
--rw-r--r--   0        0        0     2034 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/file.py
--rw-r--r--   0        0        0     2844 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/helpers.py
--rw-r--r--   0        0        0     1669 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/make.py
--rw-r--r--   0        0        0     6902 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/request.py
--rw-r--r--   0        0        0      802 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/auth/schema.py
--rw-r--r--   0        0        0     9824 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0     1780 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/cache.py
--rw-r--r--   0        0        0     1612 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/checkers.py
--rw-r--r--   0        0        0     2856 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/config.py
--rw-r--r--   0        0        0     1442 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/context.py
--rw-r--r--   0        0        0      522 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/custom.py
--rw-r--r--   0        0        0    24693 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/data.py
--rw-r--r--   0        0        0     2146 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/file.py
--rw-r--r--   0        0        0     2073 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/menu.py
--rw-r--r--   0        0        0     4797 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/schema.py
--rw-r--r--   0        0        0      409 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/config/wrapper.py
--rw-r--r--   0        0        0      499 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/console.py
--rw-r--r--   0        0        0      788 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/constants.py
--rw-r--r--   0        0        0     3401 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/context/exit.py
--rw-r--r--   0        0        0     1135 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/context/run_async.py
--rw-r--r--   0        0        0     1004 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/context/stdout.py
--rw-r--r--   0        0        0     3460 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/dates.py
--rw-r--r--   0        0        0     1040 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     1781 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/hash.py
--rw-r--r--   0        0        0     7226 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/classes.py
--rw-r--r--   0        0        0     2588 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/close.py
--rw-r--r--   0        0        0      477 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/globals.py
--rw-r--r--   0        0        0     1670 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/helpers.py
--rw-r--r--   0        0        0     2098 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/logger.py
--rw-r--r--   0        0        0     1672 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/logs.py
--rw-r--r--   0        0        0     5955 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/other.py
--rw-r--r--   0        0        0     3652 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/logs/stdout.py
--rw-r--r--   0        0        0      601 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/manager.py
--rw-r--r--   0        0        0      388 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/me.py
--rw-r--r--   0        0        0     4161 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/menu.py
--rw-r--r--   0        0        0      659 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/merge.py
--rw-r--r--   0        0        0     1710 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/paths/check.py
--rw-r--r--   0        0        0     3091 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/paths/common.py
--rw-r--r--   0        0        0      279 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/paths/manage.py
--rw-r--r--   0        0        0     5269 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/paths/paths.py
--rw-r--r--   0        0        0     1034 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/profiles/data.py
--rw-r--r--   0        0        0     2785 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/profiles/manage.py
--rw-r--r--   0        0        0     1583 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/profiles/tools.py
--rw-r--r--   0        0        0    10893 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/progress.py
--rw-r--r--   0        0        0     4406 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/run.py
--rw-r--r--   0        0        0        1 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/sems.py
--rw-r--r--   0        0        0     1595 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     4680 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/settings.py
--rw-r--r--   0        0        0      417 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/system/free.py
--rw-r--r--   0        0        0     3279 2024-04-27 15:37:09.024659 ofscraper-3.9.4/ofscraper/utils/system/network.py
--rw-r--r--   0        0        0     2472 2024-04-27 15:37:09.028659 ofscraper-3.9.4/ofscraper/utils/system/system.py
--rw-r--r--   0        0        0     2002 2024-04-27 15:37:09.028659 ofscraper-3.9.4/ofscraper/utils/text.py
--rw-r--r--   0        0        0     2117 2024-04-27 15:37:34.264635 ofscraper-3.9.4/pyproject.toml
--rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 ofscraper-3.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-07 17:03:44.537793 ofscraper-3.9.5/LICENSE
+-rw-r--r--   0        0        0     4213 2024-05-07 17:03:44.537793 ofscraper-3.9.5/README.md
+-rwxr-xr-x   0        0        0      283 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/__main__.py
+-rw-r--r--   0        0        0     1690 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/__version__.py
+-rw-r--r--   0        0        0     1625 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/__version__.pye
+-rw-r--r--   0        0        0        1 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/actions/__init__.py
+-rw-r--r--   0        0        0     8505 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/actions/like.py
+-rw-r--r--   0        0        0    10057 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/actions/process.py
+-rw-r--r--   0        0        0    21617 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/actions/scraper.py
+-rw-r--r--   0        0        0    16237 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/archive.py
+-rw-r--r--   0        0        0      274 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/common/logs.py
+-rw-r--r--   0        0        0    14697 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1479 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/init.py
+-rw-r--r--   0        0        0    14238 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     2912 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/me.py
+-rw-r--r--   0        0        0    18538 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/messages.py
+-rw-r--r--   0        0        0    13861 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     8717 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     6176 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     1718 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/subscriptions/helpers.py
+-rw-r--r--   0        0        0     3381 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/subscriptions/individual.py
+-rw-r--r--   0        0        0    12660 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/subscriptions/lists.py
+-rw-r--r--   0        0        0     8171 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/subscriptions/subscriptions.py
+-rw-r--r--   0        0        0    17241 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     1460 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/base.py
+-rw-r--r--   0        0        0      876 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0    15560 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     6005 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/models.py
+-rw-r--r--   0        0        0     1771 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/multiprocessprogress.py
+-rw-r--r--   0        0        0    20499 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     5156 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0    18427 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/sessionmanager.py
+-rw-r--r--   0        0        0      156 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/button.py
+-rw-r--r--   0        0        0     1689 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/boolfield.py
+-rw-r--r--   0        0        0     1370 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/datefield.py
+-rw-r--r--   0        0        0      629 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/mediafield.py
+-rw-r--r--   0        0        0      694 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/numfield.py
+-rw-r--r--   0        0        0     1302 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/pricefield.py
+-rw-r--r--   0        0        0      678 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/responsefield.py
+-rw-r--r--   0        0        0     1417 2024-05-07 17:03:44.541793 ofscraper-3.9.5/ofscraper/classes/table/fields/selectfield.py
+-rw-r--r--   0        0        0     1487 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/fields/textsearch.py
+-rw-r--r--   0        0        0     2460 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/fields/timefield.py
+-rw-r--r--   0        0        0     1893 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/inputs/filterinput.py
+-rw-r--r--   0        0        0      117 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/inputs/intergerinput.py
+-rw-r--r--   0        0        0      113 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/inputs/strinput.py
+-rw-r--r--   0        0        0      297 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/row_names.py
+-rw-r--r--   0        0        0     4583 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/status.py
+-rw-r--r--   0        0        0    21258 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/table.py
+-rw-r--r--   0        0        0      156 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/classes/table/table_console.py
+-rw-r--r--   0        0        0    26132 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/commands/check.py
+-rw-r--r--   0        0        0    11014 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/commands/manual.py
+-rw-r--r--   0        0        0      430 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/commands/picker.py
+-rwxr-xr-x   0        0        0     3810 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0       53 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/binary.py
+-rw-r--r--   0        0        0     1655 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/config.py
+-rw-r--r--   0        0        0     1628 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/constants.py
+-rw-r--r--   0        0        0       74 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/date.py
+-rw-r--r--   0        0        0      190 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/download.py
+-rw-r--r--   0        0        0      204 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/files.py
+-rw-r--r--   0        0        0     1375 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/general.py
+-rw-r--r--   0        0        0       93 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/logger.py
+-rw-r--r--   0        0        0       69 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/metadata.py
+-rw-r--r--   0        0        0      862 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/other_url.py
+-rw-r--r--   0        0        0     1908 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/prompts.py
+-rw-r--r--   0        0        0     1808 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/req.py
+-rw-r--r--   0        0        0      271 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/table.py
+-rw-r--r--   0        0        0   265533 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/test_constants.py
+-rw-r--r--   0        0        0      248 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/time.py
+-rw-r--r--   0        0        0     3594 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/const/url.py
+-rw-r--r--   0        0        0        1 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    15609 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations.py
+-rw-r--r--   0        0        0      206 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/helpers.py
+-rw-r--r--   0        0        0     8568 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/labels.py
+-rw-r--r--   0        0        0    19443 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/media.py
+-rw-r--r--   0        0        0    11553 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/merge.py
+-rw-r--r--   0        0        0     8494 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/messages.py
+-rw-r--r--   0        0        0     8928 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/others.py
+-rw-r--r--   0        0        0    10366 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/posts.py
+-rw-r--r--   0        0        0     6725 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/profile.py
+-rw-r--r--   0        0        0     7485 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/stories.py
+-rw-r--r--   0        0        0     4810 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/db/operations_/wrapper.py
+-rw-r--r--   0        0        0    10881 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/alt_download.py
+-rw-r--r--   0        0        0    10682 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/alt_downloadbatch.py
+-rw-r--r--   0        0        0     4901 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/download.py
+-rw-r--r--   0        0        0    17167 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/downloadbatch.py
+-rw-r--r--   0        0        0     9077 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/downloadnormal.py
+-rw-r--r--   0        0        0    10787 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/main_download.py
+-rw-r--r--   0        0        0    11235 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/main_downloadbatch.py
+-rw-r--r--   0        0        0     1414 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/shared/classes/retries.py
+-rw-r--r--   0        0        0     1356 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/shared/classes/session.py
+-rw-r--r--   0        0        0     3795 2024-05-07 17:03:44.545793 ofscraper-3.9.5/ofscraper/download/shared/common/alt_common.py
+-rw-r--r--   0        0        0     6372 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/common/general.py
+-rw-r--r--   0        0        0     2063 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/common/main_common.py
+-rw-r--r--   0        0        0     2341 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/globals.py
+-rw-r--r--   0        0        0     9440 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/keyhelpers.py
+-rw-r--r--   0        0        0     3431 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/log.py
+-rw-r--r--   0        0        0      317 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/media.py
+-rw-r--r--   0        0        0      790 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/message.py
+-rw-r--r--   0        0        0     3927 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/metadata.py
+-rw-r--r--   0        0        0     2590 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/paths.py
+-rw-r--r--   0        0        0      453 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/progress.py
+-rw-r--r--   0        0        0     1155 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/download/shared/utils/text.py
+-rw-r--r--   0        0        0     8075 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/media/helpers.py
+-rw-r--r--   0        0        0     5019 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/media/main.py
+-rw-r--r--   0        0        0     3136 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/date.py
+-rw-r--r--   0        0        0     3143 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/flags.py
+-rw-r--r--   0        0        0      957 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/helpers.py
+-rw-r--r--   0        0        0      726 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/other.py
+-rw-r--r--   0        0        0     7561 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/price.py
+-rw-r--r--   0        0        0     1538 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/sort.py
+-rw-r--r--   0        0        0     1454 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/filters/models/subtype.py
+-rw-r--r--   0        0        0     3414 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/models/retriver.py
+-rw-r--r--   0        0        0     8105 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/models/selector.py
+-rw-r--r--   0        0        0     2466 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/helpers/model_helpers.py
+-rw-r--r--   0        0        0    15219 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/helpers/prompt_helpers.py
+-rw-r--r--   0        0        0      846 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     7747 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0      917 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/actions.py
+-rw-r--r--   0        0        0     6595 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/area.py
+-rw-r--r--   0        0        0     8257 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/auth.py
+-rw-r--r--   0        0        0     4438 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/binary.py
+-rw-r--r--   0        0        0    27916 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/config.py
+-rw-r--r--   0        0        0     1879 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/menu.py
+-rw-r--r--   0        0        0     3112 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/merge.py
+-rw-r--r--   0        0        0    16090 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/model.py
+-rw-r--r--   0        0        0     4135 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_groups/profile.py
+-rw-r--r--   0        0        0     7609 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    10346 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0     1342 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      567 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/runner/exit.py
+-rw-r--r--   0        0        0     1578 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/runner/load.py
+-rw-r--r--   0        0        0     2743 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/runner/run.py
+-rw-r--r--   0        0        0        1 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     3803 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/actions.py
+-rw-r--r--   0        0        0     1838 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/areas.py
+-rw-r--r--   0        0        0       12 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/globals.py
+-rw-r--r--   0        0        0     8419 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/common_args.py
+-rw-r--r--   0        0        0    18709 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/main_args.py
+-rw-r--r--   0        0        0     1349 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/manual_args.py
+-rw-r--r--   0        0        0     1618 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/message_args.py
+-rw-r--r--   0        0        0     1619 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/paid_args.py
+-rw-r--r--   0        0        0     1986 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/post_args.py
+-rw-r--r--   0        0        0     1672 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/groups/story_args.py
+-rw-r--r--   0        0        0     5571 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/helpers.py
+-rw-r--r--   0        0        0     1928 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/parse.py
+-rw-r--r--   0        0        0      395 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/quality.py
+-rw-r--r--   0        0        0      960 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/read.py
+-rw-r--r--   0        0        0      721 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/user.py
+-rw-r--r--   0        0        0      403 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/args/write.py
+-rw-r--r--   0        0        0     2148 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/context.py
+-rw-r--r--   0        0        0     1680 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/data.py
+-rw-r--r--   0        0        0     2034 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/file.py
+-rw-r--r--   0        0        0     2844 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/helpers.py
+-rw-r--r--   0        0        0     1669 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/make.py
+-rw-r--r--   0        0        0     6902 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/request.py
+-rw-r--r--   0        0        0      802 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/auth/schema.py
+-rw-r--r--   0        0        0     9824 2024-05-07 17:03:44.549793 ofscraper-3.9.5/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0     1780 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/cache.py
+-rw-r--r--   0        0        0     1612 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/checkers.py
+-rw-r--r--   0        0        0     2856 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/config.py
+-rw-r--r--   0        0        0     1442 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/context.py
+-rw-r--r--   0        0        0      522 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/custom.py
+-rw-r--r--   0        0        0    24693 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/data.py
+-rw-r--r--   0        0        0     2146 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/file.py
+-rw-r--r--   0        0        0     2073 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/menu.py
+-rw-r--r--   0        0        0     4797 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/schema.py
+-rw-r--r--   0        0        0      409 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/config/wrapper.py
+-rw-r--r--   0        0        0      499 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      788 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/constants.py
+-rw-r--r--   0        0        0     3401 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/context/exit.py
+-rw-r--r--   0        0        0     1135 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/context/run_async.py
+-rw-r--r--   0        0        0     1004 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/context/stdout.py
+-rw-r--r--   0        0        0     3460 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0     1040 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     1745 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/hash.py
+-rw-r--r--   0        0        0     7226 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/classes.py
+-rw-r--r--   0        0        0     2588 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/close.py
+-rw-r--r--   0        0        0      477 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/globals.py
+-rw-r--r--   0        0        0     1670 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/helpers.py
+-rw-r--r--   0        0        0     2098 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/logger.py
+-rw-r--r--   0        0        0     1672 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/logs.py
+-rw-r--r--   0        0        0     5955 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/other.py
+-rw-r--r--   0        0        0     3652 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/logs/stdout.py
+-rw-r--r--   0        0        0      601 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/manager.py
+-rw-r--r--   0        0        0      576 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/me.py
+-rw-r--r--   0        0        0     4161 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/menu.py
+-rw-r--r--   0        0        0     1022 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/merge.py
+-rw-r--r--   0        0        0     1710 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/paths/check.py
+-rw-r--r--   0        0        0     3091 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/paths/common.py
+-rw-r--r--   0        0        0      703 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/paths/manage.py
+-rw-r--r--   0        0        0     4912 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/paths/paths.py
+-rw-r--r--   0        0        0     1034 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/profiles/data.py
+-rw-r--r--   0        0        0     2785 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/profiles/manage.py
+-rw-r--r--   0        0        0     1583 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/profiles/tools.py
+-rw-r--r--   0        0        0    10893 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/progress.py
+-rw-r--r--   0        0        0     4406 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/run.py
+-rw-r--r--   0        0        0        1 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/sems.py
+-rw-r--r--   0        0        0     1672 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     4691 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/settings.py
+-rw-r--r--   0        0        0      417 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/system/free.py
+-rw-r--r--   0        0        0     3279 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/system/network.py
+-rw-r--r--   0        0        0     2472 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/system/system.py
+-rw-r--r--   0        0        0     2002 2024-05-07 17:03:44.553793 ofscraper-3.9.5/ofscraper/utils/text.py
+-rw-r--r--   0        0        0     2117 2024-05-07 17:04:09.753831 ofscraper-3.9.5/pyproject.toml
+-rw-r--r--   0        0        0     6424 1970-01-01 00:00:00.000000 ofscraper-3.9.5/PKG-INFO
```

### Comparing `ofscraper-3.9.4/LICENSE` & `ofscraper-3.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/README.md` & `ofscraper-3.9.5/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/actions/like.py` & `ofscraper-3.9.5/ofscraper/actions/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/actions/process.py` & `ofscraper-3.9.5/ofscraper/actions/process.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/actions/scraper.py` & `ofscraper-3.9.5/ofscraper/actions/scraper.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,17 +36,18 @@
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.context.stdout as stdout
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.system.free as free
 import ofscraper.utils.system.system as system
 from ofscraper.db.operations_.media import batch_mediainsert
-from ofscraper.db.operations_.profile import check_profile_table_exists,get_profile_info
-
-
+from ofscraper.db.operations_.profile import (
+    check_profile_table_exists,
+    get_profile_info,
+)
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
 
 
 @free.space_checker
 async def process_messages(model_id, username, c):
@@ -370,17 +371,15 @@
             username = profile.scrape_profile(model_id).get("username")
             if username == constants.getattr(
                 "DELETED_MODEL_PLACEHOLDER"
             ) and await check_profile_table_exists(
                 model_id=model_id, username=username
             ):
                 username = (
-                    await get_profile_info(
-                        model_id=model_id, username=username
-                    )
+                    await get_profile_info(model_id=model_id, username=username)
                     or username
                 )
             log.info(f"Processing {username}_{model_id}")
             await operations.table_init_create(model_id=model_id, username=username)
             log.debug(f"Created table for {username}_{model_id}")
             all_posts = list(
                 map(
```

### Comparing `ofscraper-3.9.4/ofscraper/api/archive.py` & `ofscraper-3.9.5/ofscraper/api/archive.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 r"""
                                                              
-  _____/ ____\______ ________________    ____   ___________ 
- /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
-(  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
- \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
+r"""
+                                                             
+ _______  _______         _______  _______  _______  _______  _______  _______  _______ 
+(  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
+| (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
+| |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
+| |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
+| |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
+| (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
+(_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
+                                                                                      
+"""
                  \/     \/           \/            \/         
 """
 
 import asyncio
 import logging
 import math
 import traceback
@@ -16,32 +24,34 @@
 
 import ofscraper.api.common.logs as common_logs
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.settings as settings
+from ofscraper.db.operations_.media import get_archived_media
+from ofscraper.db.operations_.posts import (
+    get_archived_post_info,
+    get_youngest_archived_date,
+)
 from ofscraper.utils.context.run_async import run
 from ofscraper.utils.logs.helpers import is_trace
-from ofscraper.db.operations_.posts import get_archived_post_info,get_youngest_archived_date
-from ofscraper.db.operations_.media import get_archived_media
-
 
 log = logging.getLogger("shared")
 
 
 sem = None
 
 
 @run
 async def get_archived_posts_progress(model_id, username, forced_after=None, c=None):
 
     oldarchived = None
     if not settings.get_api_cache_disabled():
-        oldarchived=await get_archived_post_info(model_id=model_id, username=username)
+        oldarchived = await get_archived_post_info(model_id=model_id, username=username)
     else:
         oldarchived = []
     trace_log_old(oldarchived)
 
     log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
     oldarchived = list(filter(lambda x: x is not None, oldarchived))
     after = await get_after(model_id, username, forced_after)
@@ -52,15 +62,15 @@
     progress_utils.archived_layout.visible = False
     return data
 
 
 @run
 async def get_archived_posts(model_id, username, forced_after=None, c=None):
     if not settings.get_api_cache_disabled():
-        oldarchived=await get_archived_post_info(model_id=model_id, username=username)
+        oldarchived = await get_archived_post_info(model_id=model_id, username=username)
     else:
         oldarchived = []
     trace_log_old(oldarchived)
 
     log.debug(f"[bold]Archived Cache[/bold] {len(oldarchived)} found")
     oldarchived = list(filter(lambda x: x is not None, oldarchived))
     after = await get_after(model_id, username, forced_after)
@@ -259,17 +269,15 @@
     missing_items = list(filter(lambda x: x.get("downloaded") != 1, curr))
     missing_items = list(sorted(missing_items, key=lambda x: x.get("posted_at") or 0))
     if len(missing_items) == 0:
         log.debug(
             "Using newest db date because,all downloads in db marked as downloaded"
         )
         return arrow.get(
-            await get_youngest_archived_date(
-                model_id=model_id, username=username
-            )
+            await get_youngest_archived_date(model_id=model_id, username=username)
         ).float_timestamp
     else:
         log.debug(
             f"Setting date slightly before earliest missing item\nbecause {len(missing_items)} posts in db are marked as undownloaded"
         )
         return arrow.get(missing_items[0]["posted_at"] or 0).float_timestamp
```

### Comparing `ofscraper-3.9.4/ofscraper/api/highlights.py` & `ofscraper-3.9.5/ofscraper/api/highlights.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,16 @@
         )
         return await process_stories_tasks(tasks)
 
 
 async def scrape_stories(c, user_id, job_progress=None) -> list:
     stories = None
     new_tasks = []
+    task = None
+
     await asyncio.sleep(1)
     url = constants.getattr("highlightsWithAStoryEP").format(user_id)
     try:
         task = (
             job_progress.add_task(
                 f"user id -> {user_id}",
                 visible=True,
@@ -341,14 +343,16 @@
     return highlightResponse
 
 
 async def scrape_highlight_list(c, user_id, job_progress=None, offset=0) -> list:
     new_tasks = []
     await asyncio.sleep(1)
     url = constants.getattr("highlightsWithStoriesEP").format(user_id, offset)
+    task = None
+
     try:
         task = (
             job_progress.add_task(
                 f"scraping highlight list  offset-> {offset}",
                 visible=True,
             )
             if job_progress
@@ -374,14 +378,16 @@
     return data, new_tasks
 
 
 async def scrape_highlights(c, id, job_progress=None) -> list:
     new_tasks = []
     await asyncio.sleep(1)
     url = constants.getattr("storyEP").format(id)
+    task = None
+
     try:
         task = (
             job_progress.add_task(
                 f"highlights id -> {id}",
                 visible=True,
             )
             if job_progress
```

### Comparing `ofscraper-3.9.4/ofscraper/api/init.py` & `ofscraper-3.9.5/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/api/labels.py` & `ofscraper-3.9.5/ofscraper/api/labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,16 @@
 
 
 async def scrape_labels(c, model_id, job_progress=None, offset=0):
     labels = None
     new_tasks = []
     await asyncio.sleep(1)
     url = constants.getattr("labelsEP").format(model_id, offset)
+    task = None
+
     try:
 
         task = (
             job_progress.add_task(
                 f"labels offset -> {offset}",
                 visible=True,
             )
@@ -311,14 +313,16 @@
     return list(responseDict.values())
 
 
 async def scrape_posts_labels(c, label, model_id, job_progress=None, offset=0):
     posts = None
     new_tasks = []
     url = constants.getattr("labelledPostsEP").format(model_id, offset, label["id"])
+    tasks = None
+
     await asyncio.sleep(1)
     try:
 
         task = (
             job_progress.add_task(
                 f": getting posts from label -> {label['name']}",
                 visible=True,
```

### Comparing `ofscraper-3.9.4/ofscraper/api/me.py` & `ofscraper-3.9.5/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/api/messages.py` & `ofscraper-3.9.5/ofscraper/api/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,82 +20,71 @@
 import ofscraper.api.common.logs as common_logs
 import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.settings as settings
+from ofscraper.db.operations_.media import get_messages_media
+from ofscraper.db.operations_.messages import (
+    get_messages_post_info,
+    get_youngest_message_date,
+)
 from ofscraper.utils.context.run_async import run
 from ofscraper.utils.logs.helpers import is_trace
-from ofscraper.db.operations_.messages import get_messages_post_info,get_youngest_message_date
-from ofscraper.db.operations_.media import get_messages_media
-
-
 
 log = logging.getLogger("shared")
-sleeper=None
-
+sleeper = None
 
 
 @run
 async def get_messages_progress(model_id, username, forced_after=None, c=None):
     global after
-    oldmessages=None
+    oldmessages = None
     if not settings.get_api_cache_disabled():
-        oldmessages=await get_messages_post_info(model_id=model_id, username=username)
+        oldmessages = await get_messages_post_info(model_id=model_id, username=username)
     else:
         oldmessages = []
     trace_log_old(oldmessages)
 
     before = (read_args.retriveArgs().before or arrow.now()).float_timestamp
     after = await get_after(model_id, username, forced_after)
     log_after_before(after, before, username)
 
     filteredArray = get_filterArray(after, before, oldmessages)
     splitArrays = get_split_array(filteredArray)
     # Set charged sleeper
     get_sleeper()
     tasks = get_tasks(splitArrays, filteredArray, oldmessages, model_id, c)
-    data = await process_tasks(tasks, model_id)
+    data = await process_tasks(tasks, model_id, after)
     progress_utils.messages_layout.visible = False
     return data
 
 
 @run
 async def get_messages(model_id, username, forced_after=None, c=None):
-    global after
-
-    oldmessages=None
+    oldmessages = None
     if not settings.get_api_cache_disabled():
-        oldmessages=await get_messages_post_info(model_id=model_id, username=username)
+        oldmessages = await get_messages_post_info(model_id=model_id, username=username)
     else:
         oldmessages = []
     trace_log_old(oldmessages)
 
     before = (read_args.retriveArgs().before or arrow.now()).float_timestamp
     after = await get_after(model_id, username, forced_after)
     log_after_before(after, before, username)
 
-    log.info(
-        f"""
-Setting initial message scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
-[yellow]Hint: append ' --after 2000' to command to force scan of all messages + download of new files only[/yellow]
-[yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all messages + download/re-download of all files[/yellow]
-
-        """
-    )
-
     filteredArray = get_filterArray(after, before, oldmessages)
     splitArrays = get_split_array(filteredArray)
     with progress_utils.set_up_api_messages():
         tasks = get_tasks(splitArrays, filteredArray, oldmessages, model_id, c)
-        return await process_tasks(tasks, model_id)
+        return await process_tasks(tasks, model_id, after)
 
 
-async def process_tasks(tasks, model_id):
+async def process_tasks(tasks, model_id, after):
     page_count = 0
     responseArray = []
     overall_progress = progress_utils.overall_progress
     page_task = overall_progress.add_task(
         f"Message Content Pages Progress: {page_count}", visible=True
     )
     seen = set()
@@ -321,26 +310,30 @@
         constants.getattr("messagesNextEP")
         if message_id
         else constants.getattr("messagesEP")
     )
     url = ep.format(model_id, message_id)
     log.debug(f"{message_id if message_id else 'init'} {url}")
     new_tasks = []
+    tasks = None
+
     await asyncio.sleep(1)
     try:
         async with c.requests_async(url=url, sleeper=get_sleeper()) as r:
             task = (
                 job_progress.add_task(
                     f": Message ID-> {message_id if message_id else 'initial'}"
                 )
                 if job_progress
                 else None
             )
             messages = (await r.json_())["list"]
-            log_id = f"offset messageid:{message_id if message_id else 'init messageid'}"
+            log_id = (
+                f"offset messageid:{message_id if message_id else 'init messageid'}"
+            )
             if not bool(messages):
                 log.debug(f"{log_id} -> no messages found")
                 return [], []
             log.debug(f"{log_id} -> number of messages found {len(messages)}")
             log.debug(
                 f"{log_id} -> first date {arrow.get(messages[0].get('createdAt') or messages[0].get('postedAt')).format(constants.getattr('API_DATE_FORMAT'))}"
             )
@@ -457,17 +450,15 @@
         sorted(missing_items, key=lambda x: arrow.get(x.get("posted_at") or 0))
     )
     if len(missing_items) == 0:
         log.debug(
             "Using newest db date because,all downloads in db are marked as downloaded"
         )
         return arrow.get(
-            await get_youngest_message_date(
-                model_id=model_id, username=username
-            )
+            await get_youngest_message_date(model_id=model_id, username=username)
         ).float_timestamp
     else:
         log.debug(
             f"Setting date slightly before oldest missing item\nbecause {len(missing_items)} messages in db are marked as undownloaded"
         )
         return arrow.get(missing_items[0]["posted_at"]).float_timestamp
 
@@ -508,23 +499,24 @@
         )
         # Check if there are more elements remaining after this chunk
         if i + chunk_size > len(responseArray):
             break  # Exit the loop if we've processed all elements
 
 
 def log_after_before(after, before, username):
-    log.info(f"Messages before = {arrow.get(before).format(constants.getattr('API_DATE_FORMAT'))}")
 
     log.info(
         f"""
-Setting initial message scan date for {username} to {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))}
+Setting Message range for {username} from {arrow.get(after).format(constants.getattr('API_DATE_FORMAT'))} to {arrow.get(before).format(constants.getattr('API_DATE_FORMAT'))}
+
 [yellow]Hint: append ' --after 2000' to command to force scan of all messages + download of new files only[/yellow]
 [yellow]Hint: append ' --after 2000 --force-all' to command to force scan of all messages + download/re-download of all files[/yellow]
 
         """
     )
 
+
 def get_sleeper():
     global sleeper
     if not sleeper:
-        sleeper=sessionManager.SessionSleep(sleep=8)
+        sleeper = sessionManager.SessionSleep(sleep=8)
     return sleeper
```

### Comparing `ofscraper-3.9.4/ofscraper/api/paid.py` & `ofscraper-3.9.5/ofscraper/api/paid.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/api/pinned.py` & `ofscraper-3.9.5/ofscraper/api/pinned.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 r"""
                                                              
-  _____/ ____\______ ________________    ____   ___________ 
- /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
-(  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
- \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
+r"""
+                                                             
+ _______  _______         _______  _______  _______  _______  _______  _______  _______ 
+(  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
+| (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
+| |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
+| |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
+| |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
+| (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
+(_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
+                                                                                      
+"""
                  \/     \/           \/            \/         
 """
 
 import asyncio
 import logging
 import math
 import traceback
```

### Comparing `ofscraper-3.9.4/ofscraper/api/profile.py` & `ofscraper-3.9.5/ofscraper/api/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,23 +66,22 @@
         log.traceback_(traceback.format_exc())
         raise E
 
 
 async def scrape_profile_helper_async(c, username: Union[int, str]):
     data = cache.get(f"username_{username}", default=None)
     log.trace(f"username date: {data}")
+    url = constants.getattr("profileEP").format(username)
     if data and not read_args.retriveArgs().update_profile:
         return data
     try:
 
-        log.info(f"to get profile {username}")
+        log.info(f"getting {username} with {url}")
         await asyncio.sleep(1)
-        async with c.requests_async(
-            constants.getattr("profileEP").format(username)
-        ) as r:
+        async with c.requests_async(url) as r:
             if r.status == 404:
                 return {"username": constants.getattr("DELETED_MODEL_PLACEHOLDER")}
             cache.set(
                 f"username_{username}",
                 await r.json_(),
                 int(constants.getattr("PROFILE_DATA_EXPIRY_ASYNC")),
             )
```

### Comparing `ofscraper-3.9.4/ofscraper/api/subscriptions/helpers.py` & `ofscraper-3.9.5/ofscraper/api/subscriptions/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/api/subscriptions/individual.py` & `ofscraper-3.9.5/ofscraper/api/subscriptions/individual.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,13 +68,15 @@
     tasks = [
         asyncio.create_task(profile.scrape_profile_helper_async(c, account))
         for account in accounts
     ]
     for task in asyncio.as_completed(tasks):
         try:
             result = await task
+            log.debug(f"subscription data found for {result['username']} ")
+            log.trace(result)
             output.append(result)
         except Exception as E:
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
             continue
     return output
```

### Comparing `ofscraper-3.9.4/ofscraper/api/subscriptions/lists.py` & `ofscraper-3.9.5/ofscraper/api/subscriptions/lists.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/api/subscriptions/subscriptions.py` & `ofscraper-3.9.5/ofscraper/api/subscriptions/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/api/timeline.py` & `ofscraper-3.9.5/ofscraper/api/timeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 r"""
                                                              
-  _____/ ____\______ ________________    ____   ___________ 
- /  _ \   __\/  ___// ___\_  __ \__  \  /  _ \_/ __ \_  __ \
-(  <_> )  |  \___ \\  \___|  | \// __ \(  <_> )  ___/|  | \/
- \____/|__| /____  >\___  >__|  (____  /\____/ \___  >__|   
+r"""
+                                                             
+ _______  _______         _______  _______  _______  _______  _______  _______  _______ 
+(  ___  )(  ____ \       (  ____ \(  ____ \(  ____ )(  ___  )(  ____ )(  ____ \(  ____ )
+| (   ) || (    \/       | (    \/| (    \/| (    )|| (   ) || (    )|| (    \/| (    )|
+| |   | || (__     _____ | (_____ | |      | (____)|| (___) || (____)|| (__    | (____)|
+| |   | ||  __)   (_____)(_____  )| |      |     __)|  ___  ||  _____)|  __)   |     __)
+| |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
+| (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
+(_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
+                                                                                      
+"""
                  \/     \/           \/            \/         
 """
 
 import asyncio
 import logging
 import math
 import traceback
@@ -17,19 +25,21 @@
 import ofscraper.api.common.logs as common_logs
 import ofscraper.classes.sessionmanager as sessionManager
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
 import ofscraper.utils.progress as progress_utils
 import ofscraper.utils.settings as settings
+from ofscraper.db.operations_.media import get_timeline_media
+from ofscraper.db.operations_.posts import (
+    get_timeline_posts_info,
+    get_youngest_timeline_date,
+)
 from ofscraper.utils.context.run_async import run
 from ofscraper.utils.logs.helpers import is_trace
-from ofscraper.db.operations_.posts import get_timeline_posts_info,get_youngest_timeline_date
-from ofscraper.db.operations_.media import get_timeline_media
-
 
 log = logging.getLogger("shared")
 
 
 @run
 async def get_timeline_posts_progress(model_id, username, forced_after=None, c=None):
 
@@ -289,17 +299,15 @@
     )
     missing_items = list(sorted(missing_items, key=lambda x: arrow.get(x["posted_at"])))
     if len(missing_items) == 0:
         log.debug(
             "Using using newest db date, because all downloads in db marked as downloaded"
         )
         return arrow.get(
-            await get_youngest_timeline_date(
-                model_id=model_id, username=username
-            )
+            await get_youngest_timeline_date(model_id=model_id, username=username)
         ).float_timestamp
     else:
         log.debug(
             f"Setting date slightly before oldest missing item\nbecause {len(missing_items)} posts in db are marked as undownloaded"
         )
         return arrow.get(missing_items[0]["posted_at"]).float_timestamp
 
@@ -312,16 +320,19 @@
 
     url = (
         constants.getattr("timelineNextEP").format(model_id, str(timestamp))
         if timestamp
         else constants.getattr("timelineEP").format(model_id)
     )
     log.debug(url)
-    await asyncio.sleep(1)
     new_tasks = []
+    tasks = None
+
+    await asyncio.sleep(1)
+
     try:
         task = (
             job_progress.add_task(
                 f"Timestamp -> {arrow.get(math.trunc(float(timestamp))).format(constants.getattr('API_DATE_FORMAT')) if timestamp is not None  else 'initial'}",
                 visible=True,
             )
             if job_progress
```

### Comparing `ofscraper-3.9.4/ofscraper/classes/base.py` & `ofscraper-3.9.5/ofscraper/classes/base.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/classes/labels.py` & `ofscraper-3.9.5/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/classes/media.py` & `ofscraper-3.9.5/ofscraper/classes/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/classes/models.py` & `ofscraper-3.9.5/ofscraper/classes/models.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/classes/multiprocessprogress.py` & `ofscraper-3.9.5/ofscraper/classes/multiprocessprogress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/classes/placeholder.py` & `ofscraper-3.9.5/ofscraper/classes/placeholder.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,15 @@
 
 
 class basePlaceholder:
     def __init__(self) -> None:
         self._ele = None
 
     def create_variables_base(self):
-        my_profile = profile_data.get_my_info()
-        my_id, my_username = me.parse_user(my_profile)
+        my_id, my_username = me.parse_user()
         self._variables = {
             "config_path": common_paths.get_config_home(),
             "profile": profile_data.get_active_profile(),
             "site_name": "Onlyfans",
             "save_location": common_paths.get_save_location(mediatype=self._ele),
             "my_id": my_id,
             "my_username": my_username,
```

### Comparing `ofscraper-3.9.4/ofscraper/classes/posts.py` & `ofscraper-3.9.5/ofscraper/classes/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/classes/sessionmanager.py` & `ofscraper-3.9.5/ofscraper/classes/sessionmanager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
-import time
 import contextlib
 import logging
 import ssl
 import threading
+import time
 import traceback
 
 import aiohttp
 import aiohttp.client_exceptions
 import arrow
 import certifi
 import httpx
@@ -15,15 +15,14 @@
 from tenacity import AsyncRetrying, Retrying, retry_if_not_exception_type
 
 import ofscraper.utils.auth.request as auth_requests
 import ofscraper.utils.config.data as data
 import ofscraper.utils.constants as constants
 
 
-
 def is_rate_limited(exception):
     return (
         isinstance(exception, aiohttp.ClientResponseError)
         and (
             getattr(exception, "status_code", None)
             or getattr(exception, "status", None) in {429, 504}
         )
@@ -36,61 +35,69 @@
             )
             in {429, 504}
         )
     )
 
 
 class SessionSleep:
-    def __init__(self,sleep=None):
+    def __init__(self, sleep=None):
         self._sleep = sleep
         self._last_date = arrow.now()
-        self._alock=asyncio.Lock()
+        self._alock = asyncio.Lock()
+
     async def async_toomany_req(self):
         async with self._alock:
             self.toomany_req()
+
     def toomany_req(self):
-        log=logging.getLogger("shared")
-        dif_min=constants.getattr("SESSION_SLEEP_INCREASE_TIME_DIFF")
+        log = logging.getLogger("shared")
+        dif_min = constants.getattr("SESSION_SLEEP_INCREASE_TIME_DIFF")
         if self._sleep is None:
             self._sleep = constants.getattr("SESSION_SLEEP_INIT")
             log.debug(f"too many req => setting sleep to init [{self._sleep} seconds]")
         elif arrow.now().float_timestamp - self._last_date.float_timestamp < dif_min:
-            log.debug(f"too many req => not changing sleep [{self._sleep} seconds] because last call less than {dif_min} seconds")
+            log.debug(
+                f"too many req => not changing sleep [{self._sleep} seconds] because last call less than {dif_min} seconds"
+            )
             return self._sleep
         else:
             self._sleep = self._sleep * 2
             log.debug(f"too many req => setting sleep to [{self._sleep} seconds]")
         self._last_date = arrow.now()
-        return self._sleep     
+        return self._sleep
+
     async def async_do_sleep(self):
         if self._sleep:
-            logging.getLogger("shared").debug(f"too many req => waiting [{self._sleep} seconds] before next req")
+            logging.getLogger("shared").debug(
+                f"too many req => waiting [{self._sleep} seconds] before next req"
+            )
             await asyncio.sleep(self._sleep)
+
     def do_sleep(self):
         if self._sleep:
-            logging.getLogger("shared").debug(f"too many req => waiting [{self._sleep} seconds] before next req")
+            logging.getLogger("shared").debug(
+                f"too many req => waiting [{self._sleep} seconds] before next req"
+            )
             time.sleep(self._sleep)
+
     @property
     def sleep(self):
         return self._sleep
-    @sleep.setter
-    def sleep(self,val):
-        self._sleep=val
-
-
 
+    @sleep.setter
+    def sleep(self, val):
+        self._sleep = val
 
 
 class CustomTenacity(AsyncRetrying):
     """
     A custom context manager using tenacity for asynchronous retries with wait strategies and stopping without exceptions.
     """
 
-    def __init__(self,
-     wait_random=None, wait_exponential=None, *args, **kwargs):
+    def __init__(self, wait_random=None, wait_exponential=None, *args, **kwargs):
         super().__init__(*args, after=self._after_func, **kwargs)
         self.wait_random = wait_random or tenacity.wait.wait_random(
             min=constants.getattr("OF_MIN_WAIT_SESSION_DEFAULT"),
             max=constants.getattr("OF_MAX_WAIT_SESSION_DEFAULT"),
         )
         self.wait_exponential = wait_exponential or tenacity.wait_exponential(
             min=constants.getattr("OF_MIN_WAIT_EXPONENTIAL_SESSION_DEFAULT"),
@@ -184,15 +191,16 @@
             "OF_MIN_WAIT_EXPONENTIAL_SESSION_DEFAULT"
         )
         self._wait_max_exponential = wait_max_exponential or constants.getattr(
             "OF_MAX_WAIT_EXPONENTIAL_SESSION_DEFAULT"
         )
         self._log = log or logging.getLogger("shared")
         auth_requests.read_request_auth(forced=None) if new_request_auth else None
-        self._sleeper=SessionSleep()
+        self._sleeper = SessionSleep()
+
     async def __aenter__(self):
         self._async = True
         if self._backend == "aio":
             self._session = aiohttp.ClientSession(
                 connector=aiohttp.TCPConnector(limit=self._connect_limit),
             )
 
@@ -261,29 +269,29 @@
         wait_max=None,
         log=None,
         total_timeout=None,
         connect_timeout=None,
         pool_connect_timeout=None,
         read_timeout=None,
         sync_sem=None,
-        sleeper=None
+        sleeper=None,
     ):
         auth_requests.read_request_auth(forced=True) if sign else None
 
         headers = self._create_headers(headers, url, sign) if headers is None else None
         cookies = self._create_cookies() if cookies is None else None
         json = json or None
         params = params or None
         r = None
         log = log or self._log
         min = wait_min or self._wait_min
         max = wait_max or self._wait_max
         retries = retries or self._retries
         sync_sem = self._sync_sem or sync_sem
-        sleeper=sleeper or self._sleeper
+        sleeper = sleeper or self._sleeper
         for _ in Retrying(
             retry=retry_if_not_exception_type(
                 (KeyboardInterrupt, asyncio.TimeoutError)
             ),
             stop=tenacity.stop.stop_after_attempt(retries),
             wait=tenacity.wait.wait_random(min=min, max=max),
             before=lambda x: (
@@ -319,15 +327,15 @@
                     elif not r.ok:
                         log.debug(f"[bold]failed: [bold] {r.url}")
                         log.debug(f"[bold]status: [bold] {r.status}")
                         log.debug(f"[bold]response text [/bold]: {r.text_()}")
                         log.debug(f"[bold]headers[/bold]: {r.headers}")
                         r.raise_for_status()
                 except Exception as E:
-                    if(is_rate_limited(E)):
+                    if is_rate_limited(E):
                         sleeper.toomany_req()
                     log.traceback_(E)
                     log.traceback_(traceback.format_exc())
                     raise E
         yield r
         sync_sem.release()
 
@@ -361,15 +369,15 @@
         wait_min = wait_min or self._wait_min
         wait_max = wait_max or self._wait_max
         wait_min_exponential = wait_min_exponential or self._wait_min_exponential
         wait_max_exponential = wait_max_exponential or self._wait_max_exponential
         log = log or self._log
         retries = retries or self._retries
         sem = sem or self._sem
-        sleeper=sleeper or self._sleeper
+        sleeper = sleeper or self._sleeper
         async for _ in CustomTenacity(
             wait_exponential=tenacity.wait.wait_exponential(
                 multiplier=2, min=wait_min_exponential, max=wait_max_exponential
             ),
             retry=retry_if_not_exception_type(
                 (KeyboardInterrupt, asyncio.TimeoutError)
             ),
@@ -437,29 +445,30 @@
                     elif not r.ok:
                         log.debug(f"[bold]failed: [bold] {r.url}")
                         log.debug(f"[bold]status: [bold] {r.status}")
                         log.debug(f"[bold]response text [/bold]: {await r.text_()}")
                         log.debug(f"[bold]headers[/bold]: {r.headers}")
                         r.raise_for_status()
                 except Exception as E:
-                    if(is_rate_limited(E)):
+                    if is_rate_limited(E):
                         await sleeper.async_toomany_req()
                     log.traceback_(E)
                     log.traceback_(traceback.format_exc())
                     sem.release()
                     raise E
         yield r
         sem.release()
 
     @property
     def sleep(self):
         return self._sleeper._sleep
+
     @sleep.setter
-    def sleep(self,val):
-        self._sleeper._sleep=val
+    def sleep(self, val):
+        self._sleeper._sleep = val
 
     async def _httpx_funct_async(self, *args, **kwargs):
         t = await self._session.request(*args, **kwargs)
         t.ok = not t.is_error
         t.json_ = lambda: self.factoryasync(t.json)
         t.text_ = lambda: self.factoryasync(t.text)
         t.status = t.status_code
@@ -486,8 +495,8 @@
         r.status_code = r.status
         r.read_ = r.content.read
         return r
 
     async def factoryasync(self, input):
         if callable(input):
             return input()
-        return input
+        return input
```

### Comparing `ofscraper-3.9.4/ofscraper/commands/check.py` & `ofscraper-3.9.5/ofscraper/commands/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,61 +15,43 @@
 import ofscraper.api.messages as messages_
 import ofscraper.api.paid as paid_
 import ofscraper.api.pinned as pinned
 import ofscraper.api.profile as profile
 import ofscraper.api.timeline as timeline
 import ofscraper.classes.posts as posts_
 import ofscraper.classes.sessionmanager as sessionManager
-import ofscraper.classes.table as table
+import ofscraper.classes.table.table as table
 import ofscraper.db.operations as operations
 import ofscraper.download.downloadnormal as downloadnormal
 import ofscraper.models.selector as selector
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.args.write as write_args
 import ofscraper.utils.auth.request as auth_requests
 import ofscraper.utils.cache as cache
 import ofscraper.utils.console as console_
 import ofscraper.utils.constants as constants
 import ofscraper.utils.context.stdout as stdout
 import ofscraper.utils.settings as settings
 import ofscraper.utils.system.network as network
+from ofscraper.classes.table.row_names import row_names_all
+from ofscraper.db.operations_.media import batch_mediainsert, get_media_ids_downloaded
 from ofscraper.download.shared.utils.text import textDownloader
-from ofscraper.db.operations_.media import batch_mediainsert,get_media_ids_downloaded
-
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
 console = console_.get_shared_console()
-ROW_NAMES = (
-    "Number",
-    "Download_Cart",
-    "UserName",
-    "Downloaded",
-    "Unlocked",
-    "Times_Detected",
-    "Length",
-    "Mediatype",
-    "Post_Date",
-    "Post_Media_Count",
-    "Responsetype",
-    "Price",
-    "Post_ID",
-    "Media_ID",
-    "Text",
-)
+
 ROWS = []
-app = None
 ALL_MEDIA = {}
 MEDIA_KEY = ["id", "postid", "username"]
 
 
 def process_download_cart():
     while True:
-        global app
-        if not app or app.row_queue.empty():
+        if table.row_queue.empty():
             time.sleep(10)
             continue
         try:
             process_item()
         except Exception:
             # handle getting new downloads
             None
@@ -81,23 +63,23 @@
         if not network.check_cdm():
             log.info("error was raised by cdm checker\ncdm will not be check again\n\n")
         else:
             log.info("cdm checker was fine\ncdm will not be check again\n\n")
     process_download_cart.counter = process_download_cart.counter + 1
     log.info("Getting items from cart")
     try:
-        row, key = app.row_queue.get()
+        row, key = table.row_queue.get()
     except Exception as E:
         log.error(f"Error getting item from queue: {E}")
         return
     for count, _ in enumerate(range(0, 2)):
         try:
-            username = row[app.row_names.index("UserName")].plain
-            post_id = row[app.row_names.index("Post_ID")].plain
-            media_id = int(row[app.row_names.index("Media_ID")].plain)
+            username = row[list(row_names_all()).index("username")].plain
+            post_id = int(row[list(row_names_all()).index("post_id")].plain)
+            media_id = int(row[list(row_names_all()).index("media_id")].plain)
             media = ALL_MEDIA.get(
                 "_".join(map(lambda x: str(x), [media_id, post_id, username]))
             )
             if not media:
                 raise Exception(f"No data for {media_id}_{post_id}_{username}")
             log.info(f"Added url {media.url or media.mpd}")
             log.info("Sending URLs to OF-Scraper")
@@ -116,26 +98,25 @@
                 values = downloadnormal.process_dicts(username, model_id, [media])
                 if values is None or values[-1] == 1:
                     raise Exception("Download is marked as skipped")
             else:
                 raise Exception("Issue getting download")
 
             log.info("Download Finished")
-            app.update_cell(key, "Download_Cart", "[downloaded]")
-            app.update_cell(key, "Downloaded", True)
+            table.app.update_cell(key, "download_cart", "[downloaded]")
             break
         except Exception as E:
             if count == 1:
-                app.update_cell(key, "Download_Cart", "[failed]")
+                table.app.update_cell(key, "download_cart", "[failed]")
                 raise E
             log.info("Download Failed Refreshing data")
             data_refill(media_id, post_id, username, model_id)
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
-    if app.row_queue.empty():
+    if table.row_queue.empty():
         log.info("Download cart is currently empty")
 
 
 @run
 async def data_refill(media_id, post_id, target_name, model_id):
     args = read_args.retriveArgs()
     if args.command == "msg_check":
@@ -573,17 +554,15 @@
 async def get_downloaded(user_name, model_id, paid=False):
     downloaded = {}
 
     await operations.table_init_create(model_id=model_id, username=user_name)
     paid = await get_paid_ids(model_id, user_name) if paid else []
     [
         downloaded.update({ele: downloaded.get(ele, 0) + 1})
-        for ele in get_media_ids_downloaded(
-            model_id=model_id, username=user_name
-        )
+        for ele in get_media_ids_downloaded(model_id=model_id, username=user_name)
         + paid
     ]
 
     return downloaded
 
 
 @run
@@ -620,28 +599,18 @@
     start_table(ROWS_)
 
 
 def start_table(ROWS_):
     global app
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
-    app = table.InputApp()
-    app.mutex = threading.Lock()
-    app.row_queue = queue.Queue()
-    ROWS = get_first_row()
-    ROWS.extend(ROWS_)
-
-    app.table_data = ROWS
-    app.row_names = ROW_NAMES
-    app._filtered_rows = app.table_data[1:]
-    app.run()
-
-
-def get_first_row():
-    return [ROW_NAMES]
+    ROWS = ROWS_
+    app = table.app(
+        table_data=ROWS, mutex=threading.Lock(), mediatype=init_media_type_helper()
+    )
 
 
 def texthelper(text):
     text = text or ""
     text = inspect.cleandoc(text)
     text = re.sub(" +$", "", text)
     text = re.sub("^ +", "", text)
@@ -669,53 +638,66 @@
 
 
 def checkmarkhelper(ele):
     return "[]" if unlocked_helper(ele) else "Not Unlocked"
 
 
 async def row_gather(username, model_id, paid=False):
-    # fix text
+    # fix tex
     global ROWS
     downloaded = await get_downloaded(username, model_id, paid=paid)
 
     mediadict = {}
     [
         mediadict.update({ele.id: mediadict.get(ele.id, []) + [ele]})
         for ele in list(filter(lambda x: x.canview, ALL_MEDIA.values()))
     ]
     out = []
+
     media_sorted = sorted(
         ALL_MEDIA.values(), key=lambda x: arrow.get(x.date), reverse=True
     )
-    for _, ele in enumerate(media_sorted):
+    for count, ele in enumerate(media_sorted):
         out.append(
-            [
-                None,
-                checkmarkhelper(ele),
-                username,
-                ele.id in downloaded
+            {
+                "index": count,
+                "number": None,
+                "download_cart": checkmarkhelper(ele),
+                "username": username,
+                "downloaded": ele.id in downloaded
                 or cache.get(ele.postid) is not None
                 or cache.get(ele.filename) is not None,
-                unlocked_helper(ele),
-                times_helper(ele, mediadict, downloaded),
-                ele.numeric_duration,
-                ele.mediatype,
-                datehelper(ele.formatted_postdate),
-                len(ele._post.post_media),
-                ele.responsetype,
-                "Free" if ele._post.price == 0 else "{:.2f}".format(ele._post.price),
-                ele.postid,
-                ele.id,
-                texthelper(ele.text),
-            ]
+                "unlocked": unlocked_helper(ele),
+                "times_detected": times_helper(ele, mediadict, downloaded),
+                "post_media_count": len(ele._post.post_media),
+                "mediatype": ele.mediatype,
+                "post_date": datehelper(ele.formatted_postdate),
+                "media": len(ele._post.post_media),
+                "length": ele.numeric_duration,
+                "responsetype": ele.responsetype,
+                "price": (
+                    "Free" if ele._post.price == 0 else "{:.2f}".format(ele._post.price)
+                ),
+                "post_id": ele.postid,
+                "media_id": ele.id,
+                "text": ele.post.db_sanitized_text,
+            }
         )
     ROWS = ROWS or []
     ROWS.extend(out)
 
 
+def init_media_type_helper():
+    args = read_args.retriveArgs()
+    mediatype = args.mediatype
+    args.mediatype = None
+    write_args.setArgs(args)
+    return mediatype
+
+
 def reset_time_line_cache(model_id):
     cache.set(f"timeline_check_{model_id}", [])
     cache.set(f"archived_check_{model_id}", [])
     cache.set(f"labels_check_{model_id}", [])
     cache.set(f"pinned_check_{model_id}", [])
     cache.close()
```

### Comparing `ofscraper-3.9.4/ofscraper/commands/manual.py` & `ofscraper-3.9.5/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/commands/scraper.py` & `ofscraper-3.9.5/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/const/config.py` & `ofscraper-3.9.5/ofscraper/const/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/const/general.py` & `ofscraper-3.9.5/ofscraper/const/general.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 MODEL_PRICE_PLACEHOLDER = "Unknown_Price"
 disclaimers = [
     "This tool is not affiliated, associated, or partnered with OnlyFans in any way. We are not authorized, endorsed, or sponsored by OnlyFans. All OnlyFans trademarks remain the property of Fenix International Limited.",
     "This tool is for educational purposes only and is not intended for actual use. Should you choose to actually use it you accept all consequences and agree that you are not using it to redistribute content or  for any other action that will cause loss of revenue to creators or platforms scraped.",
 ]
 APP_TOKEN = "33d57ade8c02dbc5a333db99ff9ae26a"
 CONTINUE_BOOL = True
-WINDOWS_MAX_PATH = 255
+WINDOWS_MAX_PATH_BYTES = 530
 MAC_MAX_PATH = 255
-LINUX_MAX_FILE = 254
+LINUX_MAX_FILE_NAME_BYTES = 254
 BUF_SIZE = 1000000
 MAX_TEXT_LENGTH = 70
 MAX_TEXT_WORKER = 30
 FILE_COUNT_PLACEHOLDER = True
 DELETED_MODEL_PLACEHOLDER = "modeldeleted"
 LARGE_TRACE_CHUNK_SIZE = 100
+FILTER_SELF_MEDIA = True
```

### Comparing `ofscraper-3.9.4/ofscraper/const/other_url.py` & `ofscraper-3.9.5/ofscraper/const/other_url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/const/prompts.py` & `ofscraper-3.9.5/ofscraper/const/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/const/req.py` & `ofscraper-3.9.5/ofscraper/const/req.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 MAX_THREAD_WORKERS = 20
 API_MAX_AREAS = 2
 API_TIMEOUT_PER_TASK = 500
 API_REQUEST_THREADONLY = ["Windows", "Linux", "Darwin"]
 
 SESSION_SLEEP_INIT = 2
-SESSION_SLEEP_INCREASE_TIME_DIFF=30
-MESSAGE_SLEEP_DEFAULT=0
+SESSION_SLEEP_INCREASE_TIME_DIFF = 30
+MESSAGE_SLEEP_DEFAULT = 0
 # page must be 50 post, and 50 is a reasonable size for max number of pages
 REASONABLE_MAX_PAGE = 50
 MIN_PAGE_POST_COUNT = 50
 
 # messages
 REASONABLE_MAX_PAGE_MESSAGES = 80
```

### Comparing `ofscraper-3.9.4/ofscraper/const/test_constants.py` & `ofscraper-3.9.5/ofscraper/const/test_constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/const/url.py` & `ofscraper-3.9.5/ofscraper/const/url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/db/operations.py` & `ofscraper-3.9.5/ofscraper/db/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
 import logging
 import pathlib
-import shutil
 
 import arrow
 from rich.console import Console
 
 import ofscraper.classes.labels as labels
 import ofscraper.classes.placeholder as placeholder
 import ofscraper.utils.cache as cache
@@ -71,14 +70,15 @@
 from ofscraper.db.operations_.stories import (
     add_column_stories_ID,
     create_stories_table,
     make_stories_table_changes,
     modify_unique_constriant_stories,
 )
 from ofscraper.utils.context.run_async import run
+from ofscraper.utils.paths.manage import copy_path
 
 console = Console()
 log = logging.getLogger("shared")
 
 
 @run
 async def create_tables(model_id=None, username=None, db_path=None, **kwargs):
@@ -129,19 +129,18 @@
         raise E
 
 
 def restore_backup_transition(backup, model_id, username, db_path=None, **kwargs):
     database = db_path or placeholder.databasePlaceholder().databasePathHelper(
         model_id, username
     )
-    shutil.copy2(backup, database)
+    copy_path(backup, database)
     log.debug(f"restored {database} from {backup}")
 
 
-
 def get_group_difference(model_id=None, username=None, db_path=None):
 
     changes = get_schema_changes(model_id=model_id, username=username, db_path=db_path)
     groupA = [
         "media_hash",
         "media_model_id",
         "posts_model_id",
@@ -384,31 +383,31 @@
     )
     database_copy = None
     now = arrow.now().float_timestamp
     last = cache.get(f"{username}_{model_id}_db_backup", default=now)
     if backup:
         database_copy = database_path.parent / "backup" / f"{backup}"
         database_copy.parent.mkdir(parents=True, exist_ok=True)
-        shutil.copy2(database_path, database_copy)
+        copy_path(database_path, database_copy)
     elif now - last > constants.getattr("DBINTERVAL") and database_path.exists():
         database_copy = placeholder.databasePlaceholder().databasePathCopyHelper(
             model_id, username
         )
         database_copy.parent.mkdir(parents=True, exist_ok=True)
-        shutil.copy2(database_path, database_copy)
+        copy_path(database_path, database_copy)
         cache.set(f"{username}_{model_id}_db_backup", now)
     elif (
         not pathlib.Path(database_path.parent / "backup").exists()
         or len(list(pathlib.Path(database_path.parent / "backup").iterdir())) == 0
     ):
         database_copy = placeholder.databasePlaceholder().databasePathCopyHelper(
             model_id, username
         )
         database_copy.parent.mkdir(parents=True, exist_ok=True)
-        shutil.copy2(database_path, database_copy)
+        copy_path(database_path, database_copy)
         cache.set(f"{username}_{model_id}_db_backup", now)
     cache.close()
     return database_copy
 
 
 @run
 async def table_init_create(model_id=None, username=None, **kwargs):
```

### Comparing `ofscraper-3.9.4/ofscraper/db/operations_/labels.py` & `ofscraper-3.9.5/ofscraper/db/operations_/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/db/operations_/media.py` & `ofscraper-3.9.5/ofscraper/db/operations_/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,29 +143,31 @@
 SELECT media_id FROM medias where downloaded=(1) and model_id=(?)
 """
 getTimelineMedia = """
 SELECT
 media_id,post_id,link,directory
 filename,size,api_type,media_type
 preview,linked,downloaded,created_at,posted_at,hash,model_id,unlocked
-FROM medias where api_type=('Timeline') and model_id=(?)
+FROM medias where LOWER(api_type) in ('timeline','posts','post') and model_id=(?)
 """
 getArchivedMedia = """
 SELECT
 media_id,post_id,link,directory
 filename,size,api_type,media_type
 preview,linked,downloaded,created_at,posted_at,hash,model_id,unlocked
-FROM medias where api_type=('Archived') and model_id=(?)
+FROM medias where LOWER(api_type) in ('archived') and model_id=(?)
 """
 getMessagesMedia = """
 SELECT 
-media_id,post_id,link,directory
-filename,size,api_type,media_type
-preview,linked,downloaded,created_at,posted_at,hash,model_id,unlocked
-FROM medias where api_type=('Message') or api_type=('Messages') and model_id=(?)
+  media_id, post_id, link, directory,
+  filename, size, api_type, media_type,
+  preview, linked, downloaded, created_at, posted_at, hash, model_id, unlocked
+FROM medias
+WHERE LOWER(api_type) IN ('message', 'messages') -- Use IN for multiple values
+AND model_id = ?;  -- Prepared statement placeholder
 """
 
 
 @wrapper.operation_wrapper_async
 def create_media_table(model_id=None, username=None, conn=None, db_path=None, **kwargs):
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(mediaCreate)
@@ -452,27 +454,37 @@
 
 @wrapper.operation_wrapper_async
 def get_messages_media(conn=None, model_id=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(getMessagesMedia, [model_id])
         data = [dict(row) for row in cur.fetchall()]
         return [
-            dict(ele, posted_at=arrow.get(ele["posted_at"] or 0).float_timestamp)
+            dict(
+                ele,
+                posted_at=arrow.get(
+                    ele["posted_at"] or ele["created_at"] or 0
+                ).float_timestamp,
+            )
             for ele in data
         ]
 
 
 @run
 @wrapper.operation_wrapper_async
 def get_archived_media(conn=None, model_id=None, **kwargs) -> list:
     with contextlib.closing(conn.cursor()) as cur:
         cur.execute(getArchivedMedia, [model_id])
         data = [dict(row) for row in cur.fetchall()]
         return [
-            dict(ele, posted_at=arrow.get(ele["posted_at"] or 0).float_timestamp)
+            dict(
+                ele,
+                posted_at=arrow.get(
+                    ele["posted_at"] or ele["created_at"] or 0
+                ).float_timestamp,
+            )
             for ele in data
         ]
 
 
 @run
 @wrapper.operation_wrapper_async
 def get_timeline_media(model_id=None, username=None, conn=None, **kwargs) -> list:
```

### Comparing `ofscraper-3.9.4/ofscraper/db/operations_/merge.py` & `ofscraper-3.9.5/ofscraper/db/operations_/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import logging
 import pathlib
 import traceback
 
 import ofscraper.utils.paths.paths as paths
-from ofscraper.db.operations import (
-    create_tables,
-    modify_tables,
-)
+from ofscraper.db.operations import create_tables, modify_tables
 from ofscraper.db.operations_.labels import (
     get_all_labels_transition,
     write_labels_table_transition,
 )
 from ofscraper.db.operations_.media import (
     get_all_medias_transition,
     write_media_table_transition,
@@ -28,60 +25,75 @@
 from ofscraper.db.operations_.posts import (
     get_all_posts_transition,
     write_post_table_transition,
 )
 from ofscraper.db.operations_.profile import (
     get_all_models,
     get_all_profiles,
+    get_single_model_via_profile,
     write_models_table,
     write_profile_table_transition,
-    get_single_model_via_profile
 )
 from ofscraper.db.operations_.stories import (
     get_all_stories_transition,
     write_stories_table_transition,
 )
 from ofscraper.utils.context.run_async import run
 
 log = logging.getLogger("shared")
 
 
 @run
-async def batch_database_changes(new_root, old_root):
+async def batch_database_changes(new_root, old_root, user_dbs=None):
 
     if not pathlib.Path(old_root).is_dir():
         raise FileNotFoundError("Path is not dir")
     old_root = pathlib.Path(old_root)
     new_root = pathlib.Path(new_root)
     new_root.mkdir(exist_ok=True, parents=True)
     new_db_path = new_root / "user_data.db"
     db_merger = MergeDatabase(new_db_path)
 
     await create_tables(db_path=new_db_path)
-    failures=[]
-    for ele in paths.get_all_db(old_root):
+    failures = []
+    for ele in user_dbs or paths.get_all_db(old_root):
         if ele == new_db_path:
             continue
-        log.info(f"Merging {ele} with {new_db_path}")
+        log.info(f"Merging {new_root} with {ele}")
         try:
             model_id = get_single_model_via_profile(db_path=ele)
             if not model_id:
                 raise Exception("Not exactly one model_id in profile table")
             elif not str(model_id).isnumeric():
                 raise Exception("Found model_id was not numeric")
             await create_tables(db_path=ele)
             await modify_tables(model_id=model_id, db_path=ele)
             await db_merger(ele)
 
         except Exception as E:
-            failures.append({"path":str(ele),"reason":E})
+            failures.append({"path": str(ele), "reason": E})
             log.error(f"Issue getting required info for {ele}")
             log.traceback_(E)
             log.traceback_(traceback.format_exc())
-    log.info("\n\n\n".join(list(map(lambda x:str([(key,value) for key,value in x.items()]),failures))))
+    log.info(
+        "\n\n\n".join(
+            list(
+                map(lambda x: str([(key, value) for key, value in x.items()]), failures)
+            )
+        )
+    )
+    return failures
+
+
+@run
+async def merge_single_table(db_merger, ele, model_id):
+    await create_tables(db_path=ele)
+    await modify_tables(model_id=model_id, db_path=ele)
+    db_merger(ele)
+
 
 class MergeDatabase:
     def __init__(self, new_db_path):
         self._data_init = False
         self._new_db = new_db_path
         self._media_keys = ["media_id", "model_id"]
         self._label_keys = ["post_id", "label_id", "model_id"]
```

### Comparing `ofscraper-3.9.4/ofscraper/db/operations_/messages.py` & `ofscraper-3.9.5/ofscraper/db/operations_/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,14 @@
         curr_posts = helpers.converthelper(curr_posts)
         await update_messages_table(curr_posts, model_id=model_id, username=username)
 
 
 async def get_oldest_message_date(model_id=None, username=None, **kwargs):
     data = await media.get_messages_media(model_id=model_id, username=username)
     last_item = sorted(data, key=lambda x: arrow.get(x["posted_at"] or 0))[0]
-    return last_item["posted_at"] or 0
+    return last_item["posted_at"]
 
 
 async def get_youngest_message_date(model_id=None, username=None, **kwargs):
     data = await media.get_messages_media(model_id=model_id, username=username)
     last_item = sorted(data, key=lambda x: arrow.get(x["posted_at"] or 0))[-1]
-    return last_item["posted_at"] or 0
+    return last_item["posted_at"]
```

### Comparing `ofscraper-3.9.4/ofscraper/db/operations_/others.py` & `ofscraper-3.9.5/ofscraper/db/operations_/others.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/db/operations_/posts.py` & `ofscraper-3.9.5/ofscraper/db/operations_/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/db/operations_/profile.py` & `ofscraper-3.9.5/ofscraper/db/operations_/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/db/operations_/stories.py` & `ofscraper-3.9.5/ofscraper/db/operations_/stories.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/db/operations_/wrapper.py` & `ofscraper-3.9.5/ofscraper/db/operations_/wrapper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/alt_download.py` & `ofscraper-3.9.5/ofscraper/download/alt_download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/alt_downloadbatch.py` & `ofscraper-3.9.5/ofscraper/download/alt_downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/download.py` & `ofscraper-3.9.5/ofscraper/download/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 import json
 import logging
 import subprocess
 import traceback
 
-import ofscraper.db.operations as operations
 import ofscraper.download.downloadbatch as batchdownloader
 import ofscraper.download.downloadnormal as normaldownloader
 import ofscraper.filters.media.helpers as helpers
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.config.data as config_data
 import ofscraper.utils.constants as constants
 import ofscraper.utils.hash as hash
 import ofscraper.utils.separate as seperate
 import ofscraper.utils.settings as settings
 import ofscraper.utils.system.system as system
+from ofscraper.db.operations_.media import (
+    get_media_ids_downloaded,
+    get_media_ids_downloaded_model,
+)
 from ofscraper.download.shared.utils.text import textDownloader
-from ofscraper.db.operations_.media import get_media_ids_downloaded,get_media_ids_downloaded_model
-
 
 
 def medialist_filter(medialist, model_id, username):
     log = logging.getLogger("shared")
+    medialist = seperate.seperate_by_self(medialist)
+
     if read_args.retriveArgs().force_all:
         log.info("forcing all")
     elif read_args.retriveArgs().force_model_unique:
         log.info("Downloading unique medi afor model")
         media_ids = set(
-            get_media_ids_downloaded_model(
-                model_id=model_id, username=username
-            )
+            get_media_ids_downloaded_model(model_id=model_id, username=username)
         )
         log.debug(
             f"Number of unique media ids in database for {username}: {len(media_ids)}"
         )
         medialist = seperate.separate_by_id(medialist, media_ids)
         log.debug(f"Number of new mediaids with dupe ids removed: {len(medialist)}")
         medialist = seperate.seperate_avatars(medialist)
         log.debug("Removed previously downloaded avatars/headers")
         log.debug(f"Final Number of media to download {len(medialist)}")
     else:
         log.info("Downloading unique media across all models")
-        media_ids = set(
-            get_media_ids_downloaded(model_id=model_id, username=username)
-        )
+        media_ids = set(get_media_ids_downloaded(model_id=model_id, username=username))
         log.debug("Number of unique media ids in database for all models")
         medialist = seperate.separate_by_id(medialist, media_ids)
         log.debug(f"Number of new mediaids with dupe ids removed: {len(medialist)}")
         medialist = seperate.seperate_avatars(medialist)
         log.debug("Removed previously downloaded avatars/headers")
         log.debug(f"Final Number of media to download {len(medialist)} ")
+
     return medialist
 
 
 def download_process(username, model_id, medialist, posts=None):
     data = None
     if read_args.retriveArgs().metadata:
         medialist = (
```

### Comparing `ofscraper-3.9.4/ofscraper/download/downloadbatch.py` & `ofscraper-3.9.5/ofscraper/download/downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/downloadnormal.py` & `ofscraper-3.9.5/ofscraper/download/downloadnormal.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/main_download.py` & `ofscraper-3.9.5/ofscraper/download/main_download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/main_downloadbatch.py` & `ofscraper-3.9.5/ofscraper/download/main_downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/shared/classes/retries.py` & `ofscraper-3.9.5/ofscraper/download/shared/classes/retries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/shared/classes/session.py` & `ofscraper-3.9.5/ofscraper/download/shared/classes/session.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/shared/common/alt_common.py` & `ofscraper-3.9.5/ofscraper/download/shared/common/alt_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import ofscraper.download.shared.utils.paths as common_paths
 import ofscraper.utils.dates as dates
 import ofscraper.utils.settings as settings
 import ofscraper.utils.system.system as system
 from ofscraper.db.operations_.media import download_media_update
 
 
-
 async def handle_result_alt(
     sharedPlaceholderObj, ele, audio, video, username, model_id
 ):
     tempPlaceholder = await placeholder.tempFilePlaceholder(
         ele, f"temp_{ele.id or await ele.final_filename}.mp4"
     ).init()
     temp_path = tempPlaceholder.tempfilepath
```

### Comparing `ofscraper-3.9.4/ofscraper/download/shared/common/general.py` & `ofscraper-3.9.5/ofscraper/download/shared/common/general.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/shared/common/main_common.py` & `ofscraper-3.9.5/ofscraper/download/shared/common/main_common.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import arrow
 
 import ofscraper.download.shared.common.general as common
 import ofscraper.download.shared.globals as common_globals
 import ofscraper.download.shared.utils.log as common_logs
 import ofscraper.download.shared.utils.paths as common_paths
 import ofscraper.utils.dates as dates
-from ofscraper.db.operations_.media import download_media_update
 import ofscraper.utils.system.system as system
+from ofscraper.db.operations_.media import download_media_update
 
 
 async def handle_result_main(result, ele, username, model_id):
     total, temp, placeholderObj = result
     path_to_file = placeholderObj.trunicated_filepath
     await common.size_checker(temp, ele, total)
     common_globals.log.debug(
```

### Comparing `ofscraper-3.9.4/ofscraper/download/shared/globals.py` & `ofscraper-3.9.5/ofscraper/download/shared/globals.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/shared/utils/keyhelpers.py` & `ofscraper-3.9.5/ofscraper/download/shared/utils/keyhelpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/shared/utils/log.py` & `ofscraper-3.9.5/ofscraper/download/shared/utils/log.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/shared/utils/message.py` & `ofscraper-3.9.5/ofscraper/download/shared/utils/message.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/shared/utils/metadata.py` & `ofscraper-3.9.5/ofscraper/download/shared/utils/metadata.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import ofscraper.db.operations as operations
 import ofscraper.download.shared.common.general as common
 import ofscraper.download.shared.globals as common_globals
 import ofscraper.download.shared.utils.media as media
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.cache as cache
 import ofscraper.utils.constants as constants
-from ofscraper.download.shared.utils.log import get_medialog
 from ofscraper.db.operations_.media import download_media_update
+from ofscraper.download.shared.utils.log import get_medialog
 
 
 async def force_download(ele, username, model_id):
     await download_media_update(
         ele,
         filename=None,
         model_id=model_id,
```

### Comparing `ofscraper-3.9.4/ofscraper/download/shared/utils/paths.py` & `ofscraper-3.9.5/ofscraper/download/shared/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/download/shared/utils/text.py` & `ofscraper-3.9.5/ofscraper/download/shared/utils/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/filters/media/helpers.py` & `ofscraper-3.9.5/ofscraper/filters/media/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/filters/media/main.py` & `ofscraper-3.9.5/ofscraper/filters/media/main.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/filters/models/date.py` & `ofscraper-3.9.5/ofscraper/filters/models/date.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/filters/models/flags.py` & `ofscraper-3.9.5/ofscraper/filters/models/flags.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/filters/models/helpers.py` & `ofscraper-3.9.5/ofscraper/filters/models/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/filters/models/other.py` & `ofscraper-3.9.5/ofscraper/filters/models/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/filters/models/price.py` & `ofscraper-3.9.5/ofscraper/filters/models/price.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/filters/models/sort.py` & `ofscraper-3.9.5/ofscraper/filters/models/sort.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/filters/models/subtype.py` & `ofscraper-3.9.5/ofscraper/filters/models/subtype.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/models/retriver.py` & `ofscraper-3.9.5/ofscraper/models/retriver.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             return await get_via_list(count)
         elif "ALL" in read_args.retriveArgs().usernames:
             return await get_via_list(count)
         elif read_args.retriveArgs().individual:
             return await get_via_individual()
         elif read_args.retriveArgs().list:
             return get_via_list(count)
-        elif (sum(count) // 10) > len(read_args.retriveArgs().usernames):
+        elif (sum(count) // 10) >= len(read_args.retriveArgs().usernames):
             return await get_via_individual()
         else:
             return await get_via_list(count)
 
 
 async def get_via_list(count):
     out = []
@@ -78,12 +78,11 @@
     to the model(s) whose content they would like to scrape.
     """
     return prompts.model_selector(parsed_subscriptions)
 
 
 # check if auth is valid
 def get_sub_count():
-    my_profile = me.scrape_user()
-    name, username = me_util.parse_user(my_profile)
+    name, username = me_util.parse_user()
     subscribe_count = me.parse_subscriber_count()
     me_util.print_user(name, username)
     return subscribe_count
```

### Comparing `ofscraper-3.9.4/ofscraper/models/selector.py` & `ofscraper-3.9.5/ofscraper/models/selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,21 @@
         read_args.retriveArgs().usernames = list(map(lambda x: x.name, selectedusers))
         PARSED_SUBS = selectedusers
         write_args.setArgs(args)
     elif "ALL" in args.usernames:
         PARSED_SUBS = filterNSort()
     elif args.usernames:
         usernameset = set(args.usernames)
-        PARSED_SUBS = list(filter(lambda x: x.name or x.id in usernameset, ALL_SUBS))
+        PARSED_SUBS = list(
+            filter(
+                lambda x: (x.name in usernameset) or (str(x.id) in usernameset),
+                ALL_SUBS,
+            )
+        )
+
     return PARSED_SUBS
 
 
 def setfilter(forced=False):
     global args
     while True:
         choice = prompts.decide_filters_menu()
```

### Comparing `ofscraper-3.9.4/ofscraper/prompts/helpers/model_helpers.py` & `ofscraper-3.9.5/ofscraper/prompts/helpers/model_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/prompts/helpers/prompt_helpers.py` & `ofscraper-3.9.5/ofscraper/prompts/helpers/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/prompts/keybindings.py` & `ofscraper-3.9.5/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/prompts/promptConvert.py` & `ofscraper-3.9.5/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/actions.py` & `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/area.py` & `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/area.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/auth.py` & `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/binary.py` & `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/binary.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/config.py` & `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,15 +469,15 @@
                 "choices": ["deviint", "digitalcriminals", "sneaky"],
             },
             {
                 "type": "list",
                 "name": "cache-mode",
                 "message": "sqlite should be fine unless your using a network drive\nSee https://grantjenks.com/docs/diskcache/tutorial.html#caveats ",
                 "default": data.cache_mode_helper(),
-                "choices": ["sqlite", "json", "disabled","api_disabled"],
+                "choices": ["sqlite", "json", "disabled", "api_disabled"],
             },
             {
                 "type": "list",
                 "name": "backend",
                 "choices": [Choice("aio", "aiohttp"), Choice("httpx", "httpx")],
                 "message": "Select Which Backend you want:\n",
                 "default": data.get_backend() or "",
```

### Comparing `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/menu.py` & `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/merge.py` & `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/merge.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,12 +75,28 @@
                 "message": "Confirm merge: ",
                 "instruction": f"user_data.db files from {folder} will be merged into {str(pathlib.Path(new_db,'user_data.db'))}",
                 "choices": [
                     Choice(True, "Yes"),
                     Choice(False, "No"),
                     Choice(None, "Back to Main Menu"),
                 ],
-                "default":False
+                "default": False,
             }
         ]
     )
     return answer[name]
+
+
+def model_id_prompt():
+    answer = promptClasses.batchConverter(
+        *[
+            {
+                "type": "inpit",
+                "name": "database",
+                "message": "Username/UD: ",
+                "option_instruction": """
+                Preferably the model ID
+                """,
+            },
+        ]
+    )
+    return answer["database"]
```

### Comparing `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/model.py` & `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/model.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/prompts/prompt_groups/profile.py` & `ofscraper-3.9.5/ofscraper/prompts/prompt_groups/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/prompts/prompt_strings.py` & `ofscraper-3.9.5/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/prompts/prompt_validators.py` & `ofscraper-3.9.5/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/prompts/prompts.py` & `ofscraper-3.9.5/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/runner/exit.py` & `ofscraper-3.9.5/ofscraper/runner/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/runner/load.py` & `ofscraper-3.9.5/ofscraper/runner/load.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/runner/run.py` & `ofscraper-3.9.5/ofscraper/runner/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/actions.py` & `ofscraper-3.9.5/ofscraper/utils/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/args/areas.py` & `ofscraper-3.9.5/ofscraper/utils/args/areas.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/args/groups/common_args.py` & `ofscraper-3.9.5/ofscraper/utils/args/groups/common_args.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import functools
 import itertools
 import re
 
 import cloup as click
+from humanfriendly import parse_size
 
 import ofscraper.utils.args.helpers as helpers
 from ofscraper.__version__ import __version__
 from ofscraper.const.constants import KEY_OPTIONS
 
 
 def common_params(func):
@@ -69,44 +70,15 @@
             ),
             default="NORMAL",
             callback=lambda ctx, param, value: value.upper() if value else None,
         ),
         help="Settings for logging",
     )
     @click.option_group(
-        "Advanced Program Options",
-        click.option(
-            "-nc",
-            "--no-cache",
-            help="Disable cache and forces consecutive api scan",
-            default=False,
-            is_flag=True,
-        ),
-        click.option(
-            "-nca",
-            "--no-api-cache",
-            help="Forces consecutive api scan",
-            default=False,
-            is_flag=True,
-        ),
-        click.option(
-            "-k",
-            "--key-mode",
-            help="Key mode override",
-            default=None,
-            type=click.Choice(KEY_OPTIONS),
-        ),
-        click.option(
-            "-dr",
-            "--dynamic-rules",
-            help="Dynamic signing",
-            default=None,
-            type=click.Choice(["dc", "deviint", "sneaky"], case_sensitive=False),
-            callback=lambda ctx, param, value: value.lower() if value else None,
-        ),
+        "Download Options",
         click.option(
             "-ar",
             "--no-auto-resume",
             help="Cleanup temp .part files (removes resume ability)",
             default=False,
             is_flag=True,
         ),
@@ -127,21 +99,18 @@
         click.option(
             "-dp",
             "--downloadthreads",
             help="Number of threads to use (minimum 1)",
             default=None,
             type=int,
         ),
-        click.option(
-            "-up",
-            "--update-profile",
-            help="Get up-to-date profile info instead of cache",
-            default=False,
-            is_flag=True,
-        ),
+        help="Options for downloads and download performance",
+    )
+    @click.option_group(
+        "Metadata Options",
         click.option(
             "-md",
             "--metadata",
             "metadata",
             help="""
             \b
             Skip media downloads and gather metadata only 
@@ -165,14 +134,63 @@
             "metadata",
             help="""
             \b
             Skip media downloads, gather metadata, and mark all media as downloaded 
             [select one --metadata or --metadata-update or --metadata-complete]""",
             flag_value="complete",
         ),
+        help="Options generating metadata",
+    )
+    @functools.wraps(func)
+    @click.pass_context
+    def wrapper(ctx, *args, **kwargs):
+        return func(ctx, *args, **kwargs)
+
+    return wrapper
+
+
+def common_advanced_params(func):
+    @click.option_group(
+        "Advanced Program Options",
+        click.option(
+            "-nc",
+            "--no-cache",
+            help="Disable cache and forces consecutive api scan",
+            default=False,
+            is_flag=True,
+        ),
+        click.option(
+            "-nca",
+            "--no-api-cache",
+            help="Forces consecutive api scan",
+            default=False,
+            is_flag=True,
+        ),
+        click.option(
+            "-k",
+            "--key-mode",
+            help="Key mode override",
+            default=None,
+            type=click.Choice(KEY_OPTIONS),
+        ),
+        click.option(
+            "-dr",
+            "--dynamic-rules",
+            help="Dynamic signing",
+            default=None,
+            type=click.Choice(["dc", "deviint", "sneaky"], case_sensitive=False),
+            callback=lambda ctx, param, value: value.lower() if value else None,
+        ),
+        click.option(
+            "-up",
+            "--update-profile",
+            help="Get up-to-date profile info instead of using cache",
+            default=False,
+            is_flag=True,
+        ),
         click.option(
             "-ds",
             "--download-script",
             "download_script",
             help="""
             \b
             runs a script post model download
@@ -187,67 +205,73 @@
         return func(ctx, *args, **kwargs)
 
     return wrapper
 
 
 def common_other_params(func):
     @click.option_group(
-        "Downloading options",
+        "Media Filters",
         click.option(
             "-q",
             "--quality",
             type=click.Choice(["240", "720", "source"], case_sensitive=False),
         ),
         click.option(
-            "-lb",
-            "--label",
-            help="Filter by label (use helpers.label_helper to process)",
+            "-mt",
+            "--mediatype",
+            help="Filter by media type (Videos, Audios, Images)",
             default=[],
             required=False,
-            type=helpers.label_helper,
+            type=helpers.mediatype_helper,
             callback=lambda ctx, param, value: (
                 list(set(itertools.chain.from_iterable(value))) if value else []
             ),
             multiple=True,
         ),
-        help="Options for controlling download behavior",
+        click.option(
+            "-sx",
+            "--size-max",
+            help="Filter out files larger than the given size (bytes or human-readable, e.g., 10mb)",
+            required=False,
+            type=parse_size,
+        ),
+        click.option(
+            "-sm",
+            "--size-min",
+            help="Filter out files smaller than the given size (bytes or human-readable, e.g., 10mb)",
+            required=False,
+            type=parse_size,
+        ),
+        help="Options for controlling which media is downloaded",
     )
-
     @click.option_group(
         "Filename Modification options",
         click.option(
             "-g",
             "--original",
             help="Don't truncate long paths",
             is_flag=True,
         ),
-
         click.option(
             "-tt",
             "--text-type",
             help="set length based on word or letter",
             type=click.Choice(["word", "letter"], case_sensitive=False),
+            default="word",
         ),
-
         click.option(
             "-sr",
             "--space-replacer",
             help="character to replace spaces with",
         ),
-        click.option(
-            "-tl",
-            "--textlength",
-            help="max length of text",
-            type=click.INT
-        ),
-help="""
+        click.option("-tl", "--textlength", help="max length of text", type=click.INT),
+        help="""
 \b
 Options for controlling the output of the final filename after placeholders are replaced
-"""
-     )
-
+""",
+    )
     @functools.wraps(func)
     @click.pass_context
     def wrapper(ctx, *args, **kwargs):
         return func(ctx, *args, **kwargs)
 
     return wrapper
```

### Comparing `ofscraper-3.9.4/ofscraper/utils/args/groups/main_args.py` & `ofscraper-3.9.5/ofscraper/utils/args/groups/main_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,19 @@
 
 
 @click.group(
     help="OF-Scraper Options",
     context_settings=dict(help_option_names=["-h", "--help"]),
     invoke_without_command=True,
 )
+@common.common_params
+@common.common_other_params
 @click.option_group(
     "Content Options",
     click.option(
-        "-q",
-        "--quality",
-        type=click.Choice(["240", "720", "source"], case_sensitive=False),
-    ),
-    click.option(
         "-o",
         "--posts",
         "--post",
         help="""
         Select areas for batch actions (comma or space separated).
         Options: HighLights, Archived, Messages, Timeline, Pinned, Stories, Purchased, Profile, Labels, All
         """,
@@ -137,30 +134,14 @@
             "--dupe-model",
             "--force_model_unique",
             help="Only download files not present for the current model in the database",
             default=False,
             is_flag=True,
         ),
     ),
-    click.constraints.mutually_exclusive(
-        click.option(
-            "-to",
-            "--protected-only",
-            help="Only download content that requires decryption",
-            default=False,
-            is_flag=True,
-        ),
-        click.option(
-            "-no",
-            "--normal-only",
-            help="Only download content that does not require decryption",
-            default=False,
-            is_flag=True,
-        ),
-    ),
     click.option(
         "-lb",
         "--label",
         help="Filter by label (use helpers.label_helper to process)",
         default=[],
         required=False,
         type=helpers.label_helper,
@@ -178,40 +159,14 @@
     click.option(
         "-af",
         "--after",
         help="Process posts at or after the given date (MM/DD/YYYY) for likes, unlikes, and downloads",
         type=helpers.arrow_helper,
     ),
     click.option(
-        "-mt",
-        "--mediatype",
-        help="Filter by media type (Videos, Audios, Images)",
-        default=[],
-        required=False,
-        type=helpers.mediatype_helper,
-        callback=lambda ctx, param, value: (
-            list(set(itertools.chain.from_iterable(value))) if value else []
-        ),
-        multiple=True,
-    ),
-    click.option(
-        "-sx",
-        "--size-max",
-        help="Filter out files larger than the given size (bytes or human-readable, e.g., 10mb)",
-        required=False,
-        type=parse_size,
-    ),
-    click.option(
-        "-sm",
-        "--size-min",
-        help="Filter out files smaller than the given size (bytes or human-readable, e.g., 10mb)",
-        required=False,
-        type=parse_size,
-    ),
-    click.option(
         "-mm/-ms",
         "--mass-only/--mass-skip",
         "mass_msg",
         help="""
         \b
         Flag for enabling/disabling mass content or promos 
         [select one --mass-only or --mass-skip]""",
@@ -259,14 +214,15 @@
 )
 @click.option_group(
     "User Selection Options",
     click.option(
         "-u",
         "--usernames",
         "--username",
+        # "username",
         help="Select which username to process (name,name2). Set to ALL for all users",
         default=None,
         type=helpers.username_helper,  # Assuming you'll still use this helper function
         multiple=True,  # Use `multiple=True` for accepting multiple values
         callback=lambda ctx, param, value: (
             list(set(itertools.chain.from_iterable(value))) if value else []
         ),
@@ -409,15 +365,15 @@
     click.option(
         "-ao",
         "--all-promo-only/--all-promo-skip",
         "all_promo",
         help="""
             \b
             Flag for enabling/disabling  accounts with any promo price
-            [select one ppall-promo-only or --all-promo-skip]""",
+            [select one all-promo-only or --all-promo-skip]""",
         default=None,
         required=False,
         is_flag=True,
     ),
     click.option(
         "-ts/-es",
         "--active-subscription/--expired-subscription",
@@ -625,12 +581,11 @@
             help="Search entire enabled lists before filtering for usernames when --username is provided",
             default=False,
             is_flag=True,
         ),
     ),
     help="Choose how usernames are searched, and define the order in which users are processed for actions",
 )
-@common.common_other_params
-@common.common_params
+@common.common_advanced_params
 @click.pass_context
 def program(ctx, *args, **kwargs):
     return ctx.params, ctx.info_name
```

### Comparing `ofscraper-3.9.4/ofscraper/utils/args/groups/manual_args.py` & `ofscraper-3.9.5/ofscraper/utils/args/groups/manual_args.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 
 @click.command(
     "manual",
     help="Manually download media by providing a list of urls or IDs",
     short_help="Manually download media by providing a list of urls or IDs",
 )
+@common.common_params
+@common.common_other_params
 @click.constraints.require_one(
     click.option(
         "-u",
         "--url",
         help="A space or comma seperated list of urls to download",
         default=None,
         multiple=True,
@@ -38,12 +40,11 @@
 @click.option(
     "-fo",
     "--force",
     help="Force retrieval of new messages info from API",
     is_flag=True,
     default=False,
 )
-@common.common_other_params
-@common.common_params
+@common.common_advanced_params
 @click.pass_context
 def manual(ctx, *args, **kwargs):
     return ctx.params, ctx.info_name
```

### Comparing `ofscraper-3.9.4/ofscraper/utils/args/groups/message_args.py` & `ofscraper-3.9.5/ofscraper/utils/args/groups/message_args.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
                Produces a media table from messages with filterable entries and quick downloads""",
     help="""
 The msg_check subcommand gathers information on media content from messages
 It presents this data in a table format with filtering options for focused searches 
 Allows unlocked media entries to be directly downloaded through the table
 """,
 )
+@common.common_params
+@common.common_other_params
 @click.constraints.require_one(
     click.option(
         "-u",
         "--url",
         help="Scan messages via space or comma seperated list of urls",
         default=None,
         multiple=True,
@@ -43,12 +45,11 @@
 @click.option(
     "-fo",
     "--force",
     help="Force retrieval of new messages info from API",
     is_flag=True,
     default=False,
 )
-@common.common_other_params
-@common.common_params
+@common.common_advanced_params
 @click.pass_context
 def message_check(ctx, *args, **kwargs):
     return ctx.params, ctx.info_name
```

### Comparing `ofscraper-3.9.4/ofscraper/utils/args/groups/paid_args.py` & `ofscraper-3.9.5/ofscraper/utils/args/groups/paid_args.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
                Produces a media table from purchases with filterable entries and quick downloads""",
     help="""
 The paid_check subcommand gathers information on media content from purchases
 It presents this data in a table format with filtering options for focused searches 
 Allows unlocked media entries to be directly downloaded through the table
 """,
 )
+@common.common_params
+@common.common_other_params
 @click.constraints.require_one(
     click.option(
         "-u",
         "--usernames",
         "--username",
         "check_usernames",
         help="Scan purchases via username(s)",
@@ -45,12 +47,11 @@
 @click.option(
     "-fo",
     "--force",
     help="Force retrieval of new purchases info from API",
     is_flag=True,
     default=False,
 )
-@common.common_other_params
-@common.common_params
+@common.common_advanced_params
 @click.pass_context
 def paid_check(ctx, *args, **kwargs):
     return ctx.params, ctx.info_name
```

### Comparing `ofscraper-3.9.4/ofscraper/utils/args/groups/post_args.py` & `ofscraper-3.9.5/ofscraper/utils/args/groups/post_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     "post_check",
     short_help="""\b
                Produces a media table from posts with filterable entries and quick downloads""",
     help="""The post_check subcommand gathers information on media content from posts
 It presents this data in a table format with filtering options for focused searches 
 Allows unlocked media entries to be directly downloaded through the table""",
 )
+@common.common_params
+@common.common_other_params
 @click.constraints.require_one(
     click.option(
         "-u",
         "--url",
         help="Scan posts via space or comma seperated list of urls",
         default=None,
         multiple=True,
@@ -54,12 +56,11 @@
         ["Timeline", "Pinned", "Archived", "Labels"], case_sensitive=False
     ),
     callback=lambda ctx, param, value: (
         list(set(helpers.post_check_area(value))) if value else None
     ),
     multiple=True,
 )
-@common.common_other_params
-@common.common_params
+@common.common_advanced_params
 @click.pass_context
 def post_check(ctx, *args, **kwargs):
     return ctx.params, ctx.info_name
```

### Comparing `ofscraper-3.9.4/ofscraper/utils/args/groups/story_args.py` & `ofscraper-3.9.5/ofscraper/utils/args/groups/story_args.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,16 @@
                Produces a media table from stories and highlights with filterable entries and quick downloads""",
     help="""
 The story_check subcommand gathers information on media content from stories and highlights
 It presents this data in a table format with filtering options for focused searches 
 Allows unlocked media entries to be directly downloaded through the table
 """,
 )
+@common.common_params
+@common.common_other_params
 @click.constraints.require_one(
     click.option(
         "-u",
         "--usernames",
         "--username",
         "check_usernames",
         help="Scan stories/highlights via username(s)",
@@ -45,12 +47,11 @@
 @click.option(
     "-fo",
     "--force",
     help="Force retrieval of new messages info from API",
     is_flag=True,
     default=False,
 )
-@common.common_other_params
-@common.common_params
+@common.common_advanced_params
 @click.pass_context
 def story_check(ctx, *args, **kwargs):
     return ctx.params, ctx.info_name
```

### Comparing `ofscraper-3.9.4/ofscraper/utils/args/helpers.py` & `ofscraper-3.9.5/ofscraper/utils/args/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/args/parse.py` & `ofscraper-3.9.5/ofscraper/utils/args/parse.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/args/read.py` & `ofscraper-3.9.5/ofscraper/utils/args/read.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import sys
 
 import ofscraper.utils.args.globals as global_args
 import ofscraper.utils.args.parse as parse_args
 import ofscraper.utils.manager as manager
 
 
@@ -16,12 +17,14 @@
         raise E
 
 
 def retriveArgs():
     try:
         if not global_args.args:
             global_args.args = parse_args.parse_args()
+            logging.getLogger("shared").debug(f"args set to {global_args.args}")
+
         return global_args.args
     except SystemExit as E:
         if not any(ele in sys.argv[1:] for ele in ["-h", "-v"]):
             print(f"Passed Args {sys.argv[1:]}")
         raise E
```

### Comparing `ofscraper-3.9.4/ofscraper/utils/args/user.py` & `ofscraper-3.9.5/ofscraper/utils/args/user.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/auth/context.py` & `ofscraper-3.9.5/ofscraper/utils/auth/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/auth/data.py` & `ofscraper-3.9.5/ofscraper/utils/auth/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/auth/file.py` & `ofscraper-3.9.5/ofscraper/utils/auth/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/auth/helpers.py` & `ofscraper-3.9.5/ofscraper/utils/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/auth/make.py` & `ofscraper-3.9.5/ofscraper/utils/auth/make.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/auth/request.py` & `ofscraper-3.9.5/ofscraper/utils/auth/request.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/auth/schema.py` & `ofscraper-3.9.5/ofscraper/utils/auth/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/binaries.py` & `ofscraper-3.9.5/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/cache.py` & `ofscraper-3.9.5/ofscraper/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/checkers.py` & `ofscraper-3.9.5/ofscraper/utils/checkers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/config/config.py` & `ofscraper-3.9.5/ofscraper/utils/config/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/config/context.py` & `ofscraper-3.9.5/ofscraper/utils/config/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/config/custom.py` & `ofscraper-3.9.5/ofscraper/utils/config/custom.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/config/data.py` & `ofscraper-3.9.5/ofscraper/utils/config/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/config/file.py` & `ofscraper-3.9.5/ofscraper/utils/config/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/config/menu.py` & `ofscraper-3.9.5/ofscraper/utils/config/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/config/schema.py` & `ofscraper-3.9.5/ofscraper/utils/config/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/constants.py` & `ofscraper-3.9.5/ofscraper/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/context/exit.py` & `ofscraper-3.9.5/ofscraper/utils/context/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/context/run_async.py` & `ofscraper-3.9.5/ofscraper/utils/context/run_async.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/context/stdout.py` & `ofscraper-3.9.5/ofscraper/utils/context/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/dates.py` & `ofscraper-3.9.5/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/encoding.py` & `ofscraper-3.9.5/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/hash.py` & `ofscraper-3.9.5/ofscraper/utils/hash.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 import xxhash
 
 import ofscraper.classes.placeholder as placeholder
 import ofscraper.db.operations as operations
 import ofscraper.utils.config.data as config_data
 import ofscraper.utils.constants as constants
-from ofscraper.db.operations_.media import get_dupe_media_files,get_dupe_media_hashes
-
+from ofscraper.db.operations_.media import get_dupe_media_files, get_dupe_media_hashes
 
 log = logging.getLogger("shared")
 
 
 fileHashes = {}
 
 
@@ -38,19 +37,15 @@
     log.debug(f"{file_data} => hash: {hash}")
     return hash
 
 
 def remove_dupes_hash(username, model_id, mediatype=None):
     if not config_data.get_hash(mediatype=mediatype):
         return
-    hashes = get_dupe_media_hashes(
-        username=username, model_id=model_id, mediatype=None
-    )
+    hashes = get_dupe_media_hashes(username=username, model_id=model_id, mediatype=None)
     for hash in hashes:
-        files = get_dupe_media_files(
-            username=username, model_id=model_id, hash=hash
-        )
+        files = get_dupe_media_files(username=username, model_id=model_id, hash=hash)
         filter_files = list(filter(lambda x: pathlib.Path(x).is_file(), files))
         if len(filter_files) < 2:
             continue
         [pathlib.Path(ele).unlink(missing_ok=True) for ele in filter_files[1:]]
     #
```

### Comparing `ofscraper-3.9.4/ofscraper/utils/logs/classes.py` & `ofscraper-3.9.5/ofscraper/utils/logs/classes.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/logs/close.py` & `ofscraper-3.9.5/ofscraper/utils/logs/close.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/logs/helpers.py` & `ofscraper-3.9.5/ofscraper/utils/logs/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/logs/logger.py` & `ofscraper-3.9.5/ofscraper/utils/logs/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/logs/logs.py` & `ofscraper-3.9.5/ofscraper/utils/logs/logs.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/logs/other.py` & `ofscraper-3.9.5/ofscraper/utils/logs/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/logs/stdout.py` & `ofscraper-3.9.5/ofscraper/utils/logs/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/manager.py` & `ofscraper-3.9.5/ofscraper/utils/manager.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/menu.py` & `ofscraper-3.9.5/ofscraper/utils/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/merge.py` & `ofscraper-3.9.5/ofscraper/utils/merge.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,10 +14,20 @@
         folder = prompts.folder_prompt_db()
         new_db_folder = prompts.new_db_prompt()
         confirm = prompts.confirm_prompt_db(folder, new_db_folder)
         if confirm is False:
             continue
         elif confirm is None:
             break
-        else:
-            merge.batch_database_changes(new_db_folder, folder)
-            break
+    merge_loop(new_db_folder, folder)
+
+
+def merge_loop(new_db_folder, folder):
+    db_merger = merge.MergeDatabase()
+    while True:
+        failures = merge.batch_database_changes(new_db_folder, folder)
+        # if len(failures)==0:
+        #     return
+        # for failure in failures:
+        #     print("[red]Please read the following selections carfully[/red]")
+        #     model_id=prompts.model_id_prompt()
+        #     if model_id.isnumeric():
```

### Comparing `ofscraper-3.9.4/ofscraper/utils/paths/check.py` & `ofscraper-3.9.5/ofscraper/utils/paths/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/paths/common.py` & `ofscraper-3.9.5/ofscraper/utils/paths/common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/paths/paths.py` & `ofscraper-3.9.5/ofscraper/utils/paths/paths.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,18 +47,18 @@
                 data.get_TempDir(mediatype="videos")
                 or common_paths.get_save_location(mediatype="videos"),
                 data.get_TempDir(mediatype="images")
                 or common_paths.get_save_location(mediatype="imaegs"),
             ]
         )
         for ele in roots:
-            if ele is None:
+            if ele == None:
                 continue
             for file in filter(
-                lambda x: re.search("\.part$|^temp_", str(x)) is not None,
+                lambda x: re.search("\.part$|^temp_", str(x)) != None,
                 pathlib.Path(ele).glob("**/*"),
             ):
                 file.unlink(missing_ok=True)
 
 
 def truncate(path):
     path = pathlib.Path(os.path.normpath(path))
@@ -69,33 +69,47 @@
     elif platform.system() == "Darwin":
         return _mac_truncateHelper(path)
     else:
         return pathlib.Path(path)
 
 
 def _windows_truncateHelper(path):
+    encode = "utf16"
     path = pathlib.Path(os.path.normpath(path))
-    if len(str(path)) <= constants.getattr("WINDOWS_MAX_PATH"):
+    if len(str(path).encode("utf16")) <= constants.getattr("WINDOWS_MAX_PATH_BYTES"):
         return path
     path = pathlib.Path(path)
     dir = path.parent
     file = path.name
     match = re.search("_[0-9]+\.[a-z4]*$", path.name, re.IGNORECASE) or re.search(
         "\.[a-z4]*$", path.name, re.IGNORECASE
     )
     if match:
         ext = match.group(0)
     else:
         ext = ""
-    # -1 is for / between parentdirs and file
-    fileLength = constants.getattr("WINDOWS_MAX_PATH") - len(ext) - len(str(dir)) - 1
-    newFile = f"{re.sub(ext,'',file)[:fileLength]}{ext}"
-    final = pathlib.Path(dir, newFile)
-    log.debug(f"path: {final} path size: {len(str(final))}")
-    return pathlib.Path(dir, newFile)
+    file = re.sub(ext, "", path.name)
+    max_bytes = (
+        constants.getattr("WINDOWS_MAX_PATH_BYTES")
+        - len(ext.encode(encode))
+        - len(str(dir).encode(encode))
+    )
+    if max_bytes <= 0:
+        raise (f"dir to larger then max bytes {path}")
+    low, high = 0, len(file)
+    while low < high:
+        mid = (low + high) // 2
+        if len(file[:mid].encode(encode)) <= max_bytes:
+            low = mid + 1
+        else:
+            high = mid
+    newFile = f"{file[:high]}{ext}"
+    final_path = pathlib.Path(dir, newFile)
+    log.debug(f"path: {path} filepath bytesize: {len(path.encode(encode))}")
+    return final_path
 
 
 def _mac_truncateHelper(path):
     path = pathlib.Path(os.path.normpath(path))
     if len(str(path)) <= constants.getattr("MAC_MAX_PATH"):
         return path
     dir = path.parent
@@ -109,58 +123,39 @@
     final = pathlib.Path(dir, newFile)
     log.debug(f"path: {final} path size: {len(str(final))}")
     log.debug(f"path: {final} filename size: {len(str(final.name))}")
     return pathlib.Path(dir, newFile)
 
 
 def _linux_truncateHelper(path):
+    encode = "utf8"
     path = pathlib.Path(os.path.normpath(path))
     dir = path.parent
     match = re.search("_[0-9]+\.[a-z4]*$", path.name, re.IGNORECASE) or re.search(
         "\.[a-z4]*$", path.name, re.IGNORECASE
     )
     ext = match.group(0) if match else ""
     file = re.sub(ext, "", path.name)
-    maxbytes = constants.getattr("LINUX_MAX_FILE") - len(ext.encode("utf8"))
-    small = 0
-    large = len(file)
-    target = None
-    maxLength = constants.getattr("LINUX_MAX_FILE") - len(ext)
-    if len(path.name.encode("utf8")) <= maxbytes:
-        target = large
-    while True and not target:
-        if len(file[:large].encode("utf8")) == maxbytes:
-            target = large
-        elif len(file[:small].encode("utf8")) == maxbytes:
-            target = small
-        elif large == small:
-            target = large
-        elif large == small + 1:
-            target = small
-        elif len(file[:large].encode("utf8")) > maxbytes:
-            large = int((small + large) / 2)
-        elif len(file[:large].encode("utf8")) < maxbytes:
-            small = large
-            large = int((large + maxLength) / 2)
-    newFile = f"{file[:target]}{ext}"
-    log.debug(f"path: {path} filename bytesize: {len(newFile.encode('utf8'))}")
+    max_bytes = constants.getattr("LINUX_MAX_FILE_NAME_BYTES") - len(ext.encode(encode))
+    low, high = 0, len(file)
+    while low < high:
+        mid = (low + high) // 2
+        if len(file[:mid].encode(encode)) <= max_bytes:
+            low = mid + 1
+        else:
+            high = mid
+    newFile = f"{file[:high]}{ext}"
+    log.debug(f"path: {path} filename bytesize: {len(newFile.encode(encode))}")
     return pathlib.Path(dir, newFile)
 
 
 def cleanDB():
     try:
         pathlib.Path(common_paths.get_profile_path() / "db.lock").unlink(
             missing_ok=True
         )
     except PermissionError:
         None
 
 
 def speed_file():
     return pathlib.Path(common_paths.get_profile_path() / "speed.zip")
-
-
-def get_all_db(path):
-    for ele in filter(
-        lambda x: re.search("user_data.db$", str(x)) and not re.search("(backup.db|_copy)",str(x)), pathlib.Path(path).glob("**/*")
-    ):
-        yield ele
```

### Comparing `ofscraper-3.9.4/ofscraper/utils/profiles/data.py` & `ofscraper-3.9.5/ofscraper/utils/profiles/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/profiles/manage.py` & `ofscraper-3.9.5/ofscraper/utils/profiles/manage.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/profiles/tools.py` & `ofscraper-3.9.5/ofscraper/utils/profiles/tools.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/progress.py` & `ofscraper-3.9.5/ofscraper/utils/progress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/run.py` & `ofscraper-3.9.5/ofscraper/utils/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/separate.py` & `ofscraper-3.9.5/ofscraper/utils/separate.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 | |   | || (                   ) || |      | (\ (   | (   ) || (      | (      | (\ (   
 | (___) || )             /\____) || (____/\| ) \ \__| )   ( || )      | (____/\| ) \ \__
 (_______)|/              \_______)(_______/|/   \__/|/     \||/       (_______/|/   \__/
                                                                                       
 """
 
 import ofscraper.utils.cache as cache
+import ofscraper.utils.constants as constants
+import ofscraper.utils.me as me_util
 
 
 def separate_by_id(data: list, media_ids: list) -> list:
     media_ids = set(media_ids)
     return list(filter(lambda x: x.id not in media_ids, data))
 
 
@@ -28,10 +30,11 @@
     if ele.postid and ele.responsetype == "profile":
         value = cache.get(ele.postid, default=False)
         cache.close()
         return value
     return False
 
 
-# def separate_database_results_by_id(results: list, media_ids: list) -> list:
-#     filtered_results = [r for r in results if r[0] not in media_ids]
-#     return filtered_results
+def seperate_by_self(data):
+    my_id = me_util.get_id()
+    if constants.getattr("FILTER_SELF_MEDIA"):
+        return list(filter(lambda x: x.post.fromuser != my_id, data))
```

### Comparing `ofscraper-3.9.4/ofscraper/utils/settings.py` & `ofscraper-3.9.5/ofscraper/utils/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,38 +50,42 @@
     return (
         read_args.retriveArgs().original
         or not config_data.get_truncation(mediatype=mediatype)
     ) is False
 
 
 def get_text_type(mediatype=None):
-    return (
-        read_args.retriveArgs().text_type or config_data.get_textType(mediatype=mediatype)
+    return read_args.retriveArgs().text_type or config_data.get_textType(
+        mediatype=mediatype
     )
 
 
 def get_space_replacer(mediatype=None):
-    return (
-        read_args.retriveArgs().space_replacer or config_data.get_spacereplacer(mediatype=mediatype)
+    return read_args.retriveArgs().space_replacer or config_data.get_spacereplacer(
+        mediatype=mediatype
     )
 
 
 def get_textlength(mediatype=None):
-    return (
-        read_args.retriveArgs().text_length or config_data.get_textlength(mediatype=mediatype)
+    return read_args.retriveArgs().text_length or config_data.get_textlength(
+        mediatype=mediatype
     )
 
+
 def get_cache_disabled():
     return (
         read_args.retriveArgs().no_cache or config_data.get_cache_mode() == "disabled"
     )
 
+
 def get_api_cache_disabled():
-     return (
-        read_args.retriveArgs().no_cache or read_args.retriveArgs().no_api_cache or config_data.get_cache_mode() == "api_disabled"
+    return (
+        read_args.retriveArgs().no_cache
+        or read_args.retriveArgs().no_api_cache
+        or config_data.get_cache_mode() == "api_disabled"
     )
 
 
 def get_dynamic_rules():
     return read_args.retriveArgs().dynamic_rules or config_data.get_dynamic()
```

### Comparing `ofscraper-3.9.4/ofscraper/utils/system/network.py` & `ofscraper-3.9.5/ofscraper/utils/system/network.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/system/system.py` & `ofscraper-3.9.5/ofscraper/utils/system/system.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/ofscraper/utils/text.py` & `ofscraper-3.9.5/ofscraper/utils/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.4/pyproject.toml` & `ofscraper-3.9.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "3.9.4"
+version = "3.9.5"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.14"
```

### Comparing `ofscraper-3.9.4/PKG-INFO` & `ofscraper-3.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 3.9.4
+Version: 3.9.5
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ofscraper Version: 3.9.4 Summary: automatically
+Metadata-Version: 2.1 Name: ofscraper Version: 3.9.5 Summary: automatically
 scrape onlyfans Author: datawhores Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Provides-Extra: pyinstaller Requires-Dist: aiofiles
 (>=23.2.1,<24.0.0) Requires-Dist: aiohttp (==3.9.4) Requires-Dist:
 aioprocessing (>=2.0.1,<3.0.0) Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: arrow (>=1.3.0,<2.0.0) Requires-Dist: browser-cookie3 (==0.19.1)
```

