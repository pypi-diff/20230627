# Comparing `tmp/Openfisca-Paris-4.0.1.tar.gz` & `tmp/Openfisca-Paris-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Openfisca-Paris-4.0.1.tar", last modified: Tue Jun 27 10:23:05 2023, max compression
+gzip compressed data, was "Openfisca-Paris-4.0.2.tar", last modified: Tue Jun 27 12:34:16 2023, max compression
```

## Comparing `Openfisca-Paris-4.0.1.tar` & `Openfisca-Paris-4.0.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.670545 Openfisca-Paris-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/LICENSE.AGPL.txt
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.662545 Openfisca-Paris-4.0.1/Openfisca_Paris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      793 2023-06-27 10:23:05.000000 Openfisca-Paris-4.0.1/Openfisca_Paris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3595 2023-06-27 10:23:05.000000 Openfisca-Paris-4.0.1/Openfisca_Paris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 10:23:05.000000 Openfisca-Paris-4.0.1/Openfisca_Paris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-27 10:23:05.000000 Openfisca-Paris-4.0.1/Openfisca_Paris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-27 10:23:05.000000 Openfisca-Paris-4.0.1/Openfisca_Paris.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      793 2023-06-27 10:23:05.670545 Openfisca-Paris-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2097 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.662545 Openfisca-Paris-4.0.1/openfisca_paris/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.662545 Openfisca-Paris-4.0.1/openfisca_paris/familles/
--rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/familles/aspeh.py
--rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/familles/paris_energie_familles.py
--rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/familles/paris_forfait_familles.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.658545 Openfisca-Paris-4.0.1/openfisca_paris/parameters/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.662545 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.662545 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/familles/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.662545 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/familles/aspeh/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/familles/aspeh/aide_aspeh.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/familles/aspeh/plafond_aspeh.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/familles/paris_energie_familles.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/familles/paris_forfait_familles.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.666545 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement/
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement/aide_couple_avec_enf.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      141 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement/aide_couple_ss_enf.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement/aide_pers_isol.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement/aide_pl_apd_couple.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement/aide_pl_apd_pers_isol.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement/aide_pl_fam.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement/plafond_pl.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement/plafond_pl_apd.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement/plafond_pl_avec_enf.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement/plafond_pl_fam.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      161 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement/taux_effort_min.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.666545 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement_familles/
--rw-r--r--   0 runner    (1001) docker     (122)      145 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement_familles/montant_2enf.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement_familles/montant_bas_3enf.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement_familles/montant_bas_enf_sup.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      142 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement_familles/montant_haut_3enf.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement_familles/montant_haut_enf_sup.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement_familles/plafond_2enf.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      150 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement_familles/plafond_bas_3enf.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      198 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_logement_familles/plafond_haut_3enf.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/paris_pass.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.666545 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/personnes_agees/
--rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/personnes_agees/paris_complement_sante.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/personnes_agees/paris_logement.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/personnes_agees/personnes_agees.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      495 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/personnes_agees/psol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.666545 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/personnes_handicapees/
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/personnes_handicapees/paris_complement_sante.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/personnes_handicapees/psol.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.670545 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/plfm/
--rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/plfm/aide_1er_plafond_plfm.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      136 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/plfm/aide_2eme_plafond_plfm.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/plfm/deuxieme_plafond_plfm.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      229 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/plfm/premier_plafond_plfm.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/smic_net_mensuel.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    10499 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/paris.py
--rw-r--r--   0 runner    (1001) docker     (122)      713 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/paris_complement_sante.py
--rw-r--r--   0 runner    (1001) docker     (122)     9335 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/paris_logement.py
--rw-r--r--   0 runner    (1001) docker     (122)     4975 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/paris_logement_fam.py
--rw-r--r--   0 runner    (1001) docker     (122)     2362 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/paris_logement_fam_mono.py
--rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/paris_pass.py
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/paris_solidarite.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.670545 Openfisca-Paris-4.0.1/openfisca_paris/personnes_agees/
--rw-r--r--   0 runner    (1001) docker     (122)     1986 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/personnes_agees/paris_complement_sante.py
--rw-r--r--   0 runner    (1001) docker     (122)     3248 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/personnes_agees/paris_logement.py
--rw-r--r--   0 runner    (1001) docker     (122)      582 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/personnes_agees/paris_pass_seniors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/personnes_agees/personnes_agees.py
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/personnes_agees/psol.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 10:23:05.670545 Openfisca-Paris-4.0.1/openfisca_paris/personnes_handicapees/
--rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/personnes_handicapees/paris_complement_sante.py
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/personnes_handicapees/paris_pass_access.py
--rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/personnes_handicapees/personne_handicapee.py
--rw-r--r--   0 runner    (1001) docker     (122)     2808 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/openfisca_paris/personnes_handicapees/psol.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 10:23:05.670545 Openfisca-Paris-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-06-27 10:22:31.000000 Openfisca-Paris-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.243126 Openfisca-Paris-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    34519 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/LICENSE.AGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.231126 Openfisca-Paris-4.0.2/Openfisca_Paris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2023-06-27 12:34:16.000000 Openfisca-Paris-4.0.2/Openfisca_Paris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3595 2023-06-27 12:34:16.000000 Openfisca-Paris-4.0.2/Openfisca_Paris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-27 12:34:16.000000 Openfisca-Paris-4.0.2/Openfisca_Paris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-27 12:34:16.000000 Openfisca-Paris-4.0.2/Openfisca_Paris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       44 2023-06-27 12:34:16.000000 Openfisca-Paris-4.0.2/Openfisca_Paris.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      793 2023-06-27 12:34:16.243126 Openfisca-Paris-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2097 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.231126 Openfisca-Paris-4.0.2/openfisca_paris/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.235126 Openfisca-Paris-4.0.2/openfisca_paris/familles/
+-rw-r--r--   0 runner    (1001) docker     (122)     1427 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/familles/aspeh.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3022 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/familles/paris_energie_familles.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1732 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/familles/paris_forfait_familles.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.227126 Openfisca-Paris-4.0.2/openfisca_paris/parameters/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.235126 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.235126 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/familles/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.235126 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/familles/aspeh/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/familles/aspeh/aide_aspeh.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/familles/aspeh/plafond_aspeh.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      654 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/familles/paris_energie_familles.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/familles/paris_forfait_familles.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.239126 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement/
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement/aide_couple_avec_enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement/aide_couple_ss_enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement/aide_pers_isol.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement/aide_pl_apd_couple.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement/aide_pl_apd_pers_isol.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement/aide_pl_fam.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      251 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement/plafond_pl.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      257 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement/plafond_pl_apd.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement/plafond_pl_avec_enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement/plafond_pl_fam.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement/taux_effort_min.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.239126 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement_familles/
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement_familles/montant_2enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement_familles/montant_bas_3enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement_familles/montant_bas_enf_sup.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement_familles/montant_haut_3enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement_familles/montant_haut_enf_sup.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement_familles/plafond_2enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      150 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement_familles/plafond_bas_3enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      198 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_logement_familles/plafond_haut_3enf.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      148 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/paris_pass.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.239126 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/personnes_agees/
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/personnes_agees/paris_complement_sante.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/personnes_agees/paris_logement.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/personnes_agees/personnes_agees.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/personnes_agees/psol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.239126 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/personnes_handicapees/
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/personnes_handicapees/paris_complement_sante.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      455 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/personnes_handicapees/psol.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.243126 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/plfm/
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/plfm/aide_1er_plafond_plfm.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      136 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/plfm/aide_2eme_plafond_plfm.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/plfm/deuxieme_plafond_plfm.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/plfm/premier_plafond_plfm.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/smic_net_mensuel.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    10499 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/paris.py
+-rw-r--r--   0 runner    (1001) docker     (122)      713 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/paris_complement_sante.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9335 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/paris_logement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4975 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/paris_logement_fam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2362 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/paris_logement_fam_mono.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1594 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/paris_pass.py
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/paris_solidarite.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.243126 Openfisca-Paris-4.0.2/openfisca_paris/personnes_agees/
+-rw-r--r--   0 runner    (1001) docker     (122)     1986 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/personnes_agees/paris_complement_sante.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3248 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/personnes_agees/paris_logement.py
+-rw-r--r--   0 runner    (1001) docker     (122)      582 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/personnes_agees/paris_pass_seniors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/personnes_agees/personnes_agees.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/personnes_agees/psol.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-27 12:34:16.243126 Openfisca-Paris-4.0.2/openfisca_paris/personnes_handicapees/
+-rw-r--r--   0 runner    (1001) docker     (122)     2239 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/personnes_handicapees/paris_complement_sante.py
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/personnes_handicapees/paris_pass_access.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1175 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/personnes_handicapees/personne_handicapee.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2808 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/openfisca_paris/personnes_handicapees/psol.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-27 12:34:16.243126 Openfisca-Paris-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1166 2023-06-27 12:33:33.000000 Openfisca-Paris-4.0.2/setup.py
```

### Comparing `Openfisca-Paris-4.0.1/LICENSE.AGPL.txt` & `Openfisca-Paris-4.0.2/LICENSE.AGPL.txt`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/Openfisca_Paris.egg-info/PKG-INFO` & `Openfisca-Paris-4.0.2/Openfisca_Paris.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Openfisca-Paris
-Version: 4.0.1
+Version: 4.0.2
 Summary: Plugin OpenFisca pour les aides sociales de la mairie de Paris
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: benefit france paris microsimulation social tax
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `Openfisca-Paris-4.0.1/Openfisca_Paris.egg-info/SOURCES.txt` & `Openfisca-Paris-4.0.2/Openfisca_Paris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/PKG-INFO` & `Openfisca-Paris-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Openfisca-Paris
-Version: 4.0.1
+Version: 4.0.2
 Summary: Plugin OpenFisca pour les aides sociales de la mairie de Paris
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: benefit france paris microsimulation social tax
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `Openfisca-Paris-4.0.1/README.md` & `Openfisca-Paris-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/familles/aspeh.py` & `Openfisca-Paris-4.0.2/openfisca_paris/familles/aspeh.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/familles/paris_energie_familles.py` & `Openfisca-Paris-4.0.2/openfisca_paris/familles/paris_energie_familles.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/familles/paris_forfait_familles.py` & `Openfisca-Paris-4.0.2/openfisca_paris/familles/paris_forfait_familles.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/familles/paris_energie_familles.yaml` & `Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/familles/paris_energie_familles.yaml`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/familles/paris_forfait_familles.yaml` & `Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/familles/paris_forfait_familles.yaml`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/personnes_agees/paris_complement_sante.yaml` & `Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/personnes_agees/paris_complement_sante.yaml`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/parameters/paris/personnes_agees/paris_logement.yaml` & `Openfisca-Paris-4.0.2/openfisca_paris/parameters/paris/personnes_agees/paris_logement.yaml`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/paris.py` & `Openfisca-Paris-4.0.2/openfisca_paris/paris.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/paris_complement_sante.py` & `Openfisca-Paris-4.0.2/openfisca_paris/paris_complement_sante.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/paris_logement.py` & `Openfisca-Paris-4.0.2/openfisca_paris/paris_logement.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/paris_logement_fam.py` & `Openfisca-Paris-4.0.2/openfisca_paris/paris_logement_fam.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/paris_logement_fam_mono.py` & `Openfisca-Paris-4.0.2/openfisca_paris/paris_logement_fam_mono.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/paris_pass.py` & `Openfisca-Paris-4.0.2/openfisca_paris/paris_pass.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/paris_solidarite.py` & `Openfisca-Paris-4.0.2/openfisca_paris/paris_solidarite.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/personnes_agees/paris_complement_sante.py` & `Openfisca-Paris-4.0.2/openfisca_paris/personnes_agees/paris_complement_sante.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/personnes_agees/paris_logement.py` & `Openfisca-Paris-4.0.2/openfisca_paris/personnes_agees/paris_logement.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/personnes_agees/paris_pass_seniors.py` & `Openfisca-Paris-4.0.2/openfisca_paris/personnes_agees/paris_pass_seniors.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/personnes_agees/personnes_agees.py` & `Openfisca-Paris-4.0.2/openfisca_paris/personnes_agees/personnes_agees.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/personnes_agees/psol.py` & `Openfisca-Paris-4.0.2/openfisca_paris/personnes_agees/psol.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/personnes_handicapees/paris_complement_sante.py` & `Openfisca-Paris-4.0.2/openfisca_paris/personnes_handicapees/paris_complement_sante.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/personnes_handicapees/paris_pass_access.py` & `Openfisca-Paris-4.0.2/openfisca_paris/personnes_handicapees/paris_pass_access.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/personnes_handicapees/personne_handicapee.py` & `Openfisca-Paris-4.0.2/openfisca_paris/personnes_handicapees/personne_handicapee.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/openfisca_paris/personnes_handicapees/psol.py` & `Openfisca-Paris-4.0.2/openfisca_paris/personnes_handicapees/psol.py`

 * *Files identical despite different names*

### Comparing `Openfisca-Paris-4.0.1/setup.py` & `Openfisca-Paris-4.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="Openfisca-Paris",
-    version="4.0.1",
+    version="4.0.2",
     author="OpenFisca Team",
     author_email="contact@openfisca.fr",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python",
```

