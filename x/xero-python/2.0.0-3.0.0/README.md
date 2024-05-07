# Comparing `tmp/xero_python-2.0.0.tar.gz` & `tmp/xero_python-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xero_python-2.0.0.tar", last modified: Thu Feb  8 06:24:09 2024, max compression
+gzip compressed data, was "xero_python-3.0.0.tar", last modified: Mon May  6 18:55:20 2024, max compression
```

## Comparing `xero_python-2.0.0.tar` & `xero_python-3.0.0.tar`

### file list

```diff
@@ -1,656 +1,656 @@
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.700743 xero_python-2.0.0/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      118 2024-01-31 17:49:22.000000 xero_python-2.0.0/AUTHORS.md
--rw-r--r--   0 manish.tanwar   (501) staff       (20)       60 2024-01-31 17:49:22.000000 xero_python-2.0.0/HISTORY.md
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1077 2024-01-31 17:49:22.000000 xero_python-2.0.0/LICENSE
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      258 2024-01-31 17:49:22.000000 xero_python-2.0.0/MANIFEST.in
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    26054 2024-02-08 06:24:09.700625 xero_python-2.0.0/PKG-INFO
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    25128 2024-01-31 17:49:22.000000 xero_python-2.0.0/README.md
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      111 2024-01-31 17:49:22.000000 xero_python-2.0.0/requirements.txt
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      293 2024-02-08 06:24:09.701010 xero_python-2.0.0/setup.cfg
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1586 2024-02-08 06:18:51.000000 xero_python-2.0.0/setup.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.525465 xero_python-2.0.0/tests/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      297 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.525673 xero_python-2.0.0/tests/accounting/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)       24 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/accounting/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.526184 xero_python-2.0.0/tests/accounting/api/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)       24 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/accounting/api/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.526820 xero_python-2.0.0/tests/accounting/api/cassettes/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3082 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/accounting/api/cassettes/test_get_organisations.yaml
--rw-r--r--   0 manish.tanwar   (501) staff       (20)   372290 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/accounting/api/cassettes/test_invoice_attachment_upload_and_download.yaml
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.527786 xero_python-2.0.0/tests/accounting/api/fixtures/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    54574 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/accounting/api/fixtures/inv-0032.pdf
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    24730 2024-02-08 06:18:51.000000 xero_python-2.0.0/tests/accounting/api/test_accounting_api.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.528551 xero_python-2.0.0/tests/cassettes/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    71720 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/cassettes/test_vcr.yaml
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4210 2024-02-08 06:18:51.000000 xero_python-2.0.0/tests/conftest.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.529658 xero_python-2.0.0/tests/identity/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)       24 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/identity/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.530347 xero_python-2.0.0/tests/identity/api/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)       24 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/identity/api/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.530836 xero_python-2.0.0/tests/identity/api/cassettes/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1077 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/identity/api/cassettes/test_get_connections.yaml
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1082 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/identity/api/test_identity_api.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.532038 xero_python-2.0.0/tests/test_api_client/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1325 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/test_api_client/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.532487 xero_python-2.0.0/tests/test_api_client/cassettes/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3082 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/test_api_client/cassettes/test_call_api_get_organisations.yaml
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2891 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/test_api_client/cassettes/test_token_api_refresh_token.yaml
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    11773 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/test_api_client/test_deserializer.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9814 2024-02-08 06:18:51.000000 xero_python-2.0.0/tests/test_api_client/test_oauth2.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    11877 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/test_api_client/test_serializer.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      538 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/test_executor.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2601 2024-01-31 17:49:22.000000 xero_python-2.0.0/tests/test_single_dispatch_str.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.534011 xero_python-2.0.0/xero_python/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      129 2024-02-08 06:18:51.000000 xero_python-2.0.0/xero_python/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.535454 xero_python-2.0.0/xero_python/accounting/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9527 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.536565 xero_python-2.0.0/xero_python/accounting/api/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      115 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/api/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)   766435 2024-02-08 06:18:51.000000 xero_python-2.0.0/xero_python/accounting/api/accounting_api.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      615 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/api/exception_handler.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.578332 xero_python-2.0.0/xero_python/accounting/models/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9427 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    21659 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/account.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      962 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/account_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1607 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/accounts.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2324 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/accounts_payable.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2354 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/accounts_receivable.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2677 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/action.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1578 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/actions.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    11191 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/address.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    11833 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/address_for_organisation.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9524 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/allocation.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1694 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/allocations.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5767 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/attachment.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1694 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/attachments.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3851 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/balance_details.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2707 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/balances.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    22262 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/bank_transaction.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1858 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/bank_transactions.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    14381 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/bank_transfer.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1771 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/bank_transfers.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    19213 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/batch_payment.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2967 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/batch_payment_delete.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1887 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/batch_payment_delete_by_url_param.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7359 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/batch_payment_details.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1771 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/batch_payments.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2102 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/bill.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6367 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/branding_theme.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1800 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/branding_themes.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6165 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/budget.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4225 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/budget_balance.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3376 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/budget_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4177 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/budget_lines.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1578 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/budgets.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4074 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/cis_org_setting.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1740 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/cis_org_settings.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2670 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/cis_setting.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1713 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/cis_settings.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    46381 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/contact.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5186 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/contact_group.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1771 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/contact_groups.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4479 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/contact_person.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1607 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/contacts.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3620 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/conversion_balances.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2542 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/conversion_date.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3862 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/country_code.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    28233 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/credit_note.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1713 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/credit_notes.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1662 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/currencies.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2287 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/currency.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3196 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/currency_code.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7371 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/element.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8912 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/employee.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1636 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/employees.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3853 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/error.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    11540 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/expense_claim.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1771 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/expense_claims.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3611 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/external_link.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3909 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/history_record.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1800 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/history_records.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2475 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/import_summary.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8021 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/import_summary_accounts.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1792 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/import_summary_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1662 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/import_summary_organisation.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    37542 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/invoice.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1690 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/invoice_reminder.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1858 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/invoice_reminders.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1607 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/invoices.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    17257 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/item.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1520 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/items.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8857 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/journal.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    11322 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/journal_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1607 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/journals.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      582 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/line_amount_types.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    15045 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/line_item.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3448 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/line_item_item.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4693 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/line_item_tracking.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    14905 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/linked_transaction.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1916 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/linked_transactions.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    14384 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/manual_journal.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7857 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/manual_journal_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1800 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/manual_journals.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1907 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/online_invoice.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1800 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/online_invoices.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    36578 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/organisation.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1752 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/organisations.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    17593 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/overpayment.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1723 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/overpayments.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    25558 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/payment.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1785 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/payment_delete.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7124 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/payment_service.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1829 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/payment_services.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2118 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/payment_term.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      676 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/payment_term_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1607 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/payments.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5412 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/phone.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    18343 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/prepayment.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1694 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/prepayments.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4803 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/purchase.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    27432 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/purchase_order.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1800 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/purchase_orders.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    21933 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/quote.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      587 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/quote_line_amount_types.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      647 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/quote_status_codes.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1549 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/quotes.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    15859 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/receipt.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1607 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/receipts.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    18820 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/repeating_invoice.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1887 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/repeating_invoices.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6110 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/report.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2092 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/report_attribute.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2256 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/report_cell.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2913 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/report_fields.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2771 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/report_row.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3452 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/report_rows.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8330 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/report_with_row.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1641 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/report_with_rows.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1578 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/reports.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1717 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/request_empty.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      590 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/row_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3195 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/sales_tracking_category.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7997 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/schedule.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3545 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/setup.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4321 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/tax_component.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    15457 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/tax_rate.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1626 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/tax_rates.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4040 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/tax_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    20827 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/ten_ninety_nine_contact.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    17370 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/ten_nintey_nine_contact.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7481 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/time_zone.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1913 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/tracking_categories.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7202 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/tracking_category.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5241 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/tracking_option.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1650 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/tracking_options.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7432 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/user.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1520 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/users.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1693 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/accounting/models/validation_error.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.580090 xero_python-2.0.0/xero_python/api_client/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    27017 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/api_client/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7399 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/api_client/configuration.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9836 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/api_client/deserializer.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    12122 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/api_client/oauth2.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7337 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/api_client/serializer.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.580349 xero_python-2.0.0/xero_python/appstore/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1042 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/appstore/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.580940 xero_python-2.0.0/xero_python/appstore/api/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      110 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/appstore/api/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    13877 2024-02-08 06:18:51.000000 xero_python-2.0.0/xero_python/appstore/api/app_store_api.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.585205 xero_python-2.0.0/xero_python/appstore/models/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      947 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/appstore/models/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2945 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/appstore/models/create_usage_record.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5105 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/appstore/models/plan.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3237 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/appstore/models/price.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4837 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/appstore/models/problem_details.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5399 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/appstore/models/product.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9016 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/appstore/models/subscription.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8619 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/appstore/models/subscription_item.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1963 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/appstore/models/update_usage_record.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8962 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/appstore/models/usage_record.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1969 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/appstore/models/usage_records_list.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.585698 xero_python-2.0.0/xero_python/assets/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1335 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.586470 xero_python-2.0.0/xero_python/assets/api/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      101 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/api/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    18739 2024-02-08 06:18:51.000000 xero_python-2.0.0/xero_python/assets/api/asset_api.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.590665 xero_python-2.0.0/xero_python/assets/models/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1249 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/models/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    15830 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/models/asset.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      655 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/models/asset_status.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      665 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/models/asset_status_query_param.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8812 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/models/asset_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2284 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/models/assets.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9196 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/models/book_depreciation_detail.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    11640 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/models/book_depreciation_setting.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5500 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/models/error.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6341 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/models/field_validation_errors_element.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3674 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/models/pagination.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5539 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/models/resource_validation_errors_element.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    10228 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/assets/models/setting.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.591182 xero_python-2.0.0/xero_python/exceptions/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4576 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/exceptions/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2817 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/exceptions/http_status_exceptions.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.591536 xero_python-2.0.0/xero_python/file/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      820 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.592105 xero_python-2.0.0/xero_python/file/api/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)       99 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/api/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    55263 2024-02-08 06:18:51.000000 xero_python-2.0.0/xero_python/file/api/files_api.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.595903 xero_python-2.0.0/xero_python/file/models/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      736 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/models/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4100 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/models/association.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6863 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/models/file_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3382 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/models/files.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4619 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/models/folder.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1513 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/models/folders.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3536 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/models/inline_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3554 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/models/inline_object1.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      763 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/models/object_group.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2218 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/models/object_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3879 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/models/upload_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4488 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/file/models/user.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.596252 xero_python-2.0.0/xero_python/finance/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4760 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.596813 xero_python-2.0.0/xero_python/finance/api/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      106 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/api/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    43803 2024-02-08 06:18:51.000000 xero_python-2.0.0/xero_python/finance/api/finance_api.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.615294 xero_python-2.0.0/xero_python/finance/models/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4669 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    12667 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/account_usage.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4551 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/account_usage_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4983 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/balance_sheet_account_detail.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2693 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/balance_sheet_account_group.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3956 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/balance_sheet_account_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4123 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/balance_sheet_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5340 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/bank_statement_accounting_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2890 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/bank_statement_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6492 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/bank_transaction_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6805 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/cash_account_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4142 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/cash_balance.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5850 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/cash_validation_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6990 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/cashflow_account.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3501 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/cashflow_activity.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4556 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/cashflow_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3214 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/cashflow_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6724 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/contact_detail.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2674 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/contact_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4226 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/contact_total_detail.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5112 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/contact_total_other.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4402 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/credit_note_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8485 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/current_statement_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    20091 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/data_source_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5229 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/history_record_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6705 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/income_by_contact_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4261 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/invoice_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4386 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/line_item_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3870 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/lock_history_model.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3618 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/lock_history_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1765 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/manual_journal_total.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4421 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/overpayment_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9358 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/payment_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5740 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/pnl_account.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2988 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/pnl_account_class.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3644 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/pnl_account_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5405 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/practice_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4381 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/prepayment_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3390 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/problem.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1046 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/problem_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5078 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/profit_and_loss_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3911 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/report_history_model.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3579 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/report_history_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3090 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/statement_balance_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    13393 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/statement_line_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    22842 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/statement_lines_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    13592 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/statement_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4032 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/total_detail.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3905 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/total_other.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    10544 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/trial_balance_account.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2649 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/trial_balance_entry.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4429 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/trial_balance_movement.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3541 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/trial_balance_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3566 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/user_activities_response.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    12981 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/finance/models/user_response.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.615514 xero_python-2.0.0/xero_python/identity/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      586 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/identity/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.616450 xero_python-2.0.0/xero_python/identity/api/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      109 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/identity/api/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      750 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/identity/api/exception_handler.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5625 2024-02-08 06:18:51.000000 xero_python-2.0.0/xero_python/identity/api/identity_api.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.618238 xero_python-2.0.0/xero_python/identity/models/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      492 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/identity/models/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5143 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/identity/models/access_token.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7188 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/identity/models/connection.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4283 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/identity/models/refresh_token.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1832 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/models.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.618631 xero_python-2.0.0/xero_python/payrollau/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6978 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.619619 xero_python-2.0.0/xero_python/payrollau/api/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      113 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/api/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    96156 2024-02-08 06:18:51.000000 xero_python-2.0.0/xero_python/payrollau/api/payroll_au_api.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.645772 xero_python-2.0.0/xero_python/payrollau/models/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6880 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3569 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/account.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1144 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/account_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      660 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/allowance_category.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      692 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/allowance_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3119 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/api_exception.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6071 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/bank_account.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      625 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/calendar_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3961 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/country_of_residence.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5380 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/deduction_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9852 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/deduction_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      549 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/deduction_type_calculation_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9487 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/earnings_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    21870 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/earnings_rate.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      588 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/earnings_rate_calculation_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      971 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/earnings_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    35590 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/employee.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      509 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/employee_status.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1588 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/employees.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      638 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/employment_basis.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      499 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/employment_termination_payment_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      513 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/employment_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      526 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/entitlement_final_pay_payout_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5716 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/home_address.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      645 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/income_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3669 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/leave_accrual_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    10598 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/leave_application.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1839 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/leave_applications.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4494 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/leave_balance.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1016 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/leave_category_code.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4492 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/leave_earnings_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    10136 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/leave_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      681 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/leave_line_calculation_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1577 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/leave_lines.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4841 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/leave_period.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      570 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/leave_period_status.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    11646 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/leave_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      596 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/leave_type_contribution_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      674 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/manual_tax_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7942 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/opening_balances.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7310 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/paid_leave_earnings_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4236 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/pay_item.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1560 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/pay_items.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      507 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/pay_out_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    14719 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/pay_run.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      497 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/pay_run_status.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1549 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/pay_runs.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5064 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/pay_template.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      655 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/payment_frequency_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8385 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/payroll_calendar.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1810 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/payroll_calendars.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    16494 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/payslip.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8178 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/payslip_lines.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1551 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/payslip_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    10615 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/payslip_summary.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1559 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/payslips.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      541 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/rate_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4936 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/reimbursement_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1868 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/reimbursement_lines.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5612 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/reimbursement_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      592 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/residency_status.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      592 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/senior_marital_status.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4859 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/settings.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1580 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/settings_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2995 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/settings_tracking_categories.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3257 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/settings_tracking_categories_employee_groups.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3307 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/settings_tracking_categories_timesheet_categories.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      570 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/state.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    12093 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/super_fund.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4088 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/super_fund_product.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1858 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/super_fund_products.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      502 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/super_fund_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1636 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/super_funds.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8280 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/super_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4068 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/super_membership.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      582 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/superannuation_calculation_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      601 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/superannuation_contribution_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    10003 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/superannuation_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    24172 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/tax_declaration.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6143 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/tax_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      711 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/tax_scale_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      563 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/tfn_exemption_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8712 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/timesheet.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4983 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/timesheet_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1609 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/timesheet_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      586 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/timesheet_status.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1617 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/timesheets.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1645 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/validation_error.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      572 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollau/models/work_condition.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.645988 xero_python-2.0.0/xero_python/payrollnz/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8007 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.646821 xero_python-2.0.0/xero_python/payrollnz/api/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      113 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/api/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)   205671 2024-02-08 06:18:51.000000 xero_python-2.0.0/xero_python/payrollnz/api/payroll_nz_api.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.672246 xero_python-2.0.0/xero_python/payrollnz/models/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7909 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4086 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/account.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1552 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/accounts.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5999 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/address.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8594 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/bank_account.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    10860 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/benefit.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      640 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/calendar_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7308 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/deduction.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5257 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/deduction_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3023 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/deduction_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2991 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/deductions.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    10566 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/earnings_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5493 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/earnings_order.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3304 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/earnings_order_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3272 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/earnings_orders.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    12582 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/earnings_rate.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3153 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/earnings_rate_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3135 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/earnings_rates.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6394 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/earnings_template.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3295 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/earnings_template_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    13464 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3375 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_earnings_templates.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7801 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_leave.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4301 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_balance.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3271 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_balances.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2980 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    10706 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_setup.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3215 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_setup_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    13344 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3178 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_type_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3146 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_types.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2928 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_leaves.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2986 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4570 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_opening_balance.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3429 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_opening_balances_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2712 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_pay_template.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3252 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_pay_template_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3182 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_pay_templates.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4503 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_leave_balance.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3442 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_leave_balance_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8014 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_leave_summary.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3492 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_leaves_summaries.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    19815 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_sick_leave.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3544 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_sick_leave_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3492 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_sick_leaves.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    21571 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_tax.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3116 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employee_tax_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2954 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employees.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3885 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employment.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3060 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/employment_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2725 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/gross_earnings_history.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2303 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/invalid_field.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2687 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/leave_accrual_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    10848 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/leave_earnings_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4949 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/leave_period.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2965 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/leave_periods.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6560 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/leave_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3042 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/leave_type_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3010 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/leave_types.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3542 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/pagination.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    11777 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/pay_run.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7678 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/pay_run_calendar.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3260 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/pay_run_calendar_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3228 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/pay_run_calendars.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2931 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/pay_run_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2899 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/pay_runs.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    28891 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/pay_slip.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2968 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/pay_slip_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2936 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/pay_slips.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5038 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/payment_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2950 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/payment_method.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3204 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/payment_method_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5106 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/problem.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    11135 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/reimbursement.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5447 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/reimbursement_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3171 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/reimbursement_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3153 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/reimbursements.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    12190 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/salary_and_wage.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3243 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/salary_and_wage_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3191 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/salary_and_wages.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2902 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/settings.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5484 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/statutory_deduction.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      882 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/statutory_deduction_category.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4878 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/statutory_deduction_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3389 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/statutory_deduction_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3357 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/statutory_deductions.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6358 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/superannuation_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3047 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/superannuation_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3015 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/superannuations.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      739 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/tax_code.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5126 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/tax_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6462 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/tax_settings.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9649 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/timesheet.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    11016 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/timesheet_earnings_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5970 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/timesheet_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3204 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/timesheet_line_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3023 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/timesheet_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2991 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/timesheets.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3299 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/tracking_categories.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3679 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrollnz/models/tracking_category.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.672423 xero_python-2.0.0/xero_python/payrolluk/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7208 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.672965 xero_python-2.0.0/xero_python/payrolluk/api/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      113 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/api/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      614 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/api/exception_handler.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)   211207 2024-02-08 06:18:51.000000 xero_python-2.0.0/xero_python/payrolluk/api/payroll_uk_api.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.694537 xero_python-2.0.0/xero_python/payrolluk/models/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7110 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4175 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/account.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1552 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/accounts.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5284 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/address.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3810 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/bank_account.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    15279 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/benefit.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5049 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/benefit_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2949 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/benefit_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2917 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/benefits.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2582 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/court_order_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    18040 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/deduction.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4352 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/deduction_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3023 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/deduction_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2991 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/deductions.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9494 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/earnings_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5493 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/earnings_order.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3304 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/earnings_order_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3272 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/earnings_orders.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    12972 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/earnings_rate.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3153 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/earnings_rate_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3135 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/earnings_rates.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6394 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/earnings_template.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3295 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/earnings_template_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    14870 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     7801 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_leave.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4301 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_leave_balance.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3271 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_leave_balances.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2980 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_leave_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8210 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_leave_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3178 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_leave_type_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3146 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_leave_types.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2928 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_leaves.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2986 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8493 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_opening_balances.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3414 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_opening_balances_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2712 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_pay_template.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3252 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_pay_template_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3305 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_pay_templates.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4503 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_leave_balance.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3442 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_leave_balance_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8014 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_leave_summary.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3492 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_leaves_summaries.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    19815 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_sick_leave.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3544 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_sick_leave_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3492 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_sick_leaves.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    11263 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_tax.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3116 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employee_tax_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2954 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employees.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5139 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employment.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3060 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/employment_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2303 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/invalid_field.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2687 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/leave_accrual_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6705 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/leave_earnings_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4949 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/leave_period.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2965 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/leave_periods.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8352 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/leave_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3042 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/leave_type_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3010 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/leave_types.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3542 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/pagination.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    12379 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/pay_run.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     8264 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/pay_run_calendar.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3260 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/pay_run_calendar_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3228 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/pay_run_calendars.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2931 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/pay_run_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2899 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/pay_runs.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5038 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/payment_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3073 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/payment_method.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3204 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/payment_method_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    26544 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/payslip.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2968 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/payslip_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2936 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/payslips.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5106 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/problem.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4599 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/reimbursement.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3578 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/reimbursement_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3171 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/reimbursement_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3153 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/reimbursements.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    11173 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/salary_and_wage.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3243 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/salary_and_wage_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3191 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/salary_and_wages.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2902 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/settings.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5484 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/statutory_deduction.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      978 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/statutory_deduction_category.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6148 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/tax_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9565 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/timesheet.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     6869 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/timesheet_earnings_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5970 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/timesheet_line.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3204 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/timesheet_line_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3023 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/timesheet_object.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2991 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/timesheets.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3299 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/tracking_categories.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3679 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/payrolluk/models/tracking_category.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.694716 xero_python-2.0.0/xero_python/project/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1474 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/__init__.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.695380 xero_python-2.0.0/xero_python/project/api/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      106 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/api/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    58069 2024-02-08 06:18:51.000000 xero_python-2.0.0/xero_python/project/api/project_api.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.699811 xero_python-2.0.0/xero_python/project/models/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1383 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/__init__.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2076 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/amount.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      498 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/charge_type.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3032 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/currency_code.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2343 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/error.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4280 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/pagination.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    19641 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/project.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4416 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/project_create_or_update.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1627 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/project_patch.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)      477 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/project_status.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2939 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/project_user.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2206 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/project_users.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2154 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/projects.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    14302 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/task.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     4333 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/task_create_or_update.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2115 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/tasks.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     2190 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/time_entries.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     9410 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/time_entry.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     5854 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/project/models/time_entry_create_or_update.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    12596 2024-01-31 17:56:09.000000 xero_python-2.0.0/xero_python/rest.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     3125 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/single_dispatch_str.py
--rw-r--r--   0 manish.tanwar   (501) staff       (20)     1162 2024-01-31 17:49:22.000000 xero_python-2.0.0/xero_python/utils.py
-drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-02-08 06:24:09.700121 xero_python-2.0.0/xero_python.egg-info/
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    26054 2024-02-08 06:24:09.000000 xero_python-2.0.0/xero_python.egg-info/PKG-INFO
--rw-r--r--   0 manish.tanwar   (501) staff       (20)    28279 2024-02-08 06:24:09.000000 xero_python-2.0.0/xero_python.egg-info/SOURCES.txt
--rw-r--r--   0 manish.tanwar   (501) staff       (20)        1 2024-02-08 06:24:09.000000 xero_python-2.0.0/xero_python.egg-info/dependency_links.txt
--rw-r--r--   0 manish.tanwar   (501) staff       (20)       37 2024-02-08 06:24:09.000000 xero_python-2.0.0/xero_python.egg-info/requires.txt
--rw-r--r--   0 manish.tanwar   (501) staff       (20)       12 2024-02-08 06:24:09.000000 xero_python-2.0.0/xero_python.egg-info/top_level.txt
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.576281 xero_python-3.0.0/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      118 2024-01-31 17:49:22.000000 xero_python-3.0.0/AUTHORS.md
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)       60 2024-01-31 17:49:22.000000 xero_python-3.0.0/HISTORY.md
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1077 2024-01-31 17:49:22.000000 xero_python-3.0.0/LICENSE
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      258 2024-01-31 17:49:22.000000 xero_python-3.0.0/MANIFEST.in
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    26054 2024-05-06 18:55:20.576165 xero_python-3.0.0/PKG-INFO
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    25128 2024-01-31 17:49:22.000000 xero_python-3.0.0/README.md
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      111 2024-01-31 17:49:22.000000 xero_python-3.0.0/requirements.txt
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      293 2024-05-06 18:55:20.576626 xero_python-3.0.0/setup.cfg
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1586 2024-05-03 16:19:11.000000 xero_python-3.0.0/setup.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.327228 xero_python-3.0.0/tests/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      297 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.327488 xero_python-3.0.0/tests/accounting/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)       24 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/accounting/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.328067 xero_python-3.0.0/tests/accounting/api/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)       24 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/accounting/api/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.328976 xero_python-3.0.0/tests/accounting/api/cassettes/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3082 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/accounting/api/cassettes/test_get_organisations.yaml
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)   372290 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/accounting/api/cassettes/test_invoice_attachment_upload_and_download.yaml
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.330604 xero_python-3.0.0/tests/accounting/api/fixtures/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    54574 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/accounting/api/fixtures/inv-0032.pdf
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    24730 2024-02-08 06:18:51.000000 xero_python-3.0.0/tests/accounting/api/test_accounting_api.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.331473 xero_python-3.0.0/tests/cassettes/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    71720 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/cassettes/test_vcr.yaml
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4210 2024-02-08 06:18:51.000000 xero_python-3.0.0/tests/conftest.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.332272 xero_python-3.0.0/tests/identity/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)       24 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/identity/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.332699 xero_python-3.0.0/tests/identity/api/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)       24 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/identity/api/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.333397 xero_python-3.0.0/tests/identity/api/cassettes/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1077 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/identity/api/cassettes/test_get_connections.yaml
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1082 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/identity/api/test_identity_api.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.335349 xero_python-3.0.0/tests/test_api_client/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1325 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/test_api_client/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.336979 xero_python-3.0.0/tests/test_api_client/cassettes/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3082 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/test_api_client/cassettes/test_call_api_get_organisations.yaml
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2891 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/test_api_client/cassettes/test_token_api_refresh_token.yaml
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    11773 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/test_api_client/test_deserializer.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9814 2024-02-08 06:18:51.000000 xero_python-3.0.0/tests/test_api_client/test_oauth2.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    11877 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/test_api_client/test_serializer.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      538 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/test_executor.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2601 2024-01-31 17:49:22.000000 xero_python-3.0.0/tests/test_single_dispatch_str.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.339753 xero_python-3.0.0/xero_python/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      129 2024-05-03 16:19:11.000000 xero_python-3.0.0/xero_python/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.342481 xero_python-3.0.0/xero_python/accounting/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9527 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.344821 xero_python-3.0.0/xero_python/accounting/api/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      115 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/api/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)   768922 2024-05-03 16:19:07.000000 xero_python-3.0.0/xero_python/accounting/api/accounting_api.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      615 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/accounting/api/exception_handler.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.395960 xero_python-3.0.0/xero_python/accounting/models/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9427 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    21659 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/account.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      962 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/account_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1607 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/accounts.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2324 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/accounts_payable.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2354 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/accounts_receivable.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2677 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/action.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1578 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/actions.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    11191 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/address.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    11833 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/address_for_organisation.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9524 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/allocation.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1694 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/allocations.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5767 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/attachment.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1694 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/attachments.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3851 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/balance_details.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2707 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/balances.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    22262 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/bank_transaction.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1858 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/bank_transactions.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    14381 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/bank_transfer.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1771 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/bank_transfers.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    19213 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/batch_payment.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2967 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/batch_payment_delete.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1887 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/batch_payment_delete_by_url_param.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7359 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/batch_payment_details.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1771 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/batch_payments.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2102 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/bill.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6367 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/branding_theme.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1800 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/branding_themes.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6165 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/budget.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4225 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/budget_balance.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3376 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/budget_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4177 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/accounting/models/budget_lines.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1578 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/budgets.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4074 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/cis_org_setting.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1740 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/cis_org_settings.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2670 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/cis_setting.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1713 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/cis_settings.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    46381 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/contact.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5186 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/contact_group.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1771 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/contact_groups.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4479 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/contact_person.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1607 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/contacts.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3620 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/conversion_balances.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2542 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/conversion_date.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3862 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/country_code.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    28233 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/credit_note.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1713 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/credit_notes.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1662 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/currencies.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2287 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/currency.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3196 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/currency_code.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7371 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/element.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8912 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/employee.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1636 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/employees.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3853 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/error.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    11540 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/expense_claim.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1771 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/expense_claims.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3611 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/external_link.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3909 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/history_record.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1800 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/history_records.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2475 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/import_summary.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8021 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/import_summary_accounts.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1792 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/import_summary_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1662 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/import_summary_organisation.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    37542 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/invoice.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1690 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/invoice_reminder.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1858 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/invoice_reminders.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1607 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/invoices.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    17257 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/item.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1520 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/items.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8857 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/journal.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    11322 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/journal_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1607 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/journals.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      582 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/line_amount_types.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    15045 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/line_item.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3448 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/line_item_item.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4693 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/line_item_tracking.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    14905 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/linked_transaction.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1916 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/linked_transactions.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    14384 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/manual_journal.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7857 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/manual_journal_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1800 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/manual_journals.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1907 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/online_invoice.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1800 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/online_invoices.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    36578 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/organisation.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1752 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/organisations.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    17593 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/overpayment.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1723 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/overpayments.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    26397 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/payment.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1785 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/payment_delete.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7124 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/payment_service.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1829 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/payment_services.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2118 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/payment_term.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      676 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/payment_term_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1607 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/payments.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5412 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/phone.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    18343 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/prepayment.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1694 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/prepayments.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4803 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/purchase.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    27432 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/purchase_order.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1800 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/purchase_orders.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    21933 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/quote.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      587 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/quote_line_amount_types.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      647 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/quote_status_codes.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1549 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/quotes.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    15859 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/receipt.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1607 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/receipts.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    18820 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/repeating_invoice.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1887 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/repeating_invoices.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6110 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/report.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2092 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/report_attribute.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2256 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/report_cell.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2913 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/report_fields.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2771 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/report_row.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3452 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/report_rows.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8330 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/report_with_row.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1641 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/report_with_rows.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1578 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/reports.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1717 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/request_empty.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      590 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/row_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3195 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/sales_tracking_category.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7997 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/schedule.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3545 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/setup.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4321 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/tax_component.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    15481 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/tax_rate.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1626 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/tax_rates.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4130 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/tax_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    20827 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/ten_ninety_nine_contact.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    17370 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/accounting/models/ten_nintey_nine_contact.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7481 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/time_zone.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1913 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/tracking_categories.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7202 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/tracking_category.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5241 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/tracking_option.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1650 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/tracking_options.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7432 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/user.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1520 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/users.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1693 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/accounting/models/validation_error.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.400882 xero_python-3.0.0/xero_python/api_client/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    27017 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/api_client/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7399 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/api_client/configuration.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9836 2024-02-18 12:45:04.000000 xero_python-3.0.0/xero_python/api_client/deserializer.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    12122 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/api_client/oauth2.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7337 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/api_client/serializer.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.401755 xero_python-3.0.0/xero_python/appstore/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1042 2024-05-03 16:19:01.000000 xero_python-3.0.0/xero_python/appstore/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.403379 xero_python-3.0.0/xero_python/appstore/api/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      110 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/appstore/api/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    13877 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/appstore/api/app_store_api.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.412015 xero_python-3.0.0/xero_python/appstore/models/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      947 2024-05-03 16:19:01.000000 xero_python-3.0.0/xero_python/appstore/models/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2945 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/appstore/models/create_usage_record.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5105 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/appstore/models/plan.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3237 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/appstore/models/price.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4837 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/appstore/models/problem_details.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5399 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/appstore/models/product.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9016 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/appstore/models/subscription.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8619 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/appstore/models/subscription_item.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1963 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/appstore/models/update_usage_record.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8962 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/appstore/models/usage_record.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1969 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/appstore/models/usage_records_list.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.412378 xero_python-3.0.0/xero_python/assets/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1335 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.413982 xero_python-3.0.0/xero_python/assets/api/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      101 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/api/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    18739 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/api/asset_api.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.420017 xero_python-3.0.0/xero_python/assets/models/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1249 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/models/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    15830 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/models/asset.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      655 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/models/asset_status.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      665 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/models/asset_status_query_param.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8812 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/models/asset_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2284 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/models/assets.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9196 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/models/book_depreciation_detail.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    11640 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/models/book_depreciation_setting.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5500 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/models/error.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6341 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/models/field_validation_errors_element.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3674 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/models/pagination.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5539 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/models/resource_validation_errors_element.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    10228 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/assets/models/setting.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.420595 xero_python-3.0.0/xero_python/exceptions/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4576 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/exceptions/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2817 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/exceptions/http_status_exceptions.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.420967 xero_python-3.0.0/xero_python/file/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      820 2024-05-03 16:19:01.000000 xero_python-3.0.0/xero_python/file/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.421680 xero_python-3.0.0/xero_python/file/api/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)       99 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/file/api/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    55263 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/file/api/files_api.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.426265 xero_python-3.0.0/xero_python/file/models/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      736 2024-05-03 16:19:01.000000 xero_python-3.0.0/xero_python/file/models/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4100 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/file/models/association.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6863 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/file/models/file_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3382 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/file/models/files.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4619 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/file/models/folder.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1513 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/file/models/folders.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3536 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/file/models/inline_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3554 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/file/models/inline_object1.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      763 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/file/models/object_group.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2218 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/file/models/object_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3879 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/file/models/upload_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4488 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/file/models/user.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.426684 xero_python-3.0.0/xero_python/finance/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4760 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.427302 xero_python-3.0.0/xero_python/finance/api/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      106 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/api/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    43803 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/api/finance_api.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.450995 xero_python-3.0.0/xero_python/finance/models/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4669 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    12667 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/account_usage.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4551 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/account_usage_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4983 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/balance_sheet_account_detail.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2693 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/balance_sheet_account_group.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3956 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/balance_sheet_account_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4123 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/balance_sheet_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5340 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/bank_statement_accounting_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2890 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/bank_statement_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6492 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/bank_transaction_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6805 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/cash_account_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4142 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/cash_balance.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5850 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/cash_validation_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6990 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/cashflow_account.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3501 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/cashflow_activity.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4556 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/cashflow_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3214 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/cashflow_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6724 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/contact_detail.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2674 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/contact_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4226 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/contact_total_detail.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5112 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/contact_total_other.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4402 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/credit_note_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8485 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/current_statement_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    20091 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/data_source_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5229 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/history_record_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6705 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/income_by_contact_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4261 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/invoice_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4386 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/line_item_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3870 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/lock_history_model.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3618 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/lock_history_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1765 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/manual_journal_total.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4421 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/overpayment_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9358 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/payment_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5740 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/pnl_account.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2988 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/pnl_account_class.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3644 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/pnl_account_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5405 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/practice_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4381 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/prepayment_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3390 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/problem.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1046 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/problem_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5078 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/profit_and_loss_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3911 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/report_history_model.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3579 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/report_history_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3090 2024-05-03 16:19:03.000000 xero_python-3.0.0/xero_python/finance/models/statement_balance_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    13393 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/statement_line_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    22842 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/statement_lines_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    13592 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/statement_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4032 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/total_detail.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3905 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/total_other.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    10544 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/trial_balance_account.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2649 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/trial_balance_entry.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4429 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/trial_balance_movement.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3541 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/trial_balance_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3566 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/user_activities_response.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    12981 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/finance/models/user_response.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.451397 xero_python-3.0.0/xero_python/identity/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      586 2024-05-03 16:19:01.000000 xero_python-3.0.0/xero_python/identity/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.453308 xero_python-3.0.0/xero_python/identity/api/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      109 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/identity/api/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      750 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/identity/api/exception_handler.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5625 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/identity/api/identity_api.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.455013 xero_python-3.0.0/xero_python/identity/models/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      492 2024-05-03 16:19:01.000000 xero_python-3.0.0/xero_python/identity/models/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5143 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/identity/models/access_token.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7188 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/identity/models/connection.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4283 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/identity/models/refresh_token.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1832 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/models.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.455482 xero_python-3.0.0/xero_python/payrollau/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6978 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.456582 xero_python-3.0.0/xero_python/payrollau/api/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      113 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/api/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    96156 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/api/payroll_au_api.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.494476 xero_python-3.0.0/xero_python/payrollau/models/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6880 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3569 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/account.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1144 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/account_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      660 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/allowance_category.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      664 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/allowance_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3119 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/api_exception.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6071 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/bank_account.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      625 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/calendar_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3961 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/country_of_residence.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5380 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/deduction_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9852 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/deduction_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      549 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/deduction_type_calculation_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9487 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/earnings_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    21870 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/earnings_rate.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      588 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/earnings_rate_calculation_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      971 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/earnings_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    35590 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/employee.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      509 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/employee_status.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1588 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/employees.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      638 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/employment_basis.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      499 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/employment_termination_payment_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      513 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/employment_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      526 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/entitlement_final_pay_payout_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5716 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/home_address.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      645 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/income_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3669 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/leave_accrual_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    10598 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/leave_application.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1839 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/leave_applications.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4494 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/leave_balance.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1016 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/leave_category_code.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4492 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/leave_earnings_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    10136 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/leave_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      681 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/leave_line_calculation_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1577 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/leave_lines.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4841 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/leave_period.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      570 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/leave_period_status.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    11646 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/leave_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      596 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/leave_type_contribution_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      674 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/manual_tax_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7942 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/opening_balances.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7310 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/paid_leave_earnings_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4236 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/pay_item.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1560 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/pay_items.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      507 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/pay_out_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    14719 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/pay_run.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      497 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/pay_run_status.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1549 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/pay_runs.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5064 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/pay_template.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      655 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/payment_frequency_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8385 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/payroll_calendar.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1810 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/payroll_calendars.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    16494 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/payslip.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8178 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/payslip_lines.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1551 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/payslip_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    10615 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/payslip_summary.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1559 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/payslips.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      541 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/rate_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4936 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/reimbursement_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1868 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/reimbursement_lines.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5612 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/reimbursement_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      592 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/residency_status.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      592 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/senior_marital_status.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4859 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/settings.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1580 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/settings_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2995 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/settings_tracking_categories.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3257 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/settings_tracking_categories_employee_groups.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3307 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/settings_tracking_categories_timesheet_categories.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      570 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/state.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    12093 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/super_fund.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4088 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/super_fund_product.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1858 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/super_fund_products.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      502 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/super_fund_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1636 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/super_funds.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8280 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/super_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4068 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/super_membership.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      582 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/superannuation_calculation_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      601 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/superannuation_contribution_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    10003 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/superannuation_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    24172 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/tax_declaration.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6143 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/tax_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      711 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/tax_scale_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      563 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/tfn_exemption_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8712 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/timesheet.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4983 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/timesheet_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1609 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/timesheet_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      586 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/timesheet_status.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1617 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/timesheets.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1645 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/validation_error.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      572 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollau/models/work_condition.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.494693 xero_python-3.0.0/xero_python/payrollnz/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8007 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.495315 xero_python-3.0.0/xero_python/payrollnz/api/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      113 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/api/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)   205671 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrollnz/api/payroll_nz_api.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.536854 xero_python-3.0.0/xero_python/payrollnz/models/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7909 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4086 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/account.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1552 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/accounts.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5999 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/address.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8594 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/bank_account.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    10860 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/benefit.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      640 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/calendar_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7308 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/deduction.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5257 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/deduction_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3023 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/deduction_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2991 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/deductions.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    10566 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/earnings_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5493 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/earnings_order.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3304 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/earnings_order_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3272 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/earnings_orders.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    12582 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/earnings_rate.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3153 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/earnings_rate_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3135 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/earnings_rates.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6394 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/earnings_template.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3295 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/earnings_template_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    13464 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3375 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_earnings_templates.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7801 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_leave.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4301 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_balance.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3271 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_balances.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2980 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    10706 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_setup.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3215 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_setup_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    13344 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3178 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_type_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3146 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_types.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2928 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_leaves.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2986 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4570 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_opening_balance.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3429 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_opening_balances_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2712 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_pay_template.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3252 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_pay_template_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3182 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_pay_templates.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4503 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_leave_balance.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3442 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_leave_balance_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8014 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_leave_summary.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3492 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_leaves_summaries.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    19815 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_sick_leave.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3544 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_sick_leave_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3492 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_sick_leaves.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    21571 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_tax.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3116 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employee_tax_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2954 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employees.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3885 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employment.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3060 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/employment_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2725 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/gross_earnings_history.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2303 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/invalid_field.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2687 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/leave_accrual_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    10848 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/leave_earnings_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4949 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/leave_period.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2965 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/leave_periods.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6560 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/leave_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3042 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/leave_type_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3010 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/leave_types.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3542 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/pagination.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    11777 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/pay_run.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7678 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/pay_run_calendar.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3260 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/pay_run_calendar_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3228 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/pay_run_calendars.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2931 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/pay_run_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2899 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/pay_runs.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    28891 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/pay_slip.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2968 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/pay_slip_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2936 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/pay_slips.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5038 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/payment_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2950 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/payment_method.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3204 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/payment_method_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5106 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/problem.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    11135 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/reimbursement.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5447 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/reimbursement_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3171 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/reimbursement_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3153 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/reimbursements.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    12190 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/salary_and_wage.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3243 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/salary_and_wage_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3191 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/salary_and_wages.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2902 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/settings.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5484 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/statutory_deduction.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      882 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/statutory_deduction_category.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4878 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/statutory_deduction_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3389 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/statutory_deduction_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3357 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/statutory_deductions.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6358 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/superannuation_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3047 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/superannuation_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3015 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/superannuations.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      739 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/tax_code.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5126 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/tax_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6462 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/tax_settings.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9649 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/timesheet.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    11016 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/timesheet_earnings_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5970 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/timesheet_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3204 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/timesheet_line_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3023 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/timesheet_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2991 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/timesheets.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3299 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/tracking_categories.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3679 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrollnz/models/tracking_category.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.537052 xero_python-3.0.0/xero_python/payrolluk/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7208 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.538158 xero_python-3.0.0/xero_python/payrolluk/api/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      113 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/api/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      614 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/payrolluk/api/exception_handler.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)   211207 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/api/payroll_uk_api.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.567709 xero_python-3.0.0/xero_python/payrolluk/models/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7110 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4175 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/account.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1552 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/accounts.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5284 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/address.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3810 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/bank_account.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    15279 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/benefit.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5049 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/benefit_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2949 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/benefit_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2917 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/benefits.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2582 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/court_order_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    18040 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/deduction.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4352 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/deduction_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3023 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/deduction_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2991 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/deductions.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9494 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/earnings_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5493 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/earnings_order.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3304 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/earnings_order_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3272 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/earnings_orders.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    12972 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/earnings_rate.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3153 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/earnings_rate_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3135 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/earnings_rates.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6394 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/earnings_template.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3295 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/earnings_template_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    14870 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     7801 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_leave.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4301 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_leave_balance.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3271 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_leave_balances.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2980 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_leave_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8210 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_leave_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3178 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_leave_type_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3146 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_leave_types.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2928 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_leaves.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2986 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8493 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_opening_balances.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3414 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_opening_balances_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2712 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_pay_template.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3252 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_pay_template_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3305 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_pay_templates.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4503 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_leave_balance.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3442 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_leave_balance_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8014 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_leave_summary.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3492 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_leaves_summaries.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    19815 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_sick_leave.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3544 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_sick_leave_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3492 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_sick_leaves.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    11263 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_tax.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3116 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employee_tax_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2954 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employees.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5139 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employment.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3060 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/employment_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2303 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/invalid_field.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2687 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/leave_accrual_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6705 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/leave_earnings_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4949 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/leave_period.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2965 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/leave_periods.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8352 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/leave_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3042 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/leave_type_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3010 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/leave_types.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3542 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/pagination.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    12379 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/pay_run.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     8264 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/pay_run_calendar.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3260 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/pay_run_calendar_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3228 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/pay_run_calendars.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2931 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/pay_run_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2899 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/pay_runs.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5038 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/payment_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3073 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/payment_method.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3204 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/payment_method_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    26544 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/payslip.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2968 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/payslip_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2936 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/payslips.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5106 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/problem.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4599 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/reimbursement.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3578 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/reimbursement_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3171 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/reimbursement_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3153 2024-05-03 16:19:04.000000 xero_python-3.0.0/xero_python/payrolluk/models/reimbursements.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    11173 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/salary_and_wage.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3243 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/salary_and_wage_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3191 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/salary_and_wages.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2902 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/settings.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5484 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/statutory_deduction.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      978 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/statutory_deduction_category.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6148 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/tax_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9565 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/timesheet.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     6869 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/timesheet_earnings_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5970 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/timesheet_line.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3204 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/timesheet_line_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3023 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/timesheet_object.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2991 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/timesheets.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3299 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/tracking_categories.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3679 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/payrolluk/models/tracking_category.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.568209 xero_python-3.0.0/xero_python/project/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1474 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/__init__.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.568658 xero_python-3.0.0/xero_python/project/api/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      106 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/api/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    58069 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/api/project_api.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.575213 xero_python-3.0.0/xero_python/project/models/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1383 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/__init__.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2076 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/amount.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      498 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/charge_type.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3032 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/currency_code.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2343 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/error.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4280 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/pagination.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    19641 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/project.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4416 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/project_create_or_update.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1627 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/project_patch.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)      477 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/project_status.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2939 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/project_user.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2206 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/project_users.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2154 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/projects.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    14302 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/task.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     4333 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/task_create_or_update.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2115 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/tasks.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     2190 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/time_entries.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     9410 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/time_entry.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     5854 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/project/models/time_entry_create_or_update.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    12596 2024-05-03 16:19:05.000000 xero_python-3.0.0/xero_python/rest.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     3125 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/single_dispatch_str.py
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)     1162 2024-01-31 17:49:22.000000 xero_python-3.0.0/xero_python/utils.py
+drwxr-xr-x   0 manish.tanwar   (501) staff       (20)        0 2024-05-06 18:55:20.575815 xero_python-3.0.0/xero_python.egg-info/
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    26054 2024-05-06 18:55:20.000000 xero_python-3.0.0/xero_python.egg-info/PKG-INFO
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)    28279 2024-05-06 18:55:20.000000 xero_python-3.0.0/xero_python.egg-info/SOURCES.txt
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)        1 2024-05-06 18:55:20.000000 xero_python-3.0.0/xero_python.egg-info/dependency_links.txt
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)       37 2024-05-06 18:55:20.000000 xero_python-3.0.0/xero_python.egg-info/requires.txt
+-rw-r--r--   0 manish.tanwar   (501) staff       (20)       12 2024-05-06 18:55:20.000000 xero_python-3.0.0/xero_python.egg-info/top_level.txt
```

### Comparing `xero_python-2.0.0/LICENSE` & `xero_python-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/PKG-INFO` & `xero_python-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xero_python
-Version: 2.0.0
+Version: 3.0.0
 Summary: Official Python sdk for Xero API generated by OpenAPI spec for oAuth2
 Author: Xero Developer API
 Author-email: api@xero.com
 License: MIT license
 Keywords: xero python sdk API oAuth
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `xero_python-2.0.0/README.md` & `xero_python-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/setup.py` & `xero_python-3.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,9 +44,9 @@
     license="MIT license",
     long_description="\n\n".join((read_file("README.md"), read_file("HISTORY.md"))),
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="xero python sdk API oAuth",
     name="xero_python",
     packages=find_packages(include=["xero_python", "xero_python.*"]),
-    version="2.0.0",
+    version="3.0.0",
 )
```

### Comparing `xero_python-2.0.0/tests/accounting/api/cassettes/test_get_organisations.yaml` & `xero_python-3.0.0/tests/accounting/api/cassettes/test_get_organisations.yaml`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/accounting/api/cassettes/test_invoice_attachment_upload_and_download.yaml` & `xero_python-3.0.0/tests/accounting/api/cassettes/test_invoice_attachment_upload_and_download.yaml`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/accounting/api/fixtures/inv-0032.pdf` & `xero_python-3.0.0/tests/accounting/api/fixtures/inv-0032.pdf`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/accounting/api/test_accounting_api.py` & `xero_python-3.0.0/tests/accounting/api/test_accounting_api.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/cassettes/test_vcr.yaml` & `xero_python-3.0.0/tests/cassettes/test_vcr.yaml`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/conftest.py` & `xero_python-3.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/identity/api/cassettes/test_get_connections.yaml` & `xero_python-3.0.0/tests/identity/api/cassettes/test_get_connections.yaml`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/identity/api/test_identity_api.py` & `xero_python-3.0.0/tests/identity/api/test_identity_api.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/test_api_client/__init__.py` & `xero_python-3.0.0/tests/test_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/test_api_client/cassettes/test_call_api_get_organisations.yaml` & `xero_python-3.0.0/tests/test_api_client/cassettes/test_call_api_get_organisations.yaml`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/test_api_client/cassettes/test_token_api_refresh_token.yaml` & `xero_python-3.0.0/tests/test_api_client/cassettes/test_token_api_refresh_token.yaml`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/test_api_client/test_deserializer.py` & `xero_python-3.0.0/tests/test_api_client/test_deserializer.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/test_api_client/test_oauth2.py` & `xero_python-3.0.0/tests/test_api_client/test_oauth2.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/test_api_client/test_serializer.py` & `xero_python-3.0.0/tests/test_api_client/test_serializer.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/test_executor.py` & `xero_python-3.0.0/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/tests/test_single_dispatch_str.py` & `xero_python-3.0.0/tests/test_single_dispatch_str.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/__init__.py` & `xero_python-3.0.0/xero_python/accounting/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/api/accounting_api.py` & `xero_python-3.0.0/xero_python/accounting/api/accounting_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
     Contact: api@xero.com
     Generated by: https://openapi-generator.tech
 """
 
 """
-    OpenAPI spec version: 3.0.0
+    OpenAPI spec version: 3.0.3
 """
 
 import importlib
 import re  # noqa: F401
 
 from xero_python import exceptions
 from xero_python.api_client import ApiClient, ModelFinder
@@ -16670,30 +16670,104 @@
                 _preload_content=_preload_content,
                 _request_timeout=_request_timeout,
                 collection_formats=collection_formats,
             )
         except exceptions.HTTPStatusException as error:
             raise translate_status_exception(error, self, "get_reports_list")
 
+    def get_tax_rate_by_tax_type(
+        self,
+        xero_tenant_id,
+        tax_type,
+        _return_http_data_only=True,
+        _preload_content=True,
+        _request_timeout=None,
+    ):
+        """Retrieves a specific tax rate according to given TaxType code  # noqa: E501
+        OAuth2 scope: accounting.settings, accounting.settings.read
+        :param str xero_tenant_id: Xero identifier for Tenant (required)
+        :param str tax_type: A valid TaxType code (required)
+        :param bool _return_http_data_only: return received data only
+        :param bool _preload_content: load received data in models
+        :param bool _request_timeout: maximum wait time for response
+        :return: TaxRates
+        """
+
+        # verify the required parameter 'xero_tenant_id' is set
+        if xero_tenant_id is None:
+            raise ValueError(
+                "Missing the required parameter `xero_tenant_id` "
+                "when calling `get_tax_rate_by_tax_type`"
+            )
+        # verify the required parameter 'tax_type' is set
+        if tax_type is None:
+            raise ValueError(
+                "Missing the required parameter `tax_type` "
+                "when calling `get_tax_rate_by_tax_type`"
+            )
+
+        collection_formats = {}
+        path_params = {
+            "TaxType": tax_type,
+        }
+
+        query_params = []
+
+        header_params = {
+            "xero-tenant-id": xero_tenant_id,
+        }
+
+        local_var_files = {}
+        form_params = []
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params["Accept"] = self.api_client.select_header_accept(
+            ["application/json"]
+        )
+
+        # Authentication setting
+        auth_settings = ["OAuth2"]
+        url = self.get_resource_url("/TaxRates/{TaxType}")
+
+        try:
+            return self.api_client.call_api(
+                url,
+                "GET",
+                path_params,
+                query_params,
+                header_params,
+                body=body_params,
+                post_params=form_params,
+                files=local_var_files,
+                response_type="TaxRates",
+                response_model_finder=self.get_model_finder(),
+                auth_settings=auth_settings,
+                _return_http_data_only=_return_http_data_only,
+                _preload_content=_preload_content,
+                _request_timeout=_request_timeout,
+                collection_formats=collection_formats,
+            )
+        except exceptions.HTTPStatusException as error:
+            raise translate_status_exception(error, self, "get_tax_rate_by_tax_type")
+
     def get_tax_rates(
         self,
         xero_tenant_id,
         where=empty,
         order=empty,
-        tax_type=empty,
         _return_http_data_only=True,
         _preload_content=True,
         _request_timeout=None,
     ):
         """Retrieves tax rates  # noqa: E501
         OAuth2 scope: accounting.settings, accounting.settings.read
         :param str xero_tenant_id: Xero identifier for Tenant (required)
         :param str where: Filter by an any element
         :param str order: Order by an any element
-        :param str tax_type: Filter by tax type
         :param bool _return_http_data_only: return received data only
         :param bool _preload_content: load received data in models
         :param bool _request_timeout: maximum wait time for response
         :return: TaxRates
         """
 
         # verify the required parameter 'xero_tenant_id' is set
@@ -16710,17 +16784,14 @@
 
         if where is not empty:
             query_params.append(("where", where))
 
         if order is not empty:
             query_params.append(("order", order))
 
-        if tax_type is not empty:
-            query_params.append(("TaxType", tax_type))
-
         header_params = {
             "xero-tenant-id": xero_tenant_id,
         }
 
         local_var_files = {}
         form_params = []
```

### Comparing `xero_python-2.0.0/xero_python/accounting/api/exception_handler.py` & `xero_python-3.0.0/xero_python/accounting/api/exception_handler.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/__init__.py` & `xero_python-3.0.0/xero_python/accounting/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/account.py` & `xero_python-3.0.0/xero_python/accounting/models/account.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/account_type.py` & `xero_python-3.0.0/xero_python/accounting/models/account_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/accounts.py` & `xero_python-3.0.0/xero_python/accounting/models/accounts.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/accounts_payable.py` & `xero_python-3.0.0/xero_python/accounting/models/accounts_payable.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/accounts_receivable.py` & `xero_python-3.0.0/xero_python/accounting/models/accounts_receivable.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/action.py` & `xero_python-3.0.0/xero_python/accounting/models/action.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/actions.py` & `xero_python-3.0.0/xero_python/accounting/models/actions.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/address.py` & `xero_python-3.0.0/xero_python/accounting/models/address.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/address_for_organisation.py` & `xero_python-3.0.0/xero_python/accounting/models/address_for_organisation.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/allocation.py` & `xero_python-3.0.0/xero_python/accounting/models/allocation.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/allocations.py` & `xero_python-3.0.0/xero_python/accounting/models/allocations.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/attachment.py` & `xero_python-3.0.0/xero_python/accounting/models/attachment.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/attachments.py` & `xero_python-3.0.0/xero_python/accounting/models/attachments.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/balance_details.py` & `xero_python-3.0.0/xero_python/accounting/models/balance_details.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/balances.py` & `xero_python-3.0.0/xero_python/accounting/models/balances.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/bank_transaction.py` & `xero_python-3.0.0/xero_python/accounting/models/bank_transaction.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/bank_transactions.py` & `xero_python-3.0.0/xero_python/accounting/models/bank_transactions.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/bank_transfer.py` & `xero_python-3.0.0/xero_python/accounting/models/bank_transfer.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/bank_transfers.py` & `xero_python-3.0.0/xero_python/accounting/models/bank_transfers.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/batch_payment.py` & `xero_python-3.0.0/xero_python/accounting/models/batch_payment.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/batch_payment_delete.py` & `xero_python-3.0.0/xero_python/accounting/models/batch_payment_delete.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/batch_payment_delete_by_url_param.py` & `xero_python-3.0.0/xero_python/accounting/models/batch_payment_delete_by_url_param.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/batch_payment_details.py` & `xero_python-3.0.0/xero_python/accounting/models/batch_payment_details.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/batch_payments.py` & `xero_python-3.0.0/xero_python/accounting/models/batch_payments.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/bill.py` & `xero_python-3.0.0/xero_python/accounting/models/bill.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/branding_theme.py` & `xero_python-3.0.0/xero_python/accounting/models/branding_theme.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/branding_themes.py` & `xero_python-3.0.0/xero_python/accounting/models/branding_themes.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/budget.py` & `xero_python-3.0.0/xero_python/accounting/models/budget.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/budget_balance.py` & `xero_python-3.0.0/xero_python/accounting/models/budget_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/budget_line.py` & `xero_python-3.0.0/xero_python/accounting/models/budget_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/budget_lines.py` & `xero_python-3.0.0/xero_python/accounting/models/budget_lines.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/budgets.py` & `xero_python-3.0.0/xero_python/accounting/models/budgets.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/cis_org_setting.py` & `xero_python-3.0.0/xero_python/accounting/models/cis_org_setting.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/cis_org_settings.py` & `xero_python-3.0.0/xero_python/accounting/models/cis_org_settings.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/cis_setting.py` & `xero_python-3.0.0/xero_python/accounting/models/cis_setting.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/cis_settings.py` & `xero_python-3.0.0/xero_python/accounting/models/cis_settings.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/contact.py` & `xero_python-3.0.0/xero_python/accounting/models/contact.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/contact_group.py` & `xero_python-3.0.0/xero_python/accounting/models/contact_group.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/contact_groups.py` & `xero_python-3.0.0/xero_python/accounting/models/contact_groups.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/contact_person.py` & `xero_python-3.0.0/xero_python/accounting/models/contact_person.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/contacts.py` & `xero_python-3.0.0/xero_python/accounting/models/contacts.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/conversion_balances.py` & `xero_python-3.0.0/xero_python/accounting/models/conversion_balances.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/conversion_date.py` & `xero_python-3.0.0/xero_python/accounting/models/conversion_date.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/country_code.py` & `xero_python-3.0.0/xero_python/accounting/models/country_code.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/credit_note.py` & `xero_python-3.0.0/xero_python/accounting/models/credit_note.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/credit_notes.py` & `xero_python-3.0.0/xero_python/accounting/models/credit_notes.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/currencies.py` & `xero_python-3.0.0/xero_python/accounting/models/currencies.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/currency.py` & `xero_python-3.0.0/xero_python/accounting/models/currency.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/currency_code.py` & `xero_python-3.0.0/xero_python/accounting/models/currency_code.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/element.py` & `xero_python-3.0.0/xero_python/accounting/models/element.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/employee.py` & `xero_python-3.0.0/xero_python/accounting/models/employee.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/employees.py` & `xero_python-3.0.0/xero_python/accounting/models/employees.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/error.py` & `xero_python-3.0.0/xero_python/accounting/models/error.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/expense_claim.py` & `xero_python-3.0.0/xero_python/accounting/models/expense_claim.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/expense_claims.py` & `xero_python-3.0.0/xero_python/accounting/models/expense_claims.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/external_link.py` & `xero_python-3.0.0/xero_python/accounting/models/external_link.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/history_record.py` & `xero_python-3.0.0/xero_python/accounting/models/history_record.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/history_records.py` & `xero_python-3.0.0/xero_python/accounting/models/history_records.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/import_summary.py` & `xero_python-3.0.0/xero_python/accounting/models/import_summary.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/import_summary_accounts.py` & `xero_python-3.0.0/xero_python/accounting/models/import_summary_accounts.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/import_summary_object.py` & `xero_python-3.0.0/xero_python/accounting/models/import_summary_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/import_summary_organisation.py` & `xero_python-3.0.0/xero_python/accounting/models/import_summary_organisation.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/invoice.py` & `xero_python-3.0.0/xero_python/accounting/models/invoice.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/invoice_reminder.py` & `xero_python-3.0.0/xero_python/accounting/models/invoice_reminder.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/invoice_reminders.py` & `xero_python-3.0.0/xero_python/accounting/models/invoice_reminders.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/invoices.py` & `xero_python-3.0.0/xero_python/accounting/models/invoices.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/item.py` & `xero_python-3.0.0/xero_python/accounting/models/item.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/items.py` & `xero_python-3.0.0/xero_python/accounting/models/items.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/journal.py` & `xero_python-3.0.0/xero_python/accounting/models/journal.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/journal_line.py` & `xero_python-3.0.0/xero_python/accounting/models/journal_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/journals.py` & `xero_python-3.0.0/xero_python/accounting/models/journals.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/line_amount_types.py` & `xero_python-3.0.0/xero_python/accounting/models/line_amount_types.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/line_item.py` & `xero_python-3.0.0/xero_python/accounting/models/line_item.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/line_item_item.py` & `xero_python-3.0.0/xero_python/accounting/models/line_item_item.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/line_item_tracking.py` & `xero_python-3.0.0/xero_python/accounting/models/line_item_tracking.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/linked_transaction.py` & `xero_python-3.0.0/xero_python/accounting/models/linked_transaction.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/linked_transactions.py` & `xero_python-3.0.0/xero_python/accounting/models/linked_transactions.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/manual_journal.py` & `xero_python-3.0.0/xero_python/accounting/models/manual_journal.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/manual_journal_line.py` & `xero_python-3.0.0/xero_python/accounting/models/manual_journal_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/manual_journals.py` & `xero_python-3.0.0/xero_python/accounting/models/manual_journals.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/online_invoice.py` & `xero_python-3.0.0/xero_python/accounting/models/online_invoice.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/online_invoices.py` & `xero_python-3.0.0/xero_python/accounting/models/online_invoices.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/organisation.py` & `xero_python-3.0.0/xero_python/accounting/models/organisation.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/organisations.py` & `xero_python-3.0.0/xero_python/accounting/models/organisations.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/overpayment.py` & `xero_python-3.0.0/xero_python/accounting/models/overpayment.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/overpayments.py` & `xero_python-3.0.0/xero_python/accounting/models/overpayments.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/payment.py` & `xero_python-3.0.0/xero_python/accounting/models/payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         "bank_account_number": "str",
         "particulars": "str",
         "details": "str",
         "has_account": "bool",
         "has_validation_errors": "bool",
         "status_attribute_string": "str",
         "validation_errors": "list[ValidationError]",
+        "warnings": "list[ValidationError]",
     }
 
     attribute_map = {
         "invoice": "Invoice",
         "credit_note": "CreditNote",
         "prepayment": "Prepayment",
         "overpayment": "Overpayment",
@@ -83,14 +84,15 @@
         "bank_account_number": "BankAccountNumber",
         "particulars": "Particulars",
         "details": "Details",
         "has_account": "HasAccount",
         "has_validation_errors": "HasValidationErrors",
         "status_attribute_string": "StatusAttributeString",
         "validation_errors": "ValidationErrors",
+        "warnings": "Warnings",
     }
 
     def __init__(
         self,
         invoice=None,
         credit_note=None,
         prepayment=None,
@@ -114,14 +116,15 @@
         bank_account_number=None,
         particulars=None,
         details=None,
         has_account=False,
         has_validation_errors=False,
         status_attribute_string=None,
         validation_errors=None,
+        warnings=None,
     ):  # noqa: E501
         """Payment - a model defined in OpenAPI"""  # noqa: E501
 
         self._invoice = None
         self._credit_note = None
         self._prepayment = None
         self._overpayment = None
@@ -144,14 +147,15 @@
         self._bank_account_number = None
         self._particulars = None
         self._details = None
         self._has_account = None
         self._has_validation_errors = None
         self._status_attribute_string = None
         self._validation_errors = None
+        self._warnings = None
         self.discriminator = None
 
         if invoice is not None:
             self.invoice = invoice
         if credit_note is not None:
             self.credit_note = credit_note
         if prepayment is not None:
@@ -200,14 +204,16 @@
             self.has_account = has_account
         if has_validation_errors is not None:
             self.has_validation_errors = has_validation_errors
         if status_attribute_string is not None:
             self.status_attribute_string = status_attribute_string
         if validation_errors is not None:
             self.validation_errors = validation_errors
+        if warnings is not None:
+            self.warnings = warnings
 
     @property
     def invoice(self):
         """Gets the invoice of this Payment.  # noqa: E501
 
 
         :return: The invoice of this Payment.  # noqa: E501
@@ -837,7 +843,30 @@
         Displays array of validation error messages from the API  # noqa: E501
 
         :param validation_errors: The validation_errors of this Payment.  # noqa: E501
         :type: list[ValidationError]
         """
 
         self._validation_errors = validation_errors
+
+    @property
+    def warnings(self):
+        """Gets the warnings of this Payment.  # noqa: E501
+
+        Displays array of warning messages from the API  # noqa: E501
+
+        :return: The warnings of this Payment.  # noqa: E501
+        :rtype: list[ValidationError]
+        """
+        return self._warnings
+
+    @warnings.setter
+    def warnings(self, warnings):
+        """Sets the warnings of this Payment.
+
+        Displays array of warning messages from the API  # noqa: E501
+
+        :param warnings: The warnings of this Payment.  # noqa: E501
+        :type: list[ValidationError]
+        """
+
+        self._warnings = warnings
```

### Comparing `xero_python-2.0.0/xero_python/accounting/models/payment_delete.py` & `xero_python-3.0.0/xero_python/accounting/models/payment_delete.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/payment_service.py` & `xero_python-3.0.0/xero_python/accounting/models/payment_service.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/payment_services.py` & `xero_python-3.0.0/xero_python/accounting/models/payment_services.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/payment_term.py` & `xero_python-3.0.0/xero_python/accounting/models/payment_term.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/payment_term_type.py` & `xero_python-3.0.0/xero_python/accounting/models/payment_term_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/payments.py` & `xero_python-3.0.0/xero_python/accounting/models/payments.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/phone.py` & `xero_python-3.0.0/xero_python/accounting/models/phone.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/prepayment.py` & `xero_python-3.0.0/xero_python/accounting/models/prepayment.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/prepayments.py` & `xero_python-3.0.0/xero_python/accounting/models/prepayments.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/purchase.py` & `xero_python-3.0.0/xero_python/accounting/models/purchase.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/purchase_order.py` & `xero_python-3.0.0/xero_python/accounting/models/purchase_order.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/purchase_orders.py` & `xero_python-3.0.0/xero_python/accounting/models/purchase_orders.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/quote.py` & `xero_python-3.0.0/xero_python/accounting/models/quote.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/quote_line_amount_types.py` & `xero_python-3.0.0/xero_python/accounting/models/quote_line_amount_types.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/quote_status_codes.py` & `xero_python-3.0.0/xero_python/accounting/models/quote_status_codes.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/quotes.py` & `xero_python-3.0.0/xero_python/accounting/models/quotes.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/receipt.py` & `xero_python-3.0.0/xero_python/accounting/models/receipt.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/receipts.py` & `xero_python-3.0.0/xero_python/accounting/models/receipts.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/repeating_invoice.py` & `xero_python-3.0.0/xero_python/accounting/models/repeating_invoice.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/repeating_invoices.py` & `xero_python-3.0.0/xero_python/accounting/models/repeating_invoices.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/report.py` & `xero_python-3.0.0/xero_python/accounting/models/report.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/report_attribute.py` & `xero_python-3.0.0/xero_python/accounting/models/report_attribute.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/report_cell.py` & `xero_python-3.0.0/xero_python/accounting/models/report_cell.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/report_fields.py` & `xero_python-3.0.0/xero_python/accounting/models/report_fields.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/report_row.py` & `xero_python-3.0.0/xero_python/accounting/models/report_row.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/report_rows.py` & `xero_python-3.0.0/xero_python/accounting/models/report_rows.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/report_with_row.py` & `xero_python-3.0.0/xero_python/accounting/models/report_with_row.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/report_with_rows.py` & `xero_python-3.0.0/xero_python/accounting/models/report_with_rows.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/reports.py` & `xero_python-3.0.0/xero_python/accounting/models/reports.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/request_empty.py` & `xero_python-3.0.0/xero_python/accounting/models/request_empty.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/row_type.py` & `xero_python-3.0.0/xero_python/accounting/models/row_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/sales_tracking_category.py` & `xero_python-3.0.0/xero_python/accounting/models/sales_tracking_category.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/schedule.py` & `xero_python-3.0.0/xero_python/accounting/models/schedule.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/setup.py` & `xero_python-3.0.0/xero_python/accounting/models/setup.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/tax_component.py` & `xero_python-3.0.0/xero_python/accounting/models/tax_component.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/tax_rate.py` & `xero_python-3.0.0/xero_python/accounting/models/tax_rate.py`

 * *Files 0% similar despite different names*

```diff
@@ -337,14 +337,15 @@
             "SRLVG",
             "IM",
             "IMESS",
             "IMN33",
             "IMRE",
             "BADDEBTRECOVERY",
             "USSALESTAX",
+            "BLINPUT3",
             "None",
         ]  # noqa: E501
 
         if report_tax_type:
             if report_tax_type not in allowed_values:
                 raise ValueError(
                     "Invalid value for `report_tax_type` ({0}), must be one of {1}".format(  # noqa: E501
```

### Comparing `xero_python-2.0.0/xero_python/accounting/models/tax_rates.py` & `xero_python-3.0.0/xero_python/accounting/models/tax_rates.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/tax_type.py` & `xero_python-3.0.0/xero_python/accounting/models/tax_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,7 +140,10 @@
     TXRCREY24 = "TXRCREY24"
     IMY24 = "IMY24"
     IMESSY24 = "IMESSY24"
     IMN33Y24 = "IMN33Y24"
     IMREY24 = "IMREY24"
     BADDEBTRECOVERYY24 = "BADDEBTRECOVERYY24"
     OSOUTPUT2 = "OSOUTPUT2"
+    BLINPUT3 = "BLINPUT3"
+    BLINPUT3Y23 = "BLINPUT3Y23"
+    BLINPUT3Y24 = "BLINPUT3Y24"
```

### Comparing `xero_python-2.0.0/xero_python/accounting/models/ten_ninety_nine_contact.py` & `xero_python-3.0.0/xero_python/accounting/models/ten_ninety_nine_contact.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/ten_nintey_nine_contact.py` & `xero_python-3.0.0/xero_python/accounting/models/ten_nintey_nine_contact.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/time_zone.py` & `xero_python-3.0.0/xero_python/accounting/models/time_zone.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/tracking_categories.py` & `xero_python-3.0.0/xero_python/accounting/models/tracking_categories.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/tracking_category.py` & `xero_python-3.0.0/xero_python/accounting/models/tracking_category.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/tracking_option.py` & `xero_python-3.0.0/xero_python/accounting/models/tracking_option.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/tracking_options.py` & `xero_python-3.0.0/xero_python/accounting/models/tracking_options.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/user.py` & `xero_python-3.0.0/xero_python/accounting/models/user.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/users.py` & `xero_python-3.0.0/xero_python/accounting/models/users.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/accounting/models/validation_error.py` & `xero_python-3.0.0/xero_python/accounting/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/api_client/__init__.py` & `xero_python-3.0.0/xero_python/api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/api_client/configuration.py` & `xero_python-3.0.0/xero_python/api_client/configuration.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/api_client/deserializer.py` & `xero_python-3.0.0/xero_python/api_client/deserializer.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/api_client/oauth2.py` & `xero_python-3.0.0/xero_python/api_client/oauth2.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/api_client/serializer.py` & `xero_python-3.0.0/xero_python/api_client/serializer.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/appstore/__init__.py` & `xero_python-3.0.0/xero_python/appstore/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/appstore/api/app_store_api.py` & `xero_python-3.0.0/xero_python/appstore/api/app_store_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     These endpoints are for Xero Partners to interact with the App Store Billing platform  # noqa: E501
 
     Contact: api@xero.com
     Generated by: https://openapi-generator.tech
 """
 
 """
-    OpenAPI spec version: 3.0.0
+    OpenAPI spec version: 3.0.3
 """
 
 import importlib
 import re  # noqa: F401
 
 from xero_python import exceptions
 from xero_python.api_client import ApiClient, ModelFinder
```

### Comparing `xero_python-2.0.0/xero_python/appstore/models/__init__.py` & `xero_python-3.0.0/xero_python/appstore/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/appstore/models/create_usage_record.py` & `xero_python-3.0.0/xero_python/appstore/models/create_usage_record.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/appstore/models/plan.py` & `xero_python-3.0.0/xero_python/appstore/models/plan.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/appstore/models/price.py` & `xero_python-3.0.0/xero_python/appstore/models/price.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/appstore/models/problem_details.py` & `xero_python-3.0.0/xero_python/appstore/models/problem_details.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/appstore/models/product.py` & `xero_python-3.0.0/xero_python/appstore/models/product.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/appstore/models/subscription.py` & `xero_python-3.0.0/xero_python/appstore/models/subscription.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/appstore/models/subscription_item.py` & `xero_python-3.0.0/xero_python/appstore/models/subscription_item.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/appstore/models/update_usage_record.py` & `xero_python-3.0.0/xero_python/appstore/models/update_usage_record.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/appstore/models/usage_record.py` & `xero_python-3.0.0/xero_python/appstore/models/usage_record.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/appstore/models/usage_records_list.py` & `xero_python-3.0.0/xero_python/appstore/models/usage_records_list.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/__init__.py` & `xero_python-3.0.0/xero_python/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/api/asset_api.py` & `xero_python-3.0.0/xero_python/assets/api/asset_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     The Assets API exposes fixed asset related functions of the Xero Accounting application and can be used for a variety of purposes such as creating assets, retrieving asset valuations etc.  # noqa: E501
 
     Contact: api@xero.com
     Generated by: https://openapi-generator.tech
 """
 
 """
-    OpenAPI spec version: 3.0.0
+    OpenAPI spec version: 3.0.3
 """
 
 import importlib
 import re  # noqa: F401
 
 from xero_python import exceptions
 from xero_python.api_client import ApiClient, ModelFinder
```

### Comparing `xero_python-2.0.0/xero_python/assets/models/__init__.py` & `xero_python-3.0.0/xero_python/assets/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/models/asset.py` & `xero_python-3.0.0/xero_python/assets/models/asset.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/models/asset_status.py` & `xero_python-3.0.0/xero_python/assets/models/asset_status.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/models/asset_status_query_param.py` & `xero_python-3.0.0/xero_python/assets/models/asset_status_query_param.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/models/asset_type.py` & `xero_python-3.0.0/xero_python/assets/models/asset_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/models/assets.py` & `xero_python-3.0.0/xero_python/assets/models/assets.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/models/book_depreciation_detail.py` & `xero_python-3.0.0/xero_python/assets/models/book_depreciation_detail.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/models/book_depreciation_setting.py` & `xero_python-3.0.0/xero_python/assets/models/book_depreciation_setting.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/models/error.py` & `xero_python-3.0.0/xero_python/assets/models/error.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/models/field_validation_errors_element.py` & `xero_python-3.0.0/xero_python/assets/models/field_validation_errors_element.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/models/pagination.py` & `xero_python-3.0.0/xero_python/assets/models/pagination.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/models/resource_validation_errors_element.py` & `xero_python-3.0.0/xero_python/assets/models/resource_validation_errors_element.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/assets/models/setting.py` & `xero_python-3.0.0/xero_python/assets/models/setting.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/exceptions/__init__.py` & `xero_python-3.0.0/xero_python/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/exceptions/http_status_exceptions.py` & `xero_python-3.0.0/xero_python/exceptions/http_status_exceptions.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/file/__init__.py` & `xero_python-3.0.0/xero_python/file/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/file/api/files_api.py` & `xero_python-3.0.0/xero_python/file/api/files_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     These endpoints are specific to Xero Files API  # noqa: E501
 
     Contact: api@xero.com
     Generated by: https://openapi-generator.tech
 """
 
 """
-    OpenAPI spec version: 3.0.0
+    OpenAPI spec version: 3.0.3
 """
 
 import importlib
 import re  # noqa: F401
 
 from xero_python import exceptions
 from xero_python.api_client import ApiClient, ModelFinder
```

### Comparing `xero_python-2.0.0/xero_python/file/models/__init__.py` & `xero_python-3.0.0/xero_python/file/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/file/models/association.py` & `xero_python-3.0.0/xero_python/file/models/association.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/file/models/file_object.py` & `xero_python-3.0.0/xero_python/file/models/file_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/file/models/files.py` & `xero_python-3.0.0/xero_python/file/models/files.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/file/models/folder.py` & `xero_python-3.0.0/xero_python/file/models/folder.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/file/models/folders.py` & `xero_python-3.0.0/xero_python/file/models/folders.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/file/models/inline_object.py` & `xero_python-3.0.0/xero_python/file/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/file/models/inline_object1.py` & `xero_python-3.0.0/xero_python/file/models/inline_object1.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/file/models/object_group.py` & `xero_python-3.0.0/xero_python/file/models/object_group.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/file/models/object_type.py` & `xero_python-3.0.0/xero_python/file/models/object_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/file/models/upload_object.py` & `xero_python-3.0.0/xero_python/file/models/upload_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/file/models/user.py` & `xero_python-3.0.0/xero_python/file/models/user.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/__init__.py` & `xero_python-3.0.0/xero_python/finance/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/api/finance_api.py` & `xero_python-3.0.0/xero_python/finance/api/finance_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     The Finance API is a collection of endpoints which customers can use in the course of a loan application, which may assist lenders to gain the confidence they need to provide capital.  # noqa: E501
 
     Contact: api@xero.com
     Generated by: https://openapi-generator.tech
 """
 
 """
-    OpenAPI spec version: 3.0.0
+    OpenAPI spec version: 3.0.3
 """
 
 import importlib
 import re  # noqa: F401
 
 from xero_python import exceptions
 from xero_python.api_client import ApiClient, ModelFinder
```

### Comparing `xero_python-2.0.0/xero_python/finance/models/__init__.py` & `xero_python-3.0.0/xero_python/finance/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/account_usage.py` & `xero_python-3.0.0/xero_python/finance/models/account_usage.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/account_usage_response.py` & `xero_python-3.0.0/xero_python/finance/models/account_usage_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/balance_sheet_account_detail.py` & `xero_python-3.0.0/xero_python/finance/models/balance_sheet_account_detail.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/balance_sheet_account_group.py` & `xero_python-3.0.0/xero_python/finance/models/balance_sheet_account_group.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/balance_sheet_account_type.py` & `xero_python-3.0.0/xero_python/finance/models/balance_sheet_account_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/balance_sheet_response.py` & `xero_python-3.0.0/xero_python/finance/models/balance_sheet_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/bank_statement_accounting_response.py` & `xero_python-3.0.0/xero_python/finance/models/bank_statement_accounting_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/bank_statement_response.py` & `xero_python-3.0.0/xero_python/finance/models/bank_statement_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/bank_transaction_response.py` & `xero_python-3.0.0/xero_python/finance/models/bank_transaction_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/cash_account_response.py` & `xero_python-3.0.0/xero_python/finance/models/cash_account_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/cash_balance.py` & `xero_python-3.0.0/xero_python/finance/models/cash_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/cash_validation_response.py` & `xero_python-3.0.0/xero_python/finance/models/cash_validation_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/cashflow_account.py` & `xero_python-3.0.0/xero_python/finance/models/cashflow_account.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/cashflow_activity.py` & `xero_python-3.0.0/xero_python/finance/models/cashflow_activity.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/cashflow_response.py` & `xero_python-3.0.0/xero_python/finance/models/cashflow_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/cashflow_type.py` & `xero_python-3.0.0/xero_python/finance/models/cashflow_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/contact_detail.py` & `xero_python-3.0.0/xero_python/finance/models/contact_detail.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/contact_response.py` & `xero_python-3.0.0/xero_python/finance/models/contact_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/contact_total_detail.py` & `xero_python-3.0.0/xero_python/finance/models/contact_total_detail.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/contact_total_other.py` & `xero_python-3.0.0/xero_python/finance/models/contact_total_other.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/credit_note_response.py` & `xero_python-3.0.0/xero_python/finance/models/credit_note_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/current_statement_response.py` & `xero_python-3.0.0/xero_python/finance/models/current_statement_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/data_source_response.py` & `xero_python-3.0.0/xero_python/finance/models/data_source_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/history_record_response.py` & `xero_python-3.0.0/xero_python/finance/models/history_record_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/income_by_contact_response.py` & `xero_python-3.0.0/xero_python/finance/models/income_by_contact_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/invoice_response.py` & `xero_python-3.0.0/xero_python/finance/models/invoice_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/line_item_response.py` & `xero_python-3.0.0/xero_python/finance/models/line_item_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/lock_history_model.py` & `xero_python-3.0.0/xero_python/finance/models/lock_history_model.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/lock_history_response.py` & `xero_python-3.0.0/xero_python/finance/models/lock_history_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/manual_journal_total.py` & `xero_python-3.0.0/xero_python/finance/models/manual_journal_total.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/overpayment_response.py` & `xero_python-3.0.0/xero_python/finance/models/overpayment_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/payment_response.py` & `xero_python-3.0.0/xero_python/finance/models/payment_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/pnl_account.py` & `xero_python-3.0.0/xero_python/finance/models/pnl_account.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/pnl_account_class.py` & `xero_python-3.0.0/xero_python/finance/models/pnl_account_class.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/pnl_account_type.py` & `xero_python-3.0.0/xero_python/finance/models/pnl_account_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/practice_response.py` & `xero_python-3.0.0/xero_python/finance/models/practice_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/prepayment_response.py` & `xero_python-3.0.0/xero_python/finance/models/prepayment_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/problem.py` & `xero_python-3.0.0/xero_python/finance/models/problem.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/problem_type.py` & `xero_python-3.0.0/xero_python/finance/models/problem_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/profit_and_loss_response.py` & `xero_python-3.0.0/xero_python/finance/models/profit_and_loss_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/report_history_model.py` & `xero_python-3.0.0/xero_python/finance/models/report_history_model.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/report_history_response.py` & `xero_python-3.0.0/xero_python/finance/models/report_history_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/statement_balance_response.py` & `xero_python-3.0.0/xero_python/finance/models/statement_balance_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/statement_line_response.py` & `xero_python-3.0.0/xero_python/finance/models/statement_line_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/statement_lines_response.py` & `xero_python-3.0.0/xero_python/finance/models/statement_lines_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/statement_response.py` & `xero_python-3.0.0/xero_python/finance/models/statement_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/total_detail.py` & `xero_python-3.0.0/xero_python/finance/models/total_detail.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/total_other.py` & `xero_python-3.0.0/xero_python/finance/models/total_other.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/trial_balance_account.py` & `xero_python-3.0.0/xero_python/finance/models/trial_balance_account.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/trial_balance_entry.py` & `xero_python-3.0.0/xero_python/finance/models/trial_balance_entry.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/trial_balance_movement.py` & `xero_python-3.0.0/xero_python/finance/models/trial_balance_movement.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/trial_balance_response.py` & `xero_python-3.0.0/xero_python/finance/models/trial_balance_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/user_activities_response.py` & `xero_python-3.0.0/xero_python/finance/models/user_activities_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/finance/models/user_response.py` & `xero_python-3.0.0/xero_python/finance/models/user_response.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/identity/__init__.py` & `xero_python-3.0.0/xero_python/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/identity/api/exception_handler.py` & `xero_python-3.0.0/xero_python/identity/api/exception_handler.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/identity/api/identity_api.py` & `xero_python-3.0.0/xero_python/identity/api/identity_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     These endpoints are related to managing authentication tokens and identity for Xero API  # noqa: E501
 
     Contact: api@xero.com
     Generated by: https://openapi-generator.tech
 """
 
 """
-    OpenAPI spec version: 3.0.0
+    OpenAPI spec version: 3.0.3
 """
 
 import importlib
 import re  # noqa: F401
 
 from xero_python import exceptions
 from xero_python.api_client import ApiClient, ModelFinder
```

### Comparing `xero_python-2.0.0/xero_python/identity/models/access_token.py` & `xero_python-3.0.0/xero_python/identity/models/access_token.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/identity/models/connection.py` & `xero_python-3.0.0/xero_python/identity/models/connection.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/identity/models/refresh_token.py` & `xero_python-3.0.0/xero_python/identity/models/refresh_token.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/models.py` & `xero_python-3.0.0/xero_python/models.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/__init__.py` & `xero_python-3.0.0/xero_python/payrollau/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/api/payroll_au_api.py` & `xero_python-3.0.0/xero_python/payrollau/api/payroll_au_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     This is the Xero Payroll API for orgs in Australia region.  # noqa: E501
 
     Contact: api@xero.com
     Generated by: https://openapi-generator.tech
 """
 
 """
-    OpenAPI spec version: 3.0.0
+    OpenAPI spec version: 3.0.3
 """
 
 import importlib
 import re  # noqa: F401
 
 from xero_python import exceptions
 from xero_python.api_client import ApiClient, ModelFinder
```

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/__init__.py` & `xero_python-3.0.0/xero_python/payrollau/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/account.py` & `xero_python-3.0.0/xero_python/payrollau/models/account.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/account_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/account_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/allowance_category.py` & `xero_python-3.0.0/xero_python/payrollau/models/allowance_category.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/allowance_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/allowance_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,11 +26,10 @@
 
     CAR = "CAR"
     TRANSPORT = "TRANSPORT"
     LAUNDRY = "LAUNDRY"
     MEALS = "MEALS"
     TRAVEL = "TRAVEL"
     OTHER = "OTHER"
-    JOBKEEPER = "JOBKEEPER"
     TOOLS = "TOOLS"
     TASKS = "TASKS"
     QUALIFICATIONS = "QUALIFICATIONS"
```

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/api_exception.py` & `xero_python-3.0.0/xero_python/payrollau/models/api_exception.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/bank_account.py` & `xero_python-3.0.0/xero_python/payrollau/models/bank_account.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/calendar_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/calendar_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/country_of_residence.py` & `xero_python-3.0.0/xero_python/payrollau/models/country_of_residence.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/deduction_line.py` & `xero_python-3.0.0/xero_python/payrollau/models/deduction_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/deduction_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/deduction_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/deduction_type_calculation_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/deduction_type_calculation_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/earnings_line.py` & `xero_python-3.0.0/xero_python/payrollau/models/earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/earnings_rate.py` & `xero_python-3.0.0/xero_python/payrollau/models/earnings_rate.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/earnings_rate_calculation_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/earnings_rate_calculation_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/earnings_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/earnings_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/employee.py` & `xero_python-3.0.0/xero_python/payrollau/models/employee.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/employees.py` & `xero_python-3.0.0/xero_python/payrollau/models/employees.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/employment_basis.py` & `xero_python-3.0.0/xero_python/payrollau/models/employment_basis.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/employment_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/employment_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/entitlement_final_pay_payout_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/entitlement_final_pay_payout_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/home_address.py` & `xero_python-3.0.0/xero_python/payrollau/models/home_address.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/income_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/income_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/leave_accrual_line.py` & `xero_python-3.0.0/xero_python/payrollau/models/leave_accrual_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/leave_application.py` & `xero_python-3.0.0/xero_python/payrollau/models/leave_application.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/leave_applications.py` & `xero_python-3.0.0/xero_python/payrollau/models/leave_applications.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/leave_balance.py` & `xero_python-3.0.0/xero_python/payrollau/models/leave_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/leave_category_code.py` & `xero_python-3.0.0/xero_python/payrollau/models/leave_category_code.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/leave_earnings_line.py` & `xero_python-3.0.0/xero_python/payrollau/models/leave_earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/leave_line.py` & `xero_python-3.0.0/xero_python/payrollau/models/leave_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/leave_line_calculation_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/leave_line_calculation_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/leave_lines.py` & `xero_python-3.0.0/xero_python/payrollau/models/leave_lines.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/leave_period.py` & `xero_python-3.0.0/xero_python/payrollau/models/leave_period.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/leave_period_status.py` & `xero_python-3.0.0/xero_python/payrollau/models/leave_period_status.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/leave_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/leave_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/leave_type_contribution_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/leave_type_contribution_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/manual_tax_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/manual_tax_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/opening_balances.py` & `xero_python-3.0.0/xero_python/payrollau/models/opening_balances.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/paid_leave_earnings_line.py` & `xero_python-3.0.0/xero_python/payrollau/models/paid_leave_earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/pay_item.py` & `xero_python-3.0.0/xero_python/payrollau/models/pay_item.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/pay_items.py` & `xero_python-3.0.0/xero_python/payrollau/models/pay_items.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/pay_run.py` & `xero_python-3.0.0/xero_python/payrollau/models/pay_run.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/pay_runs.py` & `xero_python-3.0.0/xero_python/payrollau/models/pay_runs.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/pay_template.py` & `xero_python-3.0.0/xero_python/payrollau/models/pay_template.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/payment_frequency_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/payment_frequency_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/payroll_calendar.py` & `xero_python-3.0.0/xero_python/payrollau/models/payroll_calendar.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/payroll_calendars.py` & `xero_python-3.0.0/xero_python/payrollau/models/payroll_calendars.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/payslip.py` & `xero_python-3.0.0/xero_python/payrollau/models/payslip.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/payslip_lines.py` & `xero_python-3.0.0/xero_python/payrollau/models/payslip_lines.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/payslip_object.py` & `xero_python-3.0.0/xero_python/payrollau/models/payslip_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/payslip_summary.py` & `xero_python-3.0.0/xero_python/payrollau/models/payslip_summary.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/payslips.py` & `xero_python-3.0.0/xero_python/payrollau/models/payslips.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/rate_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/rate_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/reimbursement_line.py` & `xero_python-3.0.0/xero_python/payrollau/models/reimbursement_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/reimbursement_lines.py` & `xero_python-3.0.0/xero_python/payrollau/models/reimbursement_lines.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/reimbursement_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/reimbursement_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/residency_status.py` & `xero_python-3.0.0/xero_python/payrollau/models/residency_status.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/senior_marital_status.py` & `xero_python-3.0.0/xero_python/payrollau/models/senior_marital_status.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/settings.py` & `xero_python-3.0.0/xero_python/payrollau/models/settings.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/settings_object.py` & `xero_python-3.0.0/xero_python/payrollau/models/settings_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/settings_tracking_categories.py` & `xero_python-3.0.0/xero_python/payrollau/models/settings_tracking_categories.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/settings_tracking_categories_employee_groups.py` & `xero_python-3.0.0/xero_python/payrollau/models/settings_tracking_categories_employee_groups.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/settings_tracking_categories_timesheet_categories.py` & `xero_python-3.0.0/xero_python/payrollau/models/settings_tracking_categories_timesheet_categories.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/state.py` & `xero_python-3.0.0/xero_python/payrollau/models/state.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/super_fund.py` & `xero_python-3.0.0/xero_python/payrollau/models/super_fund.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/super_fund_product.py` & `xero_python-3.0.0/xero_python/payrollau/models/super_fund_product.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/super_fund_products.py` & `xero_python-3.0.0/xero_python/payrollau/models/super_fund_products.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/super_funds.py` & `xero_python-3.0.0/xero_python/payrollau/models/super_funds.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/super_line.py` & `xero_python-3.0.0/xero_python/payrollau/models/super_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/super_membership.py` & `xero_python-3.0.0/xero_python/payrollau/models/super_membership.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/superannuation_calculation_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/superannuation_calculation_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/superannuation_contribution_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/superannuation_contribution_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/superannuation_line.py` & `xero_python-3.0.0/xero_python/payrollau/models/superannuation_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/tax_declaration.py` & `xero_python-3.0.0/xero_python/payrollau/models/tax_declaration.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/tax_line.py` & `xero_python-3.0.0/xero_python/payrollau/models/tax_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/tax_scale_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/tax_scale_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/tfn_exemption_type.py` & `xero_python-3.0.0/xero_python/payrollau/models/tfn_exemption_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/timesheet.py` & `xero_python-3.0.0/xero_python/payrollau/models/timesheet.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/timesheet_line.py` & `xero_python-3.0.0/xero_python/payrollau/models/timesheet_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/timesheet_object.py` & `xero_python-3.0.0/xero_python/payrollau/models/timesheet_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/timesheet_status.py` & `xero_python-3.0.0/xero_python/payrollau/models/timesheet_status.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/timesheets.py` & `xero_python-3.0.0/xero_python/payrollau/models/timesheets.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/validation_error.py` & `xero_python-3.0.0/xero_python/payrollau/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollau/models/work_condition.py` & `xero_python-3.0.0/xero_python/payrollau/models/work_condition.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/__init__.py` & `xero_python-3.0.0/xero_python/payrollnz/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/api/payroll_nz_api.py` & `xero_python-3.0.0/xero_python/payrollnz/api/payroll_nz_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     This is the Xero Payroll API for orgs in the NZ region.  # noqa: E501
 
     Contact: api@xero.com
     Generated by: https://openapi-generator.tech
 """
 
 """
-    OpenAPI spec version: 3.0.0
+    OpenAPI spec version: 3.0.3
 """
 
 import importlib
 import re  # noqa: F401
 
 from xero_python import exceptions
 from xero_python.api_client import ApiClient, ModelFinder
```

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/__init__.py` & `xero_python-3.0.0/xero_python/payrollnz/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/account.py` & `xero_python-3.0.0/xero_python/payrollnz/models/account.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/accounts.py` & `xero_python-3.0.0/xero_python/payrollnz/models/accounts.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/address.py` & `xero_python-3.0.0/xero_python/payrollnz/models/address.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/bank_account.py` & `xero_python-3.0.0/xero_python/payrollnz/models/bank_account.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/benefit.py` & `xero_python-3.0.0/xero_python/payrollnz/models/benefit.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/calendar_type.py` & `xero_python-3.0.0/xero_python/payrollnz/models/calendar_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/deduction.py` & `xero_python-3.0.0/xero_python/payrollnz/models/deduction.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/deduction_line.py` & `xero_python-3.0.0/xero_python/payrollnz/models/deduction_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/deduction_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/deduction_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/deductions.py` & `xero_python-3.0.0/xero_python/payrollnz/models/deductions.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/earnings_line.py` & `xero_python-3.0.0/xero_python/payrollnz/models/earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/earnings_order.py` & `xero_python-3.0.0/xero_python/payrollnz/models/earnings_order.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/earnings_order_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/earnings_order_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/earnings_orders.py` & `xero_python-3.0.0/xero_python/payrollnz/models/earnings_orders.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/earnings_rate.py` & `xero_python-3.0.0/xero_python/payrollnz/models/earnings_rate.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/earnings_rate_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/earnings_rate_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/earnings_rates.py` & `xero_python-3.0.0/xero_python/payrollnz/models/earnings_rates.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/earnings_template.py` & `xero_python-3.0.0/xero_python/payrollnz/models/earnings_template.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/earnings_template_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/earnings_template_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_earnings_templates.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_earnings_templates.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_leave.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_leave.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_balance.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_balances.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_balances.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_setup.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_setup.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_setup_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_setup_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_type.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_type_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_type_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_leave_types.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_leave_types.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_leaves.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_leaves.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_opening_balance.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_opening_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_opening_balances_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_opening_balances_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_pay_template.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_pay_template.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_pay_template_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_pay_template_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_pay_templates.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_pay_templates.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_leave_balance.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_leave_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_leave_balance_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_leave_balance_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_leave_summary.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_leave_summary.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_leaves_summaries.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_leaves_summaries.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_sick_leave.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_sick_leave.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_sick_leave_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_sick_leave_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_statutory_sick_leaves.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_statutory_sick_leaves.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_tax.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_tax.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employee_tax_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employee_tax_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employees.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employees.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employment.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employment.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/employment_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/employment_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/gross_earnings_history.py` & `xero_python-3.0.0/xero_python/payrollnz/models/gross_earnings_history.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/invalid_field.py` & `xero_python-3.0.0/xero_python/payrollnz/models/invalid_field.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/leave_accrual_line.py` & `xero_python-3.0.0/xero_python/payrollnz/models/leave_accrual_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/leave_earnings_line.py` & `xero_python-3.0.0/xero_python/payrollnz/models/leave_earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/leave_period.py` & `xero_python-3.0.0/xero_python/payrollnz/models/leave_period.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/leave_periods.py` & `xero_python-3.0.0/xero_python/payrollnz/models/leave_periods.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/leave_type.py` & `xero_python-3.0.0/xero_python/payrollnz/models/leave_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/leave_type_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/leave_type_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/leave_types.py` & `xero_python-3.0.0/xero_python/payrollnz/models/leave_types.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/pagination.py` & `xero_python-3.0.0/xero_python/payrollnz/models/pagination.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/pay_run.py` & `xero_python-3.0.0/xero_python/payrollnz/models/pay_run.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/pay_run_calendar.py` & `xero_python-3.0.0/xero_python/payrollnz/models/pay_run_calendar.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/pay_run_calendar_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/pay_run_calendar_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/pay_run_calendars.py` & `xero_python-3.0.0/xero_python/payrollnz/models/pay_run_calendars.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/pay_run_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/pay_run_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/pay_runs.py` & `xero_python-3.0.0/xero_python/payrollnz/models/pay_runs.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/pay_slip.py` & `xero_python-3.0.0/xero_python/payrollnz/models/pay_slip.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/pay_slip_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/pay_slip_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/pay_slips.py` & `xero_python-3.0.0/xero_python/payrollnz/models/pay_slips.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/payment_line.py` & `xero_python-3.0.0/xero_python/payrollnz/models/payment_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/payment_method.py` & `xero_python-3.0.0/xero_python/payrollnz/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/payment_method_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/payment_method_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/problem.py` & `xero_python-3.0.0/xero_python/payrollnz/models/problem.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/reimbursement.py` & `xero_python-3.0.0/xero_python/payrollnz/models/reimbursement.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/reimbursement_line.py` & `xero_python-3.0.0/xero_python/payrollnz/models/reimbursement_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/reimbursement_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/reimbursement_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/reimbursements.py` & `xero_python-3.0.0/xero_python/payrollnz/models/reimbursements.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/salary_and_wage.py` & `xero_python-3.0.0/xero_python/payrollnz/models/salary_and_wage.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/salary_and_wage_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/salary_and_wage_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/salary_and_wages.py` & `xero_python-3.0.0/xero_python/payrollnz/models/salary_and_wages.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/settings.py` & `xero_python-3.0.0/xero_python/payrollnz/models/settings.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/statutory_deduction.py` & `xero_python-3.0.0/xero_python/payrollnz/models/statutory_deduction.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/statutory_deduction_category.py` & `xero_python-3.0.0/xero_python/payrollnz/models/statutory_deduction_category.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/statutory_deduction_line.py` & `xero_python-3.0.0/xero_python/payrollnz/models/statutory_deduction_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/statutory_deduction_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/statutory_deduction_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/statutory_deductions.py` & `xero_python-3.0.0/xero_python/payrollnz/models/statutory_deductions.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/superannuation_line.py` & `xero_python-3.0.0/xero_python/payrollnz/models/superannuation_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/superannuation_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/superannuation_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/superannuations.py` & `xero_python-3.0.0/xero_python/payrollnz/models/superannuations.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/tax_code.py` & `xero_python-3.0.0/xero_python/payrollnz/models/tax_code.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/tax_line.py` & `xero_python-3.0.0/xero_python/payrollnz/models/tax_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/tax_settings.py` & `xero_python-3.0.0/xero_python/payrollnz/models/tax_settings.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/timesheet.py` & `xero_python-3.0.0/xero_python/payrollnz/models/timesheet.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/timesheet_earnings_line.py` & `xero_python-3.0.0/xero_python/payrollnz/models/timesheet_earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/timesheet_line.py` & `xero_python-3.0.0/xero_python/payrollnz/models/timesheet_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/timesheet_line_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/timesheet_line_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/timesheet_object.py` & `xero_python-3.0.0/xero_python/payrollnz/models/timesheet_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/timesheets.py` & `xero_python-3.0.0/xero_python/payrollnz/models/timesheets.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/tracking_categories.py` & `xero_python-3.0.0/xero_python/payrollnz/models/tracking_categories.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrollnz/models/tracking_category.py` & `xero_python-3.0.0/xero_python/payrollnz/models/tracking_category.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/__init__.py` & `xero_python-3.0.0/xero_python/payrolluk/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/api/exception_handler.py` & `xero_python-3.0.0/xero_python/payrolluk/api/exception_handler.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/api/payroll_uk_api.py` & `xero_python-3.0.0/xero_python/payrolluk/api/payroll_uk_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     This is the Xero Payroll API for orgs in the UK region.  # noqa: E501
 
     Contact: api@xero.com
     Generated by: https://openapi-generator.tech
 """
 
 """
-    OpenAPI spec version: 3.0.0
+    OpenAPI spec version: 3.0.3
 """
 
 import importlib
 import re  # noqa: F401
 
 from xero_python import exceptions
 from xero_python.api_client import ApiClient, ModelFinder
```

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/__init__.py` & `xero_python-3.0.0/xero_python/payrolluk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/account.py` & `xero_python-3.0.0/xero_python/payrolluk/models/account.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/accounts.py` & `xero_python-3.0.0/xero_python/payrolluk/models/accounts.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/address.py` & `xero_python-3.0.0/xero_python/payrolluk/models/address.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/bank_account.py` & `xero_python-3.0.0/xero_python/payrolluk/models/bank_account.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/benefit.py` & `xero_python-3.0.0/xero_python/payrolluk/models/benefit.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/benefit_line.py` & `xero_python-3.0.0/xero_python/payrolluk/models/benefit_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/benefit_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/benefit_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/benefits.py` & `xero_python-3.0.0/xero_python/payrolluk/models/benefits.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/court_order_line.py` & `xero_python-3.0.0/xero_python/payrolluk/models/court_order_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/deduction.py` & `xero_python-3.0.0/xero_python/payrolluk/models/deduction.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/deduction_line.py` & `xero_python-3.0.0/xero_python/payrolluk/models/deduction_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/deduction_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/deduction_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/deductions.py` & `xero_python-3.0.0/xero_python/payrolluk/models/deductions.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/earnings_line.py` & `xero_python-3.0.0/xero_python/payrolluk/models/earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/earnings_order.py` & `xero_python-3.0.0/xero_python/payrolluk/models/earnings_order.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/earnings_order_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/earnings_order_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/earnings_orders.py` & `xero_python-3.0.0/xero_python/payrolluk/models/earnings_orders.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/earnings_rate.py` & `xero_python-3.0.0/xero_python/payrolluk/models/earnings_rate.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/earnings_rate_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/earnings_rate_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/earnings_rates.py` & `xero_python-3.0.0/xero_python/payrolluk/models/earnings_rates.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/earnings_template.py` & `xero_python-3.0.0/xero_python/payrolluk/models/earnings_template.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/earnings_template_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/earnings_template_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_leave.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_leave.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_leave_balance.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_leave_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_leave_balances.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_leave_balances.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_leave_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_leave_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_leave_type.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_leave_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_leave_type_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_leave_type_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_leave_types.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_leave_types.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_leaves.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_leaves.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_opening_balances.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_opening_balances.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_opening_balances_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_opening_balances_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_pay_template.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_pay_template.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_pay_template_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_pay_template_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_pay_templates.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_pay_templates.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_leave_balance.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_leave_balance.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_leave_balance_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_leave_balance_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_leave_summary.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_leave_summary.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_leaves_summaries.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_leaves_summaries.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_sick_leave.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_sick_leave.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_sick_leave_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_sick_leave_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_statutory_sick_leaves.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_statutory_sick_leaves.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_tax.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_tax.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employee_tax_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employee_tax_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employees.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employees.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employment.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employment.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/employment_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/employment_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/invalid_field.py` & `xero_python-3.0.0/xero_python/payrolluk/models/invalid_field.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/leave_accrual_line.py` & `xero_python-3.0.0/xero_python/payrolluk/models/leave_accrual_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/leave_earnings_line.py` & `xero_python-3.0.0/xero_python/payrolluk/models/leave_earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/leave_period.py` & `xero_python-3.0.0/xero_python/payrolluk/models/leave_period.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/leave_periods.py` & `xero_python-3.0.0/xero_python/payrolluk/models/leave_periods.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/leave_type.py` & `xero_python-3.0.0/xero_python/payrolluk/models/leave_type.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/leave_type_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/leave_type_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/leave_types.py` & `xero_python-3.0.0/xero_python/payrolluk/models/leave_types.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/pagination.py` & `xero_python-3.0.0/xero_python/payrolluk/models/pagination.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/pay_run.py` & `xero_python-3.0.0/xero_python/payrolluk/models/pay_run.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/pay_run_calendar.py` & `xero_python-3.0.0/xero_python/payrolluk/models/pay_run_calendar.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/pay_run_calendar_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/pay_run_calendar_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/pay_run_calendars.py` & `xero_python-3.0.0/xero_python/payrolluk/models/pay_run_calendars.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/pay_run_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/pay_run_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/pay_runs.py` & `xero_python-3.0.0/xero_python/payrolluk/models/pay_runs.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/payment_line.py` & `xero_python-3.0.0/xero_python/payrolluk/models/payment_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/payment_method.py` & `xero_python-3.0.0/xero_python/payrolluk/models/payment_method.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/payment_method_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/payment_method_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/payslip.py` & `xero_python-3.0.0/xero_python/payrolluk/models/payslip.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/payslip_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/payslip_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/payslips.py` & `xero_python-3.0.0/xero_python/payrolluk/models/payslips.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/problem.py` & `xero_python-3.0.0/xero_python/payrolluk/models/problem.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/reimbursement.py` & `xero_python-3.0.0/xero_python/payrolluk/models/reimbursement.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/reimbursement_line.py` & `xero_python-3.0.0/xero_python/payrolluk/models/reimbursement_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/reimbursement_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/reimbursement_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/reimbursements.py` & `xero_python-3.0.0/xero_python/payrolluk/models/reimbursements.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/salary_and_wage.py` & `xero_python-3.0.0/xero_python/payrolluk/models/salary_and_wage.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/salary_and_wage_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/salary_and_wage_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/salary_and_wages.py` & `xero_python-3.0.0/xero_python/payrolluk/models/salary_and_wages.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/settings.py` & `xero_python-3.0.0/xero_python/payrolluk/models/settings.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/statutory_deduction.py` & `xero_python-3.0.0/xero_python/payrolluk/models/statutory_deduction.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/statutory_deduction_category.py` & `xero_python-3.0.0/xero_python/payrolluk/models/statutory_deduction_category.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/tax_line.py` & `xero_python-3.0.0/xero_python/payrolluk/models/tax_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/timesheet.py` & `xero_python-3.0.0/xero_python/payrolluk/models/timesheet.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/timesheet_earnings_line.py` & `xero_python-3.0.0/xero_python/payrolluk/models/timesheet_earnings_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/timesheet_line.py` & `xero_python-3.0.0/xero_python/payrolluk/models/timesheet_line.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/timesheet_line_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/timesheet_line_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/timesheet_object.py` & `xero_python-3.0.0/xero_python/payrolluk/models/timesheet_object.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/timesheets.py` & `xero_python-3.0.0/xero_python/payrolluk/models/timesheets.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/tracking_categories.py` & `xero_python-3.0.0/xero_python/payrolluk/models/tracking_categories.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/payrolluk/models/tracking_category.py` & `xero_python-3.0.0/xero_python/payrolluk/models/tracking_category.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/__init__.py` & `xero_python-3.0.0/xero_python/project/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/api/project_api.py` & `xero_python-3.0.0/xero_python/project/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     This is the Xero Projects API  # noqa: E501
 
     Contact: api@xero.com
     Generated by: https://openapi-generator.tech
 """
 
 """
-    OpenAPI spec version: 3.0.0
+    OpenAPI spec version: 3.0.3
 """
 
 import importlib
 import re  # noqa: F401
 
 from xero_python import exceptions
 from xero_python.api_client import ApiClient, ModelFinder
```

### Comparing `xero_python-2.0.0/xero_python/project/models/__init__.py` & `xero_python-3.0.0/xero_python/project/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/amount.py` & `xero_python-3.0.0/xero_python/project/models/amount.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/currency_code.py` & `xero_python-3.0.0/xero_python/project/models/currency_code.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/error.py` & `xero_python-3.0.0/xero_python/project/models/error.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/pagination.py` & `xero_python-3.0.0/xero_python/project/models/pagination.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/project.py` & `xero_python-3.0.0/xero_python/project/models/project.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/project_create_or_update.py` & `xero_python-3.0.0/xero_python/project/models/project_create_or_update.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/project_patch.py` & `xero_python-3.0.0/xero_python/project/models/project_patch.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/project_user.py` & `xero_python-3.0.0/xero_python/project/models/project_user.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/project_users.py` & `xero_python-3.0.0/xero_python/project/models/project_users.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/projects.py` & `xero_python-3.0.0/xero_python/project/models/projects.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/task.py` & `xero_python-3.0.0/xero_python/project/models/task.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/task_create_or_update.py` & `xero_python-3.0.0/xero_python/project/models/task_create_or_update.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/tasks.py` & `xero_python-3.0.0/xero_python/project/models/tasks.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/time_entries.py` & `xero_python-3.0.0/xero_python/project/models/time_entries.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/time_entry.py` & `xero_python-3.0.0/xero_python/project/models/time_entry.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/project/models/time_entry_create_or_update.py` & `xero_python-3.0.0/xero_python/project/models/time_entry_create_or_update.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/rest.py` & `xero_python-3.0.0/xero_python/rest.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/single_dispatch_str.py` & `xero_python-3.0.0/xero_python/single_dispatch_str.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python/utils.py` & `xero_python-3.0.0/xero_python/utils.py`

 * *Files identical despite different names*

### Comparing `xero_python-2.0.0/xero_python.egg-info/PKG-INFO` & `xero_python-3.0.0/xero_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xero-python
-Version: 2.0.0
+Version: 3.0.0
 Summary: Official Python sdk for Xero API generated by OpenAPI spec for oAuth2
 Author: Xero Developer API
 Author-email: api@xero.com
 License: MIT license
 Keywords: xero python sdk API oAuth
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `xero_python-2.0.0/xero_python.egg-info/SOURCES.txt` & `xero_python-3.0.0/xero_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

