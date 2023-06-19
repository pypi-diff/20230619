# Comparing `tmp/odoo12-addon-somconnexio-12.0.2.2.2.tar.gz` & `tmp/odoo12-addon-somconnexio-12.0.2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo12-addon-somconnexio-12.0.2.2.2.tar", last modified: Mon Jun 12 17:42:40 2023, max compression
+gzip compressed data, was "dist/odoo12-addon-somconnexio-12.0.2.3.0.tar", last modified: Mon Jun 19 13:23:23 2023, max compression
```

## Comparing `odoo12-addon-somconnexio-12.0.2.2.2.tar` & `odoo12-addon-somconnexio-12.0.2.3.0.tar`

### file list

```diff
@@ -1,596 +1,600 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/
--rw-r--r--   0 root         (0) root         (0)     4972 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4507 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/README.md
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9643 2023-06-12 17:15:23.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/__manifest__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/controllers/
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/controllers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5170 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/controllers/controllers.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/controllers/http.py
--rw-rw-rw-   0 root         (0) root         (0)     3458 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/controllers/public_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/correos_services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/correos_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4432 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/correos_services/shipment.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/
--rw-rw-rw-   0 root         (0) root         (0)    46993 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account.account.template-sc.csv
--rw-rw-rw-   0 root         (0) root         (0)      712 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account_chart_template_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     2954 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account_group.xml
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account_journal.xml
--rw-rw-rw-   0 root         (0) root         (0)     2599 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account_payment_mode.xml
--rw-rw-rw-   0 root         (0) root         (0)     4496 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account_payment_term.xml
--rw-rw-rw-   0 root         (0) root         (0)     1730 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account_tax.xml
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account_tax_group.xml
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/analytic_account.xml
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/base_automation.xml
--rw-rw-rw-   0 root         (0) root         (0)     2241 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/company.xml
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/contract_compute_current_tariff_cron.xml
--rw-rw-rw-   0 root         (0) root         (0)     3786 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/contract_terminate_reason.xml
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/contract_terminate_user_reason.xml
--rw-rw-rw-   0 root         (0) root         (0)      947 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/crm_stage_data.xml
--rw-rw-rw-   0 root         (0) root         (0)      658 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/crm_track_correos_delivery_cron.xml
--rw-rw-rw-   0 root         (0) root         (0)     1238 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/discovery_channel.xml
--rw-rw-rw-   0 root         (0) root         (0)      752 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/fiber_signal_type_data.xml
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/hr_attendance_place.xml
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/ir_config_pararameter.xml
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/ir_sequence.xml
--rw-rw-rw-   0 root         (0) root         (0)    13962 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/mail_activity_type.xml
--rw-rw-rw-   0 root         (0) root         (0)      150 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/mail_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     3266 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/mail_mass_mailing_list_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/mis_report.xml
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/operation_request_terminate_reason.xml
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/partner_action_tag_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/partner_priority.xml
--rw-rw-rw-   0 root         (0) root         (0)    13582 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/previous_provider_data.xml
--rw-rw-rw-   0 root         (0) root         (0)     1459 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_attribute.xml
--rw-rw-rw-   0 root         (0) root         (0)     7767 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_attribute_value.xml
--rw-rw-rw-   0 root         (0) root         (0)     2455 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_categories.xml
--rw-rw-rw-   0 root         (0) root         (0)     7830 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_category_technology_supplier_data.xml
--rw-rw-rw-   0 root         (0) root         (0)    10349 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_pack_line.xml
--rw-rw-rw-   0 root         (0) root         (0)    40646 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_product.xml
--rw-rw-rw-   0 root         (0) root         (0)     5653 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_template_attribute_line_data.xml
--rw-rw-rw-   0 root         (0) root         (0)    11160 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_template_data.xml
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/res.partner.bank.xml
--rw-rw-rw-   0 root         (0) root         (0)      426 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/res.users.xml
--rw-rw-rw-   0 root         (0) root         (0)     3704 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/res_bank_data.xml
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/service_supplier.xml
--rw-rw-rw-   0 root         (0) root         (0)      591 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/service_technology.xml
--rw-rw-rw-   0 root         (0) root         (0)     1908 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/service_technology_service_supplier.xml
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/share_type.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/demo/
--rw-rw-rw-   0 root         (0) root         (0)     6259 2023-06-12 17:15:23.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/demo/partner.xml
--rw-rw-rw-   0 root         (0) root         (0)    13717 2023-06-12 12:44:50.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/demo/pricelist.xml
--rw-rw-rw-   0 root         (0) root         (0)     2346 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/demo/subscription_requests.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/helpers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/helpers/date.py
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/helpers/language.py
--rw-rw-rw-   0 root         (0) root         (0)     1846 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/i18n/
--rw-rw-rw-   0 root         (0) root         (0)   320073 2023-06-12 12:44:50.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/i18n/ca_ES.po
--rw-rw-rw-   0 root         (0) root         (0)   329543 2023-06-12 12:44:50.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/i18n/es.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/listeners/
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/listeners/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3078 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/listeners/contract_line_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/listeners/contract_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/listeners/crm_lead_listener.py
--rw-rw-rw-   0 root         (0) root         (0)      742 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/listeners/partner_bank_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     1355 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/listeners/partner_listener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.8/pre-clean-mail-tracking-value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.8.11/
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.8.11/post-create-copy-contract-service-info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.8.4/
--rw-rw-rw-   0 root         (0) root         (0)     2709 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.8.4/post-create-copy-contract-service-info.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.8.4/pre-create-one-gb-wo-cost.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9/
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9/post-link-crm-to-contract.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9/post-migrate-change-address.py
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9/pre-migrate-change-address.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9/pre-uniform-contracts-wo-number.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9.13/
--rw-rw-rw-   0 root         (0) root         (0)     1215 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9.13/post-change-activities-user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9.2/
--rw-rw-rw-   0 root         (0) root         (0)      533 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9.2/post-upper-sponsorship-code.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9.9/
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9.9/post-import-es-geonames.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-recompute-is-from-pack.py
--rw-rw-rw-   0 root         (0) root         (0)      803 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-relate-is-from-not-pack-attribute-with-existing-products.py
--rw-rw-rw-   0 root         (0) root         (0)     1260 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-create-is-from-pack-attribute.py
--rw-rw-rw-   0 root         (0) root         (0)      575 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-set-xml-id-unlimited-20GB.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     1191 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.1.6/post-set-state_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.1.8/
--rw-rw-rw-   0 root         (0) root         (0)      242 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.1.8/pre-assign-imd-manual-created-activity-types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     2293 2023-06-12 12:44:50.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.2.0/pre-fix-catalog-externalId.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/erppeek/
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/erppeek/README.md
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/erppeek/erppeek.ini
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/erppeek/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)     1043 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/erppeek/update_contract_line_product_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/
--rw-rw-rw-   0 root         (0) root         (0)     1838 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_asset.py
--rw-rw-rw-   0 root         (0) root         (0)      931 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_banking_mandate.py
--rw-rw-rw-   0 root         (0) root         (0)     6377 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_invoice.py
--rw-rw-rw-   0 root         (0) root         (0)     2367 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_invoice_line.py
--rw-rw-rw-   0 root         (0) root         (0)      142 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_journal.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_move.py
--rw-rw-rw-   0 root         (0) root         (0)     3769 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_move_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1330 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_payment_order.py
--rw-rw-rw-   0 root         (0) root         (0)     1897 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_payment_return_email_gateway.py
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_tax.py
--rw-rw-rw-   0 root         (0) root         (0)    21169 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/aged_partner_balance.py
--rw-rw-rw-   0 root         (0) root         (0)     7108 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/aged_partner_balance_xlsx.py
--rw-rw-rw-   0 root         (0) root         (0)    39338 2023-06-12 12:44:50.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/contract.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/contract_info/
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/contract_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/contract_info/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3230 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/contract_info/broadband.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/contract_info/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/contract_terminate_reason.py
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/contract_terminate_user_reason.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/coop_agreement.py
--rw-rw-rw-   0 root         (0) root         (0)    21856 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/crm_lead.py
--rw-rw-rw-   0 root         (0) root         (0)    11230 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      151 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/discovery_channel.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/fiber_signal_type.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/hr_attendance.py
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/hr_attendance_place.py
--rw-rw-rw-   0 root         (0) root         (0)     3864 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/hr_employee.py
--rw-rw-rw-   0 root         (0) root         (0)     4417 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/ir_model_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/ir_server_action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/isp_info/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/isp_info/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3680 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/isp_info/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3644 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/isp_info/broadband.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/isp_info/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)     1570 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/l10n_es_aeat_report.py
--rw-rw-rw-   0 root         (0) root         (0)     3881 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/mail_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/mail_thread.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/mass_mailing.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/mobile_contract_otrs_view.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/opencell_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/operation_request.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/operation_request_terminate_reason.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/partner_action_tag.py
--rw-rw-rw-   0 root         (0) root         (0)     2816 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/partner_otrs_view.py
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/payment_return.py
--rw-rw-rw-   0 root         (0) root         (0)     3407 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/payment_return_line.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/previous_provider.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/product_attribute_value.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/product_category_technology_supplier.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/product_pack_line.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/product_pricelist.py
--rw-rw-rw-   0 root         (0) root         (0)     5752 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/product_product.py
--rw-rw-rw-   0 root         (0) root         (0)      640 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/product_template.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/res_company.py
--rw-rw-rw-   0 root         (0) root         (0)    22511 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/res_partner_bank.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/service_supplier.py
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/service_technology.py
--rw-rw-rw-   0 root         (0) root         (0)     2509 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/stock_move_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1818 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/stock_production_lot.py
--rw-rw-rw-   0 root         (0) root         (0)    12471 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/subscription_request.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/utm_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/access.py
--rw-rw-rw-   0 root         (0) root         (0)     1310 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/account_hierarchy_resource.py
--rw-rw-rw-   0 root         (0) root         (0)     5121 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/crm_account_hierarchy.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/customer.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/opencell_resource.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/opencell_types/
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/opencell_types/address.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/opencell_types/custom_field.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/opencell_types/description.py
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/services.py
--rw-rw-rw-   0 root         (0) root         (0)     2144 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2944 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_strategies.py
--rw-rw-rw-   0 root         (0) root         (0)     3430 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_service.py
--rw-rw-rw-   0 root         (0) root         (0)     5227 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_strategies.py
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/customer_update_service.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/opencell_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/subscription_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/adsl_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1152 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/base_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     2508 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/broadband_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/customer_data_from_res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-06-12 13:12:45.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/fiber_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1749 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/mobile_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/router_4G_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/service_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/update_ticket_with_error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/account_asset_report_xls.py
--rw-rw-rw-   0 root         (0) root         (0)    20209 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/aged_partner_balance.xml
--rw-rw-rw-   0 root         (0) root         (0)     3285 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/crm_lead_creation_email_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     1363 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/invoice_claim_1_capital_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     1398 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/invoice_claim_1_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     1969 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/mobile_can_be_linked_with_fiber_mail_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/mobile_linked_with_fiber_mail_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     3799 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/new_sim_sending_letter_template.xml
--rw-rw-rw-   0 root         (0) root         (0)      720 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/report_paperformat.xml
--rw-rw-rw-   0 root         (0) root         (0)     8425 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/sim_sending_letter_template.xml
--rw-rw-rw-   0 root         (0) root         (0)     3036 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/sponsor_sell_back_template.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/security/
--rw-rw-rw-   0 root         (0) root         (0)     7111 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/security/ir.model.access.csv
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/security/res_groups.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5557 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/account_invoice_process.py
--rw-rw-rw-   0 root         (0) root         (0)      500 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/account_invoice_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3164 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/account_payment_group_process.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/bank_from_iban_getter.py
--rw-rw-rw-   0 root         (0) root         (0)     3602 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/change_partner_emails.py
--rw-rw-rw-   0 root         (0) root         (0)     5468 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_change_tariff_process.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_change_tariff_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1657 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_contract_process.py
--rw-rw-rw-   0 root         (0) root         (0)     7641 2023-06-12 17:15:23.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_contract_service.py
--rw-rw-rw-   0 root         (0) root         (0)     3710 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_email_change_process.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_email_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_iban_change_process.py
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_iban_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2809 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_one_shot_process.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_one_shot_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/
--rw-rw-rw-   0 root         (0) root         (0)      166 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2008 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/adsl.py
--rw-rw-rw-   0 root         (0) root         (0)     1054 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/ba.py
--rw-rw-rw-   0 root         (0) root         (0)    13704 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10651 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/fiber.py
--rw-rw-rw-   0 root         (0) root         (0)     3378 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/router4g.py
--rw-rw-rw-   0 root         (0) root         (0)     8974 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/crm_lead_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/discovery_channel_service.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/get_activation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      352 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/hashids_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/partner_email_change_process.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/partner_email_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)     8806 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/product_catalog_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/provider_service.py
--rw-rw-rw-   0 root         (0) root         (0)     5730 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/res_partner_service.py
--rw-rw-rw-   0 root         (0) root         (0)    21653 2023-06-12 17:15:23.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/schemas.py
--rw-rw-rw-   0 root         (0) root         (0)     5848 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/subscription_request_service.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/vat_normalizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/somoffice/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/somoffice/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/somoffice/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     2167 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/somoffice/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/
--rw-rw-rw-   0 root         (0) root         (0)     9682 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/activities.png
--rw-rw-rw-   0 root         (0) root         (0)    12957 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/broadband_contract.png
--rw-rw-rw-   0 root         (0) root         (0)    13548 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/broadband_lead_lines.png
--rw-rw-rw-   0 root         (0) root         (0)     6550 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/emails.png
--rw-rw-rw-   0 root         (0) root         (0)    15486 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/mobile_contract.png
--rw-rw-rw-   0 root         (0) root         (0)    15574 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/mobile_lead_lines.png
--rw-rw-rw-   0 root         (0) root         (0)    15844 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/packs.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/img/
--rw-rw-rw-   0 root         (0) root         (0)    17014 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/img/sc-image.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/js/
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/js/holidays_highlighter.js
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/js/many2many_tags_contract_email.js
--rw-rw-rw-   0 root         (0) root         (0)      605 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/js/many2one_tags_crm_lead_email.js
--rw-rw-rw-   0 root         (0) root         (0)     2931 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/js/my_attendances.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/xml/
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/xml/activity.xml
--rw-rw-rw-   0 root         (0) root         (0)      684 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/xml/attendance.xml
--rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/xml/contract_email.xml
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/xml/mail_chatter_buttons.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4825 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-12 17:15:23.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/common_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/correos_services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/correos_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7677 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/correos_services/test_shipment.py
--rw-rw-rw-   0 root         (0) root         (0)     3047 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)     6137 2023-06-12 13:12:45.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10823 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/test_contract_line_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     5866 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/test_contract_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     3491 2023-06-12 13:12:45.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/test_crm_lead_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/test_partner_bank_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     7360 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/test_partner_listener.py
--rw-rw-rw-   0 root         (0) root         (0)     2599 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/test_res_partner_listener.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4310 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_account_invoice.py
--rw-rw-rw-   0 root         (0) root         (0)     3598 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_account_move_line.py
--rw-rw-rw-   0 root         (0) root         (0)     3854 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_account_payment_order.py
--rw-rw-rw-   0 root         (0) root         (0)     5342 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_account_payment_return_gateway.py
--rw-rw-rw-   0 root         (0) root         (0)     4540 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_broadband_isp_info.py
--rw-rw-rw-   0 root         (0) root         (0)    33841 2023-06-12 17:15:23.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_contract.py
--rw-rw-rw-   0 root         (0) root         (0)     5657 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_coop_agreement.py
--rw-rw-rw-   0 root         (0) root         (0)    85607 2023-06-12 13:12:45.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_crm_lead.py
--rw-rw-rw-   0 root         (0) root         (0)     9390 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1646 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_hr_attendance_process.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_mail_activity.py
--rw-rw-rw-   0 root         (0) root         (0)     5484 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_mass_mailing.py
--rw-rw-rw-   0 root         (0) root         (0)     6492 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_mobile_isp_info.py
--rw-rw-rw-   0 root         (0) root         (0)     2485 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_opencell_configuration_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     9187 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_payment_return.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_previous_provider.py
--rw-rw-rw-   0 root         (0) root         (0)    28217 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_product_category_technology_supplier.py
--rw-rw-rw-   0 root         (0) root         (0)     1579 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_product_product.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_product_template.py
--rw-rw-rw-   0 root         (0) root         (0)     2932 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_production_lot.py
--rw-rw-rw-   0 root         (0) root         (0)    46314 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_res_partner_bank.py
--rw-rw-rw-   0 root         (0) root         (0)     5237 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_server_action.py
--rw-rw-rw-   0 root         (0) root         (0)    10862 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_service_supplier.py
--rw-rw-rw-   0 root         (0) root         (0)     4876 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_stock_move_line.py
--rw-rw-rw-   0 root         (0) root         (0)    26854 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_subscription_request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_models/test_address.py
--rw-rw-rw-   0 root         (0) root         (0)    11179 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_models/test_crm_account_hierarchy.py
--rw-rw-rw-   0 root         (0) root         (0)     4261 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_models/test_customer.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_models/test_description.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_models/test_opencell_service_codes.py
--rw-rw-rw-   0 root         (0) root         (0)     4105 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_models/test_subscription.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15080 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_service.py
--rw-rw-rw-   0 root         (0) root         (0)    10511 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_strategies.py
--rw-rw-rw-   0 root         (0) root         (0)     6230 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_service.py
--rw-rw-rw-   0 root         (0) root         (0)    15234 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_strategies.py
--rw-rw-rw-   0 root         (0) root         (0)     2335 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/test_customer_update_service.py
--rw-rw-rw-   0 root         (0) root         (0)     7743 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/test_subscription_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5744 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/test_adsl_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/test_customer_data_from_res_partner.py
--rw-rw-rw-   0 root         (0) root         (0)    10104 2023-06-12 13:12:45.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/test_fiber_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     6530 2023-06-12 13:12:45.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/test_mobile_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     4644 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/test_router_4G_data_from_crm_lead_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1657 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/test_update_ticket_with_error.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/sc_test_case.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_process/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_process/base_test_contract_process.py
--rw-rw-rw-   0 root         (0) root         (0)    25341 2023-06-12 13:12:45.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_process/test_fiber_contract_process.py
--rw-rw-rw-   0 root         (0) root         (0)     9744 2023-06-12 13:12:45.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_process/test_mobile_contract_process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_services/
--rw-rw-rw-   0 root         (0) root         (0)    71859 2023-06-12 17:15:23.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_contract_service.py
--rw-rw-rw-   0 root         (0) root         (0)     6513 2023-06-12 17:15:23.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_count_controller.py
--rw-rw-rw-   0 root         (0) root         (0)    19447 2023-06-12 17:15:23.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_get_fiber_contracts_to_pack_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7776 2023-06-12 17:15:23.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_search_controller.py
--rw-rw-rw-   0 root         (0) root         (0)    43501 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_account_invoice_service.py
--rw-rw-rw-   0 root         (0) root         (0)     7531 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_change_partner_emails.py
--rw-rw-rw-   0 root         (0) root         (0)    15498 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_contract_change_tariff_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2980 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_contract_contract_process.py
--rw-rw-rw-   0 root         (0) root         (0)    12908 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_contract_email_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)    13013 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_contract_iban_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_contract_one_shot_service.py
--rw-rw-rw-   0 root         (0) root         (0)    34346 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_crm_lead_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1769 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_discovery_channel_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1456 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_get_activation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_hashids_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1501 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_mass_mailing_unsubscribe.py
--rw-rw-rw-   0 root         (0) root         (0)     6003 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_partner_email_change_service.py
--rw-rw-rw-   0 root         (0) root         (0)    16662 2023-06-12 12:44:50.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_product_catalog_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2141 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_provider_service.py
--rw-rw-rw-   0 root         (0) root         (0)    18948 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_res_partner_service.py
--rw-rw-rw-   0 root         (0) root         (0)     8798 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_subscription_request_service.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_vat_normalizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/somoffice/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/somoffice/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/somoffice/test_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-12 17:41:01.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9061 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_account_payment_line_create.py
--rw-rw-rw-   0 root         (0) root         (0)     9357 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_address_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     5693 2023-06-12 12:44:50.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_compensation_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     2552 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_force_oc_integration_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    21666 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_holder_change.py
--rw-rw-rw-   0 root         (0) root         (0)     3581 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_force_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     4007 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     5504 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_invoice_payment_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     9940 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_mobile_tariff_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    13855 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_one_shot_request_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    12968 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_tariff_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     3322 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_terminate_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)    30774 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_create_lead_from_partner_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     4421 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_create_subscription_from_partner.py
--rw-rw-rw-   0 root         (0) root         (0)      837 2023-06-12 13:12:45.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_crm_lead_generate_SIM_delivery_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     1780 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_crm_lead_remesa_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     2911 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_crm_leads_validate_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_mail_compose_message_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     1648 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_partner_check_somoffice_email.py
--rw-rw-rw-   0 root         (0) root         (0)     7011 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_partner_email_change_wizard.py
--rw-rw-rw-   0 root         (0) root         (0)     4028 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_payment_order_generated_to_upload_queued_wizard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/account_asset_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     2886 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/account_invoice_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/account_move.xml
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/account_move_line.xml
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/account_payment_order_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      471 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/account_tax_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/act_account_move_to_account_move_line_open.xml
--rw-rw-rw-   0 root         (0) root         (0)     1347 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/adsl_service_contract_info_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/aeat_report_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     2690 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/broadband_isp_info_view.xml
--rw-rw-rw-   0 root         (0) root         (0)    25408 2023-06-12 12:44:50.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/contract_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1117 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/coop_agreement_view.xml
--rw-rw-rw-   0 root         (0) root         (0)    12099 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/crm_lead.xml
--rw-rw-rw-   0 root         (0) root         (0)    15207 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/crm_lead_line.xml
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/data_range_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1283 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/hr_attendance.xml
--rw-rw-rw-   0 root         (0) root         (0)      765 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/ir_action_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     9621 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/mail_activity_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/mail_mail_statistics_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      476 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/mass_mailing_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     3474 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/menus.xml
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/mis_budget_item_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/mm_fiber_service_contract_info.xml
--rw-rw-rw-   0 root         (0) root         (0)     1711 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/mobile_isp_info_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1009 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/mobile_service_contract_info_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/open_boards_activities.xml
--rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/operation_request.xml
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/orange_fiber_service_contract_info.xml
--rw-rw-rw-   0 root         (0) root         (0)     1042 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/partner_action_tag_views.xml
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/payment_return_import_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      743 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/payment_return_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/previous_provider_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/product_attribute_views.xml
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/product_category_technology_supplier_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/product_pricelist_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     2416 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/product_product_view.xml
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/product_template_view.xml
--rw-rw-rw-   0 root         (0) root         (0)     1199 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/res_company_view.xml
--rw-rw-rw-   0 root         (0) root         (0)    13562 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/res_partner_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/router_4G_service_contract_info.xml
--rw-rw-rw-   0 root         (0) root         (0)      781 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/service_technology_service_supplier.xml
--rw-rw-rw-   0 root         (0) root         (0)      637 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/stock_move_line_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/stock_production_lot.xml
--rw-rw-rw-   0 root         (0) root         (0)     6239 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/subscription_request_view.xml
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/templates_js.xml
--rw-rw-rw-   0 root         (0) root         (0)      640 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/vodafone_fiber_service_contract_info.xml
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/xoln_fiber_service_contract_info.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/
--rw-rw-rw-   0 root         (0) root         (0)     1170 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_financial_report/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_financial_report/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.xml
--rw-rw-rw-   0 root         (0) root         (0)     1658 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_invoice_confirm/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_invoice_confirm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_invoice_confirm/account_invoice_confirm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_payment_line_create/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_payment_line_create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2542 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create.py
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create_view.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_address_change/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_address_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8088 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.py
--rw-rw-rw-   0 root         (0) root         (0)     4084 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_compensation/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_compensation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5033 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.py
--rw-rw-rw-   0 root         (0) root         (0)     3492 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_force_oc_integration/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_force_oc_integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.py
--rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_holder_change/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_holder_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12025 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.py
--rw-rw-rw-   0 root         (0) root         (0)     3069 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_iban_change/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_iban_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3782 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.py
--rw-rw-rw-   0 root         (0) root         (0)     1939 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_iban_change_force/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_iban_change_force/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      643 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.py
--rw-rw-rw-   0 root         (0) root         (0)     1994 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_invoice_payment/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_invoice_payment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2088 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.py
--rw-rw-rw-   0 root         (0) root         (0)     1235 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4572 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py
--rw-rw-rw-   0 root         (0) root         (0)     2550 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_one_shot_request/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_one_shot_request/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4650 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2134 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_tariff_change/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_tariff_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5592 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.py
--rw-rw-rw-   0 root         (0) root         (0)     2684 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_terminate/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_terminate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/create_lead_from_partner/
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/create_lead_from_partner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11844 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py
--rw-rw-rw-   0 root         (0) root         (0)    10758 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/create_subscription_from_partner/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/create_subscription_from_partner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2193 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.py
--rw-rw-rw-   0 root         (0) root         (0)     1810 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      600 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.py
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/
--rw-rw-rw-   0 root         (0) root         (0)       48 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.py
--rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_remesa/
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_remesa/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1515 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.py
--rw-rw-rw-   0 root         (0) root         (0)     1070 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_leads_validate/
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_leads_validate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.py
--rw-rw-rw-   0 root         (0) root         (0)     1082 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/import_payment_group/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/import_payment_group/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      738 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.py
--rw-rw-rw-   0 root         (0) root         (0)     1093 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/invoice_claim_1_send/
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/invoice_claim_1_send/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.py
--rw-rw-rw-   0 root         (0) root         (0)      970 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/mail_compose_message/
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/mail_compose_message/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2234 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/mail_compose_message/mail_compose_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.py
--rw-rw-rw-   0 root         (0) root         (0)     1210 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/partner_email_change/
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/partner_email_change/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.py
--rw-rw-rw-   0 root         (0) root         (0)     3484 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/payment_order_confirm/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/payment_order_confirm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.py
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      887 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.py
--rw-rw-rw-   0 root         (0) root         (0)      938 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/product_publish/
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/product_publish/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1008 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/product_publish/product_publish.py
--rw-rw-rw-   0 root         (0) root         (0)     3253 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/product_publish/product_publish.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/test_mailing/
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/test_mailing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1964 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-12 10:56:18.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo12_addon_somconnexio.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4972 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo12_addon_somconnexio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    32533 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo12_addon_somconnexio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo12_addon_somconnexio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo12_addon_somconnexio.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     2998 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo12_addon_somconnexio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/odoo12_addon_somconnexio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 17:42:40.000000 odoo12-addon-somconnexio-12.0.2.2.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     5934 2023-06-12 13:12:45.000000 odoo12-addon-somconnexio-12.0.2.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/
+-rw-r--r--   0 root         (0) root         (0)     4972 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     4507 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9782 2023-06-19 11:48:33.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/__manifest__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/controllers/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/controllers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5170 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/controllers/controllers.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/controllers/http.py
+-rw-rw-rw-   0 root         (0) root         (0)     3458 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/controllers/public_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/correos_services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/correos_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4432 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/correos_services/shipment.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/
+-rw-rw-rw-   0 root         (0) root         (0)    46993 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account.account.template-sc.csv
+-rw-rw-rw-   0 root         (0) root         (0)      712 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account_chart_template_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2954 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account_group.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account_journal.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account_payment_mode.xml
+-rw-rw-rw-   0 root         (0) root         (0)     4496 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account_payment_term.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1730 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account_tax.xml
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account_tax_group.xml
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/analytic_account.xml
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/base_automation.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2241 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/company.xml
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/contract_compute_current_tariff_cron.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3786 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/contract_terminate_reason.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/contract_terminate_user_reason.xml
+-rw-rw-rw-   0 root         (0) root         (0)      947 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/crm_stage_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      658 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/crm_track_correos_delivery_cron.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/discovery_channel.xml
+-rw-rw-rw-   0 root         (0) root         (0)      752 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/fiber_signal_type_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      837 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/hr_attendance_place.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/ir_config_pararameter.xml
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/ir_sequence.xml
+-rw-rw-rw-   0 root         (0) root         (0)    13962 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/mail_activity_type.xml
+-rw-rw-rw-   0 root         (0) root         (0)      150 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/mail_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3266 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/mail_mass_mailing_list_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/mis_report.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/operation_request_terminate_reason.xml
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/partner_action_tag_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/partner_priority.xml
+-rw-rw-rw-   0 root         (0) root         (0)    13582 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/previous_provider_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1459 2023-06-19 09:35:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_attribute.xml
+-rw-rw-rw-   0 root         (0) root         (0)     7767 2023-06-19 09:35:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_attribute_value.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2455 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_categories.xml
+-rw-rw-rw-   0 root         (0) root         (0)     7830 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_category_technology_supplier_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)    11481 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_pack_line.xml
+-rw-rw-rw-   0 root         (0) root         (0)    41333 2023-06-19 09:35:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_product.xml
+-rw-rw-rw-   0 root         (0) root         (0)     5653 2023-06-19 09:35:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_template_attribute_line_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)    11160 2023-06-19 09:35:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_template_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/res.partner.bank.xml
+-rw-rw-rw-   0 root         (0) root         (0)      426 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/res.users.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3704 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/res_bank_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/service_supplier.xml
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/service_technology.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1908 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/service_technology_service_supplier.xml
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/share_type.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/demo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/demo/contract/
+-rw-rw-rw-   0 root         (0) root         (0)     2573 2023-06-19 10:08:38.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/demo/contract/contract.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2023-06-19 10:08:38.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/demo/contract/contract_pack.xml
+-rw-rw-rw-   0 root         (0) root         (0)     4018 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/demo/contract/contract_shared_data.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6655 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/demo/partner.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2749 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/demo/product.pricelist.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2346 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/demo/subscription_requests.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/helpers/date.py
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/helpers/language.py
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)   322385 2023-06-19 10:08:38.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/i18n/ca_ES.po
+-rw-rw-rw-   0 root         (0) root         (0)   331855 2023-06-19 10:08:38.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/i18n/es.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/listeners/
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/listeners/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/listeners/contract_line_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/listeners/contract_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/listeners/crm_lead_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)      742 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/listeners/partner_bank_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/listeners/partner_listener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.8/pre-clean-mail-tracking-value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.8.11/
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.8.11/post-create-copy-contract-service-info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.8.4/
+-rw-rw-rw-   0 root         (0) root         (0)     2709 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.8.4/post-create-copy-contract-service-info.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.8.4/pre-create-one-gb-wo-cost.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9/post-link-crm-to-contract.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9/post-migrate-change-address.py
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9/pre-migrate-change-address.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9/pre-uniform-contracts-wo-number.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9.13/
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9.13/post-change-activities-user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9.2/
+-rw-rw-rw-   0 root         (0) root         (0)      533 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9.2/post-upper-sponsorship-code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1886 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9.9/post-import-es-geonames.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-recompute-is-from-pack.py
+-rw-rw-rw-   0 root         (0) root         (0)      803 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-relate-is-from-not-pack-attribute-with-existing-products.py
+-rw-rw-rw-   0 root         (0) root         (0)     1260 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-create-is-from-pack-attribute.py
+-rw-rw-rw-   0 root         (0) root         (0)      575 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-set-xml-id-unlimited-20GB.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.1.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.1.6/post-set-state_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.1.8/
+-rw-rw-rw-   0 root         (0) root         (0)      242 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.1.8/pre-assign-imd-manual-created-activity-types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     2293 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.2.0/pre-fix-catalog-externalId.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/erppeek/
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/erppeek/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/erppeek/erppeek.ini
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/erppeek/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1043 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/erppeek/update_contract_line_product_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1838 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_asset.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_banking_mandate.py
+-rw-rw-rw-   0 root         (0) root         (0)     6377 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_invoice.py
+-rw-rw-rw-   0 root         (0) root         (0)     2367 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_invoice_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_journal.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_move.py
+-rw-rw-rw-   0 root         (0) root         (0)     3769 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_move_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_payment_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     1897 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_payment_return_email_gateway.py
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_tax.py
+-rw-rw-rw-   0 root         (0) root         (0)    21169 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/aged_partner_balance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7108 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/aged_partner_balance_xlsx.py
+-rw-rw-rw-   0 root         (0) root         (0)    40172 2023-06-19 10:08:38.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/contract.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/contract_info/
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/contract_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/contract_info/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3230 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/contract_info/broadband.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/contract_info/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/contract_terminate_reason.py
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/contract_terminate_user_reason.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/coop_agreement.py
+-rw-rw-rw-   0 root         (0) root         (0)    21856 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/crm_lead.py
+-rw-rw-rw-   0 root         (0) root         (0)    11230 2023-06-19 09:35:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      151 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/discovery_channel.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/fiber_signal_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/hr_attendance.py
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/hr_attendance_place.py
+-rw-rw-rw-   0 root         (0) root         (0)     3864 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/hr_employee.py
+-rw-rw-rw-   0 root         (0) root         (0)     4417 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/ir_model_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/ir_server_action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/isp_info/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/isp_info/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3680 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/isp_info/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3644 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/isp_info/broadband.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/isp_info/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/l10n_es_aeat_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     3881 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/mail_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/mail_thread.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/mass_mailing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/mobile_contract_otrs_view.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/opencell_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/operation_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/operation_request_terminate_reason.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/partner_action_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     2816 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/partner_otrs_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/payment_return.py
+-rw-rw-rw-   0 root         (0) root         (0)     3407 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/payment_return_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/previous_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/product_attribute_value.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/product_category_technology_supplier.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/product_pack_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/product_pricelist.py
+-rw-rw-rw-   0 root         (0) root         (0)     6021 2023-06-19 11:43:39.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/product_product.py
+-rw-rw-rw-   0 root         (0) root         (0)      640 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/product_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/res_company.py
+-rw-rw-rw-   0 root         (0) root         (0)    22511 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/res_partner_bank.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/service_supplier.py
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/service_technology.py
+-rw-rw-rw-   0 root         (0) root         (0)     2509 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/stock_move_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1818 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/stock_production_lot.py
+-rw-rw-rw-   0 root         (0) root         (0)    12471 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/subscription_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/utm_source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/access.py
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/account_hierarchy_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)     5121 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/crm_account_hierarchy.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/customer.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/opencell_resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/opencell_types/
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/opencell_types/address.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/opencell_types/custom_field.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/opencell_types/description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     2144 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2944 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_strategies.py
+-rw-rw-rw-   0 root         (0) root         (0)     3430 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5227 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_strategies.py
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/customer_update_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/opencell_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/subscription_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/adsl_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1152 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/base_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     2508 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/broadband_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/customer_data_from_res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2762 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/fiber_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1749 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/mobile_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/router_4G_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/service_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/update_ticket_with_error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/account_asset_report_xls.py
+-rw-rw-rw-   0 root         (0) root         (0)    20209 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/aged_partner_balance.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/crm_lead_creation_email_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/invoice_claim_1_capital_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1398 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/invoice_claim_1_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1969 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/mobile_can_be_linked_with_fiber_mail_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/mobile_linked_with_fiber_mail_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3799 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/new_sim_sending_letter_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)      720 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/report_paperformat.xml
+-rw-rw-rw-   0 root         (0) root         (0)     8425 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/sim_sending_letter_template.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/sponsor_sell_back_template.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/security/
+-rw-rw-rw-   0 root         (0) root         (0)     7111 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/security/ir.model.access.csv
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/security/res_groups.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5557 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/account_invoice_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      500 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/account_invoice_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3164 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/account_payment_group_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/bank_from_iban_getter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3602 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/change_partner_emails.py
+-rw-rw-rw-   0 root         (0) root         (0)     5468 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_change_tariff_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_change_tariff_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1657 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_contract_process.py
+-rw-rw-rw-   0 root         (0) root         (0)    11694 2023-06-19 10:08:38.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_contract_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3710 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_email_change_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_email_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_iban_change_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_iban_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2809 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_one_shot_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_one_shot_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/
+-rw-rw-rw-   0 root         (0) root         (0)      166 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/adsl.py
+-rw-rw-rw-   0 root         (0) root         (0)     1054 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/ba.py
+-rw-rw-rw-   0 root         (0) root         (0)    13757 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10896 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/fiber.py
+-rw-rw-rw-   0 root         (0) root         (0)     3378 2023-06-19 09:35:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/router4g.py
+-rw-rw-rw-   0 root         (0) root         (0)     8974 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/crm_lead_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/discovery_channel_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/get_activation_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/hashids_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/partner_email_change_process.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/partner_email_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     8806 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/product_catalog_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/provider_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5730 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/res_partner_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    22074 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/schemas.py
+-rw-rw-rw-   0 root         (0) root         (0)     5848 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/subscription_request_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/vat_normalizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/somoffice/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/somoffice/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/somoffice/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/somoffice/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/
+-rw-rw-rw-   0 root         (0) root         (0)     9682 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/activities.png
+-rw-rw-rw-   0 root         (0) root         (0)    12957 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/broadband_contract.png
+-rw-rw-rw-   0 root         (0) root         (0)    13548 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/broadband_lead_lines.png
+-rw-rw-rw-   0 root         (0) root         (0)     6550 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/emails.png
+-rw-rw-rw-   0 root         (0) root         (0)    15486 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/mobile_contract.png
+-rw-rw-rw-   0 root         (0) root         (0)    15574 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/mobile_lead_lines.png
+-rw-rw-rw-   0 root         (0) root         (0)    15844 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/packs.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)    17014 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/img/sc-image.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/js/
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/js/holidays_highlighter.js
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/js/many2many_tags_contract_email.js
+-rw-rw-rw-   0 root         (0) root         (0)      605 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/js/many2one_tags_crm_lead_email.js
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/js/my_attendances.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/xml/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/xml/activity.xml
+-rw-rw-rw-   0 root         (0) root         (0)      684 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/xml/attendance.xml
+-rw-rw-rw-   0 root         (0) root         (0)      287 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/xml/contract_email.xml
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/xml/mail_chatter_buttons.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4825 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/common_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/correos_services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/correos_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7677 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/correos_services/test_shipment.py
+-rw-rw-rw-   0 root         (0) root         (0)     3047 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     6988 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10823 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/test_contract_line_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     5866 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/test_contract_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     3485 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/test_crm_lead_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/test_partner_bank_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     7360 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/test_partner_listener.py
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/test_res_partner_listener.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_account_invoice.py
+-rw-rw-rw-   0 root         (0) root         (0)     3598 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_account_move_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     3854 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_account_payment_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     5342 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_account_payment_return_gateway.py
+-rw-rw-rw-   0 root         (0) root         (0)     4540 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_broadband_isp_info.py
+-rw-rw-rw-   0 root         (0) root         (0)    34365 2023-06-19 10:08:38.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_contract.py
+-rw-rw-rw-   0 root         (0) root         (0)     5657 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_coop_agreement.py
+-rw-rw-rw-   0 root         (0) root         (0)    85560 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_crm_lead.py
+-rw-rw-rw-   0 root         (0) root         (0)     9390 2023-06-19 09:35:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1646 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_hr_attendance_process.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_mail_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)     5484 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_mass_mailing.py
+-rw-rw-rw-   0 root         (0) root         (0)     6492 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_mobile_isp_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_opencell_configuration_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     9187 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_payment_return.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_previous_provider.py
+-rw-rw-rw-   0 root         (0) root         (0)    28217 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_product_category_technology_supplier.py
+-rw-rw-rw-   0 root         (0) root         (0)     2018 2023-06-19 11:43:39.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_product_product.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_product_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_production_lot.py
+-rw-rw-rw-   0 root         (0) root         (0)    46314 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_res_partner_bank.py
+-rw-rw-rw-   0 root         (0) root         (0)     5237 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_server_action.py
+-rw-rw-rw-   0 root         (0) root         (0)    10862 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_service_supplier.py
+-rw-rw-rw-   0 root         (0) root         (0)     4876 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_stock_move_line.py
+-rw-rw-rw-   0 root         (0) root         (0)    26854 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_subscription_request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_models/test_address.py
+-rw-rw-rw-   0 root         (0) root         (0)    11179 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_models/test_crm_account_hierarchy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_models/test_customer.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_models/test_description.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_models/test_opencell_service_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4105 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_models/test_subscription.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15080 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    10511 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_strategies.py
+-rw-rw-rw-   0 root         (0) root         (0)     6230 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    15234 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_strategies.py
+-rw-rw-rw-   0 root         (0) root         (0)     2335 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/test_customer_update_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7743 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/test_subscription_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5744 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/test_adsl_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/test_customer_data_from_res_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)    10739 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/test_fiber_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     6540 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/test_mobile_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     4644 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/test_router_4G_data_from_crm_lead_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1657 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/test_update_ticket_with_error.py
+-rw-rw-rw-   0 root         (0) root         (0)      925 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/sc_test_case.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_process/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_process/base_test_contract_process.py
+-rw-rw-rw-   0 root         (0) root         (0)    26941 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_process/test_fiber_contract_process.py
+-rw-rw-rw-   0 root         (0) root         (0)     9819 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_process/test_mobile_contract_process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_services/
+-rw-rw-rw-   0 root         (0) root         (0)    71869 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_contract_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     6613 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_count_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    19447 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_get_fiber_contracts_to_pack_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    27093 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_search_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    43501 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_account_invoice_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7531 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_change_partner_emails.py
+-rw-rw-rw-   0 root         (0) root         (0)    15498 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_contract_change_tariff_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2980 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_contract_contract_process.py
+-rw-rw-rw-   0 root         (0) root         (0)    12908 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_contract_email_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    13013 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_contract_iban_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_contract_one_shot_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    34346 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_crm_lead_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1769 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_discovery_channel_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1456 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_get_activation_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_hashids_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1501 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_mass_mailing_unsubscribe.py
+-rw-rw-rw-   0 root         (0) root         (0)     6003 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_partner_email_change_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    16699 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_product_catalog_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2141 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_provider_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    18948 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_res_partner_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     8798 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_subscription_request_service.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_vat_normalizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/somoffice/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/somoffice/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/somoffice/test_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-19 13:22:42.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9061 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_account_payment_line_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     9357 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_address_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     5722 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_compensation_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     2552 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_force_oc_integration_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    21666 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_holder_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     3581 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_force_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     4007 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     5504 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_invoice_payment_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    21108 2023-06-19 10:08:38.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_mobile_tariff_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    13855 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_one_shot_request_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    12968 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_tariff_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3322 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_terminate_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)    30774 2023-06-19 09:35:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_create_lead_from_partner_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     4421 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_create_subscription_from_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_crm_lead_generate_SIM_delivery_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_crm_lead_remesa_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     2911 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_crm_leads_validate_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_mail_compose_message_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     1648 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_partner_check_somoffice_email.py
+-rw-rw-rw-   0 root         (0) root         (0)     7011 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_partner_email_change_wizard.py
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_payment_order_generated_to_upload_queued_wizard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/
+-rw-rw-rw-   0 root         (0) root         (0)      595 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/account_asset_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/account_invoice_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/account_move.xml
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/account_move_line.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/account_payment_order_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      471 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/account_tax_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/act_account_move_to_account_move_line_open.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1347 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/adsl_service_contract_info_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/aeat_report_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2690 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/broadband_isp_info_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)    25408 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/contract_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/coop_agreement_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)    12099 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/crm_lead.xml
+-rw-rw-rw-   0 root         (0) root         (0)    15207 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/crm_lead_line.xml
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/data_range_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/hr_attendance.xml
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/ir_action_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     9621 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/mail_activity_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/mail_mail_statistics_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      476 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/mass_mailing_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/menus.xml
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/mis_budget_item_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/mm_fiber_service_contract_info.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/mobile_isp_info_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/mobile_service_contract_info_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/open_boards_activities.xml
+-rw-rw-rw-   0 root         (0) root         (0)      826 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/operation_request.xml
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/orange_fiber_service_contract_info.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1042 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/partner_action_tag_views.xml
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/payment_return_import_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      743 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/payment_return_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/previous_provider_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/product_attribute_views.xml
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/product_category_technology_supplier_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/product_pricelist_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     2416 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/product_product_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/product_template_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/res_company_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)    13562 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/res_partner_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/router_4G_service_contract_info.xml
+-rw-rw-rw-   0 root         (0) root         (0)      781 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/service_technology_service_supplier.xml
+-rw-rw-rw-   0 root         (0) root         (0)      637 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/stock_move_line_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/stock_production_lot.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6239 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/subscription_request_view.xml
+-rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/templates_js.xml
+-rw-rw-rw-   0 root         (0) root         (0)      640 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/vodafone_fiber_service_contract_info.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/xoln_fiber_service_contract_info.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/
+-rw-rw-rw-   0 root         (0) root         (0)     1170 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_financial_report/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_financial_report/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.py
+-rw-rw-rw-   0 root         (0) root         (0)      568 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1658 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_invoice_confirm/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_invoice_confirm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_invoice_confirm/account_invoice_confirm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_payment_line_create/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_payment_line_create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2542 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create_view.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_address_change/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_address_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8088 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     4084 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_compensation/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_compensation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5033 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3492 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_force_oc_integration/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_force_oc_integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1683 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_holder_change/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_holder_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12025 2023-06-19 09:35:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     3069 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_iban_change/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_iban_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3782 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     1939 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_iban_change_force/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_iban_change_force/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      643 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.py
+-rw-rw-rw-   0 root         (0) root         (0)     1994 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_invoice_payment/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_invoice_payment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2088 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1235 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14915 2023-06-19 10:08:38.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-06-19 10:08:38.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_one_shot_request/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_one_shot_request/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4650 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2134 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_tariff_change/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_tariff_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5592 2023-06-19 09:35:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     2684 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_terminate/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_terminate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/create_lead_from_partner/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/create_lead_from_partner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11844 2023-06-19 09:35:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)    10758 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/create_subscription_from_partner/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/create_subscription_from_partner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2193 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1810 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      600 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.py
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.py
+-rw-rw-rw-   0 root         (0) root         (0)     1083 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_remesa/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_remesa/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1515 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.py
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_leads_validate/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_leads_validate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1082 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/import_payment_group/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/import_payment_group/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1093 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/invoice_claim_1_send/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/invoice_claim_1_send/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.py
+-rw-rw-rw-   0 root         (0) root         (0)      970 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/mail_compose_message/
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/mail_compose_message/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/mail_compose_message/mail_compose_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.py
+-rw-rw-rw-   0 root         (0) root         (0)     1210 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/partner_email_change/
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/partner_email_change/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.py
+-rw-rw-rw-   0 root         (0) root         (0)     3484 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/payment_order_confirm/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/payment_order_confirm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      283 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.py
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      887 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.py
+-rw-rw-rw-   0 root         (0) root         (0)      938 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/product_publish/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/product_publish/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/product_publish/product_publish.py
+-rw-rw-rw-   0 root         (0) root         (0)     3253 2023-06-19 09:35:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/product_publish/product_publish.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/test_mailing/
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/test_mailing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1964 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2023-06-16 15:05:37.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo12_addon_somconnexio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4972 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo12_addon_somconnexio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    32711 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo12_addon_somconnexio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo12_addon_somconnexio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo12_addon_somconnexio.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo12_addon_somconnexio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/odoo12_addon_somconnexio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 13:23:23.000000 odoo12-addon-somconnexio-12.0.2.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     5934 2023-06-19 10:08:38.000000 odoo12-addon-somconnexio-12.0.2.3.0/setup.py
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/PKG-INFO` & `odoo12-addon-somconnexio-12.0.2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-somconnexio
-Version: 12.0.2.2.2
+Version: 12.0.2.3.0
 Summary: Odoo Som Connexió customizations
 Home-page: https://coopdevs.org
 Author: Coopdevs Treball SCCL
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/README.md` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/README.md`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/__manifest__.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/__manifest__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 {
     "name": "Odoo Som Connexió customizations",
-    "version": "12.0.2.2.2",
+    "version": "12.0.2.3.0",
     "depends": [
         "account_asset_management",
         "account_banking_sepa_credit_transfer",
         "account_banking_sepa_direct_debit",
         "account_cancel",
         "account_chart_update",
         "account_due_list",
@@ -222,16 +222,19 @@
         "wizards/test_mailing/test_mailing.xml",
         "views/mass_mailing_view.xml",
         "views/mail_mail_statistics_view.xml",
         "data/product_pack_line.xml",
     ],
     "demo": [
         "demo/partner.xml",
-        "demo/pricelist.xml",
+        "demo/product.pricelist.csv",
         "demo/subscription_requests.xml",
+        "demo/contract/contract.xml",
+        "demo/contract/contract_pack.xml",
+        "demo/contract/contract_shared_data.xml",
     ],
     "qweb": [
         "static/src/xml/activity.xml",
         "static/src/xml/attendance.xml",
         "static/src/xml/contract_email.xml",
         "static/src/xml/mail_chatter_buttons.xml",
     ],
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/controllers/controllers.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/controllers/controllers.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/controllers/http.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/controllers/http.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/controllers/public_controller.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/controllers/public_controller.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/correos_services/shipment.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/correos_services/shipment.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account.account.template-sc.csv` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account.account.template-sc.csv`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account_chart_template_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account_chart_template_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account_group.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account_group.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account_journal.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account_journal.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account_payment_mode.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account_payment_mode.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account_payment_term.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account_payment_term.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/account_tax.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/account_tax.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/analytic_account.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/analytic_account.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/base_automation.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/base_automation.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/company.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/company.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/contract_compute_current_tariff_cron.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/contract_compute_current_tariff_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/contract_terminate_reason.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/contract_terminate_reason.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/contract_terminate_user_reason.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/contract_terminate_user_reason.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/crm_stage_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/crm_stage_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/crm_track_correos_delivery_cron.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/crm_track_correos_delivery_cron.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/discovery_channel.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/discovery_channel.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/fiber_signal_type_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/fiber_signal_type_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/hr_attendance_place.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/hr_attendance_place.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/ir_config_pararameter.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/ir_config_pararameter.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/ir_sequence.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/ir_sequence.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/mail_activity_type.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/mail_activity_type.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/mail_mass_mailing_list_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/mail_mass_mailing_list_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/mis_report.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/mis_report.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/operation_request_terminate_reason.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/operation_request_terminate_reason.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/partner_action_tag_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/partner_action_tag_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/partner_priority.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/partner_priority.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/previous_provider_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/previous_provider_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_attribute.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_attribute.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_attribute_value.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_attribute_value.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_categories.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_categories.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_category_technology_supplier_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_category_technology_supplier_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_pack_line.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_pack_line.xml`

 * *Files 4% similar despite different names*

#### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_pack_line.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_pack_line.xml`

```diff
@@ -7,14 +7,25 @@
     <field name="quantity" eval="1.0"/>
   </record>
   <record id="PackFibra100MbIL20GB_components_mobile" model="product.pack.line">
     <field name="parent_product_id" ref="PackFibra100MbIL20GB"/>
     <field name="product_id" ref="TrucadesIllimitades20GBPack"/>
     <field name="quantity" eval="1.0"/>
   </record>
+  <!-- Pack 300Mb + Il 20GB -->
+  <record id="PackFibra300MbIL20GB_components_fibra" model="product.pack.line">
+    <field name="parent_product_id" ref="PackFibra300MbIL20GB"/>
+    <field name="product_id" ref="Fibra300Mb"/>
+    <field name="quantity" eval="1.0"/>
+  </record>
+  <record id="PackFibra300MbIL20GB_components_mobile" model="product.pack.line">
+    <field name="parent_product_id" ref="PackFibra300MbIL20GB"/>
+    <field name="product_id" ref="TrucadesIllimitades20GBPack"/>
+    <field name="quantity" eval="1.0"/>
+  </record>
   <!-- Pack 600Mb + 2 Il 20GB -->
   <record id="PackFibra600MbIL20GB_components_fibra" model="product.pack.line">
     <field name="parent_product_id" ref="PackFibra600MbIL20GB"/>
     <field name="product_id" ref="Fibra600Mb"/>
     <field name="quantity" eval="1.0"/>
   </record>
   <record id="PackFibra600MbIL20GB_components_mobile" model="product.pack.line">
@@ -40,14 +51,25 @@
     <field name="quantity" eval="1.0"/>
   </record>
   <record id="PackSenseFixFibra100MbIL20GB_components_mobile" model="product.pack.line">
     <field name="parent_product_id" ref="PackSenseFixFibra100MbIL20GB"/>
     <field name="product_id" ref="TrucadesIllimitades20GBPack"/>
     <field name="quantity" eval="1.0"/>
   </record>
+  <!-- Pack 300Mb sense fix + 2 Il 20GB -->
+  <record id="PackSenseFixFibra300MbIL20GB_components_fibra" model="product.pack.line">
+    <field name="parent_product_id" ref="PackSenseFixFibra300MbIL20GB"/>
+    <field name="product_id" ref="SenseFixFibra300Mb"/>
+    <field name="quantity" eval="1.0"/>
+  </record>
+  <record id="PackSenseFixFibra300MbIL20GB_components_mobile" model="product.pack.line">
+    <field name="parent_product_id" ref="PackSenseFixFibra300MbIL20GB"/>
+    <field name="product_id" ref="TrucadesIllimitades20GBPack"/>
+    <field name="quantity" eval="1.0"/>
+  </record>
   <!-- Compartides 300Mb + 50GB compartides 2 mobils -->
   <record id="CompartidesFibra300Mb2mobils_components_fibra" model="product.pack.line">
     <field name="parent_product_id" ref="CompartidesFibra300Mb2mobils"/>
     <field name="product_id" ref="Fibra300Mb"/>
     <field name="quantity" eval="1.0"/>
   </record>
   <record id="CompartidesFibra300Mb2mobils_components_mobile1" model="product.pack.line">
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_product.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_product.xml`

 * *Files 1% similar despite different names*

#### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_product.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_product.xml`

```diff
@@ -637,14 +637,20 @@
     <!-- Pack -->
     <record id="PackFibra100MbIL20GB" model="product.product">
       <field name="name">Fibra 100 Mb + mòbil IL 20 GB</field>
       <field name="custom_name">Fibra 100 Mb + mòbil IL 20 GB</field>
       <field name="default_code">SE_SC_REC_PACK_FIBER_100_UNL_20480</field>
       <field name="pack_ok">True</field>
     </record>
+    <record id="PackFibra300MbIL20GB" model="product.product">
+      <field name="name">Fibra 300 Mb + mòbil IL 20 GB</field>
+      <field name="custom_name">Fibra 300 Mb + mòbil IL 20 GB</field>
+      <field name="default_code">SE_SC_REC_PACK_FIBER_300_UNL_20480</field>
+      <field name="pack_ok">True</field>
+    </record>
     <record id="PackFibra600MbIL20GB" model="product.product">
       <field name="name">Fibra 600 Mb + mòbil IL 20 GB</field>
       <field name="custom_name">Fibra 600 Mb + mòbil IL 20 GB</field>
       <field name="default_code">SE_SC_REC_PACK_FIBER_600_UNL_20480</field>
       <field name="pack_ok">True</field>
     </record>
     <record id="PackFibra1GbIL20GB" model="product.product">
@@ -655,14 +661,20 @@
     </record>
     <record id="PackSenseFixFibra100MbIL20GB" model="product.product">
       <field name="name">Fibra 100Mb Sense Fix + mòbil IL 20 GB</field>
       <field name="custom_name">Fibra 100Mb Sense Fix + mòbil IL 20 GB</field>
       <field name="default_code">SE_SC_REC_PACK_FIBER_100_SF_UNL_20480</field>
       <field name="pack_ok">True</field>
     </record>
+    <record id="PackSenseFixFibra300MbIL20GB" model="product.product">
+      <field name="name">Fibra 300Mb Sense Fix + mòbil IL 20 GB</field>
+      <field name="custom_name">Fibra 300Mb Sense Fix + mòbil IL 20 GB</field>
+      <field name="default_code">SE_SC_REC_PACK_FIBER_300_SF_UNL_20480</field>
+      <field name="pack_ok">True</field>
+    </record>
     <!-- Compartides -->
     <!-- Compartides 300Mb -->
     <record id="CompartidesFibra300Mb2mobils" model="product.product">
       <field name="name">Fibra 300Mb + Fix + 50 GB compartides 2 mòbils</field>
       <field name="custom_name">Fibra 300Mb + Fix + 50 GB compartides 2 mòbils</field>
       <field name="default_code">SE_SC_REC_PACK_FIBER_300_2_MOBILES_50</field>
       <field name="pack_ok">True</field>
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_template_attribute_line_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_template_attribute_line_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/product_template_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/product_template_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/res_bank_data.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/res_bank_data.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/service_supplier.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/service_supplier.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/service_technology.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/service_technology.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/service_technology_service_supplier.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/service_technology_service_supplier.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/data/share_type.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/data/share_type.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/demo/partner.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/demo/partner.xml`

 * *Files 1% similar despite different names*

#### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/demo/partner.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/demo/partner.xml`

```diff
@@ -14,14 +14,21 @@
     <field name="zip">17855</field>
     <field name="lang">es_ES</field>
     <field name="cooperator_register_number">855</field>
     <field name="member" eval="True"/>
     <field name="country_id" ref="base.es"/>
     <field name="state_id" ref="base.state_es_gi"/>
   </record>
+  <record id="demo_bank_id_partner_1_demo" model="res.partner.bank">
+    <field name="acc_number">ES71 0030 2053 0912 3456 7895</field>
+    <field name="sanitized_acc_number">ES7100302053091234567895</field>
+    <field name="acc_holder_name">Felip</field>
+    <field name="partner_id" ref="somconnexio.res_partner_1_demo"/>
+    <field name="bank_id">1</field>
+  </record>
   <record id="res_partner_2_demo" model="res.partner">
     <field name="name">Sara Merna</field>
     <field name="firstname">Sara</field>
     <field name="lastname">Merna</field>
     <field name="customer" eval="True"/>
     <field name="is_company" eval="False"/>
     <field name="email">sara.merna@demo.net</field>
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/demo/subscription_requests.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/demo/subscription_requests.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/hooks.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/hooks.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/i18n/ca_ES.po` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/i18n/ca_ES.po`

 * *Files 1% similar despite different names*

```diff
@@ -625,14 +625,19 @@
 msgstr "Missatges del lloc web"
 
 #. module: contract
 #: model:ir.model.fields,help:contract.field_contract_contract__website_message_ids
 msgid "Website communication history"
 msgstr "Historial de comunicacions del lloc web"
 
+#. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__mobile_contracts_to_share_with
+msgid "With which mobile contracts should it share data with?"
+msgstr "Amb quins mòbils vol compartir les dades?"
+
 #. module: contract
 #: model_terms:ir.ui.view,arch_db:contract.view_res_partner_filter
 msgid "With running contracts"
 msgstr "Amb contractes vigents"
 
 #. module: contract
 #: model_terms:ir.ui.view,arch_db:contract.contract_contract_form_view
@@ -1474,14 +1479,24 @@
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__shared_bond_id
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__shared_bond_id
 msgid "Shared bond ID"
 msgstr "ID abonament compartit"
 
+#. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__shared_bond_id_to_join
+msgid "Shared bond id to join option"
+msgstr "A quin abonament compartit la volem afegir?"
+
+#. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__sharing_data_options
+msgid "Sharing bond option"
+msgstr "Opcions per compartir dades mòbils"
+
 #. module: easy_my_coop
 #: model:ir.model.fields,field_description:easy_my_coop.field_subscription_request__skip_control_ng
 msgid "Skip control"
 msgstr "Passar els controls"
 
 #. module: easy_my_coop
 #: model:ir.model.fields,field_description:easy_my_coop.field_operation_request__state
@@ -2395,14 +2410,20 @@
 #: code:addons/somconnexio/models/res_partner.py:260
 #: code:addons/somconnexio/models/subscription_request.py:209
 #, python-format
 msgid "A partner with VAT %s already exists in our system"
 msgstr "Ja existeix un contacte amb VAT %s al sistema."
 
 #. module: somconnexio
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:309
+#, python-format
+msgid "A new shared bond creation cannot be an exceptional change"
+msgstr "Un canvi de tarifa per crear un abonament de compartides no pot ser excepcional"
+
+#. module: somconnexio
 #: selection:broadband.isp.info,previous_service:0
 msgid "ADSL"
 msgstr "ADSL"
 
 #. module: somconnexio
 #: model:product.product,name:somconnexio.ADSL20MB1000MinFix
 #: model:product.product,name:somconnexio.ADSL20MB100MinFixMobile
@@ -2498,14 +2519,21 @@
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_contract_one_shot_request_wizard
 msgid "Add"
 msgstr "Afegir"
 
 #. module: somconnexio
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:149
+#: model:shared.bond.type,name:somconnexio.existing_shared_bond
+#, python-format
+msgid "Add line to existing shared bond"
+msgstr "Afegir línia mòbil a un abonament existent"
+
+#. module: somconnexio
 #: model:ir.actions.act_window,name:somconnexio.move_line_add_to_payment_debit_order_action
 msgid "Add to Payment/Debit Order"
 msgstr "Afegiu a ordre de pagament/cobrament"
 
 #. module: somconnexio
 #: code:addons/somconnexio/listeners/contract_line_listener.py:47
 #, python-format
@@ -3251,14 +3279,21 @@
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_partner_form_lead_creation_wizard_button
 msgid "Create Lead"
 msgstr "Obrir petició de servei manualment"
 
 #. module: somconnexio
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:148
+#: model:shared.bond.type,name:somconnexio.new_shared_bond
+#, python-format
+msgid "Create new shared bond"
+msgstr "Crear un nou abonament"
+
+#. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.move_line_add_to_payment_debit_order_form
 msgid "Create Payment Lines"
 msgstr "Crea línies de pagament"
 
 #. module: somconnexio
 #: model:ir.model,name:somconnexio.model_move_line_add_to_payment_debit_order
 msgid "Create payment lines from account move line tree view"
@@ -4587,14 +4622,20 @@
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_res_company__max_sponsees_number
 msgid "Max Sponsees Number"
 msgstr "Número màxim d'apadrinats"
 
 #. module: somconnexio
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:265
+#, python-format
+msgid "Maximum 3 mobile contracts to build a shared data bond""
+msgstr "Només pots escollir tres mòbils per compartir dades"
+
+#. module: somconnexio
 #: code:addons/somconnexio/models/res_partner.py:459
 #, python-format
 msgid "Maximum number of sponsees exceeded"
 msgstr "Número màxim d'apadrinats excedit"
 
 #. module: somconnexio
 #: model:product.attribute,name:somconnexio.Min
@@ -6225,14 +6266,15 @@
 #. module: somconnexio
 #: model:mail.activity.type,name:somconnexio.mail_activity_type_take_out_fix
 msgid "Take Out Fix"
 msgstr "Treure fix"
 
 #. module: somconnexio
 #: code:addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.py:68
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:141
 #, python-format
 msgid "Tariff change"
 msgstr "Canvi tarifa"
 
 #. module: somconnexio
 #: model:mail.activity.type,name:somconnexio.mail_activity_type_tariff_change
 msgid "Tarrif Change"
@@ -6423,14 +6465,19 @@
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__broadband_ticket_number
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__mobile_1_ticket_number
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__ticket_number
 msgid "Ticket Number"
 msgstr "Número de tiquet"
 
 #. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__fiber_contract_to_link
+msgid "To which fiber contract should be linked?"
+msgstr "A quin contracte de fibra els volem vincular?"
+
+#. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__tree_view_notes
 msgid "Tree View Notes"
 msgstr "Notes"
 
 #. module: somconnexio
 #: model:mis.report,name:somconnexio.mis_report_trial_balance
 msgid "Trial balance"
@@ -6828,15 +6875,15 @@
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_res_partner__volunteer
 #: model:ir.model.fields,field_description:somconnexio.field_res_users__volunteer
 msgid "Volunteer"
 msgstr "Voluntari"
 
 #. module: somconnexio
-#: code:addons/somconnexio/models/stock_move_line.py:58
+#: code:addons/somconnexio/models/stock_move_line.py:5
 #, python-format
 msgid "Warning"
 msgstr "Alerta"
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.crm_lead_line_search_view
 #: model_terms:ir.ui.view,arch_db:somconnexio.crm_lead_pack_search_view
@@ -6861,15 +6908,16 @@
 
 #. module: somconnexio
 #: model:discovery.channel,name:somconnexio.social_networks
 msgid "Xarxes socials (Facebook, Twitter, Instagram, Linkedin, etc)"
 msgstr "Xarxes socials (Facebook, Twitter, Instagram, Linkedin, etc)"
 
 #. module: somconnexio
-#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:24
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:20
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:39
 #: code:addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py:99
 #: code:addons/somconnexio/wizards/partner_email_change/partner_email_change.py:11
 #: selection:contract.holder.change.wizard,has_mobile_pack_offer_text:0
 #: selection:partner.create.lead.wizard,has_mobile_pack_offer_text:0
 #: selection:partner.email.change.wizard,change_contact_email:0
 #: selection:partner.email.change.wizard,change_contracts_emails:0
 #: selection:partner.email.change.wizard,change_somoffice_email:0
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/i18n/es.po` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/i18n/es.po`

 * *Files 0% similar despite different names*

```diff
@@ -618,14 +618,19 @@
 msgstr "Mensajes del sitio web"
 
 #. module: contract
 #: model:ir.model.fields,help:contract.field_contract_contract__website_message_ids
 msgid "Website communication history"
 msgstr "Historial de comunicación del sitio web"
 
+#. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__mobile_contracts_to_share_with
+msgid "With which mobile contracts should it share data with?"
+msgstr "Con qué móviles quiere compartir los datos?"
+
 #. module: contract
 #: model_terms:ir.ui.view,arch_db:contract.view_res_partner_filter
 msgid "With running contracts"
 msgstr "Con contratos vigentes"
 
 #. module: contract
 #: model_terms:ir.ui.view,arch_db:contract.contract_contract_form_view
@@ -2420,14 +2425,20 @@
 #: code:addons/somconnexio/models/res_partner.py:260
 #: code:addons/somconnexio/models/subscription_request.py:209
 #, python-format
 msgid "A partner with VAT %s already exists in our system"
 msgstr "Ya existe un contacto con VAT %s en el sistema"
 
 #. module: somconnexio
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:309
+#, python-format
+msgid "A new shared bond creation cannot be an exceptional change"
+msgstr "Un cambio de tarifa para un nuevo bono compartido no puede ser excepcional"
+
+#. module: somconnexio
 #: selection:broadband.isp.info,previous_service:0
 msgid "ADSL"
 msgstr ""
 
 #. module: somconnexio
 #: model:product.product,custom_name:somconnexio.ADSL20MB100MinFixMobile
 #: model:product.product,showed_name:somconnexio.ADSL20MB100MinFixMobile
@@ -2537,14 +2548,21 @@
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.view_form_contract_one_shot_request_wizard
 msgid "Add"
 msgstr "Añadir"
 
 #. module: somconnexio
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:149
+#: model:shared.bond.type,name:somconnexio.existing_shared_bond
+#, python-format
+msgid "Add line to existing shared bond"
+msgstr "Añadir línia móvil a un bono existente"
+
+#. module: somconnexio
 #: model:ir.actions.act_window,name:somconnexio.move_line_add_to_payment_debit_order_action
 msgid "Add to Payment/Debit Order"
 msgstr "Añadir a orden de pago/cobro"
 
 #. module: somconnexio
 #: code:addons/somconnexio/listeners/contract_line_listener.py:47
 #, python-format
@@ -3304,14 +3322,21 @@
 
 #. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.move_line_add_to_payment_debit_order_form
 msgid "Create Payment Lines"
 msgstr "Crear líneas de pago"
 
 #. module: somconnexio
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:148
+#: model:shared.bond.type,name:somconnexio.new_shared_bond
+#, python-format
+msgid "Create new shared bond"
+msgstr "Crear un bono nuevo"
+
+#. module: somconnexio
 #: model:ir.model,name:somconnexio.model_move_line_add_to_payment_debit_order
 msgid "Create payment lines from account move line tree view"
 msgstr "Crear línieas de pago de la lista formulario de apuntes contables"
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_adsl_service_contract_info__create_uid
 #: model:ir.model.fields,field_description:somconnexio.field_broadband_isp_info__create_uid
@@ -4751,14 +4776,20 @@
 
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_res_company__max_sponsees_number
 msgid "Max Sponsees Number"
 msgstr "Número máximo de apadrinados"
 
 #. module: somconnexio
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:265
+#, python-format
+msgid "Maximum 3 mobile contracts to build a shared data bond"
+msgstr "Sólo puedes escoger tres móviles para compartir datos"
+
+#. module: somconnexio
 #: code:addons/somconnexio/models/res_partner.py:459
 #, python-format
 msgid "Maximum number of sponsees exceeded"
 msgstr "Número máximo de apadrinados excedido"
 
 #. module: somconnexio
 #: model:product.attribute,name:somconnexio.Min
@@ -6247,14 +6278,24 @@
 #. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_isp_info__shared_bond_id
 #: model:ir.model.fields,field_description:somconnexio.field_mobile_service_contract_info__shared_bond_id
 msgid "Shared bond ID"
 msgstr "ID bono compartido"
 
 #. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__shared_bond_id_to_join
+msgid "Shared bond id to join option"
+msgstr "A qué bono compartido la queremos añadir?"
+
+#. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__sharing_data_options
+msgid "Sharing bond option"
+msgstr "Opciones per compartir datos móviles"
+
+#. module: somconnexio
 #: model_terms:ir.ui.view,arch_db:somconnexio.sim_sending_letter_lang_template
 msgid "Si tens qualsevol dubte, posa’t en contacte amb l’equip de treball... ens fa molta il·lusió atendre’t,<br/><br/>\n"
 "                    <strong>Telèfon</strong>:<br/><br/>\n"
 "                    93 131 17 28 (de dilluns a divendres de 10h a 14h)<br/>\n"
 "                    693 761 723 (només per urgències, de 9h a 21h, tots els dies de la setmana)<br/><br/>\n"
 "                    Si tens una urgència fora d’aquest horari, envia un correu electrònic amb la paraula URGENT a l’assumpte, a:<br/>"
 msgstr "Si tienes cualquier duda, ponte en contacto con el equipo de trabajo, nos ilusiona atenderte,<br/><br/>\n"
@@ -6422,14 +6463,15 @@
 #: model:product.product,custom_name:somconnexio.EnviamentSIM
 #: model:product.product,showed_name:somconnexio.EnviamentSIM
 msgid "Targeta SIM amb enviament ordinari (2,05€ IVA inclòs)"
 msgstr "Tarjeta SIM con envío ordinario (2,05€ IVA incluido)"
 
 #. module: somconnexio
 #: code:addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.py:68
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:141
 #, python-format
 msgid "Tariff change"
 msgstr "Cambio de tarifa"
 
 #. module: somconnexio
 #: model:mail.activity.type,name:somconnexio.mail_activity_type_tariff_change
 msgid "Tarrif Change"
@@ -6619,14 +6661,19 @@
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__broadband_ticket_number
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead__mobile_1_ticket_number
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__ticket_number
 msgid "Ticket Number"
 msgstr "Número de tíquet"
 
 #. module: somconnexio
+#: model:ir.model.fields,field_description:somconnexio.field_contract_mobile_tariff_change_wizard__fiber_contract_to_link
+msgid "To which fiber contract should be linked?"
+msgstr "Con qué contrato de fibra los queremos vincular?"
+
+#. module: somconnexio
 #: model:ir.model.fields,field_description:somconnexio.field_crm_lead_line__tree_view_notes
 msgid "Tree View Notes"
 msgstr "Notas"
 
 #. module: somconnexio
 #: model:mis.report,name:somconnexio.mis_report_trial_balance
 msgid "Trial balance"
@@ -7061,15 +7108,16 @@
 
 #. module: somconnexio
 #: model:discovery.channel,name:somconnexio.social_networks
 msgid "Xarxes socials (Facebook, Twitter, Instagram, Linkedin, etc)"
 msgstr "Redes Sociales (Facebook, Twitter, Instagram, Linkedin, etc)"
 
 #. module: somconnexio
-#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:24
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:20
+#: code:addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py:39
 #: code:addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py:99
 #: code:addons/somconnexio/wizards/partner_email_change/partner_email_change.py:11
 #: selection:contract.holder.change.wizard,has_mobile_pack_offer_text:0
 #: selection:partner.create.lead.wizard,has_mobile_pack_offer_text:0
 #: selection:partner.email.change.wizard,change_contact_email:0
 #: selection:partner.email.change.wizard,change_contracts_emails:0
 #, python-format
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/listeners/contract_line_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/listeners/contract_line_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/listeners/contract_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/listeners/contract_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/listeners/crm_lead_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/listeners/crm_lead_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/listeners/partner_bank_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/listeners/partner_bank_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/listeners/partner_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/listeners/partner_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.8.4/post-create-copy-contract-service-info.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.8.4/post-create-copy-contract-service-info.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.8.4/pre-create-one-gb-wo-cost.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.8.4/pre-create-one-gb-wo-cost.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9/post-link-crm-to-contract.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9/post-link-crm-to-contract.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9/pre-migrate-change-address.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9/pre-migrate-change-address.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9/pre-uniform-contracts-wo-number.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9/pre-uniform-contracts-wo-number.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9.13/post-change-activities-user.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9.13/post-change-activities-user.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9.2/post-upper-sponsorship-code.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9.2/post-upper-sponsorship-code.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.1.9.9/post-import-es-geonames.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.1.9.9/post-import-es-geonames.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-relate-is-from-not-pack-attribute-with-existing-products.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/post-relate-is-from-not-pack-attribute-with-existing-products.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-create-is-from-pack-attribute.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-create-is-from-pack-attribute.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-set-xml-id-unlimited-20GB.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.0.0/pre-set-xml-id-unlimited-20GB.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.1.6/post-set-state_id.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.1.6/post-set-state_id.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/12.0.2.2.0/pre-fix-catalog-externalId.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/12.0.2.2.0/pre-fix-catalog-externalId.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/erppeek/README.md` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/erppeek/README.md`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/migrations/erppeek/update_contract_line_product_id.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/migrations/erppeek/update_contract_line_product_id.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/__init__.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_asset.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_asset.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_banking_mandate.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_banking_mandate.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_invoice.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_invoice.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_invoice_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_invoice_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_move_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_move_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_payment_order.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_payment_order.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/account_payment_return_email_gateway.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/account_payment_return_email_gateway.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/aged_partner_balance.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/aged_partner_balance.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/aged_partner_balance_xlsx.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/aged_partner_balance_xlsx.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/contract.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,35 @@
 
 class Contract(models.Model):
     _inherit = 'contract.contract'
 
     def _get_default_journal(self):
         return self.env.ref('somconnexio.consumption_invoices_journal')
 
+    def name_get(self):
+        res = []
+        for contract in self:
+            if contract.is_broadband:
+                address = (
+                    contract.service_partner_id
+                    if contract.service_partner_id
+                    else contract.partner_id
+                )
+                name = "{} - {}, {}, {}, {}".format(
+                    contract.name,
+                    address.full_street,
+                    address.city,
+                    address.zip,
+                    address.state_id.name,
+                )
+                res.append((contract.id, name))
+            else:
+                res.append((contract.id, contract.name))
+        return res
+
     name = fields.Char(compute='_compute_name', store=True, readonly=True)
     service_technology_id = fields.Many2one(
         'service.technology',
         'Service Technology',
         required=True,
     )
     service_supplier_id = fields.Many2one(
@@ -339,14 +360,15 @@
             self.env.cr.execute(
                 "DELETE FROM sharing_data_contracts WHERE id = %s or contract_id = %s",
                 (contract.id, contract.id)
             )
             if contract.shared_bond_id:
                 contracts_with_shared_bond = (
                     self.env["contract.contract"].search([
+                        ("partner_id", "=", contract.partner_id.id),
                         ("is_terminated", "=", False),
                         (
                             "service_technology_id",
                             "=",
                             self.env.ref("somconnexio.service_technology_mobile").id,
                         ),
                         ("shared_bond_id", "=", contract.shared_bond_id),
@@ -577,18 +599,19 @@
             elif contract_type == 'router4G':
                 record.router_4G_service_contract_info_id.icc = (
                     record.icc
                 )
 
     @api.depends('phone_number')
     def _compute_name(self):
-        self.name = self.phone_number
+        for contract in self:
+            contract.name = contract.phone_number
 
-        if not self.name and self.service_contract_type == "router4G":
-            self.name = self.router_4G_service_contract_info_id.name
+            if not contract.name and contract.service_contract_type == "router4G":
+                contract.name = contract.router_4G_service_contract_info_id.name
 
     @api.onchange('service_supplier_id')
     def onchange_service_supplier_id(self):
         coaxial = self.env.ref('somconnexio.coaxial_fiber_signal')
         ftth = self.env.ref('somconnexio.FTTH_fiber_signal')
         neba_ftth = self.env.ref('somconnexio.FTTH_neba_fiber_signal')
         indirect = self.env.ref('somconnexio.indirect_fiber_signal')
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/contract_info/base.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/contract_info/base.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/contract_info/broadband.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/contract_info/broadband.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/contract_info/mobile.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/contract_info/mobile.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/coop_agreement.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/coop_agreement.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/crm_lead.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/crm_lead.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/hr_employee.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/hr_employee.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/ir_model_data.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/ir_model_data.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/ir_server_action.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/ir_server_action.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/isp_info/base.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/isp_info/base.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/isp_info/broadband.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/isp_info/broadband.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/isp_info/mobile.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/isp_info/mobile.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/l10n_es_aeat_report.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/l10n_es_aeat_report.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/mail_activity.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/mail_activity.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/mass_mailing.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/mass_mailing.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/mobile_contract_otrs_view.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/mobile_contract_otrs_view.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/opencell_configuration.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/opencell_configuration.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/partner_action_tag.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/partner_action_tag.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/partner_otrs_view.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/partner_otrs_view.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/payment_return.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/payment_return.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/payment_return_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/payment_return_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/product_product.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/product_product.py`

 * *Files 9% similar despite different names*

```diff
@@ -132,27 +132,36 @@
 
     def get_offer(self):
         """
         Return the same product but the one with offer.
         Ex. If we execute this method for Unilimited 20GB
         it return Unilimited 20GB Pack
         """
+
+        if self.has_sharing_data_bond:
+            # Sharing data tariff products are already an offer
+            return
+
         attributes_with_pack = (
             self.attribute_value_ids
             + self.env.ref("somconnexio.IsInPack")
             - self.env.ref("somconnexio.IsNotInPack")
         )
         return self._related_product(attributes_with_pack)
 
     def get_product_without_offer(self):
         """
         Return the same product but the one without offer.
         Ex. If we execute this method for Unilimited 20GB Pack
         it return Unilimited 20GB
         """
+        if self.has_sharing_data_bond:
+            # Sharing data tariff products do not have a without offer correspondance
+            return
+
         attributes_without_pack = (
             self.attribute_value_ids
             - self.env.ref("somconnexio.IsInPack")
             + self.env.ref("somconnexio.IsNotInPack")
         )
         return self._related_product(attributes_without_pack)
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/product_template.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/product_template.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/res_company.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/res_company.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/res_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/stock_move_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/stock_move_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/stock_production_lot.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/stock_production_lot.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/models/subscription_request.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/models/subscription_request.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/account_hierarchy_resource.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/account_hierarchy_resource.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/crm_account_hierarchy.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/crm_account_hierarchy.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/customer.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/customer.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/services.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/services.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_models/subscription.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_models/subscription.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_strategies.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_create_strategies.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_strategies.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/crm_account_hierarchy_update_strategies.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/customer_update_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/customer_update_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/opencell_services/subscription_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/opencell_services/subscription_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/adsl_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/adsl_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/base_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/base_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/broadband_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/broadband_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/customer_data_from_res_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/customer_data_from_res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/fiber_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/fiber_data_from_crm_lead_line.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 from .broadband_data_from_crm_lead_line import BroadbandDataFromCRMLeadLine
 
 
 class FiberDataFromCRMLeadLine(BroadbandDataFromCRMLeadLine):
 
     def build(self):
         fiber_data = super().build()
-        fiber_data.update({
-            "previous_contract_pon": self.isp_info.previous_contract_pon,
-            "previous_contract_fiber_speed": self._previous_contract_fiber_speed(
-                self.isp_info.previous_contract_fiber_speed),
-            "mobile_pack_contracts": self._mobile_pack_contracts(
-                self.isp_info.mobile_pack_contracts
-            ),
-            "all_grouped_SIMS_recieved": self._have_all_grouped_mbl_SIMS(),
-            "has_grouped_mobile_with_previous_owner": (
-                self._has_grouped_mobile_with_previous_owner()
-            ),
-            "technology": fiber_data.get("technology") or "Fibra"
-        })
+        fiber_data.update(
+            {
+                "previous_contract_pon": self.isp_info.previous_contract_pon,
+                "previous_contract_fiber_speed": self._previous_contract_fiber_speed(
+                    self.isp_info.previous_contract_fiber_speed
+                ),
+                "mobile_pack_contracts": self._mobile_pack_contracts(
+                    self.isp_info.mobile_pack_contracts
+                ),
+                "all_grouped_SIMS_recieved": self._have_all_grouped_mbl_SIMS(),
+                "has_grouped_mobile_with_previous_owner": (
+                    self._has_grouped_mobile_with_previous_owner()
+                ),
+                "technology": fiber_data.get("technology") or "Fibra",
+                "product_ba_mm": self._product_ba_mm(),
+            }
+        )
         return FiberData(**fiber_data)
 
     def _previous_contract_fiber_speed(self, value):
         if value:
             return value.replace(" ", "")
         else:
             return ""
@@ -44,7 +48,26 @@
         previous_owners = \
             self.crm_lead_line.lead_id.lead_line_ids.filtered(
                 'is_mobile').mapped('mobile_isp_info').mapped(
                     'previous_owner_vat_number')
         if any(previous_owners):
             return True
         return False
+
+    def _product_ba_mm(self):
+        is_pack = self.crm_lead_line.lead_id.lead_line_ids.filtered(
+            "is_mobile"
+        ).filtered("is_from_pack")
+        is_shared = (
+            self.crm_lead_line.lead_id.lead_line_ids.filtered("is_mobile")
+            .mapped("product_id")
+            .filtered("has_sharing_data_bond")
+        )
+        product_ba_mm = "fibra_{}".format(
+            self.crm_lead_line.product_id.without_lang().get_catalog_name("Bandwidth")
+        )
+        if is_shared:
+            product_ba_mm = "{}_shared".format(product_ba_mm)
+        elif is_pack:
+            product_ba_mm = "{}_pack".format(product_ba_mm)
+
+        return product_ba_mm
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/mobile_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/mobile_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/service_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/service_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/otrs_factories/update_ticket_with_error.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/otrs_factories/update_ticket_with_error.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/account_asset_report_xls.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/account_asset_report_xls.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/aged_partner_balance.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/aged_partner_balance.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/crm_lead_creation_email_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/crm_lead_creation_email_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/invoice_claim_1_capital_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/invoice_claim_1_capital_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/invoice_claim_1_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/invoice_claim_1_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/mobile_can_be_linked_with_fiber_mail_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/mobile_can_be_linked_with_fiber_mail_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/mobile_linked_with_fiber_mail_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/mobile_linked_with_fiber_mail_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/new_sim_sending_letter_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/new_sim_sending_letter_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/report_paperformat.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/report_paperformat.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/sim_sending_letter_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/sim_sending_letter_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/reports/sponsor_sell_back_template.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/reports/sponsor_sell_back_template.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/security/ir.model.access.csv` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/security/ir.model.access.csv`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/__init__.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/account_invoice_process.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/account_invoice_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/account_payment_group_process.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/account_payment_group_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/bank_from_iban_getter.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/bank_from_iban_getter.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/change_partner_emails.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/change_partner_emails.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_change_tariff_process.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_change_tariff_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_contract_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_contract_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_contract_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,107 @@
-from odoo.exceptions import MissingError
 from odoo import _
-
-from otrs_somconnexio.services.search_tickets_service import SearchTicketsService
+from odoo.addons.base_rest.http import wrapJsonException
+from odoo.exceptions import MissingError
 from otrs_somconnexio.otrs_models.configurations.changes.change_tariff import (
     ChangeTariffTicketConfiguration,
 )
+from otrs_somconnexio.services.search_tickets_service import SearchTicketsService
+from werkzeug.exceptions import BadRequest
 
-from .vat_normalizer import VATNormalizer
+from .res_partner_service import AddressService
 
 
 class ContractService:
     def __init__(self, env):
         self.env = env
         self.Contract = self.env["contract.contract"]
 
     def search(self, **params):
-        code = params.get('code')
-        phone_number = params.get('phone_number')
-        partner_vat = params.get('partner_vat')
+        code = params.get("code")
+        phone_number = params.get("phone_number")
+        partner_vat = params.get("partner_vat")
+        limit = params.get("limit", 10)
+        offset = params.get("offset", 0)
+        sortBy = params.get("sortBy", "")
+        sortOrder = params.get("sortOrder", "")
+        customer_ref = params.get("customer_ref", "")
+        if limit:
+            if isinstance(limit, int) or isinstance(limit, str) and limit.isdigit():
+                limit = int(limit)
+            else:
+                raise wrapJsonException(
+                    BadRequest("Limit must be numeric"),
+                    include_description=True,
+                )
+        if offset:
+            if isinstance(offset, int) or isinstance(offset, str) and offset.isdigit():
+                offset = int(offset)
+            else:
+                raise wrapJsonException(
+                    BadRequest("Offset must be numeric"),
+                    include_description=True,
+                )
+        if sortBy:
+            if sortBy not in self.env["contract.contract"].fields_get():
+                raise wrapJsonException(
+                    BadRequest("Invalid field to sortBy"), include_description=True
+                )
+        if sortOrder:
+            if sortOrder == "ASCENDENT":
+                pass
+            elif sortOrder == "DESCENDENT":
+                sortOrder = " DESC"
+            else:
+                raise wrapJsonException(
+                    BadRequest("sortOrder must be ASCENDING or DESCENDING"),
+                    include_description=True,
+                )
 
         if code:
-            contracts = self.Contract.sudo().search(
-                [('code', '=', code)]
-            )
-            search_param = 'code'
+            domain = [("code", "=", code)]
+            search_param = "code"
+        elif customer_ref:
+            domain = [("partner_id.ref", "=", customer_ref)]
+            search_param = "customer_ref"
         elif phone_number:
-            contracts = self.Contract.sudo().search(
-                [("phone_number", "=", phone_number)]
-            )
+            domain = [("phone_number", "=", phone_number)]
             search_param = "phone_number"
         elif partner_vat:
-            partner = (
-                self.env["res.partner"]
-                .sudo()
-                .search(
-                    [
-                        (
-                            "vat",
-                            "ilike",
-                            VATNormalizer(partner_vat).convert_spanish_vat(),
-                        ),
-                        ("parent_id", "=", False),
-                    ]
-                )
-            )
-            contracts = self.Contract.sudo().search([("partner_id", "=", partner.id)])
+            domain = [
+                ("partner_id.vat", "=", partner_vat),
+                ("partner_id.parent_id", "=", False),
+            ]
             search_param = "partner_vat"
+        domain += [("is_terminated", "=", False)]
+        contracts = self.Contract.sudo().search(
+            domain, limit=limit, offset=offset, order=sortBy + sortOrder
+        )
         if not contracts:
             raise MissingError(
                 _('No contract with {}: {} could be found'.format(
                     search_param, params.get(search_param)))
                 )
 
-        return [self._to_dict(contract) for contract in contracts]
+        ret = {"contracts": [self._to_dict(contract) for contract in contracts]}
+        if limit or offset or sortBy:
+            ret["paging"] = {
+                "limit": limit,
+                "offset": offset,
+                "totalNumberOfRecords": self.Contract.sudo().search_count(domain),
+            }
+            if sortBy:
+                ret["paging"].update(
+                    {
+                        "sortBy": sortBy,
+                        "sortOrder": "DESCENDENT"
+                        if sortOrder == " DESC"
+                        else "ASCENDENT",
+                    }
+                )
+        return ret
 
     def create(self, **params):
         self.Contract.with_delay().create_contract(**params)
         return {"result": "OK"}
 
     def count(self):
         domain_contracts = [('is_terminated', '=', False)]
@@ -102,15 +147,16 @@
                     "=",
                     self.env.ref("somconnexio.service_technology_fiber").id,
                 ),
             ]
         )
         if params.get('mobiles_sharing_data') == 'true':
             contracts = contracts.filtered(
-                lambda c: len(c.children_pack_contract_ids) < 3
+                lambda c: len(c.children_pack_contract_ids) < 3 or
+                not c.children_pack_contract_ids
             )
         else:
             contracts = contracts.filtered(
                 lambda c: not c.children_pack_contract_ids
             )
 
         contracts = self._filter_out_fibers_used_in_OTRS_tickets(contracts)
@@ -130,31 +176,73 @@
 
         fiber_signal = contract.fiber_signal_type_id and \
             contract.fiber_signal_type_id.code or False
 
         return {
             "id": contract.id,
             "code": contract.code,
+            "email": contract.partner_id.email,
             "customer_firstname": contract.partner_id.firstname,
             "customer_lastname": contract.partner_id.lastname,
             "customer_ref": contract.partner_id.ref,
             "customer_vat": contract.partner_id.vat,
             "phone_number": contract.phone_number,
             "current_tariff_product": contract.current_tariff_product.default_code,
+            "description": contract.current_tariff_product.with_context(
+                lang=contract.lang
+            ).custom_name,
             "ticket_number": contract.ticket_number,
             "technology": contract.service_technology_id.name,
             "supplier": contract.service_supplier_id.name,
             "lang": contract.lang,
             "iban": contract.mandate_id.partner_bank_id.sanitized_acc_number,
             "is_terminated": contract.is_terminated,
             "date_start": contract.date_start,
             "date_end": contract.date_end,
             "fiber_signal": fiber_signal,
+            "subscription_type": (
+                "mobile" if contract.service_contract_type == "mobile" else "broadband"
+            ),
+            "address": AddressService(self.env, contract.service_partner_id).__dict__,
+            "subscription_technology": (
+                contract.service_contract_type
+                if contract.service_contract_type in (
+                    "adsl", "mobile"
+                )
+                else "fiber"
+            ),
+            "available_operations": self._available_operations(contract),
+            "parent_contract": contract.parent_pack_contract_id.code
+            if contract.parent_pack_contract_id
+            else "",
+            "shared_bond_id": contract.shared_bond_id,
+            "price": self._product_price(contract.current_tariff_product),
+            "has_landline_phone": not bool(contract.current_tariff_product.without_fix)
+            if contract.service_contract_type != "mobile"
+            else False,
+            "bandwidth": int(
+                contract.current_tariff_product.without_lang().get_catalog_name(
+                    "Bandwidth"
+                )
+                or 0
+            ),
         }
 
+    def _available_operations(self, contract):
+        if contract.service_contract_type == "mobile":
+            if contract.shared_bond_id:
+                return ["AddOneShotMobile"]
+            else:
+                return ["ChangeTariffMobile", "AddOneShotMobile"]
+        elif contract.current_tariff_product.without_fix:
+            return ["ChangeTariffFiberOutLandline"]
+        elif contract.service_contract_type == "adsl":
+            return ["ChangeTariffFiberLandline"]
+        return []
+
     def _filter_out_fibers_used_in_OTRS_tickets(self, contracts):
         """
         From a list of fiber contracts, search if any of their codes are
         already referenced in OTRS new mobile change tariff tickets
         (DF OdooContractRefRelacionat).
         If so, that fiber contract is about to be linked to a mobile offer,
         and shouldn't be available for others.
@@ -203,7 +291,11 @@
             ('stage_id', 'not in', stages_to_discard)
         ])
 
         already_linked_contracts = mbl_lead_lines.mapped(
             'mobile_isp_info').mapped('linked_fiber_contract_id')
 
         return contracts - already_linked_contracts
+
+    def _product_price(self, product):
+        pricelist_id = self.env["product.pricelist"].search([("code", "=", "21IVA")])
+        return product.with_context(pricelist=pricelist_id.id).price
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_email_change_process.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_email_change_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_iban_change_process.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_iban_change_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_one_shot_process.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_one_shot_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/adsl.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/adsl.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/ba.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/ba.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/base.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     @staticmethod
     def _to_dict(contract):
         return {
             "id": contract.id,
             "code": contract.code,
             "partner_id": contract.partner_id.id,
             "ticket_number": contract.ticket_number,
+            "create_reason": contract.create_reason,
         }
 
     def _prepare_create_line(self, line):
         product = (
             self.env["product.product"]
             .sudo()
             .search([("default_code", "=", line["product_code"])])
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/fiber.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/fiber.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,21 +159,27 @@
             )
             for contract in mobile_contracts:
                 contract.parent_pack_contract_id = id
 
     def _relate_new_fiber_with_existing_mobile_contracts(
             self, contract_dict):
         """
-        Check if within fiber CRMLead there is a mobile with
-        pack product, in which case, do nothing (fiber contract
-        is needed to be packed with it).
-        If no one found, pack it with an already existing partner's
-        mobile contract, if appropiate according to its tariff.
+        Link new fiber to an existing mobile contract, except:
+          - New fiber contract comes from location_change
+          - Within the fiber CRMLead there is a mobile with
+            pack product (the fiber contract is needed to be
+            packed with that mobile).
+          - No existing mobile contract is found with appropiate
+            mobile tariffs to be packed.
         """
 
+        # Check that fiber contract does not come from a location change
+        if contract_dict["create_reason"] == "location_change":
+            return
+
         # Check if fiber CRMLead has mobile with pack product
         crm_lead_line = self.env["crm.lead.line"].sudo().search(
             [("ticket_number", "=", contract_dict["ticket_number"])]
         )
         mobile_lines = crm_lead_line.lead_id.lead_line_ids.filtered(
             "is_mobile").filtered("is_from_pack")
         if mobile_lines:
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/mobile.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/mobile.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/contract_process/router4g.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/contract_process/router4g.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/crm_lead_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/crm_lead_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/discovery_channel_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/discovery_channel_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/get_activation_date.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/get_activation_date.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/partner_email_change_process.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/partner_email_change_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/product_catalog_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/product_catalog_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/provider_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/provider_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/res_partner_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/res_partner_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/schemas.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,29 +587,47 @@
     "contracts": {"type": ["dict", "string"], "required": True},
     "start_date": {"type": "string"},
     "summary": {"type": "string"},
     "done": {"type": "boolean"},
 }
 
 S_CONTRACT_SEARCH = {
+    "customer_ref": {
+        "type": "string",
+        "excludes": ["code", "partner_vat", "phone_number"],
+        "required": True
+    },
     "code": {
         "type": "string",
-        "excludes": ["partner_vat", "phone_number"],
+        "excludes": ["partner_vat", "phone_number", "customer_ref"],
         "required": True
     },
     "partner_vat": {
         "type": "string",
-        "excludes": ["code", "phone_number"],
+        "excludes": ["code", "phone_number", "customer_ref"],
         "required": True
     },
     "phone_number": {
         "type": "string",
-        "excludes": ["partner_vat", "code"],
+        "excludes": ["partner_vat", "code", "customer_ref"],
         "required": True
     },
+    "limit": {
+        "type": "string",
+    },
+    "offset": {
+        "type": "string",
+    },
+    "sortBy": {
+        "type": "string",
+    },
+    "sortOrder": {
+        "type": "string",
+        "dependencies": ['sortBy']
+    }
 }
 
 S_CONTRACT_GET_FIBER_CONTRACTS_TO_PACK = {
     "partner_ref": {
         "type": "string",
         "required": True,
     },
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/services/subscription_request_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/services/subscription_request_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/somoffice/user.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/somoffice/user.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/activities.png` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/activities.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/broadband_contract.png` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/broadband_contract.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/broadband_lead_lines.png` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/broadband_lead_lines.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/emails.png` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/emails.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/mobile_contract.png` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/mobile_contract.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/mobile_lead_lines.png` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/mobile_lead_lines.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/description/packs.png` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/description/packs.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/img/sc-image.png` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/img/sc-image.png`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/js/holidays_highlighter.js` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/js/holidays_highlighter.js`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/js/many2many_tags_contract_email.js` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/js/many2many_tags_contract_email.js`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/js/many2one_tags_crm_lead_email.js` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/js/many2one_tags_crm_lead_email.js`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/js/my_attendances.js` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/js/my_attendances.js`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/static/src/xml/attendance.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/static/src/xml/attendance.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/__init__.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/correos_services/test_shipment.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/correos_services/test_shipment.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/factories.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/factories.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/helpers.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/helpers.py`

 * *Files 23% similar despite different names*

```diff
@@ -77,83 +77,108 @@
         "state_id": odoo_env.ref("base.state_es_b"),
         "customer": True,
         "ref": random_ref(),
         "lang": random.choice(["es_ES", "ca_ES"]),
     }
 
 
-def crm_lead_create(
-    odoo_env, partner_id, service_category, portability=False, pack=False
+def crm_lead_line_create(
+    odoo_env, service_category, portability, shared_bond_id="ABC1234"
 ):
     product_switcher = {
-        "mobile": odoo_env.ref("somconnexio.TrucadesIllimitades20GBPack") if pack else odoo_env.ref("somconnexio.TrucadesIllimitades20GB"),  # noqa
+        "mobile": odoo_env.ref("somconnexio.TrucadesIllimitades20GB"),
+        "pack": odoo_env.ref("somconnexio.TrucadesIllimitades20GBPack"),
+        "shared_data": odoo_env.ref("somconnexio.50GBCompartides2mobils"),
         "fiber": odoo_env.ref("somconnexio.Fibra100Mb"),
         "adsl": odoo_env.ref("somconnexio.ADSL20MBSenseFix"),
         "4G": odoo_env.ref("somconnexio.Router4G"),
     }
-    crm_lead_line_args = {
-        "name": "CRM Lead",
-        "product_id": product_switcher[service_category].id,
-    }
-    isp_info_args = (
+    base_isp_info_args = (
         {
             "type": "portability",
             "previous_contract_type": "contract",
             "previous_provider": odoo_env.ref("somconnexio.previousprovider39").id,
-            "phone_number": None,
             "previous_owner_vat_number": faker.vat_id(),
             "previous_owner_name": faker.first_name(),
-            'previous_owner_first_name': faker.last_name(),
+            "previous_owner_first_name": faker.last_name(),
         }
         if portability
         else {"type": "new"}
     )
+    base_ba_isp_info_args = {
+        "service_full_street": faker.address(),
+        "service_city": faker.city(),
+        "service_zip_code": "08015",
+        "service_state_id": odoo_env.ref("base.state_es_b").id,
+        "service_country_id": odoo_env.ref("base.es").id,
+    }
 
-    if service_category == "mobile":
-        isp_info_args.update({
+    isp_info_args_switcher = {
+        "mobile": {"phone_number": random_mobile_phone(), "icc": random_icc(odoo_env)},
+        "pack": {"phone_number": random_mobile_phone(), "icc": random_icc(odoo_env)},
+        "shared_data": {
             "phone_number": random_mobile_phone(),
-            'icc': random_icc(odoo_env)
-        })
-        isp_info = odoo_env["mobile.isp.info"].create(isp_info_args)
-        crm_lead_line_args.update({"mobile_isp_info": isp_info.id})
+            "shared_bond_id": shared_bond_id,
+        },
+        "fiber": dict(**base_ba_isp_info_args, phone_number=random_landline_number()),
+        "adsl": dict(**base_ba_isp_info_args, phone_number=random_landline_number()),
+        "4G": dict(**base_ba_isp_info_args, phone_number="-"),
+    }
+    model_switcher = {
+        "mobile": "mobile.isp.info",
+        "pack": "mobile.isp.info",
+        "shared_data": "mobile.isp.info",
+        "fiber": "broadband.isp.info",
+        "adsl": "broadband.isp.info",
+        "4G": "broadband.isp.info",
+    }
+    isp_info = odoo_env[model_switcher[service_category]].create(
+        dict(**base_isp_info_args, **isp_info_args_switcher[service_category])
+    )
+    crm_lead_line_args = {
+        "name": "CRM Lead",
+        "product_id": product_switcher[service_category].id,
+    }
+    if service_category in ["fiber", "adsl", "4G"]:
+        crm_lead_line_args.update(
+            {
+                "broadband_isp_info": isp_info.id,
+            }
+        )
     else:
-        isp_info_args.update(
+        crm_lead_line_args.update(
             {
-                "phone_number": "-" if service_category == "4G" else random_landline_number(),  # noqa
-                "service_full_street": faker.address(),
-                "service_city": faker.city(),
-                "service_zip_code": "08015",
-                "service_state_id": odoo_env.ref("base.state_es_b").id,
-                "service_country_id": odoo_env.ref("base.es").id,
+                "mobile_isp_info": isp_info.id,
             }
         )
-        isp_info = odoo_env["broadband.isp.info"].create(isp_info_args)
-        crm_lead_line_args.update({"broadband_isp_info": isp_info.id})
 
-    crm_lead_line_ids = [odoo_env["crm.lead.line"].create(crm_lead_line_args).id]
+    return odoo_env["crm.lead.line"].create(crm_lead_line_args)
 
-    if pack and service_category == "fiber":
-        isp_info_args = {
-            "type": "new",
-            "phone_number": random_mobile_phone(),
-        }
-        isp_info = odoo_env["mobile.isp.info"].create({
-            "type": "new",
-            "phone_number": random_mobile_phone(),
-            "icc": random_icc(odoo_env),
-        })
-        mobile_crm_lead_line_args = {
-            "name": "CRM Lead",
-            "product_id": product_switcher["mobile"].id,
-            "mobile_isp_info": isp_info.id,
-        }
-        crm_lead_line_ids.append(
-            odoo_env["crm.lead.line"].create(mobile_crm_lead_line_args).id
-        )
 
+def crm_lead_create(
+    odoo_env,
+    partner_id,
+    service_category,
+    portability=False,
+):
+    if service_category in ["mobile", "fiber", "adsl", "4G"]:
+        crm_lead_line_ids = [
+            crm_lead_line_create(odoo_env, service_category, portability).id,
+        ]
+    elif service_category == "pack":
+        crm_lead_line_ids = [
+            crm_lead_line_create(odoo_env, "fiber", portability).id,
+            crm_lead_line_create(odoo_env, service_category, portability).id,
+        ]
+    elif service_category == "shared_data":
+        crm_lead_line_ids = [
+            crm_lead_line_create(odoo_env, "fiber", portability).id,
+            crm_lead_line_create(odoo_env, service_category, portability).id,
+            crm_lead_line_create(odoo_env, service_category, portability).id,
+        ]
     return odoo_env["crm.lead"].create(
         {
             "name": "Test Lead",
             "partner_id": partner_id.id,
             "iban": partner_id.bank_ids[0].sanitized_acc_number,
             "lead_line_ids": [(6, 0, crm_lead_line_ids)],
             "stage_id": odoo_env.ref("crm.stage_lead1").id,
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/test_contract_line_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/test_contract_line_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/test_contract_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/test_contract_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/test_crm_lead_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/test_crm_lead_listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,17 @@
         queue_jobs_after = self.env['queue.job'].search_count([])
 
         self.assertEqual(queue_jobs_before, queue_jobs_after - 1)
 
         queue_jobs_before = queue_jobs_after
 
         crm_lead_to_link = crm_lead_create(
-            self.env, self.partner_id, "fiber", portability=False, pack=True
+            self.env,
+            self.partner_id,
+            "pack",
         )
         crm_lead_to_link.action_set_remesa()
         crm_lead_to_link.action_set_won()
 
         queue_jobs_after = self.env["queue.job"].search_count([])
         jobs_domain = [
             ("method_name", "=", "link_pack_tickets"),
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/test_partner_bank_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/test_partner_bank_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/test_partner_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/test_partner_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/listeners/test_res_partner_listener.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/listeners/test_res_partner_listener.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_account_invoice.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_account_invoice.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_account_move_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_account_move_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_account_payment_order.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_account_payment_order.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_account_payment_return_gateway.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_account_payment_return_gateway.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_broadband_isp_info.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_broadband_isp_info.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_contract.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_contract.py`

 * *Files 0% similar despite different names*

```diff
@@ -709,36 +709,36 @@
 
         # Create second mobile contract sharing data with the first one
         mbl_vals_contract['mobile_contract_service_info_id'] = msci.copy().id
         mbl_2_contract = self.Contract.create(mbl_vals_contract)
 
         self.assertTrue(mbl_2_contract.sharing_bond_contract_ids)
         self.assertEquals(
-            mbl_2_contract.sharing_bond_contract_ids.ids,
-            [mbl_1_contract.id, mbl_2_contract.id]
+            set(mbl_2_contract.sharing_bond_contract_ids.ids),
+            set([mbl_1_contract.id, mbl_2_contract.id])
         )
         self.assertEquals(
-            fiber_contract.children_pack_contract_ids.ids,
-            [mbl_1_contract.id, mbl_2_contract.id]
+            set(fiber_contract.children_pack_contract_ids.ids),
+            set([mbl_1_contract.id, mbl_2_contract.id])
         )
         self.assertEquals(fiber_contract.number_contracts_in_pack, 3)
 
         # Create third mobile contract sharing data with the other two
         mbl_vals_contract['mobile_contract_service_info_id'] = msci.copy().id
         mbl_3_contract = self.Contract.create(mbl_vals_contract)
 
         self.assertTrue(mbl_3_contract.sharing_bond_contract_ids)
         self.assertEquals(len(mbl_3_contract.sharing_bond_contract_ids), 3)
         self.assertEquals(
-            mbl_3_contract.sharing_bond_contract_ids.ids,
-            [mbl_1_contract.id, mbl_2_contract.id, mbl_3_contract.id]
+            set(mbl_3_contract.sharing_bond_contract_ids.ids),
+            set([mbl_1_contract.id, mbl_2_contract.id, mbl_3_contract.id])
         )
         self.assertEquals(
-            fiber_contract.children_pack_contract_ids.ids,
-            [mbl_1_contract.id, mbl_2_contract.id, mbl_3_contract.id]
+            set(fiber_contract.children_pack_contract_ids.ids),
+            set([mbl_1_contract.id, mbl_2_contract.id, mbl_3_contract.id])
         )
         self.assertEquals(fiber_contract.number_contracts_in_pack, 4)
 
     def test_not_pack_contract_id(self, *args):
         partner_id = self.partner.id
         vals_contract = {
             'name': 'Test Contract Broadband',
@@ -824,7 +824,19 @@
                 ).id,
                 "exceptional_change": True,
                 "otrs_checked": True,
                 "send_notification": False,
             }
         )
         mock_change_tariff_create.return_value.button_change.assert_called_once_with()
+
+    def test_display_name_broadband_contracts(self, *args):
+        contract = self.browse_ref("somconnexio.contract_fibra_600")
+
+        expected_name = "{} - {}, {}, {}, {}".format(
+            contract.name,
+            contract.service_partner_id.full_street,
+            contract.service_partner_id.city,
+            contract.service_partner_id.zip,
+            contract.service_partner_id.state_id.name,
+        )
+        self.assertEqual(contract.display_name, expected_name)
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_coop_agreement.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_coop_agreement.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_crm_lead.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_crm_lead.py`

 * *Files 0% similar despite different names*

```diff
@@ -664,16 +664,15 @@
                 mobile_isp_info_2.phone_number,
                 broadband_isp_info.phone_number
             ])
 
         )
 
     def test_crm_lead_right_archive_crm_lead_line(self):
-        crm_lead = crm_lead_create(self.env, self.partner_id, "fiber",
-                                   portability=True, pack=True)
+        crm_lead = crm_lead_create(self.env, self.partner_id, "pack", portability=True)
         mobile_crm_lead_line = crm_lead.lead_line_ids.filtered("is_mobile")
 
         self.assertTrue(mobile_crm_lead_line.active)
         self.assertEqual(crm_lead.sims_to_deliver, 'one')
 
         mobile_crm_lead_line.toggle_active()
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_hr_attendance_process.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_hr_attendance_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_mail_activity.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_mail_activity.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_mass_mailing.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_mass_mailing.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_mobile_isp_info.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_mobile_isp_info.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_opencell_configuration_wrapper.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_opencell_configuration_wrapper.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_payment_return.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_payment_return.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_previous_provider.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_previous_provider.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_product_category_technology_supplier.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_product_category_technology_supplier.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_product_product.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_product_product.py`

 * *Files 26% similar despite different names*

```diff
@@ -29,7 +29,19 @@
         product = self.browse_ref('somconnexio.Fibra100Mb')
         old_value = product.default_code
         product.write({'default_code': 'new-default-code-value'})
         expected_msg = "Field '{}' edited from '{}' to '{}'".format(
             'default_code', old_value, 'new-default-code-value'
         )
         message_post_mock.assert_called_once_with(body=expected_msg)
+
+    def test_get_offer_sharing_product(self):
+        sharing_data_product = self.browse_ref('somconnexio.50GBCompartides2mobils')
+
+        self.assertFalse(sharing_data_product.get_offer())
+
+    def test_get_product_without_offer_sharing_product(self):
+        sharing_data_product = self.browse_ref('somconnexio.50GBCompartides2mobils')
+
+        self.assertFalse(
+            sharing_data_product.get_product_without_offer(),
+        )
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_product_template.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_product_template.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_production_lot.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_production_lot.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_res_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_res_partner_bank.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_res_partner_bank.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_server_action.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_server_action.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_service_supplier.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_service_supplier.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_stock_move_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_stock_move_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/models/test_subscription_request.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/models/test_subscription_request.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_models/test_address.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_models/test_address.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_models/test_crm_account_hierarchy.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_models/test_crm_account_hierarchy.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_models/test_customer.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_models/test_customer.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_models/test_opencell_service_codes.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_models/test_opencell_service_codes.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_models/test_subscription.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_models/test_subscription.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_strategies.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_create_strategies.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_strategies.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/test_crm_account_hierarchy_update_strategies.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/test_customer_update_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/test_customer_update_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/opencell_services/test_subscription_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/opencell_services/test_subscription_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/test_adsl_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/test_adsl_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/test_customer_data_from_res_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/test_customer_data_from_res_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/test_fiber_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/test_fiber_data_from_crm_lead_line.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,38 +8,33 @@
 from ..helpers import crm_lead_create
 from ..sc_test_case import SCTestCase
 
 
 class FiberDataFromCRMLeadLineTest(SCTestCase):
     def setUp(self, *args, **kwargs):
         super().setUp(*args, **kwargs)
-        self.partner_id = self.browse_ref('somconnexio.res_partner_2_demo')
+        self.partner_id = self.browse_ref("somconnexio.res_partner_2_demo")
 
     def test_build(self):
         ba_crm_lead = crm_lead_create(self.env, self.partner_id, "fiber")
         crm_lead_line = ba_crm_lead.lead_line_ids[0]
         broadband_isp_info = crm_lead_line.broadband_isp_info
 
         fiber_data = FiberDataFromCRMLeadLine(crm_lead_line).build()
 
         self.assertEqual(fiber_data.order_id, crm_lead_line.id)
         self.assertEqual(fiber_data.technology, "Fibra")
         self.assertEqual(fiber_data.phone_number, broadband_isp_info.phone_number)
         self.assertEqual(
-            fiber_data.service_address,
-            broadband_isp_info.service_full_street)
-        self.assertEqual(
-            fiber_data.service_city,
-            broadband_isp_info.service_city)
-        self.assertEqual(
-            fiber_data.service_zip,
-            broadband_isp_info.service_zip_code)
+            fiber_data.service_address, broadband_isp_info.service_full_street
+        )
+        self.assertEqual(fiber_data.service_city, broadband_isp_info.service_city)
+        self.assertEqual(fiber_data.service_zip, broadband_isp_info.service_zip_code)
         self.assertEqual(
-            fiber_data.service_subdivision,
-            broadband_isp_info.service_state_id.name
+            fiber_data.service_subdivision, broadband_isp_info.service_state_id.name
         )
         self.assertEqual(fiber_data.service_subdivision_code, "B")
         self.assertEqual(
             fiber_data.shipment_address, broadband_isp_info.delivery_full_street
         )
         self.assertEqual(fiber_data.shipment_city, broadband_isp_info.delivery_city)
         self.assertEqual(fiber_data.shipment_zip, broadband_isp_info.delivery_zip_code)
@@ -48,18 +43,20 @@
         )
         self.assertEqual(fiber_data.notes, crm_lead_line.lead_id.description)
         self.assertEqual(fiber_data.iban, crm_lead_line.lead_id.iban)
         self.assertEqual(fiber_data.email, crm_lead_line.lead_id.email_from)
         self.assertEqual(fiber_data.product, crm_lead_line.product_id.default_code)
         self.assertFalse(fiber_data.all_grouped_SIMS_recieved)
         self.assertFalse(fiber_data.has_grouped_mobile_with_previous_owner)
+        self.assertEqual(fiber_data.product_ba_mm, "fibra_100")
 
     def test_portability_build(self):
-        ba_crm_lead = crm_lead_create(self.env, self.partner_id, "fiber",
-                                      portability=True)
+        ba_crm_lead = crm_lead_create(
+            self.env, self.partner_id, "fiber", portability=True
+        )
         crm_lead_line = ba_crm_lead.lead_line_ids[0]
         broadband_isp_info = crm_lead_line.broadband_isp_info
         broadband_isp_info.write({"previous_service": "fiber"})
 
         fiber_data = FiberDataFromCRMLeadLine(crm_lead_line).build()
 
         self.assertEqual(fiber_data.phone_number, broadband_isp_info.phone_number)
@@ -74,41 +71,47 @@
         )
         self.assertEqual(
             fiber_data.previous_provider, broadband_isp_info.previous_provider.code
         )
         self.assertEqual(fiber_data.previous_service, "Fibra")
 
     def test_check_phone_number_build(self):
-        ba_crm_lead = crm_lead_create(self.env, self.partner_id, "fiber",
-                                      portability=True)
+        ba_crm_lead = crm_lead_create(
+            self.env, self.partner_id, "fiber", portability=True
+        )
         crm_lead_line = ba_crm_lead.lead_line_ids[0]
         crm_lead_line.check_phone_number = True
 
         fiber_data = FiberDataFromCRMLeadLine(crm_lead_line).build()
 
-        self.assertEqual(fiber_data.phone_number, 'REVISAR FIX')
+        self.assertEqual(fiber_data.phone_number, "REVISAR FIX")
 
     def test_change_address_build(self):
         service_supplier = self.browse_ref("somconnexio.service_supplier_vodafone")
-        ba_crm_lead = crm_lead_create(self.env, self.partner_id, "fiber",
-                                      portability=True)
+        ba_crm_lead = crm_lead_create(
+            self.env, self.partner_id, "fiber", portability=True
+        )
         crm_lead_line = ba_crm_lead.lead_line_ids[0]
         broadband_isp_info = crm_lead_line.broadband_isp_info
-        broadband_isp_info.write({
-            "type": "location_change",
-            "service_supplier_id": service_supplier.id,
-            "mm_fiber_coverage": MMFibreCoverage.VALUES[2][0],
-            "vdf_fiber_coverage": VdfFibreCoverage.VALUES[3][0],
-            "orange_fiber_coverage": OrangeFibreCoverage.VALUES[1][0],
-            "adsl_coverage": ADSLCoverage.VALUES[6][0],
-            "previous_contract_phone": "666666666",
-            "previous_contract_address": "Calle Teper",
-            "previous_contract_pon": "VDF0001",
-            "previous_contract_fiber_speed": self.browse_ref('somconnexio.100Mb').name,
-        })
+        broadband_isp_info.write(
+            {
+                "type": "location_change",
+                "service_supplier_id": service_supplier.id,
+                "mm_fiber_coverage": MMFibreCoverage.VALUES[2][0],
+                "vdf_fiber_coverage": VdfFibreCoverage.VALUES[3][0],
+                "orange_fiber_coverage": OrangeFibreCoverage.VALUES[1][0],
+                "adsl_coverage": ADSLCoverage.VALUES[6][0],
+                "previous_contract_phone": "666666666",
+                "previous_contract_address": "Calle Teper",
+                "previous_contract_pon": "VDF0001",
+                "previous_contract_fiber_speed": self.browse_ref(
+                    "somconnexio.100Mb"
+                ).name,
+            }
+        )
 
         fiber_data = FiberDataFromCRMLeadLine(crm_lead_line).build()
 
         self.assertEqual(fiber_data.previous_internal_provider, service_supplier.ref)
         self.assertEqual(fiber_data.mm_fiber_coverage, MMFibreCoverage.VALUES[2][0])
         self.assertEqual(fiber_data.vdf_fiber_coverage, VdfFibreCoverage.VALUES[3][0])
         self.assertEqual(
@@ -145,75 +148,99 @@
                 "service_supplier_id": self.ref(
                     "somconnexio.service_supplier_masmovil"
                 ),
                 "mobile_contract_service_info_id": mobile_contract_service_info.id,
                 "bank_id": partner.bank_ids.id,
             }
         )
-        ba_crm_lead = crm_lead_create(self.env, self.partner_id, "fiber",
-                                      portability=True)
+        ba_crm_lead = crm_lead_create(
+            self.env, self.partner_id, "fiber", portability=True
+        )
         crm_lead_line = ba_crm_lead.lead_line_ids[0]
         broadband_isp_info = crm_lead_line.broadband_isp_info
-        broadband_isp_info.write({
-            "type": "location_change",
-            "service_supplier_id": self.browse_ref(
-                "somconnexio.service_supplier_vodafone").id,
-            "mobile_pack_contracts": [(6, 0, [mobile_contract.id])],
-        })
+        broadband_isp_info.write(
+            {
+                "type": "location_change",
+                "service_supplier_id": self.browse_ref(
+                    "somconnexio.service_supplier_vodafone"
+                ).id,
+                "mobile_pack_contracts": [(6, 0, [mobile_contract.id])],
+            }
+        )
 
         fiber_data = FiberDataFromCRMLeadLine(crm_lead_line).build()
 
-        self.assertEqual(
-            fiber_data.mobile_pack_contracts,
-            mobile_contract.code
-        )
+        self.assertEqual(fiber_data.mobile_pack_contracts, mobile_contract.code)
         self.assertEqual(fiber_data.type, "location_change")
 
     def test_grouped_mobile_params_true(self):
-        pack_crm_lead = crm_lead_create(self.env, self.partner_id, "fiber",
-                                        portability=True, pack=True)
+        pack_crm_lead = crm_lead_create(
+            self.env, self.partner_id, "pack", portability=True
+        )
         mbl_lead_line = pack_crm_lead.lead_line_ids.filtered(
-            lambda line: line.is_mobile)
+            lambda line: line.is_mobile
+        )
         mbl_lead_line.mobile_isp_info_has_sim = True
         mbl_lead_line.mobile_isp_info.update(
             {
-                'previous_owner_vat_number': '1234G',
-                'previous_owner_name': 'Owner',
-                'previous_owner_first_name': 'Previous',
+                "previous_owner_vat_number": "1234G",
+                "previous_owner_name": "Owner",
+                "previous_owner_first_name": "Previous",
             }
         )
         fiber_lead_line = pack_crm_lead.lead_line_ids.filtered(
-            lambda line: not line.is_mobile)
+            lambda line: not line.is_mobile
+        )
 
         fiber_data = FiberDataFromCRMLeadLine(fiber_lead_line).build()
 
         self.assertTrue(mbl_lead_line.mobile_isp_info.has_sim)
         self.assertTrue(fiber_data.all_grouped_SIMS_recieved)
         self.assertTrue(fiber_data.has_grouped_mobile_with_previous_owner)
 
     def test_grouped_mobile_params_false(self):
-        pack_crm_lead = crm_lead_create(self.env, self.partner_id, "fiber",
-                                        portability=True, pack=True)
+        pack_crm_lead = crm_lead_create(
+            self.env, self.partner_id, "pack", portability=True
+        )
         mbl_lead_line = pack_crm_lead.lead_line_ids.filtered(
-            lambda line: line.is_mobile)
-        mbl_lead_line_2 = mbl_lead_line.copy()
-        new_mobile_isp_info = self.env['mobile.isp.info'].create({
-            'type': 'new',
-            'has_sim': True,
-        })
-        mbl_lead_line_2.write({
-            "mobile_isp_info": new_mobile_isp_info.id
-        })
-
-        pack_crm_lead.write({
-            "lead_line_ids": [(4, mbl_lead_line_2.id, False)]
-        })
+            lambda line: line.is_mobile
+        )
+        mbl_lead_line.mobile_isp_info.update(
+            {
+                "previous_owner_vat_number": False,
+                "previous_owner_name": False,
+                "previous_owner_first_name": False,
+            }
+        )
 
         fiber_lead_line = pack_crm_lead.lead_line_ids.filtered(
-            lambda line: not line.is_mobile)
+            lambda line: not line.is_mobile
+        )
 
         fiber_data = FiberDataFromCRMLeadLine(fiber_lead_line).build()
 
-        self.assertFalse(mbl_lead_line.mobile_isp_info.has_sim)
-        self.assertTrue(mbl_lead_line_2.mobile_isp_info.has_sim)
         self.assertFalse(fiber_data.all_grouped_SIMS_recieved)
         self.assertFalse(fiber_data.has_grouped_mobile_with_previous_owner)
+
+    def test_fiber_product_ba_mm_with_mobile_pack(self):
+        pack_crm_lead = crm_lead_create(
+            self.env, self.partner_id, "pack", portability=True
+        )
+        fiber_lead_line = pack_crm_lead.lead_line_ids.filtered(
+            lambda line: not line.is_mobile
+        )
+
+        fiber_data = FiberDataFromCRMLeadLine(fiber_lead_line).build()
+
+        self.assertEqual(fiber_data.product_ba_mm, "fibra_100_pack")
+
+    def test_fiber_product_ba_mm_with_shared_data_mobile(self):
+        crm_lead = crm_lead_create(
+            self.env, self.partner_id, "shared_data", portability=True
+        )
+        fiber_lead_line = crm_lead.lead_line_ids.filtered(
+            lambda line: not line.is_mobile
+        )
+
+        fiber_data = FiberDataFromCRMLeadLine(fiber_lead_line).build()
+
+        self.assertEqual(fiber_data.product_ba_mm, "fibra_100_shared")
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/test_mobile_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/test_mobile_data_from_crm_lead_line.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,16 +76,18 @@
         self.assertEqual(mobile_data.sc_icc, mobile_isp_info.icc)
         self.assertEqual(mobile_data.icc, mobile_isp_info.icc_donor)
         self.assertFalse(mobile_data.is_grouped_with_fiber)
         self.assertFalse(mobile_data.sim_delivery_tracking_code)
 
     def test_has_lead_fiber_service_actual_pack(self):
         pack_crm_lead = crm_lead_create(
-            self.env, self.partner_id, "fiber",
-            pack=True)
+            self.env,
+            self.partner_id,
+            "pack",
+        )
 
         mbl_pack_lead_line = pack_crm_lead.lead_line_ids.filtered(
             lambda line: line.is_mobile)
 
         mobile_data_pack_line = MobileDataFromCRMLeadLine(
             mbl_pack_lead_line).build()
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/test_router_4G_data_from_crm_lead_line.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/test_router_4G_data_from_crm_lead_line.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/otrs_factories/test_update_ticket_with_error.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/otrs_factories/test_update_ticket_with_error.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/sc_test_case.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/sc_test_case.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_process/base_test_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_process/base_test_contract_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_process/test_fiber_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_process/test_fiber_contract_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,17 +101,15 @@
         self, mock_relate_with_mobile, SetFiberContractCodeMock,
         UnblockMobilePackTicketMock, *args
     ):
         pack_code = self.browse_ref(
             "somconnexio.TrucadesIllimitades20GBPack"
         ).default_code
         new_ticket_number = "123454321"
-        crm_lead = crm_lead_create(
-            self.env, self.partner, "fiber", portability=False, pack=True
-        )
+        crm_lead = crm_lead_create(self.env, self.partner, "pack", portability=False)
         for line in crm_lead.lead_line_ids:
             if line.product_id.default_code == pack_code:
                 line.ticket_number = new_ticket_number
             else:
                 line.ticket_number = self.ticket_number
         content = FiberContractProcess(self.env).create(**self.data)
         contract = self.env["contract.contract"].browse(content["id"])
@@ -136,14 +134,15 @@
 
         mock_relate_with_mobile.assert_called_once_with(
             {
                 "id": contract.id,
                 "code": contract.code,
                 "partner_id": contract.partner_id.id,
                 "ticket_number": contract.ticket_number,
+                "create_reason": contract.create_reason,
             }
         )
 
     @patch(
         "odoo.addons.somconnexio.services.get_activation_date.date",
         spec=["today"],
     )
@@ -189,17 +188,15 @@
             },
         )
 
         pack_code = self.browse_ref(
             "somconnexio.TrucadesIllimitades20GBPack"
         ).default_code
         new_ticket_number = "123454321"
-        crm_lead = crm_lead_create(
-            self.env, self.partner, "fiber", portability=False, pack=True
-        )
+        crm_lead = crm_lead_create(self.env, self.partner, "pack", portability=False)
         for line in crm_lead.lead_line_ids:
             if line.product_id.default_code == pack_code:
                 line.ticket_number = new_ticket_number
             else:
                 line.ticket_number = self.ticket_number
         content = FiberContractProcess(self.env).create(**self.data)
         contract = self.env["contract.contract"].browse(content["id"])
@@ -222,14 +219,15 @@
 
         mock_relate_with_mobile.assert_called_once_with(
             {
                 "id": contract.id,
                 "code": contract.code,
                 "partner_id": contract.partner_id.id,
                 "ticket_number": contract.ticket_number,
+                "create_reason": contract.create_reason,
             }
         )
 
     @patch(
         "odoo.addons.somconnexio.services.contract_process.fiber.UnblockMobilePackTicket"  # noqa
     )
     @patch(
@@ -243,15 +241,18 @@
         UnblockMobilePackTicketMock, *args
     ):
         no_pack_product = self.browse_ref(
             "somconnexio.TrucadesIllimitades20GB"
         )
         new_ticket_number = "123454321"
         crm_lead = crm_lead_create(
-            self.env, self.partner, "fiber", portability=False, pack=True
+            self.env,
+            self.partner,
+            "pack",
+            portability=False,
         )
         for line in crm_lead.lead_line_ids:
             if line.is_mobile:
                 line.product_id = no_pack_product.id
                 line.ticket_number = new_ticket_number
             else:
                 line.ticket_number = self.ticket_number
@@ -268,14 +269,15 @@
 
         mock_relate_with_mobile.assert_called_once_with(
             {
                 "id": contract.id,
                 "code": contract.code,
                 "partner_id": contract.partner_id.id,
                 "ticket_number": contract.ticket_number,
+                "create_reason": contract.create_reason,
             }
         )
 
     @patch(
         "odoo.addons.somconnexio.services.contract_process.fiber.UnblockMobilePackTicket"  # noqa
     )
     @patch(
@@ -285,15 +287,18 @@
         "odoo.addons.somconnexio.services.contract_process.fiber.FiberContractProcess._relate_new_fiber_with_existing_mobile_contracts"  # noqa
     )
     def test_create_fiber_unblock_shared_mobile_tickets(
         self, mock_relate_with_mobile, SetFiberContractCodeMock,
         UnblockMobilePackTicketMock, *args
     ):
         crm_lead = crm_lead_create(
-            self.env, self.partner, "fiber", portability=False, pack=True
+            self.env,
+            self.partner,
+            "pack",
+            portability=False,
         )
         crm_lead_line = crm_lead.lead_line_ids.filtered("is_mobile").copy()
         crm_lead.write({"crm_lead_lines": [(4, crm_lead_line.id, 0)]})
         shared_product = self.browse_ref(
             "somconnexio.50GBCompartides2mobils"
         )
         first_ticket_number = "123456"
@@ -340,14 +345,15 @@
 
         mock_relate_with_mobile.assert_called_once_with(
             {
                 "id": contract.id,
                 "code": contract.code,
                 "partner_id": contract.partner_id.id,
                 "ticket_number": contract.ticket_number,
+                "create_reason": contract.create_reason,
             }
         )
 
     def _get_introduced_date(self, activation_date):
         introduced_date = activation_date - timedelta(days=2)
         while not introduced_date.weekday() < 5:  # 5 Sat, 6 Sun
             introduced_date = introduced_date - timedelta(days=1)
@@ -545,26 +551,62 @@
         CRM also has a mobile pack petition, no change is done
         """
 
         # Create packable mobile contract
         self.env['contract.contract'].create(self.vals_mobile_contract)
 
         crm_lead = crm_lead_create(
-            self.env, self.partner, "fiber", portability=False, pack=True
+            self.env,
+            self.partner,
+            "pack",
+            portability=False,
         )
         fiber_lead_line = crm_lead.lead_line_ids.filtered('is_fiber')
         fiber_lead_line.ticket_number = self.ticket_number
 
         FiberContractProcess(self.env).create(**self.data)
 
         mock_send_email.assert_not_called()
         mock_change_tariff_create.assert_not_called()
         mock_update_pack_mobile_tickets.assert_called_once()
 
     @patch(
+        "odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ContractMobileTariffChangeWizard.button_change"  # noqa
+    )
+    @patch(
+        "odoo.addons.somconnexio.services.contract_process.fiber.FiberContractProcess._update_pack_mobile_tickets"  # noqa
+    )
+    @patch('odoo.addons.mail.models.mail_template.MailTemplate.send_mail')
+    def test_relate_with_one_mobile_contract_location_change_case(
+        self, mock_send_email, mock_update_pack_mobile_tickets,
+        mock_change_tariff_create, *args
+    ):
+        """
+        Check that if a location_change fiber is created no mobile contract
+        is related with it
+        """
+
+        crm_lead = crm_lead_create(
+            self.env, self.partner, "pack", portability=False
+        )
+        fiber_lead_line = crm_lead.lead_line_ids.filtered('is_fiber')
+        fiber_lead_line.ticket_number = self.ticket_number
+        fiber_lead_line.create_reason = "location_change"
+
+        # Create packable mobile contract
+        self.env['contract.contract'].create(self.vals_mobile_contract)
+
+        contract = FiberContractProcess(self.env).create(**self.data)
+
+        mock_send_email.assert_not_called()
+        mock_change_tariff_create.assert_not_called()
+        mock_update_pack_mobile_tickets.assert_called_once()
+        self.assertEquals(contract["create_reason"], "location_change")
+
+    @patch(
         "odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ContractMobileTariffChangeWizard.create",  # noqa
         return_value=Mock(spec=['button_change'])
     )
     @patch(
         "odoo.addons.somconnexio.services.contract_process.fiber.FiberContractProcess._update_pack_mobile_tickets"  # noqa
     )
     @patch('odoo.addons.mail.models.mail_template.MailTemplate.send_mail')
@@ -581,24 +623,21 @@
 
         non_pack_mbl_product = self.browse_ref('somconnexio.150Min1GB')
         pack_mobile_product_id = self.browse_ref(
             "somconnexio.TrucadesIllimitades20GBPack"
         ).id
 
         # Create packable mobile contract
-        mbl_contract = self.env['contract.contract'].create(
-            self.vals_mobile_contract
-        )
-        crm_lead = crm_lead_create(
-            self.env, self.partner, "fiber", portability=False, pack=True
-        )
-        fiber_lead_line = crm_lead.lead_line_ids.filtered('is_fiber')
+        mbl_contract = self.env["contract.contract"].create(self.vals_mobile_contract)
+        crm_lead = crm_lead_create(self.env, self.partner, "pack", portability=False)
+        fiber_lead_line = crm_lead.lead_line_ids.filtered("is_fiber")
         fiber_lead_line.ticket_number = self.ticket_number
-        mobile_lead_line = crm_lead.lead_line_ids.filtered(
-            "is_mobile").filtered("is_from_pack")
+        mobile_lead_line = crm_lead.lead_line_ids.filtered("is_mobile").filtered(
+            "is_from_pack"
+        )
         mobile_lead_line.product_id = non_pack_mbl_product.id
 
         content = FiberContractProcess(self.env).create(**self.data)
 
         mock_change_tariff_create.assert_called_once_with(
             {
                 "summary": "Automatic mobile tariff change",
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_process/test_mobile_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_process/test_mobile_contract_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,15 +95,18 @@
     @patch(
         "odoo.addons.somconnexio.services.contract_process.fiber.SetFiberContractCodeMobileTicket"  # noqa
     )
     def test_create_mobile_pack_contract_link_parent_contract(
         self, *args
     ):
         crm_lead = crm_lead_create(
-            self.env, self.partner, "fiber", portability=False, pack=True
+            self.env,
+            self.partner,
+            "pack",
+            portability=False,
         )
         for line in crm_lead.lead_line_ids:
             if line.product_id.default_code == self.pack_code:
                 line.ticket_number = self.mobile_ticket_number
             else:
                 line.ticket_number = self.fiber_ticket_number
 
@@ -133,15 +136,18 @@
     @patch(
         "odoo.addons.somconnexio.services.contract_process.fiber.SetFiberContractCodeMobileTicket"  # noqa
     )
     def test_create_mobile_pack_contract_link_with_contract_line(
         self, *args
     ):
         crm_lead = crm_lead_create(
-            self.env, self.partner, "fiber", portability=False, pack=True
+            self.env,
+            self.partner,
+            "pack",
+            portability=False,
         )
         for line in crm_lead.lead_line_ids:
             if line.product_id.default_code == self.pack_code:
                 line.ticket_number = self.mobile_ticket_number
             else:
                 line.ticket_number = self.fiber_ticket_number
 
@@ -172,15 +178,18 @@
     @patch(
         "odoo.addons.somconnexio.services.contract_process.fiber.UnblockMobilePackTicket"  # noqa
     )
     def test_raise_error_if_not_found_parent_pack_contract(
         self, *args
     ):
         crm_lead = crm_lead_create(
-            self.env, self.partner, "fiber", portability=False, pack=True
+            self.env,
+            self.partner,
+            "pack",
+            portability=False,
         )
         for line in crm_lead.lead_line_ids:
             if line.product_id.default_code == self.pack_code:
                 line.ticket_number = self.mobile_ticket_number
             else:
                 line.ticket_number = self.fiber_ticket_number
         mobile_content = self.data
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_contract_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_contract_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import json
+from datetime import date, timedelta
+
 import odoo
 from faker import Faker
-from ...common_service import BaseEMCRestCaseAdmin
-from datetime import date, timedelta
 from mock import patch
-from ....services.contract_contract_process import ContractContractProcess, \
-    ErrorUnsuportedTechnology
 from odoo.exceptions import UserError
+
+from ....services.contract_contract_process import (
+    ContractContractProcess,
+    ErrorUnsuportedTechnology,
+)
+from ...common_service import BaseEMCRestCaseAdmin
+
 HOST = "127.0.0.1"
 PORT = odoo.tools.config["http_port"]
 
 
 @patch("pyopencell.resources.subscription.Subscription.get")
 @patch("odoo.addons.somconnexio.models.contract.CRMAccountHierarchyFromContractCreateService")  # noqa
 class TestContractController(BaseEMCRestCaseAdmin):
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_count_controller.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_count_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,23 @@
 class TestContractCountController(BaseEMCRestCaseAdmin):
 
     def setUp(self, *args, **kwargs):
         super().setUp(*args, **kwargs)
         self.Contract = self.env['contract.contract']
         self.Partner = self.env['res.partner']
         vodafone_fiber_contract_service_info = self.env[
-            'vodafone.fiber.service.contract.info'
-        ].create({
-            'phone_number': '654321123',
-            'vodafone_id': '123',
-            'vodafone_offer_code': '456',
-        })
-        partner = self.browse_ref('somconnexio.res_partner_2_demo')
+            "vodafone.fiber.service.contract.info"
+        ].create(
+            {
+                "phone_number": "654321123",
+                "vodafone_id": "123",
+                "vodafone_offer_code": "456",
+            }
+        )
+        partner = self.browse_ref("somconnexio.res_partner_1_demo")
         partner_id = partner.id
         service_partner = self.env['res.partner'].create({
             'parent_id': partner_id,
             'name': 'Partner service OK',
             'type': 'service'
         })
         product_ref = self.browse_ref('somconnexio.Fibra100Mb')
@@ -75,34 +77,34 @@
             'state': 'done'
         }
 
     def test_route_count_one_contract_active(self, *args):
         url = "/public-api/contract-count"
         count_contract = self.env['contract.contract'].search_count([])
         self.Contract.unlink()
-        self.assertEquals(count_contract, 0)
+        self.assertEquals(count_contract, 7)  # 7 demo data contracts
         self.Contract.create(self.vals_contract)
         response = self.http_get(url)
         self.assertEquals(response.status_code, 200)
         decoded_response = json.loads(response.content.decode("utf-8"))
         self.assertIn('contracts', decoded_response)
-        self.assertEquals(decoded_response["contracts"], 1)
+        self.assertEquals(decoded_response["contracts"], 8)  # +1
 
     def test_route_doesnt_count_one_contract_terminated(self, *args):
         url = "/public-api/contract-count"
         count_contract = self.env['contract.contract'].search_count([])
         self.Contract.unlink()
-        self.assertEquals(count_contract, 0)
+        self.assertEquals(count_contract, 7)  # 7 demo data contracts
         self.vals_contract['is_terminated'] = True
         self.Contract.create(self.vals_contract)
         response = self.http_get(url)
         self.assertEquals(response.status_code, 200)
         decoded_response = json.loads(response.content.decode("utf-8"))
         self.assertIn('contracts', decoded_response)
-        self.assertEquals(decoded_response["contracts"], 0)
+        self.assertEquals(decoded_response["contracts"], 7)  # +0
 
     def test_route_count_one_member(self, *args):
         url = "/public-api/contract-count"
         response = self.http_get(url)
         self.assertEquals(response.status_code, 200)
         decoded_response = json.loads(response.content.decode("utf-8"))
         self.assertIn('members', decoded_response)
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/contract_services/test_contract_get_fiber_contracts_to_pack_controller.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/contract_services/test_contract_get_fiber_contracts_to_pack_controller.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_account_invoice_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_account_invoice_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_change_partner_emails.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_change_partner_emails.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_contract_change_tariff_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_contract_change_tariff_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_contract_contract_process.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_contract_contract_process.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_contract_email_change_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_contract_email_change_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_contract_iban_change_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_contract_iban_change_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_contract_one_shot_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_contract_one_shot_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_crm_lead_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_crm_lead_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_discovery_channel_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_discovery_channel_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_get_activation_date.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_get_activation_date.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_mass_mailing_unsubscribe.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_mass_mailing_unsubscribe.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_partner_email_change_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_partner_email_change_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_product_catalog_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_product_catalog_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 
 
 class TestProductCatalogController(BaseEMCRestCaseAdmin):
 
     def setUp(self):
         super().setUp()
         self.url = "/api/product-catalog"
-        self.code = "0IVA"
-        self.demo_pricelist = self.browse_ref('somconnexio.pricelist_without_IVA')
+        self.code = "21IVA"
+        self.url_with_code = "{}?code={}".format(self.url, self.code)
+        self.demo_pricelist = self.browse_ref("somconnexio.pricelist_21_IVA")
 
         # Mobile product
         self.mbl_product = self.browse_ref('somconnexio.150Min1GB')
         self.mbl_product.product_tmpl_id.catalog_attribute_id = (
             self.browse_ref('somconnexio.150Min')
         )
         self.mbl_product.product_tmpl_id.catalog_attribute_id.catalog_name = (
@@ -105,19 +106,18 @@
         self.assertEquals(response.status_code, 200)
         self.assertEquals(response.reason, "OK")
 
     def test_price_list_count(self):
         response = self.http_get(self.url)
         content = json.loads(response.content.decode("utf-8"))
 
-        # DEMO pricelist 'pricelist_without_IVA'
-        self.assertEqual(len(content["pricelists"]), 1)
+        self.assertEqual(len(content["pricelists"]), 2)
 
     def test_price_list_content(self):
-        response = self.http_get(self.url)
+        response = self.http_get(self.url_with_code)
         content = json.loads(response.content.decode("utf-8"))
 
         obtained_pricelist = content.get("pricelists")[0].get('products')
         service_products = self._get_service_products()
 
         self.assertEqual(
             len(service_products),
@@ -146,15 +146,15 @@
             ("categ_id", '=', self.env.ref('somconnexio.mobile_service').id)
         ])
         mobile_products = self.env["product.product"].search([
             ("product_tmpl_id", 'in', [tmpl.id for tmpl in mobile_products_templ_ids]),
             ("public", '=', True)
         ])
 
-        response = self.http_get("{}?categ=mobile".format(self.url))
+        response = self.http_get("{}&categ=mobile".format(self.url_with_code))
         content = json.loads(response.content.decode("utf-8"))
         obtained_pricelists = content.get("pricelists")
         obtained_mobile_catalog = obtained_pricelists[0].get("products")
         self.assertEqual(len(obtained_pricelists), 1)
         self.assertEqual(len(obtained_mobile_catalog), len(mobile_products))
         self.assertEqual(obtained_mobile_catalog[0]["category"], "mobile")
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_provider_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_provider_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_res_partner_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_res_partner_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_subscription_request_service.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_subscription_request_service.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/services/test_vat_normalizer.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/services/test_vat_normalizer.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/somoffice/test_user.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/somoffice/test_user.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_account_payment_line_create.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_account_payment_line_create.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_address_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_address_change_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_compensation_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_compensation_wizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,18 +44,18 @@
             ),
             'vodafone_fiber_service_contract_info_id': (
                 self.vodafone_fiber_contract_service_info.id
             ),
             'bank_id': self.partner.bank_ids.id,
             'contract_line_ids': [(0, 0, contract_line)],
         }
-        self.contract = self.env['contract.contract'].create(vals_contract)
-        self.pricelist_item = self.env["product.pricelist.item"].search(
-            [('product_id', '=', self.product.id)]
-        )
+        self.contract = self.env["contract.contract"].create(vals_contract)
+        self.pricelist_item = self.browse_ref(
+            "somconnexio.pricelist_without_IVA"
+        ).item_ids.filtered(lambda i: i.product_id == self.product)
         self.price = self.pricelist_item.fixed_price
         self.days_without_service = 2.0
         self.tax = self.env['account.tax'].search([
             ('name', '=', 'IVA 21% (Servicios)')
         ])
         self.tax.code = 'TAX_HIGH'
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_force_oc_integration_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_force_oc_integration_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_holder_change.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_holder_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_force_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_force_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_iban_change_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_invoice_payment_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_invoice_payment_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_mobile_tariff_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,228 +1,310 @@
-from mock import patch
-from datetime import date, datetime, timedelta
-
-from ...helpers.date import first_day_next_month, date_to_str
-from ..sc_test_case import SCTestCase
-from odoo.exceptions import ValidationError, MissingError
-
-
-class TestContractTariffChangeWizard(SCTestCase):
-
-    def setUp(self, *args, **kwargs):
-        super().setUp(*args, **kwargs)
-        self.user_admin = self.browse_ref('base.user_admin')
-        self.partner_id = self.browse_ref('somconnexio.res_partner_2_demo')
-        partner_id = self.partner_id.id
-        service_partner = self.env['res.partner'].create({
-            'parent_id': partner_id,
-            'name': 'Service partner',
-            'type': 'service'
-        })
-        masmovil_mobile_contract_service_info = self.env[
-            'mobile.service.contract.info'
-        ].create({
-            'phone_number': '654321123',
-            'icc': '123',
-        })
-        product = self.env.ref("somconnexio.TrucadesIllimitades20GB")
-        self.new_product = self.env.ref("somconnexio.150Min1GB")
-        contract_line = {
-            "name": product.name,
-            "product_id": product.id,
-            "date_start": datetime.now() - timedelta(days=12),
-        }
-        vals_contract = {
-            'name': 'Test Contract Broadband',
-            'partner_id': partner_id,
-            'service_partner_id': service_partner.id,
-            'invoice_partner_id': partner_id,
-            'service_technology_id': self.ref(
-                "somconnexio.service_technology_mobile"
-            ),
-            'service_supplier_id': self.ref(
-                "somconnexio.service_supplier_masmovil"
-            ),
-            'mobile_contract_service_info_id': (
-                masmovil_mobile_contract_service_info.id
-            ),
-            "contract_line_ids": [(0, 0, contract_line)],
-            "email_ids": [(6, 0, [partner_id])],
-        }
-        self.contract = self.env["contract.contract"].create(vals_contract)
-
-    @patch("odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ChangeTariffTicket")  # noqa
-    @patch("odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ChangeTariffExceptionalTicket")  # noqa
-    @patch("odoo.addons.somconnexio.services.contract_contract_service.ContractService.get_fiber_contracts_to_pack")  # noqa
-    def test_wizard_mobile_tariff_change_ok(
-            self, mock_get_fiber_contracts_to_pack,
-            MockExceptionalChangeTariffTicket, MockChangeTariffTicket):
-
-        # No bonified mobile product available
-        mock_get_fiber_contracts_to_pack.side_effect = MissingError("")
-
-        wizard = self.env['contract.mobile.tariff.change.wizard'].with_context(  # noqa
-            active_id=self.contract.id
-        ).sudo(
-            self.user_admin
-        ).create({
-            "summary": "test",
-            "new_tariff_product_id": self.new_product.id,
-            "otrs_checked": True,
-        })
-
-        partner_activities_before = self.env['mail.activity'].search(
-            [('partner_id', '=', self.partner_id.id)]
-        )
-        wizard.button_change()
-
-        partner_activities_after = self.env['mail.activity'].search(
-            [('partner_id', '=', self.partner_id.id)],
-        )
-
-        expected_start_date = first_day_next_month()
-        self.assertEquals(len(partner_activities_after) -
-                          len(partner_activities_before), 1)
-        created_activity = partner_activities_after[-1]
-        self.assertEquals(created_activity.user_id, self.user_admin)
-        self.assertEquals(
-            created_activity.activity_type_id,
-            self.browse_ref('somconnexio.mail_activity_type_tariff_change')
+from datetime import date, timedelta
+from odoo import models, fields, api, _
+from odoo.exceptions import MissingError
+
+from ...services.contract_contract_service import ContractService
+
+
+class ContractHolderChangeWizard(models.TransientModel):
+    _name = 'contract.holder.change.wizard'
+    partner_id = fields.Many2one(
+        'res.partner',
+        string='Partner',
+        required=True,
+    )
+    contract_id = fields.Many2one('contract.contract')
+    change_date = fields.Date('Change Date', required=True)
+    payment_mode = fields.Many2one(
+        'account.payment.mode',
+        string='Payment mode',
+        required=True,
+    )
+    banking_mandate_required = fields.Boolean(
+        related="payment_mode.payment_method_id.bank_account_required"
+    )
+    available_banking_mandates = fields.Many2many(
+        'account.banking.mandate',
+        compute="_compute_available_banking_mandates"
+    )
+    banking_mandate_id = fields.Many2one(
+        'account.banking.mandate',
+        string='Banking mandate',
+    )
+    email_ids = fields.Many2many(
+        'res.partner',
+        string='Emails',
+        required=True,
+    )
+    available_email_ids = fields.Many2many(
+        "res.partner", string="Available Emails", compute="_compute_available_email_ids"
+    )
+    notes = fields.Text(
+        string='Notes',
+    )
+    has_mobile_pack_offer_text = fields.Selection(
+        [("yes", _("Yes")), ("no", "No")],
+        string="Is mobile pack offer available?",
+        compute="_compute_has_mobile_pack_offer_text",
+        readonly=True,
+    )
+    available_products = fields.Many2many(
+        "product.product",
+        compute="_compute_available_products",
+    )
+    fiber_contract_to_link = fields.Many2one(
+        "contract.contract",
+        string="Fiber contract to link",
+        compute="_compute_fiber_contract_to_link"
+    )
+    product_id = fields.Many2one(
+        "product.product",
+        string="Product",
+        required=True,
+    )
+
+    @api.model
+    def default_get(self, fields_list):
+        defaults = super().default_get(fields_list)
+        defaults["contract_id"] = self.env.context["active_id"]
+        contract = self.env["contract.contract"].browse(self.env.context["active_id"])
+        defaults["payment_mode"] = self.env.ref(
+            "somconnexio.payment_mode_inbound_sepa"
+        ).id
+        defaults["change_date"] = date.today()
+        defaults["product_id"] = contract.current_tariff_product.id
+        return defaults
+
+    @api.depends("partner_id")
+    def _compute_available_email_ids(self):
+        if self.partner_id:
+            self.available_email_ids = [
+                (6, 0, self.partner_id.get_available_email_ids())
+            ]
+
+    @api.multi
+    @api.depends("partner_id")
+    def _compute_available_banking_mandates(self):
+        if self.partner_id:
+            partner_mandates = self.env['account.banking.mandate'].search([
+                ('partner_id', '=', self.partner_id.id),
+            ])
+            self.available_banking_mandates = partner_mandates
+
+    @api.multi
+    @api.depends("partner_id")
+    def _compute_fiber_contract_to_link(self):
+        if self.partner_id:
+            service = ContractService(self.env)
+            try:
+                fiber_contracts = service.get_fiber_contracts_to_pack(
+                    partner_ref=self.partner_id.ref
+                )
+            except MissingError:
+                self.fiber_contract_to_link = False
+            else:
+                self.fiber_contract_to_link = fiber_contracts[0]["id"]
+
+    @api.depends("fiber_contract_to_link")
+    def _compute_has_mobile_pack_offer_text(self):
+        self.has_mobile_pack_offer_text = "yes" if self.fiber_contract_to_link else "no"
+
+    @api.depends("fiber_contract_to_link")
+    def _compute_available_products(self):
+        old_contract_category = (
+            self.contract_id.current_tariff_product.product_tmpl_id.categ_id
         )
-        self.assertEquals(created_activity.done, True)
-        self.assertEquals(created_activity.summary, "test")
-
-        # Check NO bonified product available
-        self.assertIn(
-            "('attribute_value_ids', '!=', " +
-            str(self.env.ref('somconnexio.IsInPack').id) + ")",
-            wizard.product_domain
+        product_templates = self.env["product.template"].search(
+            [
+                ("categ_id", "=", old_contract_category.id),
+            ]
         )
-        self.assertEquals(wizard.start_date, expected_start_date)
-        MockChangeTariffTicket.assert_called_once_with(
-            self.partner_id.vat,
-            self.partner_id.ref,
-            {
-                "phone_number": self.contract.phone_number,
-                "new_product_code": self.new_product.default_code,
-                "current_product_code": self.contract.current_tariff_product.default_code,  # noqa
-                "effective_date": date_to_str(expected_start_date),
-                "subscription_email": self.partner_id.email,
-                "language": self.partner_id.lang,
-                "fiber_linked": False,
-                "send_notification": False,
-            },
+        product_search_domain = [
+            ("product_tmpl_id", "in", product_templates.ids),
+            ("public", "=", "True"),
+        ]
+        if (
+            old_contract_category == self.env.ref('somconnexio.mobile_service')
+            and self.fiber_contract_to_link
+                ):
+            product_search_domain = product_search_domain[:-1]
+            product_search_domain.extend(
+                [
+                    "|",
+                    (
+                        "attribute_value_ids",
+                        "=",
+                        self.env.ref("somconnexio.IsInPack").id,
+                    ),
+                    ("public", "=", "True"),
+                ]
+            )
+        self.available_products = self.env['product.product'].search(
+            product_search_domain
         )
-        MockChangeTariffTicket.return_value.create.assert_called_once()
-        MockExceptionalChangeTariffTicket.assert_not_called()
 
-    @patch("odoo.addons.somconnexio.services.contract_contract_service.ContractService.get_fiber_contracts_to_pack")  # noqa
-    def test_wizard_mobile_tariff_change_not_checked(
-            self, mock_get_fiber_contracts_to_pack):
-
-        mock_get_fiber_contracts_to_pack.side_effect = MissingError("")
-
-        wizard = self.env['contract.mobile.tariff.change.wizard'].with_context(  # noqa
-            active_id=self.contract.id
-        ).sudo(
-            self.user_admin
-        ).create({
-            "summary": "test",
-            "new_tariff_product_id": self.new_product.id,
+    @api.multi
+    def button_change(self):
+        self.ensure_one()
+        crm_lead_line = self._create_new_crm_lead_line()
+        new_contract = self._create_new_contract(crm_lead_line)
+        self._terminate_contract(new_contract)
+        return True
+
+    def _get_or_create_service_partner_id(self):
+
+        service_partner = self.env['res.partner'].search([
+            ('parent_id', '=', self.partner_id.id),
+            ('type', '=', 'service'),
+            ('street', 'ilike', self.contract_id.service_partner_id.street),
+        ], limit=1)
+
+        if not service_partner:
+            service_partner = self.env['res.partner'].create({
+                'parent_id': self.partner_id.id,
+                'name': 'New partner service',
+                'type': 'service',
+                'street': self.contract_id.service_partner_id.street,
+                'street2': self.contract_id.service_partner_id.street2,
+                'city': self.contract_id.service_partner_id.city,
+                'zip': self.contract_id.service_partner_id.zip,
+                'state_id': self.contract_id.service_partner_id.state_id.id,
+                'country_id': self.contract_id.service_partner_id.country_id.id,
+            })
+
+        return service_partner
+
+    def _create_new_crm_lead_line(self):
+        isp_info_params = {
+            "type": "holder_change",
+            "phone_number": self.contract_id.phone_number,
+        }
+        line_params = {
+            "name": self.contract_id.current_tariff_product.name,
+            "product_id": self.product_id.id,
+            "product_tmpl_id": self.contract_id.current_tariff_product.product_tmpl_id.id,  # noqa
+            "category_id": self.contract_id.current_tariff_product.product_tmpl_id.categ_id.id,  # noqa
+        }
+        if self.contract_id.is_broadband:
+            broadband_isp_info = self.env["broadband.isp.info"].create(isp_info_params)
+            line_params.update({"broadband_isp_info": broadband_isp_info.id})
+        else:
+            if (self.contract_id.is_mobile and self.fiber_contract_to_link and
+                    self.product_id.product_is_pack_exclusive):
+                isp_info_params[
+                    "linked_fiber_contract_id"
+                ] = self.fiber_contract_to_link.id
+            mobile_isp_info = self.env["mobile.isp.info"].create(isp_info_params)
+            line_params.update({"mobile_isp_info": mobile_isp_info.id})
+
+        crm_lead_line = self.env["crm.lead.line"].create(line_params)
+
+        self.env['crm.lead'].create({
+            "name": _("Change Holder process"),
+            "description": self.notes,
+            "partner_id": self.partner_id.id,
+            "lead_line_ids": [(6, 0, [crm_lead_line.id])],
+            "iban": self.banking_mandate_id.partner_bank_id.sanitized_acc_number,
+            "stage_id": self.env.ref("crm.stage_lead4").id
         })
+        return crm_lead_line
 
-        self.assertRaisesRegex(
-            ValidationError,
-            "You must check if any previous tariff change is found in OTRS",
-            wizard.button_change
-        )
-
-    @patch("odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ChangeTariffTicket")  # noqa
-    @patch("odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ChangeTariffExceptionalTicket")  # noqa
-    @patch("odoo.addons.somconnexio.services.contract_contract_service.ContractService.get_fiber_contracts_to_pack")  # noqa
-    def test_wizard_mobile_tariff_change_bonified_product_ok(
-            self, mock_get_fiber_contracts_to_pack,
-            MockExceptionalChangeTariffTicket, MockChangeTariffTicket):
-
-        code = "828282"
-        # Bonified product available
-        mock_get_fiber_contracts_to_pack.return_value = [{"code": code}]
-
-        self.pack_product = self.env.ref("somconnexio.TrucadesIllimitades20GBPack")
-
-        wizard = self.env['contract.mobile.tariff.change.wizard'].with_context(  # noqa
-            active_id=self.contract.id
-        ).sudo(
-            self.user_admin
-        ).create({
-            "summary": "test",
-            "new_tariff_product_id": self.pack_product.id,
-            "otrs_checked": True,
-        })
-        wizard.button_change()
+    def _create_new_contract(self, crm_lead_line):
+        service_partner = self._get_or_create_service_partner_id()
+        new_contract_params = {
+            'partner_id': self.partner_id.id,
+            'service_partner_id': service_partner.id,
+            'payment_mode_id': self.payment_mode.id,
+            'mandate_id': self.banking_mandate_id.id,
+            'email_ids': [(6, 0, [email.id for email in self.email_ids])],
+            'journal_id': self.contract_id.journal_id.id,
+            'service_technology_id': self.contract_id.service_technology_id.id,
+            'service_supplier_id': self.contract_id.service_supplier_id.id,
+            'contract_line_ids': [
+                (0, 0, self._prepare_create_line(line))
+                for line in self.contract_id.contract_line_ids
+                if (
+                    (not line.date_end or line.date_end > date.today()) and
+                    line.product_id.categ_id not in (
+                        self.env.ref('somconnexio.mobile_oneshot_service'),
+                        self.env.ref('somconnexio.broadband_oneshot_service'),
+                        self.env.ref('somconnexio.broadband_oneshot_adsl_service'),
+                    )
+                )
+            ],
+            'crm_lead_line_id': crm_lead_line.id,
+        }
 
-        # Check bonified product available
-        self.assertNotIn(
-            "('attribute_value_ids', '!=', " +
-            str(self.env.ref('somconnexio.IsInPack').id) + ")",
-            wizard.product_domain
-        )
-        MockChangeTariffTicket.assert_called_once_with(
-            self.partner_id.vat,
-            self.partner_id.ref,
-            {
-                "phone_number": self.contract.phone_number,
-                "new_product_code": self.pack_product.default_code,
-                "current_product_code": self.contract.current_tariff_product.default_code,  # noqa
-                "effective_date": date_to_str(first_day_next_month()),
-                "subscription_email": self.partner_id.email,
-                "language": self.partner_id.lang,
-                "fiber_linked": code,
-                "send_notification": False,
-            },
+        # TODO: This code is duplicated in ContractServiceProcess
+        if self.contract_id.mobile_contract_service_info_id:
+            name_contract_info = "mobile_contract_service_info_id"
+        elif self.contract_id.adsl_service_contract_info_id:
+            name_contract_info = "adsl_service_contract_info_id"
+        elif self.contract_id.vodafone_fiber_service_contract_info_id:
+            name_contract_info = "vodafone_fiber_service_contract_info_id"
+        elif self.contract_id.mm_fiber_service_contract_info_id:
+            name_contract_info = "mm_fiber_service_contract_info_id"
+        elif self.contract_id.router_4G_service_contract_info_id:
+            name_contract_info = "router_4G_service_contract_info_id"
+        contract_info = getattr(self.contract_id, name_contract_info)
+        new_contract_params["name"] = contract_info.phone_number
+        new_contract_params[name_contract_info] = contract_info.copy().id
+
+        if (self.contract_id.is_mobile and self.fiber_contract_to_link and
+                self.product_id.product_is_pack_exclusive):
+            new_contract_params[
+                "parent_pack_contract_id"
+            ] = self.fiber_contract_to_link.id
+        return self.env["contract.contract"].create(new_contract_params)
+
+    def _terminate_contract(self, new_contract):
+        self.contract_id.terminate_contract(
+            self.env.ref('somconnexio.reason_holder_change'),
+            'New contract created with ID: {}\nNotes: {}'.format(
+                new_contract.id,
+                self.notes or ''
+            ),
+            self.change_date,
+            self.env.ref('somconnexio.user_reason_other'),
         )
-        MockChangeTariffTicket.return_value.create.assert_called_once()
-        MockExceptionalChangeTariffTicket.assert_not_called()
-
-    @patch("odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ChangeTariffTicket")  # noqa
-    @patch("odoo.addons.somconnexio.wizards.contract_mobile_tariff_change.contract_mobile_tariff_change.ChangeTariffExceptionalTicket")  # noqa
-    @patch("odoo.addons.somconnexio.services.contract_contract_service.ContractService.get_fiber_contracts_to_pack")  # noqa
-    def test_wizard_mobile_exceptional_tariff_change_ok(
-            self, mock_get_fiber_contracts_to_pack,
-            MockExceptionalChangeTariffTicket, MockChangeTariffTicket):
-
-        # No bonified mobile product available
-        mock_get_fiber_contracts_to_pack.side_effect = MissingError("")
-
-        wizard = self.env['contract.mobile.tariff.change.wizard'].with_context(  # noqa
-            active_id=self.contract.id
-        ).sudo(
-            self.user_admin
-        ).create({
-            "summary": "test",
-            "exceptional_change": True,
-            "new_tariff_product_id": self.new_product.id,
-            "send_notification": True,
-            "otrs_checked": True,
-        })
 
-        wizard.button_change()
+        message = _("""
+            Holder change wizard
+            New contract created with ID: {}
+            Notes: {}
+            """)
+        self.contract_id.message_post(
+            message.format(new_contract.id, self.notes or '')
+        )
 
-        expected_start_date = date.today()
+    def _prepare_create_line(self, line):
+        return {
+            "name": self.product_id.name,
+            "product_id": self.product_id.id,
+            "date_start": self.change_date + timedelta(days=1),
+        }
 
-        self.assertEquals(wizard.start_date, expected_start_date)
-        MockExceptionalChangeTariffTicket.assert_called_once_with(
-            self.partner_id.vat,
-            self.partner_id.ref,
-            {
-                "phone_number": self.contract.phone_number,
-                "new_product_code": self.new_product.default_code,
-                "current_product_code": self.contract.current_tariff_product.default_code,  # noqa
-                "effective_date": date_to_str(expected_start_date),
-                "subscription_email": self.partner_id.email,
-                "language": self.partner_id.lang,
-                "fiber_linked": False,
-                "send_notification": True,
-            },
-        )
-        MockExceptionalChangeTariffTicket.return_value.create.assert_called_once()
-        MockChangeTariffTicket.assert_not_called()
+    @api.onchange('partner_id')
+    def check_partner_id_change(self):
+        self.service_partner_id = False
+        self.bank_id = False
+        self.email_ids = False
+
+        if not self.partner_id:
+            partner_id_domain = []
+            bank_domain = []
+        else:
+            partner_id_domain = [
+                '|',
+                ('id', '=', self.partner_id.id),
+                ('parent_id', '=', self.partner_id.id)
+            ]
+            bank_domain = [
+                ('partner_id', '=', self.partner_id.id)
+            ]
+
+        return {
+            'domain': {
+                'service_partner_id': partner_id_domain,
+                'bank_id': bank_domain
+            }
+        }
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_one_shot_request_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_one_shot_request_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_tariff_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_tariff_change_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_contract_terminate_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_contract_terminate_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_create_lead_from_partner_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_create_lead_from_partner_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_create_subscription_from_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_create_subscription_from_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_crm_lead_generate_SIM_delivery_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_crm_lead_generate_SIM_delivery_wizard.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from ..sc_test_case import SCTestCase
 
 
 class TestCRMLeadsGenerateSIMDeliveryWizard(SCTestCase):
 
     def setUp(self, *args, **kwargs):
         super().setUp(*args, **kwargs)
-        self.partner_id = self.browse_ref('somconnexio.res_partner_2_demo')
-        self.pack_crm_lead = crm_lead_create(self.env, self.partner_id, "fiber",
-                                             portability=True, pack=True)
+        self.partner_id = self.browse_ref("somconnexio.res_partner_2_demo")
+        self.pack_crm_lead = crm_lead_create(
+            self.env, self.partner_id, "pack", portability=True
+        )
 
     def test_wizard_OK(self):
 
         self.pack_crm_lead.action_set_remesa()
 
         wizard = self.env['crm.lead.generate.sim.delivery.wizard'].with_context(
             active_ids=[self.pack_crm_lead.id]
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_crm_lead_remesa_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_crm_lead_remesa_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_crm_leads_validate_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_crm_leads_validate_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_mail_compose_message_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_mail_compose_message_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_partner_check_somoffice_email.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_partner_check_somoffice_email.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_partner_email_change_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_partner_email_change_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/tests/wizards/test_payment_order_generated_to_upload_queued_wizard.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/tests/wizards/test_payment_order_generated_to_upload_queued_wizard.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/account_asset_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/account_asset_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/account_invoice_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/account_invoice_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/account_move.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/account_move.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/account_move_line.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/account_move_line.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/account_payment_order_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/account_payment_order_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/adsl_service_contract_info_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/adsl_service_contract_info_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/aeat_report_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/aeat_report_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/broadband_isp_info_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/broadband_isp_info_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/contract_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/contract_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/coop_agreement_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/coop_agreement_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/crm_lead.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/crm_lead.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/crm_lead_line.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/crm_lead_line.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/hr_attendance.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/hr_attendance.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/ir_action_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/ir_action_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/mail_activity_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/mail_activity_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/mail_mail_statistics_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/mail_mail_statistics_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/menus.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/menus.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/mis_budget_item_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/mis_budget_item_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/mm_fiber_service_contract_info.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/mm_fiber_service_contract_info.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/mobile_isp_info_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/mobile_isp_info_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/mobile_service_contract_info_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/mobile_service_contract_info_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/open_boards_activities.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/open_boards_activities.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/operation_request.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/operation_request.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/partner_action_tag_views.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/partner_action_tag_views.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/payment_return_import_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/payment_return_import_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/payment_return_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/payment_return_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/previous_provider_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/previous_provider_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/product_attribute_views.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/product_attribute_views.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/product_category_technology_supplier_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/product_category_technology_supplier_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/product_pricelist_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/product_pricelist_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/product_product_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/product_product_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/res_company_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/res_company_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/res_partner_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/res_partner_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/router_4G_service_contract_info.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/router_4G_service_contract_info.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/service_technology_service_supplier.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/service_technology_service_supplier.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/stock_move_line_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/stock_move_line_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/subscription_request_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/subscription_request_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/templates_js.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/templates_js.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/vodafone_fiber_service_contract_info.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/vodafone_fiber_service_contract_info.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/views/xoln_fiber_service_contract_info.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/views/xoln_fiber_service_contract_info.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/__init__.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/__init__.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_financial_report/aged_partner_balance.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_financial_report/general_ledger.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_invoice_confirm/account_invoice_confirm.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_invoice_confirm/account_invoice_confirm.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create_view.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/account_payment_line_create/account_payment_line_create_view.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_address_change/contract_address_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_compensation/contract_compensation.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_force_oc_integration/contract_force_oc_integration.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_holder_change/contract_holder_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_iban_change/contract_iban_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_iban_change_force/contract_iban_change_force.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_invoice_payment/contract_invoice_payment.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,124 +1,129 @@
-from datetime import date
-from otrs_somconnexio.otrs_models.ticket_types.change_tariff_ticket import (
-    ChangeTariffTicket, ChangeTariffExceptionalTicket
-)
-
-from odoo import fields, api, _
-from odoo.exceptions import MissingError, ValidationError
-
-from ...services.contract_contract_service import ContractService
-from ..contract_tariff_change.contract_tariff_change import (
-    ContractTariffChangeWizard)
-from ...helpers.date import first_day_next_month, date_to_str
-
-
-class ContractMobileTariffChangeWizard(ContractTariffChangeWizard):
-    _name = 'contract.mobile.tariff.change.wizard'
-
-    fiber_contract_code_to_link = fields.Char()
-    has_mobile_pack_offer_text = fields.Selection(
-        [('yes', _('Yes')), ('no', 'No')],
-        string='Is mobile pack offer available?',
-        readonly=True
+from datetime import datetime, date
+from calendar import monthrange
+
+from odoo import models, fields, api, _
+from odoo.addons.queue_job.job import job
+from ...services.contract_one_shot_process import ContractOneShotProcess
+
+
+class ContractOneShotRequestWizard(models.TransientModel):
+    _name = 'contract.one.shot.request.wizard'
+    contract_id = fields.Many2one('contract.contract')
+    summary = fields.Char(required=True)
+    done = fields.Boolean(required=True)
+    location = fields.Char()
+    note = fields.Char()
+
+    product_category_id = fields.Many2one(
+        'product.category',
+        compute="_load_product_category_id"
     )
-    new_tariff_product_id = fields.Many2one(
+    start_date = fields.Date('Start Date', required=True)
+    one_shot_product_id = fields.Many2one(
         'product.product',
-        string='New tariff',
-        required=True
-    )
-    exceptional_change = fields.Boolean(default=False)
-    send_notification = fields.Boolean(
-        string='Send notification', default=False
-    )
-    otrs_checked = fields.Boolean(
-        string='I have checked OTRS and no other tariff change is pending',
-        default=False,
-    )
-    product_domain = fields.Char()
-    location = fields.Char(
-        related='contract_id.phone_number'
+        string='One Shot products',
     )
+    activity_type = fields.Many2one('mail.activity.type')
 
     @api.model
     def default_get(self, fields_list):
         defaults = super().default_get(fields_list)
-        defaults['fiber_contract_code_to_link'] = \
-            self._default_fiber_contract_code_to_link(
-                self.env.context['active_id']
-            )
-        defaults['has_mobile_pack_offer_text'] = \
-            "yes" if defaults['fiber_contract_code_to_link'] else "no"
-        defaults['product_domain'] = self._default_product_domain(
-            defaults['fiber_contract_code_to_link']
-        )
+        defaults['contract_id'] = self.env.context['active_id']
+        defaults['start_date'] = datetime.strftime(date.today(), "%Y-%m-%d")
         return defaults
 
-    def _default_fiber_contract_code_to_link(self, contract_id):
-        contract = self.env["contract.contract"].browse(contract_id)
-        partner_ref = contract.partner_id.ref
-
-        service = ContractService(self.env)
-        try:
-            fiber_contracts = service.get_fiber_contracts_to_pack(
-                partner_ref=partner_ref)
-        except MissingError:
+    @api.depends("contract_id")
+    def _load_product_category_id(self):
+        if not self.contract_id:
             return False
+        if self.contract_id.is_mobile:
+            self.product_category_id = self.env.ref(
+                'somconnexio.mobile_oneshot_service').id
+        elif self.contract_id.service_technology_id == self.env.ref(
+            'somconnexio.service_technology_adsl'
+        ):
+            self.product_category_id = self.env.ref(
+                'somconnexio.broadband_oneshot_adsl_service'
+            ).id
         else:
-            return fiber_contracts[0]['code']
-
-    def _default_product_domain(self, has_mobile_pack_offer):
-        mbl_product_templates = self.env["product.template"].search([
-            ('categ_id', '=', self.env.ref('somconnexio.mobile_service').id),
-        ])
-        product_search_domain = [
-            ('product_tmpl_id', 'in', mbl_product_templates.ids),
-            ('active', '=', True),
-            ('attribute_value_ids', '!=', self.env.ref('somconnexio.IsInPack').id)
+            self.product_category_id = self.env.ref(
+                'somconnexio.broadband_oneshot_service'
+            ).id
+
+    @api.onchange("one_shot_product_id")
+    def onchange_one_shot_product_id(self):
+        router_list = [
+            self.env.ref('somconnexio.EnviamentRouter_product_template'),
+            self.env.ref('somconnexio.RecollidaRouter_product_template')
+        ]
+        one_shot_list = [
+            self.env.ref(
+                'somconnexio.SMSMassius500SMS_product_template'
+            ),
+            self.env.ref(
+                'somconnexio.DadesAddicionals1GBSenseCost_product_template'
+            )
         ]
-        if has_mobile_pack_offer:
-            del product_search_domain[-1]
-        return product_search_domain
-
-    def button_change(self):
-        self.ensure_one()
 
-        if not self.otrs_checked:
-            raise ValidationError(_(
-                "You must check if any previous tariff change is found in OTRS"
-            ))
-
-        partner = self.contract_id.partner_id
-
-        if self.exceptional_change:
-            self.start_date = date.today()
-            Ticket = ChangeTariffExceptionalTicket
+        if self.one_shot_product_id.product_tmpl_id in one_shot_list:
+            self.summary = ""
+            self.done = True
+            self.activity_type = self.env.ref('somconnexio.mail_activity_type_one_shot')
+        elif self.one_shot_product_id.product_tmpl_id in router_list:
+            self.summary = ""
+            self.done = True
+            self.activity_type = self.env.ref('somconnexio.mail_activity_type_router_send_or_return')  # noqa
         else:
-            self.start_date = first_day_next_month()
-            Ticket = ChangeTariffTicket
+            self.summary = ""
+            self.done = False
+            self.activity_type = self.env.ref('somconnexio.mail_activity_type_sim_change')  # noqa
 
-        fields_dict = {
-            "phone_number": self.contract_id.phone_number,
-            "new_product_code": self.new_tariff_product_id.default_code,
-            "current_product_code": self.current_tariff_product.default_code,
-            "subscription_email": self.contract_id.email_ids[0].email,
-            "effective_date": date_to_str(self.start_date),
-            "language": partner.lang,
-            "fiber_linked": False,
-            "send_notification": self.send_notification,
-        }
+    def button_add(self):
+        self.ensure_one()
 
-        if self.new_tariff_product_id.product_is_pack_exclusive:
-            fields_dict["fiber_linked"] = self.fiber_contract_code_to_link
+        one_shot_contract_line = {
+            "name": self.one_shot_product_id.name,
+            "product_id": self.one_shot_product_id.id,
+            "date_start": self.start_date,
+            "date_end": self._get_last_day_of_month(self.start_date)
+        }
 
-        Ticket(partner.vat, partner.ref, fields_dict).create()
+        self.contract_id.write(
+            {'contract_line_ids': [(0, 0, one_shot_contract_line)]}
+        )
 
-        message = _("OTRS change tariff ticket created. Tariff to be changed from '{}' to '{}' with start_date: {}")  # noqa
+        message = _("One shot product '{}' added on '{}'")
         self.contract_id.message_post(
             message.format(
-                self.current_tariff_contract_line.product_id.showed_name,
-                self.new_tariff_product_id.showed_name,
+                self.one_shot_product_id.showed_name,
                 self.start_date,
             )
         )
+
         self._create_activity()
         return True
+
+    def _get_last_day_of_month(self, request_date):
+        #  Touple with weekday (0-6) and number of days (28-31) for a given month
+        month_range = monthrange(request_date.year, request_date.month)
+
+        return date(request_date.year, request_date.month, month_range[1])
+
+    def _create_activity(self):
+        self.env['mail.activity'].create({
+            'summary': self.summary,
+            'res_id': self.contract_id.id,
+            'res_model_id': self.env.ref('contract.model_contract_contract').id,
+            'user_id': self.env.user.id,
+            'activity_type_id': self.activity_type.id,
+            'done': self.done,
+            'date_done': date.today(),
+            'date_deadline': date.today(),
+            'location': self.location,
+            'note': self.note,
+        })
+
+    @job
+    def run_from_api(self, **params):
+        service = ContractOneShotProcess(self.env)
+        service.run_from_api(**params)
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.xml`

 * *Files 12% similar despite different names*

#### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_mobile_tariff_change/contract_mobile_tariff_change.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.xml`

```diff
@@ -1,44 +1,41 @@
 <?xml version="1.0" encoding="utf-8"?>
 <odoo>
   <data>
-    <record id="view_form_contract_mobile_tariff_change_wizard" model="ir.ui.view">
-      <field name="name">Contract Mobile Tariff Change Wizard</field>
-      <field name="model">contract.mobile.tariff.change.wizard</field>
+    <record id="view_form_contract_tariff_change_wizard" model="ir.ui.view">
+      <field name="name">Contract Tariff Change Wizard</field>
+      <field name="model">contract.tariff.change.wizard</field>
       <field name="arch" type="xml">
         <form>
           <group>
             <field name="contract_id" invisible="1"/>
-            <field name="product_domain" invisible="1"/>
-            <field name="exceptional_change"/>
-            <field name="send_notification" attrs="{'invisible': [('exceptional_change','=',False)]}"/>
-            <separator/>
-            <field name="has_mobile_pack_offer_text" widget="Radio"/>
-            <field name="current_tariff_product" options="{'no_open': True,'no_create': 1,'no_create_edit': 1}"/>
-            <field name="new_tariff_product_id" domain="product_domain"/>
+            <field name="product_category_id" invisible="1"/>
+            <field name="current_tariff_product" options="{&quot;no_open&quot;: True,&quot;no_create&quot;: 1,&quot;no_create_edit&quot;: 1}"/>
+            <field name="new_tariff_product_id" domain="[('product_tmpl_id.categ_id.id', '=', product_category_id),                             ('custom_name', 'not ilike', context.get('ba') and 'borda'),                             ('name', 'not ilike', context.get('ba') and 'borda')]"/>
+            <field name="start_date"/>
             <field name="summary"/>
+            <field name="location"/>
+            <field name="done"/>
             <field name="note"/>
-            <separator/>
-            <!-- TODO: Remove confirm logic if check is done in OTRs-->
-            <field name="otrs_checked"/>
           </group>
           <footer>
             <button type="object" name="button_change" string="Change"/>
             <button special="cancel" string="Cancel" class="btn-secondary"/>
           </footer>
         </form>
       </field>
     </record>
-    <act_window id="action_contract_mobile_tariff_change_wizard" name="Change Mobile Tariff" res_model="contract.mobile.tariff.change.wizard" view_type="form" view_mode="form" target="new"/>
-    <record id="view_contract_form_mobile_tariff_change_wizard_button" model="ir.ui.view">
-      <field name="name">contract.form.mobile.tariff.change.wizard.button</field>
+    <act_window id="action_contract_tariff_change_wizard" name="Change Tariff" res_model="contract.tariff.change.wizard" view_type="form" view_mode="form" target="new"/>
+    <record id="view_contract_form_tariff_change_wizard_button" model="ir.ui.view">
+      <field name="name">contract.form.tariff.change.wizard.button</field>
       <field name="model">contract.contract</field>
       <field name="inherit_id" ref="contract.contract_contract_form_view"/>
       <field name="arch" type="xml">
         <button name="action_contract_send" position="after">
+          <button name="%(action_contract_tariff_change_wizard)d" string="Change Tariff" type="action" context="{'default_active_id': active_id}" groups="somconnexio.group_somconnexio_admin"/>
           <field name="is_broadband" invisible="1"/>
-          <button name="%(action_contract_mobile_tariff_change_wizard)d" string="Change Tariff Mobile" type="action" context="{'default_active_id': active_id}" attrs="{'invisible': [('is_broadband', '=', True)]}"/>
+          <button name="%(action_contract_tariff_change_wizard)d" string="Change Tariff BA" type="action" context="{'default_active_id': active_id, 'ba': True}" attrs="{'invisible': [('is_broadband', '=', False)]}"/>
         </button>
       </field>
     </record>
   </data>
 </odoo>
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_tariff_change/contract_tariff_change.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,129 +1,149 @@
-from datetime import datetime, date
-from calendar import monthrange
+from datetime import date, timedelta
 
 from odoo import models, fields, api, _
 from odoo.addons.queue_job.job import job
-from ...services.contract_one_shot_process import ContractOneShotProcess
+from ...services.contract_change_tariff_process import ContractChangeTariffProcess
+from odoo.exceptions import ValidationError
 
 
-class ContractOneShotRequestWizard(models.TransientModel):
-    _name = 'contract.one.shot.request.wizard'
+class ContractTariffChangeWizard(models.TransientModel):
+    _name = 'contract.tariff.change.wizard'
     contract_id = fields.Many2one('contract.contract')
     summary = fields.Char(required=True)
-    done = fields.Boolean(required=True)
+    done = fields.Boolean(default=True)
     location = fields.Char()
     note = fields.Char()
 
     product_category_id = fields.Many2one(
         'product.category',
-        compute="_load_product_category_id"
+        compute="_compute_product_category_id"
     )
-    start_date = fields.Date('Start Date', required=True)
-    one_shot_product_id = fields.Many2one(
+    start_date = fields.Date('Start Date')
+
+    current_tariff_contract_line = fields.Many2one(
+        'contract.line',
+        related='contract_id.current_tariff_contract_line',
+    )
+
+    current_tariff_product = fields.Many2one(
+        'product.product',
+        related='current_tariff_contract_line.product_id',
+        string="Current Tariff"
+    )
+
+    new_tariff_product_id = fields.Many2one(
         'product.product',
-        string='One Shot products',
+        string='New tariff',
+    )
+
+    service_contract_type = fields.Char(
+        'contract.contract',
+        related='contract_id.service_contract_type',
     )
-    activity_type = fields.Many2one('mail.activity.type')
 
     @api.model
     def default_get(self, fields_list):
         defaults = super().default_get(fields_list)
         defaults['contract_id'] = self.env.context['active_id']
-        defaults['start_date'] = datetime.strftime(date.today(), "%Y-%m-%d")
         return defaults
 
     @api.depends("contract_id")
-    def _load_product_category_id(self):
+    def _compute_product_category_id(self):
         if not self.contract_id:
             return False
+
         if self.contract_id.is_mobile:
             self.product_category_id = self.env.ref(
-                'somconnexio.mobile_oneshot_service').id
-        elif self.contract_id.service_technology_id == self.env.ref(
-            'somconnexio.service_technology_adsl'
-        ):
+                'somconnexio.mobile_service')
+        elif self.contract_id.is_fiber:
             self.product_category_id = self.env.ref(
-                'somconnexio.broadband_oneshot_adsl_service'
-            ).id
+                'somconnexio.broadband_fiber_service')
         else:
             self.product_category_id = self.env.ref(
-                'somconnexio.broadband_oneshot_service'
-            ).id
-
-    @api.onchange("one_shot_product_id")
-    def onchange_one_shot_product_id(self):
-        router_list = [
-            self.env.ref('somconnexio.EnviamentRouter_product_template'),
-            self.env.ref('somconnexio.RecollidaRouter_product_template')
-        ]
-        one_shot_list = [
-            self.env.ref(
-                'somconnexio.SMSMassius500SMS_product_template'
-            ),
-            self.env.ref(
-                'somconnexio.DadesAddicionals1GBSenseCost_product_template'
-            )
-        ]
+                'somconnexio.broadband_adsl_service').id
 
-        if self.one_shot_product_id.product_tmpl_id in one_shot_list:
-            self.summary = ""
-            self.done = True
-            self.activity_type = self.env.ref('somconnexio.mail_activity_type_one_shot')
-        elif self.one_shot_product_id.product_tmpl_id in router_list:
-            self.summary = ""
-            self.done = True
-            self.activity_type = self.env.ref('somconnexio.mail_activity_type_router_send_or_return')  # noqa
-        else:
-            self.summary = ""
-            self.done = False
-            self.activity_type = self.env.ref('somconnexio.mail_activity_type_sim_change')  # noqa
+    @api.onchange("new_tariff_product_id")
+    def onchange_new_tariff_product_id(self):
+        if self.new_tariff_product_id:
+            self.summary = " ".join([_('Tariff change'), self.new_tariff_product_id.showed_name])  # noqa
 
-    def button_add(self):
+    def button_change(self):
         self.ensure_one()
 
-        one_shot_contract_line = {
-            "name": self.one_shot_product_id.name,
-            "product_id": self.one_shot_product_id.id,
+        if not self.start_date:
+            raise ValidationError(_("Start date required"))
+
+        available_relations = self.env['product.category.technology.supplier'].search([
+            ('service_technology_id', '=', self.contract_id.service_technology_id.id),
+            ('service_supplier_id', '=', self.contract_id.service_supplier_id.id)
+        ])
+        available_categories = [c.product_category_id.id for c in available_relations]
+        available_products_categ = self.env['product.template'].search([
+            ('categ_id', 'in', available_categories)
+        ])
+        if self.new_tariff_product_id.product_tmpl_id not in available_products_categ:
+            raise ValidationError(_(
+                'Neither Service Technology nor Service Supplier cannot be changed'
+            ))
+        current_tariff_line_dct = {
+            "name": self.current_tariff_contract_line.product_id.name,
+            "product_id": self.current_tariff_contract_line.product_id.id,
+            "date_start": self.current_tariff_contract_line.date_start,
+            "date_end": self.start_date - timedelta(days=1)
+        }
+        new_tariff_line_dct = {
+            "name": self.new_tariff_product_id.name,
+            "product_id": self.new_tariff_product_id.id,
             "date_start": self.start_date,
-            "date_end": self._get_last_day_of_month(self.start_date)
         }
-
         self.contract_id.write(
-            {'contract_line_ids': [(0, 0, one_shot_contract_line)]}
+            {'contract_line_ids': [
+                (0, 0, new_tariff_line_dct),
+                (1, self.current_tariff_contract_line.id, current_tariff_line_dct)
+            ]}
         )
-
-        message = _("One shot product '{}' added on '{}'")
+        message = _("Contract tariff to be changed from '{}' to '{}' with start_date: {}")  # noqa
         self.contract_id.message_post(
             message.format(
-                self.one_shot_product_id.showed_name,
+                self.current_tariff_contract_line.product_id.showed_name,
+                self.new_tariff_product_id.showed_name,
                 self.start_date,
             )
         )
 
+        if (
+            self.contract_id.is_pack and
+            self.new_tariff_product_id.product_tmpl_id.categ_id == self.env.ref(
+                "somconnexio.mobile_service"
+                ) and not
+            self.new_tariff_product_id.product_is_pack_exclusive
+                ):
+            message = _("Pack broken because of mobile tariff change. Old linked fiber contract ref: '{}'")  # noqa
+            self.contract_id.message_post(
+                message.format(
+                    self.contract_id.parent_pack_contract_id.code
+                )
+            )
+            self.contract_id.break_packs()
+
         self._create_activity()
         return True
 
-    def _get_last_day_of_month(self, request_date):
-        #  Touple with weekday (0-6) and number of days (28-31) for a given month
-        month_range = monthrange(request_date.year, request_date.month)
-
-        return date(request_date.year, request_date.month, month_range[1])
-
     def _create_activity(self):
         self.env['mail.activity'].create({
             'summary': self.summary,
             'res_id': self.contract_id.id,
             'res_model_id': self.env.ref('contract.model_contract_contract').id,
             'user_id': self.env.user.id,
-            'activity_type_id': self.activity_type.id,
+            'activity_type_id': self.env.ref('somconnexio.mail_activity_type_tariff_change').id,  # noqa
             'done': self.done,
             'date_done': date.today(),
             'date_deadline': date.today(),
             'location': self.location,
             'note': self.note,
         })
 
     @job
     def run_from_api(self, **params):
-        service = ContractOneShotProcess(self.env)
+        service = ContractChangeTariffProcess(self.env)
         service.run_from_api(**params)
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_one_shot_request/contract_one_shot_request.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/contract_terminate/contract_terminate.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/create_lead_from_partner/create_lead_from_partner.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/create_subscription_from_partner/create_subscription_from_partner.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_generate_SIM_delivery/crm_lead_generate_SIM_delivery.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_print_SIM_delivery_label/crm_lead_print_SIM_delivery_label.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_lead_remesa/crm_lead_remesa.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/crm_leads_validate/crm_leads_validate.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/import_payment_group/import_payment_group.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/invoice_claim_1_send/invoice_claim_1_send.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/mail_compose_message/mail_compose_message.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/mail_compose_message/mail_compose_message.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/move_line_add_to_payment_debit_order/move_line_add_to_payment_debit_order.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/partner_check_somoffice_email/partner_check_somoffice_email.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/partner_email_change/partner_email_change.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/payment_order_confirm/payment_order_confirm.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/payment_order_generated_to_uploaded_queued/payment_order_generated_to_uploaded_queued.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/product_publish/product_publish.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/product_publish/product_publish.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/product_publish/product_publish.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/product_publish/product_publish.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.py` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.py`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.xml` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo/addons/somconnexio/wizards/test_mailing/test_mailing.xml`

 * *Files identical despite different names*

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo12_addon_somconnexio.egg-info/PKG-INFO` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo12_addon_somconnexio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-somconnexio
-Version: 12.0.2.2.2
+Version: 12.0.2.3.0
 Summary: Odoo Som Connexió customizations
 Home-page: https://coopdevs.org
 Author: Coopdevs Treball SCCL
 License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo12_addon_somconnexio.egg-info/SOURCES.txt` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo12_addon_somconnexio.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,19 @@
 odoo/addons/somconnexio/data/res.users.xml
 odoo/addons/somconnexio/data/res_bank_data.xml
 odoo/addons/somconnexio/data/service_supplier.xml
 odoo/addons/somconnexio/data/service_technology.xml
 odoo/addons/somconnexio/data/service_technology_service_supplier.xml
 odoo/addons/somconnexio/data/share_type.xml
 odoo/addons/somconnexio/demo/partner.xml
-odoo/addons/somconnexio/demo/pricelist.xml
+odoo/addons/somconnexio/demo/product.pricelist.csv
 odoo/addons/somconnexio/demo/subscription_requests.xml
+odoo/addons/somconnexio/demo/contract/contract.xml
+odoo/addons/somconnexio/demo/contract/contract_pack.xml
+odoo/addons/somconnexio/demo/contract/contract_shared_data.xml
 odoo/addons/somconnexio/helpers/__init__.py
 odoo/addons/somconnexio/helpers/date.py
 odoo/addons/somconnexio/helpers/language.py
 odoo/addons/somconnexio/i18n/ca_ES.po
 odoo/addons/somconnexio/i18n/es.po
 odoo/addons/somconnexio/listeners/__init__.py
 odoo/addons/somconnexio/listeners/contract_line_listener.py
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/odoo12_addon_somconnexio.egg-info/requires.txt` & `odoo12-addon-somconnexio-12.0.2.3.0/odoo12_addon_somconnexio.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -59,10 +59,10 @@
 odoo12-addon-web-favicon==12.0.1.0.0.99.dev14
 odoo12-addon-web-no-bubble==12.0.1.0.0.99.dev8
 odoo12-addon-web-responsive==12.0.2.3.2
 odoo12-addon-web-searchbar-full-width==12.0.1.0.0.99.dev6
 odoo12-addon-web-widget-open-tab==12.0.1.0.1.99.dev2
 odoo12-addon-web_m2x_options
 odoo<12.1dev,>=12.0a
-otrs-somconnexio==0.4.48
+otrs-somconnexio==0.4.52
 pyopencell==0.4.5
 python-stdnum==1.14
```

### Comparing `odoo12-addon-somconnexio-12.0.2.2.2/setup.py` & `odoo12-addon-somconnexio-12.0.2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,14 @@
         "external_dependencies_override": {
             "python": {
                 "correos_preregistro": "correos-preregistro==0.0.6",
                 "correos_seguimiento": "correos-seguimiento==0.0.3",
                 "factory": "factory-boy",
                 "faker": "faker==9.3.1",
                 "hashids": "hashids==1.3.1",
-                "otrs_somconnexio": "otrs-somconnexio==0.4.48",
+                "otrs_somconnexio": "otrs-somconnexio==0.4.52",
                 "pyopencell": "pyopencell==0.4.5",
                 "stdnum": "python-stdnum==1.14",
             },
         },
     },
 )
```

