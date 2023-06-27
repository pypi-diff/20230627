# Comparing `tmp/global_chem-1.8.tar.gz` & `tmp/global_chem-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "global_chem-1.8.tar", last modified: Sat Nov 19 16:00:10 2022, max compression
+gzip compressed data, was "global_chem-1.8.1.tar", last modified: Tue Jun 27 14:56:53 2023, max compression
```

## Comparing `global_chem-1.8.tar` & `global_chem-1.8.1.tar`

### file list

```diff
@@ -1,169 +1,198 @@
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:10.003641 global_chem-1.8/
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1093 2022-11-19 16:00:10.003228 global_chem-1.8/PKG-INFO
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.875200 global_chem-1.8/global_chem/
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4804 2022-11-19 15:15:15.000000 global_chem-1.8/global_chem/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      238 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/__main__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.882867 global_chem-1.8/global_chem/animals/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-27 20:07:10.000000 global_chem-1.8/global_chem/animals/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.883900 global_chem-1.8/global_chem/animals/snakes/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-27 20:07:01.000000 global_chem-1.8/global_chem/animals/snakes/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    38357 2022-11-19 14:51:22.000000 global_chem-1.8/global_chem/animals/snakes/drugs_from_snake_venom.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      321 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/cli.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.885399 global_chem-1.8/global_chem/education/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/education/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.888836 global_chem-1.8/global_chem/education/cengage/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/education/cengage/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4602 2022-11-19 14:51:22.000000 global_chem-1.8/global_chem/education/cengage/organic_and_inorganic_bronsted_acids.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.892090 global_chem-1.8/global_chem/environment/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/environment/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9553 2022-11-19 15:40:12.000000 global_chem-1.8/global_chem/environment/alternative_jet_fuels.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2106 2022-11-19 14:51:22.000000 global_chem-1.8/global_chem/environment/chemicals_from_biomass.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9696 2022-11-19 14:51:22.000000 global_chem-1.8/global_chem/environment/emerging_perfluoroalkyls.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.893176 global_chem-1.8/global_chem/food/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/food/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.898248 global_chem-1.8/global_chem/food/color_additives/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/food/color_additives/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5620 2022-11-19 14:51:22.000000 global_chem-1.8/global_chem/food/color_additives/fda_list_five.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    26611 2022-11-19 14:51:22.000000 global_chem-1.8/global_chem/food/color_additives/fda_list_four.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6232 2022-11-19 14:51:22.000000 global_chem-1.8/global_chem/food/color_additives/fda_list_one.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    12448 2022-11-19 14:51:22.000000 global_chem-1.8/global_chem/food/color_additives/fda_list_seven.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5657 2022-11-19 14:51:22.000000 global_chem-1.8/global_chem/food/color_additives/fda_list_six.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5343 2022-11-19 14:51:22.000000 global_chem-1.8/global_chem/food/color_additives/fda_list_three.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5111 2022-11-19 14:51:22.000000 global_chem-1.8/global_chem/food/color_additives/fda_list_two.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.899705 global_chem-1.8/global_chem/food/salt/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/food/salt/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2304 2022-11-19 14:51:22.000000 global_chem-1.8/global_chem/food/salt/salt.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.900628 global_chem-1.8/global_chem/formulation/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/formulation/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.901439 global_chem-1.8/global_chem/formulation/excipients/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/formulation/excipients/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1783 2022-09-02 17:44:42.000000 global_chem-1.8/global_chem/formulation/excipients/allergen_inactive_ingredients.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.902716 global_chem-1.8/global_chem/formulation/excipients/biopharmaceutics_class_three/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/formulation/excipients/biopharmaceutics_class_three/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4134 2022-11-19 15:41:31.000000 global_chem-1.8/global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.904128 global_chem-1.8/global_chem/formulation/excipients/monoclonal_antibodies/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/formulation/excipients/monoclonal_antibodies/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4080 2022-11-19 14:58:02.000000 global_chem-1.8/global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    42123 2022-11-19 15:14:46.000000 global_chem-1.8/global_chem/global_chem.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.905197 global_chem-1.8/global_chem/interstellar_space/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/interstellar_space/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    10891 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/interstellar_space/interstellar_space.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.905766 global_chem-1.8/global_chem/materials/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/materials/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.906492 global_chem-1.8/global_chem/materials/clay/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/materials/clay/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7263 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/materials/clay/montmorillonite_adsorption.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.907640 global_chem-1.8/global_chem/materials/polymers/
--rw-r--r--   0 sulimansharif   (501) staff       (20)      116 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/materials/polymers/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    18019 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/materials/polymers/common_monomer_repeating_units.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.908527 global_chem-1.8/global_chem/medicinal_chemistry/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/medicinal_chemistry/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.911946 global_chem-1.8/global_chem/medicinal_chemistry/cannabinoids/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/medicinal_chemistry/cannabinoids/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)   206471 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    32010 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.912978 global_chem-1.8/global_chem/medicinal_chemistry/chinese/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/medicinal_chemistry/chinese/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1103 2022-11-19 14:58:02.000000 global_chem-1.8/global_chem/medicinal_chemistry/chinese/how_to_live_longer.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.916107 global_chem-1.8/global_chem/medicinal_chemistry/rings/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/medicinal_chemistry/rings/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    13832 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2694 2022-11-19 14:58:02.000000 global_chem-1.8/global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    14543 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/medicinal_chemistry/rings/rings_in_drugs.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.920423 global_chem-1.8/global_chem/medicinal_chemistry/scaffolds/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/medicinal_chemistry/scaffolds/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    48105 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/medicinal_chemistry/scaffolds/common_r_group_replacements.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    22232 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/medicinal_chemistry/scaffolds/iupac_blue_book.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7459 2022-11-19 14:58:02.000000 global_chem-1.8/global_chem/medicinal_chemistry/scaffolds/privileged_scaffolds.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.923956 global_chem-1.8/global_chem/medicinal_chemistry/warheads/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/medicinal_chemistry/warheads/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3465 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/medicinal_chemistry/warheads/common_warheads_covalent_inhibitors.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3181 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/medicinal_chemistry/warheads/electrophilic_warheads_for_kinases.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.975783 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:47:37.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:55:15.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/access_group_antibiotics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:49:36.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/anaesthetics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:51:49.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/anaphylaxis_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:52:49.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/anticonvulsants.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:52:14.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/antidotes.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:54:19.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/antifilarials.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:54:31.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/antischistosomals_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:54:57.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/cysticidal_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:53:49.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/intestinal_anthelminthics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:50:04.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/medical_gases.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:50:54.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/non_steroidal_anti_inflammatory_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:51:10.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/opioid_analgesics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:51:29.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/palliative_care.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:49:47.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/preoperative_medicines.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:55:47.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/reserve_group_antibiotics.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-08-22 01:55:30.000000 global_chem-1.8/global_chem/medicinal_chemistry/world_health_organization/watch_group_antibiotics.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.979547 global_chem-1.8/global_chem/miscellaneous/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/miscellaneous/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2139 2022-11-19 14:58:02.000000 global_chem-1.8/global_chem/miscellaneous/amino_acids.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9650 2022-11-19 14:58:02.000000 global_chem-1.8/global_chem/miscellaneous/open_smiles.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)      396 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/miscellaneous/regex_patterns.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3724 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/miscellaneous/vitamins.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.988769 global_chem-1.8/global_chem/narcotics/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/narcotics/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    41346 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/narcotics/pihkal.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2155 2022-11-19 14:58:02.000000 global_chem-1.8/global_chem/narcotics/schedule_five.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    17624 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/narcotics/schedule_four.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    57945 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/narcotics/schedule_one.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4816 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/narcotics/schedule_three.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    14153 2022-11-19 14:58:02.000000 global_chem-1.8/global_chem/narcotics/schedule_two.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.989509 global_chem-1.8/global_chem/organic_synthesis/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/organic_synthesis/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.989890 global_chem-1.8/global_chem/organic_synthesis/bidendate_phosphine_ligands/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/organic_synthesis/bidendate_phosphine_ligands/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7973 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/organic_synthesis/bidendate_phosphine_ligands/nickel_ligands.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.991035 global_chem-1.8/global_chem/organic_synthesis/protecting_groups/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/organic_synthesis/protecting_groups/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    42927 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/organic_synthesis/protecting_groups/amino_acid_protecting_groups.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.992867 global_chem-1.8/global_chem/organic_synthesis/solvents/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/organic_synthesis/solvents/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5293 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/organic_synthesis/solvents/common_organic_solvents.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.993692 global_chem-1.8/global_chem/peptides/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/peptides/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     3489 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/peptides/lanthipeptides.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.994488 global_chem-1.8/global_chem/proteins/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/proteins/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.994680 global_chem-1.8/global_chem/proteins/kinases/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/proteins/kinases/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.995028 global_chem-1.8/global_chem/proteins/kinases/braf/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/proteins/kinases/braf/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     7617 2022-11-19 14:58:02.000000 global_chem-1.8/global_chem/proteins/kinases/braf/braf_inhibitors.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.995961 global_chem-1.8/global_chem/proteins/kinases/scaffolds/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/proteins/kinases/scaffolds/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     5167 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/proteins/kinases/scaffolds/privileged_kinase_inhibitors.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.996465 global_chem-1.8/global_chem/sex/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/sex/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.996836 global_chem-1.8/global_chem/sex/contraceptives/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-09-03 13:09:29.000000 global_chem-1.8/global_chem/sex/contraceptives/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     4434 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/sex/contraceptives/oral_contraceptives.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.998335 global_chem-1.8/global_chem/sex/exsens/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/sex/exsens/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)    16558 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/sex/exsens/exsens_products.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9160 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/sex/exsens/lube.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.999255 global_chem-1.8/global_chem/sex/tainted_sexual_enhancements/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/sex/tainted_sexual_enhancements/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1269 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/sex/tainted_sexual_enhancements/tainted_sexual_enhancements.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.999819 global_chem-1.8/global_chem/skin/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/skin/__init__.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:10.000362 global_chem-1.8/global_chem/skin/sunscreen/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/skin/sunscreen/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/skin/sunscreen/sunscreen.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:10.000992 global_chem-1.8/global_chem/skin/transdermal_and_dermal_delivery/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-09-21 11:47:11.000000 global_chem-1.8/global_chem/skin/transdermal_and_dermal_delivery/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     9628 2022-11-19 14:58:03.000000 global_chem-1.8/global_chem/skin/transdermal_and_dermal_delivery/surfactants.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:10.002343 global_chem-1.8/global_chem/warfare/
--rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2022-07-31 12:37:34.000000 global_chem-1.8/global_chem/warfare/__init__.py
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2511 2022-11-19 15:41:41.000000 global_chem-1.8/global_chem/warfare/organophosphorous_nerve_agents.py
-drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2022-11-19 16:00:09.881749 global_chem-1.8/global_chem.egg-info/
--rw-r--r--   0 sulimansharif   (501) staff       (20)     1093 2022-11-19 16:00:08.000000 global_chem-1.8/global_chem.egg-info/PKG-INFO
--rw-r--r--   0 sulimansharif   (501) staff       (20)     6464 2022-11-19 16:00:08.000000 global_chem-1.8/global_chem.egg-info/SOURCES.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2022-11-19 16:00:08.000000 global_chem-1.8/global_chem.egg-info/dependency_links.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2022-11-19 16:00:08.000000 global_chem-1.8/global_chem.egg-info/not-zip-safe
--rw-r--r--   0 sulimansharif   (501) staff       (20)      592 2022-11-19 16:00:08.000000 global_chem-1.8/global_chem.egg-info/requires.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       12 2022-11-19 16:00:08.000000 global_chem-1.8/global_chem.egg-info/top_level.txt
--rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2022-11-19 16:00:10.003764 global_chem-1.8/setup.cfg
--rw-r--r--   0 sulimansharif   (501) staff       (20)     2369 2022-11-19 14:58:03.000000 global_chem-1.8/setup.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.990833 global_chem-1.8.1/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1195 2023-06-27 14:56:53.990225 global_chem-1.8.1/PKG-INFO
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.848008 global_chem-1.8.1/global_chem/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6954 2023-06-27 14:51:37.000000 global_chem-1.8.1/global_chem/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      238 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/__main__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.864388 global_chem-1.8.1/global_chem/animals/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/animals/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.865126 global_chem-1.8.1/global_chem/animals/snakes/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/animals/snakes/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    38357 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/animals/snakes/drugs_from_snake_venom.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      321 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/cli.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.866040 global_chem-1.8.1/global_chem/education/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/education/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.866911 global_chem-1.8.1/global_chem/education/cengage/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/education/cengage/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4602 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/education/cengage/organic_and_inorganic_bronsted_acids.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.869408 global_chem-1.8.1/global_chem/environment/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/environment/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9553 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/environment/alternative_jet_fuels.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2106 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/environment/chemicals_from_biomass.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9696 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/environment/emerging_perfluoroalkyls.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.869908 global_chem-1.8.1/global_chem/food/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/food/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.875746 global_chem-1.8.1/global_chem/food/color_additives/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/food/color_additives/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5620 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/food/color_additives/fda_list_five.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    26611 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/food/color_additives/fda_list_four.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     6232 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/food/color_additives/fda_list_one.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    12448 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/food/color_additives/fda_list_seven.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5657 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/food/color_additives/fda_list_six.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5343 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/food/color_additives/fda_list_three.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5111 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/food/color_additives/fda_list_two.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.876339 global_chem-1.8.1/global_chem/food/fruits/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/food/fruits/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.882124 global_chem-1.8.1/global_chem/food/fruits/mango/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/food/fruits/mango/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1631 2023-06-27 14:51:36.000000 global_chem-1.8.1/global_chem/food/fruits/mango/fattyacids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1442 2023-06-27 14:51:37.000000 global_chem-1.8.1/global_chem/food/fruits/mango/flavonoids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1297 2023-06-27 14:51:37.000000 global_chem-1.8.1/global_chem/food/fruits/mango/mango_amino_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5816 2023-06-27 14:51:36.000000 global_chem-1.8.1/global_chem/food/fruits/mango/mango_phytocompounds.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1122 2023-06-27 14:51:36.000000 global_chem-1.8.1/global_chem/food/fruits/mango/phenolicacids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1161 2023-06-27 14:51:36.000000 global_chem-1.8.1/global_chem/food/fruits/mango/vitamins.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.883270 global_chem-1.8.1/global_chem/food/salt/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/food/salt/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2304 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/food/salt/salt.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.883853 global_chem-1.8.1/global_chem/formulation/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/formulation/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.884325 global_chem-1.8.1/global_chem/formulation/excipients/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/formulation/excipients/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1783 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/formulation/excipients/allergen_inactive_ingredients.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.885343 global_chem-1.8.1/global_chem/formulation/excipients/biopharmaceutics_class_three/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/formulation/excipients/biopharmaceutics_class_three/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4134 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.886927 global_chem-1.8.1/global_chem/formulation/excipients/monoclonal_antibodies/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/formulation/excipients/monoclonal_antibodies/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4080 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    47493 2023-06-27 14:51:36.000000 global_chem-1.8.1/global_chem/global_chem.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.889485 global_chem-1.8.1/global_chem/interstellar_space/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/interstellar_space/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      678 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/interstellar_space/asteroid_ryugu.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    10891 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/interstellar_space/interstellar_space.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.890453 global_chem-1.8.1/global_chem/materials/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/materials/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.891250 global_chem-1.8.1/global_chem/materials/clay/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/materials/clay/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7263 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/materials/clay/montmorillonite_adsorption.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.892964 global_chem-1.8.1/global_chem/materials/polymers/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      116 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/materials/polymers/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    18019 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/materials/polymers/common_monomer_repeating_units.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.893868 global_chem-1.8.1/global_chem/medicinal_chemistry/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.918807 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1263 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      535 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/alcohols.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      757 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/aldehydes.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1083 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/amino_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5131 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/cannabinoids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)   206471 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      914 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/esters_and_lactones.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      997 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/fatty_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1937 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/flavanoidglycosides.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2941 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/hydrocarbons.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      959 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/ketones.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1123 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/nitrogenous_compounds.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1321 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/non_cannabinoids_phenols.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    32010 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      540 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/pigments.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    33609 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/proteins_glycoproteins_enzymes.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1122 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/steroids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2032 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/sugars.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5409 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/terpenes.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      418 2023-06-27 14:15:06.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/vitamins.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.920332 global_chem-1.8.1/global_chem/medicinal_chemistry/chinese/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/chinese/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1103 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/chinese/how_to_live_longer.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.924932 global_chem-1.8.1/global_chem/medicinal_chemistry/rings/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/rings/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    13832 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2694 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    14543 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/rings/rings_in_drugs.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.928029 global_chem-1.8.1/global_chem/medicinal_chemistry/scaffolds/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/scaffolds/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    48105 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/scaffolds/common_r_group_replacements.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    22232 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/scaffolds/iupac_blue_book.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7459 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/scaffolds/privileged_scaffolds.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.930069 global_chem-1.8.1/global_chem/medicinal_chemistry/warheads/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/warheads/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3465 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/warheads/common_warheads_covalent_inhibitors.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3181 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/warheads/electrophilic_warheads_for_kinases.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.944917 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/access_group_antibiotics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/anaesthetics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/anaphylaxis_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/anticonvulsants.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/antidotes.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/antifilarials.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/antischistosomals_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/cysticidal_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/intestinal_anthelminthics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/medical_gases.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/non_steroidal_anti_inflammatory_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/opioid_analgesics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/palliative_care.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/preoperative_medicines.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/reserve_group_antibiotics.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/medicinal_chemistry/world_health_organization/watch_group_antibiotics.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.949711 global_chem-1.8.1/global_chem/miscellaneous/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/miscellaneous/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2139 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/miscellaneous/amino_acids.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9650 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/miscellaneous/open_smiles.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      396 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/miscellaneous/regex_patterns.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3724 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/miscellaneous/vitamins.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.965161 global_chem-1.8.1/global_chem/narcotics/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/narcotics/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    41346 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/narcotics/pihkal.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2155 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/narcotics/schedule_five.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    17624 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/narcotics/schedule_four.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    57945 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/narcotics/schedule_one.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4816 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/narcotics/schedule_three.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    14153 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/narcotics/schedule_two.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.966035 global_chem-1.8.1/global_chem/organic_synthesis/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/organic_synthesis/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.966759 global_chem-1.8.1/global_chem/organic_synthesis/bidendate_phosphine_ligands/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/organic_synthesis/bidendate_phosphine_ligands/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7973 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/organic_synthesis/bidendate_phosphine_ligands/nickel_ligands.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.967892 global_chem-1.8.1/global_chem/organic_synthesis/protecting_groups/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/organic_synthesis/protecting_groups/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    42927 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/organic_synthesis/protecting_groups/amino_acid_protecting_groups.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.971271 global_chem-1.8.1/global_chem/organic_synthesis/solvents/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/organic_synthesis/solvents/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5293 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/organic_synthesis/solvents/common_organic_solvents.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.973343 global_chem-1.8.1/global_chem/peptides/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/peptides/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     3489 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/peptides/lanthipeptides.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.974365 global_chem-1.8.1/global_chem/proteins/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/proteins/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.974776 global_chem-1.8.1/global_chem/proteins/kinases/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/proteins/kinases/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.975533 global_chem-1.8.1/global_chem/proteins/kinases/braf/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/proteins/kinases/braf/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7617 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/proteins/kinases/braf/braf_inhibitors.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.976752 global_chem-1.8.1/global_chem/proteins/kinases/scaffolds/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/proteins/kinases/scaffolds/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     5167 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/proteins/kinases/scaffolds/privileged_kinase_inhibitors.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.977474 global_chem-1.8.1/global_chem/sex/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/sex/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.979025 global_chem-1.8.1/global_chem/sex/contraceptives/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/sex/contraceptives/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     4434 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/sex/contraceptives/oral_contraceptives.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.983422 global_chem-1.8.1/global_chem/sex/exsens/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/sex/exsens/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)    16558 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/sex/exsens/exsens_products.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9160 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/sex/exsens/lube.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.984504 global_chem-1.8.1/global_chem/sex/tainted_sexual_enhancements/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/sex/tainted_sexual_enhancements/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1269 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/sex/tainted_sexual_enhancements/tainted_sexual_enhancements.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.985343 global_chem-1.8.1/global_chem/skin/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/skin/__init__.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.986180 global_chem-1.8.1/global_chem/skin/sunscreen/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/skin/sunscreen/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/skin/sunscreen/sunscreen.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.987403 global_chem-1.8.1/global_chem/skin/transdermal_and_dermal_delivery/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/skin/transdermal_and_dermal_delivery/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     9628 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/skin/transdermal_and_dermal_delivery/surfactants.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.989018 global_chem-1.8.1/global_chem/warfare/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        0 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/warfare/__init__.py
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2511 2023-04-11 15:37:28.000000 global_chem-1.8.1/global_chem/warfare/organophosphorous_nerve_agents.py
+drwxr-xr-x   0 sulimansharif   (501) staff       (20)        0 2023-06-27 14:56:53.863818 global_chem-1.8.1/global_chem.egg-info/
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     1195 2023-06-27 14:56:53.000000 global_chem-1.8.1/global_chem.egg-info/PKG-INFO
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     7981 2023-06-27 14:56:53.000000 global_chem-1.8.1/global_chem.egg-info/SOURCES.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2023-06-27 14:56:53.000000 global_chem-1.8.1/global_chem.egg-info/dependency_links.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)        1 2023-06-27 14:56:33.000000 global_chem-1.8.1/global_chem.egg-info/not-zip-safe
+-rw-r--r--   0 sulimansharif   (501) staff       (20)      592 2023-06-27 14:56:53.000000 global_chem-1.8.1/global_chem.egg-info/requires.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       12 2023-06-27 14:56:53.000000 global_chem-1.8.1/global_chem.egg-info/top_level.txt
+-rw-r--r--   0 sulimansharif   (501) staff       (20)       38 2023-06-27 14:56:53.991339 global_chem-1.8.1/setup.cfg
+-rw-r--r--   0 sulimansharif   (501) staff       (20)     2469 2023-06-27 14:52:23.000000 global_chem-1.8.1/setup.py
```

### Comparing `global_chem-1.8/PKG-INFO` & `global_chem-1.8.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global_chem
-Version: 1.8
+Version: 1.8.1
 Summary: UNKNOWN
 Home-page: https://www.github.com/Sulstice/global-chem
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: MPL 2.0
 Description: GlobalChem - Your Chemical Knowledge Graph for Chemistry
 Keywords: smiles molecules chemistry organic iupac
@@ -15,14 +15,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: graphing
 Provides-Extra: forcefields
 Provides-Extra: bioinformatics
 Provides-Extra: cheminformatics
 Provides-Extra: quantum_chemistry
 Provides-Extra: development_operations
```

### Comparing `global_chem-1.8/global_chem/animals/snakes/drugs_from_snake_venom.py` & `global_chem-1.8.1/global_chem/animals/snakes/drugs_from_snake_venom.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/education/cengage/organic_and_inorganic_bronsted_acids.py` & `global_chem-1.8.1/global_chem/education/cengage/organic_and_inorganic_bronsted_acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/environment/alternative_jet_fuels.py` & `global_chem-1.8.1/global_chem/environment/alternative_jet_fuels.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/environment/chemicals_from_biomass.py` & `global_chem-1.8.1/global_chem/environment/chemicals_from_biomass.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/environment/emerging_perfluoroalkyls.py` & `global_chem-1.8.1/global_chem/environment/emerging_perfluoroalkyls.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/food/color_additives/fda_list_five.py` & `global_chem-1.8.1/global_chem/food/color_additives/fda_list_five.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/food/color_additives/fda_list_four.py` & `global_chem-1.8.1/global_chem/food/color_additives/fda_list_four.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/food/color_additives/fda_list_one.py` & `global_chem-1.8.1/global_chem/food/color_additives/fda_list_one.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/food/color_additives/fda_list_seven.py` & `global_chem-1.8.1/global_chem/food/color_additives/fda_list_seven.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/food/color_additives/fda_list_six.py` & `global_chem-1.8.1/global_chem/food/color_additives/fda_list_six.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/food/color_additives/fda_list_three.py` & `global_chem-1.8.1/global_chem/food/color_additives/fda_list_three.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/food/color_additives/fda_list_two.py` & `global_chem-1.8.1/global_chem/food/color_additives/fda_list_two.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/food/salt/salt.py` & `global_chem-1.8.1/global_chem/food/salt/salt.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/formulation/excipients/allergen_inactive_ingredients.py` & `global_chem-1.8.1/global_chem/formulation/excipients/allergen_inactive_ingredients.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py` & `global_chem-1.8.1/global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py` & `global_chem-1.8.1/global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/global_chem.py` & `global_chem-1.8.1/global_chem/global_chem.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,18 +40,36 @@
 
 from global_chem.warfare.organophosphorous_nerve_agents import OrganoPhosphorousNerveAgents
 
 # Education
 
 from global_chem.education.cengage.organic_and_inorganic_bronsted_acids import OrganicAndInorganicBronstedAcids
 
-# Medicinal Chemistry - Cannabis
+# Medicinal Chemistry - Cannabinoids
 
 from global_chem.medicinal_chemistry.cannabinoids.phytocannabinoids import PhytoCannabinoids
 from global_chem.medicinal_chemistry.cannabinoids.constituents_of_cannabis_sativa import ConstituentsOfCannabisSativa
+from global_chem.medicinal_chemistry.cannabinoids.acids import CannabisAcids
+from global_chem.medicinal_chemistry.cannabinoids.alcohols import CannabisAlcohols
+from global_chem.medicinal_chemistry.cannabinoids.aldehydes import CannabisAldehydes
+from global_chem.medicinal_chemistry.cannabinoids.amino_acids import CannabisAminoAcids
+from global_chem.medicinal_chemistry.cannabinoids.cannabinoids import Cannabinoids
+from global_chem.medicinal_chemistry.cannabinoids.esters_and_lactones import CannabisEstersAndLactones
+from global_chem.medicinal_chemistry.cannabinoids.fatty_acids import CannabisFattyAcids
+from global_chem.medicinal_chemistry.cannabinoids.flavanoidglycosides import CannabisFlavanoidGlycosides
+from global_chem.medicinal_chemistry.cannabinoids.hydrocarbons import CannabisHydrocarbons
+from global_chem.medicinal_chemistry.cannabinoids.ketones import CannabisKetones
+from global_chem.medicinal_chemistry.cannabinoids.nitrogenous_compounds import CannabisNitrogenousCompounds
+from global_chem.medicinal_chemistry.cannabinoids.non_cannabinoids_phenols import NonCannabinoidPhenols
+from global_chem.medicinal_chemistry.cannabinoids.pigments import CannabisPigments
+from global_chem.medicinal_chemistry.cannabinoids.proteins_glycoproteins_enzymes import CannabisProteinsGlycoproteinsEnzymes
+from global_chem.medicinal_chemistry.cannabinoids.steroids import CannabisSteroids
+from global_chem.medicinal_chemistry.cannabinoids.sugars import CannabisSugars
+from global_chem.medicinal_chemistry.cannabinoids.terpenes import CannabisTerpenes
+from global_chem.medicinal_chemistry.cannabinoids.vitamins import CannabisVitamins
 
 # Medicinal Chemistry - International
 
 from global_chem.medicinal_chemistry.chinese.how_to_live_longer import HowToLiveLonger
 
 # Medicinal Chemistry - Warheads
 
@@ -89,26 +107,38 @@
 from global_chem.food.color_additives.fda_list_two import FDAListTwo
 from global_chem.food.color_additives.fda_list_three import FDAListThree
 from global_chem.food.color_additives.fda_list_four import FDAListFour
 from global_chem.food.color_additives.fda_list_five import FDAListFive
 from global_chem.food.color_additives.fda_list_six import FDAListSix
 from global_chem.food.color_additives.fda_list_seven import FDAListSeven
 
+
+
+# Food/Fruits/Mango
+
+from global_chem.food.fruits.mango.mango_phytocompounds import MangoPhytoCompounds
+from global_chem.food.fruits.mango.fattyacids import MangoFattyAcids
+from global_chem.food.fruits.mango.flavonoids import MangoFlavonoids
+from global_chem.food.fruits.mango.phenolicacids import MangoPhenolicAcids
+from global_chem.food.fruits.mango.vitamins import MangoVitamins
+from global_chem.food.fruits.mango.mango_amino_acids import MangoAminoAcids
+
 # Narcotics
 
 from global_chem.narcotics.pihkal import Pihkal
 from global_chem.narcotics.schedule_one import ScheduleOne
 from global_chem.narcotics.schedule_two import ScheduleTwo
 from global_chem.narcotics.schedule_three import ScheduleThree
 from global_chem.narcotics.schedule_four import ScheduleFour
 from global_chem.narcotics.schedule_five import ScheduleFive
 
 # Interstellar Space
 
 from global_chem.interstellar_space.interstellar_space import InterstellarSpace
+from global_chem.interstellar_space.asteroid_ryugu import AsteroidRyugu
 
 # Biopharmaceutics - Excipients
 
 from global_chem.formulation.excipients.monoclonal_antibodies.monoclonal_antibodies import MonoclonalAntibodies
 from global_chem.formulation.excipients.biopharmaceutics_class_three.cimetidine_and_acyclovir import CimetidineAndAcyclovir
 
 # Miscellaneous
@@ -243,19 +273,19 @@
         smarts = {}
 
 class PrintNode:
 
     __version__ = '0.0.1'
 
     '''
-    
-    Hack for now, 
-    
-    Print Node function to get the network printed out. Feature first, refactor later. 
-    
+
+    Hack for now,
+
+    Print Node function to get the network printed out. Feature first, refactor later.
+
     '''
 
     def __init__(self, val, parent=None):
 
         self.val = val
         self.parent = parent
         self.children = []
@@ -353,91 +383,116 @@
 
 class GraphNetworkError(Exception):
 
     __version_error_parser__ = "1.0.4"
     __allow_update__ = False
 
     '''
-    
+
     Raise the Network Error if the Node cannot be found.
-    
+
     '''
     def __init__(self, message, errors):
         super().__init__(message)
         self.errors = errors
 
 class GlobalChem(object):
 
     __version__ = "1.0.4"
     __allow_update__ = False
 
     """
-    
+
     GlobalChem will be the master class of all variables, as the content store grows we can use this as the parent class.
-    
+
     """
 
     # NODE CONTRIBUTORS
     # -----------------
 
     # Thank you to the contributors to the node network that made this project alive.
 
     __NODES__ = {
         'global_chem': Node,
-        'emerging_perfluoroalkyls': EmergingPerFluoroAlkyls,                      # Asuka Orr & Suliman Sharif
-        'montmorillonite_adsorption': MontmorilloniteAdsorption,                  # Asuka Orr & Suliman Sharif
-        'common_monomer_repeating_units': CommonMonomerRepeatingUnits,            # Suliman Sharif
-        'electrophilic_warheads_for_kinases': ElectrophilicWarheadsForKinases,    # Ruibin Liu & Suliman Sharif
-        'common_warheads_covalent_inhibitors': CommonWarheadsCovalentInhibitors,  # Shaoqi Zhan & Suliman Sharif
-        'rings_in_drugs': RingsInDrugs,                                           # Alexander Mackerell Jr. & Suliman Sharif
-        'iupac_blue_book_rings': IUPACBlueBookRings,                              # Suliman Sharif
-        'phase_2_hetereocyclic_rings': Phase2HetereoCyclicRings,                  # Suliman Sharif
-        'privileged_scaffolds': PrivilegedScaffolds,                              # Suliman Sharif
-        'iupac_blue_book': IUPACBlueBook,                                         # Suliman Sharif
-        'common_r_group_replacements': CommonRGroupReplacements,                  # Sunhwan Jo & Suliman Sharif
-        'braf_inhibitors': BRAFInhibitors,                                        # Aarion Romany & Suliman Sharif
-        'privileged_kinase_inhibitors': PrivilegedKinaseInhibitors,               # Suliman Sharif
-        'common_organic_solvents': CommonOrganicSolvents,                         # Suliman Sharif
-        'amino_acid_protecting_groups': AminoAcidProtectingGroups,                # Aziza Frank & Suliman Sharif
-        'schedule_one': ScheduleOne,                                              # Suliman Sharif
-        'schedule_two': ScheduleTwo,                                              # Suliman Sharif
-        'schedule_three': ScheduleThree,                                          # Suliman Sharif
-        'schedule_four': ScheduleFour,                                            # Suliman Sharif
-        'schedule_five': ScheduleFive,                                            # Suliman Sharif
-        'interstellar_space': InterstellarSpace,                                  # Suliman Sharif
-        'vitamins': Vitamins,                                                     # Suliman Sharif
-        'open_smiles': OpenSmiles,                                                # Suliman Sharif
-        'amino_acids': AminoAcids,                                                # Suliman Sharif
-        'pihkal': Pihkal,                                                         # Suliman Sharif
-        'nickel_ligands': NickelBidendatePhosphineLigands,                        # Suliman Sharif
-        'cimetidine_and_acyclovir': CimetidineAndAcyclovir,                       # Suliman Sharif
-        'how_to_live_longer': HowToLiveLonger,                                    # Suliman Sharif
-        'monoclonal_antibodies': MonoclonalAntibodies,                            # Asuka Orr & Suliman Sharif
-        'lube': Lube,                                                             # Daniel Khavrutskii & Suliman Sharif
-        'tainted_sexual_enhancements': TaintedSexualEnhancements,                 # Suliman Sharif
-        'salt': Salt,                                                             # Suliman Sharif
-        'exsens_products': ExsensProducts,                                        # Rebecca Pinette-Dorin & Suliman Sharif
-        'fda_list_one': FDAListOne,                                               # Mike Wostner & Suliman Sharif
-        'fda_list_two': FDAListTwo,                                               # Mike Wostner & Suliman Sharif
-        'fda_list_three': FDAListThree,                                           # Mike Wostner & Suliman Sharif
-        'fda_list_four': FDAListFour,                                             # Mike Wostner & Suliman Sharif
-        'fda_list_five': FDAListFive,                                             # Mike Wostner & Suliman Sharif
-        'fda_list_six': FDAListSix,                                               # Mike Wostner & Suliman Sharif
-        'fda_list_seven': FDAListSeven,                                           # Mike Wostner & Suliman Sharif
-        'constituents_of_cannabis_sativa': ConstituentsOfCannabisSativa,          # Ian Jones & Bettina Lier & Suliman Sharif
-        'phytocannabinoids': PhytoCannabinoids,                                   # Ian Jones & Bettina Lier & Suliman Sharif
-        'organophosphorous_nerve_agents': OrganoPhosphorousNerveAgents,           # Suliman Sharif
-        'organic_and_inorganic_bronsted_acids': OrganicAndInorganicBronstedAcids, # Nathaniel McClean & Suliman Sharif
-        'chemicals_from_biomass': ChemicalsFromBioMass,                           # Anthony Maiorana & Suliman Sharif
-        'drugs_from_snake_venom': DrugsFromSnakeVenom,                            # Suliman Sharif
-        'oral_contraceptives': OralContraceptives,                                # Suliman Sharif
-        'surfactants': Surfactants,                                               # Yiling Nan & Suliman Sharif
-        'lanthipeptides': LanthiPeptides,                                         # Prabin Baral & Suliman Sharif
-        'alternative_jet_fuels': AlternativeJetFuels,                             # Suliman Sharif
-        'common_regex_patterns': CommonRegexPatterns,                             # Chris Burke & Suliman Sharif
+        'emerging_perfluoroalkyls': EmergingPerFluoroAlkyls,                             # Asuka Orr & Suliman Sharif
+        'montmorillonite_adsorption': MontmorilloniteAdsorption,                         # Asuka Orr & Suliman Sharif
+        'common_monomer_repeating_units': CommonMonomerRepeatingUnits,                   # Suliman Sharif
+        'electrophilic_warheads_for_kinases': ElectrophilicWarheadsForKinases,           # Ruibin Liu & Suliman Sharif
+        'common_warheads_covalent_inhibitors': CommonWarheadsCovalentInhibitors,         # Shaoqi Zhan & Suliman Sharif
+        'rings_in_drugs': RingsInDrugs,                                                  # Alexander Mackerell Jr. & Suliman Sharif
+        'iupac_blue_book_rings': IUPACBlueBookRings,                                     # Suliman Sharif
+        'phase_2_hetereocyclic_rings': Phase2HetereoCyclicRings,                         # Suliman Sharif
+        'privileged_scaffolds': PrivilegedScaffolds,                                     # Suliman Sharif
+        'iupac_blue_book': IUPACBlueBook,                                                # Suliman Sharif
+        'common_r_group_replacements': CommonRGroupReplacements,                         # Sunhwan Jo & Suliman Sharif
+        'braf_inhibitors': BRAFInhibitors,                                               # Aarion Romany & Suliman Sharif
+        'privileged_kinase_inhibitors': PrivilegedKinaseInhibitors,                      # Suliman Sharif
+        'common_organic_solvents': CommonOrganicSolvents,                                # Suliman Sharif
+        'amino_acid_protecting_groups': AminoAcidProtectingGroups,                       # Aziza Frank & Suliman Sharif
+        'schedule_one': ScheduleOne,                                                     # Suliman Sharif
+        'schedule_two': ScheduleTwo,                                                     # Suliman Sharif
+        'schedule_three': ScheduleThree,                                                 # Suliman Sharif
+        'schedule_four': ScheduleFour,                                                   # Suliman Sharif
+        'schedule_five': ScheduleFive,                                                   # Suliman Sharif
+        'interstellar_space': InterstellarSpace,                                         # Suliman Sharif
+        'asteroid_ryugu': AsteroidRyugu,                                                 # Josh Farrell & Suliman Sharif
+        'vitamins': Vitamins,                                                            # Suliman Sharif
+        'open_smiles': OpenSmiles,                                                       # Suliman Sharif
+        'amino_acids': AminoAcids,                                                       # Suliman Sharif
+        'pihkal': Pihkal,                                                                # Suliman Sharif
+        'nickel_ligands': NickelBidendatePhosphineLigands,                               # Suliman Sharif
+        'cimetidine_and_acyclovir': CimetidineAndAcyclovir,                              # Suliman Sharif
+        'how_to_live_longer': HowToLiveLonger,                                           # Suliman Sharif
+        'monoclonal_antibodies': MonoclonalAntibodies,                                   # Asuka Orr & Suliman Sharif
+        'lube': Lube,                                                                    # Daniel Khavrutskii & Suliman Sharif
+        'tainted_sexual_enhancements': TaintedSexualEnhancements,                        # Suliman Sharif
+        'salt': Salt,                                                                    # Suliman Sharif
+        'exsens_products': ExsensProducts,                                               # Rebecca Pinette-Dorin & Suliman Sharif
+        'fda_list_one': FDAListOne,                                                      # Mike Wostner & Suliman Sharif
+        'fda_list_two': FDAListTwo,                                                      # Mike Wostner & Suliman Sharif
+        'fda_list_three': FDAListThree,                                                  # Mike Wostner & Suliman Sharif
+        'fda_list_four': FDAListFour,                                                    # Mike Wostner & Suliman Sharif
+        'fda_list_five': FDAListFive,                                                    # Mike Wostner & Suliman Sharif
+        'fda_list_six': FDAListSix,                                                      # Mike Wostner & Suliman Sharif
+        'fda_list_seven': FDAListSeven,                                                  # Mike Wostner & Suliman Sharif
+        'constituents_of_cannabis_sativa': ConstituentsOfCannabisSativa,                 # Ian Jones & Bettina Lier & Suliman Sharif
+        'phytocannabinoids': PhytoCannabinoids,                                          # Ian Jones & Bettina Lier & Suliman Sharif
+        'cannabis_acids': CannabisAcids,                                                 # Suliman Sharif
+        'cannabis_alcohols': CannabisAlcohols,                                           # Suliman Sharif
+        'cannabis_aldehydes': CannabisAldehydes,                                         # Suliman Sharif
+        'cannabis_amino_acids': CannabisAminoAcids,                                      # Suliman Sharif
+        'cannabinoids': Cannabinoids,                                                    # Suliman Sharif
+        'cannabis_esters_and_lactones': CannabisEstersAndLactones,                       # Suliman Sharif
+        'cannabis_fatty_acids': CannabisFattyAcids,                                      # Suliman Sharif
+        'cannabis_flavanoid_glycosides': CannabisFlavanoidGlycosides,                    # Suliman Sharif
+        'cannabis_hydrocarbons': CannabisHydrocarbons,                                   # Suliman Sharif
+        'cannabis_ketones': CannabisKetones,                                             # Suliman Sharif
+        'cannabis_nitrogenous_compounds': CannabisNitrogenousCompounds,                  # Suliman Sharif
+        'non_cannabinoid_phenols': NonCannabinoidPhenols,                                # Suliman Sharif
+        'cannabis_pigments': CannabisPigments,                                           # Suliman Sharif
+        'cannabis_proteins_glycoproteins_enzymes': CannabisProteinsGlycoproteinsEnzymes, # Suliman Sharif
+        'cannabis_steroids': CannabisSteroids,                                           # Suliman Sharif
+        'cannabis_sugars': CannabisSugars,                                               # Suliman Sharif
+        'cannabis_terpenes': CannabisTerpenes,                                           # Suliman Sharif
+        'cannabis_vitamins': CannabisVitamins,                                           # Suliman Sharif
+        'organophosphorous_nerve_agents': OrganoPhosphorousNerveAgents,                  # Suliman Sharif
+        'organic_and_inorganic_bronsted_acids': OrganicAndInorganicBronstedAcids,        # Nathaniel McClean & Suliman Sharif
+        'chemicals_from_biomass': ChemicalsFromBioMass,                                  # Anthony Maiorana & Suliman Sharif
+        'drugs_from_snake_venom': DrugsFromSnakeVenom,                                   # Suliman Sharif
+        'oral_contraceptives': OralContraceptives,                                       # Suliman Sharif
+        'surfactants': Surfactants,                                                      # Yiling Nan & Suliman Sharif
+        'lanthipeptides': LanthiPeptides,                                                # Prabin Baral & Suliman Sharif
+        'alternative_jet_fuels': AlternativeJetFuels,                                    # Suliman Sharif
+        'common_regex_patterns': CommonRegexPatterns,                                    # Chris Burke & Suliman Sharif
+        'mango_phytocompounds': MangoPhytoCompounds,                                     # Damilola Bodun & Sevien Schulhoff & Suliman Sharif
+        'mango_amino_acids': MangoAminoAcids,                                            # Damilola Bodun & Sevien Schulhoff & Suliman Sharif
+        'mango_phenolic_acids': MangoPhenolicAcids,                                      # Damilola Bodun & Sevien Schulhoff & Suliman Sharif
+        'mango_fatty_acids': MangoFattyAcids,                                            # Damilola Bodun & Sevien Schulhoff & Suliman Sharif
+        'mango_vitamins': MangoVitamins,                                                 # Damilola Bodun & Sevien Schulhoff & Suliman Sharif
+        'mango_flavonoids': MangoFlavonoids                                              # Damilola Bodun & Sevien Schulhoff & Suliman Sharif
     }
 
     __INCOMPLETE_NODES = {
         # 'named_reactions_in_organic_synthesis': NamedReactionsInOrganicSynthesis # Aziza Frank & Bettina Lier & Suliman Sharif
     }
 
     def __init__(self, verbose=False):
@@ -941,15 +996,15 @@
 
                     object_path = os.path.join(''.join(dirpath.rsplit(absolute_file_path)), file).split(self.splitter)
 
                     if debugger:
                         print ("Node Object Paths: %s: " % object_path)
 
                     path_objects.append(object_path)
-        
+
         # Add the objects recursively
 
         for chemical_object in path_objects:
 
             chemical_object.reverse()
             chemical_object = chemical_object + ['global_chem']
 
@@ -1394,8 +1449,8 @@
 
             return 1 + min(
                 min_dist(string_1, string_2 + 1),
                 min_dist(string_1 + 1, string_2),
                 min_dist(string_1 + 1, string_2 + 1),
             )
 
-        return min_dist(0, 0)
+        return min_dist(0, 0)
```

### Comparing `global_chem-1.8/global_chem/interstellar_space/interstellar_space.py` & `global_chem-1.8.1/global_chem/interstellar_space/interstellar_space.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/materials/clay/montmorillonite_adsorption.py` & `global_chem-1.8.1/global_chem/materials/clay/montmorillonite_adsorption.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/materials/polymers/common_monomer_repeating_units.py` & `global_chem-1.8.1/global_chem/materials/polymers/common_monomer_repeating_units.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py` & `global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py` & `global_chem-1.8.1/global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/medicinal_chemistry/chinese/how_to_live_longer.py` & `global_chem-1.8.1/global_chem/medicinal_chemistry/chinese/how_to_live_longer.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py` & `global_chem-1.8.1/global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py` & `global_chem-1.8.1/global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/medicinal_chemistry/rings/rings_in_drugs.py` & `global_chem-1.8.1/global_chem/medicinal_chemistry/rings/rings_in_drugs.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/medicinal_chemistry/scaffolds/common_r_group_replacements.py` & `global_chem-1.8.1/global_chem/medicinal_chemistry/scaffolds/common_r_group_replacements.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/medicinal_chemistry/scaffolds/iupac_blue_book.py` & `global_chem-1.8.1/global_chem/medicinal_chemistry/scaffolds/iupac_blue_book.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/medicinal_chemistry/scaffolds/privileged_scaffolds.py` & `global_chem-1.8.1/global_chem/medicinal_chemistry/scaffolds/privileged_scaffolds.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/medicinal_chemistry/warheads/common_warheads_covalent_inhibitors.py` & `global_chem-1.8.1/global_chem/medicinal_chemistry/warheads/common_warheads_covalent_inhibitors.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/medicinal_chemistry/warheads/electrophilic_warheads_for_kinases.py` & `global_chem-1.8.1/global_chem/medicinal_chemistry/warheads/electrophilic_warheads_for_kinases.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/miscellaneous/amino_acids.py` & `global_chem-1.8.1/global_chem/miscellaneous/amino_acids.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/miscellaneous/open_smiles.py` & `global_chem-1.8.1/global_chem/miscellaneous/open_smiles.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/miscellaneous/vitamins.py` & `global_chem-1.8.1/global_chem/miscellaneous/vitamins.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/narcotics/pihkal.py` & `global_chem-1.8.1/global_chem/narcotics/pihkal.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/narcotics/schedule_five.py` & `global_chem-1.8.1/global_chem/narcotics/schedule_five.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/narcotics/schedule_four.py` & `global_chem-1.8.1/global_chem/narcotics/schedule_four.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/narcotics/schedule_one.py` & `global_chem-1.8.1/global_chem/narcotics/schedule_one.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/narcotics/schedule_three.py` & `global_chem-1.8.1/global_chem/narcotics/schedule_three.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/narcotics/schedule_two.py` & `global_chem-1.8.1/global_chem/narcotics/schedule_two.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/organic_synthesis/bidendate_phosphine_ligands/nickel_ligands.py` & `global_chem-1.8.1/global_chem/organic_synthesis/bidendate_phosphine_ligands/nickel_ligands.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/organic_synthesis/protecting_groups/amino_acid_protecting_groups.py` & `global_chem-1.8.1/global_chem/organic_synthesis/protecting_groups/amino_acid_protecting_groups.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/organic_synthesis/solvents/common_organic_solvents.py` & `global_chem-1.8.1/global_chem/organic_synthesis/solvents/common_organic_solvents.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/peptides/lanthipeptides.py` & `global_chem-1.8.1/global_chem/peptides/lanthipeptides.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/proteins/kinases/braf/braf_inhibitors.py` & `global_chem-1.8.1/global_chem/proteins/kinases/braf/braf_inhibitors.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/proteins/kinases/scaffolds/privileged_kinase_inhibitors.py` & `global_chem-1.8.1/global_chem/proteins/kinases/scaffolds/privileged_kinase_inhibitors.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/sex/contraceptives/oral_contraceptives.py` & `global_chem-1.8.1/global_chem/sex/contraceptives/oral_contraceptives.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/sex/exsens/exsens_products.py` & `global_chem-1.8.1/global_chem/sex/exsens/exsens_products.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/sex/exsens/lube.py` & `global_chem-1.8.1/global_chem/sex/exsens/lube.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/sex/tainted_sexual_enhancements/tainted_sexual_enhancements.py` & `global_chem-1.8.1/global_chem/sex/tainted_sexual_enhancements/tainted_sexual_enhancements.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/skin/transdermal_and_dermal_delivery/surfactants.py` & `global_chem-1.8.1/global_chem/skin/transdermal_and_dermal_delivery/surfactants.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem/warfare/organophosphorous_nerve_agents.py` & `global_chem-1.8.1/global_chem/warfare/organophosphorous_nerve_agents.py`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/global_chem.egg-info/PKG-INFO` & `global_chem-1.8.1/global_chem.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global-chem
-Version: 1.8
+Version: 1.8.1
 Summary: UNKNOWN
 Home-page: https://www.github.com/Sulstice/global-chem
 Author: Suliman Sharif
 Author-email: sharifsuliman1@gmail.com
 License: MPL 2.0
 Description: GlobalChem - Your Chemical Knowledge Graph for Chemistry
 Keywords: smiles molecules chemistry organic iupac
@@ -15,14 +15,16 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: graphing
 Provides-Extra: forcefields
 Provides-Extra: bioinformatics
 Provides-Extra: cheminformatics
 Provides-Extra: quantum_chemistry
 Provides-Extra: development_operations
```

### Comparing `global_chem-1.8/global_chem.egg-info/SOURCES.txt` & `global_chem-1.8.1/global_chem.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -24,34 +24,61 @@
 global_chem/food/color_additives/fda_list_five.py
 global_chem/food/color_additives/fda_list_four.py
 global_chem/food/color_additives/fda_list_one.py
 global_chem/food/color_additives/fda_list_seven.py
 global_chem/food/color_additives/fda_list_six.py
 global_chem/food/color_additives/fda_list_three.py
 global_chem/food/color_additives/fda_list_two.py
+global_chem/food/fruits/__init__.py
+global_chem/food/fruits/mango/__init__.py
+global_chem/food/fruits/mango/fattyacids.py
+global_chem/food/fruits/mango/flavonoids.py
+global_chem/food/fruits/mango/mango_amino_acids.py
+global_chem/food/fruits/mango/mango_phytocompounds.py
+global_chem/food/fruits/mango/phenolicacids.py
+global_chem/food/fruits/mango/vitamins.py
 global_chem/food/salt/__init__.py
 global_chem/food/salt/salt.py
 global_chem/formulation/__init__.py
 global_chem/formulation/excipients/__init__.py
 global_chem/formulation/excipients/allergen_inactive_ingredients.py
 global_chem/formulation/excipients/biopharmaceutics_class_three/__init__.py
 global_chem/formulation/excipients/biopharmaceutics_class_three/cimetidine_and_acyclovir.py
 global_chem/formulation/excipients/monoclonal_antibodies/__init__.py
 global_chem/formulation/excipients/monoclonal_antibodies/monoclonal_antibodies.py
 global_chem/interstellar_space/__init__.py
+global_chem/interstellar_space/asteroid_ryugu.py
 global_chem/interstellar_space/interstellar_space.py
 global_chem/materials/__init__.py
 global_chem/materials/clay/__init__.py
 global_chem/materials/clay/montmorillonite_adsorption.py
 global_chem/materials/polymers/__init__.py
 global_chem/materials/polymers/common_monomer_repeating_units.py
 global_chem/medicinal_chemistry/__init__.py
 global_chem/medicinal_chemistry/cannabinoids/__init__.py
+global_chem/medicinal_chemistry/cannabinoids/acids.py
+global_chem/medicinal_chemistry/cannabinoids/alcohols.py
+global_chem/medicinal_chemistry/cannabinoids/aldehydes.py
+global_chem/medicinal_chemistry/cannabinoids/amino_acids.py
+global_chem/medicinal_chemistry/cannabinoids/cannabinoids.py
 global_chem/medicinal_chemistry/cannabinoids/constituents_of_cannabis_sativa.py
+global_chem/medicinal_chemistry/cannabinoids/esters_and_lactones.py
+global_chem/medicinal_chemistry/cannabinoids/fatty_acids.py
+global_chem/medicinal_chemistry/cannabinoids/flavanoidglycosides.py
+global_chem/medicinal_chemistry/cannabinoids/hydrocarbons.py
+global_chem/medicinal_chemistry/cannabinoids/ketones.py
+global_chem/medicinal_chemistry/cannabinoids/nitrogenous_compounds.py
+global_chem/medicinal_chemistry/cannabinoids/non_cannabinoids_phenols.py
 global_chem/medicinal_chemistry/cannabinoids/phytocannabinoids.py
+global_chem/medicinal_chemistry/cannabinoids/pigments.py
+global_chem/medicinal_chemistry/cannabinoids/proteins_glycoproteins_enzymes.py
+global_chem/medicinal_chemistry/cannabinoids/steroids.py
+global_chem/medicinal_chemistry/cannabinoids/sugars.py
+global_chem/medicinal_chemistry/cannabinoids/terpenes.py
+global_chem/medicinal_chemistry/cannabinoids/vitamins.py
 global_chem/medicinal_chemistry/chinese/__init__.py
 global_chem/medicinal_chemistry/chinese/how_to_live_longer.py
 global_chem/medicinal_chemistry/rings/__init__.py
 global_chem/medicinal_chemistry/rings/iupac_blue_book_rings.py
 global_chem/medicinal_chemistry/rings/phase_2_hetereocyclic_rings.py
 global_chem/medicinal_chemistry/rings/rings_in_drugs.py
 global_chem/medicinal_chemistry/scaffolds/__init__.py
```

### Comparing `global_chem-1.8/global_chem.egg-info/requires.txt` & `global_chem-1.8.1/global_chem.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `global_chem-1.8/setup.py` & `global_chem-1.8.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 else:
     long_description = 'GlobalChem - Your Chemical Knowledge Graph for Chemistry'
 
 # exec
 # ----
 setup(
     name="global_chem",
-    version="1.8",
+    version="1.8.1",
     packages=find_packages(),
     license='MPL 2.0',
     author="Suliman Sharif",
     author_email="sharifsuliman1@gmail.com",
     url="https://www.github.com/Sulstice/global-chem",
     install_requires=[],
     long_description=long_description,
@@ -64,11 +64,13 @@
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
     test_suite='tests',
     tests_require=TEST_REQUIREMENTS,
 )
```

