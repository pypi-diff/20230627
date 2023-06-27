# Comparing `tmp/wwpdb.utils.emdb-1.3.tar.gz` & `tmp/wwpdb.utils.emdb-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.utils.emdb-1.3.tar", last modified: Sun May 14 15:05:25 2023, max compression
+gzip compressed data, was "wwpdb.utils.emdb-1.4.tar", last modified: Tue Jun 27 11:53:16 2023, max compression
```

## Comparing `wwpdb.utils.emdb-1.3.tar` & `wwpdb.utils.emdb-1.4.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.360524 wwpdb.utils.emdb-1.3/
--rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-05-14 15:05:25.360524 wwpdb.utils.emdb-1.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-05-14 15:05:25.360524 wwpdb.utils.emdb-1.3/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2223 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.352523 wwpdb.utils.emdb-1.3/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.352523 wwpdb.utils.emdb-1.3/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.352523 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/
--rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/EmdbSchema.py
--rw-r--r--   0 vsts      (1001) docker     (123)      143 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.356523 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/
--rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)   664004 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (123)  2282514 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)      368 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/generatedsnamespaces.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.360524 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/data/
--rw-r--r--   0 vsts      (1001) docker     (123)   217704 2023-05-14 15:04:22.000000 wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/data/emdb-v3.xsd
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-14 15:05:25.352523 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-05-14 15:05:25.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      896 2023-05-14 15:05:25.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 15:05:25.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-05-14 15:05:25.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-14 15:05:10.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       77 2023-05-14 15:05:25.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-05-14 15:05:25.000000 wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.640441 wwpdb.utils.emdb-1.4/
+-rw-r--r--   0 vsts      (1001) docker     (123)      106 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-06-27 11:53:16.640441 wwpdb.utils.emdb-1.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       46 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-27 11:53:16.640441 wwpdb.utils.emdb-1.4/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2278 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.636441 wwpdb.utils.emdb-1.4/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.636441 wwpdb.utils.emdb-1.4/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.636441 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)      322 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/EmdbSchema.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      143 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.636441 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/atomcheck/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/atomcheck/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11264 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/atomcheck/atomcheck.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.640441 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      139 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)   668369 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1866 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (123)  2286661 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/emdb.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)      389 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/generatedsnamespaces.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     1196 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2490 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.640441 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)   219336 2023-06-27 11:52:28.000000 wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/data/emdb-v3.xsd
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-27 11:53:16.636441 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      719 2023-06-27 11:53:16.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      975 2023-06-27 11:53:16.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 11:53:16.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       87 2023-06-27 11:53:16.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-27 11:53:00.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      101 2023-06-27 11:53:16.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-27 11:53:16.000000 wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/top_level.txt
```

### Comparing `wwpdb.utils.emdb-1.3/PKG-INFO` & `wwpdb.utils.emdb-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.3
+Version: 1.4
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.3/setup.py` & `wwpdb.utils.emdb-1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,16 @@
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     entry_points={"console_scripts": ["em_emd_conversion=wwpdb.utils.config.emdb.cif_emdb_translator:main"]},
     #
-    install_requires=["lxml", "mmcif", "wwpdb.utils.config>=0.22.2"],
+    install_requires=["lxml", "mmcif", "wwpdb.utils.config>=0.22.2",
+                      "mrcfile", "biopython", "numpy"],
     packages=find_packages(exclude=["wwpdb.utils.tests-emdb", "mock-data", "tests.*", "wwpdb.utils.emdb/cif_emdb)translator/*test*.py"]),
     include_package_data=True,
     package_data={
         # If any package contains *.md or *.rst ...  files, include them:
         "": ["*.md", "*.rst", "*.txt", "*.cfg"],
     },
     #
```

### Comparing `wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py` & `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
     class Constants(object):
         """
         There are many constants in use for the translation.
         They have been collected here for ease of use.
         """
 
-        XML_OUT_VERSION = "3.0.3.3"
+        XML_OUT_VERSION = "3.0.4.1"
 
         # Cif categories
         CITATION = "citation"
         CITATION_AUTHOR = "citation_author"
         DATABASE_2 = "database_2"
         EM_ADMIN = "em_admin"
         EM_DEPUI = "em_depui"
@@ -588,14 +588,15 @@
             "_em_map.pixel_spacing_z": '<xs:element name="z" type="pixel_spacing_type"/>',
             "_em_particle_selection.reference_model": '<xs:element name="reference_model" type="xs:token" minOccurs="0"/>',
             "_em_particle_selection.method": '<xs:element name="method" type="xs:string" minOccurs="0"/>',
             "_em_particle_selection.details": '<xs:element name="details" type="xs:string" minOccurs="0"/>',
             "_em_particle_selection.num_particles_selected": '<xs:element name="number_selected" type="xs:positiveInteger" minOccurs="0"/>',
             "_em_software.name": '<xs:element name="name" type="xs:token" minOccurs="0"/>',
             "_em_software.version": '<xs:element name="version" type="xs:token" minOccurs="0"/>',
+            "_em_software.category": '<xs:element name="category" type="xs:token" minOccurs="0"/>',
             "_em_software.details": '<xs:element name="processing_details" type="xs:string" minOccurs="0"/>',
             "_em_specimen.concentration": '<xs:element name="concentration" minOccurs="0">',
             "_em_specimen.id": '<xs:element name="specimen_preparation_id" type="xs:positiveInteger"/>',
             "_em_specimen.details": '<xs:element name="details" type="xs:string" minOccurs="0">',
             "_em_staining.type": '<xs:element name="type">',
             "_em_staining.material": '<xs:element name="material" type="xs:token">',
             "_em_staining.details": '<xs:element name="details" type="xs:string" minOccurs="0">',
@@ -789,14 +790,18 @@
             "_pdbx_contact_author.phone": '<xs:element name="telephone" type="telephone_number_type"/>',
             "_pdbx_contact_author.fax": '<xs:element name="fax" type="telephone_number_type"/>',
             "_entity_src_nat.pdbx_ncbi_taxonomy_id": '<xs:attribute name="database">',
             "_entity_src_gen.pdbx_gene_src_ncbi_taxonomy_id": '<xs:attribute name="database">',
             "_pdbx_entity_src_syn.ncbi_taxonomy_id": '<xs:attribute name="database">',
             "_entity_poly.pdbx_seq_one_letter_code": '<xs:element name="string" type="xs:token" minOccurs="0">',
             "_struct_ref.db_name": '<xs:element name="external_references" minOccurs="0" maxOccurs="unbounded">',
+            "_struct_ref.db_code": '<xs:element name="external_references" minOccurs="0" maxOccurs="unbounded">',
+            "_struct_ref.pdbx_db_accession": '<xs:element name="external_references" minOccurs="0" maxOccurs="unbounded">',
+            "_pdbx_struct_ref_seq_depositor_info.db_name": '<xs:element name="external_references" minOccurs="0" maxOccurs="unbounded">',
+            "_pdbx_struct_ref_seq_depositor_info.db_accession": '<xs:element name="external_references" minOccurs="0" maxOccurs="unbounded">',
             "_entity_src_gen.pdbx_host_org_ncbi_taxonomy_id": '<xs:attribute name="database">',
             "_entity_src_gen.pdbx_host_org_scientific_name": '<xs:element name="organism" type="organism_type"/>',
             "_entity.formula_weight": '<xs:element name="experimental" minOccurs="0">',
             "_entity_src_nat.common_name": '<xs:element name="organism" type="organism_type"/>',
             "_entity_src_nat.pdbx_organism_scientific": '<xs:element name="organism" type="organism_type"/>',
             "_entity_src_gen.pdbx_gene_src_scientific_name": '<xs:element name="organism" type="organism_type"/>',
             "_pdbx_entity_src_syn.organism_scientific": '<xs:element name="organism" type="organism_type"/>',
@@ -1338,14 +1343,15 @@
                 const.PDBX_DATABASE_STATUS,
                 const.PDBX_ENTITY_NONPOLY,
                 const.PDBX_DEPOSITOR_INFO,
                 const.PDBX_OBS_SPR,
                 const.PDBX_AUDIT_SUPPORT,
                 const.PDBX_CONTACT_AUTHOR,
                 const.STRUCT,
+                const.STRUCT_REF,
                 const.STRUCT_KEYWORDS,
                 const.PDBX_ENTITY_SRC_SYN,
                 const.EM_SUPERSEDE,
                 const.EM_OBSOLETE,
             ],
         )
         self.cif = Cif(container)
@@ -1357,15 +1363,15 @@
         Write out XML file.
         A translation from cif to XML needs to have taken place.
 
         Parameters:
         @param xml_out_file_name: name of the xml file
         """
         # self.xml_out is the xml object representing conversion from cif
-        if self.xml_out is None or self.xml_out._hasContent() is False:
+        if self.xml_out is None or self.xml_out.has__content() is False:
             txt = u"There is no content to write out. No output file will be written."
             self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
             self.log_formatted(self.error_log_string, "(" + self.entry_in_translation_log.id + ")" + self.Constants.REQUIRED_ALERT + txt)
             return
         # xml_out_file is the actual xml file that will be written into and saved
         xml_out_file = open(xml_out_file_name, "w") if xml_out_file_name else sys.stdout
         xml_out_file.write('<?xml version="1.0" encoding="UTF-8"?>\n')
@@ -1795,36 +1801,45 @@
                 def set_el_version(soft, soft_in):
                     """
                     XSD: <xs:element name="version" type="xs:token" minOccurs="0"/>
                     CIF: _em_software.version
                     """
                     set_cif_value(soft.set_version, "version", const.EM_SOFTWARE, cif_list=soft_in)
 
+                def set_el_category(soft, soft_in):
+                    """
+                    XSD: <xs:element name="category" type="xs:token" minOccurs="0"/>
+                    CIF: _em_software.category
+                    """
+                    set_cif_value(soft.set_category, "category", const.EM_SOFTWARE, cif_list=soft_in)
+
                 def set_el_processing_details(soft, soft_in):
                     """
                     XSD: <xs:element name="processing_details" type="xs:string" minOccurs="0"/>
                     CIF: _em_software.details
                     """
                     set_cif_value(soft.set_processing_details, "details", const.EM_SOFTWARE, cif_list=soft_in)
 
                 # element 1
                 set_el_name(soft, soft_in)
                 # element 2
                 set_el_version(soft, soft_in)
                 # element 3
+                set_el_category(soft, soft_in)
+                # element 4
                 set_el_processing_details(soft, soft_in)
 
             if software_category in category_dict:
                 soft_list = emdb.software_list_type()
                 for soft_in in category_dict[software_category]:
                     soft = emdb.software_type()
                     set_software_type(software_category, soft, soft_in)
-                    if soft._hasContent():
+                    if soft.has__content():
                         soft_list.add_software(soft)
-                if soft_list._hasContent():
+                if soft_list.has__content():
                     setter_func(soft_list)
 
         def assert_get_value(key, dic):
             """
             Return dict[value] but throw an exception if key is not found
 
             @param key: key of (key,value) pair
@@ -2088,15 +2103,15 @@
                         obs_entry = emdb.supersedes_type()
                         set_supersedes_type(obs_entry, obs_in)
                         obs_list.add_entry(obs_entry)
 
                 obsolete_in = make_dict(const.EM_OBSOLETE, "id")
                 obs_list = emdb.obsolete_listType()
                 set_obsolete_list_type(obs_list, obsolete_in)
-                if obs_list._hasContent():
+                if obs_list.has__content():
                     admin.set_obsolete_list(obs_list)
 
             def set_el_superseded_by_list(admin):
                 """
                 If this element appears means that the current entry is obsoleted.
                 The newer entry which replaces this entry is listed here.
                 XSD: <xs:element name="superseded_by_list" minOccurs="0"> has
@@ -2148,15 +2163,15 @@
                         spr_entry = emdb.supersedes_type()
                         set_supersede_entry(spr_entry, spr_in)
                         supersed_list.add_entry(spr_entry)
 
                 supr_in = make_dict(const.EM_SUPERSEDE, "id")
                 supersede_list = emdb.superseded_by_listType()
                 set_supersede_by_list(supersede_list, supr_in)
-                if supersede_list._hasContent():
+                if supersede_list.has__content():
                     admin.set_superseded_by_list(supersede_list)
 
             def set_el_grant_support(admin, aud_sup_in):
                 """
                 XSD: <xs:element name="grant_support" minOccurs="0">
                 CIF: _pdbx_audit_support
                 """
@@ -2204,20 +2219,20 @@
                     for _aud_sup_key, aud_sup in aud_sup_in.items():
                         el_funding_body = get_cif_value("funding_organization", const.PDBX_AUDIT_SUPPORT, cif_list=aud_sup)
                         # el_code = get_cif_value('grant_number', const.PDBX_AUDIT_SUPPORT, cif_list=aud_sup)
                         # el_country = get_cif_value('country', const.PDBX_AUDIT_SUPPORT, cif_list=aud_sup)
                         if el_funding_body is not None:  # or el_code is not None or el_country is not None:
                             grant_ref = emdb.grant_reference_type()
                             set_grant_reference_type(grant_ref, aud_sup)
-                            if grant_ref._hasContent():
+                            if grant_ref.has__content():
                                 grant_support.add_grant_reference(grant_ref)
 
                 grant_support = emdb.grant_supportType()
                 set_grant_support_type(grant_support, aud_sup_in)
-                if grant_support._hasContent():
+                if grant_support.has__content():
                     admin.set_grant_support(grant_support)
 
             def set_el_contact_author(admin, contact_auth_in):
                 """
                 XSD: <xs:element name="contact_author" maxOccurs="unbounded" minOccurs="0">
                 CIF: _pdbx_contact_author
                 """
@@ -2427,33 +2442,27 @@
                     el_email,
                     el_telephone,
                     el_fax,
                 ]
                 if any(x is not None for x in contact_author_type_list):
                     cont_author = emdb.contact_authorType()
                     set_contact_author_type(cont_author, contact_auth_in)
-                    if cont_author._hasContent():
+                    if cont_author.has__content():
                         admin.add_contact_author(cont_author)
 
             def set_el_title(admin):
                 """
                 XSD: <xs:element name="title" type="xs:token">
                 The value is _struct.title if _em_depui.same_title_as_pdb.
                 Otherwise it is _em_admin.title
                 CIF: _em_depui.same_title_as_pdb  YES/NO
                     YES: CIF: _struct.title
                     NO: CIF: _em_admin.title
                 """
-                same_as_pdb = get_cif_value("same_title_as_pdb", const.EM_DEPUI)
-                if same_as_pdb == "YES":
-                    # CIF: _struct.title
-                    set_cif_value(admin.set_title, "title", const.STRUCT)
-                else:
-                    # CIF: _em_admin.title
-                    set_cif_value(admin.set_title, "title", const.EM_ADMIN)
+                set_cif_value(admin.set_title, "title", const.EM_ADMIN)
 
             def set_el_authors_list(admin):
                 """
                 XSD: <xs:element name="authors_list_type"> is a sequence of elements <author>
                 CIF: _em_depui.same_authors_as_pdb YES/NO
                     YES: CIF: _em_author_list
                         _em_author_list.ordinal
@@ -2466,63 +2475,51 @@
                         _audit_author.name
                         _audit_author.pdbx_ordinal
                         _audit_author.identifier_ORCID
                         ? 'First, A.'           1  0000-0002-5251-4674
                         ? 'Second-Second, B.' 2  0000-0001-6748-9339
                 """
 
-                def set_authors_list_type(authors_list, authors_in, same_as_pdb):
+                def set_authors_list_type(authors_list, authors_in):
                     """
                     XSD: <xs:element name="authors_list"> has
                      ... 1 element of author_ORCID_type
                     """
 
-                    def set_author_orcid_type(author_with_ORCID, auth_in, same_as_pdb):
+                    def set_author_orcid_type(author_with_ORCID, auth_in):
                         """
-                        XSD: <xs:complexType name="author_ORCID_type"> extends author_type and has
+                        XSD: <xs:complexType name="author_ORCID_type"> extends author_type and hashttps://rcsbpdb.atlassian.net/browse/DAOTHER-2725has
                         ... 1 attribute
                         XSD: <xs:attribute name="ORCID" type="ORCID_type"/>
                             CIF: _audit_author.identifier_ORCID  ? 'First, A.'           1  0000-0002-5251-4674
                             CIF: _em_author_list.ordinal            1
                                  _em_author_list.author             'Turner, J.'
                                  _em_author_list.identifier_ORCID   0000-0002-5251-4674
                         """
-                        if same_as_pdb == "YES":
-                            # CIF: _audit_author
-                            set_cif_value(author_with_ORCID.set_ORCID, "identifier_ORCID", const.AUDIT_AUTHOR, cif_list=auth_in)
-                            author = get_cif_value("name", const.AUDIT_AUTHOR, cif_list=auth_in)
-                        else:
-                            # CIF: _em_author_list
-                            set_cif_value(author_with_ORCID.set_ORCID, "identifier_ORCID", const.EM_AUTHOR_LIST, cif_list=auth_in)
-                            author = get_cif_value("author", const.EM_AUTHOR_LIST, cif_list=auth_in)
+
+                        set_cif_value(author_with_ORCID.set_ORCID, "identifier_ORCID", const.EM_AUTHOR_LIST, cif_list=auth_in)
+                        author = get_cif_value("author", const.EM_AUTHOR_LIST, cif_list=auth_in)
 
                         fmt_auth = format_author(author)
                         if fmt_auth != "":
                             author_with_ORCID.set_valueOf_(fmt_auth)
                         else:
                             txt = u"Author (%s) is not added to the list of authors as the format is wrong." % author
                             self.current_entry_log.warn_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.warn_title + txt))
                             self.log_formatted(self.warn_log_string, const.NOT_REQUIRED_ALERT + txt)
 
                     for _auth_id, auth_in in authors_in.items():
                         author_with_orcid = emdb.author_ORCID_type()
-                        set_author_orcid_type(author_with_orcid, auth_in, same_as_pdb)
+                        set_author_orcid_type(author_with_orcid, auth_in)
                         authors_list.add_author(author_with_orcid)
 
-                authors_in = {}
-                same_as_pdb = get_cif_value("same_authors_as_pdb", const.EM_DEPUI)
-                if same_as_pdb == "YES":
-                    # CIF: _audit_author
-                    authors_in = make_dict(const.AUDIT_AUTHOR, "pdbx_ordinal", 2)
-                else:  # same_as_pdb == 'NO' or None
-                    # CIF: _em_author_list
-                    authors_in = make_dict(const.EM_AUTHOR_LIST, "ordinal", 2)
+                authors_in = make_dict(const.EM_AUTHOR_LIST, "ordinal", 2)
 
                 authors_list = emdb.authors_listType()
-                set_authors_list_type(authors_list, authors_in, same_as_pdb)
+                set_authors_list_type(authors_list, authors_in)
                 admin.set_authors_list(authors_list)
 
             def set_el_details():
                 """
                 EMDB administration details
                 XSD: <xs:element name="details" type="xs:token" minOccurs="0">
                 CIF: _em_admin.details
@@ -2668,15 +2665,15 @@
                         XSD: <xs:element name="author" type="author_order_type" maxOccurs="unbounded"/>
                         Citation authors
                         """
                         if cite_id_in in auth_dict:
                             if len(auth_dict[cite_id_in]) > 0:
                                 for auth_in in auth_dict[cite_id_in]:
                                     author = emdb.author_order_type(valueOf_=format_author(auth_in[0]), ORCID=auth_in[2], order=int(auth_in[1]))
-                                    if author._hasContent():
+                                    if author.has__content():
                                         pub.add_author(author)
                             else:
                                 txt = u"No authors for citation id (%s) found. At least one is required." % cite_id_in
                                 self.current_entry_log.error_logs.append(
                                     self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt)
                                 )
                                 self.log_formatted(self.error_log_string, "(" + self.entry_in_translation_log.id + ")" + const.REQUIRED_ALERT + txt)
@@ -3185,31 +3182,36 @@
                         emdb_ref_list_in = x_ref_dict_in["EMDB"]
                         for emdb_ref_in in emdb_ref_list_in:
                             emdb_ref = emdb.emdb_cross_reference_type()
                             set_ref_el_emdb_id(emdb_ref, emdb_ref_in)
                             set_ref_el_relationship(emdb_ref, emdb_ref_in)
                             set_ref_el_details(emdb_ref, emdb_ref_in)
 
-                            if emdb_ref._hasContent():
+                            if emdb_ref.has__content():
                                 emdb_ref_list.add_emdb_reference(emdb_ref)
 
                     if "EMDB" in rel_entries_dict_in:
                         emdb_rel_list_in = rel_entries_dict_in["EMDB"]
                         for rel_in in emdb_rel_list_in:
-                            cross_ref = emdb.emdb_cross_reference_type()
-                            set_rel_el_emdb_id(cross_ref, rel_in)
-                            set_rel_el_relationship(cross_ref, rel_in)
-                            set_rel_el_details(cross_ref, rel_in)
+                            em_id = get_cif_value("db_id", const.PDBX_DATABASE_RELATED, rel_in)
+                            db2_in = assert_get_value(const.DATABASE_2, self.cif)
+                            dict_db2_in = {t[0]: t[1] for t in db2_in}
+                            emdb_id = dict_db2_in[('_database_2.database_id', 'EMDB')][1]
+                            if em_id != emdb_id:
+                                cross_ref = emdb.emdb_cross_reference_type()
+                                set_rel_el_emdb_id(cross_ref, rel_in)
+                                set_rel_el_relationship(cross_ref, rel_in)
+                                set_rel_el_details(cross_ref, rel_in)
 
-                            if cross_ref._hasContent():
-                                emdb_ref_list.add_emdb_reference(cross_ref)
+                                if cross_ref.has__content():
+                                    emdb_ref_list.add_emdb_reference(cross_ref)
 
                 emdb_ref_list = emdb.emdb_cross_reference_list_type()
                 set_emdb_cross_ref_list_type(emdb_ref_list, x_ref_dict_in)
-                if emdb_ref_list._hasContent():
+                if emdb_ref_list.has__content():
                     cross_references.set_emdb_list(emdb_ref_list)
 
             def set_el_pdb_list(cross_references, x_ref_dict_in):
                 """
                 XSD: <xs:element name="pdb_list" type="pdb_cross_reference_list_type" minOccurs="0">
                 """
 
@@ -3238,15 +3240,15 @@
                         txt = None
                         if rel_in == "IN FRAME":
                             pdb_ref.set_relationship(emdb.relationshipType(in_frame="FULLOVERLAP"))
                             txt = u"The value (FULLOVERLAP) is given to (pdb_ref.set_relationship)."
                         else:
                             pdb_ref.set_relationship(emdb.relationshipType(other="unknown"))
                             txt = u"The value (unknown) is given to (pdb_ref.set_relationship)."
-                        if pdb_ref._hasContent():
+                        if pdb_ref.has__content():
                             pdb_ref_list.add_pdb_reference(pdb_ref)
                             if txt is not None:
                                 self.current_entry_log.warn_logs.append(
                                     self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.change_title + txt)
                                 )
                                 self.log_formatted(self.warn_log_string, const.CHANGE_MADE + txt)
 
@@ -3269,15 +3271,15 @@
                             set_el_relationship(pdb_ref, pdb_ref_in)
                             # element 3
                             set_el_details(pdb_ref, pdb_ref_in)
 
                 if "PDB" in x_ref_dict_in:
                     pdb_ref_list = emdb.pdb_cross_reference_list_type()
                     set_pdb_cross_ref_list_type(pdb_ref_list, x_ref_dict_in)
-                    if pdb_ref_list._hasContent():
+                    if pdb_ref_list.has__content():
                         cross_references.set_pdb_list(pdb_ref_list)
 
             def set_el_auxiliary_link_list(cross_references):
                 """
                 <xs:element name="auxiliary_link_list" minOccurs="0">
                 ..a list of one and only one element
                 """
@@ -3316,17 +3318,17 @@
                     set_el_details()
 
                 aux_link_list = emdb.auxiliary_link_listType()
                 aux_link_list_in = self.cif.get(const.EM_DB_REFERENCE_AUXILIARY)
                 for aux_in in aux_link_list_in:
                     aux = emdb.auxiliary_link_type()
                     set_aux_link_type(aux, aux_in)
-                    if aux._hasContent():
+                    if aux.has__content():
                         aux_link_list.add_auxiliary_link(aux)
-                if aux_link_list._hasContent():
+                if aux_link_list.has__content():
                     cross_references.set_auxiliary_link_list(aux_link_list)
 
             # element 1
             set_el_citation_list(cross_references)
             x_ref_dict_in = make_list_of_dicts(const.EM_DB_REFERENCE, "db_name")
             # element 2
             set_el_emdb_list(cross_references, x_ref_dict_in)
@@ -3699,15 +3701,15 @@
                             # element 3
                             # XSD: <xs:element name="method" type="xs:token" minOccurs="0"/>
                             # CIF: method doesn't exist in the dictionary!!!!
                             # mol_weight.set_method()
 
                     mol_weight = emdb.molecular_weight_type()
                     set_molecular_weight_type(mol_weight)
-                    if mol_weight._hasContent():
+                    if mol_weight.has__content():
                         supra_mol.set_molecular_weight(mol_weight)
 
                 def set_sup_mol_base_source(sup_mol, cif_category, src_in):
                     """
                     Creates the base source element for supramolecules
 
                     Parameters:
@@ -3786,15 +3788,15 @@
                         if flags_dict["add_cell"]:
                             set_el_cell(nat_src, cif_category, sup_mol_nat_src_in)
                         if flags_dict["add_organelle"]:
                             set_el_organelle(nat_src, cif_category, sup_mol_nat_src_in)
                         if flags_dict["add_cellular_location"]:
                             set_el_cellular_location(nat_src, cif_category, sup_mol_nat_src_in)
 
-                        if nat_src._hasContent():
+                        if nat_src.has__content():
                             if flags_dict["add_nat_src"]:
                                 sup_mol.add_natural_source(nat_src)
                             else:
                                 sup_mol.set_natural_source(nat_src)
                             break
 
                 def set_sup_mol_rec_exp(sup_mol, sup_mol_id_in, rec_exp_dict_in, add_rec_exp=False, virus=False):
@@ -3810,15 +3812,15 @@
                     @param virus: boolean - if true use host_system instead of recombinant_expression
                     """
                     if rec_exp_dict_in is not None:
                         if sup_mol_id_in in rec_exp_dict_in:
                             for rec_exp_in in rec_exp_dict_in[sup_mol_id_in]:
                                 r_exp = emdb.recombinant_source_type()
                                 set_recombinant_source_type(r_exp, rec_exp_in)
-                                if r_exp._hasContent():
+                                if r_exp.has__content():
                                     if add_rec_exp is False:
                                         if virus is False:
                                             sup_mol.set_recombinant_expression(r_exp)
                                         else:
                                             sup_mol.set_host_system(r_exp)
                                         break
                                     else:
@@ -3921,15 +3923,15 @@
                                 for m_in in macro_list_in:
                                     a_macromol = emdb.macromoleculeType(macromolecule_id=int(m_in))
                                     a_macromol.original_tagname_ = "macromolecule"
                                     macro_list.add_macromolecule(a_macromol)
                                 txt = u"Macromolecule (%s) added to the list of macromolecules." % int(m_in)  # pylint: disable=undefined-loop-variable
                                 self.current_entry_log.info_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.info_title + txt))
                                 self.log_formatted(self.info_log_string, const.INFO_ALERT + txt)
-                                if macro_list._hasContent():
+                                if macro_list.has__content():
                                     sup_mol.set_macromolecule_list(macro_list)
                             else:
                                 txt = u"No macromolecule found for (%s)." % id_list_item
                                 self.current_entry_log.warn_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.warn_title + txt))
                                 self.log_formatted(self.warn_log_string, const.NOT_REQUIRED_ALERT + txt)
 
                     def set_el_details(sup_mol, sup_in):
@@ -4116,15 +4118,15 @@
                                 set_attr_ncbi(virus_name, nat_src_in)
                                 set_cif_value(virus_name.set_valueOf_, "organism", const.EM_ENTITY_ASSEMBLY_NATURALSOURCE, cif_list=nat_src_in)
                                 # additionally, set the supramolecule name
                                 set_cif_value(virus_sup_mol.set_name, "organism", const.EM_ENTITY_ASSEMBLY_NATURALSOURCE, cif_list=nat_src_in, constructor=emdb.sci_name_type)
 
                             virus_name = emdb.virus_species_name_type()
                             set_virus_species_name_type(virus_name)
-                            if virus_name._hasContent():
+                            if virus_name.has__content():
                                 virus_sup_mol.set_sci_species_name(virus_name)
 
                         def set_el_sci_species_strain(virus_sup_mol, nat_src_in):
                             """
                             XSD: <xs:element name="sci_species_strain" type="xs:string" maxOccurs="1" minOccurs="0">
                             XPath: /element(*,virus_supramolecule_type)/sci_species_strain
                             CIF: _em_entity_assembly_naturalsource.strain ?
@@ -4206,15 +4208,15 @@
                                 nat_host_list_in = virus_nat_host_dict_in[sup_mol_id_in]
                                 for nat_host_in in nat_host_list_in:
                                     attr_ncbi = get_cif_value("ncbi_tax_id", const.EM_VIRUS_NATURAL_HOST, cif_list=nat_host_in)
                                     organism = get_cif_value("organism", const.EM_VIRUS_NATURAL_HOST, cif_list=nat_host_in)
                                     if any(x is not None for x in [attr_ncbi, organism]):
                                         nat_host = emdb.virus_host_type()
                                         set_virus_natural_host_type(nat_host, nat_host_in)
-                                        if nat_host._hasContent():
+                                        if nat_host.has__content():
                                             virus_sup_mol.add_natural_host(nat_host)
 
                         def set_el_host_system(virus_sup_mol, sup_mol_id_in, rec_exp_dict_in):
                             """
                             XSD: <xs:element name="host_system" type="recombinant_source_type">
                             """
                             set_sup_mol_rec_exp(virus_sup_mol, sup_mol_id_in, rec_exp_dict_in, virus=True)
@@ -4272,15 +4274,15 @@
                                     # element 1
                                     set_el_name(virus_shell, vs_in)
                                     # element 2
                                     set_el_diameter(virus_shell, vs_in)
                                     # element 3
                                     set_el_triangulation(virus_shell, vs_in)
 
-                                    if virus_shell._hasContent():
+                                    if virus_shell.has__content():
                                         virus_sup_mol.add_virus_shell(virus_shell)
 
                         def set_el_virus_type(virus_sup_mol, virus_in):
                             """
                             XSD:  <xs:element name="virus_type">; base xs:token with restriction
                             CIF: _em_virus_entity.virus_type PRION
                             """
@@ -4619,35 +4621,35 @@
                                 # (RIBOSOME or COMPLEX), VIRUS, ORGANELLE OR CELLULAR COMPONENT,
                                 # TISSUE, CELL
                                 sup_type = get_cif_value("type", const.EM_ENTITY_ASSEMBLY, sup_in)
                                 if sup_type is not None:
                                     if sup_type in ["RIBOSOME", "COMPLEX"]:
                                         complex_sup_mol = emdb.complex_supramolecule_type()
                                         set_complex_supramolecule_type(complex_sup_mol, sup_in, sup_mol_id_in, sup_mol_dicts, sample)
-                                        if complex_sup_mol._hasContent():
+                                        if complex_sup_mol.has__content():
                                             sup_list.add_supramolecule(complex_sup_mol)
                                     elif sup_type == "VIRUS":
                                         virus_sup_mol = emdb.virus_supramolecule_type()
                                         set_virus_supramolecule_type(virus_sup_mol, sup_in, sup_mol_id_in, sup_mol_dicts, sample)
-                                        if virus_sup_mol._hasContent():
+                                        if virus_sup_mol.has__content():
                                             sup_list.add_supramolecule(virus_sup_mol)
                                     elif sup_type == "ORGANELLE OR CELLULAR COMPONENT":
                                         org_or_cell_sup_mol = emdb.organelle_or_cellular_component_supramolecule_type()
                                         set_orgorcell_supmol_type(org_or_cell_sup_mol, sup_in, sup_mol_id_in, sup_mol_dicts, sample)
-                                        if org_or_cell_sup_mol._hasContent():
+                                        if org_or_cell_sup_mol.has__content():
                                             sup_list.add_supramolecule(org_or_cell_sup_mol)
                                     elif sup_type == "TISSUE":
                                         tissue_sup_mol = emdb.tissue_supramolecule_type()
                                         set_tissue_supramolecule_type(tissue_sup_mol, sup_in, sup_mol_id_in, sup_mol_dicts, sample)
-                                        if tissue_sup_mol._hasContent():
+                                        if tissue_sup_mol.has__content():
                                             sup_list.add_supramolecule(tissue_sup_mol)
                                     elif sup_type == "CELL":
                                         cell_sup_mol = emdb.cell_supramolecule_type()
                                         set_cell_supramolecule_type(cell_sup_mol, sup_in, sup_mol_id_in, sup_mol_dicts, sample)
-                                        if cell_sup_mol._hasContent():
+                                        if cell_sup_mol.has__content():
                                             sup_list.add_supramolecule(cell_sup_mol)
                                     else:
                                         txt = u"Supramolecule type not implemented. (_em_entity_assembly.type) is (%s)" % sup_type
                                         self.current_entry_log.error_logs.append(
                                             self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt)
                                         )
                                         self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
@@ -4896,15 +4898,15 @@
                         genetically modified or synthetic sources keyed by entity_id
                     @param cif_category: contains the source info
                     XSD: <xs:element name="natural_source" type="molecule_source_type" minOccurs="0"/>
                     """
                     if ent_src_dict is not None and cif_category is not None:
                         mol_src_dict = {"add_organ": True, "add_tissue": True, "add_cell": True, "add_organelle": True, "add_cellular_location": True}
                         nat_src = make_mol_src(cif_category, ent_src_dict, mol_src_dict)
-                        if nat_src._hasContent():
+                        if nat_src.has__content():
                             mol.set_natural_source(nat_src)
 
                 def set_base_mol_with_dict(mol, ent_in, ent_id_in, mol_dicts):
                     """
                     Set the dictionary and cif category for base_macromolecule_type
 
                     Parameters:
@@ -5059,47 +5061,70 @@
                         """
 
                         def set_external_references_type(cross_ref, rel_in):
                             """
                             XSD: <xs:element name="external_references" maxOccurs="unbounded" minOccurs="0"> has
                             .. 1 attribute
                             .. an extension of xs:token
+                            FOr Map-model entries:
                             CIF: _struct_ref.db_name UNP
                             CIF: _struct_ref.db_code ?
-                            """
-                            db_code = get_cif_value("db_code", const.STRUCT_REF, rel_in)
-                            if db_code is not None:
-                                db_in = get_cif_value("db_name", const.STRUCT_REF, rel_in)
-                                if db_in == "UNP":
-                                    set_cif_value(cross_ref.set_type, "db_name", const.STRUCT_REF, cif_list=rel_in, cif_value="UNIPROTKB")
-                                    set_cif_value(cross_ref.set_valueOf_, "db_code", const.STRUCT_REF, cif_list=rel_in)
-                                elif db_in == "GB":
-                                    set_cif_value(cross_ref.set_type, "db_name", const.STRUCT_REF, cif_list=rel_in, cif_value="GENBANK")
-                                    set_cif_value(cross_ref.set_valueOf_, "db_code", const.STRUCT_REF, cif_list=rel_in)
-                                elif db_in is not None:
-                                    set_cif_value(cross_ref.set_type, "db_name", const.STRUCT_REF, cif_list=rel_in)
-                                    set_cif_value(cross_ref.set_valueOf_, "db_code", const.STRUCT_REF, cif_list=rel_in)
+                            For map only entries:
+                            CIF: _pdbx_struct_ref_seq_depositor_info.db_name UNP
+                            CIF: _pdbx_struct_ref_seq_depositor_info.db_accession ?
+                            """
+                            db2_in = assert_get_value(const.DATABASE_2, self.cif)
+                            db_id_dict = make_list_of_dicts(const.DATABASE_2, "database_id", db2_in, 2)
+                            if "PDB" in db_id_dict:
+                                dict_db2_in = {t[0]: t[1] for t in db2_in}
+                                pdb_id = dict_db2_in[('_database_2.database_id', 'PDB')][1]
+                                if pdb_id is not None:
+                                    db_code = get_cif_value("db_code", const.STRUCT_REF, rel_in)
+                                    if db_code is not None:
+                                        db_in = get_cif_value("db_name", const.STRUCT_REF, rel_in)
+                                        if db_in == "UNP":
+                                            set_cif_value(cross_ref.set_type, "db_name", const.STRUCT_REF, cif_list=rel_in, cif_value="UNIPROTKB")
+                                            set_cif_value(cross_ref.set_valueOf_, "pdbx_db_accession", const.STRUCT_REF, cif_list=rel_in)
+                                        elif db_in == "GB":
+                                            set_cif_value(cross_ref.set_type, "db_name", const.STRUCT_REF, cif_list=rel_in, cif_value="GENBANK")
+                                            set_cif_value(cross_ref.set_valueOf_, "db_code", const.STRUCT_REF, cif_list=rel_in)
+                                        elif db_in is not None and db_in != "PDB":
+                                            set_cif_value(cross_ref.set_type, "db_name", const.STRUCT_REF, cif_list=rel_in)
+                                            set_cif_value(cross_ref.set_valueOf_, "db_code", const.STRUCT_REF, cif_list=rel_in)
+                            if "PDB" not in db_id_dict:
+                                db_code = get_cif_value("db_accession", const.PDBX_DEPOSITOR_INFO, rel_in)
+                                if db_code is not None:
+                                    db_in = get_cif_value("db_name", const.PDBX_DEPOSITOR_INFO, rel_in)
+                                    if db_in == "UNP":
+                                        set_cif_value(cross_ref.set_type, "db_name", const.PDBX_DEPOSITOR_INFO, cif_list=rel_in, cif_value="UNIPROTKB")
+                                        set_cif_value(cross_ref.set_valueOf_, "db_accession", const.PDBX_DEPOSITOR_INFO, cif_list=rel_in)
+                                    elif db_in == "GB":
+                                        set_cif_value(cross_ref.set_type, "db_name", const.PDBX_DEPOSITOR_INFO, cif_list=rel_in, cif_value="GENBANK")
+                                        set_cif_value(cross_ref.set_valueOf_, "db_accession", const.PDBX_DEPOSITOR_INFO, cif_list=rel_in)
+                                    elif db_in is not None and db_in != "PDB":
+                                        set_cif_value(cross_ref.set_type, "db_name", const.PDBX_DEPOSITOR_INFO, cif_list=rel_in)
+                                        set_cif_value(cross_ref.set_valueOf_, "db_accession", const.PDBX_DEPOSITOR_INFO, cif_list=rel_in)
 
                         if ent_id_in in ent_ref_dict:
                             ent_ref_list_in = ent_ref_dict[ent_id_in]
                             for rel_in in ent_ref_list_in:
                                 cross_ref = emdb.external_referencesType()
                                 set_external_references_type(cross_ref, rel_in)
-                                if cross_ref._hasContent():
+                                if cross_ref.has__content():
                                     seq.add_external_references(cross_ref)
 
                     seq = emdb.sequenceType()
                     # element 1
                     set_el_string(seq, ent_poly_in)
                     # element 2
                     set_el_discrepancy_list()
                     # element 3
                     set_el_external_references(seq, ent_id_in, ent_ref_dict)
 
-                    if seq._hasContent():
+                    if seq.has__content():
                         mol.set_sequence(seq)
 
                 def set_mol_rec_exp(mol, ent_id_in, mol_rec_exp_dict):
                     """
                     Set recombinant expression for a macromolecule
 
                     Parameters:
@@ -5112,15 +5137,15 @@
                     .. 5 elements
                     """
                     if mol_rec_exp_dict is not None:
                         if ent_id_in in mol_rec_exp_dict:
                             r_exp_in = mol_rec_exp_dict[ent_id_in]
                             r_exp = emdb.recombinant_source_type()
                             set_recombinant_source_type(r_exp, r_exp_in)
-                            if r_exp._hasContent():
+                            if r_exp.has__content():
                                 mol.set_recombinant_expression(r_exp)
                     else:
                         txt = u"The dictionary for recombinant expression for macromolecule id (%s) not found." % ent_id_in
                         self.current_entry_log.warn_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.warn_title + txt))
                         self.log_formatted(self.warn_log_string, const.NOT_REQUIRED_ALERT + txt)
 
                 def set_mol_syn_src(syn_src, mol, cif_category, src_dict_in, flags_dict):
@@ -5190,33 +5215,33 @@
                         if flags_dict["add_cell"]:
                             set_el_cell(syn_src, cif_category, mol_syn_src_in)
                         if flags_dict["add_organelle"]:
                             set_el_organelle(syn_src, cif_category, mol_syn_src_in)
                         if flags_dict["add_cellular_location"]:
                             set_el_cellular_location(syn_src, cif_category, mol_syn_src_in)
 
-                        if syn_src._hasContent():
+                        if syn_src.has__content():
                             if flags_dict["add_syn_src"]:
                                 mol.add_synthetic_source(syn_src)
                             else:
                                 mol.set_synthetic_source(syn_src)
                             break
 
                 def set_rna_macromolecule_type(rna_mol, ent_in, ent_id_in, ent_poly_in, src_dicts):
                     """
                     XSD: <xs:complexType name="rna_macromolecule_type"> has
                     .. a base of base_macromolecule_type and
                     .. a sequence of 5 elements
                     """
 
-                    def set_el_sequence(rna_mol, ent_poly_in, ent_id_in, ent_ref_dict):
+                    def set_el_sequence(rna_mol, ent_poly_in, ent_id_in, src_dict):
                         """
                         XSD:  <xs:element name="sequence">
                         """
-                        set_mol_seq(rna_mol, ent_poly_in, ent_id_in, ent_ref_dict)
+                        set_mol_seq(rna_mol, ent_poly_in, ent_id_in, src_dict)
 
                     def set_el_classification():
                         """
                         XSD: <xs:element name="classification" minOccurs="0">
                         CIF: ??
                         """
 
@@ -5271,20 +5296,20 @@
                 def set_dna_macromolecule_type(dna_mol, ent_in, ent_id_in, ent_poly_in, src_dicts):
                     """
                     XSD: <xs:complexType name="dna_macromolecule_type"> has
                     .. a base of base_macromolecule_type and
                     .. a sequence of 5 elements
                     """
 
-                    def set_el_sequence(dna_mol, ent_poly_in, ent_id_in, ent_ref_dict):
+                    def set_el_sequence(dna_mol, ent_poly_in, ent_id_in, src_dict):
                         """
                         XSD: <xs:element name="sequence">
                         CIF: in ent_ref_dict
                         """
-                        set_mol_seq(dna_mol, ent_poly_in, ent_id_in, ent_ref_dict)
+                        set_mol_seq(dna_mol, ent_poly_in, ent_id_in, src_dict)
 
                     def set_el_classification(dna_mol):
                         """
                         XSD: <xs:element name="classification" minOccurs="0">
                         CIF:
                         """
                         set_cif_value(dna_mol.set_classification, cif_value="DNA")
@@ -5381,19 +5406,19 @@
                         XSD: <xs:element name="enantiomer">
                         """
                         if ent_type_in == const.ENT_POLYPEPTIDE_D:
                             set_cif_value(p_mol.set_enantiomer, cif_value="DEXTRO")
                         else:
                             set_cif_value(p_mol.set_enantiomer, cif_value="LEVO")
 
-                    def set_el_sequence(p_mol, ent_poly_in, ent_id_in, ent_ref_dict):
+                    def set_el_sequence(p_mol, ent_poly_in, ent_id_in, src_dict):
                         """
                         XSD: <xs:element name="sequence">
                         """
-                        set_mol_seq(p_mol, ent_poly_in, ent_id_in, ent_ref_dict)
+                        set_mol_seq(p_mol, ent_poly_in, ent_id_in, src_dict)
 
                     def set_el_ec_number(p_mol, ent_in):
                         """
                         XSD: <xs:element name="ec_number" maxOccurs="unbounded" minOccurs="0">
                         CIF: _entity.pdbx_ec ? (Enzyme classification. Format: "EC 3.4.11.4")
                         """
                         ec_num_in = get_cif_value("pdbx_ec", const.ENTITY, cif_list=ent_in)
@@ -5469,19 +5494,19 @@
                 def set_other_macromolecule_type(other_mol, ent_in, ent_id_in, ent_poly_in, src_dicts):
                     """
                     XSD: <xs:complexType name="other_macromolecule_type"> has
                     .. a base of base_macromolecule_type and
                     .. a sequence of 5 elements
                     """
 
-                    def set_el_sequence(other_mol, ent_poly_in, ent_id_in, ent_ref_dict):
+                    def set_el_sequence(other_mol, ent_poly_in, ent_id_in, src_dict):
                         """
                         XSD: <xs:element name="sequence" minOccurs="0">
                         """
-                        set_mol_seq(other_mol, ent_poly_in, ent_id_in, ent_ref_dict)
+                        set_mol_seq(other_mol, ent_poly_in, ent_id_in, src_dict)
 
                     def set_el_classification():
                         """
                         XSD: <xs:element name="classification" type="xs:token">
                         """
                         other_mol.set_classification(ent_type_in)
 
@@ -5571,14 +5596,16 @@
                 # Create dictionaries keyed by entity_id
                 ent_poly_dict = make_dict(const.ENTITY_POLY, const.K_ENTITY_ID)
                 ent_non_poly_dict = make_dict(const.PDBX_ENTITY_NONPOLY, const.K_ENTITY_ID)
                 ent_src_nat_dict = make_dict(const.ENTITY_SRC_NAT, const.K_ENTITY_ID)
                 ent_src_gen_dict = make_dict(const.ENTITY_SRC_GEN, const.K_ENTITY_ID)
                 ent_src_syn_dict = make_dict(const.PDBX_ENTITY_SRC_SYN, const.K_ENTITY_ID)
                 ent_ref_dict = make_list_of_dicts(const.PDBX_DEPOSITOR_INFO, const.K_ENTITY_ID)
+                struct_ref_dict = make_list_of_dicts(const.STRUCT_REF, const.K_ENTITY_ID)
+                ent_ref_dict.update(struct_ref_dict)
                 src_dicts = {"ent_src_nat_dict": ent_src_nat_dict, "ent_src_gen_dict": ent_src_gen_dict, "ent_src_syn_dict": ent_src_syn_dict, "ent_ref_dict": ent_ref_dict}
                 entity_list_in = self.cif.get(const.ENTITY, None)
                 for ent_in in entity_list_in:
                     ent_id_in = get_cif_value(const.K_ID, const.ENTITY, ent_in)
                     if ent_id_in in ent_poly_dict:
                         ent_poly_in = ent_poly_dict[ent_id_in]
                         ent_type_in = get_cif_value("type", const.ENTITY_POLY, ent_poly_in)
@@ -5608,15 +5635,15 @@
                             self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
                     elif ent_id_in in ent_non_poly_dict:
                         # Entity non-poly
                         lig_mol = emdb.ligand_macromolecule_type()
                         set_ligand_macromolecule_type(lig_mol, ent_in, ent_id_in, src_dicts)
                         mol_list.add_macromolecule(lig_mol)
 
-                    if mol_list._hasContent():
+                    if mol_list.has__content():
                         sample.set_macromolecule_list(mol_list)
 
             # element 1
             set_el_name()
             # element 2
             set_el_supramolecule_list(sample)
             # element 3
@@ -5808,15 +5835,15 @@
                     stain = emdb.stainingType()
                     # element 1
                     set_el_type(stain, stain_in)
                     # element 2
                     set_el_material(stain, stain_in)
                     # element 3
                     set_el_details(stain, stain_in)
-                    if stain._hasContent():
+                    if stain.has__content():
                         specimen.set_staining(stain)
 
             def set_el_sugar_embedding(specimen, sp_id_in, embed_dict_in):
                 """
                 XSD: <xs:element name="sugar_embedding" minOccurs="0">
                 """
 
@@ -5848,15 +5875,15 @@
                 if sp_id_in in embed_dict_in:
                     embed_in = embed_dict_in[sp_id_in]
                     el_material = get_cif_value("material", const.EM_EMBEDDING, cif_list=embed_in)
                     el_details = get_cif_value("details", const.EM_EMBEDDING, cif_list=embed_in)
                     if any(x is not None for x in [el_material, el_details]):
                         embed = emdb.sugar_embeddingType()
                         set_sugar_embedding_type(embed, embed_in)
-                        if embed._hasContent():
+                        if embed.has__content():
                             specimen.set_sugar_embedding(embed)
 
             def set_el_shadowing(specimen, sp_id_in, shadow_dict_in):
                 """
                 XSD: <xs:element name="shadowing" minOccurs="0">
                 """
 
@@ -5922,15 +5949,15 @@
                     el_material = get_cif_value("material", const.EM_SHADOWING, cif_list=shadow_in)
                     el_angle = get_cif_value("angle", const.EM_SHADOWING, cif_list=shadow_in)
                     el_thickness = get_cif_value("thickness", const.EM_SHADOWING, cif_list=shadow_in)
                     el_details = get_cif_value("details", const.EM_SHADOWING, cif_list=shadow_in)
                     if any(x is not None for x in [el_material, el_angle, el_thickness, el_details]):
                         shadow = emdb.shadowingType()
                         set_shadowing_type(shadow)
-                        if shadow._hasContent():
+                        if shadow.has__content():
                             specimen.set_shadowing(shadow)
 
             def set_el_grid(specimen, sp_id_in, grid_dict_in, film_dict_in, pretreat_dict_in):
                 """
                 XSD: <xs:element name="grid" type="grid_type">
                 """
 
@@ -6143,15 +6170,15 @@
                     # element 6
                     set_el_details(grid, grid_in)
 
                 if sp_id_in in grid_dict_in:
                     grid_in = grid_dict_in[sp_id_in]
                     grid = emdb.grid_type()
                     set_grid_type(grid, film_dict_in, pretreat_dict_in)
-                    if grid._hasContent():
+                    if grid.has__content():
                         specimen.set_grid(grid)
 
             def set_el_vitrification(specimen, sp_id_in, vitr_dict_in):
                 """
                 XSD: <xs:element name="vitrification" type="vitrification_type" minOccurs="0">
                 """
 
@@ -6286,15 +6313,15 @@
                     # element 7
                     set_el_method()
 
                 if sp_id_in in vitr_dict_in:
                     vitr_in = vitr_dict_in[sp_id_in]
                     vitr = emdb.vitrification_type()
                     set_vitrification_type(vitr, vitr_in)
-                    if vitr._hasContent():
+                    if vitr.has__content():
                         specimen.set_vitrification(vitr)
 
             def set_el_details(specimen, spec_prep_in):
                 """
                 XSD: <xs:element name="details" type="xs:string" minOccurs="0">
                 CIF: _em_specimen.details
                 """
@@ -6386,17 +6413,17 @@
                 fs_present = get_cif_value("fiducial_markers", const.EM_TOMOGRAPHY_SPECIMEN, tom_prep_in)
                 if tom_id_in in fid_dict_in and fs_present == "YES":
                     fid_list = emdb.fiducial_markers_listType()
                     fid_list_in = fid_dict_in[tom_id_in]
                     for fid_in in fid_list_in:
                         fid = emdb.fiducial_marker_type()
                         set_fiducial_marker_type(fid, fid_in)
-                        if fid._hasContent():
+                        if fid.has__content():
                             fid_list.add_fiducial_marker(fid)
-                    if fid_list._hasContent():
+                    if fid_list.has__content():
                         tom_prep.set_fiducial_markers_list(fid_list)
 
             def set_el_high_pressure_freezing(tom_prep, tom_id_in, h_pfdict_in):
                 """
                 XSD: <xs:element name="high_pressure_freezing" minOccurs="0">
                 CIF: _em_tomography_specimen.high_pressure_freezing YES
                 """
@@ -6449,15 +6476,15 @@
                 if tom_id_in in h_pfdict_in and hpf_present == "YES":
                     h_pf_in = h_pfdict_in[tom_id_in]
                     el_instrument = get_cif_value("instrument", const.EM_HIGH_PRESSURE_FREEZING, cif_list=h_pf_in)
                     el_details = get_cif_value("details", const.EM_HIGH_PRESSURE_FREEZING, cif_list=h_pf_in)
                     if any(x is not None for x in [el_instrument, el_details]):
                         h_pf = emdb.high_pressure_freezingType()
                         set_high_pressure_freezing_type(h_pf, h_pf_in)
-                        if h_pf._hasContent():
+                        if h_pf.has__content():
                             tom_prep.set_high_pressure_freezing(h_pf)
 
             def set_el_embedding_material():
                 """
                 XSD: <xs:element name="embedding_material" minOccurs="0" type="xs:token">
                 CIF: ??
                 """
@@ -6677,21 +6704,21 @@
 
                 sec_in = get_cif_value("sectioning", const.EM_TOMOGRAPHY_SPECIMEN, tom_prep_in)
                 if sec_in is not None:
                     if sec_in == "ULTRAMICROTOMY" and tom_id_in in u_tome_dict_in:
                         u_tome_in = u_tome_dict_in[tom_id_in]
                         u_tome = emdb.ultramicrotomyType()
                         set_ultramicrotomy_type(u_tome)
-                        if u_tome._hasContent():
+                        if u_tome.has__content():
                             tom_prep.set_sectioning(emdb.sectioningType(ultramicrotomy=u_tome))
                     elif sec_in == "FOCUSED ION BEAM" and tom_id_in in fib_dict_in:
                         fib_in = fib_dict_in[tom_id_in]
                         fib = emdb.focused_ion_beamType()
                         set_focused_ion_beam_type(fib)
-                        if fib._hasContent():
+                        if fib.has__content():
                             tom_prep.set_sectioning(emdb.sectioningType(focused_ion_beam=fib))
                     elif sec_in == "NO SECTIONING":
                         # XSD: choice 3: <xs:element name="other_sectioning" type="xs:string"/>
                         tom_prep.set_sectioning(emdb.sectioningType(other_sectioning=sec_in))
 
             # Create dictionaries where the tomography preparation id is key
             tom_prep_dict_in = make_dict(const.EM_TOMOGRAPHY_SPECIMEN, const.K_SPECIMEN_ID)
@@ -6816,15 +6843,15 @@
 
             cryst_dict_in = make_dict(const.EM_CRYSTAL_FORMATION, const.K_SPECIMEN_ID)
 
             if sp_id_in in cryst_dict_in:
                 cryst_in = cryst_dict_in[sp_id_in]
                 cryst = emdb.crystal_formationType()
                 set_crystal_formation_type(cryst)
-                if cryst._hasContent():
+                if cryst.has__content():
                     cryst_prep.set_crystal_formation(cryst)
 
         def set_classification(ip_id_in, final_class_dict_in, cat_soft_dict_in):
             """
             Classification for image processing
 
             @param ip_id_in: image processing id
@@ -7195,15 +7222,15 @@
                                 # element 3
                                 set_el_lower_energy_threshold(eng_flt, sp_op_in)
                                 # element 3
                                 set_el_upper_energy_threshold(eng_flt, sp_op_in)
 
                             eng_flt = emdb.energy_filterType()
                             set_energy_filter_type(eng_flt, sp_op_in)
-                            if eng_flt._hasContent():
+                            if eng_flt.has__content():
                                 sp_op.set_energy_filter(eng_flt)
 
                         def set_el_details(sp_op, sp_op_in):
                             """
                             XSD: <xs:element name="detals" type="xs:string" minOccurs="0"/>
                             CIF: _em_imaging_optics.details - NOT YET IMPLEMENTED IN mmcif dictionary
                             """
@@ -7472,18 +7499,18 @@
                         self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
                     else:
                         im_rec_list_in = im_rec_dict_in[mic_id]
                         im_rec_list = emdb.image_recording_listType()
                         for im_rec_in in im_rec_list_in:
                             im_rec = emdb.image_recordingType()
                             set_image_recording_type(im_rec, im_rec_in, im_dig_dict_in)
-                            if im_rec._hasContent():
+                            if im_rec.has__content():
                                 im_rec_list.add_image_recording(im_rec)
 
-                        if im_rec_list._hasContent():
+                        if im_rec_list.has__content():
                             mic.set_image_recording_list(im_rec_list)
 
                 def set_base_microscopy(mic_in, mic, mic_id):
                     """
                     Set all elements for base microscopy
 
                     Parameters:
@@ -7730,19 +7757,21 @@
                             elif align_proc == "ZEMLIN TABLEAU":
                                 ali_zem = emdb.zemlin_tableauType()
                                 ali.set_zemlin_tableau(ali_zem)
                             elif align_proc == "COMA FREE":
                                 ali_cf = emdb.coma_freeType()
                                 if tilt is not None:
                                     ali_cf.set_residual_tilt(emdb.residual_tilt_type(valueOf_=float(tilt), units=const.U_MRAD))
-                                ali.set_coma_free(ali_cf)
+                                if ali_cf.has__content():
+                                    ali.set_coma_free(ali_cf)
                             elif align_proc == "OTHER":
                                 ali_other = emdb.otherType()
                                 ali.set_other(ali_other)
-                            mic.set_alignment_procedure(ali)
+                            if ali.has__content():
+                                mic.set_alignment_procedure(ali)
 
                     def set_el_specialist_optics(mic, mic_id):
                         """
                         XSD: <xs:element name="specialist_optics" type="specialist_optics_type" minOccurs="0"/>
                         CIF: em_imaging_optics
                         """
                         set_special_optics(mic_id, mic)
@@ -7864,26 +7893,26 @@
 
                         def set_el_axis1(tilt_ser, ts_in):
                             """
                             XSD: <xs:element name="axis1" type="axis_type"/>
                             CIF:
                             """
                             axis1 = get_tilt_axis(ts_in, axis1=True)
-                            if axis1._hasContent():
+                            if axis1.has__content():
                                 set_cif_value(tilt_ser.set_axis1, axis1)
 
                         def set_el_axis2(tilt_ser, ts_in):
                             """
                             XSD: <xs:element name="axis2" minOccurs="0"> has
                             .. a base of axis_type and
                             .. 1 element <xs:element name="axis_rotation" minOccurs="0">???
                             CIF:
                             """
                             axis2 = get_tilt_axis(ts_in, axis1=False)
-                            if axis2._hasContent():
+                            if axis2.has__content():
                                 set_cif_value(tilt_ser.set_axis2, axis2)
 
                         def set_el_axis_rotation(tilt_ser, ts_in):
                             """
                             XSD: <xs:element name="axis_rotation" fixed="90" minOccurs="0">
                             CIF: _em_tomography.dual_tilt_axis_rotation
                             """
@@ -7906,15 +7935,15 @@
                     # Create list of tomography tilt series that has microscopy id as a key.
                     tilt_dict_in = make_list_of_dicts(const.EM_TOMOGRAPHY, const.K_IMAGING_ID)
                     if mic_id in tilt_dict_in:
                         tilt_list_in = tilt_dict_in[mic_id]
                         for ts_in in tilt_list_in:
                             tilt_ser = emdb.tilt_series_type()
                             set_tilt_series_type(tilt_ser, ts_in)
-                            if tilt_ser._hasContent():
+                            if tilt_ser.has__content():
                                 mic.add_tilt_series(tilt_ser)
 
                 def set_cryst_mic_specifics(mic_id, cryst_mic):
                     """
                     Method that sets the crystalograhy specific microscopy elements
 
                     Parameters:
@@ -7950,15 +7979,15 @@
                         tilt_str_in = get_cif_value("tilt_angle_list", const.EM_DIFFRACTION, cry_mic_in)
                         if tilt_str_in is not None:
                             tilt_list_in = tilt_str_in.strip().split(",")
                             tilt_list = emdb.tilt_listType()
                             for tilt_in in tilt_list_in:
                                 # XSD: <xs:element name="tilt_list" minOccurs="1">
                                 tilt_list.add_angle(float(tilt_in))
-                            if tilt_list._hasContent():
+                            if tilt_list.has__content():
                                 cryst_mic.set_tilt_list(tilt_list)
                                 # choice 2 (IS THIS NECESSARY ????????????)
                                 # XSD: <xs:element name="tilt_series"
                                 #      type="tilt_series_type" maxOccurs="unbounded" minOccurs="1">
 
                 mic_list_in = self.cif.get(const.EM_IMAGING, None)
                 if mic_list_in != []:
@@ -8104,15 +8133,15 @@
                         # element 4
                         set_el_software_list(part_sel)
                         # element 5
                         set_el_details(part_sel, ps_in)
 
                     part_sel = emdb.particle_selection_type()
                     set_particle_selection_type(part_sel)
-                    if part_sel._hasContent():
+                    if part_sel.has__content():
                         im_proc.add_particle_selection(part_sel)
 
                 def set_ctfcorrection(ip_id_in, im_proc, ctf_corr_dict_in):
                     """
                     Sets CTF correction
 
                     @param ip_id_in: image processing id
@@ -8240,15 +8269,15 @@
                         # element 4
                         set_el_software_list(ctf_corr, cat_soft_dict_in)
                         # element 5
                         set_el_details(ctf_corr, ctf_corr_in)
 
                     ctf_corr = emdb.ctf_correction_type()
                     set_ctf_correction_type(ctf_corr)
-                    if ctf_corr._hasContent():
+                    if ctf_corr.has__content():
                         im_proc.set_ctf_correction(ctf_corr)
 
                 def set_startup_model(ip_id_in, im_proc, st_mod_dict_in):
                     """
                     Sets startup model
 
                     @param ip_id_in: image processing id
@@ -8430,15 +8459,15 @@
                                     # element 1
                                     set_el_chain_id_list()
 
                                 el_pdb_id = get_cif_value("pdb_id", const.EM_START_MODEL, cif_list=sm_in)
                                 if el_pdb_id is not None:
                                     pdb_mt = emdb.pdb_model_type()
                                     set_pdb_model_type(pdb_mt)
-                                    if pdb_mt._hasContent():
+                                    if pdb_mt.has__content():
                                         st_map.set_pdb_model(pdb_mt)
 
                             def set_choice_insilico_model(st_map, sm_in):
                                 """
                                 XSD: <xs:element name="insilico_model" type="xs:token" minOccurs="0"/>
                                 CIF: _em_start_model.insilico_model
                                 """
@@ -8451,20 +8480,20 @@
                                 """
                                 set_cif_value(st_map.set_other, "other", const.EM_START_MODEL, cif_list=sm_in)
 
                             t_of_m = get_cif_value("type", const.EM_START_MODEL, sm_in)
                             if t_of_m == "RANDOM CONICAL TILT":
                                 rct = emdb.random_conical_tiltType()
                                 set_choice_random_conical_tilt(rct, sm_in)
-                                if rct._hasContent():
+                                if rct.has__content():
                                     st_map.set_random_conical_tilt(rct)
                             elif t_of_m == "ORTHOGONAL TILT":
                                 orth_tilt = emdb.orthogonal_tiltType()
                                 set_choice_orthogonal_tilt(orth_tilt, sm_in)
-                                if orth_tilt._hasContent():
+                                if orth_tilt.has__content():
                                     st_map.set_orthogonal_tilt(orth_tilt)
                             elif t_of_m == "EMDB MAP":
                                 set_choice_emdb_id(st_map, sm_in)
                             elif t_of_m == "PDB ENTRY":
                                 set_choice_pdb_model(st_map, sm_in)
                             elif t_of_m == "INSILICO MODEL":
                                 set_choice_insilico_model(st_map, sm_in)
@@ -8585,15 +8614,15 @@
                                     # element 3
                                     set_el_axial_symmetry(h_sym, h_sym_in)
                                     # element 4 - REMOVED
                                     # set_el_hand(h_sym)
 
                                 h_sym = emdb.helical_parameters_type()
                                 set_helical_parameters_type(h_sym, h_sym_in)
-                                if h_sym._hasContent():
+                                if h_sym.has__content():
                                     app_sym.set_helical_parameters(h_sym)
 
                             p_sym_dict_in = final_dicts["p_sym_dict_in"]
                             h_sym_dict_in = final_dicts["h_sym_dict_in"]
                             if sym_type_in in ["2D CRYSTAL" "3D CRYSTAL"]:  # pylint: disable=implicit-str-concat
                                 # choice 1
                                 set_choice_space_group()
@@ -8607,15 +8636,15 @@
                                     # choice 3
                                     set_choice_helical_parameters(h_sym_in)
 
                         sym_type_in = get_cif_value("symmetry_type", const.EM_3D_RECONSTRUCTION, final_rec_in)
                         if sym_type_in is not None:
                             app_sym = emdb.applied_symmetry_type()
                             set_applied_symmetry_type(app_sym, final_dicts)
-                            if app_sym._hasContent():
+                            if app_sym.has__content():
                                 final_rec.set_applied_symmetry(app_sym)
 
                     def set_el_algorithm(final_rec, final_rec_in):
                         """
                         XSD: <xs:element name="algorithm" type="reconstruction_algorithm_type"  minOccurs="0">
                         CIF: _em_3d_reconstruction.algorithm
                             {ALGEBRAIC (ARTS),BACK PROJECTION,EXACT BACK PROJECTION,
@@ -8789,19 +8818,19 @@
                             """
                             XSD: <xs:element name="software_list" type="software_list_type" minOccurs="0"/>
                             CIF: _em_euler_angle_assignment.order {FINAL,INITIAL}
                             """
                             order = get_cif_value("order", const.EM_EULER_ANGLE_ASSIGNMENT, ang_in)
                             if order == "INITIAL" and em_method == const.EMM_SP:
                                 set_software_list(const.SOFT_INITIAL_EULER_ASSIGNMENT, cat_soft_dict_in, ang.set_software_list)
-                                if ang._hasContent():
+                                if ang.has__content():
                                     im_proc.set_initial_angle_assignment(ang)
                             elif order == "FINAL":
                                 set_software_list(const.SOFT_FINAL_EULER_ASSIGNMENT, cat_soft_dict_in, ang.set_software_list)
-                                if ang._hasContent():
+                                if ang.has__content():
                                     im_proc.set_final_angle_assignment(ang)
 
                         def set_el_details(ang, ang_in):
                             """
                             XSD: <xs:element name="details" type="xs:string" minOccurs="0"/>
                             CIF: _em_euler_angle_assignment.details
                             """
@@ -8927,15 +8956,15 @@
                                 # element 6
                                 set_el_alpha(u_cell, cryst_in, dict_category)
                                 # element 7
                                 set_el_beta(u_cell, cryst_in, dict_category)
 
                             u_cell = emdb.unit_cell_type()
                             set_unit_cell_type(u_cell, cryst_in, dict_category, parent_req)
-                            if u_cell._hasContent():
+                            if u_cell.has__content():
                                 cryst.set_unit_cell(u_cell)
 
                         def set_choice_plane_group():
                             """
                             XSD: <xs:element name="plane_group">
                             CIF:????
                             """
@@ -8971,15 +9000,15 @@
                         el_choice_space_group = get_cif_value("space_group", const.EM_3D_CRYSTAL_ENTITY, cif_list=cryst_in)
                     elif dict_category == const.EM_2D_CRYSTAL_ENTITY:
                         el_choice_space_group = get_cif_value("plane_group", const.EM_2D_CRYSTAL_ENTITY, cif_list=cryst_in)
                     crystal_parameters_type_list = [el_a, el_b, el_c, el_c_sampling_length, el_gamma, el_alpha, el_beta, el_choice_space_group]
                     if any(x is not None for x in crystal_parameters_type_list):
                         cryst = emdb.crystal_parameters_type()
                         set_crystal_parameters_type(cryst, cryst_in, dict_category, parent_req)
-                        if cryst._hasContent():
+                        if cryst.has__content():
                             im_proc.set_crystal_parameters(cryst)
 
                 def set_non_sub_tom_final_recon(ip_id_in, im_proc, non_st_dicts):
                     """
                     Final reconstruction for non-subtomographs
 
                     @param ip_id_in: image processing id
@@ -9094,26 +9123,26 @@
                         """
                         XSD: <xs:element name="final_two_d_classification" type="classification_type" minOccurs="0"/>
                         """
                         final_2d_class_dict_in = sp_dict_list["final_2d_class_dict_in"]
                         cat_soft_dict_in = sp_dict_list["cat_soft_dict_in"]
                         if ip_id_in in final_2d_class_dict_in:
                             f2dc = set_classification(ip_id_in, final_2d_class_dict_in, cat_soft_dict_in)
-                            if f2dc._hasContent():
+                            if f2dc.has__content():
                                 im_proc.set_final_two_d_classification(f2dc)
 
                     def set_el_final_three_d_class(ip_id_in, im_proc, sp_dict_list):
                         """
                         XSD: <xs:element name="final_three_d_classification" type="classification_type" minOccurs="0"/>
                         """
                         final_class_dict_in = sp_dict_list["final_class_dict_in"]
                         cat_soft_dict_in = sp_dict_list["cat_soft_dict_in"]
                         if ip_id_in in final_class_dict_in:
                             f3dc = set_classification(ip_id_in, final_class_dict_in, cat_soft_dict_in)
-                            if f3dc._hasContent():
+                            if f3dc.has__content():
                                 im_proc.set_final_three_d_classification(f3dc)
 
                     # element 1
                     set_el_particle_selection(ip_id_in, im_proc, sp_dict_list)
                     # element 2
                     set_el_ctf_correction(ip_id_in, im_proc, sp_dict_list)
                     # element 3
@@ -9251,15 +9280,15 @@
                             set_el_details(extraction, vs_in)
 
                         vol_sel_dict_in = subtom_dicts["vol_sel_dict_in"]
                         if ip_id_in in vol_sel_dict_in:
                             vs_in = vol_sel_dict_in[ip_id_in]
                             extraction = emdb.extractionType()
                             set_extraction_type(extraction, vs_in, subtom_dicts)
-                            if extraction._hasContent():
+                            if extraction.has__content():
                                 im_proc.set_extraction(extraction)
 
                     def set_el_ctf_correction(im_proc, ip_id_in, subtom_dicts):
                         """
                         XSD: <xs:element name="ctf_correction" type="ctf_correction_type"/>
                         """
                         ctf_corr_dict_in = subtom_dicts["ctf_corr_dict_in"]
@@ -9276,15 +9305,15 @@
                         """
                         XSD: <xs:element name="final_three_d_classification" type="classification_type" minOccurs="0"/>
                         """
                         final_class_dict_in = subtom_dicts["final_class_dict_in"]
                         cat_soft_dict_in = subtom_dicts["cat_soft_dict_in"]
                         if ip_id_in in final_class_dict_in:
                             f3dc = set_classification(ip_id_in, final_class_dict_in, cat_soft_dict_in)
-                            if f3dc._hasContent():
+                            if f3dc.has__content():
                                 im_proc.set_final_three_d_classification(f3dc)
 
                     def set_el_final_angle_assignment(im_proc, subtom_dicts, em_method):
                         """
                         XSD: <xs:element name="final_angle_assignment" type="angle_assignment_type" minOccurs="0"/>
                         """
                         ang_dict_in = subtom_dicts["ang_dict_in"]
@@ -9440,15 +9469,15 @@
 
                         part_sel_dict_in = hel_dict_list["part_sel_dict_in"]
                         if ip_id_in in part_sel_dict_in:
                             ps_list_in = part_sel_dict_in[ip_id_in]
                             for ps_in in ps_list_in:
                                 seg_sel = emdb.segment_selection_type()
                                 set_segment_selection_type(seg_sel, ps_in)
-                                if seg_sel._hasContent():
+                                if seg_sel.has__content():
                                     im_proc.add_segment_selection(seg_sel)
 
                     def set_el_refinement(im_proc):
                         """
                         XSD: <xs:element name="refinement" type="refinement_type"/>
                         """
 
@@ -9461,15 +9490,15 @@
                             XSD: <xs:element name="starting_symmetry" maxOccurs="unbounded">
                             XSD: <xs:element name="software_list" type="software_list_type" minOccurs="0"/>
                             XSD: <xs:element name="details" type="xs:string" minOccurs="0"/>
                             """
 
                         refinement = emdb.refinement_type()
                         set_refinement_type()
-                        if refinement._hasContent():
+                        if refinement.has__content():
                             im_proc.set_refinement(refinement)
 
                     def set_el_startup_model(im_proc, ip_id_in, hel_dict_list):
                         """
                         XSD: <xs:element name="startup_model" type="starting_map_type" maxOccurs="unbounded" minOccurs="0">
                         """
                         st_mod_dict_in = hel_dict_list["st_mod_dict_in"]
@@ -9489,15 +9518,15 @@
                             XSD: <xs:element name="helix_length">
                             XSD: <xs:element name="straightening" type="xs:boolean" minOccurs="0"/>
                             XSD: <xs:element name="indexing">
                             """
 
                         lay_lines = emdb.layer_lines_type()
                         set_layer_lines_type()
-                        if lay_lines._hasContent():
+                        if lay_lines.has__content():
                             im_proc.set_helical_layer_lines(lay_lines)
 
                     def set_el_initial_angle_assignment():
                         """
                         XSD: <xs:element name="initial_angle_assignment" type="angle_assignment_type" minOccurs="0"/>
                         """
 
@@ -9638,15 +9667,15 @@
                             # element 2
                             set_el_resolution_range()
                             # element 3
                             set_el_software_list(mol_repl, cryst_dicts)
 
                         mol_repl = emdb.molecular_replacement_type()
                         set_molecular_replacement_type(mol_repl, cryst_dicts)
-                        if mol_repl._hasContent():
+                        if mol_repl.has__content():
                             im_proc.set_molecular_replacement(mol_repl)
 
                     def set_el_lat_dist_corr_soft_list(im_proc, cryst_dicts):
                         """
                         XSD: <xs:element name="lattice_distortion_correction_software_list" type="software_list_type" minOccurs="0"/>
                         """
                         set_software_list(const.LATTICE_DISTORTION_CORRECTION, cryst_dicts["cat_soft_dict_in"], im_proc.set_lattice_distortion_correction_software_list)
@@ -9896,17 +9925,17 @@
                                                 el_phase_residual,
                                                 el_fourier_space_coverage,
                                                 el_multiplicity,
                                             ]
                                             if any(x is not None for x in shell_type_list):
                                                 shell = emdb.shellType()
                                                 set_shell_type(shell, cs_in)
-                                                if shell._hasContent():
+                                                if shell.has__content():
                                                     cry_shell_list.add_shell(shell)
-                                        if cry_shell_list._hasContent():
+                                        if cry_shell_list.has__content():
                                             cry_stats.set_shell_list(cry_shell_list)
 
                             def set_el_details(cry_stats, cry_stats_in):
                                 """
                                 XSD: <xs:element name="details" type="xs:string" minOccurs="0"/>
                                 CIF: _em_diffraction_stats.details
                                 """
@@ -9936,15 +9965,15 @@
                             set_el_details(cry_stats, cry_stats_in)
 
                         cry_stats_dict_in = cryst_dicts["cry_stats_dict_in"]
                         if ip_id_in in cry_stats_dict_in:
                             cry_stats_in = cry_stats_dict_in[ip_id_in]
                             cry_stats = emdb.crystallography_statistics_type()
                             set_cryst_statistics_type(cry_stats, cry_stats_in)
-                            if cry_stats._hasContent():
+                            if cry_stats.has__content():
                                 im_proc.set_crystallography_statistics(cry_stats)
 
                     # element 1
                     set_el_final_reconstruction(im_proc, ip_id_in)
                     # element 2
                     set_el_crystal_parameters(im_proc, ip_id_in, cryst_dicts)
                     # element 3
@@ -10238,15 +10267,15 @@
                         Only space_group choice has mmCIF value
                         CIF: _em_map.symmetry_space_group 1
                         """
                         set_cif_value(app_sym.set_space_group, "symmetry_space_group", const.EM_MAP, cif_list=map_in, fmt=int)
 
                     app_sym = emdb.applied_symmetry_type()
                     set_applied_symmetry_type(app_sym)
-                    if app_sym._hasContent():
+                    if app_sym.has__content():
                         em_map.set_symmetry(app_sym)
 
                 def set_el_data_type(em_map, map_in):
                     """
                     XSD: <xs:element name="data_type" type="map_data_type"/>
                     CIF: _em_map.data_type 'Image stored as signed byte'
                     """
@@ -10289,15 +10318,15 @@
                         # element 2
                         set_el_row(dim, map_in)
                         # element 3
                         set_el_sec(dim, map_in)
 
                     dim = emdb.integer_vector_map_type()
                     set_integer_vector_map_type(dim, map_in)
-                    if dim._hasContent():
+                    if dim.has__content():
                         em_map.set_dimensions(dim)
 
                 def set_el_origin(em_map, map_in):
                     """
                     XSD: <xs:element name="origin">
                     """
 
@@ -10674,17 +10703,17 @@
                         set_el_contour_level(cntr, map_in)
                         # element 2
                         set_el_source(cntr, map_in)
 
                     cntr_list = emdb.contour_listType()
                     cntr = emdb.contourType()
                     set_contour_type(cntr, map_in)
-                    if cntr._hasContent():
+                    if cntr.has__content():
                         cntr_list.add_contour(cntr)
-                    if cntr_list._hasContent():
+                    if cntr_list.has__content():
                         em_map.set_contour_list(cntr_list)
 
                 def set_el_label(em_map, map_in):
                     """
                     XSD: <xs:element name="label" type="xs:token" minOccurs="0"/>
                     CIF: _em_map.label
                     """
@@ -10886,15 +10915,15 @@
                 len_pr_map_list_in = len(pr_map_list_in)
                 if len_pr_map_list_in != 1:
                     txt = u"There should be one and only one primary map. (%d) map(s) found." % len_pr_map_list_in
                     self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
                     self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
                 else:
                     em_map = make_map(pr_map_list_in[0], get_canonical_map_name(pr_map_list_in[0], "PRIMARY"))
-                    if em_map._hasContent():
+                    if em_map.has__content():
                         self.xml_out.set_map(em_map)
                     else:
                         txt = u"No information given for the primary map."
                         self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
                         self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
 
             def set_el_interpretation():
@@ -10936,19 +10965,26 @@
                                         XSD: <xs:element name="access_code">
                                         CIF: _em_3d_fitting_list.pdb_entry_id  1EHZ
                                         CIF: _em_3d_fitting_list.entry_id  1EHZ
                                         pattern "d[dA-Za-z]{3}"
                                         """
                                         accession_code = get_cif_value("accession_code", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                         access_code = get_cif_value("pdb_entry_id", const.EM_3D_FITTING_LIST, cif_list=model_in)
+                                        pdb_pattern = re.compile(r"\d[\dA-Za-z]{3}|pdb_\d{5}[\dA-Za-z]{3}")
+                                        if access_code is not None:
+                                            if not pdb_pattern.match(str(access_code)):
+                                                txt = u"(%s) PDB id is not in the correct format" % access_code
+                                                self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
+                                                self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
                                         if accession_code is None and access_code is not None:
                                             set_cif_value(model.set_access_code, "pdb_entry_id", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                         if accession_code is not None and access_code is None:
                                             set_cif_value(model.set_access_code, "accession_code", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                         if accession_code is not None and access_code is not None:
+                                            set_cif_value(model.set_access_code, "pdb_entry_id", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                             if accession_code != access_code:
                                                 txt = u"Cannot be two access_codes. If both pdb_entry_id and accession_code are populated, then both should be same."
                                                 self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
                                                 self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
 
                                     def set_el_chain(model, model_in):
                                         """
@@ -10973,14 +11009,17 @@
                                                 for a_id in ids:
                                                     set_cif_value(chain.set_chain_id, "pdb_chain_id", const.EM_3D_FITTING_LIST, cif_list=model_in, cif_value=a_id)
                                             if ids_in is None and ch_ids is not None:
                                                 c_ids = ch_ids.split(",")
                                                 for b_id in c_ids:
                                                     set_cif_value(chain.set_chain_id, "chain_id", const.EM_3D_FITTING_LIST, cif_list=model_in, cif_value=b_id)
                                             if ids_in is not None and ch_ids is not None:
+                                                ids = ids_in.split(",")
+                                                for a_id in ids:
+                                                    set_cif_value(chain.set_chain_id, "pdb_chain_id", const.EM_3D_FITTING_LIST, cif_list=model_in, cif_value=a_id)
                                                 if ids_in != ch_ids:
                                                     txt = u"Cannot be two chain_ids. If both pdb_chain_id and chain_id are populated, then both should be same."
                                                     self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
                                                     self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
 
                                         def set_el_residue_range(chain, model_in):
                                             """
@@ -10990,14 +11029,15 @@
                                             p_res_range = get_cif_value("pdb_chain_residue_range", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                             res_range = get_cif_value("chain_residue_range", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                             if p_res_range is not None and res_range is None:
                                                 set_cif_value(chain.set_residue_range, "pdb_chain_residue_range", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                             if p_res_range is None and res_range is not None:
                                                 set_cif_value(chain.set_residue_range, "chain_residue_range", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                             if p_res_range is not None and res_range is not None:
+                                                set_cif_value(chain.set_residue_range, "pdb_chain_residue_range", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                                 if p_res_range != res_range:
                                                     txt = u"Cannot be two chain_residue_range. If both pdb_chain_residue_range and chain_residue_range are populated, then both should be same."
                                                     self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
                                                     self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
 
                                         def set_el_numofcps_in_final_model(chain, model_in):
                                             """
@@ -11008,17 +11048,18 @@
 
                                         def set_el_source_name(chain, model_in):
                                             """
                                             XSD: <xs:element name="source_name" type="xs:string"  minOccurs="0" maxOccurs="1">
                                             CIF: _em_3d_fitting_list.source_name SwissModel
                                             """
                                             access_code = get_cif_value("pdb_entry_id", const.EM_3D_FITTING_LIST, cif_list=model_in)
+                                            accession_code = get_cif_value("accession_code", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                             sourcename = get_cif_value("source_name", const.EM_3D_FITTING_LIST, cif_list=model_in)
                                             set_cif_value(chain.set_source_name, "source_name", const.EM_3D_FITTING_LIST, cif_list=model_in)
-                                            if sourcename == "PDB" and access_code is None:
+                                            if sourcename == "PDB" and access_code is None and accession_code is None:
                                                 txt = u"Error! Missing PDB ID. If initial model is from PDB, then access code is mandatory."
                                                 self.current_entry_log.error_logs.append(self.ALog(log_text="(" + self.entry_in_translation_log.id + ")" + self.current_entry_log.error_title + txt))
                                                 self.log_formatted(self.error_log_string, const.REQUIRED_ALERT + txt)
 
                                         def set_el_initial_model_type(chain, model_in):
                                             """
                                             XSD: <xs:element name="initial_model_type" type="xs:string"  minOccurs="0" maxOccurs="1">
@@ -11028,15 +11069,15 @@
                                         # element 2
                                         chain = emdb.chainType()
                                         set_el_id(chain, model_in)
                                         set_el_residue_range(chain, model_in)
                                         set_el_numofcps_in_final_model(chain, model_in)
                                         set_el_source_name(chain, model_in)
                                         set_el_initial_model_type(chain, model_in)
-                                        if chain._hasContent():
+                                        if chain.has__content():
                                             model.set_chain(chain)
 
                                     def set_el_details(model, model_in):
                                         """
                                         XSD: <xs:element name="details" type="xs:string" minOccurs="0"/>
                                         CIF: _em_3d_fitting_list.details
                                         """
@@ -11047,15 +11088,15 @@
                                     set_el_chain(model, model_in)
                                     # element 3
                                     set_el_details(model, model_in)
                                 if modelling_id_in in model_dict_in:
                                     for model_in in model_dict_in[modelling_id_in]:
                                         model = emdb.initial_modelType()
                                         set_initial_model_type(model, model_in)
-                                        if model._hasContent():
+                                        if model.has__content():
                                             modelling.add_initial_model(model)
 
                             def set_el_final_model():
                                 """
                                 XSD: <xs:element name="final_model" minOccurs="0"> has
                                 .. 3 elements
                                 CIF: there is no _emd_modelling_final_model !!!
@@ -11131,17 +11172,17 @@
                         modelling_list = emdb.modelling_listType()
                         modelling_list_in = self.cif.get(const.EM_3D_FITTING)
                         model_dict_in = make_list_of_dicts(const.EM_3D_FITTING_LIST, const.K_3D_FITTING_ID)
                         for modelling_in in modelling_list_in:
                             modelling_id_in = get_cif_value(const.K_ID, const.EM_3D_FITTING, modelling_in)
                             modelling = emdb.modelling_type()
                             set_modelling_type(modelling, modelling_in, cat_soft_dict_in)
-                            if modelling._hasContent():
+                            if modelling.has__content():
                                 modelling_list.add_modelling(modelling)
-                        if modelling_list._hasContent():
+                        if modelling_list.has__content():
                             intrp.set_modelling_list(modelling_list)
 
                     def set_el_figure_list():
                         """
                         XSD: <xs:element name="figure_list" minOccurs="0">
                         CIF: ??
                         """
@@ -11185,19 +11226,19 @@
                             # element 3
                             set_el_mask_details()
 
                         mask_list_in = map_dict_in[const.MAP_MASK] if const.MAP_MASK in map_dict_in else []
                         seg_list = emdb.segmentation_listType()
                         for msk_in in mask_list_in:
                             msk = make_map(msk_in, get_canonical_map_name(msk_in, "MASK"))
-                            if msk._hasContent():
+                            if msk.has__content():
                                 seg = emdb.segmentationType()
                                 set_segmentation_type(seg, msk)
                                 seg_list.add_segmentation(seg)
-                        if seg_list._hasContent():
+                        if seg_list.has__content():
                             intrp.set_segmentation_list(seg_list)
 
                     def set_el_slices_list():
                         """
                         XSD: <xs:element name="slices_list" minOccurs="0">
                         CIF: Deprecated (2014-10-21)
                         """
@@ -11206,30 +11247,30 @@
                         """
                         XSD: <xs:element name="additional_map_list" minOccurs="0">
                         """
                         add_map_list_in = map_dict_in[const.MAP_ADD] if const.MAP_ADD in map_dict_in else []
                         add_map_list = emdb.additional_map_listType()
                         for add_map_in in add_map_list_in:
                             add_map = make_map(add_map_in, get_canonical_map_name(add_map_in, "ADDMAP"))
-                            if add_map._hasContent():
+                            if add_map.has__content():
                                 add_map_list.add_additional_map(add_map)
-                        if add_map_list._hasContent():
+                        if add_map_list.has__content():
                             intrp.set_additional_map_list(add_map_list)
 
                     def set_el_half_map_list(intrp, map_dict_in):
                         """
                         XSD: <xs:element name="half_map_list" minOccurs="0">
                         """
                         hf_map_list_in = map_dict_in[const.MAP_HALF] if const.MAP_HALF in map_dict_in else []
                         hf_map_list = emdb.half_map_listType()
                         for hf_map_in in hf_map_list_in:
                             hf_map = make_map(hf_map_in, get_canonical_map_name(hf_map_in, "HALFMAP"))
-                            if hf_map._hasContent():
+                            if hf_map.has__content():
                                 hf_map_list.add_half_map(hf_map)
-                        if hf_map_list._hasContent():
+                        if hf_map_list.has__content():
                             intrp.set_half_map_list(hf_map_list)
 
                     # element 1
                     set_el_modelling_list(intrp)
                     # element 2
                     set_el_figure_list()
                     # element 3
@@ -11240,15 +11281,15 @@
                     set_el_additional_map_list(intrp, map_dict_in)
                     # element 6
                     set_el_half_map_list(intrp, map_dict_in)
 
                 map_dict_in = make_list_of_dicts(const.EM_MAP, "type")
                 intrp = emdb.interpretation_type()
                 set_interpretation_type(intrp, map_dict_in)
-                if intrp._hasContent():
+                if intrp.has__content():
                     self.xml_out.set_interpretation(intrp)
 
             def set_el_validation():
                 """
                 XSD: <xs:element name="validation" minOccurs="0">
                 There should be 4 validation methods:
                 1. crystallography validation
@@ -11285,17 +11326,17 @@
 
                 validation = emdb.validationType()
                 fsc_list_in = self.cif.get(const.EM_FSC_CURVE, None)
                 for fsc_in in fsc_list_in:
                     fsc = emdb.fsc_curve_validation_type()
                     fsc.original_tagname_ = "fsc_curve"
                     set_fsc_curve(fsc, fsc_in)
-                    if fsc._hasContent():
+                    if fsc.has__content():
                         validation.add_validation_method(fsc)
-                if validation._hasContent():
+                if validation.has__content():
                     self.xml_out.set_validation(validation)
 
             # attribute 1
             set_attr_emdb_id()
             # attribute 2
             set_attr_version()
             # element 1
```

### Comparing `wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py` & `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/emdb.py` & `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/emdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 #
-# Generated Wed May  3 14:40:38 2023 by generateDS.py version 2.41.4.
+# Generated Wed May 24 20:24:21 2023 by generateDS.py version 2.41.5.
 # Python 3.9.5 (default, May 18 2021, 12:31:01)  [Clang 10.0.0 ]
 #
 # Command line options:
 #   ('--root-element', 'emd')
 #   ('-f', '')
-#   ('-o', 'emdb-schemas/emdb_schemas/v3/v3_0_3_3/emdb.py')
+#   ('-o', 'emdb-schemas/emdb_schemas/v3/v3_0_4_1/emdb.py')
 #   ('--no-warnings', '')
 #   ('--external-encoding', 'utf-8')
 #
 # Command line arguments:
-#   emdb-schemas/emdb_schemas/v3/v3_0_3_3/emdb.xsd
+#   emdb-schemas/emdb_schemas/v3/v3_0_4_1/emdb.xsd
 #
 # Command line:
-#   /Users/amudha/project/generateDS-2.41.4/generateDS.py --root-element="emd" -f -o "emdb-schemas/emdb_schemas/v3/v3_0_3_3/emdb.py" --no-warnings --external-encoding="utf-8" emdb-schemas/emdb_schemas/v3/v3_0_3_3/emdb.xsd
+#   /Users/amudha/project/generateDS-2.41.5/generateDS.py --root-element="emd" -f -o "emdb-schemas/emdb_schemas/v3/v3_0_4_1/emdb.py" --no-warnings --external-encoding="utf-8" emdb-schemas/emdb_schemas/v3/v3_0_4_1/emdb.xsd
 #
 # Current working directory (os.getcwd()):
 #   IdeaProjects
 #
 
 import sys
 try:
@@ -1145,14 +1145,37 @@
     CCD='CCD'
     CMOS='CMOS'
     DIRECTELECTRONDETECTOR='DIRECT ELECTRON DETECTOR'
     STORAGEPHOSPORIMAGEPLATES='STORAGE PHOSPOR (IMAGE PLATES)'
     FILM='FILM'
 
 
+class categoryType44(str, Enum):
+    CLASSIFICATION='CLASSIFICATION'
+    CRYSTALLOGRAPHYMERGING='CRYSTALLOGRAPHY MERGING'
+    CTFCORRECTION='CTF CORRECTION'
+    DIFFRACTIONINDEXING='DIFFRACTION INDEXING'
+    EWALDSPHERECORRECTION='EWALD SPHERE CORRECTION'
+    FINALEULERASSIGNMENT='FINAL EULER ASSIGNMENT'
+    IMAGEACQUISITION='IMAGE ACQUISITION'
+    INITIALEULERASSIGNMENT='INITIAL EULER ASSIGNMENT'
+    LATTICEDISTORTIONCORRECTION='LATTICE DISTORTION CORRECTION'
+    LAYERLINEINDEXING='LAYERLINE INDEXING'
+    MASKING='MASKING'
+    MODELFITTING='MODEL FITTING'
+    MODELREFINEMENT='MODEL REFINEMENT'
+    MOLECULARREPLACEMENT='MOLECULAR REPLACEMENT'
+    OTHER='OTHER'
+    PARTICLESELECTION='PARTICLE SELECTION'
+    RECONSTRUCTION='RECONSTRUCTION'
+    SERIESALIGNMENT='SERIES ALIGNMENT'
+    SYMMETRYDETERMINATION='SYMMETRY DETERMINATION'
+    VOLUMESELECTION='VOLUME SELECTION'
+
+
 class classificationType(str, Enum):
     DNA='DNA'
 
 
 class classificationType32(str, Enum):
     MESSENGER='MESSENGER'
     TRANSFER='TRANSFER'
@@ -1676,15 +1699,15 @@
     ISSN='ISSN'
     CAS='CAS'
     CSD='CSD'
     MEDLINE='MEDLINE'
     ASTM='ASTM'
 
 
-class typeType56(str, Enum):
+class typeType57(str, Enum):
     ANGULARRECONSTITUTION='ANGULAR RECONSTITUTION'
     COMMONLINE='COMMON LINE'
     NOTAPPLICABLE='NOT APPLICABLE'
     OTHER='OTHER'
     PROJECTIONMATCHING='PROJECTION MATCHING'
     RANDOMASSIGNMENT='RANDOM ASSIGNMENT'
     MAXIMUMLIKELIHOOD='MAXIMUM LIKELIHOOD'
@@ -1718,30 +1741,30 @@
 
 class unitsType40(str, Enum):
     MINUTE='MINUTE'
     HOUR='HOUR'
     DAY='DAY'
 
 
-class unitsType47(str, Enum):
+class unitsType48(str, Enum):
     PIXEL='PIXEL'
     Å='Å'
 
 
-class unitsType49(str, Enum):
+class unitsType50(str, Enum):
     PIXEL='PIXEL'
     Å='Å'
 
 
-class unitsType51(str, Enum):
+class unitsType52(str, Enum):
     PIXEL='PIXEL'
     Å='Å'
 
 
-class unitsType52(str, Enum):
+class unitsType53(str, Enum):
     PIXEL='PIXEL'
     Å='Å'
 
 
 class virus_isolateType(str, Enum):
     OTHER='OTHER'
     SEROCOMPLEX='SEROCOMPLEX'
@@ -1759,15 +1782,15 @@
     VIRUSLIKEPARTICLE='VIRUS-LIKE PARTICLE'
 
 
 class entry_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, emdb_id=None, version='3.0.3.3', admin=None, crossreferences=None, sample=None, structure_determination_list=None, map=None, interpretation=None, validation=None, gds_collector_=None, **kwargs_):
+    def __init__(self, emdb_id=None, version='3.0.4.2', admin=None, crossreferences=None, sample=None, structure_determination_list=None, map=None, interpretation=None, validation=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.emdb_id = _cast(None, emdb_id)
         self.emdb_id_nsprefix_ = None
@@ -1845,15 +1868,15 @@
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_emdb_id_type_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_emdb_id_type_patterns_, ))
     validate_emdb_id_type_patterns_ = [['^(EMD-\\d{4,})$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.admin is not None or
             self.crossreferences is not None or
             self.sample is not None or
             self.structure_determination_list is not None or
             self.map is not None or
             self.interpretation is not None or
@@ -1874,26 +1897,26 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='entry_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='entry_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='entry_type'):
         if self.emdb_id is not None and 'emdb_id' not in already_processed:
             already_processed.add('emdb_id')
             outfile.write(' emdb_id=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.emdb_id), input_name='emdb_id')), ))
-        if self.version != "3.0.3.3" and 'version' not in already_processed:
+        if self.version != "3.0.4.2" and 'version' not in already_processed:
             already_processed.add('version')
             outfile.write(' version=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.version), input_name='version')), ))
     def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='entry_type', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
@@ -2094,15 +2117,15 @@
         return self.keywords
     def set_keywords(self, keywords):
         self.keywords = keywords
     def get_replace_existing_entry(self):
         return self.replace_existing_entry
     def set_replace_existing_entry(self, replace_existing_entry):
         self.replace_existing_entry = replace_existing_entry
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.status_history_list is not None or
             self.current_status is not None or
             self.sites is not None or
             self.key_dates is not None or
             self.obsolete_list is not None or
             self.superseded_by_list is not None or
@@ -2130,15 +2153,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='admin_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='admin_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='admin_type'):
@@ -2330,15 +2353,15 @@
         self.status = status
     def add_status(self, value):
         self.status.append(value)
     def insert_status_at(self, index, value):
         self.status.insert(index, value)
     def replace_status_at(self, index, value):
         self.status[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.status
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='version_list_type', pretty_print=True):
@@ -2353,15 +2376,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='version_list_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='version_list_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='version_list_type'):
@@ -2483,15 +2506,15 @@
             value = value
             enumerations = ['PDBe', 'RCSB', 'PDBj', 'PDBc']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on processing_siteType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.date is not None or
             self.code is not None or
             self.processing_site is not None or
             self.annotator is not None or
             self.details is not None
         ):
@@ -2510,15 +2533,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='version_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='version_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='version_type'):
@@ -2660,15 +2683,15 @@
             value = value
             enumerations = ['AUCO', 'AUTH', 'AUXS', 'AUXU', 'HOLD', 'HOLD8W', 'HPUB', 'OBS', 'POLC', 'PROC', 'REFI', 'REL', 'REPL', 'REUP', 'WAIT', 'WDRN']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on status_code_type' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='code_type', pretty_print=True):
@@ -2794,15 +2817,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_emdb_id_type_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_emdb_id_type_patterns_, ))
                 result = False
         return result
     validate_emdb_id_type_patterns_ = [['^(EMD-\\d{4,})$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.date is not None or
             self.entry is not None or
             self.details is not None
         ):
             return True
         else:
@@ -2819,15 +2842,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='supersedes_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='supersedes_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='supersedes_type'):
@@ -2928,15 +2951,15 @@
         return self.code
     def set_code(self, code):
         self.code = code
     def get_country(self):
         return self.country
     def set_country(self, country):
         self.country = country
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.funding_body is not None or
             self.code is not None or
             self.country is not None
         ):
             return True
         else:
@@ -2953,15 +2976,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='grant_reference_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='grant_reference_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='grant_reference_type'):
@@ -3200,15 +3223,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_emailType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_emailType_patterns_, ))
                 result = False
         return result
     validate_emailType_patterns_ = [['^([A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\\.[A-Za-z]{2,4})$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.role is not None or
             self.title is not None or
             self.first_name is not None or
             self.middle_name is not None or
             self.last_name is not None or
             self.organization is not None or
@@ -3236,15 +3259,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='contact_details_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='contact_details_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='contact_details_type'):
@@ -3548,15 +3571,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_localType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_localType_patterns_, ))
                 result = False
         return result
     validate_localType_patterns_ = [['^(\\d+( ext. \\d+)?)$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.country is not None or
             self.area is not None or
             self.local is not None
         ):
             return True
         else:
@@ -3573,15 +3596,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='telephone_number_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='telephone_number_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='telephone_number_type'):
@@ -3705,15 +3728,15 @@
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_ORCID_type_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_ORCID_type_patterns_, ))
     validate_ORCID_type_patterns_ = [['^([0-9]{4}-[0-9]{4}-[0-9]{4}-([0-9]{3}X|[0-9]{4}))$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='author_ORCID_type', pretty_print=True):
@@ -3809,18 +3832,18 @@
         self.ns_prefix_ = ns_prefix
     def get_order(self):
         return self.order
     def set_order(self, order):
         self.order = order
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_) or
-            super(author_order_type, self)._hasContent()
+            super(author_order_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='author_order_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('author_order_type')
         if imported_ns_def_ is not None:
@@ -3919,15 +3942,15 @@
         return self.pdb_list
     def set_pdb_list(self, pdb_list):
         self.pdb_list = pdb_list
     def get_auxiliary_link_list(self):
         return self.auxiliary_link_list
     def set_auxiliary_link_list(self, auxiliary_link_list):
         self.auxiliary_link_list = auxiliary_link_list
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.citation_list is not None or
             self.emdb_list is not None or
             self.pdb_list is not None or
             self.auxiliary_link_list is not None
         ):
             return True
@@ -3945,15 +3968,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='crossreferences_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='crossreferences_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='crossreferences_type'):
@@ -4033,15 +4056,15 @@
         else:
             return citation_type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='citation_type', pretty_print=True):
@@ -4056,15 +4079,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='citation_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='citation_type', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='citation_type'):
         pass
@@ -4233,15 +4256,15 @@
         # Validate type yearType, a restriction on xs:gYear.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if value < '1900':
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on yearType' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.author or
             self.title is not None or
             self.journal is not None or
             self.journal_abbreviation is not None or
             self.country is not None or
             self.issue is not None or
@@ -4268,15 +4291,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='journal_citation')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='journal_citation', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='journal_citation'):
@@ -4623,15 +4646,15 @@
         # Validate type yearType3, a restriction on xs:gYear.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if value < '1900':
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on yearType3' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.author or
             self.editor or
             self.title is not None or
             self.thesis_title is not None or
             self.chapter_title is not None or
             self.volume is not None or
@@ -4659,15 +4682,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='non_journal_citation')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='non_journal_citation', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='non_journal_citation'):
@@ -4900,15 +4923,15 @@
         self.emdb_reference = emdb_reference
     def add_emdb_reference(self, value):
         self.emdb_reference.append(value)
     def insert_emdb_reference_at(self, index, value):
         self.emdb_reference.insert(index, value)
     def replace_emdb_reference_at(self, index, value):
         self.emdb_reference[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.emdb_reference
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='emdb_cross_reference_list_type', pretty_print=True):
@@ -4923,15 +4946,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='emdb_cross_reference_list_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='emdb_cross_reference_list_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='emdb_cross_reference_list_type'):
@@ -5020,15 +5043,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_emdb_id_type_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_emdb_id_type_patterns_, ))
                 result = False
         return result
     validate_emdb_id_type_patterns_ = [['^(EMD-\\d{4,})$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.emdb_id is not None or
             self.relationship is not None or
             self.details is not None
         ):
             return True
         else:
@@ -5045,15 +5068,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='emdb_cross_reference_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='emdb_cross_reference_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='emdb_cross_reference_type'):
@@ -5150,15 +5173,15 @@
         self.pdb_reference = pdb_reference
     def add_pdb_reference(self, value):
         self.pdb_reference.append(value)
     def insert_pdb_reference_at(self, index, value):
         self.pdb_reference.insert(index, value)
     def replace_pdb_reference_at(self, index, value):
         self.pdb_reference[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.pdb_reference
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='pdb_cross_reference_list_type', pretty_print=True):
@@ -5173,15 +5196,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='pdb_cross_reference_list_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='pdb_cross_reference_list_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='pdb_cross_reference_list_type'):
@@ -5269,16 +5292,16 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_pdb_code_type_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_pdb_code_type_patterns_, ))
                 result = False
         return result
-    validate_pdb_code_type_patterns_ = [['^(\\d[\\dA-Za-z]{3})$']]
-    def _hasContent(self):
+    validate_pdb_code_type_patterns_ = [['^(\\d[\\dA-Za-z]{3}|pdb_\\d{5}[\\dA-Za-z]{3})$']]
+    def has__content(self):
         if (
             self.pdb_id is not None or
             self.relationship is not None or
             self.details is not None
         ):
             return True
         else:
@@ -5295,15 +5318,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='pdb_cross_reference_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='pdb_cross_reference_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='pdb_cross_reference_type'):
@@ -5434,15 +5457,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_linkType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_linkType_patterns_, ))
                 result = False
         return result
     validate_linkType_patterns_ = [['^((https?|ftp)://.*)$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.type_ is not None or
             self.link is not None or
             self.details is not None
         ):
             return True
         else:
@@ -5459,15 +5482,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='auxiliary_link_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='auxiliary_link_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='auxiliary_link_type'):
@@ -5571,15 +5594,15 @@
         return self.supramolecule_list
     def set_supramolecule_list(self, supramolecule_list):
         self.supramolecule_list = supramolecule_list
     def get_macromolecule_list(self):
         return self.macromolecule_list
     def set_macromolecule_list(self, macromolecule_list):
         self.macromolecule_list = macromolecule_list
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.name is not None or
             self.supramolecule_list is not None or
             self.macromolecule_list is not None
         ):
             return True
         else:
@@ -5596,15 +5619,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='sample_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='sample_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='sample_type'):
@@ -5685,15 +5708,15 @@
         self.ns_prefix_ = ns_prefix
     def get_synonym(self):
         return self.synonym
     def set_synonym(self, synonym):
         self.synonym = synonym
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='sci_name_type', pretty_print=True):
@@ -5845,15 +5868,15 @@
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
     def validate_pos_int_or_string_type(self, value):
         result = True
         # Validate type pos_int_or_string_type, a restriction on None.
         pass
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.name is not None or
             self.category is not None or
             self.parent is not None or
             self.macromolecule_list is not None or
             self.details is not None or
             self.number_of_copies is not None or
@@ -5876,15 +5899,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='base_supramolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='base_supramolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='base_supramolecule_type'):
@@ -6070,19 +6093,19 @@
         self.synthetic_source = synthetic_source
     def add_synthetic_source(self, value):
         self.synthetic_source.append(value)
     def insert_synthetic_source_at(self, index, value):
         self.synthetic_source.insert(index, value)
     def replace_synthetic_source_at(self, index, value):
         self.synthetic_source[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.natural_source or
             self.synthetic_source or
-            super(cell_supramolecule_type, self)._hasContent()
+            super(cell_supramolecule_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='cell_supramolecule_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('cell_supramolecule_type')
         if imported_ns_def_ is not None:
@@ -6095,15 +6118,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='cell_supramolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='cell_supramolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='cell_supramolecule_type'):
@@ -6209,15 +6232,15 @@
                 return False
             value = value
             enumerations = ['NCBI']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on databaseType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.organism is not None or
             self.strain is not None or
             self.synonym_organism is not None
         ):
             return True
         else:
@@ -6234,15 +6257,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='base_source_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='base_source_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='base_source_type'):
@@ -6354,15 +6377,15 @@
         self.ns_prefix_ = ns_prefix
     def get_ncbi(self):
         return self.ncbi
     def set_ncbi(self, ncbi):
         self.ncbi = ncbi
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='organism_type', pretty_print=True):
@@ -6500,22 +6523,22 @@
         return self.ribosome_details
     def set_ribosome_details(self, ribosome_details):
         self.ribosome_details = ribosome_details
     def get_chimera(self):
         return self.chimera
     def set_chimera(self, chimera):
         self.chimera = chimera
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.natural_source or
             self.synthetic_source or
             self.recombinant_expression or
             self.molecular_weight is not None or
             self.ribosome_details is not None or
-            super(complex_supramolecule_type, self)._hasContent()
+            super(complex_supramolecule_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='complex_supramolecule_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('complex_supramolecule_type')
         if imported_ns_def_ is not None:
@@ -6528,15 +6551,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='complex_supramolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='complex_supramolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='complex_supramolecule_type'):
@@ -6671,22 +6694,22 @@
         return self.organelle
     def set_organelle(self, organelle):
         self.organelle = organelle
     def get_cellular_location(self):
         return self.cellular_location
     def set_cellular_location(self, cellular_location):
         self.cellular_location = cellular_location
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.organ is not None or
             self.tissue is not None or
             self.cell is not None or
             self.organelle is not None or
             self.cellular_location is not None or
-            super(complex_source_type, self)._hasContent()
+            super(complex_source_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='complex_source_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('complex_source_type')
         if imported_ns_def_ is not None:
@@ -6699,15 +6722,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='complex_source_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='complex_source_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='complex_source_type'):
@@ -6876,15 +6899,15 @@
                 return False
             value = value
             enumerations = ['NCBI']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on databaseType12' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.recombinant_organism is not None or
             self.recombinant_strain is not None or
             self.recombinant_cell is not None or
             self.recombinant_plasmid is not None or
             self.recombinant_synonym_organism is not None
         ):
@@ -6903,15 +6926,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='recombinant_source_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='recombinant_source_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='recombinant_source_type'):
@@ -7048,15 +7071,15 @@
         return self.theoretical
     def set_theoretical(self, theoretical):
         self.theoretical = theoretical
     def get_method(self):
         return self.method
     def set_method(self, method):
         self.method = method
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.experimental is not None or
             self.theoretical is not None or
             self.method is not None
         ):
             return True
         else:
@@ -7073,15 +7096,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='molecular_weight_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='molecular_weight_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='molecular_weight_type'):
@@ -7202,21 +7225,21 @@
         return self.molecular_weight
     def set_molecular_weight(self, molecular_weight):
         self.molecular_weight = molecular_weight
     def get_recombinant_expression(self):
         return self.recombinant_expression
     def set_recombinant_expression(self, recombinant_expression):
         self.recombinant_expression = recombinant_expression
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.natural_source or
             self.synthetic_source or
             self.molecular_weight is not None or
             self.recombinant_expression is not None or
-            super(organelle_or_cellular_component_supramolecule_type, self)._hasContent()
+            super(organelle_or_cellular_component_supramolecule_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='organelle_or_cellular_component_supramolecule_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('organelle_or_cellular_component_supramolecule_type')
         if imported_ns_def_ is not None:
@@ -7229,15 +7252,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='organelle_or_cellular_component_supramolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='organelle_or_cellular_component_supramolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='organelle_or_cellular_component_supramolecule_type'):
@@ -7350,22 +7373,22 @@
         return self.organelle
     def set_organelle(self, organelle):
         self.organelle = organelle
     def get_cellular_location(self):
         return self.cellular_location
     def set_cellular_location(self, cellular_location):
         self.cellular_location = cellular_location
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.organ is not None or
             self.tissue is not None or
             self.cell is not None or
             self.organelle is not None or
             self.cellular_location is not None or
-            super(organelle_source_type, self)._hasContent()
+            super(organelle_source_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='organelle_source_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('organelle_source_type')
         if imported_ns_def_ is not None:
@@ -7378,15 +7401,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='organelle_source_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='organelle_source_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='organelle_source_type'):
@@ -7549,21 +7572,21 @@
         return self.number_unique_components
     def set_number_unique_components(self, number_unique_components):
         self.number_unique_components = number_unique_components
     def get_molecular_weight(self):
         return self.molecular_weight
     def set_molecular_weight(self, molecular_weight):
         self.molecular_weight = molecular_weight
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.natural_source or
             self.synthetic_source or
             self.number_unique_components is not None or
             self.molecular_weight is not None or
-            super(sample_supramolecule_type, self)._hasContent()
+            super(sample_supramolecule_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='sample_supramolecule_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('sample_supramolecule_type')
         if imported_ns_def_ is not None:
@@ -7576,15 +7599,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='sample_supramolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='sample_supramolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='sample_supramolecule_type'):
@@ -7689,20 +7712,20 @@
         return self.tissue
     def set_tissue(self, tissue):
         self.tissue = tissue
     def get_cell(self):
         return self.cell
     def set_cell(self, cell):
         self.cell = cell
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.organ is not None or
             self.tissue is not None or
             self.cell is not None or
-            super(sample_source_type, self)._hasContent()
+            super(sample_source_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='sample_source_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('sample_source_type')
         if imported_ns_def_ is not None:
@@ -7715,15 +7738,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='sample_source_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='sample_source_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='sample_source_type'):
@@ -7846,19 +7869,19 @@
         self.sythetic_source = sythetic_source
     def add_sythetic_source(self, value):
         self.sythetic_source.append(value)
     def insert_sythetic_source_at(self, index, value):
         self.sythetic_source.insert(index, value)
     def replace_sythetic_source_at(self, index, value):
         self.sythetic_source[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.natural_source or
             self.sythetic_source or
-            super(tissue_supramolecule_type, self)._hasContent()
+            super(tissue_supramolecule_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='tissue_supramolecule_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('tissue_supramolecule_type')
         if imported_ns_def_ is not None:
@@ -7871,15 +7894,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='tissue_supramolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='tissue_supramolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='tissue_supramolecule_type'):
@@ -7958,19 +7981,19 @@
         return self.organ
     def set_organ(self, organ):
         self.organ = organ
     def get_tissue(self):
         return self.tissue
     def set_tissue(self, tissue):
         self.tissue = tissue
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.organ is not None or
             self.tissue is not None or
-            super(tissue_source_type, self)._hasContent()
+            super(tissue_source_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='tissue_source_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('tissue_source_type')
         if imported_ns_def_ is not None:
@@ -7983,15 +8006,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='tissue_source_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='tissue_source_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='tissue_source_type'):
@@ -8219,15 +8242,15 @@
             value = value
             enumerations = ['OTHER', 'SEROCOMPLEX', 'SEROTYPE', 'SPECIES', 'STRAIN', 'SUBSPECIES']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on virus_isolateType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.sci_species_name is not None or
             self.sci_species_strain is not None or
             self.natural_host or
             self.synthetic_host or
             self.host_system is not None or
             self.molecular_weight is not None or
@@ -8236,15 +8259,15 @@
             self.virus_isolate is not None or
             self.virus_enveloped is not None or
             self.virus_empty is not None or
             self.syn_species_name is not None or
             self.sci_species_serotype is not None or
             self.sci_species_serocomplex is not None or
             self.sci_species_subspecies is not None or
-            super(virus_supramolecule_type, self)._hasContent()
+            super(virus_supramolecule_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='virus_supramolecule_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('virus_supramolecule_type')
         if imported_ns_def_ is not None:
@@ -8257,15 +8280,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='virus_supramolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='virus_supramolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='virus_supramolecule_type'):
@@ -8474,15 +8497,15 @@
         self.ns_prefix_ = ns_prefix
     def get_ncbi(self):
         return self.ncbi
     def set_ncbi(self, ncbi):
         self.ncbi = ncbi
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='virus_species_name_type', pretty_print=True):
@@ -8557,17 +8580,17 @@
         else:
             return virus_host_type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
-            super(virus_host_type, self)._hasContent()
+            super(virus_host_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='virus_host_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('virus_host_type')
         if imported_ns_def_ is not None:
@@ -8580,15 +8603,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='virus_host_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='virus_host_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='virus_host_type'):
@@ -8650,15 +8673,15 @@
         self.macromolecule = macromolecule
     def add_macromolecule(self, value):
         self.macromolecule.append(value)
     def insert_macromolecule_at(self, index, value):
         self.macromolecule.insert(index, value)
     def replace_macromolecule_at(self, index, value):
         self.macromolecule[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.macromolecule
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='macromolecule_list_type', pretty_print=True):
@@ -8673,15 +8696,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='macromolecule_list_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='macromolecule_list_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='macromolecule_list_type'):
@@ -8842,15 +8865,15 @@
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
     def validate_pos_int_or_string_type(self, value):
         result = True
         # Validate type pos_int_or_string_type, a restriction on None.
         pass
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.name is not None or
             self.natural_source is not None or
             self.molecular_weight is not None or
             self.details is not None or
             self.number_of_copies is not None or
             self.oligomeric_state is not None or
@@ -8871,15 +8894,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='base_macromolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='base_macromolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='base_macromolecule_type'):
@@ -9069,22 +9092,22 @@
         return self.organelle
     def set_organelle(self, organelle):
         self.organelle = organelle
     def get_cellular_location(self):
         return self.cellular_location
     def set_cellular_location(self, cellular_location):
         self.cellular_location = cellular_location
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.organ is not None or
             self.tissue is not None or
             self.cell is not None or
             self.organelle is not None or
             self.cellular_location is not None or
-            super(macromolecule_source_type, self)._hasContent()
+            super(macromolecule_source_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='macromolecule_source_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('macromolecule_source_type')
         if imported_ns_def_ is not None:
@@ -9097,15 +9120,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='macromolecule_source_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='macromolecule_source_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='macromolecule_source_type'):
@@ -9272,22 +9295,22 @@
             value = value
             enumerations = ['DNA']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on classificationType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.sequence is not None or
             self.classification is not None or
             self.structure is not None or
             self.synthetic_flag is not None or
             self.synthetic_source is not None or
-            super(dna_macromolecule_type, self)._hasContent()
+            super(dna_macromolecule_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='dna_macromolecule_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('dna_macromolecule_type')
         if imported_ns_def_ is not None:
@@ -9300,15 +9323,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='dna_macromolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='dna_macromolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='dna_macromolecule_type'):
@@ -9438,19 +9461,19 @@
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             pass
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.formula is not None or
             self.synthetic_source is not None or
-            super(em_label_macromolecule_type, self)._hasContent()
+            super(em_label_macromolecule_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='em_label_macromolecule_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('em_label_macromolecule_type')
         if imported_ns_def_ is not None:
@@ -9463,15 +9486,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='em_label_macromolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='em_label_macromolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='em_label_macromolecule_type'):
@@ -9584,20 +9607,20 @@
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             pass
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.formula is not None or
             self.external_references or
             self.recombinant_expression is not None or
-            super(ligand_macromolecule_type, self)._hasContent()
+            super(ligand_macromolecule_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='ligand_macromolecule_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('ligand_macromolecule_type')
         if imported_ns_def_ is not None:
@@ -9610,15 +9633,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ligand_macromolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ligand_macromolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ligand_macromolecule_type'):
@@ -9737,23 +9760,23 @@
         return self.synthetic_flag
     def set_synthetic_flag(self, synthetic_flag):
         self.synthetic_flag = synthetic_flag
     def get_synthetic_source(self):
         return self.synthetic_source
     def set_synthetic_source(self, synthetic_source):
         self.synthetic_source = synthetic_source
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.sequence is not None or
             self.classification is not None or
             self.recombinant_expression is not None or
             self.structure is not None or
             self.synthetic_flag is not None or
             self.synthetic_source is not None or
-            super(other_macromolecule_type, self)._hasContent()
+            super(other_macromolecule_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='other_macromolecule_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('other_macromolecule_type')
         if imported_ns_def_ is not None:
@@ -9766,15 +9789,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='other_macromolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='other_macromolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='other_macromolecule_type'):
@@ -9956,22 +9979,22 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_ec_numberType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_ec_numberType_patterns_, ))
                 result = False
         return result
     validate_ec_numberType_patterns_ = [['^(([1-7]((.[1-9][0-9]?)|(.-))((.[1-9][0-9]?)|(.-))((.[1-9][0-9]?[0-9]?)|(.-)))(([ ]*,[ ]*)([1-6]((.[1-9][0-9]?)|(.-))((.[1-9][0-9]?)|(.-))((.[1-9][0-9]?[0-9]?)|(.-))))*)$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.recombinant_expression is not None or
             self.synthetic_source is not None or
             self.enantiomer is not None or
             self.sequence is not None or
             self.ec_number or
-            super(protein_or_peptide_macromolecule_type, self)._hasContent()
+            super(protein_or_peptide_macromolecule_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='protein_or_peptide_macromolecule_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('protein_or_peptide_macromolecule_type')
         if imported_ns_def_ is not None:
@@ -9984,15 +10007,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='protein_or_peptide_macromolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='protein_or_peptide_macromolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='protein_or_peptide_macromolecule_type'):
@@ -10174,23 +10197,23 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_ec_numberType33_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_ec_numberType33_patterns_, ))
                 result = False
         return result
     validate_ec_numberType33_patterns_ = [['^(\\d+(\\.(\\d+|\\-)){3})$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.sequence is not None or
             self.classification is not None or
             self.structure is not None or
             self.synthetic_flag is not None or
             self.synthetic_source is not None or
             self.ec_number or
-            super(rna_macromolecule_type, self)._hasContent()
+            super(rna_macromolecule_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='rna_macromolecule_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('rna_macromolecule_type')
         if imported_ns_def_ is not None:
@@ -10203,15 +10226,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='rna_macromolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='rna_macromolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='rna_macromolecule_type'):
@@ -10388,20 +10411,20 @@
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             pass
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.enantiomer is not None or
             self.formula is not None or
             self.external_references or
-            super(saccharide_macromolecule_type, self)._hasContent()
+            super(saccharide_macromolecule_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='saccharide_macromolecule_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('saccharide_macromolecule_type')
         if imported_ns_def_ is not None:
@@ -10414,15 +10437,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='saccharide_macromolecule_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='saccharide_macromolecule_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='saccharide_macromolecule_type'):
@@ -10595,15 +10618,15 @@
             value = value
             enumerations = ['particle', 'filament', 'twoDArray', 'threeDArray', 'helicalArray', 'cell', 'tissue']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on aggregation_stateType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.method is not None or
             self.aggregation_state is not None or
             self.macromolecules_and_complexes is not None or
             self.specimen_preparation_list is not None or
             self.microscopy_list is not None or
             self.image_processing
@@ -10623,15 +10646,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='structure_determination_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='structure_determination_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='structure_determination_type'):
@@ -10805,15 +10828,15 @@
         self.complex_id = complex_id
     def add_complex_id(self, value):
         self.complex_id.append(value)
     def insert_complex_id_at(self, index, value):
         self.complex_id.insert(index, value)
     def replace_complex_id_at(self, index, value):
         self.complex_id[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.macromolecule_id or
             self.complex_id
         ):
             return True
         else:
             return False
@@ -10829,15 +10852,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='macromolecules_and_complexes_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='macromolecules_and_complexes_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='macromolecules_and_complexes_type'):
@@ -10966,15 +10989,15 @@
         self.details = details
     def get_preparation_id(self):
         return self.preparation_id
     def set_preparation_id(self, preparation_id):
         self.preparation_id = preparation_id
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.concentration is not None or
             self.buffer is not None or
             self.staining is not None or
             self.sugar_embedding is not None or
             self.shadowing is not None or
             self.grid is not None or
@@ -10996,15 +11019,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='base_preparation_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='base_preparation_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='base_preparation_type'):
@@ -11182,15 +11205,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on phType' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 14:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on phType' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ph is not None or
             self.component or
             self.details is not None
         ):
             return True
         else:
@@ -11207,15 +11230,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='buffer_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='buffer_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='buffer_type'):
@@ -11322,15 +11345,15 @@
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             pass
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.concentration is not None or
             self.formula is not None or
             self.name is not None
         ):
             return True
         else:
@@ -11347,15 +11370,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='buffer_component_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='buffer_component_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='buffer_component_type'):
@@ -11502,15 +11525,15 @@
             value = value
             enumerations = ['COPPER', 'COPPER/PALLADIUM', 'COPPER/RHODIUM', 'GOLD', 'GRAPHENE OXIDE', 'MOLYBDENUM', 'NICKEL', 'NICKEL/TITANIUM', 'PLATINUM', 'SILICON NITRIDE', 'TITANIUM', 'TUNGSTEN']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on materialType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.model is not None or
             self.material is not None or
             self.mesh is not None or
             self.support_film or
             self.pretreatment is not None or
             self.details is not None
@@ -11530,15 +11553,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='grid_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='grid_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='grid_type'):
@@ -11710,15 +11733,15 @@
             value = value
             enumerations = ['CONTINUOUS', 'HOLEY', 'HOLEY ARRAY', 'LACEY']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on film_topologyType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.film_material is not None or
             self.film_topology is not None or
             self.film_thickness is not None
         ):
             return True
         else:
@@ -11735,15 +11758,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='film_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='film_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='film_type'):
@@ -11878,15 +11901,15 @@
             value = value
             enumerations = ['AIR', 'AMYLAMINE', 'NITROGEN', 'OTHER']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on atmosphereType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.type_ is not None or
             self.time is not None or
             self.atmosphere is not None or
             self.pressure is not None
         ):
             return True
@@ -11904,15 +11927,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='grid_pretreatment_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='grid_pretreatment_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='grid_pretreatment_type'):
@@ -12080,15 +12103,15 @@
             value = value
             enumerations = ['EMS-002 RAPID IMMERSION FREEZER', 'FEI VITROBOT MARK I', 'FEI VITROBOT MARK II', 'FEI VITROBOT MARK III', 'FEI VITROBOT MARK IV', 'GATAN CRYOPLUNGE 3', 'HOMEMADE PLUNGER', 'LEICA EM CPC', 'LEICA EM GP', 'LEICA KF80', 'LEICA PLUNGER', 'REICHERT-JUNG PLUNGER', 'SPOTITON', 'OTHER']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on instrumentType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.cryogen_name is not None or
             self.chamber_humidity is not None or
             self.chamber_temperature is not None or
             self.instrument is not None or
             self.details is not None or
             self.timed_resolved_state is not None or
@@ -12109,15 +12132,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='vitrification_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='vitrification_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='vitrification_type'):
@@ -12254,18 +12277,18 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_crystal_formation(self):
         return self.crystal_formation
     def set_crystal_formation(self, crystal_formation):
         self.crystal_formation = crystal_formation
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.crystal_formation is not None or
-            super(crystallography_preparation_type, self)._hasContent()
+            super(crystallography_preparation_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='crystallography_preparation_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('crystallography_preparation_type')
         if imported_ns_def_ is not None:
@@ -12278,15 +12301,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='crystallography_preparation_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='crystallography_preparation_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='crystallography_preparation_type'):
@@ -12370,15 +12393,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_crystal_formation_temperature_type' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 343:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_crystal_formation_temperature_type' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='crystal_formation_temperature_type', pretty_print=True):
@@ -12486,15 +12509,15 @@
                 return False
             value = value
             enumerations = ['MINUTE', 'HOUR', 'DAY']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType40' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='crystal_formation_time_type', pretty_print=True):
@@ -12569,17 +12592,17 @@
         else:
             return helical_preparation_type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
-            super(helical_preparation_type, self)._hasContent()
+            super(helical_preparation_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='helical_preparation_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('helical_preparation_type')
         if imported_ns_def_ is not None:
@@ -12592,15 +12615,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='helical_preparation_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='helical_preparation_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='helical_preparation_type'):
@@ -12648,17 +12671,17 @@
         else:
             return single_particle_preparation_type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
-            super(single_particle_preparation_type, self)._hasContent()
+            super(single_particle_preparation_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='single_particle_preparation_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('single_particle_preparation_type')
         if imported_ns_def_ is not None:
@@ -12671,15 +12694,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='single_particle_preparation_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='single_particle_preparation_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='single_particle_preparation_type'):
@@ -12727,17 +12750,17 @@
         else:
             return subtomogram_averaging_preparation_type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
-            super(subtomogram_averaging_preparation_type, self)._hasContent()
+            super(subtomogram_averaging_preparation_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='subtomogram_averaging_preparation_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('subtomogram_averaging_preparation_type')
         if imported_ns_def_ is not None:
@@ -12750,15 +12773,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='subtomogram_averaging_preparation_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='subtomogram_averaging_preparation_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='subtomogram_averaging_preparation_type'):
@@ -12836,22 +12859,22 @@
         return self.cryo_protectant
     def set_cryo_protectant(self, cryo_protectant):
         self.cryo_protectant = cryo_protectant
     def get_sectioning(self):
         return self.sectioning
     def set_sectioning(self, sectioning):
         self.sectioning = sectioning
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.fiducial_markers_list is not None or
             self.high_pressure_freezing is not None or
             self.embedding_material is not None or
             self.cryo_protectant is not None or
             self.sectioning is not None or
-            super(tomography_preparation_type, self)._hasContent()
+            super(tomography_preparation_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='tomography_preparation_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('tomography_preparation_type')
         if imported_ns_def_ is not None:
@@ -12864,15 +12887,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='tomography_preparation_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='tomography_preparation_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='tomography_preparation_type'):
@@ -12992,15 +13015,15 @@
         return self.manufacturer
     def set_manufacturer(self, manufacturer):
         self.manufacturer = manufacturer
     def get_diameter(self):
         return self.diameter
     def set_diameter(self, diameter):
         self.diameter = diameter
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.fiducial_type is not None or
             self.manufacturer is not None or
             self.diameter is not None
         ):
             return True
         else:
@@ -13017,15 +13040,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='fiducial_marker_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='fiducial_marker_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='fiducial_marker_type'):
@@ -13135,15 +13158,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_diameter_colloidal_gold' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 100:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_diameter_colloidal_gold' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='fiducial_marker_diameter_type', pretty_print=True):
@@ -13242,15 +13265,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_temperature' % {"value": value, "lineno": lineno} )
                 result = False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_temperature' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='temperature_type', pretty_print=True):
@@ -13345,15 +13368,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value < 4:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_microtome_thickness' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='ultramicrotomy_final_thickness_type', pretty_print=True):
@@ -13452,15 +13475,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_focus_ion_voltage' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 50:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_focus_ion_voltage' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='fib_voltage_type', pretty_print=True):
@@ -13558,15 +13581,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_focus_ion_current' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 200:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_focus_ion_current' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='fib_current_type', pretty_print=True):
@@ -13660,15 +13683,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_focus_ion_dose_rate' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='fib_dose_rate_type', pretty_print=True):
@@ -13750,15 +13773,15 @@
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='fib_duration_type', pretty_print=True):
@@ -13857,15 +13880,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_focus_ion_initial_thickness' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 100000:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_focus_ion_initial_thickness' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='fib_initial_thickness_type', pretty_print=True):
@@ -13960,15 +13983,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value < 10:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_focus_ion_final_thickness' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='fib_final_thickness_type', pretty_print=True):
@@ -14325,15 +14348,15 @@
             value = value
             enumerations = ['HELIUM', 'NITROGEN']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on cooling_holder_cryogenType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.specimen_preparations is not None or
             self.microscope is not None or
             self.illumination_mode is not None or
             self.imaging_mode is not None or
             self.electron_source is not None or
             self.acceleration_voltage is not None or
@@ -14373,15 +14396,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='base_microscopy_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='base_microscopy_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='base_microscopy_type'):
@@ -14730,15 +14753,15 @@
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='residual_tilt_type', pretty_print=True):
@@ -14857,15 +14880,15 @@
             value = value
             enumerations = ['ZERNIKE PHASE PLATE', 'VOLTA PHASE PLATE', 'OTHER']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on phase_plateType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.phase_plate is not None or
             self.sph_aberration_corrector is not None or
             self.chr_aberration_corrector is not None or
             self.energy_filter is not None or
             self.details is not None
         ):
@@ -14884,15 +14907,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='specialist_optics_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='specialist_optics_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='specialist_optics_type'):
@@ -15017,15 +15040,15 @@
         self.software = software
     def add_software(self, value):
         self.software.append(value)
     def insert_software_at(self, index, value):
         self.software.insert(index, value)
     def replace_software_at(self, index, value):
         self.software[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.software
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='software_list_type', pretty_print=True):
@@ -15040,15 +15063,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='software_list_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='software_list_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='software_list_type'):
@@ -15083,24 +15106,27 @@
 # end class software_list_type
 
 
 class software_type(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
-    def __init__(self, name=None, version=None, processing_details=None, gds_collector_=None, **kwargs_):
+    def __init__(self, name=None, version=None, category=None, processing_details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.name = name
         self.name_nsprefix_ = None
         self.version = version
         self.version_nsprefix_ = None
+        self.category = category
+        self.validate_categoryType44(self.category)
+        self.category_nsprefix_ = None
         self.processing_details = processing_details
         self.processing_details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
                 CurrentSubclassModule_, software_type)
             if subclass is not None:
@@ -15118,22 +15144,42 @@
         return self.name
     def set_name(self, name):
         self.name = name
     def get_version(self):
         return self.version
     def set_version(self, version):
         self.version = version
+    def get_category(self):
+        return self.category
+    def set_category(self, category):
+        self.category = category
     def get_processing_details(self):
         return self.processing_details
     def set_processing_details(self, processing_details):
         self.processing_details = processing_details
-    def _hasContent(self):
+    def validate_categoryType44(self, value):
+        result = True
+        # Validate type categoryType44, a restriction on xs:token.
+        if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
+            if not isinstance(value, str):
+                lineno = self.gds_get_node_lineno_()
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
+                return False
+            value = value
+            enumerations = ['CLASSIFICATION', 'CRYSTALLOGRAPHY MERGING', 'CTF CORRECTION', 'DIFFRACTION INDEXING', 'EWALD SPHERE CORRECTION', 'FINAL EULER ASSIGNMENT', 'IMAGE ACQUISITION', 'INITIAL EULER ASSIGNMENT', 'LATTICE DISTORTION CORRECTION', 'LAYERLINE INDEXING', 'MASKING', 'MODEL FITTING', 'MODEL REFINEMENT', 'MOLECULAR REPLACEMENT', 'OTHER', 'PARTICLE SELECTION', 'RECONSTRUCTION', 'SERIES ALIGNMENT', 'SYMMETRY DETERMINATION', 'VOLUME SELECTION']
+            if value not in enumerations:
+                lineno = self.gds_get_node_lineno_()
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on categoryType44' % {"value" : encode_str_2_3(value), "lineno": lineno} )
+                result = False
+        return result
+    def has__content(self):
         if (
             self.name is not None or
             self.version is not None or
+            self.category is not None or
             self.processing_details is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='software_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('software_type')
@@ -15147,15 +15193,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='software_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='software_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='software_type'):
@@ -15169,14 +15215,18 @@
             namespaceprefix_ = self.name_nsprefix_ + ':' if (UseCapturedNS_ and self.name_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sname>%s</%sname>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.name), input_name='name')), namespaceprefix_ , eol_))
         if self.version is not None:
             namespaceprefix_ = self.version_nsprefix_ + ':' if (UseCapturedNS_ and self.version_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sversion>%s</%sversion>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.version), input_name='version')), namespaceprefix_ , eol_))
+        if self.category is not None:
+            namespaceprefix_ = self.category_nsprefix_ + ':' if (UseCapturedNS_ and self.category_nsprefix_) else ''
+            showIndent(outfile, level, pretty_print)
+            outfile.write('<%scategory>%s</%scategory>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.category), input_name='category')), namespaceprefix_ , eol_))
         if self.processing_details is not None:
             namespaceprefix_ = self.processing_details_nsprefix_ + ':' if (UseCapturedNS_ and self.processing_details_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
             outfile.write('<%sprocessing_details>%s</%sprocessing_details>%s' % (namespaceprefix_ , self.gds_encode(self.gds_format_string(quote_xml(self.processing_details), input_name='processing_details')), namespaceprefix_ , eol_))
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
@@ -15207,14 +15257,26 @@
                 value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'version')
             value_ = self.gds_validate_string(value_, node, 'version')
             self.version = value_
             self.version_nsprefix_ = child_.prefix
+        elif nodeName_ == 'category':
+            value_ = child_.text
+            if value_:
+                value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
+            else:
+                value_ = ""
+            value_ = self.gds_parse_string(value_, node, 'category')
+            value_ = self.gds_validate_string(value_, node, 'category')
+            self.category = value_
+            self.category_nsprefix_ = child_.prefix
+            # validate type categoryType44
+            self.validate_categoryType44(self.category)
         elif nodeName_ == 'processing_details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'processing_details')
             value_ = self.gds_validate_string(value_, node, 'processing_details')
             self.processing_details = value_
             self.processing_details_nsprefix_ = child_.prefix
 # end class software_type
@@ -15269,20 +15331,20 @@
         self.tilt_series = tilt_series
     def add_tilt_series(self, value):
         self.tilt_series.append(value)
     def insert_tilt_series_at(self, index, value):
         self.tilt_series.insert(index, value)
     def replace_tilt_series_at(self, index, value):
         self.tilt_series[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.camera_length is not None or
             self.tilt_list is not None or
             self.tilt_series or
-            super(crystallography_microscopy_type, self)._hasContent()
+            super(crystallography_microscopy_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='crystallography_microscopy_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('crystallography_microscopy_type')
         if imported_ns_def_ is not None:
@@ -15295,15 +15357,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='crystallography_microscopy_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='crystallography_microscopy_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='crystallography_microscopy_type'):
@@ -15395,15 +15457,15 @@
         return self.axis2
     def set_axis2(self, axis2):
         self.axis2 = axis2
     def get_axis_rotation(self):
         return self.axis_rotation
     def set_axis_rotation(self, axis_rotation):
         self.axis_rotation = axis_rotation
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.axis1 is not None or
             self.axis2 is not None or
             self.axis_rotation is not None
         ):
             return True
         else:
@@ -15420,15 +15482,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='tilt_series_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='tilt_series_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='tilt_series_type'):
@@ -15522,15 +15584,15 @@
         self.max_angle = max_angle
     def get_angle_increment(self):
         return self.angle_increment
     def set_angle_increment(self, angle_increment):
         self.angle_increment = angle_increment
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.min_angle is not None or
             self.max_angle is not None or
             self.angle_increment is not None
         ):
             return True
         else:
@@ -15547,15 +15609,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='axis_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='axis_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='axis_type'):
@@ -15639,17 +15701,17 @@
         else:
             return helical_microscopy_type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
-            super(helical_microscopy_type, self)._hasContent()
+            super(helical_microscopy_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='helical_microscopy_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('helical_microscopy_type')
         if imported_ns_def_ is not None:
@@ -15662,15 +15724,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='helical_microscopy_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='helical_microscopy_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='helical_microscopy_type'):
@@ -15718,17 +15780,17 @@
         else:
             return single_particle_microscopy_type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
-            super(single_particle_microscopy_type, self)._hasContent()
+            super(single_particle_microscopy_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='single_particle_microscopy_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('single_particle_microscopy_type')
         if imported_ns_def_ is not None:
@@ -15741,15 +15803,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='single_particle_microscopy_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='single_particle_microscopy_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='single_particle_microscopy_type'):
@@ -15812,18 +15874,18 @@
         self.tilt_series = tilt_series
     def add_tilt_series(self, value):
         self.tilt_series.append(value)
     def insert_tilt_series_at(self, index, value):
         self.tilt_series.insert(index, value)
     def replace_tilt_series_at(self, index, value):
         self.tilt_series[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.tilt_series or
-            super(tomography_microscopy_type, self)._hasContent()
+            super(tomography_microscopy_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='tomography_microscopy_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('tomography_microscopy_type')
         if imported_ns_def_ is not None:
@@ -15836,15 +15898,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='tomography_microscopy_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='tomography_microscopy_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='tomography_microscopy_type'):
@@ -15923,15 +15985,15 @@
         self.details = details
     def get_image_processing_id(self):
         return self.image_processing_id
     def set_image_processing_id(self, image_processing_id):
         self.image_processing_id = image_processing_id
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.image_recording_id is not None or
             self.details is not None
         ):
             return True
         else:
             return False
@@ -15947,15 +16009,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='base_image_processing_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='base_image_processing_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='base_image_processing_type'):
@@ -16112,26 +16174,26 @@
         return self.merging_software_list
     def set_merging_software_list(self, merging_software_list):
         self.merging_software_list = merging_software_list
     def get_crystallography_statistics(self):
         return self.crystallography_statistics
     def set_crystallography_statistics(self, crystallography_statistics):
         self.crystallography_statistics = crystallography_statistics
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.final_reconstruction is not None or
             self.crystal_parameters is not None or
             self.startup_model or
             self.ctf_correction is not None or
             self.molecular_replacement is not None or
             self.lattice_distortion_correction_software_list is not None or
             self.symmetry_determination_software_list is not None or
             self.merging_software_list is not None or
             self.crystallography_statistics is not None or
-            super(crystallography_processing_type, self)._hasContent()
+            super(crystallography_processing_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='crystallography_processing_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('crystallography_processing_type')
         if imported_ns_def_ is not None:
@@ -16144,15 +16206,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='crystallography_processing_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='crystallography_processing_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='crystallography_processing_type'):
@@ -16307,15 +16369,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_point_groupType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_point_groupType_patterns_, ))
                 result = False
         return result
     validate_point_groupType_patterns_ = [['^(C\\d+|D\\d+|O|T|I)$'], ['^(C\\d+|D\\d+|O|T|I)$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.space_group is not None or
             self.point_group is not None or
             self.helical_parameters is not None
         ):
             return True
         else:
@@ -16332,15 +16394,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='applied_symmetry_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='applied_symmetry_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='applied_symmetry_type'):
@@ -16455,15 +16517,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_axial_symmetryType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_axial_symmetryType_patterns_, ))
                 result = False
         return result
     validate_axial_symmetryType_patterns_ = [['^([C|D][1-9][0-9]*)$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.delta_z is not None or
             self.delta_phi is not None or
             self.axial_symmetry is not None
         ):
             return True
         else:
@@ -16480,15 +16542,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='helical_parameters_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='helical_parameters_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='helical_parameters_type'):
@@ -16598,15 +16660,15 @@
         return self.b_factorSharpening
     def set_b_factorSharpening(self, b_factorSharpening):
         self.b_factorSharpening = b_factorSharpening
     def get_other(self):
         return self.other
     def set_other(self, other):
         self.other = other
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.background_masked is not None or
             self.spatial_filtering is not None or
             self.sharpening is not None or
             self.b_factorSharpening is not None or
             self.other is not None
         ):
@@ -16625,15 +16687,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='reconstruction_filtering_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='reconstruction_filtering_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='reconstruction_filtering_type'):
@@ -16689,15 +16751,15 @@
             obj_.original_tagname_ = 'sharpening'
         elif nodeName_ == 'b-factorSharpening':
             obj_ = b_factorSharpeningType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.b_factorSharpening = obj_
             obj_.original_tagname_ = 'b-factorSharpening'
         elif nodeName_ == 'other':
-            obj_ = otherType45.factory(parent_object_=self)
+            obj_ = otherType46.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.other = obj_
             obj_.original_tagname_ = 'other'
 # end class reconstruction_filtering_type
 
 
 class background_masked_type(GeneratedsSuper):
@@ -16761,15 +16823,15 @@
             value = value
             enumerations = ['SPHERE', 'SOFT SPHERE', 'GAUSSIAN', 'CIRCLE', 'RECTANGLE', 'CYLINDER', 'OTHER']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on geometrical_shapeType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.geometrical_shape is not None or
             self.dimensions is not None or
             self.software_list is not None or
             self.details is not None
         ):
             return True
@@ -16787,15 +16849,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='background_masked_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='background_masked_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='background_masked_type'):
@@ -16842,15 +16904,15 @@
             value_ = self.gds_parse_string(value_, node, 'geometrical_shape')
             value_ = self.gds_validate_string(value_, node, 'geometrical_shape')
             self.geometrical_shape = value_
             self.geometrical_shape_nsprefix_ = child_.prefix
             # validate type geometrical_shapeType
             self.validate_geometrical_shapeType(self.geometrical_shape)
         elif nodeName_ == 'dimensions':
-            obj_ = dimensionsType46.factory(parent_object_=self)
+            obj_ = dimensionsType47.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.dimensions = obj_
             obj_.original_tagname_ = 'dimensions'
         elif nodeName_ == 'software_list':
             obj_ = software_list_type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.software_list = obj_
@@ -16919,15 +16981,15 @@
             value = value
             enumerations = ['C 1 2', 'C 2 2 2', 'P 1', 'P 1 2', 'P 1 21', 'P 2', 'P 2 2 2', 'P 2 2 21', 'P 2 21 21', 'P 3', 'P 3 1 2', 'P 3 2 1', 'P 4', 'P 4 2 2', 'P 4 21 2', 'P 6', 'P 6 2 2']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on plane_groupType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.unit_cell is not None or
             self.plane_group is not None or
             self.space_group is not None
         ):
             return True
         else:
@@ -16944,15 +17006,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='crystal_parameters_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='crystal_parameters_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='crystal_parameters_type'):
@@ -17080,15 +17142,15 @@
         return self.alpha
     def set_alpha(self, alpha):
         self.alpha = alpha
     def get_beta(self):
         return self.beta
     def set_beta(self, beta):
         self.beta = beta
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.a is not None or
             self.b is not None or
             self.c is not None or
             self.c_sampling_length is not None or
             self.gamma is not None or
             self.alpha is not None or
@@ -17109,15 +17171,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='unit_cell_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='unit_cell_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='unit_cell_type'):
@@ -17243,15 +17305,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0.0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_cell_dim' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='cell_type', pretty_print=True):
@@ -17350,15 +17412,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_cell_angle' % {"value": value, "lineno": lineno} )
                 result = False
             if value >= 180.0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxExclusive restriction on allowed_cell_angle' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='cell_angle_type', pretty_print=True):
@@ -17494,15 +17556,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_emdb_id_type_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_emdb_id_type_patterns_, ))
                 result = False
         return result
     validate_emdb_id_type_patterns_ = [['^(EMD-\\d{4,})$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.random_conical_tilt is not None or
             self.orthogonal_tilt is not None or
             self.emdb_id is not None or
             self.pdb_model is not None or
             self.insilico_model is not None or
             self.other is not None or
@@ -17523,15 +17585,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='starting_map_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='starting_map_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='starting_map_type'):
@@ -17685,16 +17747,16 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_pdb_code_type_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_pdb_code_type_patterns_, ))
                 result = False
         return result
-    validate_pdb_code_type_patterns_ = [['^(\\d[\\dA-Za-z]{3})$']]
-    def _hasContent(self):
+    validate_pdb_code_type_patterns_ = [['^(\\d[\\dA-Za-z]{3}|pdb_\\d{5}[\\dA-Za-z]{3})$']]
+    def has__content(self):
         if (
             self.pdb_id is not None or
             self.chain_id_list is not None
         ):
             return True
         else:
             return False
@@ -17710,15 +17772,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='pdb_model_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='pdb_model_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='pdb_model_type'):
@@ -17840,15 +17902,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_residue_rangeType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_residue_rangeType_patterns_, ))
                 result = False
         return result
     validate_residue_rangeType_patterns_ = [['^(\\d+-\\d+)$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.chain_id or
             self.residue_range is not None
         ):
             return True
         else:
             return False
@@ -17864,15 +17926,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='chain_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='chain_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='chain_type'):
@@ -17998,15 +18060,15 @@
             value = value
             enumerations = ['MULTIPLICATION', 'DIVISION']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on correction_operationType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.phase_reversal is not None or
             self.amplitude_correction is not None or
             self.correction_operation is not None or
             self.software_list is not None or
             self.details is not None
         ):
@@ -18025,15 +18087,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ctf_correction_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ctf_correction_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ctf_correction_type'):
@@ -18154,15 +18216,15 @@
         return self.resolution_range
     def set_resolution_range(self, resolution_range):
         self.resolution_range = resolution_range
     def get_software_list(self):
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.starting_model or
             self.resolution_range is not None or
             self.software_list is not None
         ):
             return True
         else:
@@ -18179,15 +18241,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='molecular_replacement_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='molecular_replacement_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='molecular_replacement_type'):
@@ -18325,15 +18387,15 @@
         return self.shell_list
     def set_shell_list(self, shell_list):
         self.shell_list = shell_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_intensities_measured is not None or
             self.number_structure_factors is not None or
             self.fourier_space_coverage is not None or
             self.r_sym is not None or
             self.r_merge is not None or
             self.overall_phase_error is not None or
@@ -18358,15 +18420,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='crystallography_statistics_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='crystallography_statistics_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='crystallography_statistics_type'):
@@ -18489,15 +18551,15 @@
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'phase_error_rejection_criteria')
             value_ = self.gds_validate_string(value_, node, 'phase_error_rejection_criteria')
             self.phase_error_rejection_criteria = value_
             self.phase_error_rejection_criteria_nsprefix_ = child_.prefix
         elif nodeName_ == 'high_resolution':
-            obj_ = high_resolutionType53.factory(parent_object_=self)
+            obj_ = high_resolutionType54.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.high_resolution = obj_
             obj_.original_tagname_ = 'high_resolution'
         elif nodeName_ == 'shell_list':
             obj_ = shell_listType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.shell_list = obj_
@@ -18605,26 +18667,26 @@
         return self.final_angle_assignment
     def set_final_angle_assignment(self, final_angle_assignment):
         self.final_angle_assignment = final_angle_assignment
     def get_crystal_parameters(self):
         return self.crystal_parameters
     def set_crystal_parameters(self, crystal_parameters):
         self.crystal_parameters = crystal_parameters
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.final_reconstruction is not None or
             self.ctf_correction is not None or
             self.segment_selection or
             self.refinement is not None or
             self.startup_model or
             self.helical_layer_lines is not None or
             self.initial_angle_assignment is not None or
             self.final_angle_assignment is not None or
             self.crystal_parameters is not None or
-            super(helical_processing_type, self)._hasContent()
+            super(helical_processing_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='helical_processing_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('helical_processing_type')
         if imported_ns_def_ is not None:
@@ -18637,15 +18699,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='helical_processing_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='helical_processing_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='helical_processing_type'):
@@ -18803,15 +18865,15 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_selected is not None or
             self.segment_length is not None or
             self.segment_overlap is not None or
             self.total_filament_length is not None or
             self.software_list is not None or
             self.details is not None
@@ -18831,15 +18893,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='segment_selection_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='segment_selection_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='segment_selection_type'):
@@ -18983,15 +19045,15 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.startup_model or
             self.starting_symmetry or
             self.software_list is not None or
             self.details is not None
         ):
             return True
@@ -19009,15 +19071,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='refinement_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='refinement_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='refinement_type'):
@@ -19123,15 +19185,15 @@
         return self.straightening
     def set_straightening(self, straightening):
         self.straightening = straightening
     def get_indexing(self):
         return self.indexing
     def set_indexing(self, indexing):
         self.indexing = indexing
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_helices is not None or
             self.helix_length is not None or
             self.straightening is not None or
             self.indexing is not None
         ):
             return True
@@ -19149,15 +19211,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='layer_lines_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='layer_lines_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='layer_lines_type'):
@@ -19241,15 +19303,15 @@
         else:
             return number_helices(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='number_helices', pretty_print=True):
@@ -19264,15 +19326,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='number_helices')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='number_helices', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='number_helices'):
         pass
@@ -19303,15 +19365,15 @@
     def __init__(self, type_=None, projection_matching_processing=None, software_list=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.type_ = type_
-        self.validate_typeType56(self.type_)
+        self.validate_typeType57(self.type_)
         self.type__nsprefix_ = None
         self.projection_matching_processing = projection_matching_processing
         self.projection_matching_processing_nsprefix_ = None
         self.software_list = software_list
         self.software_list_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
@@ -19342,30 +19404,30 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def validate_typeType56(self, value):
+    def validate_typeType57(self, value):
         result = True
-        # Validate type typeType56, a restriction on xs:token.
+        # Validate type typeType57, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
             enumerations = ['ANGULAR RECONSTITUTION', 'COMMON LINE', 'NOT APPLICABLE', 'OTHER', 'PROJECTION MATCHING', 'RANDOM ASSIGNMENT', 'MAXIMUM LIKELIHOOD']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType56' % {"value" : encode_str_2_3(value), "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType57' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.type_ is not None or
             self.projection_matching_processing is not None or
             self.software_list is not None or
             self.details is not None
         ):
             return True
@@ -19383,15 +19445,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='angle_assignment_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='angle_assignment_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='angle_assignment_type'):
@@ -19435,16 +19497,16 @@
                 value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'type')
             value_ = self.gds_validate_string(value_, node, 'type')
             self.type_ = value_
             self.type_nsprefix_ = child_.prefix
-            # validate type typeType56
-            self.validate_typeType56(self.type_)
+            # validate type typeType57
+            self.validate_typeType57(self.type_)
         elif nodeName_ == 'projection_matching_processing':
             obj_ = projection_matching_processingType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.projection_matching_processing = obj_
             obj_.original_tagname_ = 'projection_matching_processing'
         elif nodeName_ == 'software_list':
             obj_ = software_list_type.factory(parent_object_=self)
@@ -19554,26 +19616,26 @@
         return self.final_two_d_classification
     def set_final_two_d_classification(self, final_two_d_classification):
         self.final_two_d_classification = final_two_d_classification
     def get_final_three_d_classification(self):
         return self.final_three_d_classification
     def set_final_three_d_classification(self, final_three_d_classification):
         self.final_three_d_classification = final_three_d_classification
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.particle_selection or
             self.ctf_correction is not None or
             self.startup_model or
             self.final_reconstruction is not None or
             self.initial_angle_assignment is not None or
             self.final_angle_assignment is not None or
             self.final_multi_reference_alignment is not None or
             self.final_two_d_classification is not None or
             self.final_three_d_classification is not None or
-            super(singleparticle_processing_type, self)._hasContent()
+            super(singleparticle_processing_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='singleparticle_processing_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('singleparticle_processing_type')
         if imported_ns_def_ is not None:
@@ -19586,15 +19648,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='singleparticle_processing_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='singleparticle_processing_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='singleparticle_processing_type'):
@@ -19746,15 +19808,15 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_selected is not None or
             self.reference_model is not None or
             self.method is not None or
             self.software_list is not None or
             self.details is not None
         ):
@@ -19773,15 +19835,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='particle_selection_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='particle_selection_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='particle_selection_type'):
@@ -19921,15 +19983,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on average_number_members_per_classType' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_classes is not None or
             self.average_number_members_per_class is not None or
             self.software_list is not None or
             self.details is not None
         ):
             return True
@@ -19947,15 +20009,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='classification_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='classification_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='classification_type'):
@@ -20088,24 +20150,24 @@
         return self.final_angle_assignment
     def set_final_angle_assignment(self, final_angle_assignment):
         self.final_angle_assignment = final_angle_assignment
     def get_crystal_parameters(self):
         return self.crystal_parameters
     def set_crystal_parameters(self, crystal_parameters):
         self.crystal_parameters = crystal_parameters
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.final_reconstruction is not None or
             self.extraction is not None or
             self.ctf_correction is not None or
             self.final_multi_reference_alignment is not None or
             self.final_three_d_classification is not None or
             self.final_angle_assignment is not None or
             self.crystal_parameters is not None or
-            super(subtomogram_averaging_processing_type, self)._hasContent()
+            super(subtomogram_averaging_processing_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='subtomogram_averaging_processing_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('subtomogram_averaging_processing_type')
         if imported_ns_def_ is not None:
@@ -20118,15 +20180,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='subtomogram_averaging_processing_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='subtomogram_averaging_processing_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='subtomogram_averaging_processing_type'):
@@ -20184,15 +20246,15 @@
             obj_.original_tagname_ = 'extraction'
         elif nodeName_ == 'ctf_correction':
             obj_ = ctf_correction_type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.ctf_correction = obj_
             obj_.original_tagname_ = 'ctf_correction'
         elif nodeName_ == 'final_multi_reference_alignment':
-            obj_ = final_multi_reference_alignmentType60.factory(parent_object_=self)
+            obj_ = final_multi_reference_alignmentType61.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.final_multi_reference_alignment = obj_
             obj_.original_tagname_ = 'final_multi_reference_alignment'
         elif nodeName_ == 'final_three_d_classification':
             obj_ = classification_type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.final_three_d_classification = obj_
@@ -20315,15 +20377,15 @@
             value = value
             enumerations = ['DIFFRACTION PATTERN/LAYERLINES', 'FSC 0.143 CUT-OFF', 'FSC 0.33 CUT-OFF', 'FSC 0.5 CUT-OFF', 'FSC 1/2 BIT CUT-OFF', 'FSC 3 SIGMA CUT-OFF', 'OTHER']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on resolution_methodType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_classes_used is not None or
             self.applied_symmetry is not None or
             self.algorithm is not None or
             self.resolution is not None or
             self.resolution_method is not None or
             self.reconstruction_filtering is not None or
@@ -20345,15 +20407,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_reconstruction_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_reconstruction_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_reconstruction_type'):
@@ -20523,21 +20585,21 @@
         return self.ctf_correction
     def set_ctf_correction(self, ctf_correction):
         self.ctf_correction = ctf_correction
     def get_crystal_parameters(self):
         return self.crystal_parameters
     def set_crystal_parameters(self, crystal_parameters):
         self.crystal_parameters = crystal_parameters
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.final_reconstruction is not None or
             self.series_aligment_software_list is not None or
             self.ctf_correction is not None or
             self.crystal_parameters is not None or
-            super(tomography_processing_type, self)._hasContent()
+            super(tomography_processing_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='tomography_processing_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('tomography_processing_type')
         if imported_ns_def_ is not None:
@@ -20550,15 +20612,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='tomography_processing_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='tomography_processing_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='tomography_processing_type'):
@@ -20767,15 +20829,15 @@
             value = value
             enumerations = ['IMAGE STORED AS SIGNED BYTE', 'IMAGE STORED AS SIGNED INTEGER (2 BYTES)', 'IMAGE STORED AS FLOATING POINT NUMBER (4 BYTES)']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on map_data_type' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.file is not None or
             self.symmetry is not None or
             self.data_type is not None or
             self.dimensions is not None or
             self.origin is not None or
             self.spacing is not None or
@@ -20803,15 +20865,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='map_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='map_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='map_type'):
@@ -21025,15 +21087,15 @@
         return self.row
     def set_row(self, row):
         self.row = row
     def get_sec(self):
         return self.sec
     def set_sec(self, sec):
         self.sec = sec
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.col is not None or
             self.row is not None or
             self.sec is not None
         ):
             return True
         else:
@@ -21050,15 +21112,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='integer_vector_map_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='integer_vector_map_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='integer_vector_map_type'):
@@ -21166,15 +21228,15 @@
         return self.average
     def set_average(self, average):
         self.average = average
     def get_std(self):
         return self.std
     def set_std(self, std):
         self.std = std
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.minimum is not None or
             self.maximum is not None or
             self.average is not None or
             self.std is not None
         ):
             return True
@@ -21192,15 +21254,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='map_statistics_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='map_statistics_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='map_statistics_type'):
@@ -21310,15 +21372,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_pixel_sampling' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='pixel_spacing_type', pretty_print=True):
@@ -21427,15 +21489,15 @@
         return self.additional_map_list
     def set_additional_map_list(self, additional_map_list):
         self.additional_map_list = additional_map_list
     def get_half_map_list(self):
         return self.half_map_list
     def set_half_map_list(self, half_map_list):
         self.half_map_list = half_map_list
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.modelling_list is not None or
             self.figure_list is not None or
             self.segmentation_list is not None or
             self.slices_list is not None or
             self.additional_map_list is not None or
             self.half_map_list is not None
@@ -21455,15 +21517,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='interpretation_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='interpretation_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='interpretation_type'):
@@ -21632,15 +21694,15 @@
             value = value
             enumerations = ['AB INITIO MODEL', 'BACKBONE TRACE', 'FLEXIBLE FIT', 'OTHER', 'RIGID BODY FIT']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on refinement_protocolType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.initial_model or
             self.final_model is not None or
             self.refinement_protocol is not None or
             self.software_list is not None or
             self.details is not None or
             self.target_criteria is not None or
@@ -21662,15 +21724,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='modelling_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='modelling_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='modelling_type'):
@@ -21788,15 +21850,15 @@
     def __init__(self, file=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.file = file
-        self.validate_fileType65(self.file)
+        self.validate_fileType66(self.file)
         self.file_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
                 CurrentSubclassModule_, figure_type)
@@ -21815,29 +21877,29 @@
         return self.file
     def set_file(self, file):
         self.file = file
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def validate_fileType65(self, value):
+    def validate_fileType66(self, value):
         result = True
-        # Validate type fileType65, a restriction on xs:token.
+        # Validate type fileType66, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
-                    self.validate_fileType65_patterns_, value):
-                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_fileType65_patterns_, ))
+                    self.validate_fileType66_patterns_, value):
+                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_fileType66_patterns_, ))
                 result = False
         return result
-    validate_fileType65_patterns_ = [['^(emd_\\d{4,}.+)$']]
-    def _hasContent(self):
+    validate_fileType66_patterns_ = [['^(emd_\\d{4,}.+)$']]
+    def has__content(self):
         if (
             self.file is not None or
             self.details is not None
         ):
             return True
         else:
             return False
@@ -21853,15 +21915,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='figure_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='figure_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='figure_type'):
@@ -21899,16 +21961,16 @@
                 value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'file')
             value_ = self.gds_validate_string(value_, node, 'file')
             self.file = value_
             self.file_nsprefix_ = child_.prefix
-            # validate type fileType65
-            self.validate_fileType65(self.file)
+            # validate type fileType66
+            self.validate_fileType66(self.file)
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
 # end class figure_type
@@ -21921,15 +21983,15 @@
     def __init__(self, file=None, details=None, extensiontype_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.file = file
-        self.validate_fileType66(self.file)
+        self.validate_fileType67(self.file)
         self.file_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
         self.extensiontype_ = extensiontype_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
@@ -21951,29 +22013,29 @@
         self.file = file
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
     def get_extensiontype_(self): return self.extensiontype_
     def set_extensiontype_(self, extensiontype_): self.extensiontype_ = extensiontype_
-    def validate_fileType66(self, value):
+    def validate_fileType67(self, value):
         result = True
-        # Validate type fileType66, a restriction on xs:token.
+        # Validate type fileType67, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
-                    self.validate_fileType66_patterns_, value):
-                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_fileType66_patterns_, ))
+                    self.validate_fileType67_patterns_, value):
+                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_fileType67_patterns_, ))
                 result = False
         return result
-    validate_fileType66_patterns_ = [['^(emd_\\d{4,}_fsc(_[1-9]{1,})*.xml)$']]
-    def _hasContent(self):
+    validate_fileType67_patterns_ = [['^(emd_\\d{4,}_fsc(_[1-9]{1,})*.xml)$']]
+    def has__content(self):
         if (
             self.file is not None or
             self.details is not None
         ):
             return True
         else:
             return False
@@ -21989,15 +22051,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='validation_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='validation_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='validation_type'):
@@ -22046,16 +22108,16 @@
                 value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'file')
             value_ = self.gds_validate_string(value_, node, 'file')
             self.file = value_
             self.file_nsprefix_ = child_.prefix
-            # validate type fileType66
-            self.validate_fileType66(self.file)
+            # validate type fileType67
+            self.validate_fileType67(self.file)
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
 # end class validation_type
@@ -22125,24 +22187,24 @@
         return self.weighted_r_factor
     def set_weighted_r_factor(self, weighted_r_factor):
         self.weighted_r_factor = weighted_r_factor
     def get_data_completeness(self):
         return self.data_completeness
     def set_data_completeness(self, data_completeness):
         self.data_completeness = data_completeness
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.parallel_resolution is not None or
             self.perpendicular_resolution is not None or
             self.number_observed_reflections is not None or
             self.number_unique_reflections is not None or
             self.weighted_phase_residual is not None or
             self.weighted_r_factor is not None or
             self.data_completeness is not None or
-            super(crystallography_validation_type, self)._hasContent()
+            super(crystallography_validation_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='crystallography_validation_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('crystallography_validation_type')
         if imported_ns_def_ is not None:
@@ -22155,15 +22217,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='crystallography_validation_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='crystallography_validation_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='crystallography_validation_type'):
@@ -22283,15 +22345,15 @@
         else:
             return parallel_resolution(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='parallel_resolution', pretty_print=True):
@@ -22306,15 +22368,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='parallel_resolution')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='parallel_resolution', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='parallel_resolution'):
         pass
@@ -22359,15 +22421,15 @@
         else:
             return perpendicular_resolution(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='perpendicular_resolution', pretty_print=True):
@@ -22382,15 +22444,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='perpendicular_resolution')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='perpendicular_resolution', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='perpendicular_resolution'):
         pass
@@ -22435,15 +22497,15 @@
         else:
             return number_observed_reflections(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='number_observed_reflections', pretty_print=True):
@@ -22458,15 +22520,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='number_observed_reflections')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='number_observed_reflections', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='number_observed_reflections'):
         pass
@@ -22511,15 +22573,15 @@
         else:
             return number_unique_reflections(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='number_unique_reflections', pretty_print=True):
@@ -22534,15 +22596,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='number_unique_reflections')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='number_unique_reflections', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='number_unique_reflections'):
         pass
@@ -22587,15 +22649,15 @@
         else:
             return weighted_phase_residual(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='weighted_phase_residual', pretty_print=True):
@@ -22610,15 +22672,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='weighted_phase_residual')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='weighted_phase_residual', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='weighted_phase_residual'):
         pass
@@ -22663,15 +22725,15 @@
         else:
             return weighted_r_factor(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='weighted_r_factor', pretty_print=True):
@@ -22686,15 +22748,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='weighted_r_factor')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='weighted_r_factor', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='weighted_r_factor'):
         pass
@@ -22739,15 +22801,15 @@
         else:
             return data_completeness(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='data_completeness', pretty_print=True):
@@ -22762,15 +22824,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='data_completeness')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='data_completeness', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='data_completeness'):
         pass
@@ -22816,17 +22878,17 @@
         else:
             return fsc_curve_validation_type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
-            super(fsc_curve_validation_type, self)._hasContent()
+            super(fsc_curve_validation_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='fsc_curve_validation_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('fsc_curve_validation_type')
         if imported_ns_def_ is not None:
@@ -22839,15 +22901,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='fsc_curve_validation_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='fsc_curve_validation_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='fsc_curve_validation_type'):
@@ -22895,17 +22957,17 @@
         else:
             return layer_lines_validation_type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
-            super(layer_lines_validation_type, self)._hasContent()
+            super(layer_lines_validation_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='layer_lines_validation_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('layer_lines_validation_type')
         if imported_ns_def_ is not None:
@@ -22918,15 +22980,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='layer_lines_validation_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='layer_lines_validation_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='layer_lines_validation_type'):
@@ -22974,17 +23036,17 @@
         else:
             return structure_factors_validation_type(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
-            super(structure_factors_validation_type, self)._hasContent()
+            super(structure_factors_validation_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='structure_factors_validation_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('structure_factors_validation_type')
         if imported_ns_def_ is not None:
@@ -22997,15 +23059,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='structure_factors_validation_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='structure_factors_validation_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='structure_factors_validation_type'):
@@ -23067,15 +23129,15 @@
         self.structure_determination = structure_determination
     def add_structure_determination(self, value):
         self.structure_determination.append(value)
     def insert_structure_determination_at(self, index, value):
         self.structure_determination.insert(index, value)
     def replace_structure_determination_at(self, index, value):
         self.structure_determination[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.structure_determination
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='structure_determination_listType', pretty_print=True):
@@ -23090,15 +23152,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='structure_determination_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='structure_determination_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='structure_determination_listType'):
@@ -23169,15 +23231,15 @@
         self.validation_method = validation_method
     def add_validation_method(self, value):
         self.validation_method.append(value)
     def insert_validation_method_at(self, index, value):
         self.validation_method.insert(index, value)
     def replace_validation_method_at(self, index, value):
         self.validation_method[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.validation_method
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='validationType', pretty_print=True):
@@ -23192,15 +23254,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='validationType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='validationType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='validationType'):
@@ -23320,15 +23382,15 @@
             value = value
             enumerations = ['PDBe', 'PDBj', 'RCSB', 'PDBc']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on last_processingType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.deposition is not None or
             self.last_processing is not None
         ):
             return True
         else:
             return False
@@ -23344,15 +23406,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='sitesType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='sitesType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='sitesType'):
@@ -23482,15 +23544,15 @@
         return self.obsolete
     def set_obsolete(self, obsolete):
         self.obsolete = obsolete
     def get_update(self):
         return self.update
     def set_update(self, update):
         self.update = update
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.deposition is not None or
             self.header_release is not None or
             self.map_release is not None or
             self.obsolete is not None or
             self.update is not None
         ):
@@ -23509,15 +23571,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='key_datesType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='key_datesType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='key_datesType'):
@@ -23625,15 +23687,15 @@
         self.entry = entry
     def add_entry(self, value):
         self.entry.append(value)
     def insert_entry_at(self, index, value):
         self.entry.insert(index, value)
     def replace_entry_at(self, index, value):
         self.entry[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.entry
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='obsolete_listType', pretty_print=True):
@@ -23648,15 +23710,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='obsolete_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='obsolete_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='obsolete_listType'):
@@ -23727,15 +23789,15 @@
         self.entry = entry
     def add_entry(self, value):
         self.entry.append(value)
     def insert_entry_at(self, index, value):
         self.entry.insert(index, value)
     def replace_entry_at(self, index, value):
         self.entry[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.entry
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='superseded_by_listType', pretty_print=True):
@@ -23750,15 +23812,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='superseded_by_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='superseded_by_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='superseded_by_listType'):
@@ -23829,15 +23891,15 @@
         self.grant_reference = grant_reference
     def add_grant_reference(self, value):
         self.grant_reference.append(value)
     def insert_grant_reference_at(self, index, value):
         self.grant_reference.insert(index, value)
     def replace_grant_reference_at(self, index, value):
         self.grant_reference[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.grant_reference
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='grant_supportType', pretty_print=True):
@@ -23852,15 +23914,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='grant_supportType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='grant_supportType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='grant_supportType'):
@@ -23960,15 +24022,15 @@
             value = value
             enumerations = ['UK', 'USA', 'Japan']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on countryType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.name is not None or
             self.country is not None
         ):
             return True
         else:
             return False
@@ -23984,15 +24046,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='microscopy_centerType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='microscopy_centerType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='microscopy_centerType'):
@@ -24079,17 +24141,17 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_private(self):
         return self.private
     def set_private(self, private):
         self.private = private
-    def _hasContent(self):
+    def has__content(self):
         if (
-            super(contact_authorType, self)._hasContent()
+            super(contact_authorType, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='contact_authorType', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('contact_authorType')
         if imported_ns_def_ is not None:
@@ -24102,15 +24164,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='contact_authorType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='contact_authorType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='contact_authorType'):
@@ -24179,15 +24241,15 @@
         self.author = author
     def add_author(self, value):
         self.author.append(value)
     def insert_author_at(self, index, value):
         self.author.insert(index, value)
     def replace_author_at(self, index, value):
         self.author[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.author
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='authors_listType', pretty_print=True):
@@ -24202,15 +24264,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='authors_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='authors_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='authors_listType'):
@@ -24274,17 +24336,17 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_status_id(self):
         return self.status_id
     def set_status_id(self, status_id):
         self.status_id = status_id
-    def _hasContent(self):
+    def has__content(self):
         if (
-            super(statusType, self)._hasContent()
+            super(statusType, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='statusType', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('statusType')
         if imported_ns_def_ is not None:
@@ -24297,15 +24359,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='statusType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='statusType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='statusType'):
@@ -24370,15 +24432,15 @@
         self.ns_prefix_ = ns_prefix
     def get_private(self):
         return self.private
     def set_private(self, private):
         self.private = private
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='annotatorType', pretty_print=True):
@@ -24473,15 +24535,15 @@
                 return False
             value = value
             enumerations = ['ACADEMIC', 'COMMERCIAL', 'GOVERMENT', 'OTHER']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='organizationType', pretty_print=True):
@@ -24576,15 +24638,15 @@
         self.secondary_citation = secondary_citation
     def add_secondary_citation(self, value):
         self.secondary_citation.append(value)
     def insert_secondary_citation_at(self, index, value):
         self.secondary_citation.insert(index, value)
     def replace_secondary_citation_at(self, index, value):
         self.secondary_citation[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.primary_citation is not None or
             self.secondary_citation
         ):
             return True
         else:
             return False
@@ -24600,15 +24662,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='citation_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='citation_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='citation_listType'):
@@ -24678,15 +24740,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_citation_type(self):
         return self.citation_type
     def set_citation_type(self, citation_type):
         self.citation_type = citation_type
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.citation_type is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='primary_citationType', pretty_print=True):
@@ -24701,15 +24763,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='primary_citationType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='primary_citationType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='primary_citationType'):
@@ -24794,15 +24856,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_citation_type(self):
         return self.citation_type
     def set_citation_type(self, citation_type):
         self.citation_type = citation_type
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.citation_type is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='secondary_citationType', pretty_print=True):
@@ -24817,15 +24879,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='secondary_citationType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='secondary_citationType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='secondary_citationType'):
@@ -24919,15 +24981,15 @@
         self.auxiliary_link = auxiliary_link
     def add_auxiliary_link(self, value):
         self.auxiliary_link.append(value)
     def insert_auxiliary_link_at(self, index, value):
         self.auxiliary_link.insert(index, value)
     def replace_auxiliary_link_at(self, index, value):
         self.auxiliary_link[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.auxiliary_link
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='auxiliary_link_listType', pretty_print=True):
@@ -24942,15 +25004,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='auxiliary_link_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='auxiliary_link_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='auxiliary_link_listType'):
@@ -25028,15 +25090,15 @@
                 return False
             value = value
             enumerations = ['PUBMED', 'DOI', 'ISBN', 'ISSN', 'CAS', 'CSD', 'MEDLINE', 'ASTM']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType2' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='external_referencesType', pretty_print=True):
@@ -25132,15 +25194,15 @@
                 return False
             value = value
             enumerations = ['PUBMED', 'DOI', 'ISBN', 'ISSN', 'CAS', 'CSD', 'MEDLINE', 'ASTM']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType5' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='external_referencesType4', pretty_print=True):
@@ -25242,15 +25304,15 @@
             value = value
             enumerations = ['NOOVERLAP', 'PARTIALOVERLAP', 'FULLOVERLAP']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on in_frameType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.in_frame is not None or
             self.other is not None
         ):
             return True
         else:
             return False
@@ -25266,15 +25328,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='relationshipType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='relationshipType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='relationshipType'):
@@ -25376,15 +25438,15 @@
             value = value
             enumerations = ['NOOVERLAP', 'PARTIALOVERLAP', 'FULLOVERLAP']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on in_frameType7' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.in_frame is not None or
             self.other is not None
         ):
             return True
         else:
             return False
@@ -25400,15 +25462,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='relationshipType6')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='relationshipType6', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='relationshipType6'):
@@ -25497,15 +25559,15 @@
         self.supramolecule = supramolecule
     def add_supramolecule(self, value):
         self.supramolecule.append(value)
     def insert_supramolecule_at(self, index, value):
         self.supramolecule.insert(index, value)
     def replace_supramolecule_at(self, index, value):
         self.supramolecule[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.supramolecule
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='supramolecule_listType', pretty_print=True):
@@ -25520,15 +25582,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='supramolecule_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='supramolecule_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='supramolecule_listType'):
@@ -25650,15 +25712,15 @@
                 return False
             value = value
             enumerations = ['GO', 'ARBITRARY DEFINITION', 'PROTEIN ONTOLOGY']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType9' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='categoryType', pretty_print=True):
@@ -25747,15 +25809,15 @@
         self.macromolecule = macromolecule
     def add_macromolecule(self, value):
         self.macromolecule.append(value)
     def insert_macromolecule_at(self, index, value):
         self.macromolecule.insert(index, value)
     def replace_macromolecule_at(self, index, value):
         self.macromolecule[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.macromolecule
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='macromolecule_listType', pretty_print=True):
@@ -25770,15 +25832,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='macromolecule_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='macromolecule_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='macromolecule_listType'):
@@ -25881,15 +25943,15 @@
         return self.macromolecule_id
     def set_macromolecule_id(self, macromolecule_id):
         self.macromolecule_id = macromolecule_id
     def get_number_of_copies(self):
         return self.number_of_copies
     def set_number_of_copies(self, number_of_copies):
         self.number_of_copies = number_of_copies
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.macromolecule_id is not None or
             self.number_of_copies is not None
         ):
             return True
         else:
             return False
@@ -25905,15 +25967,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='macromoleculeType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='macromoleculeType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='macromoleculeType'):
@@ -26007,15 +26069,15 @@
                 return False
             value = value
             enumerations = ['UNIPROTKB', 'UNIPARC', 'INTERPRO', 'GO']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType11' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='external_referencesType10', pretty_print=True):
@@ -26128,15 +26190,15 @@
                 return False
             value = value
             enumerations = ['MDa', 'kDa/nm']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='experimentalType', pretty_print=True):
@@ -26249,15 +26311,15 @@
                 return False
             value = value
             enumerations = ['MDa', 'kDa/nm']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType13' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='theoreticalType', pretty_print=True):
@@ -26355,15 +26417,15 @@
         return self.triangulation
     def set_triangulation(self, triangulation):
         self.triangulation = triangulation
     def get_shell_id(self):
         return self.shell_id
     def set_shell_id(self, shell_id):
         self.shell_id = shell_id
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.name is not None or
             self.diameter is not None or
             self.triangulation is not None
         ):
             return True
         else:
@@ -26380,15 +26442,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='virus_shellType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='virus_shellType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='virus_shellType'):
@@ -26503,15 +26565,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_shell_diameter' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 10000:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_shell_diameter' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='diameterType', pretty_print=True):
@@ -26610,15 +26672,15 @@
         self.external_references = external_references
     def add_external_references(self, value):
         self.external_references.append(value)
     def insert_external_references_at(self, index, value):
         self.external_references.insert(index, value)
     def replace_external_references_at(self, index, value):
         self.external_references[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.string is not None or
             self.discrepancy_list is not None or
             self.external_references
         ):
             return True
         else:
@@ -26635,15 +26697,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='sequenceType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='sequenceType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='sequenceType'):
@@ -26750,15 +26812,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_discrepancyType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_discrepancyType_patterns_, ))
                 result = False
         return result
     validate_discrepancyType_patterns_ = [['^([ ARNDCEQGHILKMFPSTWYVUOBZJX\\(\\)]\\d+[ ARNDCEQGHILKMFPSTWYVUOBZJX\\(\\)])$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.discrepancy
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='discrepancy_listType', pretty_print=True):
@@ -26773,15 +26835,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='discrepancy_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='discrepancy_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='discrepancy_listType'):
@@ -26867,15 +26929,15 @@
                 return False
             value = value
             enumerations = ['REFSEQ', 'GENBANK']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType15' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='external_referencesType14', pretty_print=True):
@@ -26971,15 +27033,15 @@
                 return False
             value = value
             enumerations = ['CAS', 'PUBCHEM', 'DRUGBANK', 'CHEBI', 'CHEMBL']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType17' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='external_referencesType16', pretty_print=True):
@@ -27091,15 +27153,15 @@
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             pass
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.string is not None or
             self.discrepancy_list is not None or
             self.external_references
         ):
             return True
         else:
@@ -27116,15 +27178,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='sequenceType18')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='sequenceType18', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='sequenceType18'):
@@ -27233,15 +27295,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_discrepancyType20_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_discrepancyType20_patterns_, ))
                 result = False
         return result
     validate_discrepancyType20_patterns_ = [['^([AGCTRYSWKMBDHVN\\.-]\\d+[AGCTRYSWKMBDHVN\\.-])$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.discrepancy
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='discrepancy_listType19', pretty_print=True):
@@ -27256,15 +27318,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='discrepancy_listType19')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='discrepancy_listType19', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='discrepancy_listType19'):
@@ -27337,15 +27399,15 @@
         self.ns_prefix_ = ns_prefix
     def get_type(self):
         return self.type_
     def set_type(self, type_):
         self.type_ = type_
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='external_referencesType21', pretty_print=True):
@@ -27451,15 +27513,15 @@
         self.external_references = external_references
     def add_external_references(self, value):
         self.external_references.append(value)
     def insert_external_references_at(self, index, value):
         self.external_references.insert(index, value)
     def replace_external_references_at(self, index, value):
         self.external_references[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.string is not None or
             self.discrepancy_list is not None or
             self.connectivity is not None or
             self.external_references
         ):
             return True
@@ -27477,15 +27539,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='sequenceType22')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='sequenceType22', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='sequenceType22'):
@@ -27600,15 +27662,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_discrepancyType24_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_discrepancyType24_patterns_, ))
                 result = False
         return result
     validate_discrepancyType24_patterns_ = [['^([ARNDCEQGHILKMFPSTWYVUOBZJX]\\d+[ARNDCEQGHILKMFPSTWYVUOBZJX])$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.discrepancy
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='discrepancy_listType23', pretty_print=True):
@@ -27623,15 +27685,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='discrepancy_listType23')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='discrepancy_listType23', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='discrepancy_listType23'):
@@ -27707,15 +27769,15 @@
         return self._n_link
     def set__n_link(self, _n_link):
         self._n_link = _n_link
     def get__c_link(self):
         return self._c_link
     def set__c_link(self, _c_link):
         self._c_link = _c_link
-    def _hasContent(self):
+    def has__content(self):
         if (
             self._n_link is not None or
             self._c_link is not None
         ):
             return True
         else:
             return False
@@ -27731,15 +27793,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='connectivityType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='connectivityType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='connectivityType'):
@@ -27809,15 +27871,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_molecule_id(self):
         return self.molecule_id
     def set_molecule_id(self, molecule_id):
         self.molecule_id = molecule_id
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.molecule_id is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='_n-linkType', pretty_print=True):
@@ -27832,15 +27894,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='_n-linkType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='_n-linkType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='_n-linkType'):
@@ -27898,15 +27960,15 @@
         else:
             return molecule_id(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='molecule_id', pretty_print=True):
@@ -27921,15 +27983,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='molecule_id')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='molecule_id', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='molecule_id'):
         pass
@@ -27980,15 +28042,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_molecule_id(self):
         return self.molecule_id
     def set_molecule_id(self, molecule_id):
         self.molecule_id = molecule_id
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.molecule_id is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='_c-linkType', pretty_print=True):
@@ -28003,15 +28065,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='_c-linkType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='_c-linkType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='_c-linkType'):
@@ -28091,15 +28153,15 @@
                 return False
             value = value
             enumerations = ['UNIPROTKB', 'UNIPARC', 'INTERPRO', 'GO', 'GENBANK']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType26' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='external_referencesType25', pretty_print=True):
@@ -28200,15 +28262,15 @@
         self.external_references = external_references
     def add_external_references(self, value):
         self.external_references.append(value)
     def insert_external_references_at(self, index, value):
         self.external_references.insert(index, value)
     def replace_external_references_at(self, index, value):
         self.external_references[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.string is not None or
             self.discrepancy_list is not None or
             self.external_references
         ):
             return True
         else:
@@ -28225,15 +28287,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='sequenceType27')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='sequenceType27', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='sequenceType27'):
@@ -28340,15 +28402,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_discrepancyType29_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_discrepancyType29_patterns_, ))
                 result = False
         return result
     validate_discrepancyType29_patterns_ = [['^([ ARNDCEQGHILKMFPSTWYVUOBZJX\\(\\)]\\d+[ ARNDCEQGHILKMFPSTWYVUOBZJX\\(\\)])$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.discrepancy
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='discrepancy_listType28', pretty_print=True):
@@ -28363,15 +28425,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='discrepancy_listType28')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='discrepancy_listType28', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='discrepancy_listType28'):
@@ -28457,15 +28519,15 @@
                 return False
             value = value
             enumerations = ['REFSEQ', 'GENBANK', 'UNIPROTKB']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType31' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='external_referencesType30', pretty_print=True):
@@ -28561,15 +28623,15 @@
                 return False
             value = value
             enumerations = ['CARDBANK']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType36' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='external_referencesType35', pretty_print=True):
@@ -28658,15 +28720,15 @@
         self.specimen_preparation = specimen_preparation
     def add_specimen_preparation(self, value):
         self.specimen_preparation.append(value)
     def insert_specimen_preparation_at(self, index, value):
         self.specimen_preparation.insert(index, value)
     def replace_specimen_preparation_at(self, index, value):
         self.specimen_preparation[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.specimen_preparation
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='specimen_preparation_listType', pretty_print=True):
@@ -28681,15 +28743,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='specimen_preparation_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='specimen_preparation_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='specimen_preparation_listType'):
@@ -28785,15 +28847,15 @@
         self.microscopy = microscopy
     def add_microscopy(self, value):
         self.microscopy.append(value)
     def insert_microscopy_at(self, index, value):
         self.microscopy.insert(index, value)
     def replace_microscopy_at(self, index, value):
         self.microscopy[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.microscopy
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='microscopy_listType', pretty_print=True):
@@ -28808,15 +28870,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='microscopy_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='microscopy_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='microscopy_listType'):
@@ -28932,15 +28994,15 @@
                 return False
             value = value
             enumerations = ['mg/mL', 'mM']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType37' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='concentrationType', pretty_print=True):
@@ -29047,15 +29109,15 @@
             value = value
             enumerations = ['NEGATIVE', 'NONE', 'POSITIVE']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on typeType38' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.type_ is not None or
             self.material is not None or
             self.details is not None
         ):
             return True
         else:
@@ -29072,15 +29134,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='stainingType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='stainingType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='stainingType'):
@@ -29180,15 +29242,15 @@
         return self.material
     def set_material(self, material):
         self.material = material
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.material is not None or
             self.details is not None
         ):
             return True
         else:
             return False
@@ -29204,15 +29266,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='sugar_embeddingType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='sugar_embeddingType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='sugar_embeddingType'):
@@ -29308,15 +29370,15 @@
         return self.thickness
     def set_thickness(self, thickness):
         self.thickness = thickness
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.material is not None or
             self.angle is not None or
             self.thickness is not None or
             self.details is not None
         ):
             return True
@@ -29334,15 +29396,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='shadowingType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='shadowingType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='shadowingType'):
@@ -29456,15 +29518,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_angle_shadowing' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 90:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_angle_shadowing' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angleType', pretty_print=True):
@@ -29563,15 +29625,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_thickness_shadowing' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 30:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_thickness_shadowing' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='thicknessType', pretty_print=True):
@@ -29666,15 +29728,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_concentration' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='concentrationType39', pretty_print=True):
@@ -29769,15 +29831,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value < 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_film_thickness' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='film_thicknessType', pretty_print=True):
@@ -29872,15 +29934,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (int)' % {"value": value, "lineno": lineno, })
                 return False
             if value > 300:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_time_glow_discharge' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='timeType', pretty_print=True):
@@ -29975,15 +30037,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value < 0.0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_pressure_glow_discharge' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='pressureType', pretty_print=True):
@@ -30082,15 +30144,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_humidity_vitrification' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 100:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_humidity_vitrification' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='chamber_humidityType', pretty_print=True):
@@ -30182,15 +30244,15 @@
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, float):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             pass
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='chamber_temperatureType', pretty_print=True):
@@ -30305,15 +30367,15 @@
         return self.time
     def set_time(self, time):
         self.time = time
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.lipid_protein_ratio is not None or
             self.lipid_mixture is not None or
             self.instrument is not None or
             self.atmosphere is not None or
             self.temperature is not None or
             self.time is not None or
@@ -30334,15 +30396,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='crystal_formationType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='crystal_formationType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='crystal_formationType'):
@@ -30483,15 +30545,15 @@
         self.fiducial_marker = fiducial_marker
     def add_fiducial_marker(self, value):
         self.fiducial_marker.append(value)
     def insert_fiducial_marker_at(self, index, value):
         self.fiducial_marker.insert(index, value)
     def replace_fiducial_marker_at(self, index, value):
         self.fiducial_marker[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.fiducial_marker
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='fiducial_markers_listType', pretty_print=True):
@@ -30506,15 +30568,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='fiducial_markers_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='fiducial_markers_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='fiducial_markers_listType'):
@@ -30598,15 +30660,15 @@
             value = value
             enumerations = ['BAL-TEC HPM 010', 'EMS-002 RAPID IMMERSION FREEZER', 'LEICA EM HPM100', 'LEICA EM PACT', 'LEICA EM PACT2', 'OTHER']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on instrumentType41' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.instrument is not None or
             self.details is not None
         ):
             return True
         else:
             return False
@@ -30622,15 +30684,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='high_pressure_freezingType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='high_pressure_freezingType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='high_pressure_freezingType'):
@@ -30722,15 +30784,15 @@
         return self.focused_ion_beam
     def set_focused_ion_beam(self, focused_ion_beam):
         self.focused_ion_beam = focused_ion_beam
     def get_other_sectioning(self):
         return self.other_sectioning
     def set_other_sectioning(self, other_sectioning):
         self.other_sectioning = other_sectioning
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.ultramicrotomy is not None or
             self.focused_ion_beam is not None or
             self.other_sectioning is not None
         ):
             return True
         else:
@@ -30747,15 +30809,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='sectioningType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='sectioningType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='sectioningType'):
@@ -30853,15 +30915,15 @@
         return self.final_thickness
     def set_final_thickness(self, final_thickness):
         self.final_thickness = final_thickness
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.instrument is not None or
             self.temperature is not None or
             self.final_thickness is not None or
             self.details is not None
         ):
             return True
@@ -30879,15 +30941,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='ultramicrotomyType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='ultramicrotomyType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='ultramicrotomyType'):
@@ -31067,15 +31129,15 @@
             value = value
             enumerations = ['GALLIUM+', 'OTHER']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on ionType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.instrument is not None or
             self.ion is not None or
             self.voltage is not None or
             self.current is not None or
             self.dose_rate is not None or
             self.duration is not None or
@@ -31099,15 +31161,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='focused_ion_beamType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='focused_ion_beamType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='focused_ion_beamType'):
@@ -31268,15 +31330,15 @@
         self.specimen_preparation_id = specimen_preparation_id
     def add_specimen_preparation_id(self, value):
         self.specimen_preparation_id.append(value)
     def insert_specimen_preparation_id_at(self, index, value):
         self.specimen_preparation_id.insert(index, value)
     def replace_specimen_preparation_id_at(self, index, value):
         self.specimen_preparation_id[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.specimen_preparation_id
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='specimen_preparationsType', pretty_print=True):
@@ -31291,15 +31353,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='specimen_preparationsType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='specimen_preparationsType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='specimen_preparationsType'):
@@ -31381,15 +31443,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (int)' % {"value": value, "lineno": lineno, })
                 return False
             if value < 25:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_acceleration_voltage' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='acceleration_voltageType', pretty_print=True):
@@ -31488,15 +31550,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_c2_aperture_diameter' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 150:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_c2_aperture_diameter' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='c2_aperture_diameterType', pretty_print=True):
@@ -31595,15 +31657,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_nominal_cs' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 20:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_nominal_cs' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='nominal_csType', pretty_print=True):
@@ -31702,15 +31764,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_defocus_min' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 20:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_defocus_min' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='nominal_defocus_minType', pretty_print=True):
@@ -31809,15 +31871,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_defocus_min' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 20:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_defocus_min' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='calibrated_defocus_minType', pretty_print=True):
@@ -31916,15 +31978,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_defocus_max' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 50:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_defocus_max' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='nominal_defocus_maxType', pretty_print=True):
@@ -32023,15 +32085,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_defocus_max' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 50:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_defocus_max' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='calibrated_defocus_maxType', pretty_print=True):
@@ -32122,15 +32184,15 @@
         return self.temperature_max
     def set_temperature_max(self, temperature_max):
         self.temperature_max = temperature_max
     def get_temperature_average(self):
         return self.temperature_average
     def set_temperature_average(self, temperature_average):
         self.temperature_average = temperature_average
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.temperature_min is not None or
             self.temperature_max is not None or
             self.temperature_average is not None
         ):
             return True
         else:
@@ -32147,15 +32209,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='temperatureType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='temperatureType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='temperatureType'):
@@ -32263,15 +32325,15 @@
         return self.other
     def set_other(self, other):
         self.other = other
     def get_legacy(self):
         return self.legacy
     def set_legacy(self, legacy):
         self.legacy = legacy
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.none is not None or
             self.basic is not None or
             self.zemlin_tableau is not None or
             self.coma_free is not None or
             self.other is not None or
             self.legacy is not None
@@ -32291,15 +32353,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='alignment_procedureType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='alignment_procedureType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='alignment_procedureType'):
@@ -32395,15 +32457,15 @@
         else:
             return noneType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='noneType', pretty_print=True):
@@ -32418,15 +32480,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='noneType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='noneType', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='noneType'):
         pass
@@ -32477,15 +32539,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_residual_tilt(self):
         return self.residual_tilt
     def set_residual_tilt(self, residual_tilt):
         self.residual_tilt = residual_tilt
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.residual_tilt is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='basicType', pretty_print=True):
@@ -32500,15 +32562,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='basicType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='basicType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='basicType'):
@@ -32564,15 +32626,15 @@
         else:
             return zemlin_tableauType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='zemlin_tableauType', pretty_print=True):
@@ -32587,15 +32649,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='zemlin_tableauType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='zemlin_tableauType', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='zemlin_tableauType'):
         pass
@@ -32646,15 +32708,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_residual_tilt(self):
         return self.residual_tilt
     def set_residual_tilt(self, residual_tilt):
         self.residual_tilt = residual_tilt
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.residual_tilt is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='coma_freeType', pretty_print=True):
@@ -32669,15 +32731,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='coma_freeType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='coma_freeType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='coma_freeType'):
@@ -32733,15 +32795,15 @@
         else:
             return otherType(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='otherType', pretty_print=True):
@@ -32756,15 +32818,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='otherType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='otherType', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='otherType'):
         pass
@@ -32821,15 +32883,15 @@
         return self.astigmatism
     def set_astigmatism(self, astigmatism):
         self.astigmatism = astigmatism
     def get_electron_beam_tilt_params(self):
         return self.electron_beam_tilt_params
     def set_electron_beam_tilt_params(self, electron_beam_tilt_params):
         self.electron_beam_tilt_params = electron_beam_tilt_params
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.astigmatism is not None or
             self.electron_beam_tilt_params is not None
         ):
             return True
         else:
             return False
@@ -32845,15 +32907,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='legacyType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='legacyType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='legacyType'):
@@ -32936,15 +32998,15 @@
         self.image_recording = image_recording
     def add_image_recording(self, value):
         self.image_recording.append(value)
     def insert_image_recording_at(self, index, value):
         self.image_recording.insert(index, value)
     def replace_image_recording_at(self, index, value):
         self.image_recording[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.image_recording
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='image_recording_listType', pretty_print=True):
@@ -32959,15 +33021,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='image_recording_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='image_recording_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='image_recording_listType'):
@@ -33117,15 +33179,15 @@
             value = value
             enumerations = ['COUNTING', 'INTEGRATING', 'OTHER', 'SUPER-RESOLUTION']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on detector_modeType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.film_or_detector_model is not None or
             self.detector_mode is not None or
             self.digitization_details is not None or
             self.number_grids_imaged is not None or
             self.number_real_images is not None or
             self.number_diffraction_images is not None or
@@ -33151,15 +33213,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='image_recordingType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='image_recordingType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='image_recordingType'):
@@ -33375,15 +33437,15 @@
                 return False
             value = value
             enumerations = ['CCD', 'CMOS', 'DIRECT ELECTRON DETECTOR', 'STORAGE PHOSPOR (IMAGE PLATES)', 'FILM']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on categoryType43' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='film_or_detector_modelType', pretty_print=True):
@@ -33496,15 +33558,15 @@
             value = value
             enumerations = ['EIKONIX IEEE 488', 'EMIL 10', 'IMACON', 'NIKON COOLSCAN', 'NIKON SUPER COOLSCAN 9000', 'OPTRONICS', 'OTHER', 'PATCHWORK DENSITOMETER', 'PERKIN ELMER', 'PRIMESCAN', 'TEMSCAN', 'ZEISS SCAI']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on scannerType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.scanner is not None or
             self.dimensions is not None or
             self.sampling_interval is not None or
             self.frames_per_image is not None
         ):
             return True
@@ -33522,15 +33584,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='digitization_detailsType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='digitization_detailsType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='digitization_detailsType'):
@@ -33636,15 +33698,15 @@
         return self.width
     def set_width(self, width):
         self.width = width
     def get_height(self):
         return self.height
     def set_height(self, height):
         self.height = height
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.width is not None or
             self.height is not None
         ):
             return True
         else:
             return False
@@ -33660,15 +33722,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='dimensionsType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='dimensionsType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='dimensionsType'):
@@ -33741,15 +33803,15 @@
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='widthType', pretty_print=True):
@@ -33831,15 +33893,15 @@
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='heightType', pretty_print=True):
@@ -33934,15 +33996,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_scaning_interval' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='sampling_intervalType', pretty_print=True):
@@ -34041,15 +34103,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_average_exposure_time_type' % {"value": value, "lineno": lineno} )
                 result = False
             if value >= 240:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxExclusive restriction on allowed_average_exposure_time_type' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='average_exposure_timeType', pretty_print=True):
@@ -34148,15 +34210,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_electron_dose' % {"value": value, "lineno": lineno} )
                 result = False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_electron_dose' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='average_electron_dose_per_imageType', pretty_print=True):
@@ -34253,15 +34315,15 @@
         return self.lower_energy_threshold
     def set_lower_energy_threshold(self, lower_energy_threshold):
         self.lower_energy_threshold = lower_energy_threshold
     def get_upper_energy_threshold(self):
         return self.upper_energy_threshold
     def set_upper_energy_threshold(self, upper_energy_threshold):
         self.upper_energy_threshold = upper_energy_threshold
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.name is not None or
             self.slit_width is not None or
             self.lower_energy_threshold is not None or
             self.upper_energy_threshold is not None
         ):
             return True
@@ -34279,15 +34341,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='energy_filterType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='energy_filterType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='energy_filterType'):
@@ -34399,15 +34461,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_energy_filter_width' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 1000:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_energy_filter_width' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='slit_widthType', pretty_print=True):
@@ -34506,15 +34568,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_energy_window' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 500:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_energy_window' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='lower_energy_thresholdType', pretty_print=True):
@@ -34613,15 +34675,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_energy_window' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 500:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_energy_window' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='upper_energy_thresholdType', pretty_print=True):
@@ -34720,15 +34782,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_camera_length' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 3000:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_camera_length' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='camera_lengthType', pretty_print=True):
@@ -34816,32 +34878,32 @@
         self.angle = angle
     def add_angle(self, value):
         self.angle.append(value)
     def insert_angle_at(self, index, value):
         self.angle.insert(index, value)
     def replace_angle_at(self, index, value):
         self.angle[index] = value
-    def validate_angleType44(self, value):
+    def validate_angleType45(self, value):
         result = True
-        # Validate type angleType44, a restriction on xs:float.
+        # Validate type angleType45, a restriction on xs:float.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, float):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value < -70:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on angleType44' % {"value": value, "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on angleType45' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 70:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on angleType44' % {"value": value, "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on angleType45' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.angle
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='tilt_listType', pretty_print=True):
@@ -34856,15 +34918,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='tilt_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='tilt_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='tilt_listType'):
@@ -34894,16 +34956,16 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'angle' and child_.text:
             sval_ = child_.text
             fval_ = self.gds_parse_float(sval_, node, 'angle')
             fval_ = self.gds_validate_float(fval_, node, 'angle')
             self.angle.append(fval_)
             self.angle_nsprefix_ = child_.prefix
-            # validate type angleType44
-            self.validate_angleType44(self.angle[-1])
+            # validate type angleType45
+            self.validate_angleType45(self.angle[-1])
 # end class tilt_listType
 
 
 class axis2Type(axis_type):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = axis_type
@@ -34931,18 +34993,18 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_axis_rotation(self):
         return self.axis_rotation
     def set_axis_rotation(self, axis_rotation):
         self.axis_rotation = axis_rotation
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.axis_rotation is not None or
-            super(axis2Type, self)._hasContent()
+            super(axis2Type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='axis2Type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('axis2Type')
         if imported_ns_def_ is not None:
@@ -34955,15 +35017,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='axis2Type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='axis2Type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='axis2Type'):
@@ -35032,15 +35094,15 @@
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='axis_rotationType', pretty_print=True):
@@ -35139,15 +35201,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_angle_tomography' % {"value": value, "lineno": lineno} )
                 result = False
             if value >= 90:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxExclusive restriction on allowed_angle_tomography' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='min_angleType', pretty_print=True):
@@ -35245,15 +35307,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_angle_tomography' % {"value": value, "lineno": lineno} )
                 result = False
             if value >= 90:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxExclusive restriction on allowed_angle_tomography' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='max_angleType', pretty_print=True):
@@ -35351,15 +35413,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_angle_increment' % {"value": value, "lineno": lineno} )
                 result = False
             if value >= 15:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxExclusive restriction on allowed_angle_increment' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angle_incrementType', pretty_print=True):
@@ -35453,15 +35515,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_rise_type' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='delta_zType', pretty_print=True):
@@ -35553,15 +35615,15 @@
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, float):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             pass
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='delta_phiType', pretty_print=True):
@@ -35664,15 +35726,15 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.low_frequency_cutoff is not None or
             self.high_frequency_cutoff is not None or
             self.filter_function is not None or
             self.software_list is not None or
             self.details is not None
         ):
@@ -35691,15 +35753,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='spatial_filteringType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='spatial_filteringType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='spatial_filteringType'):
@@ -35804,15 +35866,15 @@
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='low_frequency_cutoffType', pretty_print=True):
@@ -35893,15 +35955,15 @@
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_frequency_cutoffType', pretty_print=True):
@@ -35985,15 +36047,15 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.software_list is not None or
             self.details is not None
         ):
             return True
         else:
             return False
@@ -36009,15 +36071,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='sharpeningType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='sharpeningType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='sharpeningType'):
@@ -36101,15 +36163,15 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self._brestore is not None or
             self.software_list is not None or
             self.details is not None
         ):
             return True
         else:
@@ -36126,15 +36188,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='b-factorSharpeningType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='b-factorSharpeningType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='b-factorSharpeningType'):
@@ -36234,15 +36296,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_brestore_type' % {"value": value, "lineno": lineno} )
                 result = False
             if value >= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxExclusive restriction on allowed_brestore_type' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='_brestoreType', pretty_print=True):
@@ -36290,15 +36352,15 @@
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
 # end class _brestoreType
 
 
-class otherType45(GeneratedsSuper):
+class otherType46(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, software_list=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36307,68 +36369,68 @@
         self.software_list = software_list
         self.software_list_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, otherType45)
+                CurrentSubclassModule_, otherType46)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if otherType45.subclass:
-            return otherType45.subclass(*args_, **kwargs_)
+        if otherType46.subclass:
+            return otherType46.subclass(*args_, **kwargs_)
         else:
-            return otherType45(*args_, **kwargs_)
+            return otherType46(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_software_list(self):
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.software_list is not None or
             self.details is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='otherType45', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('otherType45')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='otherType46', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('otherType46')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'otherType45':
+        if self.original_tagname_ is not None and name_ == 'otherType46':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='otherType45')
-        if self._hasContent():
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='otherType46')
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='otherType45', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='otherType46', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='otherType45'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='otherType46'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='otherType45', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='otherType46', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.software_list is not None:
             namespaceprefix_ = self.software_list_nsprefix_ + ':' if (UseCapturedNS_ and self.software_list_nsprefix_) else ''
             self.software_list.export(outfile, level, namespaceprefix_, namespacedef_='', name_='software_list', pretty_print=pretty_print)
@@ -36397,18 +36459,18 @@
             obj_.original_tagname_ = 'software_list'
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
-# end class otherType45
+# end class otherType46
 
 
-class dimensionsType46(GeneratedsSuper):
+class dimensionsType47(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, radius=None, width=None, height=None, depth=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36421,21 +36483,21 @@
         self.height = height
         self.height_nsprefix_ = None
         self.depth = depth
         self.depth_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, dimensionsType46)
+                CurrentSubclassModule_, dimensionsType47)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if dimensionsType46.subclass:
-            return dimensionsType46.subclass(*args_, **kwargs_)
+        if dimensionsType47.subclass:
+            return dimensionsType47.subclass(*args_, **kwargs_)
         else:
-            return dimensionsType46(*args_, **kwargs_)
+            return dimensionsType47(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_radius(self):
         return self.radius
@@ -36449,50 +36511,50 @@
         return self.height
     def set_height(self, height):
         self.height = height
     def get_depth(self):
         return self.depth
     def set_depth(self, depth):
         self.depth = depth
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.radius is not None or
             self.width is not None or
             self.height is not None or
             self.depth is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='dimensionsType46', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('dimensionsType46')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='dimensionsType47', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('dimensionsType47')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'dimensionsType46':
+        if self.original_tagname_ is not None and name_ == 'dimensionsType47':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='dimensionsType46')
-        if self._hasContent():
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='dimensionsType47')
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='dimensionsType46', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='dimensionsType47', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='dimensionsType46'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='dimensionsType47'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='dimensionsType46', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='dimensionsType47', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.radius is not None:
             namespaceprefix_ = self.radius_nsprefix_ + ':' if (UseCapturedNS_ and self.radius_nsprefix_) else ''
             self.radius.export(outfile, level, namespaceprefix_, namespacedef_='', name_='radius', pretty_print=pretty_print)
@@ -36521,29 +36583,29 @@
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'radius':
             obj_ = radiusType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.radius = obj_
             obj_.original_tagname_ = 'radius'
         elif nodeName_ == 'width':
-            obj_ = widthType48.factory(parent_object_=self)
+            obj_ = widthType49.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.width = obj_
             obj_.original_tagname_ = 'width'
         elif nodeName_ == 'height':
-            obj_ = heightType50.factory(parent_object_=self)
+            obj_ = heightType51.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.height = obj_
             obj_.original_tagname_ = 'height'
         elif nodeName_ == 'depth':
             obj_ = depthType.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.depth = obj_
             obj_.original_tagname_ = 'depth'
-# end class dimensionsType46
+# end class dimensionsType47
 
 
 class radiusType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units=None, valueOf_=None, gds_collector_=None, **kwargs_):
@@ -36572,28 +36634,28 @@
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def validate_unitsType47(self, value):
-        # Validate type unitsType47, a restriction on xs:token.
+    def validate_unitsType48(self, value):
+        # Validate type unitsType48, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
             enumerations = ['PIXEL', 'Å']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType47' % {"value" : encode_str_2_3(value), "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType48' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='radiusType', pretty_print=True):
@@ -36636,21 +36698,21 @@
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
-            self.validate_unitsType47(self.units)    # validate type unitsType47
+            self.validate_unitsType48(self.units)    # validate type unitsType48
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
 # end class radiusType
 
 
-class widthType48(GeneratedsSuper):
+class widthType49(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units=None, valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36658,77 +36720,77 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, widthType48)
+                CurrentSubclassModule_, widthType49)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if widthType48.subclass:
-            return widthType48.subclass(*args_, **kwargs_)
+        if widthType49.subclass:
+            return widthType49.subclass(*args_, **kwargs_)
         else:
-            return widthType48(*args_, **kwargs_)
+            return widthType49(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def validate_unitsType49(self, value):
-        # Validate type unitsType49, a restriction on xs:token.
+    def validate_unitsType50(self, value):
+        # Validate type unitsType50, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
             enumerations = ['PIXEL', 'Å']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType49' % {"value" : encode_str_2_3(value), "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType50' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='widthType48', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('widthType48')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='widthType49', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('widthType49')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'widthType48':
+        if self.original_tagname_ is not None and name_ == 'widthType49':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='widthType48')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='widthType49')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='widthType48'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='widthType49'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='widthType48', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='widthType49', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -36740,21 +36802,21 @@
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
-            self.validate_unitsType49(self.units)    # validate type unitsType49
+            self.validate_unitsType50(self.units)    # validate type unitsType50
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class widthType48
+# end class widthType49
 
 
-class heightType50(GeneratedsSuper):
+class heightType51(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units=None, valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -36762,77 +36824,77 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, heightType50)
+                CurrentSubclassModule_, heightType51)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if heightType50.subclass:
-            return heightType50.subclass(*args_, **kwargs_)
+        if heightType51.subclass:
+            return heightType51.subclass(*args_, **kwargs_)
         else:
-            return heightType50(*args_, **kwargs_)
+            return heightType51(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def validate_unitsType51(self, value):
-        # Validate type unitsType51, a restriction on xs:token.
+    def validate_unitsType52(self, value):
+        # Validate type unitsType52, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
             enumerations = ['PIXEL', 'Å']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType51' % {"value" : encode_str_2_3(value), "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType52' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='heightType50', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('heightType50')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='heightType51', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('heightType51')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'heightType50':
+        if self.original_tagname_ is not None and name_ == 'heightType51':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='heightType50')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='heightType51')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='heightType50'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='heightType51'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='heightType50', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='heightType51', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -36844,18 +36906,18 @@
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
-            self.validate_unitsType51(self.units)    # validate type unitsType51
+            self.validate_unitsType52(self.units)    # validate type unitsType52
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class heightType50
+# end class heightType51
 
 
 class depthType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units=None, valueOf_=None, gds_collector_=None, **kwargs_):
@@ -36884,28 +36946,28 @@
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
     def set_units(self, units):
         self.units = units
     def get_valueOf_(self): return self.valueOf_
     def set_valueOf_(self, valueOf_): self.valueOf_ = valueOf_
-    def validate_unitsType52(self, value):
-        # Validate type unitsType52, a restriction on xs:token.
+    def validate_unitsType53(self, value):
+        # Validate type unitsType53, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             value = value
             enumerations = ['PIXEL', 'Å']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
-                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType52' % {"value" : encode_str_2_3(value), "lineno": lineno} )
+                self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on unitsType53' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='depthType', pretty_print=True):
@@ -36948,15 +37010,15 @@
         return self
     def _buildAttributes(self, node, attrs, already_processed):
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
-            self.validate_unitsType52(self.units)    # validate type unitsType52
+            self.validate_unitsType53(self.units)    # validate type unitsType53
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
 # end class depthType
 
 
 class random_conical_tiltType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
@@ -37003,15 +37065,15 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_images is not None or
             self.tilt_angle is not None or
             self.software_list is not None or
             self.details is not None
         ):
             return True
@@ -37029,15 +37091,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='random_conical_tiltType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='random_conical_tiltType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='random_conical_tiltType'):
@@ -37149,15 +37211,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_tilt_angle_random_conical' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 180:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_tilt_angle_random_conical' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='tilt_angleType', pretty_print=True):
@@ -37260,15 +37322,15 @@
         return self.tilt_angle2
     def set_tilt_angle2(self, tilt_angle2):
         self.tilt_angle2 = tilt_angle2
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.software_list is not None or
             self.number_images is not None or
             self.tilt_angle1 is not None or
             self.tilt_angle2 is not None or
             self.details is not None
         ):
@@ -37287,15 +37349,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='orthogonal_tiltType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='orthogonal_tiltType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='orthogonal_tiltType'):
@@ -37415,15 +37477,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_tilt_angle1Orthogonal' % {"value": value, "lineno": lineno} )
                 result = False
             if value > -30:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_tilt_angle1Orthogonal' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='tilt_angle1Type', pretty_print=True):
@@ -37522,15 +37584,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minInclusive restriction on allowed_tilt_angle2Orthogonal' % {"value": value, "lineno": lineno} )
                 result = False
             if value > 50:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd maxInclusive restriction on allowed_tilt_angle2Orthogonal' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='tilt_angle2Type', pretty_print=True):
@@ -37631,15 +37693,15 @@
             value = value
             enumerations = ['REAL', 'RECIPROCAL']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on correction_space_type' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.anisotropic is not None or
             self.correction_space is not None
         ):
             return True
         else:
             return False
@@ -37655,15 +37717,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='phase_reversalType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='phase_reversalType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='phase_reversalType'):
@@ -37761,15 +37823,15 @@
             value = value
             enumerations = ['REAL', 'RECIPROCAL']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on correction_space_type' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.factor is not None or
             self.correction_space is not None
         ):
             return True
         else:
             return False
@@ -37785,15 +37847,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='amplitude_correctionType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='amplitude_correctionType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='amplitude_correctionType'):
@@ -37898,16 +37960,16 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_pdb_code_type_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_pdb_code_type_patterns_, ))
                 result = False
         return result
-    validate_pdb_code_type_patterns_ = [['^(\\d[\\dA-Za-z]{3})$']]
-    def _hasContent(self):
+    validate_pdb_code_type_patterns_ = [['^(\\d[\\dA-Za-z]{3}|pdb_\\d{5}[\\dA-Za-z]{3})$']]
+    def has__content(self):
         if (
             self.access_code is not None or
             self.chain
         ):
             return True
         else:
             return False
@@ -37923,15 +37985,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='starting_modelType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='starting_modelType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='starting_modelType'):
@@ -38015,15 +38077,15 @@
         return self.high_resolution
     def set_high_resolution(self, high_resolution):
         self.high_resolution = high_resolution
     def get_low_resolution(self):
         return self.low_resolution
     def set_low_resolution(self, low_resolution):
         self.low_resolution = low_resolution
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.high_resolution is not None or
             self.low_resolution is not None
         ):
             return True
         else:
             return False
@@ -38039,15 +38101,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='resolution_rangeType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='resolution_rangeType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='resolution_rangeType'):
@@ -38133,15 +38195,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on resolution_type' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType', pretty_print=True):
@@ -38236,15 +38298,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on resolution_type' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='low_resolutionType', pretty_print=True):
@@ -38292,15 +38354,15 @@
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
 # end class low_resolutionType
 
 
-class high_resolutionType53(GeneratedsSuper):
+class high_resolutionType54(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='Å', valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -38308,21 +38370,21 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, high_resolutionType53)
+                CurrentSubclassModule_, high_resolutionType54)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if high_resolutionType53.subclass:
-            return high_resolutionType53.subclass(*args_, **kwargs_)
+        if high_resolutionType54.subclass:
+            return high_resolutionType54.subclass(*args_, **kwargs_)
         else:
-            return high_resolutionType53(*args_, **kwargs_)
+            return high_resolutionType54(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
@@ -38339,46 +38401,46 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on resolution_type' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType53', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('high_resolutionType53')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType54', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('high_resolutionType54')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'high_resolutionType53':
+        if self.original_tagname_ is not None and name_ == 'high_resolutionType54':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='high_resolutionType53')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='high_resolutionType54')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='high_resolutionType53'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='high_resolutionType54'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType53', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType54', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -38392,15 +38454,15 @@
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class high_resolutionType53
+# end class high_resolutionType54
 
 
 class shell_listType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, shell=None, gds_collector_=None, **kwargs_):
@@ -38435,15 +38497,15 @@
         self.shell = shell
     def add_shell(self, value):
         self.shell.append(value)
     def insert_shell_at(self, index, value):
         self.shell.insert(index, value)
     def replace_shell_at(self, index, value):
         self.shell[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.shell
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='shell_listType', pretty_print=True):
@@ -38458,15 +38520,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='shell_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='shell_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='shell_listType'):
@@ -38564,15 +38626,15 @@
         return self.multiplicity
     def set_multiplicity(self, multiplicity):
         self.multiplicity = multiplicity
     def get_shell_id(self):
         return self.shell_id
     def set_shell_id(self, shell_id):
         self.shell_id = shell_id
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.high_resolution is not None or
             self.low_resolution is not None or
             self.number_structure_factors is not None or
             self.phase_residual is not None or
             self.fourier_space_coverage is not None or
             self.multiplicity is not None
@@ -38592,15 +38654,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='shellType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='shellType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='shellType'):
@@ -38650,20 +38712,20 @@
         if value is not None and 'shell_id' not in already_processed:
             already_processed.add('shell_id')
             self.shell_id = self.gds_parse_integer(value, node, 'shell_id')
             if self.shell_id <= 0:
                 raise_parse_error(node, 'Invalid PositiveInteger')
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         if nodeName_ == 'high_resolution':
-            obj_ = high_resolutionType54.factory(parent_object_=self)
+            obj_ = high_resolutionType55.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.high_resolution = obj_
             obj_.original_tagname_ = 'high_resolution'
         elif nodeName_ == 'low_resolution':
-            obj_ = low_resolutionType55.factory(parent_object_=self)
+            obj_ = low_resolutionType56.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.low_resolution = obj_
             obj_.original_tagname_ = 'low_resolution'
         elif nodeName_ == 'number_structure_factors' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'number_structure_factors')
             if ival_ <= 0:
@@ -38688,15 +38750,15 @@
             fval_ = self.gds_parse_float(sval_, node, 'multiplicity')
             fval_ = self.gds_validate_float(fval_, node, 'multiplicity')
             self.multiplicity = fval_
             self.multiplicity_nsprefix_ = child_.prefix
 # end class shellType
 
 
-class high_resolutionType54(GeneratedsSuper):
+class high_resolutionType55(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='Å', valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -38704,21 +38766,21 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, high_resolutionType54)
+                CurrentSubclassModule_, high_resolutionType55)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if high_resolutionType54.subclass:
-            return high_resolutionType54.subclass(*args_, **kwargs_)
+        if high_resolutionType55.subclass:
+            return high_resolutionType55.subclass(*args_, **kwargs_)
         else:
-            return high_resolutionType54(*args_, **kwargs_)
+            return high_resolutionType55(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
@@ -38735,46 +38797,46 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on resolution_type' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType54', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('high_resolutionType54')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType55', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('high_resolutionType55')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'high_resolutionType54':
+        if self.original_tagname_ is not None and name_ == 'high_resolutionType55':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='high_resolutionType54')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='high_resolutionType55')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='high_resolutionType54'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='high_resolutionType55'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType54', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='high_resolutionType55', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -38788,18 +38850,18 @@
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class high_resolutionType54
+# end class high_resolutionType55
 
 
-class low_resolutionType55(GeneratedsSuper):
+class low_resolutionType56(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='Å', valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -38807,21 +38869,21 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, low_resolutionType55)
+                CurrentSubclassModule_, low_resolutionType56)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if low_resolutionType55.subclass:
-            return low_resolutionType55.subclass(*args_, **kwargs_)
+        if low_resolutionType56.subclass:
+            return low_resolutionType56.subclass(*args_, **kwargs_)
         else:
-            return low_resolutionType55(*args_, **kwargs_)
+            return low_resolutionType56(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
@@ -38838,46 +38900,46 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on resolution_type' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='low_resolutionType55', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('low_resolutionType55')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='low_resolutionType56', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('low_resolutionType56')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'low_resolutionType55':
+        if self.original_tagname_ is not None and name_ == 'low_resolutionType56':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='low_resolutionType55')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='low_resolutionType56')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='low_resolutionType55'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='low_resolutionType56'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='low_resolutionType55', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='low_resolutionType56', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -38891,15 +38953,15 @@
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class low_resolutionType55
+# end class low_resolutionType56
 
 
 class segment_lengthType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='Å', valueOf_=None, gds_collector_=None, **kwargs_):
@@ -38941,15 +39003,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on non_zero_float' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='segment_lengthType', pretty_print=True):
@@ -39044,15 +39106,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on non_zero_float' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='segment_overlapType', pretty_print=True):
@@ -39147,15 +39209,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on non_zero_float' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='total_filament_lengthType', pretty_print=True):
@@ -39234,15 +39296,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_helical_parameters(self):
         return self.helical_parameters
     def set_helical_parameters(self, helical_parameters):
         self.helical_parameters = helical_parameters
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.helical_parameters is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='starting_symmetryType', pretty_print=True):
@@ -39257,15 +39319,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='starting_symmetryType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='starting_symmetryType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='starting_symmetryType'):
@@ -39345,15 +39407,15 @@
         return self.average
     def set_average(self, average):
         self.average = average
     def get_software_list(self):
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.min is not None or
             self.max is not None or
             self.average is not None or
             self.software_list is not None
         ):
             return True
@@ -39371,15 +39433,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='helix_lengthType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='helix_lengthType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='helix_lengthType'):
@@ -39465,15 +39527,15 @@
         else:
             return min(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='min', pretty_print=True):
@@ -39488,15 +39550,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='min')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='min', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='min'):
         pass
@@ -39541,15 +39603,15 @@
         else:
             return max(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='max', pretty_print=True):
@@ -39564,15 +39626,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='max')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='max', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='max'):
         pass
@@ -39617,15 +39679,15 @@
         else:
             return average(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
-    def _hasContent(self):
+    def has__content(self):
         if (
 
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='average', pretty_print=True):
@@ -39640,15 +39702,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='average')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='average', pretty_print=pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='average'):
         pass
@@ -39699,15 +39761,15 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_software_list(self):
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.software_list is not None
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='indexingType', pretty_print=True):
@@ -39722,15 +39784,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='indexingType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='indexingType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='indexingType'):
@@ -39804,15 +39866,15 @@
         return self.merit_function
     def set_merit_function(self, merit_function):
         self.merit_function = merit_function
     def get_angular_sampling(self):
         return self.angular_sampling
     def set_angular_sampling(self, angular_sampling):
         self.angular_sampling = angular_sampling
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_reference_projections is not None or
             self.merit_function is not None or
             self.angular_sampling is not None
         ):
             return True
         else:
@@ -39829,15 +39891,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='projection_matching_processingType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='projection_matching_processingType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='projection_matching_processingType'):
@@ -39941,15 +40003,15 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_angular_sampling' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType', pretty_print=True):
@@ -40052,15 +40114,15 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_reference_projections is not None or
             self.merit_function is not None or
             self.angular_sampling is not None or
             self.software_list is not None or
             self.details is not None
         ):
@@ -40079,15 +40141,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_multi_reference_alignmentType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_multi_reference_alignmentType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_multi_reference_alignmentType'):
@@ -40140,15 +40202,15 @@
         elif nodeName_ == 'merit_function':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'merit_function')
             value_ = self.gds_validate_string(value_, node, 'merit_function')
             self.merit_function = value_
             self.merit_function_nsprefix_ = child_.prefix
         elif nodeName_ == 'angular_sampling':
-            obj_ = angular_samplingType57.factory(parent_object_=self)
+            obj_ = angular_samplingType58.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.angular_sampling = obj_
             obj_.original_tagname_ = 'angular_sampling'
         elif nodeName_ == 'software_list':
             obj_ = software_list_type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.software_list = obj_
@@ -40158,15 +40220,15 @@
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
 # end class final_multi_reference_alignmentType
 
 
-class angular_samplingType57(GeneratedsSuper):
+class angular_samplingType58(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='degrees', valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40174,21 +40236,21 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, angular_samplingType57)
+                CurrentSubclassModule_, angular_samplingType58)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if angular_samplingType57.subclass:
-            return angular_samplingType57.subclass(*args_, **kwargs_)
+        if angular_samplingType58.subclass:
+            return angular_samplingType58.subclass(*args_, **kwargs_)
         else:
-            return angular_samplingType57(*args_, **kwargs_)
+            return angular_samplingType58(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
@@ -40205,46 +40267,46 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_angular_sampling' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType57', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('angular_samplingType57')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType58', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('angular_samplingType58')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'angular_samplingType57':
+        if self.original_tagname_ is not None and name_ == 'angular_samplingType58':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='angular_samplingType57')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='angular_samplingType58')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='angular_samplingType57'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='angular_samplingType58'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType57', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType58', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -40258,18 +40320,18 @@
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class angular_samplingType57
+# end class angular_samplingType58
 
 
-class final_multi_reference_alignmentType58(GeneratedsSuper):
+class final_multi_reference_alignmentType59(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, number_reference_projections=None, merit_function=None, angular_sampling=None, software_list=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40284,21 +40346,21 @@
         self.software_list = software_list
         self.software_list_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, final_multi_reference_alignmentType58)
+                CurrentSubclassModule_, final_multi_reference_alignmentType59)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if final_multi_reference_alignmentType58.subclass:
-            return final_multi_reference_alignmentType58.subclass(*args_, **kwargs_)
+        if final_multi_reference_alignmentType59.subclass:
+            return final_multi_reference_alignmentType59.subclass(*args_, **kwargs_)
         else:
-            return final_multi_reference_alignmentType58(*args_, **kwargs_)
+            return final_multi_reference_alignmentType59(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_number_reference_projections(self):
         return self.number_reference_projections
@@ -40316,51 +40378,51 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_reference_projections is not None or
             self.merit_function is not None or
             self.angular_sampling is not None or
             self.software_list is not None or
             self.details is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType58', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('final_multi_reference_alignmentType58')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType59', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('final_multi_reference_alignmentType59')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'final_multi_reference_alignmentType58':
+        if self.original_tagname_ is not None and name_ == 'final_multi_reference_alignmentType59':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_multi_reference_alignmentType58')
-        if self._hasContent():
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_multi_reference_alignmentType59')
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_multi_reference_alignmentType58', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_multi_reference_alignmentType59', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_multi_reference_alignmentType58'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_multi_reference_alignmentType59'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType58', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType59', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.number_reference_projections is not None:
             namespaceprefix_ = self.number_reference_projections_nsprefix_ + ':' if (UseCapturedNS_ and self.number_reference_projections_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -40404,33 +40466,33 @@
         elif nodeName_ == 'merit_function':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'merit_function')
             value_ = self.gds_validate_string(value_, node, 'merit_function')
             self.merit_function = value_
             self.merit_function_nsprefix_ = child_.prefix
         elif nodeName_ == 'angular_sampling':
-            obj_ = angular_samplingType59.factory(parent_object_=self)
+            obj_ = angular_samplingType60.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.angular_sampling = obj_
             obj_.original_tagname_ = 'angular_sampling'
         elif nodeName_ == 'software_list':
             obj_ = software_list_type.factory(parent_object_=self)
             obj_.build(child_, gds_collector_=gds_collector_)
             self.software_list = obj_
             obj_.original_tagname_ = 'software_list'
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
-# end class final_multi_reference_alignmentType58
+# end class final_multi_reference_alignmentType59
 
 
-class angular_samplingType59(GeneratedsSuper):
+class angular_samplingType60(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='degrees', valueOf_=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40438,21 +40500,21 @@
         self.ns_prefix_ = None
         self.units = _cast(None, units)
         self.units_nsprefix_ = None
         self.valueOf_ = valueOf_
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, angular_samplingType59)
+                CurrentSubclassModule_, angular_samplingType60)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if angular_samplingType59.subclass:
-            return angular_samplingType59.subclass(*args_, **kwargs_)
+        if angular_samplingType60.subclass:
+            return angular_samplingType60.subclass(*args_, **kwargs_)
         else:
-            return angular_samplingType59(*args_, **kwargs_)
+            return angular_samplingType60(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_units(self):
         return self.units
@@ -40469,46 +40531,46 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (float)' % {"value": value, "lineno": lineno, })
                 return False
             if value <= 0:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd minExclusive restriction on allowed_angular_sampling' % {"value": value, "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType59', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('angular_samplingType59')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType60', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('angular_samplingType60')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'angular_samplingType59':
+        if self.original_tagname_ is not None and name_ == 'angular_samplingType60':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='angular_samplingType59')
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='angular_samplingType60')
         outfile.write('>')
         self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_, pretty_print=pretty_print)
         outfile.write(self.convert_unicode(self.valueOf_))
         outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='angular_samplingType59'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='angular_samplingType60'):
         if self.units is not None and 'units' not in already_processed:
             already_processed.add('units')
             outfile.write(' units=%s' % (self.gds_encode(self.gds_format_string(quote_attrib(self.units), input_name='units')), ))
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType59', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='angular_samplingType60', fromsubclass_=False, pretty_print=True):
         pass
     def build(self, node, gds_collector_=None):
         self.gds_collector_ = gds_collector_
         if SaveElementTreeNode:
             self.gds_elementtree_node_ = node
         already_processed = set()
         self.ns_prefix_ = node.prefix
@@ -40522,15 +40584,15 @@
         value = find_attr_value_('units', node)
         if value is not None and 'units' not in already_processed:
             already_processed.add('units')
             self.units = value
             self.units = ' '.join(self.units.split())
     def _buildChildren(self, child_, node, nodeName_, fromsubclass_=False, gds_collector_=None):
         pass
-# end class angular_samplingType59
+# end class angular_samplingType60
 
 
 class extractionType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, number_tomograms=None, number_images_used=None, reference_model=None, method=None, software_list=None, details=None, gds_collector_=None, **kwargs_):
@@ -40586,15 +40648,15 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_tomograms is not None or
             self.number_images_used is not None or
             self.reference_model is not None or
             self.method is not None or
             self.software_list is not None or
             self.details is not None
@@ -40614,15 +40676,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='extractionType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='extractionType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='extractionType'):
@@ -40711,15 +40773,15 @@
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
 # end class extractionType
 
 
-class final_multi_reference_alignmentType60(GeneratedsSuper):
+class final_multi_reference_alignmentType61(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, number_reference_projections=None, merit_function=None, software_list=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40732,21 +40794,21 @@
         self.software_list = software_list
         self.software_list_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, final_multi_reference_alignmentType60)
+                CurrentSubclassModule_, final_multi_reference_alignmentType61)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if final_multi_reference_alignmentType60.subclass:
-            return final_multi_reference_alignmentType60.subclass(*args_, **kwargs_)
+        if final_multi_reference_alignmentType61.subclass:
+            return final_multi_reference_alignmentType61.subclass(*args_, **kwargs_)
         else:
-            return final_multi_reference_alignmentType60(*args_, **kwargs_)
+            return final_multi_reference_alignmentType61(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_number_reference_projections(self):
         return self.number_reference_projections
@@ -40760,50 +40822,50 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_reference_projections is not None or
             self.merit_function is not None or
             self.software_list is not None or
             self.details is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType60', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('final_multi_reference_alignmentType60')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType61', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('final_multi_reference_alignmentType61')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'final_multi_reference_alignmentType60':
+        if self.original_tagname_ is not None and name_ == 'final_multi_reference_alignmentType61':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_multi_reference_alignmentType60')
-        if self._hasContent():
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_multi_reference_alignmentType61')
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_multi_reference_alignmentType60', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_multi_reference_alignmentType61', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_multi_reference_alignmentType60'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_multi_reference_alignmentType61'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType60', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType61', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.number_reference_projections is not None:
             namespaceprefix_ = self.number_reference_projections_nsprefix_ + ':' if (UseCapturedNS_ and self.number_reference_projections_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -40854,18 +40916,18 @@
             obj_.original_tagname_ = 'software_list'
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
-# end class final_multi_reference_alignmentType60
+# end class final_multi_reference_alignmentType61
 
 
-class extractionType61(GeneratedsSuper):
+class extractionType62(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, number_tomograms=None, number_images_used=None, reference_model=None, method=None, software_list=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -40882,21 +40944,21 @@
         self.software_list = software_list
         self.software_list_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, extractionType61)
+                CurrentSubclassModule_, extractionType62)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if extractionType61.subclass:
-            return extractionType61.subclass(*args_, **kwargs_)
+        if extractionType62.subclass:
+            return extractionType62.subclass(*args_, **kwargs_)
         else:
-            return extractionType61(*args_, **kwargs_)
+            return extractionType62(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_number_tomograms(self):
         return self.number_tomograms
@@ -40918,52 +40980,52 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_tomograms is not None or
             self.number_images_used is not None or
             self.reference_model is not None or
             self.method is not None or
             self.software_list is not None or
             self.details is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='extractionType61', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('extractionType61')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='extractionType62', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('extractionType62')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'extractionType61':
+        if self.original_tagname_ is not None and name_ == 'extractionType62':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='extractionType61')
-        if self._hasContent():
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='extractionType62')
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='extractionType61', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='extractionType62', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='extractionType61'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='extractionType62'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='extractionType61', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='extractionType62', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.number_tomograms is not None:
             namespaceprefix_ = self.number_tomograms_nsprefix_ + ':' if (UseCapturedNS_ and self.number_tomograms_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -41040,18 +41102,18 @@
             obj_.original_tagname_ = 'software_list'
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
-# end class extractionType61
+# end class extractionType62
 
 
-class final_multi_reference_alignmentType62(GeneratedsSuper):
+class final_multi_reference_alignmentType63(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, number_reference_projections=None, merit_function=None, software_list=None, details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
@@ -41064,21 +41126,21 @@
         self.software_list = software_list
         self.software_list_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
             subclass = getSubclassFromModule_(
-                CurrentSubclassModule_, final_multi_reference_alignmentType62)
+                CurrentSubclassModule_, final_multi_reference_alignmentType63)
             if subclass is not None:
                 return subclass(*args_, **kwargs_)
-        if final_multi_reference_alignmentType62.subclass:
-            return final_multi_reference_alignmentType62.subclass(*args_, **kwargs_)
+        if final_multi_reference_alignmentType63.subclass:
+            return final_multi_reference_alignmentType63.subclass(*args_, **kwargs_)
         else:
-            return final_multi_reference_alignmentType62(*args_, **kwargs_)
+            return final_multi_reference_alignmentType63(*args_, **kwargs_)
     factory = staticmethod(factory)
     def get_ns_prefix_(self):
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_number_reference_projections(self):
         return self.number_reference_projections
@@ -41092,50 +41154,50 @@
         return self.software_list
     def set_software_list(self, software_list):
         self.software_list = software_list
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_reference_projections is not None or
             self.merit_function is not None or
             self.software_list is not None or
             self.details is not None
         ):
             return True
         else:
             return False
-    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType62', pretty_print=True):
-        imported_ns_def_ = GenerateDSNamespaceDefs_.get('final_multi_reference_alignmentType62')
+    def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType63', pretty_print=True):
+        imported_ns_def_ = GenerateDSNamespaceDefs_.get('final_multi_reference_alignmentType63')
         if imported_ns_def_ is not None:
             namespacedef_ = imported_ns_def_
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
-        if self.original_tagname_ is not None and name_ == 'final_multi_reference_alignmentType62':
+        if self.original_tagname_ is not None and name_ == 'final_multi_reference_alignmentType63':
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
-        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_multi_reference_alignmentType62')
-        if self._hasContent():
+        self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_multi_reference_alignmentType63')
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
-            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_multi_reference_alignmentType62', pretty_print=pretty_print)
+            self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_multi_reference_alignmentType63', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
-    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_multi_reference_alignmentType62'):
+    def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_multi_reference_alignmentType63'):
         pass
-    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType62', fromsubclass_=False, pretty_print=True):
+    def _exportChildren(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='final_multi_reference_alignmentType63', fromsubclass_=False, pretty_print=True):
         if pretty_print:
             eol_ = '\n'
         else:
             eol_ = ''
         if self.number_reference_projections is not None:
             namespaceprefix_ = self.number_reference_projections_nsprefix_ + ':' if (UseCapturedNS_ and self.number_reference_projections_nsprefix_) else ''
             showIndent(outfile, level, pretty_print)
@@ -41186,15 +41248,15 @@
             obj_.original_tagname_ = 'software_list'
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
-# end class final_multi_reference_alignmentType62
+# end class final_multi_reference_alignmentType63
 
 
 class resolutionType(GeneratedsSuper):
     __hash__ = GeneratedsSuper.__hash__
     subclass = None
     superclass = None
     def __init__(self, units='Å', res_type=None, valueOf_=None, gds_collector_=None, **kwargs_):
@@ -41255,15 +41317,15 @@
                 return False
             value = value
             enumerations = ['BY AUTHOR']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on res_typeType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
-    def _hasContent(self):
+    def has__content(self):
         if (
             (1 if type(self.valueOf_) in [int,float] else self.valueOf_)
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='resolutionType', pretty_print=True):
@@ -41363,15 +41425,15 @@
         return self.row
     def set_row(self, row):
         self.row = row
     def get_sec(self):
         return self.sec
     def set_sec(self, sec):
         self.sec = sec
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.col is not None or
             self.row is not None or
             self.sec is not None
         ):
             return True
         else:
@@ -41388,15 +41450,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='originType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='originType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='originType'):
@@ -41492,15 +41554,15 @@
         return self.y
     def set_y(self, y):
         self.y = y
     def get_z(self):
         return self.z
     def set_z(self, z):
         self.z = z
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.x is not None or
             self.y is not None or
             self.z is not None
         ):
             return True
         else:
@@ -41517,15 +41579,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='spacingType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='spacingType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='spacingType'):
@@ -41645,15 +41707,15 @@
         return self.beta
     def set_beta(self, beta):
         self.beta = beta
     def get_gamma(self):
         return self.gamma
     def set_gamma(self, gamma):
         self.gamma = gamma
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.a is not None or
             self.b is not None or
             self.c is not None or
             self.alpha is not None or
             self.beta is not None or
             self.gamma is not None
@@ -41673,15 +41735,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='cellType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='cellType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='cellType'):
@@ -41840,15 +41902,15 @@
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_slowType_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_slowType_patterns_, ))
                 result = False
         return result
     validate_slowType_patterns_ = [['^(X|Y|Z)$']]
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.fast is not None or
             self.medium is not None or
             self.slow is not None
         ):
             return True
         else:
@@ -41865,15 +41927,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='axis_orderType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='axis_orderType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='axis_orderType'):
@@ -41987,15 +42049,15 @@
         return self.y
     def set_y(self, y):
         self.y = y
     def get_z(self):
         return self.z
     def set_z(self, z):
         self.z = z
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.x is not None or
             self.y is not None or
             self.z is not None
         ):
             return True
         else:
@@ -42012,15 +42074,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='pixel_spacingType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='pixel_spacingType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='pixel_spacingType'):
@@ -42107,15 +42169,15 @@
         self.contour = contour
     def add_contour(self, value):
         self.contour.append(value)
     def insert_contour_at(self, index, value):
         self.contour.insert(index, value)
     def replace_contour_at(self, index, value):
         self.contour[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.contour
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='contour_listType', pretty_print=True):
@@ -42130,15 +42192,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='contour_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='contour_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='contour_listType'):
@@ -42228,15 +42290,15 @@
             value = value
             enumerations = ['EMDB', 'AUTHOR', 'SOFTWARE', 'ANNOTATOR']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on sourceType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.level is not None or
             self.source is not None
         ):
             return True
         else:
             return False
@@ -42252,15 +42314,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='contourType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='contourType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='contourType'):
@@ -42359,15 +42421,15 @@
         self.modelling = modelling
     def add_modelling(self, value):
         self.modelling.append(value)
     def insert_modelling_at(self, index, value):
         self.modelling.insert(index, value)
     def replace_modelling_at(self, index, value):
         self.modelling[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.modelling
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='modelling_listType', pretty_print=True):
@@ -42382,15 +42444,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='modelling_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='modelling_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='modelling_listType'):
@@ -42461,15 +42523,15 @@
         self.figure = figure
     def add_figure(self, value):
         self.figure.append(value)
     def insert_figure_at(self, index, value):
         self.figure.insert(index, value)
     def replace_figure_at(self, index, value):
         self.figure[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.figure
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='figure_listType', pretty_print=True):
@@ -42484,15 +42546,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='figure_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='figure_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='figure_listType'):
@@ -42563,15 +42625,15 @@
         self.segmentation = segmentation
     def add_segmentation(self, value):
         self.segmentation.append(value)
     def insert_segmentation_at(self, index, value):
         self.segmentation.insert(index, value)
     def replace_segmentation_at(self, index, value):
         self.segmentation[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.segmentation
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='segmentation_listType', pretty_print=True):
@@ -42586,15 +42648,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='segmentation_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='segmentation_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='segmentation_listType'):
@@ -42636,15 +42698,15 @@
     def __init__(self, file=None, details=None, mask_details=None, gds_collector_=None, **kwargs_):
         self.gds_collector_ = gds_collector_
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.file = file
-        self.validate_fileType63(self.file)
+        self.validate_fileType64(self.file)
         self.file_nsprefix_ = None
         self.details = details
         self.details_nsprefix_ = None
         self.mask_details = mask_details
         self.mask_details_nsprefix_ = None
     def factory(*args_, **kwargs_):
         if CurrentSubclassModule_ is not None:
@@ -42669,29 +42731,29 @@
         return self.details
     def set_details(self, details):
         self.details = details
     def get_mask_details(self):
         return self.mask_details
     def set_mask_details(self, mask_details):
         self.mask_details = mask_details
-    def validate_fileType63(self, value):
+    def validate_fileType64(self, value):
         result = True
-        # Validate type fileType63, a restriction on xs:token.
+        # Validate type fileType64, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
-                    self.validate_fileType63_patterns_, value):
-                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_fileType63_patterns_, ))
+                    self.validate_fileType64_patterns_, value):
+                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_fileType64_patterns_, ))
                 result = False
         return result
-    validate_fileType63_patterns_ = [['^([emd_\\d{4,}]+.*)$']]
-    def _hasContent(self):
+    validate_fileType64_patterns_ = [['^([emd_\\d{4,}]+.*)$']]
+    def has__content(self):
         if (
             self.file is not None or
             self.details is not None or
             self.mask_details is not None
         ):
             return True
         else:
@@ -42708,15 +42770,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='segmentationType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='segmentationType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='segmentationType'):
@@ -42757,16 +42819,16 @@
                 value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'file')
             value_ = self.gds_validate_string(value_, node, 'file')
             self.file = value_
             self.file_nsprefix_ = child_.prefix
-            # validate type fileType63
-            self.validate_fileType63(self.file)
+            # validate type fileType64
+            self.validate_fileType64(self.file)
         elif nodeName_ == 'details':
             value_ = child_.text
             value_ = self.gds_parse_string(value_, node, 'details')
             value_ = self.gds_validate_string(value_, node, 'details')
             self.details = value_
             self.details_nsprefix_ = child_.prefix
         elif nodeName_ == 'mask_details':
@@ -42813,15 +42875,15 @@
         self.slice = slice
     def add_slice(self, value):
         self.slice.append(value)
     def insert_slice_at(self, index, value):
         self.slice.insert(index, value)
     def replace_slice_at(self, index, value):
         self.slice[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.slice
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='slices_listType', pretty_print=True):
@@ -42836,15 +42898,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='slices_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='slices_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='slices_listType'):
@@ -42915,15 +42977,15 @@
         self.additional_map = additional_map
     def add_additional_map(self, value):
         self.additional_map.append(value)
     def insert_additional_map_at(self, index, value):
         self.additional_map.insert(index, value)
     def replace_additional_map_at(self, index, value):
         self.additional_map[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.additional_map
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='additional_map_listType', pretty_print=True):
@@ -42938,15 +43000,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='additional_map_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='additional_map_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='additional_map_listType'):
@@ -43017,15 +43079,15 @@
         self.half_map = half_map
     def add_half_map(self, value):
         self.half_map.append(value)
     def insert_half_map_at(self, index, value):
         self.half_map.insert(index, value)
     def replace_half_map_at(self, index, value):
         self.half_map[index] = value
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.half_map
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='half_map_listType', pretty_print=True):
@@ -43040,15 +43102,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='half_map_listType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='half_map_listType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='half_map_listType'):
@@ -43122,15 +43184,15 @@
         return self.chain
     def set_chain(self, chain):
         self.chain = chain
     def get_details(self):
         return self.details
     def set_details(self, details):
         self.details = details
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.access_code is not None or
             self.chain is not None or
             self.details is not None
         ):
             return True
         else:
@@ -43147,15 +43209,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='initial_modelType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='initial_modelType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='initial_modelType'):
@@ -43223,15 +43285,15 @@
         self.gds_elementtree_node_ = None
         self.original_tagname_ = None
         self.parent_object_ = kwargs_.get('parent_object_')
         self.ns_prefix_ = None
         self.chain_id = chain_id
         self.chain_id_nsprefix_ = None
         self.residue_range = residue_range
-        self.validate_residue_rangeType64(self.residue_range)
+        self.validate_residue_rangeType65(self.residue_range)
         self.residue_range_nsprefix_ = None
         self.number_of_copies_in_final_model = number_of_copies_in_final_model
         self.number_of_copies_in_final_model_nsprefix_ = None
         self.source_name = source_name
         self.validate_source_nameType(self.source_name)
         self.source_name_nsprefix_ = None
         self.initial_model_type = initial_model_type
@@ -43268,28 +43330,28 @@
         return self.source_name
     def set_source_name(self, source_name):
         self.source_name = source_name
     def get_initial_model_type(self):
         return self.initial_model_type
     def set_initial_model_type(self, initial_model_type):
         self.initial_model_type = initial_model_type
-    def validate_residue_rangeType64(self, value):
+    def validate_residue_rangeType65(self, value):
         result = True
-        # Validate type residue_rangeType64, a restriction on xs:token.
+        # Validate type residue_rangeType65, a restriction on xs:token.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
-                    self.validate_residue_rangeType64_patterns_, value):
-                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_residue_rangeType64_patterns_, ))
+                    self.validate_residue_rangeType65_patterns_, value):
+                self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_residue_rangeType65_patterns_, ))
                 result = False
         return result
-    validate_residue_rangeType64_patterns_ = [['^(\\d+-\\d+)$']]
+    validate_residue_rangeType65_patterns_ = [['^(\\d+-\\d+)$']]
     def validate_source_nameType(self, value):
         result = True
         # Validate type source_nameType, a restriction on xs:string.
         if value is not None and Validate_simpletypes_ and self.gds_collector_ is not None:
             if not isinstance(value, str):
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
@@ -43312,15 +43374,15 @@
             value = value
             enumerations = ['experimental model', 'in silico model', 'integrative model', 'other']
             if value not in enumerations:
                 lineno = self.gds_get_node_lineno_()
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s does not match xsd enumeration restriction on initial_model_typeType' % {"value" : encode_str_2_3(value), "lineno": lineno} )
                 result = False
         return result
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.chain_id is not None or
             self.residue_range is not None or
             self.number_of_copies_in_final_model is not None or
             self.source_name is not None or
             self.initial_model_type is not None
         ):
@@ -43339,15 +43401,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='chainType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='chainType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='chainType'):
@@ -43407,16 +43469,16 @@
                 value_ = re_.sub(String_cleanup_pat_, " ", value_).strip()
             else:
                 value_ = ""
             value_ = self.gds_parse_string(value_, node, 'residue_range')
             value_ = self.gds_validate_string(value_, node, 'residue_range')
             self.residue_range = value_
             self.residue_range_nsprefix_ = child_.prefix
-            # validate type residue_rangeType64
-            self.validate_residue_rangeType64(self.residue_range)
+            # validate type residue_rangeType65
+            self.validate_residue_rangeType65(self.residue_range)
         elif nodeName_ == 'number_of_copies_in_final_model' and child_.text:
             sval_ = child_.text
             ival_ = self.gds_parse_integer(sval_, node, 'number_of_copies_in_final_model')
             if ival_ <= 0:
                 raise_parse_error(child_, 'requires positiveInteger')
             ival_ = self.gds_validate_integer(ival_, node, 'number_of_copies_in_final_model')
             self.number_of_copies_in_final_model = ival_
@@ -43502,16 +43564,16 @@
                 self.gds_collector_.add_message('Value "%(value)s"%(lineno)s is not of the correct base simple type (str)' % {"value": value, "lineno": lineno, })
                 return False
             if not self.gds_validate_simple_patterns(
                     self.validate_pdb_code_type_patterns_, value):
                 self.gds_collector_.add_message('Value "%s" does not match xsd pattern restrictions: %s' % (encode_str_2_3(value), self.validate_pdb_code_type_patterns_, ))
                 result = False
         return result
-    validate_pdb_code_type_patterns_ = [['^(\\d[\\dA-Za-z]{3})$']]
-    def _hasContent(self):
+    validate_pdb_code_type_patterns_ = [['^(\\d[\\dA-Za-z]{3}|pdb_\\d{5}[\\dA-Za-z]{3})$']]
+    def has__content(self):
         if (
             self.access_code is not None or
             self.chain or
             self.details is not None
         ):
             return True
         else:
@@ -43528,15 +43590,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='final_modelType')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='final_modelType', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='final_modelType'):
@@ -43625,18 +43687,18 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_number_subtomograms_used(self):
         return self.number_subtomograms_used
     def set_number_subtomograms_used(self, number_subtomograms_used):
         self.number_subtomograms_used = number_subtomograms_used
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_subtomograms_used is not None or
-            super(subtomogram_final_reconstruction_type, self)._hasContent()
+            super(subtomogram_final_reconstruction_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='subtomogram_final_reconstruction_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('subtomogram_final_reconstruction_type')
         if imported_ns_def_ is not None:
@@ -43649,15 +43711,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='subtomogram_final_reconstruction_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='subtomogram_final_reconstruction_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='subtomogram_final_reconstruction_type'):
@@ -43726,18 +43788,18 @@
         return self.ns_prefix_
     def set_ns_prefix_(self, ns_prefix):
         self.ns_prefix_ = ns_prefix
     def get_number_images_used(self):
         return self.number_images_used
     def set_number_images_used(self, number_images_used):
         self.number_images_used = number_images_used
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.number_images_used is not None or
-            super(non_subtom_final_reconstruction_type, self)._hasContent()
+            super(non_subtom_final_reconstruction_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='non_subtom_final_reconstruction_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('non_subtom_final_reconstruction_type')
         if imported_ns_def_ is not None:
@@ -43750,15 +43812,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='non_subtom_final_reconstruction_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='non_subtom_final_reconstruction_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='non_subtom_final_reconstruction_type'):
@@ -43839,20 +43901,20 @@
         return self.tissue
     def set_tissue(self, tissue):
         self.tissue = tissue
     def get_cell(self):
         return self.cell
     def set_cell(self, cell):
         self.cell = cell
-    def _hasContent(self):
+    def has__content(self):
         if (
             self.organ is not None or
             self.tissue is not None or
             self.cell is not None or
-            super(cell_source_type, self)._hasContent()
+            super(cell_source_type, self).has__content()
         ):
             return True
         else:
             return False
     def export(self, outfile, level, namespaceprefix_='', namespacedef_='', name_='cell_source_type', pretty_print=True):
         imported_ns_def_ = GenerateDSNamespaceDefs_.get('cell_source_type')
         if imported_ns_def_ is not None:
@@ -43865,15 +43927,15 @@
             name_ = self.original_tagname_
         if UseCapturedNS_ and self.ns_prefix_:
             namespaceprefix_ = self.ns_prefix_ + ':'
         showIndent(outfile, level, pretty_print)
         outfile.write('<%s%s%s' % (namespaceprefix_, name_, namespacedef_ and ' ' + namespacedef_ or '', ))
         already_processed = set()
         self._exportAttributes(outfile, level, already_processed, namespaceprefix_, name_='cell_source_type')
-        if self._hasContent():
+        if self.has__content():
             outfile.write('>%s' % (eol_, ))
             self._exportChildren(outfile, level + 1, namespaceprefix_, namespacedef_, name_='cell_source_type', pretty_print=pretty_print)
             showIndent(outfile, level, pretty_print)
             outfile.write('</%s%s>%s' % (namespaceprefix_, name_, eol_))
         else:
             outfile.write('/>%s' % (eol_, ))
     def _exportAttributes(self, outfile, level, already_processed, namespaceprefix_='', name_='cell_source_type'):
@@ -44191,16 +44253,16 @@
     "admin_type",
     "alignment_procedureType",
     "amplitude_correctionType",
     "angleType",
     "angle_assignment_type",
     "angle_incrementType",
     "angular_samplingType",
-    "angular_samplingType57",
-    "angular_samplingType59",
+    "angular_samplingType58",
+    "angular_samplingType60",
     "annotatorType",
     "applied_symmetry_type",
     "author_ORCID_type",
     "author_order_type",
     "authors_listType",
     "auxiliary_link_listType",
     "auxiliary_link_type",
@@ -44264,15 +44326,15 @@
     "data_completeness",
     "delta_phiType",
     "delta_zType",
     "depthType",
     "diameterType",
     "digitization_detailsType",
     "dimensionsType",
-    "dimensionsType46",
+    "dimensionsType47",
     "discrepancy_listType",
     "discrepancy_listType19",
     "discrepancy_listType23",
     "discrepancy_listType28",
     "dna_macromolecule_type",
     "em_label_macromolecule_type",
     "emdb_cross_reference_list_type",
@@ -44286,15 +44348,15 @@
     "external_referencesType16",
     "external_referencesType21",
     "external_referencesType25",
     "external_referencesType30",
     "external_referencesType35",
     "external_referencesType4",
     "extractionType",
-    "extractionType61",
+    "extractionType62",
     "fib_current_type",
     "fib_dose_rate_type",
     "fib_duration_type",
     "fib_final_thickness_type",
     "fib_initial_thickness_type",
     "fib_voltage_type",
     "fiducial_marker_diameter_type",
@@ -44303,52 +44365,52 @@
     "figure_listType",
     "figure_type",
     "film_or_detector_modelType",
     "film_thicknessType",
     "film_type",
     "final_modelType",
     "final_multi_reference_alignmentType",
-    "final_multi_reference_alignmentType58",
-    "final_multi_reference_alignmentType60",
-    "final_multi_reference_alignmentType62",
+    "final_multi_reference_alignmentType59",
+    "final_multi_reference_alignmentType61",
+    "final_multi_reference_alignmentType63",
     "final_reconstruction_type",
     "focused_ion_beamType",
     "fsc_curve_validation_type",
     "grant_reference_type",
     "grant_supportType",
     "grid_pretreatment_type",
     "grid_type",
     "half_map_listType",
     "heightType",
-    "heightType50",
+    "heightType51",
     "helical_microscopy_type",
     "helical_parameters_type",
     "helical_preparation_type",
     "helical_processing_type",
     "helix_lengthType",
     "high_frequency_cutoffType",
     "high_pressure_freezingType",
     "high_resolutionType",
-    "high_resolutionType53",
     "high_resolutionType54",
+    "high_resolutionType55",
     "image_recordingType",
     "image_recording_listType",
     "indexingType",
     "initial_modelType",
     "integer_vector_map_type",
     "interpretation_type",
     "journal_citation",
     "key_datesType",
     "layer_lines_type",
     "layer_lines_validation_type",
     "legacyType",
     "ligand_macromolecule_type",
     "low_frequency_cutoffType",
     "low_resolutionType",
-    "low_resolutionType55",
+    "low_resolutionType56",
     "lower_energy_thresholdType",
     "macromoleculeType",
     "macromolecule_listType",
     "macromolecule_list_type",
     "macromolecule_source_type",
     "macromolecules_and_complexes_type",
     "map_statistics_type",
@@ -44377,15 +44439,15 @@
     "organelle_or_cellular_component_supramolecule_type",
     "organelle_source_type",
     "organism_type",
     "organizationType",
     "originType",
     "orthogonal_tiltType",
     "otherType",
-    "otherType45",
+    "otherType46",
     "other_macromolecule_type",
     "parallel_resolution",
     "particle_selection_type",
     "pdb_cross_reference_list_type",
     "pdb_cross_reference_type",
     "pdb_model_type",
     "perpendicular_resolution",
@@ -44485,10 +44547,10 @@
     "virus_shellType",
     "virus_species_name_type",
     "virus_supramolecule_type",
     "vitrification_type",
     "weighted_phase_residual",
     "weighted_r_factor",
     "widthType",
-    "widthType48",
+    "widthType49",
     "zemlin_tableauType"
 ]
```

### Comparing `wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py` & `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/simple_test.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py` & `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/cif_emdb_translator/test_cif_to_xml_translator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/data/emdb-v3.xsd`

 * *Files 1% similar despite different names*

#### Comparing `wwpdb.utils.emdb-1.3/wwpdb/utils/emdb/data/emdb-v3.xsd` & `wwpdb.utils.emdb-1.4/wwpdb/utils/emdb/data/emdb-v3.xsd`

```diff
@@ -20,15 +20,15 @@
           <xs:sequence>
             <xs:element ref="validation_method" maxOccurs="unbounded"/>
           </xs:sequence>
         </xs:complexType>
       </xs:element>
     </xs:sequence>
     <xs:attribute name="emdb_id" type="emdb_id_type" use="required"/>
-    <xs:attribute name="version" type="xs:token" default="3.0.3.3"/>
+    <xs:attribute name="version" type="xs:token" default="3.0.4.1"/>
     <!-- <xs:attribute name="composite_structure" type="xs:boolean"/> -->
   </xs:complexType>
   <xs:complexType name="admin_type">
     <xs:sequence>
       <xs:element name="status_history_list" type="version_list_type" minOccurs="0"/>
       <xs:element name="current_status" type="version_type"/>
       <xs:element name="sites">
@@ -2509,14 +2509,40 @@
       <xs:element name="software" type="software_type" minOccurs="0" maxOccurs="unbounded"/>
     </xs:sequence>
   </xs:complexType>
   <xs:complexType name="software_type">
     <xs:sequence>
       <xs:element name="name" type="xs:token" minOccurs="0"/>
       <xs:element name="version" type="xs:token" minOccurs="0"/>
+      <xs:element name="category" minOccurs="0">
+        <xs:simpleType>
+          <xs:restriction base="xs:token">
+            <xs:enumeration value="CLASSIFICATION"/>
+            <xs:enumeration value="CRYSTALLOGRAPHY MERGING"/>
+            <xs:enumeration value="CTF CORRECTION"/>
+            <xs:enumeration value="DIFFRACTION INDEXING"/>
+            <xs:enumeration value="EWALD SPHERE CORRECTION"/>
+            <xs:enumeration value="FINAL EULER ASSIGNMENT"/>
+            <xs:enumeration value="IMAGE ACQUISITION"/>
+            <xs:enumeration value="INITIAL EULER ASSIGNMENT"/>
+            <xs:enumeration value="LATTICE DISTORTION CORRECTION"/>
+            <xs:enumeration value="LAYERLINE INDEXING"/>
+            <xs:enumeration value="MASKING"/>
+            <xs:enumeration value="MODEL FITTING"/>
+            <xs:enumeration value="MODEL REFINEMENT"/>
+            <xs:enumeration value="MOLECULAR REPLACEMENT"/>
+            <xs:enumeration value="OTHER"/>
+            <xs:enumeration value="PARTICLE SELECTION"/>
+            <xs:enumeration value="RECONSTRUCTION"/>
+            <xs:enumeration value="SERIES ALIGNMENT"/>
+            <xs:enumeration value="SYMMETRY DETERMINATION"/>
+            <xs:enumeration value="VOLUME SELECTION"/>
+          </xs:restriction>
+        </xs:simpleType>
+      </xs:element>
       <xs:element name="processing_details" type="xs:string" minOccurs="0"/>
     </xs:sequence>
   </xs:complexType>
   <xs:simpleType name="allowed_film_or_detector_model">
     <xs:restriction base="xs:token">
       <xs:enumeration value="AGFA SCIENTA FILM"/>
       <xs:enumeration value="DIRECT ELECTRON APOLLO (4k x 4k)"/>
@@ -3132,15 +3158,15 @@
     <xs:sequence>
       <xs:element name="pdb_id" type="pdb_code_type" minOccurs="0"/>
       <xs:element name="chain_id_list" type="chain_type" minOccurs="0"/>
     </xs:sequence>
   </xs:complexType>
   <xs:simpleType name="pdb_code_type">
     <xs:restriction base="xs:token">
-      <xs:pattern value="\d[\dA-Za-z]{3}"/>
+      <xs:pattern value="\d[\dA-Za-z]{3}|pdb_\d{5}[\dA-Za-z]{3}"/>
     </xs:restriction>
   </xs:simpleType>
   <xs:complexType name="chain_type">
     <xs:sequence>
       <xs:element name="chain_id" type="chain_pdb_id" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="residue_range" minOccurs="0" maxOccurs="1">
         <xs:simpleType>
```

### Comparing `wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/PKG-INFO` & `wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.emdb
-Version: 1.3
+Version: 1.4
 Summary: wwPDB EMDB to XML converter
 Home-page: https://github.com/rcsb/py-wwpdb_utils_config
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.utils.emdb-1.3/wwpdb.utils.emdb.egg-info/SOURCES.txt` & `wwpdb.utils.emdb-1.4/wwpdb.utils.emdb.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 wwpdb.utils.emdb.egg-info/entry_points.txt
 wwpdb.utils.emdb.egg-info/not-zip-safe
 wwpdb.utils.emdb.egg-info/requires.txt
 wwpdb.utils.emdb.egg-info/top_level.txt
 wwpdb/utils/__init__.py
 wwpdb/utils/emdb/EmdbSchema.py
 wwpdb/utils/emdb/__init__.py
+wwpdb/utils/emdb/atomcheck/__init__.py
+wwpdb/utils/emdb/atomcheck/atomcheck.py
 wwpdb/utils/emdb/cif_emdb_translator/README.md
 wwpdb/utils/emdb/cif_emdb_translator/__init__.py
 wwpdb/utils/emdb/cif_emdb_translator/cif_emdb_translator.py
 wwpdb/utils/emdb/cif_emdb_translator/em_emd_conversion.py
 wwpdb/utils/emdb/cif_emdb_translator/emdb.py
 wwpdb/utils/emdb/cif_emdb_translator/generatedsnamespaces.py
 wwpdb/utils/emdb/cif_emdb_translator/simple_test.py
```

