# Comparing `tmp/z0bug_odoo-2.0.8.tar.gz` & `tmp/z0bug_odoo-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/z0bug_odoo-2.0.8.tar", last modified: Thu May 25 08:55:28 2023, max compression
+gzip compressed data, was "dist/z0bug_odoo-2.0.9.tar", last modified: Tue Jun 27 16:08:19 2023, max compression
```

## Comparing `z0bug_odoo-2.0.8.tar` & `z0bug_odoo-2.0.9.tar`

### file list

```diff
@@ -1,162 +1,163 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/__main__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5923 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/asset_category.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6015 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_mode.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    17914 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_21.png
--rw-r--r--   0 odoo      (1000) odoo      (1000)     8512 2023-03-31 16:47:10.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/date_range.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    11354 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/res_partner.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5958 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_9.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    12377 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_12.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6863 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.partner_mycompany.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    28222 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_2.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5311 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_method.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8641 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/res_country_state.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5736 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_term.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    26659 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_5.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5254 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/italy_profile_account.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5649 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_fiscal_position_tax.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6034 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_term_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     4933 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/decimal_precision.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5304 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/asset_asset.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6297 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/miscellaneous.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    21273 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_4.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    11254 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_tax.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6230 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_move_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9845 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_24.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6256 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_10.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5320 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/res_bank.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8169 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_5.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    20091 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_6.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    20415 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_10.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5183 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/date_range_type.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    17619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_3.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    23271 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_11.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    36713 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_account.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9436 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_18.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6801 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/res_partner_bank.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5806 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/purchase_order.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5098 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_fiscal_year.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    13357 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_26.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    10816 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_19.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    40384 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/base.partner_admin.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5008 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/res_company.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    49021 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_6.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7618 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_14.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5548 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/product_supplierinfo.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6862 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_4.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/modules.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5485 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/withholding_tax.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7139 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_journal.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14311 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_22.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7885 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/purchase_order_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    37268 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_8.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5063 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/stock_inventory.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5185 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/withholding_tax_rate.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14221 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_16.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7940 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_15.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5681 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/asset_category_depreciation_type.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5797 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_16.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15336 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_1.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14581 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_1.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3017 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_15.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5420 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_rc_type.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    10897 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_17.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5159 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_banking_mandate.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     4987 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/dichiarazione_intento_yearly_limit.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9709 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_invoice_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8011 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/sale_order_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14993 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_3.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5289 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/dichiarazione_intento.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5496 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/res_currency_rate.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7931 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_11.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6090 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_13.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7940 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_invoice.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5573 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_move.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7118 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_20.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9911 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_13.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    12143 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_7.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    10429 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_12.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     7695 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_8.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5119 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_rc_type_tax.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    15668 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_14.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9180 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/product_product.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1436 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_7.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8985 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/product_template.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    12852 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_2.png
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6097 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/sale_order.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5212 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/stock_inventory_line.xlsx
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6561 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/data/account_fiscal_position.xlsx
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2235 2023-05-20 08:36:32.000000 z0bug_odoo-2.0.8/z0bug_odoo/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6806 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/scripts/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4491 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/z0bug_odoo_lib.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/testenv/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5945 2023-05-24 07:12:36.000000 z0bug_odoo-2.0.8/z0bug_odoo/testenv/_check4deps_.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)   113576 2023-05-23 15:08:50.000000 z0bug_odoo-2.0.8/z0bug_odoo/testenv/testenv.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       73 2023-05-24 07:19:53.000000 z0bug_odoo-2.0.8/z0bug_odoo/testenv/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    12824 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/test_common.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    14660 2023-04-15 07:25:23.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/run_pylint.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/openerp/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/openerp/osv/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/openerp/osv/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)       68 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/openerp/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      174 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/README.md
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/pudb.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/pdb.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/pylint_deprecated_modules/ipdb.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1515 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/git_run.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     3601 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/get_test_dependencies.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2084 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/test_pylint
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     8580 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/getaddons.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3134 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_test_dependencies
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6412 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/odoo_connection.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3551 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/apis.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2598 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/test_flake8
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3843 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_run_tests
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1863 2023-04-15 07:25:46.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_tnlbot.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7550 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/clone_oca_dependencies
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    28570 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/test_server.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_pr.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      775 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      117 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_shellcheck.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      618 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_70.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_PYPI.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_61.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_beta.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_MINIMAL.cfg
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3247 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_makepot
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      263 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      120 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_run_flake8
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      833 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_helpers.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      780 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/z0bug_odoo/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       11 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-07 16:23:41.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       66 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6135 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       44 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1181 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/z0bug_odoo.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/setup.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     2235 2023-05-20 07:45:02.000000 z0bug_odoo-2.0.8/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1181 2023-05-25 08:55:28.000000 z0bug_odoo-2.0.8/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)    97341 2023-05-21 13:34:13.000000 z0bug_odoo-2.0.8/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2023-06-22 03:21:52.000000 z0bug_odoo-2.0.9/z0bug_odoo/__main__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5923 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/asset_category.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6015 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_payment_mode.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    17914 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_21.png
+-rw-r--r--   0 odoo      (1000) odoo      (1000)     8512 2023-03-31 16:47:10.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/date_range.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    11354 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/res_partner.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5958 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_9.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    12377 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_12.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6863 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.partner_mycompany.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    28222 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_2.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5311 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_payment_method.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8641 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/res_country_state.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5736 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_payment_term.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    26659 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_5.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5254 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/italy_profile_account.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5649 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_fiscal_position_tax.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6034 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_payment_term_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4933 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/decimal_precision.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5304 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/asset_asset.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6297 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/miscellaneous.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    21273 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_4.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    11254 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_tax.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6230 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_move_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9845 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_24.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6256 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_10.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5320 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/res_bank.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8169 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_5.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    20091 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_6.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    20415 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_10.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5183 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/date_range_type.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    17619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_3.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    23271 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_11.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    36713 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_account.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9436 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_18.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6801 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/res_partner_bank.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5806 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/purchase_order.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5098 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_fiscal_year.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    13357 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_26.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10816 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_19.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    40384 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/base.partner_admin.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5008 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/res_company.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    49021 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_6.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7618 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_14.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5548 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/product_supplierinfo.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6862 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_4.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/modules.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5485 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/withholding_tax.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7139 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_journal.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14311 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_22.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7885 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/purchase_order_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    37268 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_8.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5063 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/stock_inventory.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5185 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/withholding_tax_rate.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14221 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_16.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7940 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_15.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5681 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/asset_category_depreciation_type.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5797 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_16.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15336 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_1.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14581 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_1.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3017 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_15.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5420 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_rc_type.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10897 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_17.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5159 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_banking_mandate.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4987 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/dichiarazione_intento_yearly_limit.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9709 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_invoice_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8011 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/sale_order_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14993 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_3.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5289 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/dichiarazione_intento.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5496 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/res_currency_rate.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7931 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_11.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6090 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_13.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7940 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_invoice.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5573 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_move.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7118 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_20.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9911 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_13.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    12143 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_7.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10429 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_12.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     7695 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_8.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5119 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_rc_type_tax.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    15668 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_14.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9180 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/product_product.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1436 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_7.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8985 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/product_template.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    12852 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_2.png
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6097 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/sale_order.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     5212 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/stock_inventory_line.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6561 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/data/account_fiscal_position.xlsx
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       42 2023-06-15 05:45:03.000000 z0bug_odoo-2.0.9/z0bug_odoo/test_pycharm_unicode.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2235 2023-06-24 06:17:11.000000 z0bug_odoo-2.0.9/z0bug_odoo/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6814 2023-06-24 13:34:21.000000 z0bug_odoo-2.0.9/z0bug_odoo/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/scripts/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4491 2023-06-25 03:11:51.000000 z0bug_odoo-2.0.9/z0bug_odoo/z0bug_odoo_lib.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo/testenv/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    10076 2023-06-07 06:59:54.000000 z0bug_odoo-2.0.9/z0bug_odoo/testenv/_check4deps_.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)   115257 2023-06-27 15:42:08.000000 z0bug_odoo-2.0.9/z0bug_odoo/testenv/testenv.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       73 2023-06-24 06:17:11.000000 z0bug_odoo-2.0.9/z0bug_odoo/testenv/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    12824 2023-06-25 03:11:51.000000 z0bug_odoo-2.0.9/z0bug_odoo/test_common.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    14737 2023-06-24 06:17:11.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/run_pylint.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/pylint_deprecated_modules/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/pylint_deprecated_modules/openerp/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/pylint_deprecated_modules/openerp/osv/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/pylint_deprecated_modules/openerp/osv/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)       68 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/pylint_deprecated_modules/openerp/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      174 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/pylint_deprecated_modules/README.md
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/pylint_deprecated_modules/pudb.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/pylint_deprecated_modules/pdb.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/pylint_deprecated_modules/ipdb.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     1515 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/git_run.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     3601 2023-06-24 13:34:21.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/get_test_dependencies.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2084 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/test_pylint
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     8580 2023-06-24 13:34:21.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/getaddons.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3134 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/travis_test_dependencies
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     6412 2023-06-22 03:20:22.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/odoo_connection.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3551 2023-06-22 03:19:59.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/apis.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     2622 2023-06-24 13:34:21.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/test_flake8
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3851 2023-06-24 13:34:21.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/travis_run_tests
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1864 2023-06-24 06:17:11.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/travis_tnlbot.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     7574 2023-06-24 13:34:21.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/clone_oca_dependencies
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    28599 2023-06-24 13:34:21.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/test_server.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      668 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8__init__MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2005 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_pr.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      593 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8__init__REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      744 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      775 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_REDUCED.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      117 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_shellcheck.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      618 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_70.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1022 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      639 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8__init__AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8__init__.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2575 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2823 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_PYPI.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      619 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_61.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      498 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8__init__NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2526 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_beta.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_AVERAGE.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      195 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_NEARBY.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      814 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8_MINIMAL.cfg
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3271 2023-06-24 06:17:11.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/travis_makepot
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      263 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      120 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/travis_run_flake8
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      833 2022-12-09 05:08:44.000000 z0bug_odoo-2.0.9/z0bug_odoo/travis/travis_helpers.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      780 2023-06-25 03:11:51.000000 z0bug_odoo-2.0.9/z0bug_odoo/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       11 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-01-07 16:23:41.000000 z0bug_odoo-2.0.9/z0bug_odoo.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       66 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6170 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       44 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1181 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/z0bug_odoo.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     2259 2023-06-24 13:34:21.000000 z0bug_odoo-2.0.9/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1181 2023-06-27 16:08:19.000000 z0bug_odoo-2.0.9/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)    65156 2023-06-24 06:17:11.000000 z0bug_odoo-2.0.9/README.rst
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/asset_category.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/asset_category.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_mode.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_payment_mode.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_21.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_21.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/date_range.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/date_range.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/res_partner.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/res_partner.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_9.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_9.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_12.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_12.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.partner_mycompany.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.partner_mycompany.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_2.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_2.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_method.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_payment_method.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/res_country_state.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/res_country_state.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_term.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_payment_term.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_5.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_5.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/italy_profile_account.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/italy_profile_account.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_fiscal_position_tax.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_fiscal_position_tax.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_payment_term_line.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_payment_term_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/decimal_precision.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/decimal_precision.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/asset_asset.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/asset_asset.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/miscellaneous.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/miscellaneous.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_4.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_4.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_tax.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_tax.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_move_line.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_move_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_24.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_24.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_10.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_10.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/res_bank.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/res_bank.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_5.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_5.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_6.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_6.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_10.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_10.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/date_range_type.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/date_range_type.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_3.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_3.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_11.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_11.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_account.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_account.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_18.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_18.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/res_partner_bank.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/res_partner_bank.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/purchase_order.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/purchase_order.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_fiscal_year.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_fiscal_year.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_26.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_26.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_19.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_19.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/base.partner_admin.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/base.partner_admin.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/res_company.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/res_company.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_6.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_6.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_14.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_14.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/product_supplierinfo.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/product_supplierinfo.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_4.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_4.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/modules.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/modules.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/withholding_tax.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/withholding_tax.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_journal.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_journal.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_22.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_22.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/purchase_order_line.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/purchase_order_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_8.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_8.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/stock_inventory.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/stock_inventory.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/withholding_tax_rate.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/withholding_tax_rate.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_16.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_16.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_15.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_15.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/asset_category_depreciation_type.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/asset_category_depreciation_type.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_16.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_16.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_1.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_1.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_1.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_1.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_15.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_15.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_rc_type.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_rc_type.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_17.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_17.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_banking_mandate.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_banking_mandate.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/dichiarazione_intento_yearly_limit.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/dichiarazione_intento_yearly_limit.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_invoice_line.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_invoice_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/sale_order_line.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/sale_order_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_3.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_3.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/dichiarazione_intento.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/dichiarazione_intento.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/res_currency_rate.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/res_currency_rate.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_11.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_11.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_13.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_13.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_invoice.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_invoice.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_move.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_move.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_20.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_20.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_13.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_13.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_7.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_7.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_12.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_12.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_8.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_8.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_rc_type_tax.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_rc_type_tax.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.res_partner_14.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.res_partner_14.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/product_product.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/product_product.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_7.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_7.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/product_template.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/product_template.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/z0bug.product_template_2.png` & `z0bug_odoo-2.0.9/z0bug_odoo/data/z0bug.product_template_2.png`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/sale_order.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/sale_order.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/stock_inventory_line.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/stock_inventory_line.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/data/account_fiscal_position.xlsx` & `z0bug_odoo-2.0.9/z0bug_odoo/data/account_fiscal_position.xlsx`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/scripts/setup.info` & `z0bug_odoo-2.0.9/z0bug_odoo/scripts/setup.info`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/scripts/main.py` & `z0bug_odoo-2.0.9/z0bug_odoo/scripts/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
@@ -58,16 +58,17 @@
     local_venv = "/devel/venv/"
     pkgpath = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
     bin_path = lib_path = ""
     path = pkgpath
     while not bin_path and path != "/" and path != os.environ["HOME"]:
         path = os.path.dirname(path)
         if os.path.isdir(path) and os.path.basename(path) in ("bin", "lib"):
-            if (os.path.isdir(os.path.join(os.path.dirname(path), "bin")) and
-                    os.path.isdir(os.path.join(os.path.dirname(path), "lib"))):
+            if os.path.isdir(
+                os.path.join(os.path.dirname(path), "bin")
+            ) and os.path.isdir(os.path.join(os.path.dirname(path), "lib")):
                 bin_path = os.path.join(os.path.dirname(path), "bin")
                 lib_path = os.path.join(os.path.dirname(path), "lib")
     if not bin_path and local_venv:
         for path in sys.path:
             if local_venv in path:
                 bin_path = os.path.join(
                     path[: path.find(local_venv)],
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/z0bug_odoo_lib.py` & `z0bug_odoo-2.0.9/z0bug_odoo/z0bug_odoo_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import os
 
 from openpyxl import load_workbook
 
 
 from python_plus import unicodes
 
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 
 class Z0bugOdoo(object):
     def __init__(self, release=None):
         try:
             import odoo.release as release
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/testenv/testenv.py` & `z0bug_odoo-2.0.9/z0bug_odoo/testenv/testenv.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-"""Test Environment v2.0.8
+"""Test Environment v2.0.9
 
 Copy this file in tests directory of your module.
 Please copy the documentation testenv.rst file too in your module.
 The __init__.py must import testenv.
 Your python test file should have to contain some following example lines:
 
 ::
@@ -57,29 +57,35 @@
 * Key value, format "external.key" (c)
 * 2 keys reference, for header/detail relationship (d)
 * Magic reference for 'product.template' / 'product.product' (e)
 
 Ordinary Odoo external reference (a) is a record of 'ir.model.data';
 you can see them from Odoo GUI interface.
 
-Test reference (b) are visible just in the test environment.
-They are identified by "z0bug." prefix module name.
+Test reference (b) are like external reference (a) but they are visible just in the
+test environment. They are identified by "z0bug." prefix module name.
 
 External key reference (c) is identified by "external." prefix followed by
-the key value used to retrieve the record.
-The field "code" or "name" are used to search record;
-for account.tax the "description" field is used.
+the key value used to retrieve the record. The field "code" or "name" are usually used
+to search record; for account.tax the "description" field is used.
 Please set self.debug_level = 2 (or more) to log these field keys.
 
 The 2 keys reference (d) needs to address child record inside header record
 at 2 level model (header/detail) relationship.
-The key MUST BE the same key of the parent record,
-plus "_", plus line identifier (usually 'sequence' field).
-i.e. "z0bug.move_1_3" means: line with sequence 3 of 'account.move.line'
-which is child of record "z0bug.move_1" of 'account.move'.
+The key MUST BE the couple of header key plus "_" and plus line key (usually 'sequence'
+field); the header key is the same key of the parent record. The line key may be:
+
+* the sequence value (if present n model)
+* the most meaningful field value
+* an index value
+
+i.e. "z0bug.invoice_1_3" means: line with sequence 3 of 'account.invoice.line'
+which is child of record "z0bug.invoice_1" of 'account.invoice'.
+i.e.: "EUR.2023-06-26" should be the key for res.currency.rate where "EUR" is the header
+key (res.currency) and "2023-06-26" is the date of rate.
 Please set self.debug_level = 2 (or more) to log these relationships.
 
 For 'product.template' (product) you must use '_template' text in reference (e).
 TestEnv inherit 'product.product' (variant) external reference.
 
 For furthermore information, please:
 
@@ -159,26 +165,33 @@
 # Please, do not change fields order
 KEY_CANDIDATE = (
     "acc_number",
     "code_prefix",
     "default_code",
     "sequence",
     "login",
-    # "description",
     "depreciation_type_id",
     "number",
     "move_name",
     "partner_id",
     "product_id",
     "product_tmpl_id",
+    "ref",
+    "reference",
+    "account_id",
     "tax_src_id",
     "tax_dest_id",
     "code",
     "name",
 )
+KEY_INCANDIDATE = {
+    "code": ["product.product"],
+    "partner_id": ["account.move.line"],
+    "ref": ["res.partner"],
+}
 KEY_OF_RESOURCE = {
     "res.users": "login",
     "account.tax": "description",
     "account.rc.type.tax": "purchase_tax_id",
 }
 REC_KEY_NAME = {"id", "code", "name"}
 if PY3:  # pragma: no cover
@@ -198,22 +211,31 @@
 
     def setUp(self):
         super(MainTest, self).setUp()
         self.odoo_major_version = release.version_info[0] if release else 0
         self.debug_level = 0
         self.PYCODESET = "utf-8"
         self._logger = _logger
+        # List of stored data by groups: grp1: [a,b,c], grp2: [d,e,f]
         self.setup_data_list = {}
+        # Data keys by group, name, resource, xref
         self.setup_data = {}
+        # List of (group, resource) for every xref
         self.setup_xrefs = {}
+        # Database structure (fields) by resource
         self.struct = {}
+        # Resource search keys: the first key is the child xref search key
         self.skeys = {}
+        # Parent resource field name for every resource
         self.parent_name = {}
+        # Parent resource name for every resource
         self.parent_resource = {}
+        # Childs one2many field name for every resource
         self.childs_name = {}
+        # Child resource name for every resource
         self.childs_resource = {}
         self.uninstallable_modules = []
         self.convey_record = {}
         self.assert_counter = 0
         for item in self.__module__.split("."):
             if item not in ("odoo", "openerp", "addons"):
                 self.module = self.env["ir.module.module"].search(
@@ -491,15 +513,15 @@
     # --  Hierarchical functions  --
     # ------------------------------
 
     def _search4parent(self, resource, parent_resource=None):
         if resource == "product.product":
             parent_resource = "product.template"
         else:
-            parent_resource = parent_resource or ".".join(resource.split(".")[:-1])
+            parent_resource = parent_resource or resource.rsplit(".", 1)[0]
         if parent_resource not in self.env:
             parent_resource = None
         if parent_resource and resource not in self.parent_resource:
             for field in self.struct[resource].keys():
                 if self.struct[resource][field].get("relation", "/") == parent_resource:
                     self.parent_name[resource] = field
                     self.parent_resource[resource] = parent_resource
@@ -576,19 +598,15 @@
             isinstance(xref, basestring)
             and re.match(r"[\w]+\.[\w][^\s]+$", xref)
         )
 
     @api.model
     def _unpack_xref(self, xref):
         # This is a 3 level external reference for header/detail relationship
-        ln = xref.split("_")
-        # Actual external reference for parent record
-        xref = "_".join(ln[:-1])
-        # Key to search for child record
-        ln = ln[-1]
+        xref, ln = xref.rsplit("_", 1)
         if ln.isdigit():
             ln = int(ln) or False
         elif isinstance(ln, basestring) and self._is_xref(ln):
             ln = self._get_xref_id(self._get_model_of_xref(xref), xref=ln, fmt="id")
         return xref, ln
 
     @api.model
@@ -712,28 +730,34 @@
                 self.skeys[resource] = [field]
                 self.log_lvl_2(
                     " 🌍 skeys[%s] = %s" % (resource, self.skeys[resource])
                 )
             else:
                 multi_key = True if self.parent_name.get(resource) else False
                 hdr_key = True if self.childs_name.get(resource) else False
+                self.skeys[resource] = []
                 for field in KEY_CANDIDATE:
                     if (
                         field == self.parent_name.get(resource)
                         or field in ("product_id", "partner_id") and hdr_key
                         or (field == "sequence" and not multi_key)
-                        or (field == "code" and resource == "product.product")
+                        or resource in KEY_INCANDIDATE.get(field, [])
                     ):
                         continue  # pragma: no cover
                     if field in self.struct[resource]:
-                        self.skeys[resource] = [field]
+                        self.skeys[resource].append(field)
                         self.log_lvl_2(
                             " 🌍 skeys[%s] = %s" % (resource, self.skeys[resource])
                         )
-                        break
+                        if (
+                            not multi_key
+                            or field == "sequence"
+                            or len(self.skeys[resource]) >= 3
+                        ):
+                            break
 
     # ---------------------------------------------
     # --  Type <char> / <text> / base functions  --
     # ---------------------------------------------
     # Return unicode even on python2
 
     @api.model
@@ -1240,21 +1264,22 @@
         return values
 
     @api.model
     def _upgrade_record(self, record, values, default={}):
         for field in list(values.keys()):
             if field in SUPERMAGIC_COLUMNS:  # pragma: no cover
                 continue
-            method = "_upgrade_field_%s" % record._fields[field].type
-            method = method if hasattr(self, method) else "_upgrade_field_base"
-            value = getattr(self, method)(record, field, values[field])
-            if not value and default.get(field):
-                value = getattr(self, method)(record, field, default[field])
-            if value is not None:
-                setattr(record, field, value)
+            if field not in default:
+                method = "_upgrade_field_%s" % record._fields[field].type
+                method = method if hasattr(self, method) else "_upgrade_field_base"
+                value = getattr(self, method)(record, field, values[field])
+                # if not value and default.get(field):
+                #     value = getattr(self, method)(record, field, default[field])
+                if value is not None:
+                    setattr(record, field, value)
         return record
 
     @api.model
     def _purge_values(self, values, timed=None):
         for field in BITTER_COLUMNS:
             if field in values:
                 del values[field]
@@ -1413,26 +1438,24 @@
     def _get_model_from_act_windows(self, act_windows):
         return act_windows.get(
             "model_name", act_windows.get("res_model", act_windows.get("model"))
         )
 
     @api.model
     def _get_src_model_from_act_windows(self, act_windows):
-        model_name = act_windows.get(
-            "src_model",
-            act_windows.get(
-                "binding_model_id", self._get_model_from_act_windows(act_windows)
-            ),
-        )
+        model_name = act_windows.get("src_model")
+        if not model_name and act_windows.get("binding_model_id"):
+            model_name = self.env.ref(act_windows["binding_model_id"])["model"]
         if not model_name or self._is_transient(model_name):
             model_name = None
             value = "%s,%d" % (act_windows["type"], act_windows["id"])
-            records = self.env["ir.values"].search([("value", "=", value)])
-            if len(records) == 1:
-                model_name = records[0].model
+            if "ir.values" in self.env:
+                records = self.env["ir.values"].search([("value", "=", value)])
+                if len(records) == 1:
+                    model_name = records[0].model
         return model_name
 
     @api.model
     def _get_model_from_records(self, records):
         if not records:  # pragma: no cover
             resource_model = None
         elif isinstance(records, basestring):
@@ -1459,60 +1482,63 @@
             records (obj): objects required by action server
             default (dict): default value to assign
             ctx (dict): context to pass to wizard during execution
 
         Returns:
             Odoo windows action to pass to wizard execution
         """
+        if not isinstance(act_windows, dict):  # pragma: no cover
+            self.raise_error("Invalid act_windows")
         self.log_lvl_2("🐞wizard starting(%s)" % act_windows.get("name"), strict=True)
         self.log_lvl_3(
             "🐞wizard starting(%s,%s,\nrec=%s,\ndef=%s,\nctx=%s)"
             % (
                 act_windows.get("name"),
                 self.dict_2_print(act_windows),
                 self.dict_2_print(records),
                 self.dict_2_print(default),
                 self.dict_2_print(ctx),
             ),
             strict=True,
         )
-        if not isinstance(act_windows, dict):  # pragma: no cover
-            self.raise_error("Invalid act_windows")
         if (
             records
             and isinstance(records, (list, tuple))
             and any([isinstance(x, (list, tuple)) for x in records])
         ):  # pragma: no cover
             self.raise_error("Invalid records type issued!")
         self._finalize_ctx_act_windows(records, act_windows, ctx)
         if ctx and ctx.get("res_id"):
             act_windows["res_id"] = ctx.pop("res_id")
+
         if records:
             # The record type have to be the same of the action windows model
             # Warning: action windows may not contain any model declaration
             # Please, do not remove test, because if model is declared in action windows
             # must match with record model type
             rec_model = self._get_model_from_records(records)
             act_model = self._get_model_from_act_windows(act_windows)
             src_model = self._get_src_model_from_act_windows(act_windows)
-            if rec_model != src_model:  # pragma: no cover
-                self.raise_error(
-                    "Records model %s differs from declared model %s in %s"
-                    % (rec_model, src_model, act_model)
-                )
-            if (
-                act_model != src_model
-                and self._is_transient(act_model)
-                and not act_windows.get("src_model")
-            ):  # pragma: no cover
-                self.log_lvl_1(
-                    "💡 You should specify the src_model %s for the action %s"
-                    % (src_model, act_windows.get("name"))
-                )
-                act_windows["src_model"] = src_model
+            if src_model:
+                # Check only for Odoo 10.0-
+                if rec_model != src_model:  # pragma: no cover
+                    self.raise_error(
+                        "Records model %s differs from declared model %s in %s"
+                        % (rec_model, src_model, act_model)
+                    )
+                if (
+                    act_model != src_model
+                    and self._is_transient(act_model)
+                    and not act_windows.get("src_model")
+                ):  # pragma: no cover
+                    self.log_lvl_1(
+                        "💡 You should specify the src_model %s for the action %s"
+                        % (src_model, act_windows.get("name"))
+                    )
+                    act_windows["src_model"] = src_model
             if "active_ids" not in act_windows["context"]:
                 act_windows["context"].update(
                     self._ctx_active_ids(records, ctx=act_windows["context"])
                 )
             if not is_iterable(records):                             # pragma: no cover
                 records = [records]
         if act_windows["type"] == "ir.actions.server":               # pragma: no cover
@@ -1586,15 +1612,20 @@
             records (obj): objects supplied for action server
 
         Returns:
             Same of <wizard_start>
         """
         # act_model = "ir.actions.act_window"
         module = self.module.name if module == "." else module
-        act_windows = self.for_xml_id(module, action_name)
+        try:
+            act_windows = self.for_xml_id(module, action_name)
+        except BaseException:
+            if not records or len(records) != 1:
+                self.raise_error(
+                    "Invalid action_name %s" % action_name)
         return self._wiz_launch(
             act_windows,
             default=default,
             ctx=ctx,
             records=records,
         )
 
@@ -1654,39 +1685,14 @@
         button_ctx={},
     ):
         """Simulate wizard execution issued by an action."""
         self.log_lvl_3(
             " 🐜 wizard running(%s, %s)"
             % (act_windows.get("name"), self.dict_2_print(act_windows))
         )
-        # if act_windows["type"] == "ir.actions.server":
-        #     if not records and "_wizard_" in act_windows:
-        #         records = act_windows.pop("_wizard_")
-        #     if not records:
-        #         raise (ValueError, "No records supplied")
-        #     if records._name != act_windows["model_name"]:
-        #         raise (ValueError, "Records model different from declared model")
-        #     ctx = {
-        #         "active_model": act_windows["model_name"],
-        #         "active_ids": [x.id for x in records],
-        #     }
-        #     eval_context = {
-        #         "env": self.env,
-        #         "model": records.with_context(ctx),
-        #         "Warning": Warning,
-        #         "record": records[0] if len(records) == 1 else None,
-        #         "records": records,
-        #         "log": self._logger,
-        #     }
-        #     eval_context.update(ctx)
-        #     act_windows = safe_eval(
-        #         act_windows["code"].strip(), eval_context, mode="exec", nocopy=True
-        #     )
-        #     return act_windows
-
         wizard = act_windows.pop("_wizard_")
         if button_name:
             return self._exec_action(wizard, button_name, web_changes=web_changes)
         return False
 
     #############################################
     #                                           #
@@ -1768,22 +1774,14 @@
 
         Returns:
             ISO format string with result date
         """
         return python_plus.compute_date(self.u(date), refdate=self.u(refdate))
 
     @api.model
-    def resource_bind(self, xref, raise_if_not_found=True, resource=None, group=None):
-        self.log_lvl_1("resource_bind() is deprecated: please use resource_browse()")
-        return self.resource_browse(xref=xref,
-                                    raise_if_not_found=raise_if_not_found,
-                                    resource=resource,
-                                    group=group)
-
-    @api.model
     def resource_browse(self, xref, raise_if_not_found=True, resource=None, group=None):
         """Bind record by xref or searching it or browsing it.
         This function returns a record using issued parameters. It works in follow ways:
 
         * With valid xref it work exactly like self.env.ref()
         * If xref is an integer it works exactly like self.browse()
         * I xref is invalid, xref is used to search record
@@ -1799,14 +1797,33 @@
 
         Returns:
             obj: the Odoo model record
 
         Raises:
             ValueError: if invalid parameters issued
         """
+        def build_domain(domain, k1, values):
+            kk = True
+            for field in self.skeys[resource]:
+                if k1 and kk:
+                    domain.append((field, "=", k1))
+                    kk = False
+                elif field in values:
+                    # domain = [(field, "=", values[field])]
+                    domain.append((field, "=", self._cast_field(
+                        resource, field, values[field], fmt="cmd")))
+            if domain and (
+                    resource not in RESOURCE_WO_COMPANY
+                    and "company_id" in self.struct[resource]
+            ):
+                domain.append("|")
+                domain.append(("company_id", "=", self.default_company().id))
+                domain.append(("company_id", "=", False))
+            return domain
+
         self.log_stack()
         self.log_lvl_3("🐞%s.resource_browse(%s)" % (resource, xref))
         # Search for Odoo standard external reference
         record = None
         if isinstance(xref, (int, long)):
             if not resource:  # pragma: no cover
                 self.raise_error("No model issued for binding")
@@ -1834,42 +1851,46 @@
             if raise_if_not_found:
                 self.raise_error("Model %s without search key" % resource)
             self._logger.info("⚠ Model %s without search key" % resource)
             return False
 
         values = self.get_resource_data(resource, xref, group=group)
         module, name = xref.split(".", 1)
-        key_field = self.skeys[resource][0]
         parent_name = self.parent_name.get(resource)
         if parent_name and self.parent_resource[resource] in self.childs_resource:
-            name, x = self._unpack_xref(name)
-            if not x:                                                # pragma: no cover
-                return False
-            domain = [(key_field, "=", x)]
-            x = self.resource_browse(
+            name, ln = self._unpack_xref(name)
+            parent_rec = self.resource_browse(
                 "%s.%s" % (module, name),
                 resource=self.parent_resource[resource],
                 raise_if_not_found=False,
                 group=group,
             )
-            if not x:                                                # pragma: no cover
+            if not parent_rec:                                       # pragma: no cover
+                if raise_if_not_found:
+                    self.raise_error(
+                        "Parent xref %s.%s not found for %s" % (module, name, resource))
+                self._logger.info(
+                    "⚠ Parent xref %s.%s not found for %s" % (module, name, resource))
                 return False
-            domain.append((parent_name, "=", x.id))
+            domain = [(parent_name, "=", parent_rec.id)]
         else:
-            if key_field in values:
-                name = values[key_field]
-            domain = [(key_field, "=", name)]
-        if (
-            resource not in RESOURCE_WO_COMPANY
-            and "company_id" in self.struct[resource]
-        ):
-            domain.append("|")
-            domain.append(("company_id", "=", self.default_company().id))
-            domain.append(("company_id", "=", False))
-        record = self.env[resource].search(domain)
+            domain = []
+            ln = parent_rec = False
+        domain = build_domain(domain, ln, values)
+        if not domain:                                               # pragma: no cover
+            if raise_if_not_found:
+                self.raise_error("Invalid search keys for model %s" % resource)
+            self._logger.info("⚠ Invalid search keys for model %s" % resource)
+            return False
+        record = self.env[resource].search(domain, limit=3)
+        if len(record) != 1 and parent_rec and isinstance(ln, (int, long)):
+            domain = [(parent_name, "=", parent_rec.id)]
+            domain = build_domain(domain, False, values)
+            if domain:
+                record = self.env[resource].search(domain)
         if len(record) == 1:
             return self.env[resource].browse(record[0].id)
         if raise_if_not_found:
             self.raise_error("External ID %s not found" % xref)  # pragma: no cover
         return False
 
     @api.model
@@ -1899,15 +1920,15 @@
         if not values:  # pragma: no cover
             self.raise_error("No values supplied for %s create" % resource)
         self.log_lvl_3(
             "🐞%s.resource_create(%s,xref=%s)"
             % (resource, self.dict_2_print(values), xref)
         )
         values = self.cast_types(resource, values, fmt="cmd", group=group)
-        if resource.startswith("account.move"):
+        if resource.startswith("account.move") and "line_ids" not in values:
             res = (
                 self.env[resource]
                 .with_context(check_move_validity=False)
                 .create(values)
             )
         else:
             res = self.env[resource].create(values)
@@ -2072,35 +2093,37 @@
             self.log_lvl_1(" 🐜 declare_all_data(%s,group=%s)" % (resource, group))
             item = "TEST_%s" % resource.upper().replace(".", "_")
             self.declare_resource_data(
                 resource, message[item], group=group, merge=merge
             )
 
     @api.model
-    def get_resource_data(self, resource, xref, group=None):
+    def get_resource_data(self, resource, xref, group=None, try_again=True):
         """Get declared resource data; may be used to test compare.
 
         Args:
             resource (str): Odoo model name or name assigned, i.e. "res.partner"
             xref (str): external reference
             group (str): if supplied select specific group data; default is "base"
 
         Returns:
             dictionary with data or empty dictionary
         """
-        xref = self._get_conveyed_value(resource, None, xref)
-        if (not resource or not group) and xref in self.setup_xrefs:
-            group, resource = self.setup_xrefs[xref]
+        if try_again:
+            xref = self._get_conveyed_value(resource, None, xref)
         group = group or "base"
         if (
             group in self.setup_data
-            and resource in self.setup_data[group]
+            and resource and resource in self.setup_data[group]
             and xref in self.setup_data[group][resource]
         ):
             return self.setup_data[group][resource][xref]
+        if try_again and xref in self.setup_xrefs:
+            group, resource = self.setup_xrefs[xref]
+            return self.get_resource_data(resource, xref, group=group, try_again=False)
         return {}  # pragma: no cover
 
     @api.model
     def get_resource_data_list(self, resource, group=None):
         """Get declared resource data list.
 
         Args:
@@ -2477,14 +2500,15 @@
         )
 
     @api.model
     def is_action(self, act_windows):
         return isinstance(act_windows, dict) and act_windows.get("type") in (
             "ir.actions.act_window",
             "ir.actions.client",
+            "ir.actions.act_window_close"
         )
 
     @api.model
     def wizard(
         self,
         module=None,
         action_name=None,
@@ -2654,15 +2678,15 @@
                     isinstance(tmpl, (list, tuple))
                     and isinstance(tmpl[0], (int, long))
                     and isinstance(tmpl[1], (int, long))
                     and isinstance(tmpl[2], dict)
                 ):
                     tmpl = tmpl[2]
                     template[ix] = tmpl
-                if not isinstance(tmpl, dict):
+                if not isinstance(tmpl, dict):                      # pragma: no cover
                     self.raise_error(
                         ("Function validate_records(): "
                          "invalid structure: %s must be a dictionary!" % tmpl)
                     )
                 if REC_KEY_NAME & set(tmpl.keys()):
                     if rec_parent:
                         repr = "line." + tmpl.get("code", tmpl.get("name", ""))[0:20]
@@ -2682,29 +2706,29 @@
         if len(record) > 1 or isinstance(record, (list, tuple)):
             for rec in record:
                 match = self.tmpl_init(
                     template, rec, nr=nr, repr=repr, rec_parent=rec_parent)
             return match
 
         resource = self._get_model_from_records(record)
-        if not resource:
+        if not resource:                                            # pragma: no cover
             self.raise_error("No valid record supplied for comparation!")
         self._load_field_struct(resource)
         childs_name = self.childs_name.get(resource)
         resource_child = self.childs_resource.get(resource)
         if resource_child:
             self._load_field_struct(resource_child)
         key = (rec_parent, record)
         template["_MATCH"] = template.get("_MATCH", {})
         template["_MATCH"][key] = 0
         for field in template.keys():
             if field in (childs_name, "id") or field.startswith("_"):
                 continue
             if self._cast_field(
-                resource, field, template[field]
+                resource, field, template[field], fmt="py"
             ) == self._convert_field_to_write(record, field):
                 template["_MATCH"][key] += 1
         if childs_name:
             merge_match(template["_MATCH"],
                         self.tmpl_init(
                             template[childs_name],
                             record[childs_name],
@@ -2722,15 +2746,15 @@
                 match = key
                 ctr = template["_MATCH"][key]
             return template, match, ctr
 
         def get_best_score(template, record, rec_parent=None, matched=[], childs=False):
             resource = self._get_model_from_records(record)
             childs_name = self.childs_name.get(resource)
-            if childs and not childs_name:
+            if childs and not childs_name:                          # pragma: no cover
                 return None, None
             ctr = -1
             match_key = match_tmpl = None
             for rec in record:
                 for tmpl in template:
                     if (tmpl, (rec_parent, rec)) in matched:
                         continue
@@ -2803,27 +2827,27 @@
                 ctr_assertion += self.tmpl_validate_record(template, rec)
             return ctr_assertion
 
         if [key for key in template["_MATCH"]][0][1] == record:
             for field in template.keys():
                 if field in (childs_name, "id") or field.startswith("_"):
                     continue
-                self.log_lvl_2(
-                    "🐞 ... assertEqual(%s.%s:'%s', %s:'%s')"
-                    % (
-                        self.tmpl_repr([template]),
-                        field,
-                        template[field],
-                        "rec(%d)" % record.id,
-                        record[field],
-                    )
-                )
+                msg_id = ("🐞 ... assertEqual(%s.%s:'%s', %s:'%s')"
+                          % (
+                              self.tmpl_repr([template]),
+                              field,
+                              template[field],
+                              "rec(%d)" % record.id,
+                              record[field],
+                          ))
+                self.log_lvl_2(msg_id)
                 self.assertEqual(
                     self._cast_field(resource, field, template[field], fmt="py"),
-                    self._cast_field(resource, field, record[field], fmt="py")
+                    self._cast_field(resource, field, record[field], fmt="py"),
+                    msg_id
                 )
                 ctr_assertion += 1
             if childs_name:
                 ctr_assertion += self.tmpl_validate_record(
                     template[childs_name], record[childs_name])
         return ctr_assertion
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/test_common.py` & `z0bug_odoo-2.0.9/z0bug_odoo/test_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     else:
         import odoo.tests.common as test_common
         from odoo.modules.module import get_module_resource  # noqa: F401
 else:
     print('No Odoo environment found!')
     sys.exit(0)
 
-__version__ = '2.0.8'
+__version__ = '2.0.9'
 
 
 class Z0bugBaseCase(test_common.BaseCase):
     def pool_env(self, model):
         """Return model pool_environment"""
         if int(release.major_version.split('.')[0]) < 8:
             return self.registry(model)
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/run_pylint.py` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/run_pylint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from __future__ import print_function
 
 import ast
 import os
+
 # import re
 import sys
 import inspect
 
 import click
 import pylint.lint
 
@@ -227,16 +228,17 @@
     # res = {
     #     key: value
     #     for key, value in (real_errors.get('by_msg') or {}).items()
     #     if key not in beta_msgs
     # }
     res = {
         key: value
-        for key, value in (hasattr(real_errors, 'by_msg')
-                           and getattr(real_errors, 'by_msg') or {}).items()
+        for key, value in (
+            hasattr(real_errors, 'by_msg') and getattr(real_errors, 'by_msg') or {}
+        ).items()
     }
     count_errors = get_count_fails(real_errors, list(beta_msgs))
     count_info = "count_errors %s" % count_errors
     print(count_info)
     if is_pr:
         print(travis_helpers.green('Starting lint check only for modules changed'))
         modules_changed = get_modules_changed(dir, branch_base)
@@ -257,16 +259,19 @@
         # pr_stats = {
         #     key: value
         #     for key, value in (pr_real_errors.get('by_msg') or {}).items()
         #     if key not in beta_msgs
         # }
         pr_stats = {
             key: value
-            for key, value in (hasattr(pr_real_errors, 'by_msg')
-                               and getattr(pr_real_errors, 'by_msg') or {}).items()
+            for key, value in (
+                hasattr(pr_real_errors, 'by_msg')
+                and getattr(pr_real_errors, 'by_msg')
+                or {}
+            ).items()
         }
         if pr_stats:
             pr_errors = get_count_fails(pr_real_errors, list(beta_msgs))
             print(
                 travis_helpers.yellow(
                     "Found %s errors in modules changed." % (pr_errors)
                 )
@@ -293,16 +298,19 @@
         # [
         #     linter_stats['by_msg'][msg]
         #     for msg in (linter_stats.get('by_msg') or {})
         #     if msg not in msgs_no_count
         # ]
         [
             linter_stats['by_msg'][msg]
-            for msg in (hasattr(linter_stats, 'by_msg')
-                        and getattr(linter_stats, 'by_msg') or {})
+            for msg in (
+                hasattr(linter_stats, 'by_msg')
+                and getattr(linter_stats, 'by_msg')
+                or {}
+            )
         ]
     )
 
 
 def is_installable_module(path):
     """return False if the path doesn't contain an installable odoo module,
     otherwise the full path to the module's manifest"""
@@ -363,21 +371,23 @@
         raise UserWarning("Python modules not found in paths %s" % (paths))
     exclude = os.environ.get('EXCLUDE', '').split(',')
     subpaths = [path for path in subpaths if os.path.basename(path) not in exclude]
     if not subpaths:
         return {'error': 0}
     cmd.extend(subpaths)
     if (
-        sys.version_info[0] == 2 and
-        'do_exit' in inspect.getargspec(pylint.lint.Run.__init__)[0]
+        sys.version_info[0] == 2
+        and 'do_exit' in inspect.getargspec(pylint.lint.Run.__init__)[0]
     ):
         # pylint has renamed this keyword argument
         pylint_res = pylint.lint.Run(cmd, do_exit=False)
-    elif (sys.version_info[0] > 2 and
-          'do_exit' in inspect.getfullargspec(pylint.lint.Run.__init__)[0]):
+    elif (
+        sys.version_info[0] > 2
+        and 'do_exit' in inspect.getfullargspec(pylint.lint.Run.__init__)[0]
+    ):
         # pylint has renamed this keyword argument
         pylint_res = pylint.lint.Run(cmd, do_exit=False)
     else:
         pylint_res = pylint.lint.Run(cmd, exit=False)
     return pylint_res.linter.stats
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/git_run.py` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/git_run.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/get_test_dependencies.py` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/get_test_dependencies.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     from test_server import get_test_dependencies
 except ImportError:
     from .getaddons import (get_dependencies, get_dependents, get_modules,
                             get_modules_info)
     from .test_server import get_test_dependencies
 
 
-__version__ = '2.0.8'
+__version__ = '2.0.9'
 
 
 def get_module_list(paths):
     res = []
     for path in paths.split(','):
         r = get_modules(os.path.expanduser(path))
         for m in r:
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/test_pylint` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/test_pylint`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/getaddons.py` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/getaddons.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     from git_run import GitRun
 except ImportError:
     try:
         from .git_run import GitRun
     except ImportError:
         from git_run import GitRun
 
-__version__ = '2.0.8'
+__version__ = '2.0.9'
 
 MANIFEST_FILES = ['__manifest__.py', '__odoo__.py', '__openerp__.py', '__terp__.py']
 
 
 def is_module(path):
     """return False if the path doesn't contain an odoo module, and the full
     path to the module manifest otherwise"""
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_test_dependencies` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/travis_test_dependencies`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/odoo_connection.py` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/odoo_connection.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/apis.py` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/apis.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/test_flake8` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/test_flake8`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 #!/usr/bin/env python
+# -*- coding: utf-8 -*-
 import os
 import subprocess
 import sys
 
 from getaddons import get_modules
 
 
-__version__ = '2.0.8'
+__version__ = '2.0.9'
 
 
 def get_build_dir():
     odoo_version = os.environ.get("VERSION")
     travis_base_dir = os.environ.get("TRAVIS_BUILD_DIR", "../..")
     tested_version = ''
     for ldir in ('./server/openerp', './openerp', './odoo'):
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_run_tests` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/travis_run_tests`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python
-# coding: utf-8
+# -*- coding: utf-8 -*-
 
 from __future__ import print_function
 from __future__ import unicode_literals
 import os
 # import subprocess
 # import shutil
 import sys
 from distutils.spawn import find_executable
 from travis_helpers import success_msg, fail_msg
 
-__version__ = '2.0.8'
+__version__ = '2.0.9'
 
 
 def main(test_list):
     """
     Loop through each test and run them, add display results at the end
 
     If the test has a .py extension, import as a list and call main function
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_tnlbot.py` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/travis_tnlbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from __future__ import print_function, unicode_literals
 
 import os
+
 # import sys
 
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 try:
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/clone_oca_dependencies` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/clone_oca_dependencies`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python
+# -*- coding: utf-8 -*-
 """Usage: clone_oca_dependencies [<checkout_dir> <build_dir>]
 
 Arguments:
 
 deps_checkout_dir: the directory in which the dependency repositories
 will be cloned
 build_dir: the directory in which the tested repositories have been cloned
@@ -29,15 +30,15 @@
 import os.path as osp
 import subprocess
 import logging
 from travis_helpers import print_flush
 from z0lib import z0lib
 
 _logger = logging.getLogger()
-__version__ = '2.0.8'
+__version__ = '2.0.9'
 
 
 def create_deps():
     return {
         'reqfilenames': [],
         'processed': set(),
     }
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/test_server.py` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/test_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,29 +11,39 @@
 import sys
 
 from six import string_types
 
 from zerobug import z0testodoo
 
 try:
-    from getaddons import (get_addons, get_applications_with_dependencies,
-                           get_dependencies, get_localizations_with_dependents,
-                           get_modules, get_modules_info)
+    from getaddons import (
+        get_addons,
+        get_applications_with_dependencies,
+        get_dependencies,
+        get_localizations_with_dependents,
+        get_modules,
+        get_modules_info,
+    )
     from travis_helpers import fail_msg, print_flush, success_msg
 except ImportError:
-    from .getaddons import (get_addons, get_applications_with_dependencies,
-                            get_dependencies, get_localizations_with_dependents,
-                            get_modules, get_modules_info)
+    from .getaddons import (
+        get_addons,
+        get_applications_with_dependencies,
+        get_dependencies,
+        get_localizations_with_dependents,
+        get_modules,
+        get_modules_info,
+    )
     from .travis_helpers import fail_msg, print_flush, success_msg
 try:
     import ConfigParser
 except ImportError:
     import configparser as ConfigParser
 
-__version__ = '2.0.8'
+__version__ = '2.0.9'
 
 LDIR = ('server/openerp', 'odoo/odoo', 'openerp', 'odoo')
 
 
 def has_test_errors(fname, dbname, odoo_version, check_loaded=True):
     """
     Check a list of log lines for test errors.
@@ -761,16 +771,17 @@
                 )
                 with open('stdout.log', 'wb') as stdout:
                     for line in iter(pipe.stdout.readline, b''):
                         stdout.write(line)
                         if sys.version_info[0] == 2:
                             print(line.strip())
                         else:
-                            print(line.strip().decode(
-                                'utf-8', errors='backslashreplace'))
+                            print(
+                                line.strip().decode('utf-8', errors='backslashreplace')
+                            )
                 returncode = pipe.wait()
                 # Find errors, except from failed mails
                 errors = has_test_errors(
                     "stdout.log", database, odoo_version, check_loaded
                 )
                 if returncode != 0:
                     all_errors.append(to_test)
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__MINIMAL.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8__init__MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_pr.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_pr.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8__init__REDUCED.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8__init__REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_REDUCED.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_REDUCED.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_REDUCED.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_AVERAGE.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8_AVERAGE.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_70.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_70.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_NEARBY.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8_NEARBY.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_PYPI.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_PYPI.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_61.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_exclude_61.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_pylint_beta.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_pylint_beta.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/cfg/travis_run_flake8_MINIMAL.cfg` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/cfg/travis_run_flake8_MINIMAL.cfg`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_makepot` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/travis_makepot`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python
+# -*- coding: utf-8 -*-
 # Copyright 2018 ACSONE SA/NV
 # License AGPL-3.0 or later (https://www.gnu.org/licenses/agpl).
 
 from __future__ import print_function
 from contextlib import contextmanager
 import os
 import subprocess
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/travis/travis_helpers.py` & `z0bug_odoo-2.0.9/z0bug_odoo/travis/travis_helpers.py`

 * *Files identical despite different names*

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo/__init__.py` & `z0bug_odoo-2.0.9/z0bug_odoo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 except ImportError:
     try:
         import openerp.release as release
         from . import test_common
     except ImportError:
         release = ''
 
-__version__ = '2.0.8'
+__version__ = '2.0.9'
 if eval(os.environ.get('TRAVIS_DEBUG_MODE', '0')) > 2:
     print('DEBUG: z0bug_odoo %s' % __version__)
     print('DEBUG: z0bug_odoo.sys.path=%s' % sys.path)
     if release:
         print('DEBUG: Odoo version detected: %s' % release.version)
     else:
         print('DEBUG: No Odoo environment found!')
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo.egg-info/SOURCES.txt` & `z0bug_odoo-2.0.9/z0bug_odoo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 README.rst
 setup.py
 z0bug_odoo/__init__.py
 z0bug_odoo/__main__.py
 z0bug_odoo/test_common.py
+z0bug_odoo/test_pycharm_unicode.py
 z0bug_odoo/z0bug_odoo_lib.py
 z0bug_odoo.egg-info/PKG-INFO
 z0bug_odoo.egg-info/SOURCES.txt
 z0bug_odoo.egg-info/dependency_links.txt
 z0bug_odoo.egg-info/entry_points.txt
 z0bug_odoo.egg-info/not-zip-safe
 z0bug_odoo.egg-info/requires.txt
```

### Comparing `z0bug_odoo-2.0.8/z0bug_odoo.egg-info/PKG-INFO` & `z0bug_odoo-2.0.9/z0bug_odoo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: z0bug-odoo
-Version: 2.0.8
+Version: 2.0.9
 Summary: Odoo testing framework
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `z0bug_odoo-2.0.8/setup.py` & `z0bug_odoo-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+# -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 setup(
     name='z0bug_odoo',
-    version='2.0.8',
+    version='2.0.9',
     description='Odoo testing framework',
     long_description="""
 Zeroincombenze(R) continuous testing framework for Odoo modules.
 
 Make avaiable test functions indipendent by Odoo version.
 """,
     classifiers=[
```

### Comparing `z0bug_odoo-2.0.8/PKG-INFO` & `z0bug_odoo-2.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: z0bug_odoo
-Version: 2.0.8
+Version: 2.0.9
 Summary: Odoo testing framework
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

