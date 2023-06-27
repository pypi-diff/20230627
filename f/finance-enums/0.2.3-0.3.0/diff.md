# Comparing `tmp/finance_enums-0.2.3.tar.gz` & `tmp/finance_enums-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+gzip compressed data, was "finance_enums-0.3.0.tar", last modified: Tue Jun 27 17:14:27 2023, max compression
```

## Comparing `finance_enums-0.2.3.tar` & `finance_enums-0.3.0.tar`

### file list

```diff
@@ -1,329 +1,66 @@
--rw-r--r--   0        0        0      544 1970-01-01 00:00:00.000000 finance_enums-0.2.3/local_dependencies/finance_enums/Cargo.toml
--rw-r--r--   0     1001      123     1587 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/Makefile
--rw-r--r--   0     1001      123        1 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/common/mod.rs
--rw-r--r--   0     1001      123   158040 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/country/iso3166.rs
--rw-r--r--   0     1001      123       34 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/country/mod.rs
--rw-r--r--   0     1001      123    11111 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/currency/iso4217.rs
--rw-r--r--   0     1001      123       33 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/currency/mod.rs
--rw-r--r--   0     1001      123    27914 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/exchange/iso10383.rs
--rw-r--r--   0     1001      123       87 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/exchange/mod.rs
--rw-r--r--   0     1001      123       44 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/instrument/iso10962.rs
--rw-r--r--   0     1001      123      470 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/instrument/mod.rs
--rw-r--r--   0     1001      123      351 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/lib.rs
--rw-r--r--   0     1001      123    22788 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/industry.rs
--rw-r--r--   0     1001      123    10841 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/industry_group.rs
--rw-r--r--   0     1001      123      314 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/mod.rs
--rw-r--r--   0     1001      123     5186 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/sector.rs
--rw-r--r--   0     1001      123    24096 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/sector/subindustry.rs
--rw-r--r--   0     1001      123      252 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/bond.rs
--rw-r--r--   0     1001      123     1287 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/commodity.rs
--rw-r--r--   0     1001      123        1 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/currency.rs
--rw-r--r--   0     1001      123      319 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/equity.rs
--rw-r--r--   0     1001      123      662 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/fund.rs
--rw-r--r--   0     1001      123      441 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/future.rs
--rw-r--r--   0     1001      123      290 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/mod.rs
--rw-r--r--   0     1001      123      448 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/option.rs
--rw-r--r--   0     1001      123      362 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/security/security.rs
--rw-r--r--   0     1001      123     1071 2023-06-17 01:04:48.000000 finance_enums-0.2.3/local_dependencies/finance_enums/src/trading/mod.rs
--rw-r--r--   0        0        0      596 1970-01-01 00:00:00.000000 finance_enums-0.2.3/Cargo.toml
--rw-r--r--   0     1001      123      414 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.bumpversion.cfg
--rw-r--r--   0     1001      123      147 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.gitattributes
--rw-r--r--   0     1001      123     3352 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0     1001      123      834 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0     1001      123      595 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      123      206 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.github/dependabot.yml
--rw-r--r--   0     1001      123     1608 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.github/workflows/build.yml
--rw-r--r--   0     1001      123     4126 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.github/workflows/publish.yml
--rw-r--r--   0     1001      123     2284 2023-06-17 01:04:48.000000 finance_enums-0.2.3/.gitignore
--rw-r--r--   0     1001      123    11351 2023-06-17 01:04:48.000000 finance_enums-0.2.3/LICENSE
--rw-r--r--   0     1001      123     1990 2023-06-17 01:04:48.000000 finance_enums-0.2.3/Makefile
--rw-r--r--   0     1001      123     1246 2023-06-17 01:04:48.000000 finance_enums-0.2.3/README.md
--rw-r--r--   0     1001      123       52 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/__init__.py
--rw-r--r--   0     1001      123       52 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_all.py
--rw-r--r--   0     1001      123      195 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_country.py
--rw-r--r--   0     1001      123      429 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_currency.py
--rw-r--r--   0     1001      123      137 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_exchange.py
--rw-r--r--   0     1001      123        0 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_instrument.py
--rw-r--r--   0     1001      123      428 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_sector.py
--rw-r--r--   0     1001      123     1024 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_security.py
--rw-r--r--   0     1001      123      513 2023-06-17 01:04:48.000000 finance_enums-0.2.3/finance_enums/tests/test_trading.py
--rw-r--r--   0     1001      123      309 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AD.png
--rw-r--r--   0     1001      123      122 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AE.png
--rw-r--r--   0     1001      123      586 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AF.png
--rw-r--r--   0     1001      123      443 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AG.png
--rw-r--r--   0     1001      123      410 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AI.png
--rw-r--r--   0     1001      123      315 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AL.png
--rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AM.png
--rw-r--r--   0     1001      123      285 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AO.png
--rw-r--r--   0     1001      123      300 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AQ.png
--rw-r--r--   0     1001      123      150 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AR.png
--rw-r--r--   0     1001      123      469 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AS.png
--rw-r--r--   0     1001      123       93 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AT.png
--rw-r--r--   0     1001      123      405 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AU.png
--rw-r--r--   0     1001      123      176 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AW.png
--rw-r--r--   0     1001      123      155 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AX.png
--rw-r--r--   0     1001      123      165 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/AZ.png
--rw-r--r--   0     1001      123      321 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BA.png
--rw-r--r--   0     1001      123      235 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BB.png
--rw-r--r--   0     1001      123      246 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BD.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BE.png
--rw-r--r--   0     1001      123      173 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BF.png
--rw-r--r--   0     1001      123      116 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BG.png
--rw-r--r--   0     1001      123      189 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BH.png
--rw-r--r--   0     1001      123      394 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BI.png
--rw-r--r--   0     1001      123      122 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BJ.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BL.png
--rw-r--r--   0     1001      123      461 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BM.png
--rw-r--r--   0     1001      123      547 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BN.png
--rw-r--r--   0     1001      123      217 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BO.png
--rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BQ.png
--rw-r--r--   0     1001      123      438 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BR.png
--rw-r--r--   0     1001      123      181 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BS.png
--rw-r--r--   0     1001      123      570 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BT.png
--rw-r--r--   0     1001      123      153 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BV.png
--rw-r--r--   0     1001      123      111 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BW.png
--rw-r--r--   0     1001      123      206 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BY.png
--rw-r--r--   0     1001      123      378 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/BZ.png
--rw-r--r--   0     1001      123      259 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CA.png
--rw-r--r--   0     1001      123      365 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CC.png
--rw-r--r--   0     1001      123      350 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CD.png
--rw-r--r--   0     1001      123      246 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CF.png
--rw-r--r--   0     1001      123      330 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CG.png
--rw-r--r--   0     1001      123      113 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CH.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CI.png
--rw-r--r--   0     1001      123      487 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CK.png
--rw-r--r--   0     1001      123      186 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CL.png
--rw-r--r--   0     1001      123      158 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CM.png
--rw-r--r--   0     1001      123      214 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CN.png
--rw-r--r--   0     1001      123      116 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CO.png
--rw-r--r--   0     1001      123      123 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CR.png
--rw-r--r--   0     1001      123      240 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CU.png
--rw-r--r--   0     1001      123      267 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CV.png
--rw-r--r--   0     1001      123      189 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CW.png
--rw-r--r--   0     1001      123      508 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CX.png
--rw-r--r--   0     1001      123      318 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CY.png
--rw-r--r--   0     1001      123      273 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/CZ.png
--rw-r--r--   0     1001      123      116 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/DE.png
--rw-r--r--   0     1001      123      358 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/DJ.png
--rw-r--r--   0     1001      123      124 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/DK.png
--rw-r--r--   0     1001      123      269 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/DM.png
--rw-r--r--   0     1001      123      158 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/DO.png
--rw-r--r--   0     1001      123      276 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/DZ.png
--rw-r--r--   0     1001      123      325 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/EC.png
--rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/EE.png
--rw-r--r--   0     1001      123      175 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/EG.png
--rw-r--r--   0     1001      123      271 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/EH.png
--rw-r--r--   0     1001      123      465 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ER.png
--rw-r--r--   0     1001      123      273 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ES.png
--rw-r--r--   0     1001      123      324 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ET.png
--rw-r--r--   0     1001      123      130 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/FI.png
--rw-r--r--   0     1001      123      456 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/FJ.png
--rw-r--r--   0     1001      123      475 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/FK.png
--rw-r--r--   0     1001      123      183 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/FM.png
--rw-r--r--   0     1001      123      150 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/FO.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/FR.png
--rw-r--r--   0     1001      123       98 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GA.png
--rw-r--r--   0     1001      123      490 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GB.png
--rw-r--r--   0     1001      123      417 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GD.png
--rw-r--r--   0     1001      123      155 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GE.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GF.png
--rw-r--r--   0     1001      123      184 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GG.png
--rw-r--r--   0     1001      123      180 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GH.png
--rw-r--r--   0     1001      123      288 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GI.png
--rw-r--r--   0     1001      123      302 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GL.png
--rw-r--r--   0     1001      123      110 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GM.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GN.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GP.png
--rw-r--r--   0     1001      123      305 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GQ.png
--rw-r--r--   0     1001      123      180 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GR.png
--rw-r--r--   0     1001      123      517 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GS.png
--rw-r--r--   0     1001      123      210 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GT.png
--rw-r--r--   0     1001      123      237 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GU.png
--rw-r--r--   0     1001      123      168 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GW.png
--rw-r--r--   0     1001      123      375 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/GY.png
--rw-r--r--   0     1001      123      321 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/HK.png
--rw-r--r--   0     1001      123      405 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/HM.png
--rw-r--r--   0     1001      123      137 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/HN.png
--rw-r--r--   0     1001      123      262 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/HR.png
--rw-r--r--   0     1001      123      171 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/HT.png
--rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/HU.png
--rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ID.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IE.png
--rw-r--r--   0     1001      123      170 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IL.png
--rw-r--r--   0     1001      123      250 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IM.png
--rw-r--r--   0     1001      123      182 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IN.png
--rw-r--r--   0     1001      123      952 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IO.png
--rw-r--r--   0     1001      123      203 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IQ.png
--rw-r--r--   0     1001      123      356 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IR.png
--rw-r--r--   0     1001      123      153 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IS.png
--rw-r--r--   0     1001      123      122 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/IT.png
--rw-r--r--   0     1001      123      453 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/JE.png
--rw-r--r--   0     1001      123      322 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/JM.png
--rw-r--r--   0     1001      123      250 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/JO.png
--rw-r--r--   0     1001      123      240 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/JP.png
--rw-r--r--   0     1001      123      294 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KE.png
--rw-r--r--   0     1001      123      327 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KG.png
--rw-r--r--   0     1001      123      271 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KH.png
--rw-r--r--   0     1001      123      604 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KI.png
--rw-r--r--   0     1001      123      413 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KM.png
--rw-r--r--   0     1001      123      618 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KN.png
--rw-r--r--   0     1001      123      233 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KP.png
--rw-r--r--   0     1001      123      447 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KR.png
--rw-r--r--   0     1001      123      195 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KW.png
--rw-r--r--   0     1001      123      456 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KY.png
--rw-r--r--   0     1001      123      331 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/KZ.png
--rw-r--r--   0     1001      123      173 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LA.png
--rw-r--r--   0     1001      123      308 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LB.png
--rw-r--r--   0     1001      123      261 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LC.png
--rw-r--r--   0     1001      123      199 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LI.png
--rw-r--r--   0     1001      123      492 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LK.png
--rw-r--r--   0     1001      123      205 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LR.png
--rw-r--r--   0     1001      123      209 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LS.png
--rw-r--r--   0     1001      123      116 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LT.png
--rw-r--r--   0     1001      123      116 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LU.png
--rw-r--r--   0     1001      123      103 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LV.png
--rw-r--r--   0     1001      123      149 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/LY.png
--rw-r--r--   0     1001      123      190 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MA.png
--rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MC.png
--rw-r--r--   0     1001      123      249 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MD.png
--rw-r--r--   0     1001      123      335 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ME.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MF.png
--rw-r--r--   0     1001      123      122 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MG.png
--rw-r--r--   0     1001      123      520 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MH.png
--rw-r--r--   0     1001      123      418 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MK.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ML.png
--rw-r--r--   0     1001      123      280 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MM.png
--rw-r--r--   0     1001      123      243 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MN.png
--rw-r--r--   0     1001      123      311 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MO.png
--rw-r--r--   0     1001      123      450 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MP.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MQ.png
--rw-r--r--   0     1001      123      266 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MR.png
--rw-r--r--   0     1001      123      454 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MS.png
--rw-r--r--   0     1001      123      174 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MT.png
--rw-r--r--   0     1001      123      132 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MU.png
--rw-r--r--   0     1001      123      187 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MV.png
--rw-r--r--   0     1001      123      231 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MW.png
--rw-r--r--   0     1001      123      247 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MX.png
--rw-r--r--   0     1001      123      304 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MY.png
--rw-r--r--   0     1001      123      395 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/MZ.png
--rw-r--r--   0     1001      123      602 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NA.png
--rw-r--r--   0     1001      123      393 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NC.png
--rw-r--r--   0     1001      123      152 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NE.png
--rw-r--r--   0     1001      123      284 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NF.png
--rw-r--r--   0     1001      123       96 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NG.png
--rw-r--r--   0     1001      123      193 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NI.png
--rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NL.png
--rw-r--r--   0     1001      123      153 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NO.png
--rw-r--r--   0     1001      123      646 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NP.png
--rw-r--r--   0     1001      123      151 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NR.png
--rw-r--r--   0     1001      123      336 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NU.png
--rw-r--r--   0     1001      123      376 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/NZ.png
--rw-r--r--   0     1001      123      179 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/OM.png
--rw-r--r--   0     1001      123      294 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PA.png
--rw-r--r--   0     1001      123       96 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PE.png
--rw-r--r--   0     1001      123      294 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PF.png
--rw-r--r--   0     1001      123      377 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PG.png
--rw-r--r--   0     1001      123      319 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PH.png
--rw-r--r--   0     1001      123      295 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PK.png
--rw-r--r--   0     1001      123       92 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PL.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PM.png
--rw-r--r--   0     1001      123      556 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PN.png
--rw-r--r--   0     1001      123      296 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PR.png
--rw-r--r--   0     1001      123      293 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PS.png
--rw-r--r--   0     1001      123      354 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PT.png
--rw-r--r--   0     1001      123      239 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PW.png
--rw-r--r--   0     1001      123      190 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/PY.png
--rw-r--r--   0     1001      123      104 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/QA.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/RE.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/RO.png
--rw-r--r--   0     1001      123      398 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/RS.png
--rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/RU.png
--rw-r--r--   0     1001      123      212 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/RW.png
--rw-r--r--   0     1001      123      334 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SA.png
--rw-r--r--   0     1001      123      477 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SB.png
--rw-r--r--   0     1001      123      517 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SC.png
--rw-r--r--   0     1001      123      222 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SD.png
--rw-r--r--   0     1001      123      130 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SE.png
--rw-r--r--   0     1001      123      249 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SG.png
--rw-r--r--   0     1001      123      490 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SH.png
--rw-r--r--   0     1001      123      173 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SI.png
--rw-r--r--   0     1001      123      153 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SJ.png
--rw-r--r--   0     1001      123      326 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SK.png
--rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SL.png
--rw-r--r--   0     1001      123      362 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SM.png
--rw-r--r--   0     1001      123      158 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SN.png
--rw-r--r--   0     1001      123      198 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SO.png
--rw-r--r--   0     1001      123      215 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SR.png
--rw-r--r--   0     1001      123      264 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SS.png
--rw-r--r--   0     1001      123      254 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ST.png
--rw-r--r--   0     1001      123      195 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SV.png
--rw-r--r--   0     1001      123      419 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SX.png
--rw-r--r--   0     1001      123      182 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SY.png
--rw-r--r--   0     1001      123      436 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/SZ.png
--rw-r--r--   0     1001      123      414 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TC.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TD.png
--rw-r--r--   0     1001      123      328 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TF.png
--rw-r--r--   0     1001      123      248 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TG.png
--rw-r--r--   0     1001      123      114 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TH.png
--rw-r--r--   0     1001      123      196 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TJ.png
--rw-r--r--   0     1001      123      384 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TK.png
--rw-r--r--   0     1001      123      280 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TL.png
--rw-r--r--   0     1001      123      486 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TM.png
--rw-r--r--   0     1001      123      285 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TN.png
--rw-r--r--   0     1001      123      142 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TO.png
--rw-r--r--   0     1001      123      263 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TR.png
--rw-r--r--   0     1001      123      466 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TT.png
--rw-r--r--   0     1001      123      482 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TV.png
--rw-r--r--   0     1001      123      235 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TW.png
--rw-r--r--   0     1001      123      511 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/TZ.png
--rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/UA.png
--rw-r--r--   0     1001      123      231 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/UG.png
--rw-r--r--   0     1001      123      333 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/UM.png
--rw-r--r--   0     1001      123      333 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/US.png
--rw-r--r--   0     1001      123      294 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/UY.png
--rw-r--r--   0     1001      123      213 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/UZ.png
--rw-r--r--   0     1001      123      282 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VA.png
--rw-r--r--   0     1001      123      239 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VC.png
--rw-r--r--   0     1001      123      197 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VE.png
--rw-r--r--   0     1001      123      471 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VG.png
--rw-r--r--   0     1001      123      795 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VI.png
--rw-r--r--   0     1001      123      205 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VN.png
--rw-r--r--   0     1001      123      427 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/VU.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/WF.png
--rw-r--r--   0     1001      123      182 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/WS.png
--rw-r--r--   0     1001      123      100 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/YE.png
--rw-r--r--   0     1001      123      108 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/YT.png
--rw-r--r--   0     1001      123      406 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ZA.png
--rw-r--r--   0     1001      123      225 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ZM.png
--rw-r--r--   0     1001      123      295 2023-06-17 01:04:48.000000 finance_enums-0.2.3/flags/ZW.png
--rw-r--r--   0     1001      123     2658 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/CA_MIC.csv
--rw-r--r--   0     1001      123    79321 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/GICS Map 2023.xlsx
--rw-r--r--   0     1001      123   509696 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/ISO10383_MIC.csv
--rw-r--r--   0     1001      123    11357 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/US_MIC.csv
--rw-r--r--   0     1001      123    67904 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/atslist053123.pdf
--rw-r--r--   0     1001      123      402 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/flags_to_strings.py
--rw-r--r--   0     1001      123   149847 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/iso10383_generated.rs
--rw-r--r--   0     1001      123     4968 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/process_mics.py
--rw-r--r--   0     1001      123      577 2023-06-17 01:04:48.000000 finance_enums-0.2.3/helpers/scrape_flags.py
--rw-r--r--   0     1001      123     1526 2023-06-17 01:04:48.000000 finance_enums-0.2.3/pyproject.toml
--rw-r--r--   0     1001      123    52004 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/country/mod.rs
--rw-r--r--   0     1001      123    23116 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/currency/mod.rs
--rw-r--r--   0     1001      123    12045 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/exchange/mod.rs
--rw-r--r--   0     1001      123        0 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/instrument/mod.rs
--rw-r--r--   0     1001      123     1350 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/lib.rs
--rw-r--r--   0     1001      123    12919 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/sector/industry.rs
--rw-r--r--   0     1001      123     6439 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/sector/industry_group.rs
--rw-r--r--   0     1001      123      190 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/sector/mod.rs
--rw-r--r--   0     1001      123     3215 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/sector/sector.rs
--rw-r--r--   0     1001      123    27863 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/sector/subindustry.rs
--rw-r--r--   0     1001      123     2013 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/bond.rs
--rw-r--r--   0     1001      123     2113 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/commodity.rs
--rw-r--r--   0     1001      123        0 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/currency.rs
--rw-r--r--   0     1001      123     2392 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/equity.rs
--rw-r--r--   0     1001      123     5893 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/fund.rs
--rw-r--r--   0     1001      123      259 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/mod.rs
--rw-r--r--   0     1001      123     3948 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/option.rs
--rw-r--r--   0     1001      123     3290 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/security/security.rs
--rw-r--r--   0     1001      123     9354 2023-06-17 01:04:48.000000 finance_enums-0.2.3/src/trading/mod.rs
--rw-r--r--   0     1001      123    17385 2023-06-17 01:05:20.000000 finance_enums-0.2.3/Cargo.lock
--rw-r--r--   0        0        0     2720 1970-01-01 00:00:00.000000 finance_enums-0.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.752507 finance_enums-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-27 17:14:07.000000 finance_enums-0.3.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-06-27 17:14:07.000000 finance_enums-0.3.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-06-27 17:14:07.000000 finance_enums-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-27 17:14:07.000000 finance_enums-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-27 17:14:07.000000 finance_enums-0.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 17:14:27.752507 finance_enums-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-27 17:14:07.000000 finance_enums-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.748507 finance_enums-0.3.0/cpp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.748507 finance_enums-0.3.0/cpp/cmake/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.748507 finance_enums-0.3.0/cpp/cmake/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/cmake/config/FinanceEnums.pc.in
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/cmake/config/FinanceEnumsConfig.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.748507 finance_enums-0.3.0/cpp/cmake/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/cmake/modules/FindColor.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/cmake/modules/FindFinanceEnums.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/cmake/modules/FindNumPy.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/cmake/modules/FindPythonHeaders.cmake
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.748507 finance_enums-0.3.0/cpp/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.752507 finance_enums-0.3.0/cpp/include/finance-enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/bond.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/commodity.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/common.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   123996 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/country.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/currency.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/equity.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30928 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/exchange.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/finance-enums.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/fund.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/future.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.752507 finance_enums-0.3.0/cpp/include/finance-enums/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/helpers/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)    40558 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/helpers/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/helpers/exports.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/instrument.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/option.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.752507 finance_enums-0.3.0/cpp/include/finance-enums/python/
+-rw-r--r--   0 runner    (1001) docker     (123)    12050 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/python/extension.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    35455 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/python/long-enums.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    57891 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/sector-mappings.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    43039 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/sector.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/security.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/include/finance-enums/trading.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.752507 finance_enums-0.3.0/cpp/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/src/finance-enums.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.752507 finance_enums-0.3.0/cpp/src/python/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-27 17:14:07.000000 finance_enums-0.3.0/cpp/src/python/extension.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.752507 finance_enums-0.3.0/finance_enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-27 17:14:07.000000 finance_enums-0.3.0/finance_enums/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.752507 finance_enums-0.3.0/finance_enums/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-27 17:14:07.000000 finance_enums-0.3.0/finance_enums/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-27 17:14:07.000000 finance_enums-0.3.0/finance_enums/tests/test_country.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-27 17:14:07.000000 finance_enums-0.3.0/finance_enums/tests/test_currency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-27 17:14:07.000000 finance_enums-0.3.0/finance_enums/tests/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:07.000000 finance_enums-0.3.0/finance_enums/tests/test_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-27 17:14:07.000000 finance_enums-0.3.0/finance_enums/tests/test_sector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-27 17:14:07.000000 finance_enums-0.3.0/finance_enums/tests/test_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-27 17:14:07.000000 finance_enums-0.3.0/finance_enums/tests/test_trading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:14:27.752507 finance_enums-0.3.0/finance_enums.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-27 17:14:27.000000 finance_enums-0.3.0/finance_enums.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-27 17:14:27.000000 finance_enums-0.3.0/finance_enums.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:14:27.000000 finance_enums-0.3.0/finance_enums.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-27 17:14:27.000000 finance_enums-0.3.0/finance_enums.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-27 17:14:07.000000 finance_enums-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:14:27.752507 finance_enums-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-27 17:14:07.000000 finance_enums-0.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `finance_enums-0.2.3/LICENSE` & `finance_enums-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.3/README.md` & `finance_enums-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `finance_enums-0.2.3/finance_enums/tests/test_security.py` & `finance_enums-0.3.0/finance_enums/tests/test_security.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,32 +9,32 @@
     FundSubType,
     MutualFundEndedness,
 )
 
 
 class TestSecurityType:
     def test_security_type_basic(self):
-        assert len(SecurityType.members()) == 12
+        assert len(SecurityType.__members__) == 12
 
     def test_equity_type_basic(self):
-        assert len(EquityType.members()) == 5
+        assert len(EquityType.__members__) == 5
 
     def test_option_type_basic(self):
-        assert len(OptionType.members()) == 2
+        assert len(OptionType.__members__) == 2
 
     def test_bond_type_basic(self):
-        assert len(BondType.members()) == 3
+        assert len(BondType.__members__) == 3
 
     def test_commodity_type_basic(self):
-        assert len(CommodityType.members()) == 3
+        assert len(CommodityType.__members__) == 3
 
     def test_fund_type_basic(self):
-        assert len(FundType.members()) == 3
+        assert len(FundType.__members__) == 3
 
     def test_option_exercise_type_basic(self):
-        assert len(OptionExerciseType.members()) == 3
+        assert len(OptionExerciseType.__members__) == 3
 
     def test_fund_subtype_basic(self):
-        assert len(FundSubType.members()) == 4
+        assert len(FundSubType.__members__) == 4
 
     def test_mutual_fund_endedness_basic(self):
-        assert len(MutualFundEndedness.members()) == 2
+        assert len(MutualFundEndedness.__members__) == 2
```

### Comparing `finance_enums-0.2.3/finance_enums/tests/test_trading.py` & `finance_enums-0.3.0/finance_enums/tests/test_trading.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from finance_enums import OrderType, Side, TimeInForce, OrderFlag, TradingType
 
 
 class TestCurrency:
     def test_order_type_basic(self):
-        assert len(OrderType.members()) == 3
+        assert len(OrderType.__members__) == 3
 
     def test_side_basic(self):
-        assert len(Side.members()) == 2
+        assert len(Side.__members__) == 3
 
     def test_time_in_force_basic(self):
-        assert len(TimeInForce.members()) == 2
+        assert len(TimeInForce.__members__) == 3
 
     def test_order_flag_basic(self):
-        assert len(OrderFlag.members()) == 4
+        assert len(OrderFlag.__members__) == 4
 
     def test_trading_type_basic(self):
-        assert len(TradingType.members()) == 4
+        assert len(TradingType.__members__) == 4
```

