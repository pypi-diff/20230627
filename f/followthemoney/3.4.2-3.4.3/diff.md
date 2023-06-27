# Comparing `tmp/followthemoney-3.4.2.tar.gz` & `tmp/followthemoney-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "followthemoney-3.4.2.tar", last modified: Fri Jun 23 08:55:21 2023, max compression
+gzip compressed data, was "followthemoney-3.4.3.tar", last modified: Tue Jun 27 13:59:11 2023, max compression
```

## Comparing `followthemoney-3.4.2.tar` & `followthemoney-3.4.3.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.825806 followthemoney-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-23 08:53:27.000000 followthemoney-3.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-23 08:53:27.000000 followthemoney-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-23 08:55:21.825806 followthemoney-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-23 08:53:27.000000 followthemoney-3.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.809806 followthemoney-3.4.2/followthemoney/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.809806 followthemoney-3.4.2/followthemoney/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/sieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.809806 followthemoney-3.4.2/followthemoney/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/export/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.813806 followthemoney-3.4.2/followthemoney/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/mapping/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/offshore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/property.py
--rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.817806 followthemoney-3.4.2/followthemoney/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Address.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Airplane.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Analyzable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Article.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Assessment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Asset.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Associate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Audio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/BankAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/CallForTenders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Company.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Contract.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/ContractAward.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/CourtCase.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/CourtCaseParty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/CryptoWallet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Debt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Directorship.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Document.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/EconomicActivity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Email.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Employment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Event.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Family.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Folder.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/HyperText.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Identification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Image.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Interest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Interval.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/LegalEntity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/License.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Membership.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Mention.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Note.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Ownership.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Package.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Page.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Pages.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Passport.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Payment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Person.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/PlainText.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Post.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/ProjectParticipant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/PublicBody.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/RealEstate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Representation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Sanction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Security.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Similar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Succession.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/TaxRoll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Thing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Trip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/UnknownLink.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/UserAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Value.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Vehicle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Vessel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Video.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema/Workbook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.817806 followthemoney-3.4.2/followthemoney/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    38829 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   118608 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/bs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/bs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    93147 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    36107 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   112813 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   112460 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    42553 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   117244 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   106802 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/fr/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   100624 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89796 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    90876 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89847 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    60112 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   131502 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   130621 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/ru/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.805806 followthemoney-3.4.2/followthemoney/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.821807 followthemoney-3.4.2/followthemoney/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89829 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.825806 followthemoney-3.4.2/followthemoney/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/address.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/gender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/iban.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/mimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/types/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-23 08:53:27.000000 followthemoney-3.4.2/followthemoney/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 08:55:21.809806 followthemoney-3.4.2/followthemoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 08:55:01.000000 followthemoney-3.4.2/followthemoney.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 08:55:21.000000 followthemoney-3.4.2/followthemoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-23 08:55:21.825806 followthemoney-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-23 08:53:27.000000 followthemoney-3.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.782174 followthemoney-3.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-27 13:57:18.000000 followthemoney-3.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-27 13:57:18.000000 followthemoney-3.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-27 13:59:11.782174 followthemoney-3.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-27 13:57:18.000000 followthemoney-3.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.770174 followthemoney-3.4.3/followthemoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.770174 followthemoney-3.4.3/followthemoney/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/sieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.770174 followthemoney-3.4.3/followthemoney/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/export/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.770174 followthemoney-3.4.3/followthemoney/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/mapping/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/offshore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Address.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Airplane.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Analyzable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Article.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Assessment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Asset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Associate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Audio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/BankAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/CallForTenders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Company.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Contract.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/ContractAward.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/CourtCase.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/CourtCaseParty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/CryptoWallet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Debt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Directorship.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Document.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/EconomicActivity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Email.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Employment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Event.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Family.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Folder.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/HyperText.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Identification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Interest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Interval.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/LegalEntity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/License.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Membership.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Mention.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Note.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Ownership.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Page.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Passport.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Payment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Person.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/PlainText.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Post.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/ProjectParticipant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/PublicBody.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/RealEstate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Representation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Sanction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Security.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Similar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Succession.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/TaxRoll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Thing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Trip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/UnknownLink.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/UserAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Value.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Vehicle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Vessel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema/Workbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16469 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    38829 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   118608 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/bs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/bs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    93147 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    36107 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   112813 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   112460 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    42553 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   117244 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   106802 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/fr/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   100993 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89796 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    90876 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89847 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.778174 followthemoney-3.4.3/followthemoney/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.782174 followthemoney-3.4.3/followthemoney/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    61741 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   132454 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   130621 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/ru/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.766174 followthemoney-3.4.3/followthemoney/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.782174 followthemoney-3.4.3/followthemoney/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89829 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.782174 followthemoney-3.4.3/followthemoney/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/gender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/iban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/mimetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/types/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-27 13:57:18.000000 followthemoney-3.4.3/followthemoney/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 13:59:11.770174 followthemoney-3.4.3/followthemoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 13:58:52.000000 followthemoney-3.4.3/followthemoney.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 13:59:11.000000 followthemoney-3.4.3/followthemoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-27 13:59:11.782174 followthemoney-3.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-27 13:57:18.000000 followthemoney-3.4.3/setup.py
```

### Comparing `followthemoney-3.4.2/LICENSE` & `followthemoney-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/PKG-INFO` & `followthemoney-3.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.4.2
+Version: 3.4.3
 Summary: UNKNOWN
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `followthemoney-3.4.2/README.md` & `followthemoney-3.4.3/README.md`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/cli/aggregate.py` & `followthemoney-3.4.3/followthemoney/cli/aggregate.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/cli/cli.py` & `followthemoney-3.4.3/followthemoney/cli/cli.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/cli/exports.py` & `followthemoney-3.4.3/followthemoney/cli/exports.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/cli/mapping.py` & `followthemoney-3.4.3/followthemoney/cli/mapping.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/cli/sieve.py` & `followthemoney-3.4.3/followthemoney/cli/sieve.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/cli/util.py` & `followthemoney-3.4.3/followthemoney/cli/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/compare.py` & `followthemoney-3.4.3/followthemoney/compare.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/exc.py` & `followthemoney-3.4.3/followthemoney/exc.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/export/common.py` & `followthemoney-3.4.3/followthemoney/export/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/export/csv.py` & `followthemoney-3.4.3/followthemoney/export/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/export/excel.py` & `followthemoney-3.4.3/followthemoney/export/excel.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/export/graph.py` & `followthemoney-3.4.3/followthemoney/export/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/export/neo4j.py` & `followthemoney-3.4.3/followthemoney/export/neo4j.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/export/rdf.py` & `followthemoney-3.4.3/followthemoney/export/rdf.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/graph.py` & `followthemoney-3.4.3/followthemoney/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/helpers.py` & `followthemoney-3.4.3/followthemoney/helpers.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/mapping/csv.py` & `followthemoney-3.4.3/followthemoney/mapping/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/mapping/entity.py` & `followthemoney-3.4.3/followthemoney/mapping/entity.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/mapping/property.py` & `followthemoney-3.4.3/followthemoney/mapping/property.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/mapping/query.py` & `followthemoney-3.4.3/followthemoney/mapping/query.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/mapping/source.py` & `followthemoney-3.4.3/followthemoney/mapping/source.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/mapping/sql.py` & `followthemoney-3.4.3/followthemoney/mapping/sql.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/messages.py` & `followthemoney-3.4.3/followthemoney/messages.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/model.py` & `followthemoney-3.4.3/followthemoney/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,18 +40,17 @@
     def generate(self) -> None:
         """Loading the model is a weird process because the schemata reference
         each other in complex ways, so the generation process cannot be fully
         run as schemata are being instantiated. Hence this process needs to be
         called once all schemata are loaded to finalise dereferencing the
         schemata."""
         for schema in self:
-            schema.generate()
+            schema.generate(self)
         for prop in self.properties:
             self.qnames[prop.qname] = prop
-            # FIXME: stubs are not correctly assigned
             for schema in prop.schema.descendants:
                 if prop.name not in schema.properties:
                     schema.properties[prop.name] = prop
 
     def _load(self, filepath: str) -> None:
         with open(filepath, "r", encoding="utf-8") as fh:
             data = yaml.safe_load(fh)
```

### Comparing `followthemoney-3.4.2/followthemoney/namespace.py` & `followthemoney-3.4.3/followthemoney/namespace.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/offshore.py` & `followthemoney-3.4.3/followthemoney/offshore.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/ontology.py` & `followthemoney-3.4.3/followthemoney/ontology.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/property.py` & `followthemoney-3.4.3/followthemoney/property.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from followthemoney.exc import InvalidModel
 from followthemoney.types import registry
 from followthemoney.rdf import NS, URIRef
 from followthemoney.util import gettext, get_entity_id
 
 if TYPE_CHECKING:
     from followthemoney.schema import Schema
+    from followthemoney.model import Model
 
 
 class ReverseSpec(TypedDict, total=False):
     name: str
     label: Optional[str]
     hidden: Optional[bool]
 
@@ -62,16 +63,14 @@
         "uri",
     )
 
     #: Invalid property names.
     RESERVED = ["id", "caption", "schema", "schemata"]
 
     def __init__(self, schema: "Schema", name: str, data: PropertySpec) -> None:
-        self.model = schema.model
-
         #: The schema which the property is defined for. This is always the
         #: most abstract schema that has this property, not the possible
         #: child schemata that inherit it.
         self.schema = schema
 
         #: Machine-readable name for this property.
         self.name = name
@@ -120,27 +119,27 @@
         #: views.
         self._reverse = data.get("reverse")
         self.reverse: Optional["Property"] = None
 
         #: RDF term for this property (i.e. the predicate URI).
         self.uri = URIRef(cast(str, data.get("rdf", NS[self.qname])))
 
-    def generate(self) -> None:
+    def generate(self, model: "Model") -> None:
         """Setup method used when loading the model in order to build out the reverse
         links of the property."""
-        self.model.properties.add(self)
+        model.properties.add(self)
 
         if self.type == registry.entity:
             if self.range is None and self._range is not None:
-                self.range = self.model.get(self._range)
+                self.range = model.get(self._range)
 
             if self.reverse is None and self.range and self._reverse:
                 if not is_mapping(self._reverse):
                     raise InvalidModel("Invalid reverse: %s" % self)
-                self.reverse = self.range._add_reverse(self._reverse, self)
+                self.reverse = self.range._add_reverse(model, self._reverse, self)
 
     @property
     def label(self) -> str:
         """User-facing title for this property."""
         return gettext(self._label)
 
     @property
```

### Comparing `followthemoney-3.4.2/followthemoney/proxy.py` & `followthemoney-3.4.3/followthemoney/proxy.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Address.yaml` & `followthemoney-3.4.3/followthemoney/schema/Address.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Airplane.yaml` & `followthemoney-3.4.3/followthemoney/schema/Airplane.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Analyzable.yaml` & `followthemoney-3.4.3/followthemoney/schema/Analyzable.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Assessment.yaml` & `followthemoney-3.4.3/followthemoney/schema/Assessment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Associate.yaml` & `followthemoney-3.4.3/followthemoney/schema/Associate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/BankAccount.yaml` & `followthemoney-3.4.3/followthemoney/schema/BankAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Call.yaml` & `followthemoney-3.4.3/followthemoney/schema/Call.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/CallForTenders.yaml` & `followthemoney-3.4.3/followthemoney/schema/CallForTenders.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Company.yaml` & `followthemoney-3.4.3/followthemoney/schema/Company.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Contract.yaml` & `followthemoney-3.4.3/followthemoney/schema/Contract.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/ContractAward.yaml` & `followthemoney-3.4.3/followthemoney/schema/ContractAward.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/CourtCase.yaml` & `followthemoney-3.4.3/followthemoney/schema/CourtCase.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/CourtCaseParty.yaml` & `followthemoney-3.4.3/followthemoney/schema/CourtCaseParty.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/CryptoWallet.yaml` & `followthemoney-3.4.3/followthemoney/schema/CryptoWallet.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Debt.yaml` & `followthemoney-3.4.3/followthemoney/schema/Debt.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Directorship.yaml` & `followthemoney-3.4.3/followthemoney/schema/Directorship.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Document.yaml` & `followthemoney-3.4.3/followthemoney/schema/Document.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -108,14 +108,16 @@
     processingStatus:
       label: "Processing status"
       hidden: true
     processingError:
       label: "Processing error"
       hidden: true
     processingAgent:
-      label: "Name and version of the processing agent used to process the Document"
+      label: "Processing agent"
+      description: "Name and version of the processing agent used to process the Document"
       type: string
     processedAt:
-      label: "Date and time of the most recent ingestion of the Document"
+      label: "Processed at"
+      description: "Date and time of the most recent ingestion of the Document"
       type: date
       matchable: false
       hidden: true
```

### Comparing `followthemoney-3.4.2/followthemoney/schema/Documentation.yml` & `followthemoney-3.4.3/followthemoney/schema/Documentation.yml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/EconomicActivity.yaml` & `followthemoney-3.4.3/followthemoney/schema/EconomicActivity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Email.yaml` & `followthemoney-3.4.3/followthemoney/schema/Email.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Employment.yaml` & `followthemoney-3.4.3/followthemoney/schema/Employment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Event.yaml` & `followthemoney-3.4.3/followthemoney/schema/Event.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Family.yaml` & `followthemoney-3.4.3/followthemoney/schema/Family.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Identification.yaml` & `followthemoney-3.4.3/followthemoney/schema/Identification.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Interval.yaml` & `followthemoney-3.4.3/followthemoney/schema/Interval.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/LegalEntity.yaml` & `followthemoney-3.4.3/followthemoney/schema/LegalEntity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Membership.yaml` & `followthemoney-3.4.3/followthemoney/schema/Membership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Mention.yaml` & `followthemoney-3.4.3/followthemoney/schema/Mention.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Message.yaml` & `followthemoney-3.4.3/followthemoney/schema/Message.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Ownership.yaml` & `followthemoney-3.4.3/followthemoney/schema/Ownership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Page.yaml` & `followthemoney-3.4.3/followthemoney/schema/Page.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Passport.yaml` & `followthemoney-3.4.3/followthemoney/schema/Passport.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Payment.yaml` & `followthemoney-3.4.3/followthemoney/schema/Payment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Person.yaml` & `followthemoney-3.4.3/followthemoney/schema/Person.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Post.yaml` & `followthemoney-3.4.3/followthemoney/schema/Post.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/ProjectParticipant.yaml` & `followthemoney-3.4.3/followthemoney/schema/ProjectParticipant.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/RealEstate.yaml` & `followthemoney-3.4.3/followthemoney/schema/RealEstate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Representation.yaml` & `followthemoney-3.4.3/followthemoney/schema/Representation.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Sanction.yaml` & `followthemoney-3.4.3/followthemoney/schema/Sanction.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Security.yaml` & `followthemoney-3.4.3/followthemoney/schema/Security.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Similar.yaml` & `followthemoney-3.4.3/followthemoney/schema/Similar.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Succession.yaml` & `followthemoney-3.4.3/followthemoney/schema/Succession.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Table.yaml` & `followthemoney-3.4.3/followthemoney/schema/Table.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/TaxRoll.yaml` & `followthemoney-3.4.3/followthemoney/schema/TaxRoll.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Thing.yaml` & `followthemoney-3.4.3/followthemoney/schema/Thing.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Trip.yaml` & `followthemoney-3.4.3/followthemoney/schema/Trip.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/UnknownLink.yaml` & `followthemoney-3.4.3/followthemoney/schema/UnknownLink.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/UserAccount.yaml` & `followthemoney-3.4.3/followthemoney/schema/UserAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema/Vehicle.yaml` & `followthemoney-3.4.3/followthemoney/schema/Vehicle.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
   caption:
     - name
     - registrationNumber
   temporalExtent:
     start:
       - buildDate
       - registrationDate
+    end:
+      - deregistrationDate
   properties:
     registrationNumber:
       label: Registration number
       type: identifier
     type:
       label: Type
     model:
@@ -40,7 +42,10 @@
         label: "Vehicles operated"
     buildDate:
       label: Build Date
       type: date
     registrationDate:
       label: Registration Date
       type: date
+    deregistrationDate:
+      label: De-registration Date
+      type: date
```

### Comparing `followthemoney-3.4.2/followthemoney/schema/Vessel.yaml` & `followthemoney-3.4.3/followthemoney/schema/Vessel.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/schema.py` & `followthemoney-3.4.3/followthemoney/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,22 +196,22 @@
 
         #: The full list of properties defined for the entity, including those
         #: inherited from parent schemata.
         self.properties: Dict[str, Property] = {}
         for name, prop in data.get("properties", {}).items():
             self.properties[name] = Property(self, name, prop)
 
-    def generate(self) -> None:
+    def generate(self, model: "Model") -> None:
         """While loading the schema, this function will validate and
         load the hierarchy, properties, and flags of the definition."""
         for extends in self._extends:
-            parent = self.model.get(extends)
+            parent = model.get(extends)
             if parent is None:
                 raise InvalidData("Invalid extends: %r" % extends)
-            parent.generate()
+            parent.generate(model)
 
             for name, prop in parent.properties.items():
                 if name not in self.properties:
                     self.properties[name] = prop
 
             self.extends.add(parent)
             for ancestor in parent.schemata:
@@ -219,15 +219,15 @@
                 self.names.add(ancestor.name)
                 ancestor.descendants.add(self)
 
             self.temporal_start |= parent.temporal_start
             self.temporal_end |= parent.temporal_end
 
         for prop in list(self.properties.values()):
-            prop.generate()
+            prop.generate(model)
 
         for featured in self.featured:
             if self.get(featured) is None:
                 raise InvalidModel("Missing featured property: %s" % featured)
 
         for caption in self.caption:
             prop_ = self.get(caption)
@@ -245,15 +245,17 @@
                 msg = "Missing edge source: %s" % self.edge_source
                 raise InvalidModel(msg)
 
             if self.target_prop is None:
                 msg = "Missing edge target: %s" % self.edge_target
                 raise InvalidModel(msg)
 
-    def _add_reverse(self, data: ReverseSpec, other: Property) -> Property:
+    def _add_reverse(
+        self, model: "Model", data: ReverseSpec, other: Property
+    ) -> Property:
         name = data.get("name")
         if name is None:
             raise InvalidModel("Unnamed reverse: %s" % other)
 
         prop = self.get(name)
         if prop is None:
             spec: PropertySpec = {
@@ -261,15 +263,15 @@
                 "type": registry.entity.name,
                 "reverse": {"name": other.name},
                 "range": other.schema.name,
                 "hidden": data.get("hidden", other.hidden),
             }
             prop = Property(self, name, spec)
             prop.stub = True
-            prop.generate()
+            prop.generate(model)
             self.properties[name] = prop
         return prop
 
     @property
     def label(self) -> str:
         """User-facing name of the schema."""
         return gettext(self._label)
@@ -347,15 +349,17 @@
         """Check if an schema can match with another schema."""
         return other in self.matchable_schemata
 
     @lru_cache(maxsize=None)
     def is_a(self, other: Union[str, "Schema"]) -> bool:
         """Check if the schema or one of its parents is the same as the given
         candidate ``other``."""
-        return self.model.get(other) in self.schemata
+        if not isinstance(other, str):
+            other = other.name
+        return other in self.names
 
     def get(self, name: Optional[str]) -> Optional[Property]:
         """Retrieve a property defined for this schema by its name."""
         if name is None:
             return None
         return self.properties.get(name)
```

### Comparing `followthemoney-3.4.2/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.3/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: ar\n"
 "Language-Team: Arabic (https://app.transifex.com/aleph/teams/76591/ar/)\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "(EU) VAT number"
 msgstr "الرقم الضريبي (الاتحاد الأوروبي)"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr "  (RO) ما هو نوع النشاط الذي يسمح للكيان القانوني بتطويره"
```

### Comparing `followthemoney-3.4.2/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.3/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.3/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: bs\n"
 "Language-Team: Bosnian (https://www.transifex.com/aleph/teams/76591/bs/)\n"
 "Plural-Forms: nplurals=3; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "(EU) VAT number"
 msgstr "(EU) VAT broj"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr "(RO) Koji tip aktivnosti legalnog entiteta je dozvoljeno razviti"
```

### Comparing `followthemoney-3.4.2/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.3/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.3/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Last-Translator: pudo <friedrich@pudo.org>, 2021\n"
 "Language: de\n"
 "Language-Team: German (https://app.transifex.com/aleph/teams/76591/de/)\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "(EU) VAT number"
 msgstr "(EU) USt-ID"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr ""
 "(RO) Die Art der wirtschaftlichen Tätigkeit, der diese Entität nachgehen darf"
```

### Comparing `followthemoney-3.4.2/followthemoney/translations/de/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.3/followthemoney/translations/de/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.3/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: es\n"
 "Language-Team: Spanish (https://app.transifex.com/aleph/teams/76591/es/)\n"
 "Plural-Forms: nplurals=3; plural=n == 1 ? 0 : n != 0 && n % 1000000 == 0 ? "
 "1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "(EU) VAT number"
 msgstr "(EU) Número VAT"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr ""
 "(RO) ¿Qué tipo de actividad se le permite desarrollar a una entidad legal?"
```

### Comparing `followthemoney-3.4.2/followthemoney/translations/es/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.3/followthemoney/translations/es/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.3/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "Language: fr\n"
 "Language-Team: French (https://app.transifex.com/aleph/teams/76591/fr/)\n"
 "Plural-Forms: nplurals=3; plural=(n == 0 || n == 1) ? 0 : n != 0 && n % "
 "1000000 == 0 ? 1 : 2;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "(EU) VAT number"
 msgstr "Numéro de TVA intracommunautaire"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr "(RO) Type d’activité qu’une entité légale est autorisée à mener"
```

### Comparing `followthemoney-3.4.2/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.3/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/translations/fr/followthemoney.po` & `followthemoney-3.4.3/followthemoney/translations/fr/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/translations/messages.pot` & `followthemoney-3.4.3/followthemoney/translations/messages.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-06-23 10:41+0200\n"
+"POT-Creation-Date: 2023-06-27 15:36+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 
-#: followthemoney/property.py:166
+#: followthemoney/property.py:165
 msgid "Property cannot be written"
 msgstr ""
 
-#: followthemoney/property.py:169
+#: followthemoney/property.py:168
 msgid "Invalid value"
 msgstr ""
 
 #: followthemoney/proxy.py:62
 msgid "No schema for entity."
 msgstr ""
 
@@ -35,19 +35,19 @@
 msgstr ""
 
 #: followthemoney/proxy.py:188
 #, python-format
 msgid "Stub property (%s): %s"
 msgstr ""
 
-#: followthemoney/schema.py:373
+#: followthemoney/schema.py:377
 msgid "Required"
 msgstr ""
 
-#: followthemoney/schema.py:377
+#: followthemoney/schema.py:381
 msgid "Entity validation failed"
 msgstr ""
 
 #. Address.label
 #. CryptoWallet.properties.publicKey.label
 #. Thing.properties.address.label
 #. Thing.properties.addressEntity.label
@@ -1566,19 +1566,29 @@
 #. Document.properties.processingError.label
 #: followthemoney/schema/Document.yaml
 msgid "Processing error"
 msgstr ""
 
 #. Document.properties.processingAgent.label
 #: followthemoney/schema/Document.yaml
+msgid "Processing agent"
+msgstr ""
+
+#. Document.properties.processingAgent.description
+#: followthemoney/schema/Document.yaml
 msgid "Name and version of the processing agent used to process the Document"
 msgstr ""
 
 #. Document.properties.processedAt.label
 #: followthemoney/schema/Document.yaml
+msgid "Processed at"
+msgstr ""
+
+#. Document.properties.processedAt.description
+#: followthemoney/schema/Document.yaml
 msgid "Date and time of the most recent ingestion of the Document"
 msgstr ""
 
 #. Documentation.label
 #: followthemoney/schema/Documentation.yml
 msgid "Documentation"
 msgstr ""
@@ -3697,14 +3707,19 @@
 msgstr ""
 
 #. Vehicle.properties.registrationDate.label
 #: followthemoney/schema/Vehicle.yaml
 msgid "Registration Date"
 msgstr ""
 
+#. Vehicle.properties.deregistrationDate.label
+#: followthemoney/schema/Vehicle.yaml
+msgid "De-registration Date"
+msgstr ""
+
 #. Vessel.label
 #: followthemoney/schema/Vessel.yaml
 msgid "Vessel"
 msgstr ""
 
 #. Vessel.plural
 #: followthemoney/schema/Vessel.yaml
```

### Comparing `followthemoney-3.4.2/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.3/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.3/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.3/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.3/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,23 +1,23 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2023-06-23 10:41+0200\n"
-"PO-Revision-Date: 2021-05-07 13:11+0000\n"
+"PO-Revision-Date: 2022-11-21 11:38+0000\n"
 "Last-Translator: jen occrp, 2023\n"
 "Language: ru\n"
 "Language-Team: Russian (https://app.transifex.com/aleph/teams/76591/ru/)\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.12.1\n"
+"Generated-By: Babel 2.11.0\n"
 
 msgid "(EU) VAT number"
 msgstr "(ЕС) Регистрационный номер плательщика НДС"
 
 msgid "(RO) What kind of activity a legal entity is allowed to develop"
 msgstr "(RO) Классификатор экономической деятельности"
 
@@ -101,14 +101,17 @@
 msgstr ""
 "Связь между двумя предположительно тождественными сущностями, например, в "
 "результате вероятностного сопоставления записей.\n"
 
 msgid "A location associated with an entity.\n"
 msgstr "Местоположение, ассоциированное с сущностью.\n"
 
+msgid "A mailbox identifier at the post office"
+msgstr "Номер абонентского ящика в почтовом отделении"
+
 msgid ""
 "A mediatory, intermediary, middleman, or broker acting on behalf of a legal "
 "entity."
 msgstr "Медиатор, посредник или брокер юридического лица"
 
 msgid "A monetary debt between two parties."
 msgstr "Кредитно-денежные отношения двух сторон."
@@ -311,14 +314,23 @@
 "Any party to legal proceedings, such as asset ownership, corporate "
 "governance or social interactions. Often used when raw data does not specify "
 "if something is a person or company.\n"
 msgstr ""
 "Любой участник судопроизводства, как то: владения (активами), корпоративного "
 "контроля или социального взаимодействия.\n"
 
+msgid ""
+"Any type of incorporated entity that cannot be owned by another (see "
+"Company). This might include charities, foundations or state-owned "
+"enterprises, depending on their  jurisdiction.\n"
+msgstr ""
+"Любой тип юридического лица, который не может быть объектом собственности "
+"(см. Компания). Например, благотворительные организации, фонды или "
+"государственные предприятия, в зависимости от юрисдикции.\n"
+
 msgid "Area"
 msgstr "Участок"
 
 msgid "Article"
 msgstr "Статья"
 
 msgid "Articles"
@@ -779,14 +791,17 @@
 
 msgid "D-U-N-S"
 msgstr "D-U-N-S-код"
 
 msgid "Date"
 msgstr "Дата"
 
+msgid "Date and time of the most recent ingestion of the Document"
+msgstr "Дата и время последней загрузки документа"
+
 msgid "Date issued"
 msgstr "Дата размещения"
 
 msgid "Date of Name Change"
 msgstr "Дата изменения названия судна"
 
 msgid "Date of awarding"
@@ -1520,14 +1535,17 @@
 
 msgid "Nagorno-Karabakh"
 msgstr "Нагорный Карабах"
 
 msgid "Name"
 msgstr "Имя"
 
+msgid "Name and version of the processing agent used to process the Document"
+msgstr "Имя и версия обработчика документа"
+
 msgid "Name of contracting authority"
 msgstr "Наименование заказчика"
 
 msgid "Names"
 msgstr "Имена"
 
 msgid "National government"
@@ -1782,14 +1800,17 @@
 
 msgid "Pictured"
 msgstr "На изображении"
 
 msgid "Place of birth"
 msgstr "Место рождения"
 
+msgid "Political"
+msgstr "Политик"
+
 msgid "Political association"
 msgstr "Политическая ассоциация"
 
 msgid "Political party"
 msgstr "Политическая партия"
 
 msgid "Port of Registration"
@@ -1977,14 +1998,17 @@
 
 msgid "Role"
 msgstr "Роль, функция"
 
 msgid "Rouble bank"
 msgstr "Наименование банка (рубли)"
 
+msgid "Russian (ОКСМ) countries classifier"
+msgstr "Общероссийский классификатор стран мира"
+
 msgid "Russian bank account code"
 msgstr "Банковский идентификационный код"
 
 msgid "Russian company ID"
 msgstr "Идентификационный номер налогоплательщика"
 
 msgid "Russian industry classifier"
@@ -2004,14 +2028,17 @@
 
 msgid "Sampling rate of the audio in Hz"
 msgstr "Частота дискретизации аудио (Гц)"
 
 msgid "Sanction"
 msgstr "Санкция"
 
+msgid "Sanction-linked entity"
+msgstr "Подсанкционное физическое или юридическое лицо"
+
 msgid "Sanctioned entity"
 msgstr "Объект санкций"
 
 msgid "Sanctions"
 msgstr "Санкции"
 
 msgid "Sark"
@@ -2085,14 +2112,21 @@
 
 msgid "South Ossetia (Occupied Georgia)"
 msgstr "Южная Осетия (оккупированная территория Грузии)"
 
 msgid "Soviet Union"
 msgstr "Советский Союз"
 
+msgid ""
+"Soviet classifier for territories, regions, districts, villages. Aka. SOATO "
+"and same as OKATO"
+msgstr ""
+"Система обозначения объектов административно-территориального деления (также "
+"ОКАТО)"
+
 msgid "Spy"
 msgstr "Шпион"
 
 msgid "Start date"
 msgstr "Дата начала"
 
 msgid "Start location"
@@ -2109,14 +2143,17 @@
 
 msgid "State-owned enterprise"
 msgstr "Государственное предприятие"
 
 msgid "Status"
 msgstr "Статус"
 
+msgid "Stock ticker symbol"
+msgstr "Тикер"
+
 msgid "Street address"
 msgstr "Адрес (улица)"
 
 msgid "Street address (ctd.)"
 msgstr "Контактный адрес (улица)"
 
 msgid "Stub property (%s): %s"
```

### Comparing `followthemoney-3.4.2/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.3/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # Translations template for PROJECT.
 # Copyright (C) 2023 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 # 
 # Translators:
-# pudo <friedrich@pudo.org>, 2021
+# pudo <friedrich@pudo.org>, 2022
 # jen occrp, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
 "POT-Creation-Date: 2023-06-23 10:41+0200\n"
-"PO-Revision-Date: 2021-05-07 13:11+0000\n"
+"PO-Revision-Date: 2022-11-21 11:38+0000\n"
 "Last-Translator: jen occrp, 2023\n"
 "Language-Team: Russian (https://app.transifex.com/aleph/teams/76591/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
 "Language: ru\n"
@@ -91,15 +91,15 @@
 #: followthemoney/schema/Address.yaml
 msgid "PO Box"
 msgstr "Абонентский ящик"
 
 #. Address.properties.postOfficeBox.description
 #: followthemoney/schema/Address.yaml
 msgid "A mailbox identifier at the post office"
-msgstr ""
+msgstr "Номер абонентского ящика в почтовом отделении"
 
 #. Address.properties.street.label
 #: followthemoney/schema/Address.yaml
 msgid "Street address"
 msgstr "Адрес (улица)"
 
 #. Address.properties.street2.label
@@ -861,14 +861,16 @@
 
 #. Company.properties.coatoCode.description
 #: followthemoney/schema/Company.yaml
 msgid ""
 "Soviet classifier for territories, regions, districts, villages. Aka. SOATO "
 "and same as OKATO"
 msgstr ""
+"Система обозначения объектов административно-территориального деления (также"
+" ОКАТО)"
 
 #. Company.properties.irsCode.label
 #: followthemoney/schema/Company.yaml
 msgid "IRS Number"
 msgstr "ИНН"
 
 #. Company.properties.irsCode.description
@@ -1000,15 +1002,15 @@
 #: followthemoney/schema/Company.yaml
 msgid "OKSM"
 msgstr "ОКСМ"
 
 #. Company.properties.oksmCode.description
 #: followthemoney/schema/Company.yaml
 msgid "Russian (ОКСМ) countries classifier"
-msgstr ""
+msgstr "Общероссийский классификатор стран мира"
 
 #. Company.properties.isinCode.label
 #. Security.properties.isin.label
 #: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
 msgid "ISIN"
 msgstr "ISIN-код"
 
@@ -1018,15 +1020,15 @@
 msgid "International Securities Identification Number"
 msgstr "Международный идентификационный код ценной бумаги"
 
 #. Company.properties.ticker.label
 #. Security.properties.ticker.label
 #: followthemoney/schema/Company.yaml followthemoney/schema/Security.yaml
 msgid "Stock ticker symbol"
-msgstr ""
+msgstr "Тикер"
 
 #. Contract.label
 #. ContractAward.properties.contract.label
 #. EconomicActivity.properties.contract.label
 #. Payment.properties.contract.label
 #: followthemoney/schema/Contract.yaml
 #: followthemoney/schema/ContractAward.yaml
@@ -1600,20 +1602,20 @@
 #: followthemoney/schema/Document.yaml
 msgid "Processing error"
 msgstr "Ошибка обработки"
 
 #. Document.properties.processingAgent.label
 #: followthemoney/schema/Document.yaml
 msgid "Name and version of the processing agent used to process the Document"
-msgstr ""
+msgstr "Имя и версия обработчика документа"
 
 #. Document.properties.processedAt.label
 #: followthemoney/schema/Document.yaml
 msgid "Date and time of the most recent ingestion of the Document"
-msgstr ""
+msgstr "Дата и время последней загрузки документа"
 
 #. Documentation.label
 #: followthemoney/schema/Documentation.yml
 msgid "Documentation"
 msgstr "Документация"
 
 #. Documentation.plural
@@ -2725,14 +2727,17 @@
 #. Organization.description
 #: followthemoney/schema/Organization.yaml
 msgid ""
 "Any type of incorporated entity that cannot be owned by another (see "
 "Company). This might include charities, foundations or state-owned "
 "enterprises, depending on their  jurisdiction.\n"
 msgstr ""
+"Любой тип юридического лица, который не может быть объектом собственности "
+"(см. Компания). Например, благотворительные организации, фонды или "
+"государственные предприятия, в зависимости от юрисдикции.\n"
 
 #. Ownership.label
 #: followthemoney/schema/Ownership.yaml
 msgid "Ownership"
 msgstr "Структура собственности"
 
 #. Ownership.plural
@@ -4169,15 +4174,15 @@
 
 #: followthemoney/types/topic.py:48
 msgid "Financial advisor"
 msgstr "Финансовый консультант"
 
 #: followthemoney/types/topic.py:49
 msgid "Political"
-msgstr ""
+msgstr "Политик"
 
 #: followthemoney/types/topic.py:50
 msgid "Close Associate"
 msgstr "Тесно связанное лицо"
 
 #: followthemoney/types/topic.py:51
 msgid "Judge"
@@ -4233,15 +4238,15 @@
 
 #: followthemoney/types/topic.py:65
 msgid "Sanctioned entity"
 msgstr "Объект санкций"
 
 #: followthemoney/types/topic.py:66
 msgid "Sanction-linked entity"
-msgstr ""
+msgstr "Подсанкционное физическое или юридическое лицо"
 
 #: followthemoney/types/topic.py:67
 msgid "Debarred entity"
 msgstr "Физическое или юридическое лицо, лишённое полномочий"
 
 #: followthemoney/types/topic.py:68
 msgid "Person of interest"
```

### Comparing `followthemoney-3.4.2/followthemoney/translations/ru/followthemoney.po` & `followthemoney-3.4.3/followthemoney/translations/ru/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.3/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/__init__.py` & `followthemoney-3.4.3/followthemoney/types/__init__.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/address.py` & `followthemoney-3.4.3/followthemoney/types/address.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/checksum.py` & `followthemoney-3.4.3/followthemoney/types/checksum.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/common.py` & `followthemoney-3.4.3/followthemoney/types/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/country.py` & `followthemoney-3.4.3/followthemoney/types/country.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/date.py` & `followthemoney-3.4.3/followthemoney/types/date.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/email.py` & `followthemoney-3.4.3/followthemoney/types/email.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/entity.py` & `followthemoney-3.4.3/followthemoney/types/entity.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/gender.py` & `followthemoney-3.4.3/followthemoney/types/gender.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/iban.py` & `followthemoney-3.4.3/followthemoney/types/iban.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/identifier.py` & `followthemoney-3.4.3/followthemoney/types/identifier.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/ip.py` & `followthemoney-3.4.3/followthemoney/types/ip.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/json.py` & `followthemoney-3.4.3/followthemoney/types/json.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/language.py` & `followthemoney-3.4.3/followthemoney/types/language.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/mimetype.py` & `followthemoney-3.4.3/followthemoney/types/mimetype.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/name.py` & `followthemoney-3.4.3/followthemoney/types/name.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/number.py` & `followthemoney-3.4.3/followthemoney/types/number.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/phone.py` & `followthemoney-3.4.3/followthemoney/types/phone.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/registry.py` & `followthemoney-3.4.3/followthemoney/types/registry.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/string.py` & `followthemoney-3.4.3/followthemoney/types/string.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/topic.py` & `followthemoney-3.4.3/followthemoney/types/topic.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/types/url.py` & `followthemoney-3.4.3/followthemoney/types/url.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney/util.py` & `followthemoney-3.4.3/followthemoney/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney.egg-info/PKG-INFO` & `followthemoney-3.4.3/followthemoney.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.4.2
+Version: 3.4.3
 Summary: UNKNOWN
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `followthemoney-3.4.2/followthemoney.egg-info/SOURCES.txt` & `followthemoney-3.4.3/followthemoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney.egg-info/entry_points.txt` & `followthemoney-3.4.3/followthemoney.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/followthemoney.egg-info/requires.txt` & `followthemoney-3.4.3/followthemoney.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `followthemoney-3.4.2/setup.py` & `followthemoney-3.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages  # type: ignore
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="followthemoney",
-    version="3.4.2",
+    version="3.4.3",
     author="Organized Crime and Corruption Reporting Project",
     author_email="data@occrp.org",
     url="https://followthemoney.tech/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
```

