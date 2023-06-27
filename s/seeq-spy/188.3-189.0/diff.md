# Comparing `tmp/seeq-spy-188.3.tar.gz` & `tmp/seeq-spy-189.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeq-spy-188.3.tar", last modified: Tue Jun 20 20:16:07 2023, max compression
+gzip compressed data, was "seeq-spy-189.0.tar", last modified: Tue Jun 27 19:11:18 2023, max compression
```

## Comparing `seeq-spy-188.3.tar` & `seeq-spy-189.0.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.508319 seeq-spy-188.3/
--rw-rw-rw-   0        0        0    33551 2023-02-10 21:28:23.000000 seeq-spy-188.3/LICENSE
--rw-rw-rw-   0        0        0      207 2023-02-10 21:28:23.000000 seeq-spy-188.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4606 2023-06-20 20:16:07.507318 seeq-spy-188.3/PKG-INFO
--rw-rw-rw-   0        0        0     4091 2023-04-18 17:55:42.000000 seeq-spy-188.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.329321 seeq-spy-188.3/seeq/
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.346319 seeq-spy-188.3/seeq/base/
--rw-rw-rw-   0        0        0       36 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/base/__init__.py
--rw-rw-rw-   0        0        0      875 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/base/proputil.py
--rw-rw-rw-   0        0        0    32535 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/base/seeq_names.py
--rw-rw-rw-   0        0        0      157 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/base/system.py
--rw-rw-rw-   0        0        0     4788 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/base/util.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.348318 seeq-spy-188.3/seeq/scripts/
--rw-rw-rw-   0        0        0    12250 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/scripts/create_monitoring_alerts.py
--rw-rw-rw-   0        0        0    49636 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/scripts/create_monitoring_workbook.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.370318 seeq-spy-188.3/seeq/spy/
--rw-rw-rw-   0        0        0     1953 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/__init__.py
--rw-rw-rw-   0        0        0    32016 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_common.py
--rw-rw-rw-   0        0        0     4687 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_config.py
--rw-rw-rw-   0        0        0     4424 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_datalab.py
--rw-rw-rw-   0        0        0     9914 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_errors.py
--rw-rw-rw-   0        0        0    49041 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_login.py
--rw-rw-rw-   0        0        0    94326 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_metadata.py
--rw-rw-rw-   0        0        0     5822 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_metadata_push_results.py
--rw-rw-rw-   0        0        0     2954 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_plot.py
--rw-rw-rw-   0        0        0    55640 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_pull.py
--rw-rw-rw-   0        0        0    68835 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_push.py
--rw-rw-rw-   0        0        0     5155 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_redaction.py
--rw-rw-rw-   0        0        0    44741 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_search.py
--rw-rw-rw-   0        0        0    20309 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_session.py
--rw-rw-rw-   0        0        0    16507 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_status.py
--rw-rw-rw-   0        0        0    20657 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_swap.py
--rw-rw-rw-   0        0        0     3471 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_upgrade.py
--rw-rw-rw-   0        0        0    10707 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_url.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.374318 seeq-spy-188.3/seeq/spy/acl/
--rw-rw-rw-   0        0        0      104 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/acl/__init__.py
--rw-rw-rw-   0        0        0    12172 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/acl/_pull.py
--rw-rw-rw-   0        0        0    11351 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/acl/_push.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.380318 seeq-spy-188.3/seeq/spy/addons/
--rw-rw-rw-   0        0        0      188 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/addons/__init__.py
--rw-rw-rw-   0        0        0    26376 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/addons/_install.py
--rw-rw-rw-   0        0        0     2408 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/addons/_permissions.py
--rw-rw-rw-   0        0        0    12137 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/addons/_search.py
--rw-rw-rw-   0        0        0     5334 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/addons/_uninstall.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.388318 seeq-spy-188.3/seeq/spy/assets/
--rw-rw-rw-   0        0        0      336 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/__init__.py
--rw-rw-rw-   0        0        0     3638 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_brochure.py
--rw-rw-rw-   0        0        0    12419 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_build.py
--rw-rw-rw-   0        0        0     3133 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_context.py
--rw-rw-rw-   0        0        0    48189 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_model.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.401318 seeq-spy-188.3/seeq/spy/assets/_trees/
--rw-rw-rw-   0        0        0       69 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/__init__.py
--rw-rw-rw-   0        0        0     1375 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_constants.py
--rw-rw-rw-   0        0        0     7325 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_csv.py
--rw-rw-rw-   0        0        0    22068 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_match.py
--rw-rw-rw-   0        0        0     2629 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_pandas.py
--rw-rw-rw-   0        0        0     6458 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_path.py
--rw-rw-rw-   0        0        0    23208 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_properties.py
--rw-rw-rw-   0        0        0    13381 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_pull.py
--rw-rw-rw-   0        0        0    58791 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_tree.py
--rw-rw-rw-   0        0        0     5897 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_utils.py
--rw-rw-rw-   0        0        0    25525 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_validate.py
--rw-rw-rw-   0        0        0     2538 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/brochure.html
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.404318 seeq-spy-188.3/seeq/spy/docs/
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.429319 seeq-spy-188.3/seeq/spy/docs/Documentation/
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.430318 seeq-spy-188.3/seeq/spy/docs/Documentation/Administration/
--rw-rw-rw-   0        0        0     6577 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Administration/User Migration.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.438318 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/
--rw-rw-rw-   0        0        0    17428 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
--rw-rw-rw-   0        0        0    33412 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
--rw-rw-rw-   0        0        0    16700 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
--rw-rw-rw-   0        0        0     8406 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
--rw-rw-rw-   0        0        0    38889 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
--rw-rw-rw-   0        0        0      870 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
--rw-rw-rw-   0        0        0   186560 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
--rw-rw-rw-   0        0        0   239024 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
--rw-rw-rw-   0        0        0   229026 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
--rw-rw-rw-   0        0        0    24627 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.448319 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/
--rw-rw-rw-   0        0        0   135771 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
--rw-rw-rw-   0        0        0   152116 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
--rw-rw-rw-   0        0        0   207271 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
--rw-rw-rw-   0        0        0      325 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/Readme.txt
--rw-rw-rw-   0        0        0   141516 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
--rw-rw-rw-   0        0        0   439966 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
--rw-rw-rw-   0        0        0   189377 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
--rw-rw-rw-   0        0        0    15177 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Command Reference.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.457319 seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/
--rw-rw-rw-   0        0        0    94677 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/Example Export.zip
--rw-rw-rw-   0        0        0   111771 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
--rw-rw-rw-   0        0        0   113084 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
--rw-rw-rw-   0        0        0  1083835 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
--rw-rw-rw-   0        0        0      429 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
--rw-rw-rw-   0        0        0   674467 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Tutorial.ipynb
--rw-rw-rw-   0        0        0    11595 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Version Considerations.ipynb
--rw-rw-rw-   0        0        0  1557151 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Workbook Templates.ipynb
--rw-rw-rw-   0        0        0    54071 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.acl.ipynb
--rw-rw-rw-   0        0        0    11195 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.jobs.ipynb
--rw-rw-rw-   0        0        0    13015 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.login.ipynb
--rw-rw-rw-   0        0        0   128103 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.pull.ipynb
--rw-rw-rw-   0        0        0    99541 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.push.ipynb
--rw-rw-rw-   0        0        0    57289 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.search.ipynb
--rw-rw-rw-   0        0        0    95777 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.swap.ipynb
--rw-rw-rw-   0        0        0    10829 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.widgets.ipynb
--rw-rw-rw-   0        0        0    69828 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.workbooks.ipynb
--rw-rw-rw-   0        0        0       60 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/docs/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/docs/_copy.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.463318 seeq-spy-188.3/seeq/spy/jobs/
--rw-rw-rw-   0        0        0      491 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/jobs/__init__.py
--rw-rw-rw-   0        0        0     9869 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/jobs/_execute.py
--rw-rw-rw-   0        0        0     6111 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/jobs/_pull.py
--rw-rw-rw-   0        0        0     9398 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/jobs/_push.py
--rw-rw-rw-   0        0        0    25737 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/jobs/_schedule.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.466318 seeq-spy-188.3/seeq/spy/notifications/
--rw-rw-rw-   0        0        0      153 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/notifications/__init__.py
--rw-rw-rw-   0        0        0    11927 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/notifications/_emails.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.467318 seeq-spy-188.3/seeq/spy/utils/
--rw-rw-rw-   0        0        0     1569 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.470317 seeq-spy-188.3/seeq/spy/widgets/
--rw-rw-rw-   0        0        0      200 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/widgets/__init__.py
--rw-rw-rw-   0        0        0     4158 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/widgets/_ipy_utils.py
--rw-rw-rw-   0        0        0    30480 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/widgets/_widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.497318 seeq-spy-188.3/seeq/spy/workbooks/
--rw-rw-rw-   0        0        0     3012 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/__init__.py
--rw-rw-rw-   0        0        0    43729 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_annotation.py
--rw-rw-rw-   0        0        0    34087 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_content.py
--rw-rw-rw-   0        0        0    40974 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_data.py
--rw-rw-rw-   0        0        0     6639 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_folder.py
--rw-rw-rw-   0        0        0    14611 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_item.py
--rw-rw-rw-   0        0        0     5448 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_item_map.py
--rw-rw-rw-   0        0        0     3033 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_load.py
--rw-rw-rw-   0        0        0     3456 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_mustache.py
--rw-rw-rw-   0        0        0    14175 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_pull.py
--rw-rw-rw-   0        0        0    23088 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_push.py
--rw-rw-rw-   0        0        0     6316 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_render.py
--rw-rw-rw-   0        0        0    27127 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_report_content_utilities.py
--rw-rw-rw-   0        0        0     4729 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_save.py
--rw-rw-rw-   0        0        0    15545 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_search.py
--rw-rw-rw-   0        0        0    37445 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_template.py
--rw-rw-rw-   0        0        0    11995 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_user.py
--rw-rw-rw-   0        0        0    52462 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_workbook.py
--rw-rw-rw-   0        0        0    48819 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_worksheet.py
--rw-rw-rw-   0        0        0    51518 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_workstep.py
--rw-rw-rw-   0        0        0   427362 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/workbooks/app.css
-drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.506319 seeq-spy-188.3/seeq_spy.egg-info/
--rw-rw-rw-   0        0        0     4606 2023-06-20 20:16:07.000000 seeq-spy-188.3/seeq_spy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4785 2023-06-20 20:16:07.000000 seeq-spy-188.3/seeq_spy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 20:16:07.000000 seeq-spy-188.3/seeq_spy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-26 16:53:37.000000 seeq-spy-188.3/seeq_spy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      311 2023-06-20 20:16:07.000000 seeq-spy-188.3/seeq_spy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-20 20:16:07.000000 seeq-spy-188.3/seeq_spy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 20:16:07.508319 seeq-spy-188.3/setup.cfg
--rw-rw-rw-   0        0        0     1677 2023-06-20 19:50:26.000000 seeq-spy-188.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.956932 seeq-spy-189.0/
+-rw-rw-rw-   0        0        0    33551 2023-02-10 21:28:23.000000 seeq-spy-189.0/LICENSE
+-rw-rw-rw-   0        0        0      207 2023-02-10 21:28:23.000000 seeq-spy-189.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4606 2023-06-27 19:11:18.955929 seeq-spy-189.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4091 2023-04-18 17:55:42.000000 seeq-spy-189.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.753929 seeq-spy-189.0/seeq/
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.769930 seeq-spy-189.0/seeq/base/
+-rw-rw-rw-   0        0        0       36 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/base/__init__.py
+-rw-rw-rw-   0        0        0      875 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/base/proputil.py
+-rw-rw-rw-   0        0        0    32794 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/base/seeq_names.py
+-rw-rw-rw-   0        0        0      157 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/base/system.py
+-rw-rw-rw-   0        0        0     4788 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/base/util.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.771926 seeq-spy-189.0/seeq/scripts/
+-rw-rw-rw-   0        0        0    12250 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/scripts/create_monitoring_alerts.py
+-rw-rw-rw-   0        0        0    49636 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/scripts/create_monitoring_workbook.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.797934 seeq-spy-189.0/seeq/spy/
+-rw-rw-rw-   0        0        0     1953 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/__init__.py
+-rw-rw-rw-   0        0        0    32016 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_common.py
+-rw-rw-rw-   0        0        0     4687 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_config.py
+-rw-rw-rw-   0        0        0     4424 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_datalab.py
+-rw-rw-rw-   0        0        0     9914 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_errors.py
+-rw-rw-rw-   0        0        0    49041 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_login.py
+-rw-rw-rw-   0        0        0    95701 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_metadata.py
+-rw-rw-rw-   0        0        0     5822 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_metadata_push_results.py
+-rw-rw-rw-   0        0        0     2954 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_plot.py
+-rw-rw-rw-   0        0        0    55640 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_pull.py
+-rw-rw-rw-   0        0        0    68835 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_push.py
+-rw-rw-rw-   0        0        0     5155 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_redaction.py
+-rw-rw-rw-   0        0        0    57799 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_search.py
+-rw-rw-rw-   0        0        0    20456 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_session.py
+-rw-rw-rw-   0        0        0    16874 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_status.py
+-rw-rw-rw-   0        0        0    20657 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_swap.py
+-rw-rw-rw-   0        0        0     3471 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_upgrade.py
+-rw-rw-rw-   0        0        0    10707 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/_url.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.802934 seeq-spy-189.0/seeq/spy/acl/
+-rw-rw-rw-   0        0        0      104 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/acl/__init__.py
+-rw-rw-rw-   0        0        0    12172 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/acl/_pull.py
+-rw-rw-rw-   0        0        0    11351 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/acl/_push.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.809928 seeq-spy-189.0/seeq/spy/addons/
+-rw-rw-rw-   0        0        0      188 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/addons/__init__.py
+-rw-rw-rw-   0        0        0    26376 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/addons/_install.py
+-rw-rw-rw-   0        0        0     2408 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/addons/_permissions.py
+-rw-rw-rw-   0        0        0    12137 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/addons/_search.py
+-rw-rw-rw-   0        0        0     5334 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/addons/_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.819933 seeq-spy-189.0/seeq/spy/assets/
+-rw-rw-rw-   0        0        0      336 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/__init__.py
+-rw-rw-rw-   0        0        0     3638 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_brochure.py
+-rw-rw-rw-   0        0        0    12419 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_build.py
+-rw-rw-rw-   0        0        0     3133 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_context.py
+-rw-rw-rw-   0        0        0    48189 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_model.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.833929 seeq-spy-189.0/seeq/spy/assets/_trees/
+-rw-rw-rw-   0        0        0       69 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/__init__.py
+-rw-rw-rw-   0        0        0     1375 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_constants.py
+-rw-rw-rw-   0        0        0     7350 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_csv.py
+-rw-rw-rw-   0        0        0    22068 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_match.py
+-rw-rw-rw-   0        0        0     2629 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_pandas.py
+-rw-rw-rw-   0        0        0     6458 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_path.py
+-rw-rw-rw-   0        0        0    23208 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_properties.py
+-rw-rw-rw-   0        0        0    13479 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_pull.py
+-rw-rw-rw-   0        0        0    58791 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_tree.py
+-rw-rw-rw-   0        0        0     5897 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_utils.py
+-rw-rw-rw-   0        0        0    25525 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/_trees/_validate.py
+-rw-rw-rw-   0        0        0     2538 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/assets/brochure.html
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.835929 seeq-spy-189.0/seeq/spy/docs/
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.868929 seeq-spy-189.0/seeq/spy/docs/Documentation/
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.870927 seeq-spy-189.0/seeq/spy/docs/Documentation/Administration/
+-rw-rw-rw-   0        0        0     6577 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Administration/User Migration.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.877929 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/
+-rw-rw-rw-   0        0        0    17428 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
+-rw-rw-rw-   0        0        0    33412 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
+-rw-rw-rw-   0        0        0    16700 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
+-rw-rw-rw-   0        0        0     8406 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
+-rw-rw-rw-   0        0        0    38889 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
+-rw-rw-rw-   0        0        0      870 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
+-rw-rw-rw-   0        0        0   186560 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
+-rw-rw-rw-   0        0        0   239024 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
+-rw-rw-rw-   0        0        0   229026 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
+-rw-rw-rw-   0        0        0    24627 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.892929 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/
+-rw-rw-rw-   0        0        0   135771 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
+-rw-rw-rw-   0        0        0   152116 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
+-rw-rw-rw-   0        0        0   207271 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
+-rw-rw-rw-   0        0        0      325 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/Readme.txt
+-rw-rw-rw-   0        0        0   141516 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
+-rw-rw-rw-   0        0        0   439966 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
+-rw-rw-rw-   0        0        0   189377 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
+-rw-rw-rw-   0        0        0    15177 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Command Reference.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.904927 seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/
+-rw-rw-rw-   0        0        0    94677 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/Example Export.zip
+-rw-rw-rw-   0        0        0   111771 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
+-rw-rw-rw-   0        0        0   113084 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
+-rw-rw-rw-   0        0        0  1083835 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
+-rw-rw-rw-   0        0        0      429 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
+-rw-rw-rw-   0        0        0   674467 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Tutorial.ipynb
+-rw-rw-rw-   0        0        0    11595 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Version Considerations.ipynb
+-rw-rw-rw-   0        0        0  1557151 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/Workbook Templates.ipynb
+-rw-rw-rw-   0        0        0    54071 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.acl.ipynb
+-rw-rw-rw-   0        0        0    11195 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.jobs.ipynb
+-rw-rw-rw-   0        0        0    13015 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.login.ipynb
+-rw-rw-rw-   0        0        0   128103 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.pull.ipynb
+-rw-rw-rw-   0        0        0    99541 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.push.ipynb
+-rw-rw-rw-   0        0        0    57647 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.search.ipynb
+-rw-rw-rw-   0        0        0    95777 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.swap.ipynb
+-rw-rw-rw-   0        0        0    10829 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.widgets.ipynb
+-rw-rw-rw-   0        0        0    69828 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/Documentation/spy.workbooks.ipynb
+-rw-rw-rw-   0        0        0       60 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/docs/_copy.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.910928 seeq-spy-189.0/seeq/spy/jobs/
+-rw-rw-rw-   0        0        0      491 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/jobs/__init__.py
+-rw-rw-rw-   0        0        0     9869 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/jobs/_execute.py
+-rw-rw-rw-   0        0        0     6111 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/jobs/_pull.py
+-rw-rw-rw-   0        0        0     9398 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/jobs/_push.py
+-rw-rw-rw-   0        0        0    25737 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/jobs/_schedule.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.912929 seeq-spy-189.0/seeq/spy/notifications/
+-rw-rw-rw-   0        0        0      153 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/notifications/__init__.py
+-rw-rw-rw-   0        0        0    11927 2023-06-27 19:11:15.000000 seeq-spy-189.0/seeq/spy/notifications/_emails.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.914936 seeq-spy-189.0/seeq/spy/utils/
+-rw-rw-rw-   0        0        0     1569 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.919931 seeq-spy-189.0/seeq/spy/widgets/
+-rw-rw-rw-   0        0        0      200 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4158 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/widgets/_ipy_utils.py
+-rw-rw-rw-   0        0        0    30480 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/widgets/_widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.945936 seeq-spy-189.0/seeq/spy/workbooks/
+-rw-rw-rw-   0        0        0     3012 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/__init__.py
+-rw-rw-rw-   0        0        0    43729 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_annotation.py
+-rw-rw-rw-   0        0        0    34087 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_content.py
+-rw-rw-rw-   0        0        0    40974 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_data.py
+-rw-rw-rw-   0        0        0     6639 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_folder.py
+-rw-rw-rw-   0        0        0    14611 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_item.py
+-rw-rw-rw-   0        0        0     5448 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_item_map.py
+-rw-rw-rw-   0        0        0     3033 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_load.py
+-rw-rw-rw-   0        0        0     3456 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_mustache.py
+-rw-rw-rw-   0        0        0    14175 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_pull.py
+-rw-rw-rw-   0        0        0    23095 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_push.py
+-rw-rw-rw-   0        0        0     6316 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_render.py
+-rw-rw-rw-   0        0        0    27127 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_report_content_utilities.py
+-rw-rw-rw-   0        0        0     4729 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_save.py
+-rw-rw-rw-   0        0        0    15545 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_search.py
+-rw-rw-rw-   0        0        0    37445 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_template.py
+-rw-rw-rw-   0        0        0    11995 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_user.py
+-rw-rw-rw-   0        0        0    52462 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_workbook.py
+-rw-rw-rw-   0        0        0    48819 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_worksheet.py
+-rw-rw-rw-   0        0        0    51518 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/_workstep.py
+-rw-rw-rw-   0        0        0   427362 2023-06-27 19:11:16.000000 seeq-spy-189.0/seeq/spy/workbooks/app.css
+drwxrwxrwx   0        0        0        0 2023-06-27 19:11:18.954930 seeq-spy-189.0/seeq_spy.egg-info/
+-rw-rw-rw-   0        0        0     4606 2023-06-27 19:11:18.000000 seeq-spy-189.0/seeq_spy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4785 2023-06-27 19:11:18.000000 seeq-spy-189.0/seeq_spy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-27 19:11:18.000000 seeq-spy-189.0/seeq_spy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-26 16:53:37.000000 seeq-spy-189.0/seeq_spy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      311 2023-06-27 19:11:18.000000 seeq-spy-189.0/seeq_spy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-27 19:11:18.000000 seeq-spy-189.0/seeq_spy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-27 19:11:18.956932 seeq-spy-189.0/setup.cfg
+-rw-rw-rw-   0        0        0     1677 2023-06-21 20:54:31.000000 seeq-spy-189.0/setup.py
```

### Comparing `seeq-spy-188.3/LICENSE` & `seeq-spy-189.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/PKG-INFO` & `seeq-spy-189.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 188.3
+Version: 189.0
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-spy-188.3/README.md` & `seeq-spy-189.0/README.md`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/base/proputil.py` & `seeq-spy-189.0/seeq/base/proputil.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/base/seeq_names.py` & `seeq-spy-189.0/seeq/base/seeq_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,20 @@
         stress_test = 'Stress Test'
         time_stream = 'TimeStream'
         tree_file = 'Tree File'
         w_i_t_s_m_l = 'WITSML'
         wonderware = 'Wonderware'
         x_h_q = 'XHQ'
     
+    class IdentityProviderDatasourceClasses:
+        l_d_a_p = 'LDAP'
+        o_auth2 = 'OAuth 2.0'
+        seeq_auth = 'Auth'
+        windows_auth = 'Windows Auth'
+    
     class LocalDatasources:
         class SeeqMetadataItemStorage:
             datasource_class = 'Seeq Metadata'
             datasource_id = 'Seeq Metadata'
             datasource_name = 'Seeq Metadata'
         
         class SeeqCalculationItemStorage:
@@ -624,14 +630,15 @@
         previous_index_at = 'Previous Index At'
         sync_result = 'Sync Result'
         indexing_schedule_supported = 'Indexing Schedule Supported'
         asset_tree_search_index_needs_updating = 'Asset Tree Search Index Needs Updating'
         sync_mode = 'Sync Mode'
         items_archived_count = 'Items Archived Count'
         indexing_duration = 'Indexing Duration'
+        provides_everyone_group_identities = 'Provides Everyone Group Identities'
         indexing_progress_timestamp = 'Indexing Progress Timestamp'
         asset_progress = 'Asset Progress'
         asset_count = 'Asset Count'
         previous_asset_count = 'Previous Asset Count'
         signal_progress = 'Signal Progress'
         signal_count = 'Signal Count'
         previous_signal_count = 'Previous Signal Count'
```

### Comparing `seeq-spy-188.3/seeq/base/util.py` & `seeq-spy-189.0/seeq/base/util.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/scripts/create_monitoring_alerts.py` & `seeq-spy-189.0/seeq/scripts/create_monitoring_alerts.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/scripts/create_monitoring_workbook.py` & `seeq-spy-189.0/seeq/scripts/create_monitoring_workbook.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/__init__.py` & `seeq-spy-189.0/seeq/spy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,11 +51,11 @@
 server_version: Optional[str] = None
 """
 Equivalent to `spy.session.server_version`
 """
 
 __all__ = ['acl', 'addons', 'assets', 'docs', 'workbooks', 'widgets', 'login', 'logout', 'plot', 'pull', 'push',
            'search', 'swap', 'PATH_ROOT', 'DEFAULT_WORKBOOK_PATH', 'GLOBALS_ONLY', 'GLOBALS_AND_ALL_WORKBOOKS',
-           'INHERIT_FROM_WORKBOOK', 'Session', 'Status', 'options', 'session', 'client', 'user', 'server_version',
-           'jobs', 'notifications', 'upgrade', 'utils', 'errors']
+           'INHERIT_FROM_WORKBOOK', 'Session', 'Status', 'options', 'session', 'client', 'user',
+           'server_version', 'jobs', 'notifications', 'upgrade', 'utils', 'errors']
 
-__version__ = '%d.%d' % (int('188'), int('3'))
+__version__ = '%d.%d' % (int('189'), int('0'))
```

### Comparing `seeq-spy-188.3/seeq/spy/_common.py` & `seeq-spy-189.0/seeq/spy/_common.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/_config.py` & `seeq-spy-189.0/seeq/spy/_config.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/_datalab.py` & `seeq-spy-189.0/seeq/spy/_datalab.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/_errors.py` & `seeq-spy-189.0/seeq/spy/_errors.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/_login.py` & `seeq-spy-189.0/seeq/spy/_login.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/_metadata.py` & `seeq-spy-189.0/seeq/spy/_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,24 +296,39 @@
             except ApiException as e:
                 _common.raise_or_catalog(status, df=push_context.push_results, column='Push Result',
                                          index=index, e=e)
 
     if _common.present(row_dict, 'Push Result'):
         return
 
+    def _row_datasource_matches_context_datasource() -> bool:
+        # We can't update tree relationships using the batch endpoint across multiple datasources. Don't bother with
+        # Asset updates if this item appears to be in a datasource that doesn't match the context. CRAB-37889
+        if _common.get(row_dict, 'Reference') is True:
+            return True
+        elif _common.present(row_dict, 'Datasource Class') and _common.present(row_dict, 'Datasource ID'):
+            return (_common.get(row_dict, 'Datasource Class') == push_context.datasource_output.datasource_class
+                    and _common.get(row_dict, 'Datasource ID') == push_context.datasource_output.datasource_id)
+        elif _common.present(row_dict, 'Datasource Name'):
+            return _common.get(row_dict, 'Datasource Name') == push_context.datasource_output.name
+        else:
+            return True
+
+    datasource_matches = _row_datasource_matches_context_datasource()
+
     scoped_data_id = get_scoped_data_id(row_dict, push_context.workbook_context.workbook_id)
     if not _common.present(row_dict, 'Datasource Class'):
         row_dict['Datasource Class'] = push_context.datasource_output.datasource_class
 
     if not _common.present(row_dict, 'Datasource ID'):
         row_dict['Datasource ID'] = push_context.datasource_output.datasource_id
 
     path = determine_path(row_dict)
     parent_data_id = None
-    if path:
+    if path and datasource_matches:
         parent_data_id = _reify_path(session, status, push_context, path)
 
     def _set_properties_by_id():
         _row_sync_token = push_context.sync_token if _needs_sync_token(session, row_dict) else None
         _set_item_properties(session, row_dict, _row_sync_token)
         _set_existing_item_push_results(session, index, push_context.push_results, row_dict)
 
@@ -829,15 +844,21 @@
 
     if _type != 'Asset' and _common.present(d, 'Asset'):
         path.append(_common.get(d, 'Asset'))
 
     return _common.path_list_to_string(path)
 
 
-def get_scoped_data_id(d, workbook_id):
+def get_scoped_data_id(d: dict, workbook_id: Optional[str]) -> str:
+    """
+    :param d: The dictionary representing this item.
+    :param workbook_id: The ID of the workbook that the item is scoped to. None or EMPTY_GUID represents global.
+    :return: The generated Data ID representing this item. This is generally in the form of
+             "[workbook_id] {item_type} path >> to >> item".
+    """
     path = determine_path(d)
 
     if not _common.present(d, 'Data ID'):
         if path:
             scoped_data_id = '%s >> %s' % (path, d['Name'])
         else:
             scoped_data_id = d['Name']
```

### Comparing `seeq-spy-188.3/seeq/spy/_metadata_push_results.py` & `seeq-spy-189.0/seeq/spy/_metadata_push_results.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/_plot.py` & `seeq-spy-189.0/seeq/spy/_plot.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/_pull.py` & `seeq-spy-189.0/seeq/spy/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/_push.py` & `seeq-spy-189.0/seeq/spy/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/_redaction.py` & `seeq-spy-189.0/seeq/spy/_redaction.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/_search.py` & `seeq-spy-189.0/seeq/spy/_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,59 +4,72 @@
 import types
 from dataclasses import dataclass
 from typing import List, Dict, Union, Mapping, Optional, Set
 
 import pandas as pd
 
 from seeq import spy
+from seeq.base.seeq_names import SeeqNames
 from seeq.sdk import *
 from seeq.spy import _common, _login, _metadata, _push, _swap
 from seeq.spy._errors import *
 from seeq.spy._redaction import safely, request_safely
 from seeq.spy._session import Session
 from seeq.spy._status import Status
 
 RESERVED_SEARCH_COLUMN_NAMES = ['Path', 'Asset', 'Type', 'Depth', 'Estimated Sample Period', 'Formula Parameters',
                                 'Datasource Name']
 
+ALL_PROPERTIES = ['@allProperties']
+
+DEFAULT_PROPERTIES = ['ID', 'Path', 'Asset', 'Name', 'Description', 'Type', 'Value Unit Of Measure', 'Datasource Name',
+                      'Archived']
+
+USE_DEFAULT_LIMIT = -1
+
 
 @dataclass
 class SearchContext:
     session: Session
     status: Status
 
-    all_properties: bool
+    include_properties: List[str]
     workbook: str
     recursive: bool
     ignore_unindexed_properties: bool
     include_archived: bool
     estimate_sample_period: dict
     include_swap_info: bool
     old_asset_format: bool
     order_by: Optional[Union[str, list]]
+    limit: int
 
     status_index: int
     columns: List[str]
     metadata: List
     ids: Set
     comparison: str
     dupe_count: int
     sample_periods: Dict
     workbook_id: str
     pd_start: Optional[pd.Timestamp]
     pd_end: Optional[pd.Timestamp]
-    use_search_items_api: bool
+    use_search_items_api_for_this_query: bool
+    used_search_items_api_at_least_once: bool
     timer: datetime.datetime
 
     items_api: ItemsApi
     trees_api: TreesApi
     formulas_api: FormulasApi
     displays_api: DisplaysApi
     display_templates_api: DisplayTemplatesApi
 
+    search_by_id_helper_for_all_queries: SearchByIDHelper
+    search_by_id_helper_for_tree_children: SearchByIDHelper
+
     def __init__(self, session: Session, status: Status):
         self.session = session
         self.status = status
 
         self.columns = list()
         self.metadata = list()
         self.ids = set()
@@ -67,19 +80,79 @@
         self.items_api = ItemsApi(session.client)
         self.trees_api = TreesApi(session.client)
         self.formulas_api = FormulasApi(session.client)
         self.displays_api = DisplaysApi(session.client)
         self.display_templates_api = DisplayTemplatesApi(session.client)
 
 
+search_by_id_helper_page_size = 1000
+
+
+class SearchByIDHelper:
+    """
+    In R62 and later, you can supply a list of filters to the search_items API in the form of ID=={ID}. This means we
+    can do far fewer round trips to satisfy a query where the user supplies a DataFrame full of IDs. This class
+    issues search_items() calls in pages and caches the results for retrieval by various parts of the search code.
+    """
+
+    def __init__(self, context: SearchContext, queries: List[dict]):
+        self.context = context
+        self.queries = queries
+        self.page_size = search_by_id_helper_page_size
+        self.current_index = -1
+        self.page = None
+
+    def get_by_index(self, index: int) -> ItemSearchPreviewV1:
+        if index > self.current_index:
+            self._get_next_page_via_search_items()
+
+        return self.page[index]
+
+    def _get_next_page_via_search_items(self):
+        filters = ['@includeUnsearchable']
+        new_current_index = self.current_index
+        while new_current_index < len(self.queries) - 1:
+            new_current_index += 1
+            if not _common.present(self.queries[new_current_index], 'ID'):
+                continue
+
+            filters.append(f"ID=={self.queries[new_current_index]['ID']}")
+
+            if len(filters) > self.page_size:
+                break
+
+        if self.context.session.options.wants_compatibility_with(188):
+            include_properties = ALL_PROPERTIES
+        else:
+            include_properties = self.context.include_properties
+
+        search_results = self.context.items_api.search_items(
+            filters=filters,
+            include_properties=include_properties,
+            limit=self.page_size
+        )
+
+        items = {item.id: item for item in search_results.items}
+        self.page = dict()
+        while self.current_index < new_current_index:
+            self.current_index += 1
+            if not _common.present(self.queries[self.current_index], 'ID'):
+                continue
+
+            self.page[self.current_index] = items.get(self.queries[self.current_index]['ID'])
+
+
 @Status.handle_keyboard_interrupt()
-def search(query, *, all_properties=False, workbook=_common.DEFAULT_WORKBOOK_PATH, recursive=True,
-           ignore_unindexed_properties=True, include_archived=False, include_swappable_assets=False,
-           estimate_sample_period=None, old_asset_format=None, order_by=None, errors=None, quiet=None, status=None,
-           session: Optional[Session] = None):
+def search(query, *, all_properties=False, include_properties: List[str] = None,
+           workbook: Optional[str] = _common.DEFAULT_WORKBOOK_PATH, recursive: bool = True,
+           ignore_unindexed_properties: bool = True, include_archived: bool = False,
+           include_swappable_assets: bool = False, estimate_sample_period: Optional[dict] = None,
+           old_asset_format: bool = None, order_by: Union[str, List[str]] = None,
+           limit: Optional[int] = USE_DEFAULT_LIMIT, errors: str = None, quiet: bool = None, status: Status = None,
+           session: Optional[Session] = None) -> pd.DataFrame:
     """
     Issues a query to the Seeq Server to retrieve metadata for signals,
     conditions, scalars and assets. This metadata can then be used to retrieve
     samples, capsules for a particular time range via spy.pull().
 
     Parameters
     ----------
@@ -128,17 +201,25 @@
                             datasource connector
         Cache Enabled       True to find items where data caching is enabled
         Scoped To           The Seeq ID of a workbook such that results are
                             limited to ONLY items scoped to that workbook.
         =================== ===================================================
 
     all_properties : bool, default False
-        True if all item properties should be retrieved. This currently makes
-        the search operation much slower as retrieval of properties for an item
-        requires a separate call.
+        Return all item properties in the result. If you would like to specify
+        exactly which properties to return (for better performance/less data),
+        use include_properties instead. If both all_properties and
+        include_properties are omitted, you will get only the properties that
+        come "for free" (no performance penalty) with the query.
+
+    include_properties : list, optional
+        A list of extra properties to include in the results. If omitted, the
+        default set of properties will be returned. If both all_properties and
+        include_properties are omitted, you will get only the properties that
+        come "for free" (no performance penalty) with the query.
 
     workbook : {str, None}, default 'Data Lab >> Data Lab Analysis'
         A path string (with ' >> ' delimiters) or an ID to indicate a workbook
         such that, in addition to globally-scoped items, the workbook's scoped
         items will also be returned in the results.
 
         If you want all items regardless of scope, use
@@ -176,38 +257,45 @@
         A dict with the keys 'Start' and 'End'. If provided, an estimated
         sample period for all signals will be included in the output. The
         values for the 'Start' and 'End' keys must be a string that
         pandas.to_datetime() can parse, or a pandas.Timestamp. The start
         and end times are used to bound the calculation of the sample period.
         If the start and end times encompass a time range that is insufficient
         to determine the sample period, a pd.NaT will be returned.
-        If the value of 'Start' is set to None, it will default to the value of
-        'End' minus 1 hour. Conversely, if the value of 'End' is set to None,
-        it will default to now.
+        If the value of 'Start' is set to None, it will default to the value
+        of 'End' minus 1 hour. Conversely, if the value of 'End' is set to
+        None, it will default to now.
 
     old_asset_format : bool, default True
-        Historically, spy.search() returned rows with a "Type" of "Asset" whereby
-        the "Asset" column was the name of the parent asset. This is inconsistent
-        with all other aspects of SPy, including spy.push(metadata). If you would
-        like Asset rows to instead be consistent with the rest of SPy (whereby
-        the "Asset" column is the name of the current asset, not the parent),
-        pass in False for this argument.
+        Historically, spy.search() returned rows with a "Type" of "Asset"
+        whereby the "Asset" column was the name of the parent asset. This is
+        inconsistent with all other aspects of SPy, including
+        spy.push(metadata). If you would like Asset rows to instead be
+        consistent with the rest of SPy (whereby the "Asset" column is the
+        name of the current asset, not the parent), pass in False for this
+        argument.
 
     order_by : {str, list}, default None
         An optional field or list of fields used to sort the search results.
-        Fields on which results can be sorted are 'ID', 'Name', and 'Description'.
+        Fields on which results can be sorted are 'ID', 'Name', and
+        'Description'.
+
+    limit : int, default 1000
+        A limit on the number of results returned. By default, the limit is
+        1000. Specify limit=None to return all results.
 
     quiet : bool, default False
         If True, suppresses progress output. Note that when status is
         provided, the quiet setting of the Status object that is passed
         in takes precedence.
 
     errors : {'raise', 'catalog'}, default 'raise'
-        If 'raise', any errors encountered will cause an exception. If 'catalog',
-        errors will be added to a 'Result' column in the status.df DataFrame.
+        If 'raise', any errors encountered will cause an exception. If
+        'catalog', errors will be added to a 'Result' column in the status.df
+        DataFrame.
 
     status : spy.Status, optional
         If specified, the supplied Status object will be updated as the command
         progresses. It gets filled in with the same information you would see
         in Jupyter in the blue/green/red table below your code while the
         command is executed. The table itself is accessible as a DataFrame via
         the status.df property.
@@ -245,16 +333,17 @@
 
     >>> search_results = spy.search({'Name': 'Humid', 'Path': 'Example >> Cooling Tower 1'}, all_properties=True)
 
     To access the stored properties:
     >>> search_results.spy.kwargs
     >>> search_results.spy.status
 
-    Search for signals that have a name that starts with 'Area' in the datasource 'Example Data' and
-    determine the sample period of each signal during the month of January 2018
+    Search for signals that have a name that starts with 'Area' in the
+    datasource 'Example Data' and determine the sample period of each signal
+    during the month of January 2018
 
     >>> search_results = spy.search({
     >>>    'Name': 'Area ?_*',
     >>>    'Datasource Name': 'Example Data'
     >>> }, estimate_sample_period=dict(Start='2018-01-01', End='2018-02-01'))
 
     Using a pandas.DataFrame as the input:
@@ -269,43 +358,70 @@
     >>> my_worksheet_items = spy.search(
     >>> 'https://seeq.com/workbook/17F31703-F0B6-4C8E-B7FD-E20897BD4819/worksheet/CE6A0B92-EE00-45FC-9EB3-D162632DBB48')
 
     """
     input_args = _common.validate_argument_types([
         (query, 'query', (str, dict, list, pd.DataFrame, pd.Series)),
         (all_properties, 'all_properties', bool),
+        (include_properties, 'include_properties', list),
         (workbook, 'workbook', str),
         (recursive, 'recursive', bool),
         (ignore_unindexed_properties, 'ignore_unindexed_properties', bool),
         (include_archived, 'include_archived', bool),
         (estimate_sample_period, 'estimate_sample_period', dict),
         (include_swappable_assets, 'include_swappable_assets', bool),
         (old_asset_format, 'old_asset_format', bool),
         (order_by, 'order_by', (str, list)),
+        (limit, 'limit', int),
         (quiet, 'quiet', bool),
         (errors, 'errors', str),
         (status, 'status', Status),
         (session, 'session', Session)
     ])
 
     status = Status.validate(status, quiet, errors)
     session = Session.validate(session)
     _login.validate_login(session, status)
 
+    if all_properties:
+        if include_properties is not None:
+            status.warn(f'If you specify all_properties=True, the include_properties argument is ignored.')
+        include_properties = ALL_PROPERTIES.copy()
+
     context = SearchContext(session, status)
-    context.all_properties = all_properties
     context.workbook = workbook
     context.recursive = recursive
     context.ignore_unindexed_properties = ignore_unindexed_properties
     context.include_archived = include_archived
     context.estimate_sample_period = estimate_sample_period
     context.include_swap_info = include_swappable_assets
     context.old_asset_format = old_asset_format
     context.order_by = order_by
 
+    if limit != USE_DEFAULT_LIMIT:
+        context.limit = limit
+    elif session.options.wants_compatibility_with(188):
+        # In v188 and earlier, there was no limiting capability.
+        context.limit = None
+    else:
+        # In v189 and later, we apply a default limit of 1000 to reduce the likelihood of a user accidentally running
+        # a search that returns a huge number of results.
+        context.limit = 1000
+
+    context.columns = ['ID', 'Type']
+    if include_properties is not None and include_properties != ALL_PROPERTIES:
+        context.columns.extend(include_properties)
+
+    context.include_properties = include_properties if include_properties is not None else list()
+
+    # The SPy user knows the formula parameters property as "Formula Parameters", but the backend knows it as
+    # "FormulaParameters". So just convert it here to keep things consistent for the SPy user.
+    context.include_properties = [p.replace('Formula Parameters', SeeqNames.Properties.formula_parameters)
+                                  for p in context.include_properties]
+
     if context.order_by:
         context.order_by = _validate_order_by(context.order_by)
 
     if context.estimate_sample_period is not None:
         if context.estimate_sample_period.keys() != {'Start', 'End'}:  # strict comparison, allowing only these two keys
             raise SPyValueError(f"estimate_sample_period must have 'Start' and 'End' keys but got "
                                 f"{context.estimate_sample_period.keys()}")
@@ -357,98 +473,99 @@
             search_df = spy.workbooks.search(search_query,
                                              status=context.status.create_inner('Find Workbook', quiet=True),
                                              session=context.session)
             context.workbook_id = search_df.iloc[0]['ID'] if len(search_df) > 0 else None
             if context.workbook == _common.DEFAULT_WORKBOOK_PATH and context.workbook_id is None:
                 context.workbook_id = _common.GLOBALS_ONLY
 
-    context.use_search_items_api = False
+    context.search_by_id_helper_for_all_queries = SearchByIDHelper(context, queries)
 
-    for status_index in range(len(queries)):
-        context.status_index = status_index
-        _process_query(context, queries[status_index])
+    context.used_search_items_api_at_least_once = False
+
+    try:
+        for status_index in range(len(queries)):
+            context.status_index = status_index
+            _process_query(context, queries[status_index])
+    except StopIteration:
+        status.warn(f'Search results limited to {context.limit}. Supply increased "limit" parameter to return more.')
 
     if context.dupe_count > 0:
-        if context.use_search_items_api:
-            arg_to_use = context.order_by if context.order_by else []
+        if context.used_search_items_api_at_least_once:
+            arg_to_use = context.order_by if context.order_by is not None else list()
             if 'ID' in arg_to_use:
                 context.status.warn(
                     f'{context.dupe_count} duplicates removed from returned DataFrame. If you used a list of '
                     f'searches, those searches may have had overlap.')
             else:
                 arg_to_use.append('ID')
                 context.status.warn(
                     f'{context.dupe_count} duplicates removed from returned DataFrame. Use order_by={arg_to_use} in '
                     f'your spy.search to ensure results are not missing any items.')
         else:
             context.status.warn(f'{context.dupe_count} duplicates removed from returned DataFrame.')
 
     context.status.update('Query successful', Status.SUCCESS)
 
-    if len(context.columns) == 0:
-        context.columns = ['ID', 'Type']
-    output_df = pd.DataFrame(data=context.metadata, columns=context.columns)
+    # We want the default properties to always appear first and in a certain order, so we make a final_column_set
+    # list, add in the additional properties, and then filter any absent properties from the final list
+    final_column_set = DEFAULT_PROPERTIES.copy()
+    final_column_set += [c for c in context.columns if c not in final_column_set]
+    final_column_set = [c for c in final_column_set if c in context.columns]
+    output_df = pd.DataFrame(data=context.metadata, columns=final_column_set)
+
     if context.order_by and not output_df.empty:
         output_df.sort_values(context.order_by, ignore_index=True, inplace=True)
 
     if old_asset_format is None:
         type_column = output_df['Type']
         if len(type_column.loc[type_column == 'Asset']) > 0:
             context.status.warn(
                 'This search result includes Assets. Consider passing in "old_asset_format=False" so that the '
                 '"Path" and "Asset" columns are populated in a way that is consistent with all other aspects '
                 'of SPy. The default behavior without this argument emulates the (incorrect) way SPy would '
                 'return such results historically.')
-            context.status.display()
 
     output_df_properties = types.SimpleNamespace(
         func='spy.search',
         kwargs=input_args,
         old_asset_format=context.old_asset_format,
         status=context.status)
 
     _common.put_properties_on_df(output_df, output_df_properties)
 
     return output_df
 
 
 def _process_query(context: SearchContext, current_query):
+    """
+    Called for each query "row" in the list of queries
+    """
     context.timer = _common.timer_start()
 
     if _common.present(current_query, 'ID'):
+        context.search_by_id_on_this_query = True
+
         # If ID is specified, short-circuit everything and just get the item directly.
-        prop_dict = dict()
         current_id = current_query['ID']
-        _add_all_properties(context, current_id, prop_dict)
-
-        # Since this method bypasses the search_items() route that would normally supply the asset ancestors, we
-        # specifically call _add_tree() to make the trees_api call that will fetch the ancestors.
-        _add_tree(context, current_id, prop_dict)
-
-        # Still need to determine sample period for signals and have NaT for non-signal items
-        if context.estimate_sample_period is not None:
-            if 'Signal' in current_query['Type']:
-                _estimate_sample_period(context, current_id, prop_dict['Name'])
-            else:
-                context.sample_periods[current_query['ID']] = pd.NaT
-
-            _add_to_dict(
-                context, prop_dict, 'Estimated Sample Period', context.sample_periods[current_query['ID']])
-
+        prop_dict = _create_prop_dict(context, current_id)
         _add_to_metadata(context, prop_dict)
 
         context.status.df.at[context.status_index, 'Time'] = _common.timer_elapsed(context.timer)
         context.status.df.at[context.status_index, 'Count'] = 1
         context.status.df.at[context.status_index, 'Result'] = 'Success'
         return
 
+    context.search_by_id_on_this_query = False
+
     # If the user wants a recursive search or there's no 'Path' in the query, then use the ItemsApi.search_items API
-    context.use_search_items_api = context.recursive or not _common.present(current_query, 'Path')
+    context.use_search_items_api_for_this_query = context.recursive or not _common.present(current_query, 'Path')
+    context.used_search_items_api_at_least_once = (context.used_search_items_api_at_least_once or
+                                                   context.use_search_items_api_for_this_query)
 
-    if not context.use_search_items_api and context.include_archived:
+    if not context.use_search_items_api_for_this_query and context.include_archived:
         # As you can see in the code below, the TreesApi.get_tree() API doesn't have the ability to request
         # archived items
         raise SPyValueError('include_archived=True can only be used with recursive searches or searches that do '
                             'not involve a Path parameter')
 
     allowed_properties = ['Type', 'Name', 'Description', 'Path', 'Asset', 'Datasource Class', 'Datasource ID',
                           'Datasource Name', 'Data ID', 'Cache Enabled', 'Scoped To']
@@ -533,22 +650,22 @@
                 filters.append('Datasource Class == %s' % _common.get(current_query, 'Datasource Class'))
 
             filter_list = [' && '.join(filters)]
             if context.include_archived:
                 filter_list.append('@includeUnsearchable')
 
             datasource_results = context.items_api.search_items(
-                filters=filter_list, types=['Datasource'], limit=100000)  # type: ItemSearchPreviewPaginatedListV1
+                filters=filter_list, types=['Datasource'], limit=100000)
 
             if len(datasource_results.items) > 1:
                 raise SPyRuntimeError('Multiple datasources found that match "%s"' % datasource_name)
             elif len(datasource_results.items) == 0:
                 raise SPyRuntimeError('No datasource found that matches "%s"' % datasource_name)
 
-            datasource = datasource_results.items[0]  # type: ItemSearchPreviewV1
+            datasource = datasource_results.items[0]
 
             @request_safely(action_description=f'get datasource details for "{datasource_name}" {datasource.id}',
                             status=context.status)
             def request_datasource_and_set_clause():
                 property_output = context.items_api.get_property(id=datasource.id, property_name='Datasource Class')
                 clauses['Datasource Class'] = ('==', property_output.value)
                 property_output = context.items_api.get_property(id=datasource.id, property_name='Datasource ID')
@@ -564,18 +681,26 @@
         filters.append(' && '.join([p + c + v for p, (c, v) in clauses.items()]))
 
     if context.include_archived:
         filters.append('@includeUnsearchable')
 
     kwargs = {
         'filters': filters,
-        'types': item_types,
-        'limit': context.session.options.search_page_size
+        'types': item_types
     }
 
+    if context.limit is None:
+        kwargs['limit'] = context.session.options.search_page_size
+    else:
+        # If the user supplied a limit argument, then use it (if it's smaller than the page size)
+        kwargs['limit'] = min(context.session.options.search_page_size, context.limit)
+
+    if context.include_properties is not None and _login.is_sdk_module_version_at_least(62):
+        kwargs['include_properties'] = context.include_properties
+
     if context.workbook:
         if context.workbook_id:
             kwargs['scope'] = context.workbook_id
         elif context.workbook != _common.DEFAULT_WORKBOOK_PATH:
             raise SPyRuntimeError(f'Workbook "{context.workbook}" not found, or is not accessible by you')
 
     if _common.present(current_query, 'Scoped To'):
@@ -605,19 +730,186 @@
             _gather_results(context, current_query, kwargs, list())
         else:
             _process_query_path_string(context, current_query, kwargs, path_to_query, list(), clauses)
 
     context.status.df.at[context.status_index, 'Result'] = 'Success'
 
 
-def _validate_order_by(order_by):
+def _gather_results(context: SearchContext, current_query, kwargs, actual_path_list=None):
+    """
+    Once we're at the appropriate depth in the tree, we can gather the results. If we're not doing a tree-based
+    query, then we just search at the top level.
+    """
+    if context.use_search_items_api_for_this_query:
+        _iterate_over_output(context, _do_search, 'items', _gather_results_via_item_search, current_query,
+                             kwargs, actual_path_list)
+    else:
+        _iterate_over_output(context, _do_search, 'children', _gather_results_via_get_tree, current_query,
+                             kwargs, actual_path_list)
+
+
+# noinspection PyUnusedLocal
+def _iterate_over_output(context: SearchContext, _output_func, _collection_name, _action_func, current_query,
+                         kwargs, _actual_path_list):
+    """
+    Handles pagination for the various ways that we need to churn through results.
+    """
+    offset = 0
+    while True:
+        output = _output_func(context, kwargs, offset)
+
+        collection = getattr(output, _collection_name)
+
+        context.status.df.at[context.status_index, 'Time'] = _common.timer_elapsed(context.timer)
+        context.status.df.at[context.status_index, 'Count'] = offset + len(collection)
+        context.status.df.at[context.status_index, 'Pages'] += 1
+        context.status.df.at[context.status_index, 'Result'] = 'Querying'
+        context.status.update('Querying Seeq Server for items', Status.RUNNING)
+
+        for item in collection:
+            _action_func(context, current_query, _actual_path_list, item)
+
+        if len(collection) != output.limit:
+            break
+
+        offset += output.limit
+
+
+def _do_search(context: SearchContext, kwargs: dict, offset):
+    """
+    Executes an actual search. Sometimes this uses the SearchItems API, sometimes it uses the GetTree API.
+    """
+    kwargs['offset'] = offset
+    if 'scope' in kwargs and isinstance(kwargs['scope'], str):
+        kwargs['scope'] = [kwargs['scope']]
+    if context.use_search_items_api_for_this_query:
+        if context.order_by:
+            kwargs['order_by'] = context.order_by
+        return context.items_api.search_items(**kwargs)
+
+    kwargs2 = {
+        'offset': kwargs['offset'],
+        'limit': kwargs['limit'],
+        'scope': _common.get(kwargs, 'scope'),
+        'exclude_globally_scoped': ('@excludeGloballyScoped' in kwargs['filters'])
+    }
+
+    if 'asset' in kwargs:
+        kwargs2['id'] = kwargs['asset']
+        tree_output = context.trees_api.get_tree(**kwargs2)
+    else:
+        tree_output = context.trees_api.get_tree_root_nodes(**kwargs2)
+    if len(kwargs['types']) > 0:
+        tree_output.children = [x for x in tree_output.children if x.type in kwargs['types']]
+
+    # This will speed up retrieval of properties in R62 and later
+    for i in range(len(tree_output.children)):
+        # Plant an index on the child object so we can find it later
+        setattr(tree_output.children[i], 'child_index', i)
+
+    # Create a SearchByIDHelper that will be called (in R62 and later) if we need to retrieve extra properties for the
+    # child. This case only happens when performing a tree-based query with recursive=False.
+    context.search_by_id_helper_for_tree_children = SearchByIDHelper(context, [{'ID': child.id} for child in
+                                                                               tree_output.children])
+
+    return tree_output
+
+
+# noinspection PyUnusedLocal
+def _gather_results_via_item_search(context: SearchContext, current_query, actual_path_list,
+                                    result: ItemSearchPreviewV1):
+    item_search_preview: ItemSearchPreviewV1 = result
+    prop_dict = _create_prop_dict(context, item_search_preview)
+    _add_to_metadata(context, prop_dict)
+
+
+def _gather_results_via_get_tree(context: SearchContext, current_query, actual_path_list, result):
+    tree_item_output: TreeItemOutputV1 = result
+
+    for prop, _attr in [('Name', 'name'), ('Description', 'description')]:
+        if prop not in current_query:
+            continue
+
+        if not _common.does_query_fragment_match(current_query[prop],
+                                                 getattr(tree_item_output, _attr),
+                                                 contains=(context.comparison == '~=')):
+            return
+
+    prop_dict = _create_prop_dict(context, tree_item_output)
+
+    _add_ancestors_to_prop_dict(
+        context, tree_item_output.type, tree_item_output.name, actual_path_list, prop_dict)
+
+    _add_to_metadata(context, prop_dict)
+
+
+def _create_prop_dict(context: SearchContext, item: Union[str, TreeItemOutputV1, ItemSearchPreviewV1]):
+    """
+    Each individual search result row is represented by a dictionary. This function creates that dictionary,
+    and handles the various permutations of types that we might encounter.
+    """
+
+    def _add_error_message_and_warn(msg):
+        _add_to_dict(context, prop_dict, 'Pull Result', msg)
+        context.status.warn(msg)
+
+    item_id = item if isinstance(item, str) else item.id
+
+    prop_dict = dict()
+
+    @request_safely(action_description=f'get included item properties for {item_id}',
+                    status=context.status,
+                    on_error=_add_error_message_and_warn)
+    def _request_item_properties():
+        output_object = _add_properties_smartly(context, item, prop_dict)
+
+        if output_object.type in ['CalculatedSignal', 'CalculatedCondition', 'CalculatedScalar', 'LiteralScalar']:
+            formula_parameters = None
+            if _login.is_sdk_module_version_at_least(62):
+                formula_parameters = output_object.parameters
+            elif (_has_requested_property(context, 'Formula') or
+                  _has_requested_property(context, 'FormulaParameters')):
+                # Formula isn't always included in the output (in this R61-and-earlier-case), and Formula Parameters
+                # is never included. So we have to make a separate request.
+                formula_output = context.formulas_api.get_item(id=output_object.id)
+                if _has_requested_property(context, 'Formula'):
+                    _add_to_dict(context, prop_dict, 'Formula', formula_output.formula)
+                formula_parameters = formula_output.parameters
+
+            if formula_parameters is not None and _has_requested_property(context, 'FormulaParameters'):
+                _add_to_dict(context, prop_dict, 'Formula Parameters', [
+                    '%s=%s' % (_p.name, _p.item.id if _p.item else _p.formula) for _p in formula_parameters
+                ])
+
+        elif output_object.type == 'ThresholdMetric':
+            formula_parameters = _metadata.formula_parameters_dict_from_threshold_metric(
+                context.session, output_object.id)
+            for key, value in formula_parameters.items():
+                _add_to_dict(context, prop_dict, key, value)
+
+        elif output_object.type == 'Display':
+            display_output = context.displays_api.get_display(id=output_object.id)
+            _add_to_dict(context, prop_dict, 'Template ID', display_output.template.id)
+            if display_output.swap is not None:
+                _add_to_dict(context, prop_dict, 'Swap Out Asset ID', display_output.swap.swap_out)
+                _add_to_dict(context, prop_dict, 'Swap In Asset ID', display_output.swap.swap_in)
+            else:
+                _add_to_dict(context, prop_dict, 'Swap Out Asset ID', display_output.template.swap_source_asset_id)
+
+        elif output_object.type == 'DisplayTemplate':
+            display_template_output = context.display_templates_api.get_display_template(id=output_object.id)
+            _add_to_dict(context, prop_dict, 'Source Workstep ID', display_template_output.source_workstep_id)
+
+    _request_item_properties()
+    return prop_dict
+
+
+def _validate_order_by(order_by: Union[str, List[str]]) -> List[str]:
     """
     Validate and process order_by arg of spy.search
-    :param order_by: {str, list}
-    :return: list
     """
     # convert string order_by to a list
     if isinstance(order_by, str):
         order_by = [order_by]
 
     # validate order_by
     order_fields = ['ID', 'Name', 'Description']
@@ -626,119 +918,228 @@
         raise SPyValueError(
             f"Invalid order_by fields: {invalid_fields}. Search results can only be ordered on "
             f"{order_fields} fields.")
 
     return order_by
 
 
-def _add_to_dict(context: SearchContext, _dict, key, val):
+def _add_properties_smartly(context: SearchContext,
+                            item: Union[str, TreeItemOutputV1, ItemSearchPreviewV1],
+                            prop_dict: dict):
+    # This function does a bunch of heavy lifting to handle the differences in how properties are returned
+    # in different versions of the SDK.
+    #
+    # R62 and later:   Extra properties are returned in ItemSearchPreviewV1 objects
+    # R61 and earlier: Extra properties must be fetched in a separate request
+
+    # The following two variables will be filled in if we find that we already had them or needed them to fulfill the
+    # user's request.
+    item_search_preview: Optional[ItemSearchPreviewV1] = None
+    item_output: Optional[ItemOutputV1] = None
+
+    # This is the variable that we use to grab all the default/common properties
+    item_object: Union[ItemSearchPreviewV1, ItemOutputV1] = item
+
+    if isinstance(item, str):
+        if _login.is_sdk_module_version_at_least(62):
+            item_search_preview = context.search_by_id_helper_for_all_queries.get_by_index(context.status_index)
+            item_object = item_search_preview
+        else:
+            # This does not need to be wrapped in request_safely because it is only called from a safe place in
+            # _create_prop_dict()
+            item_output = context.items_api.get_item_and_all_properties(id=item)
+            item_object = item_output
+    elif isinstance(item, ItemSearchPreviewV1):
+        item_search_preview = item
+
+    _add_if_available(context, prop_dict, 'ID', item_object, 'id')
+    _add_if_available(context, prop_dict, 'Name', item_object, 'name')
+    _add_if_available(context, prop_dict, 'Description', item_object, 'description')
+    _add_if_available(context, prop_dict, 'Type', item_object, 'type')
+    _add_if_available(context, prop_dict, 'Archived', item_object, 'is_archived')
+    _add_if_available(context, prop_dict, 'Scoped To', item_object, 'scoped_to')
+
+    if hasattr(item_object, 'value_unit_of_measure'):
+        if item_object.value_unit_of_measure is None and hasattr(item_object, 'source_value_unit_of_measure'):
+            uom = item_object.source_value_unit_of_measure
+        else:
+            uom = item_object.value_unit_of_measure
+
+        _add_to_dict(context, prop_dict, 'Value Unit Of Measure', uom)
+    elif item_output is not None:
+        value_unit_of_measure = [p.value for p in item_output.properties if p.name == 'Value Unit Of Measure']
+        source_value_unit_of_measure = [p.value for p in item_output.properties
+                                        if p.name == 'Source Value Unit Of Measure']
+        if len(value_unit_of_measure) == 0 and len(source_value_unit_of_measure) == 1:
+            uom = source_value_unit_of_measure[0]
+        elif len(value_unit_of_measure) == 1:
+            uom = value_unit_of_measure[0]
+        else:
+            uom = None
+
+        _add_to_dict(context, prop_dict, 'Value Unit Of Measure', uom)
+
+    if _has_requested_property(context, 'Source Value Unit Of Measure'):
+        _add_if_available(context, prop_dict, 'Source Value Unit Of Measure', item_object,
+                          'source_value_unit_of_measure')
+
+    if hasattr(item_object, 'datasource'):
+        datasource_item_preview: ItemPreviewV1 = item_object.datasource
+        _add_to_dict(context, prop_dict, 'Datasource Name',
+                     datasource_item_preview.name if datasource_item_preview else None)
+
+    if hasattr(item_object, 'ancestors'):
+        _add_ancestors_to_prop_dict_from_item_output(context, item_object, prop_dict)
+
+    if context.include_swap_info or (
+            not hasattr(item_object, 'ancestors') and
+            (_has_requested_property(context, 'Path') or _has_requested_property(context, 'Asset'))
+    ):
+        _retrieve_ancestors_and_swap_info(context, item_object.id, prop_dict)
+
+    if context.estimate_sample_period is not None:
+        _estimate_sample_period(context, item_object)
+        _add_to_dict(context, prop_dict, 'Estimated Sample Period', context.sample_periods[item_object.id])
+
+    # Check if we need any more properties. If we don't, we can avoid more API calls.
+    need_more_properties = False
+    if isinstance(item, str) and context.session.options.wants_compatibility_with(188):
+        need_more_properties = True
+    else:
+        for prop in context.include_properties:
+            if prop not in prop_dict:
+                need_more_properties = True
+                break
+
+    if not need_more_properties:
+        return item_object
+
+    if _login.is_sdk_module_version_at_least(62):
+        if item_search_preview is None and isinstance(item, TreeItemOutputV1):
+            item_search_preview = context.search_by_id_helper_for_tree_children.get_by_index(
+                getattr(item, 'child_index'))
+
+        for prop in item_search_preview.included_properties.values():  # type: ScalarPropertyV1
+            _add_included_property_to_dict(context, prop_dict, prop.name, prop.value)
+    else:
+        if item_output is None:
+            # This does not need to be wrapped in request_safely because it is only called from a safe place in
+            # _create_prop_dict()
+            item_output = context.items_api.get_item_and_all_properties(id=item_object.id)
+
+        for prop in item_output.properties:  # type: PropertyOutputV1
+            _add_included_property_to_dict(context, prop_dict, prop.name, prop.value)
+
+    return item_object
+
+
+def _add_included_property_to_dict(context: SearchContext, prop_dict: dict, prop_name: str, prop_value: object):
+    if prop_name in RESERVED_SEARCH_COLUMN_NAMES:
+        return
+
+    if not context.session.options.wants_compatibility_with(188) and not _has_requested_property(context, prop_name):
+        return
+
+    _add_to_dict(context, prop_dict, prop_name, prop_value)
+
+
+def _add_if_available(context: SearchContext, prop_dict: dict, key: str, obj: object, attr: str):
+    if hasattr(obj, attr):
+        _add_to_dict(context, prop_dict, key, getattr(obj, attr))
+
+
+def _add_to_dict(context: SearchContext, prop_dict: dict, key: str, val: object):
+    if context.session.options.wants_compatibility_with(188):
+        # In v188 and earlier, all scalar properties on items were returned as strings from
+        # items_api.get_item_and_all_properties(). So for scripts that are expecting that, cast it to a string.
+        val = str(val)
+
+    elif key.endswith('Unit Of Measure') and val == '':
+        # This property is returned as None in ItemSearchPreviewV1.value_unit_of_measure, but as an empty string in
+        # the ItemSearchPreviewV1.included_properties. Normalize to None in v189 and later.
+        val = None
+
     if key in ['Archived', 'Cache Enabled', 'Enabled', 'Unsearchable'] and isinstance(val, str):
         val = val.lower() == 'true'
-    _dict[key] = _common.none_to_nan(val)
+
+    prop_dict[key] = _common.none_to_nan(val)
 
     # We want the columns to appear in a certain order (the order we added them in) for readability
     if key not in context.columns:
         context.columns.append(key)
 
 
-def _add_ancestors_to_prop_dict_from_item_output(context: SearchContext, item_output, prop_dict):
+def _add_ancestors_to_prop_dict_from_item_output(context: SearchContext, item_output, prop_dict: dict):
     _ancestors = [a.name for a in item_output.ancestors]
     _add_ancestors_to_prop_dict(context, item_output.type, item_output.name, _ancestors, prop_dict)
 
 
-def _add_ancestors_to_prop_dict(context: SearchContext, _type, name, ancestors, prop_dict):
-    _common.add_ancestors_to_definition(_type, name, ancestors, prop_dict, context.old_asset_format)
+def _add_ancestors_to_prop_dict(context: SearchContext, item_type: str, name: str, ancestors: list, prop_dict: dict):
+    _common.add_ancestors_to_definition(item_type, name, ancestors, prop_dict, context.old_asset_format)
     for key in ['Path', 'Asset']:
         if key in prop_dict and key not in context.columns:
             context.columns.append(key)
 
 
-def _add_to_metadata(context: SearchContext, prop_dict):
+def _add_to_metadata(context: SearchContext, prop_dict: dict):
     if prop_dict['ID'] not in context.ids:
+        if len(context.metadata) == context.limit:
+            raise StopIteration()
+
         context.metadata.append(prop_dict)
         context.ids.add(prop_dict['ID'])
     else:
         context.dupe_count += 1
 
 
-def _estimate_sample_period(context: SearchContext, signal_id, signal_name):
+def _estimate_sample_period(context: SearchContext, item: Union[TreeItemOutputV1, ItemSearchPreviewV1]):
+    if 'Signal' not in item.type:
+        context.sample_periods[item.id] = pd.NaT
+        return
+
+    if item.id in context.sample_periods:
+        # Already done
+        return
+
     sampling_formula = "$signal.estimateSamplePeriod(" \
                        f"capsule('{context.pd_start.isoformat()}','{context.pd_end.isoformat()}'))"
 
     formula_run_output = safely(
-        lambda: context.formulas_api.run_formula(formula=sampling_formula, parameters=[f"signal={signal_id}"]),
+        lambda: context.formulas_api.run_formula(formula=sampling_formula, parameters=[f"signal={item.id}"]),
         action_description='estimate sample period',
         status=context.status,
         additional_errors=[400])
 
     if formula_run_output is not None and formula_run_output.scalar.value is not None:
-        context.sample_periods[signal_id] = pd.to_timedelta(
+        context.sample_periods[item.id] = pd.to_timedelta(
             formula_run_output.scalar.value, unit=formula_run_output.scalar.uom)
     else:
         context.status.warn(
-            f'Could not determine the sample period for signal "{signal_name}" {signal_id} within the '
+            f'Could not determine the sample period for signal "{item.name}" {item.id} within the '
             f'time period {context.pd_start.isoformat()} to {context.pd_end.isoformat()}. '
             f'There might not be enough data in the specified time range. Modify the time period with the '
             f'`estimate_start` and `estimate_end` arguments.'
         )
-        context.sample_periods[signal_id] = pd.NaT
+        context.sample_periods[item.id] = pd.NaT
 
 
-def _add_all_properties(context: SearchContext, _id, prop_dict):
-    def _add_error_message_and_warn(msg):
-        _add_to_dict(context, prop_dict, 'Pull Result', msg)
-        context.status.warn(msg)
-
-    @request_safely(action_description=f'get all item properties for {_id}',
-                    status=context.status,
-                    on_error=_add_error_message_and_warn)
-    def _request_item_properties():
-        item = context.items_api.get_item_and_all_properties(id=_id)  # type: ItemOutputV1
-        # Name and Type don't appear in additional properties
-        _add_to_dict(context, prop_dict, 'Name', item.name)
-        _add_to_dict(context, prop_dict, 'Type', item.type)
-        _add_to_dict(context, prop_dict, 'Scoped To', _common.none_to_nan(item.scoped_to))
-        for prop in item.properties:  # type: PropertyOutputV1
-            if prop.name not in RESERVED_SEARCH_COLUMN_NAMES:
-                _add_to_dict(context, prop_dict, prop.name, prop.value)
-
-        if item.type in ['CalculatedSignal', 'CalculatedCondition', 'CalculatedScalar', 'LiteralScalar']:
-            formula_output = context.formulas_api.get_item(id=_id)  # type: FormulaItemOutputV1
-            _add_to_dict(context, prop_dict, 'Formula Parameters', [
-                '%s=%s' % (_p.name, _p.item.id if _p.item else _p.formula) for _p in formula_output.parameters
-            ])
-
-        elif item.type == 'ThresholdMetric':
-            formula_parameters = _metadata.formula_parameters_dict_from_threshold_metric(context.session, _id)
-            for key, value in formula_parameters.items():
-                _add_to_dict(context, prop_dict, key, value)
+def _has_requested_property(context: SearchContext, prop_name: str) -> bool:
+    return prop_name in context.include_properties or context.include_properties == ALL_PROPERTIES
 
-        elif item.type == 'Display':
-            display_output = context.displays_api.get_display(id=_id)
-            _add_to_dict(context, prop_dict, 'Template ID', display_output.template.id)
-            if display_output.swap is not None:
-                _add_to_dict(context, prop_dict, 'Swap Out Asset ID', display_output.swap.swap_out)
-                _add_to_dict(context, prop_dict, 'Swap In Asset ID', display_output.swap.swap_in)
-            else:
-                _add_to_dict(context, prop_dict, 'Swap Out Asset ID', display_output.template.swap_source_asset_id)
-
-        elif item.type == 'DisplayTemplate':
-            display_template_output = context.display_templates_api.get_display_template(id=_id)
-            _add_to_dict(context, prop_dict, 'Source Workstep ID', display_template_output.source_workstep_id)
 
-    _request_item_properties()
-    return prop_dict
-
-
-def _add_tree(context: SearchContext, _id, prop_dict):
+def _retrieve_ancestors_and_swap_info(context: SearchContext, item_id: str, prop_dict: dict):
+    """
+    This function tries to economically retrieve ancestors and swap information if necessary.
+    """
     item_output = None
     if context.include_swap_info:
-        item_dependency_output = safely(lambda: context.items_api.get_formula_dependencies(id=_id),
-                                        action_description=f'get dependencies for {_id}',
-                                        status=context.status)  # type: ItemDependencyOutputV1
+        item_dependency_output: ItemDependencyOutputV1 = safely(
+            lambda: context.items_api.get_formula_dependencies(id=item_id),
+            action_description=f'get dependencies for {item_id}',
+            status=context.status)
         if item_dependency_output is not None:
             item_output = item_dependency_output
 
         dependencies_with_relevant_assets = _swap.get_swappable_assets(item_dependency_output)
 
         def _swappable_asset_dict(d):
             leaf_asset = d.ancestors[-1]
@@ -750,195 +1151,85 @@
             }
 
         swappable_assets = pd.DataFrame([_swappable_asset_dict(d) for d in dependencies_with_relevant_assets],
                                         columns=['ID', 'Type', 'Path', 'Asset'])
 
         _add_to_dict(context, prop_dict, 'Swappable Assets', swappable_assets)
     else:
-        asset_tree_output = safely(lambda: context.trees_api.get_tree(id=_id),
-                                   action_description=f'get asset tree ancestors for {_id}',
-                                   status=context.status)  # type: AssetTreeOutputV1
+        asset_tree_output: AssetTreeOutputV1 = safely(lambda: context.trees_api.get_tree(id=item_id),
+                                                      action_description=f'get asset tree ancestors for {item_id}',
+                                                      status=context.status)
         if asset_tree_output is not None:
             item_output = asset_tree_output.item
+
     if item_output is not None:
         _add_ancestors_to_prop_dict_from_item_output(context, item_output, prop_dict)
 
     return prop_dict
 
 
 def _process_query_path_string(context: SearchContext, current_query, kwargs, remaining_query_path_string,
                                actual_path_list, clauses: dict, asset_id=None):
+    """
+    Walks down an asset path and processes each level, including wildcards and regexes.
+    """
     query_path_list = _common.path_string_to_list(remaining_query_path_string)
 
     query_path_part = query_path_list[0]
 
     tree_kwargs = dict()
     tree_kwargs['limit'] = kwargs['limit']
     tree_kwargs['offset'] = 0
 
     if 'scope' in kwargs and isinstance(kwargs['scope'], str):
         tree_kwargs['scope'] = [kwargs['scope']]
 
     while True:
+        tree_output: AssetTreeOutputV1
         if not asset_id:
-            tree_output = context.trees_api.get_tree_root_nodes(**tree_kwargs)  # type: AssetTreeOutputV1
+            tree_output = context.trees_api.get_tree_root_nodes(**tree_kwargs)
         else:
             tree_kwargs['id'] = asset_id
-            tree_output = context.trees_api.get_tree(**tree_kwargs)  # type: AssetTreeOutputV1
+            tree_output = context.trees_api.get_tree(**tree_kwargs)
 
         for child in tree_output.children:  # type: TreeItemOutputV1
+            if not _common.does_query_fragment_match(query_path_part, child.name, contains=False):
+                continue
+
             if not asset_id:
                 @request_safely(action_description=f'check if "{child.name}" {child.id} has '
                                                    f'datasource matching request',
                                 status=context.status,
                                 default_value=True)
                 def _is_item_in_filter_datasources():
-                    child_item_output = context.items_api.get_item_and_all_properties(
-                        id=child.id)  # type: ItemOutputV1
+                    child_item_output = context.items_api.get_item_and_all_properties(id=child.id)
                     for prop in ['Datasource Class', 'Datasource ID']:
                         if prop in clauses:
                             _, val = clauses[prop]
                             p_list = [_p.value for _p in child_item_output.properties if
                                       _p.name == prop]
                             if len(p_list) == 0 or p_list[0] != val:
                                 return False
                     return True
 
                 # We only filter out datasource at the top level, in case the tree is mixed
                 if not _is_item_in_filter_datasources():
                     continue
 
-            if _common.does_query_fragment_match(query_path_part, child.name, contains=False):
-                actual_path_list_for_child = actual_path_list.copy()
-                actual_path_list_for_child.append(child.name)
-                if len(query_path_list) == 1:
-                    kwargs['asset'] = child.id
-                    _gather_results(context, current_query, kwargs, actual_path_list=actual_path_list_for_child)
-                else:
-                    _process_query_path_string(context,
-                                               current_query,
-                                               kwargs,
-                                               _common.path_list_to_string(query_path_list[1:]),
-                                               actual_path_list_for_child,
-                                               clauses,
-                                               child.id)
+            actual_path_list_for_child = actual_path_list.copy()
+            actual_path_list_for_child.append(child.name)
+            if len(query_path_list) == 1:
+                kwargs['asset'] = child.id
+                _gather_results(context, current_query, kwargs, actual_path_list=actual_path_list_for_child)
+            else:
+                _process_query_path_string(context,
+                                           current_query,
+                                           kwargs,
+                                           _common.path_list_to_string(query_path_list[1:]),
+                                           actual_path_list_for_child,
+                                           clauses,
+                                           child.id)
 
         if len(tree_output.children) < tree_kwargs['limit']:
             break
 
         tree_kwargs['offset'] += tree_kwargs['limit']
-
-
-# noinspection PyUnusedLocal
-def _gather_results_via_item_search(context: SearchContext, current_query, _actual_path_list, _result):
-    item_search_preview = _result  # type: ItemSearchPreviewV1
-    prop_dict = dict()
-
-    _add_ancestors_to_prop_dict_from_item_output(context, item_search_preview, prop_dict)
-
-    uom = item_search_preview.value_unit_of_measure if item_search_preview.value_unit_of_measure \
-        else item_search_preview.source_value_unit_of_measure
-    _add_to_dict(context, prop_dict, 'Value Unit Of Measure', uom)
-    datasource_item_preview = item_search_preview.datasource  # type: ItemPreviewV1
-    _add_to_dict(context, prop_dict, 'Datasource Name',
-                 datasource_item_preview.name if datasource_item_preview else None)
-    _add_common_properties(context, prop_dict, item_search_preview)
-
-
-def _gather_results_via_get_tree(context: SearchContext, current_query, _actual_path_list, _result):
-    tree_item_output = _result  # type: TreeItemOutputV1
-    prop_dict = dict()
-
-    for prop, _attr in [('Name', 'name'), ('Description', 'description')]:
-        if prop not in current_query:
-            continue
-
-        if not _common.does_query_fragment_match(current_query[prop],
-                                                 getattr(tree_item_output, _attr),
-                                                 contains=(context.comparison == '~=')):
-            return
-
-    _add_ancestors_to_prop_dict(
-        context, tree_item_output.type, tree_item_output.name, _actual_path_list, prop_dict)
-
-    _add_to_dict(context, prop_dict, 'Value Unit Of Measure', tree_item_output.value_unit_of_measure)
-    _add_common_properties(context, prop_dict, tree_item_output)
-
-
-def _add_common_properties(context: SearchContext, prop_dict, output_object):
-    _add_to_dict(context, prop_dict, 'ID', output_object.id)
-    _add_to_dict(context, prop_dict, 'Name', output_object.name)
-    _add_to_dict(context, prop_dict, 'Description', output_object.description)
-    _add_to_dict(context, prop_dict, 'Type', output_object.type)
-    _add_to_dict(context, prop_dict, 'Archived', output_object.is_archived)
-    if context.all_properties:
-        _add_all_properties(context, output_object.id, prop_dict)
-    if context.include_swap_info:
-        _add_tree(context, output_object.id, prop_dict)
-    if context.estimate_sample_period is not None:
-        _add_to_dict(context, prop_dict, 'Estimated Sample Period',
-                     context.sample_periods[output_object.id])
-    _add_to_metadata(context, prop_dict)
-
-
-def _iterate_over_output(context: SearchContext, _output_func, _collection_name, _action_func, current_query,
-                         kwargs, _actual_path_list):
-    offset = 0
-    while True:
-        output = _output_func(context, kwargs, offset)
-
-        collection = getattr(output, _collection_name)
-        # Determine sample period for all signals and have NaT for non-signal items
-        if context.estimate_sample_period is not None:
-            for item in collection:
-                if 'Signal' in item.type:
-                    _estimate_sample_period(context, item.id, item.name)
-                else:
-                    context.sample_periods[item.id] = pd.NaT
-
-        context.status.df.at[context.status_index, 'Time'] = _common.timer_elapsed(context.timer)
-        context.status.df.at[context.status_index, 'Count'] = offset + len(collection)
-        context.status.df.at[context.status_index, 'Pages'] += 1
-        context.status.df.at[context.status_index, 'Result'] = 'Querying'
-        context.status.update('Querying Seeq Server for items', Status.RUNNING)
-
-        for item in collection:
-            _action_func(context, current_query, _actual_path_list, item)
-
-        if len(collection) != output.limit:
-            break
-
-        offset += output.limit
-
-
-def _do_search(context: SearchContext, kwargs: dict, offset):
-    kwargs['offset'] = offset
-    if 'scope' in kwargs and isinstance(kwargs['scope'], str):
-        kwargs['scope'] = [kwargs['scope']]
-    if context.use_search_items_api:
-        if context.order_by:
-            kwargs['order_by'] = context.order_by
-        return context.items_api.search_items(**kwargs)
-
-    kwargs2 = {
-        'offset': kwargs['offset'],
-        'limit': kwargs['limit'],
-        'scope': _common.get(kwargs, 'scope'),
-        'exclude_globally_scoped': ('@excludeGloballyScoped' in kwargs['filters'])
-    }
-    if 'asset' in kwargs:
-        kwargs2['id'] = kwargs['asset']
-        tree_output = context.trees_api.get_tree(**kwargs2)
-    else:
-        tree_output = context.trees_api.get_tree_root_nodes(**kwargs2)
-    if len(kwargs['types']) > 0:
-        tree_output.children = [x for x in tree_output.children if x.type in kwargs['types']]
-    return tree_output
-
-
-def _gather_results(context: SearchContext, current_query, kwargs, actual_path_list=None):
-    if context.use_search_items_api:
-        _iterate_over_output(context, _do_search, 'items', _gather_results_via_item_search, current_query, kwargs,
-                             actual_path_list)
-    else:
-        _iterate_over_output(context, _do_search, 'children', _gather_results_via_get_tree, current_query, kwargs,
-                             actual_path_list)
```

### Comparing `seeq-spy-188.3/seeq/spy/_session.py` & `seeq-spy-189.0/seeq/spy/_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import textwrap
 from dataclasses import dataclass
 from typing import Optional, List
 
 import pytz
 import requests
 from dateutil.tz import tz
+
 from seeq import spy
 from seeq.sdk import *
 from seeq.sdk.configuration import ClientConfiguration
 from seeq.spy import _url, _common, _datalab, _errors
 from seeq.spy._errors import *
 
 SEEQ_SDK_RETRY_TIMEOUT_IN_SECONDS_ENV_VAR_NAME = 'SEEQ_SDK_RETRY_TIMEOUT_IN_SECONDS'
@@ -457,14 +458,17 @@
                 the timezone of any timezone-aware datetime. If set to None, naive
                 datetimes will be interpreted as being in the logged-in user's preferred
                 timezone. Timezone can be specified as str, pytz.timezone or dateutil.tzinfo.
         """
 
         _common.print_output(textwrap.dedent(help_string))
 
+    def wants_compatibility_with(self, major_version):
+        return self.compatibility is not None and self.compatibility <= major_version
+
 
 @dataclass(repr=False)
 class SqAuthRequests:
     session: Session
 
     def add_request_kwargs(self, d):
         if 'cookies' not in d:
```

### Comparing `seeq-spy-188.3/seeq/spy/_status.py` & `seeq-spy-189.0/seeq/spy/_status.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,14 +125,17 @@
                         del kwargs[kwarg]
 
                 try:
                     return func(*args, **kwargs)
                 except KeyboardInterrupt as e:
                     kwargs['status'].update('Operation canceled', Status.CANCELED)
                     raise SPyKeyboardInterrupt(e)
+                finally:
+                    # Ensures that any warnings that are added at the end of an operation are still displayed
+                    kwargs['status'].display()
 
             return out
 
         return decorator
 
     def _drain_updates(self):
         while True:
@@ -260,16 +263,20 @@
         # noinspection PyTypeChecker
         display(text)
 
         return new_message
 
     def display(self):
         """
-        Force the Status object to output its HTML-based display to the Notebook or the console
+        Force the Status object to output its HTML-based display to the Notebook or the console. Note that this will
+        still honor the quiet flag and effectively do nothing if quiet is True.
         """
+        if self._skip_display() or self.message is None:
+            return
+
         if not _common.display_supports_html():
             self.message = self._display_text(self.message)
         else:
             self.message = self._display_html(self.message)
 
     def _display_html(self, new_message):
         _common.ipython_clear_output(wait=True)
```

### Comparing `seeq-spy-188.3/seeq/spy/_swap.py` & `seeq-spy-189.0/seeq/spy/_swap.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/_upgrade.py` & `seeq-spy-189.0/seeq/spy/_upgrade.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/_url.py` & `seeq-spy-189.0/seeq/spy/_url.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/acl/_pull.py` & `seeq-spy-189.0/seeq/spy/acl/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/acl/_push.py` & `seeq-spy-189.0/seeq/spy/acl/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/addons/_install.py` & `seeq-spy-189.0/seeq/spy/addons/_install.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/addons/_permissions.py` & `seeq-spy-189.0/seeq/spy/addons/_permissions.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/addons/_search.py` & `seeq-spy-189.0/seeq/spy/addons/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/addons/_uninstall.py` & `seeq-spy-189.0/seeq/spy/addons/_uninstall.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/assets/_brochure.py` & `seeq-spy-189.0/seeq/spy/assets/_brochure.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/assets/_build.py` & `seeq-spy-189.0/seeq/spy/assets/_build.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/assets/_context.py` & `seeq-spy-189.0/seeq/spy/assets/_context.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/assets/_model.py` & `seeq-spy-189.0/seeq/spy/assets/_model.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/assets/_trees/_constants.py` & `seeq-spy-189.0/seeq/spy/assets/_trees/_constants.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/assets/_trees/_csv.py` & `seeq-spy-189.0/seeq/spy/assets/_trees/_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,16 @@
         df_no_ids.drop(columns=['ID'], inplace=True)
 
     # which of the options the csv has:
     search_cols = [x for x in _search_options if x in df_no_ids.columns]
 
     try:
         search_res = _search.search(
-            df_no_ids[search_cols], old_asset_format=True, order_by=["ID"], workbook=workbook, quiet=True
+            df_no_ids[search_cols], old_asset_format=True, order_by=["ID"], limit=None,
+            workbook=workbook, quiet=True
         )[['Name', 'ID']]
     except KeyError:
         if len(df_with_ids) == 0:
             message = f"No items were found with the specified names: {list(df_no_ids['Name'])}"
             status.exception(SPyValueError(message), throw=True)
         else:
             status.warn(f"The following names did not return search results and were "
```

### Comparing `seeq-spy-188.3/seeq/spy/assets/_trees/_match.py` & `seeq-spy-189.0/seeq/spy/assets/_trees/_match.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/assets/_trees/_pandas.py` & `seeq-spy-189.0/seeq/spy/assets/_trees/_pandas.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/assets/_trees/_path.py` & `seeq-spy-189.0/seeq/spy/assets/_trees/_path.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/assets/_trees/_properties.py` & `seeq-spy-189.0/seeq/spy/assets/_trees/_properties.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/assets/_trees/_pull.py` & `seeq-spy-189.0/seeq/spy/assets/_trees/_pull.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,16 @@
     # Get all children of the requested asset
     @request_safely(
         action_description='pull children of node',
         status=status)
     def get_search_results():
         return _search.search(query={'Asset': node_id}, all_properties=True,
                               workbook=_get_search_workbook(session, node_id, workbook_id),
-                              old_asset_format=True, order_by=['ID'], quiet=True, session=session)
+                              old_asset_format=True, order_by=['ID'], limit=None,
+                              quiet=True, session=session)
 
     search_results = get_search_results()
     if search_results is None or len(search_results) == 0:
         return df
 
     if item_ids_to_ignore is not None:
         search_results = search_results[~search_results['ID'].isin(item_ids_to_ignore)]
@@ -243,15 +244,16 @@
             if _row_is_spy_tree_root(row, spy_tree.id, spy_tree.name):
                 if df_root_id is None:
                     df_root_id = row['ID']
                 else:
                     return None
     if df_root_id is not None:
         existing_tree_df = _search.search([{'ID': df_root_id}, {'Asset': df_root_id}], workbook=workbook_id,
-                                          old_asset_format=True, order_by=['ID'], quiet=True, session=session)
+                                          old_asset_format=True, order_by=['ID'], limit=None,
+                                          quiet=True, session=session)
         existing_tree_df['Path'] = existing_tree_df.apply(_path.determine_path, axis=1)
         if 'Datasource Name' not in existing_tree_df.columns:
             existing_tree_df['Datasource Name'] = np.nan
         existing_tree_df = existing_tree_df[['ID', 'Path', 'Name', 'Type', 'Datasource Name']]
         return existing_tree_df
     else:
         return None
```

### Comparing `seeq-spy-188.3/seeq/spy/assets/_trees/_tree.py` & `seeq-spy-189.0/seeq/spy/assets/_trees/_tree.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/assets/_trees/_utils.py` & `seeq-spy-189.0/seeq/spy/assets/_trees/_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/assets/_trees/_validate.py` & `seeq-spy-189.0/seeq/spy/assets/_trees/_validate.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/assets/brochure.html` & `seeq-spy-189.0/seeq/spy/assets/brochure.html`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Administration/User Migration.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Administration/User Migration.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997474747474747%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(7, 'spy.options.compatibility = 189')], delete: [7]}}}"}*

```diff
@@ -23,15 +23,15 @@
                 "from collections import namedtuple\n",
                 "\n",
                 "from pandas import DataFrame\n",
                 "\n",
                 "from seeq import sdk, spy\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Authentication\n",
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998724489795918%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(5, 'spy.options.compatibility = 189')], delete: [5]}}}"}*

```diff
@@ -7,15 +7,15 @@
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "\n",
                 "from seeq import spy\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# Parameterized Jobs\n",
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999473905723906%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'spy.options.compatibility = 189')], delete: [4]}}}"}*

```diff
@@ -7,15 +7,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
                 "import pandas as pd\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "logical-skill",
             "metadata": {},
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999007936507937%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'spy.options.compatibility = 189')], delete: [4]}}}"}*

```diff
@@ -6,15 +6,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
                 "import pandas as pd\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999810606060606%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'spy.options.compatibility = 189')], delete: [4]}}}"}*

```diff
@@ -10,15 +10,15 @@
             },
             "outputs": [],
             "source": [
                 "import numpy as np\n",
                 "from seeq import spy\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "pycharm": {
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998468137254901%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(6, 'spy.options.compatibility = 189')], delete: [6]}}}"}*

```diff
@@ -9,15 +9,15 @@
             "source": [
                 "import os\n",
                 "from seeq import spy\n",
                 "import pandas as pd\n",
                 "import numpy as np\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "usual-insulation",
             "metadata": {},
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Command Reference.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Command Reference.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/Example Export.zip` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/Example Export.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Tutorial.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Tutorial.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996323529411765%*

 * *Differences: {"'cells'": "{4: {'source': ['spy.options.compatibility = 189']}}"}*

```diff
@@ -41,15 +41,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "You'll also want to import Pandas so that you can work with the DataFrame structures that the **spy** library consumes/produces."
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Version Considerations.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Version Considerations.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997916666666666%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(3, 'spy.options.compatibility = 189\\n')], delete: [3]}}}"}*

```diff
@@ -80,15 +80,15 @@
                     ]
                 }
             ],
             "source": [
                 "from seeq import spy\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188\n",
+                "spy.options.compatibility = 189\n",
                 "\n",
                 "# Login so we can check the Seeq Server version\n",
                 "spy.login(url='http://localhost:34216', credentials_file='../credentials.key', force=False)\n",
                 "\n",
                 "# Check the SPy version\n",
                 "print(f'SPy is at least 184.3? {spy.utils.is_spy_module_version_at_least(184, 3)}')\n",
                 "print(f'Seeq Server is at least R73.3.1? {spy.utils.is_server_version_at_least(73, 3, 1)}')"
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/Workbook Templates.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/Workbook Templates.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999210858585859%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'spy.options.compatibility = 189')], delete: [4]}}}"}*

```diff
@@ -11,15 +11,15 @@
             },
             "outputs": [],
             "source": [
                 "import pandas as pd\n",
                 "from seeq import spy\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "f4146468",
             "metadata": {
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.acl.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.acl.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999780701754386%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'spy.options.compatibility = 189')], delete: [4]}}}"}*

```diff
@@ -6,15 +6,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
                 "import pandas as pd\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.jobs.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.jobs.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997222222222222%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'spy.options.compatibility = 189')], delete: [4]}}}"}*

```diff
@@ -6,15 +6,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
                 "import pandas as pd\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# spy.jobs\n",
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.login.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.login.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996428571428572%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(3, 'spy.options.compatibility = 189')], delete: [3]}}}"}*

```diff
@@ -9,15 +9,15 @@
                 }
             },
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# spy.login\n",
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.pull.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.pull.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999094202898551%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'spy.options.compatibility = 189')], delete: [4]}}}"}*

```diff
@@ -6,15 +6,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
                 "import pandas as pd\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.push.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.push.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999905303030303%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'spy.options.compatibility = 189')], delete: [4]}}}"}*

```diff
@@ -6,15 +6,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
                 "import pandas as pd\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.search.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.search.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9946314102564102%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'spy.options.compatibility = 189')], delete: [4]}}, 7: "*

 * *            "{'source': {insert: [(2, '`spy.search()` only returns a subset of item properties as "*

 * *            'can be seen in the output above. If you want to retrieve all properties, use '*

 * *            '`all_properties=True`. Note that when interfacing with Seeq Server version R61 and '*

 * *            'earlier, this can be an expensive (slow) operation for queries that return many rows. '*

 * *            "In R62 an […]*

```diff
@@ -6,15 +6,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
                 "import pandas as pd\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
@@ -282,15 +282,15 @@
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Retrieving all properties\n",
                 "\n",
-                "`spy.search()` only returns a subset of item properties as can be seen in the output above. If you want to retrieve all properties, use `all_properties=True`. Note that this can be an expensive (slow) operation for queries that return many rows."
+                "`spy.search()` only returns a subset of item properties as can be seen in the output above. If you want to retrieve all properties, use `all_properties=True`. Note that when interfacing with Seeq Server version R61 and earlier, this can be an expensive (slow) operation for queries that return many rows. In R62 and later, this query has been optimized to be much faster."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 4,
             "metadata": {},
             "outputs": [
@@ -414,14 +414,21 @@
                 "}, all_properties=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
+                "You can also use the `include_properties=['Property Name 1', 'Property Name 2']` argument if you want to explicitly return certain properties."
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
                 "## Estimating signal sample period\n",
                 "The `estimate_sample_period` parameter adds an `Estimated Sample Period` column with a value for each signal \n",
                 "returned in search query for a specified time frame."
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.swap.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.swap.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998511904761904%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'spy.options.compatibility = 189')], delete: [4]}}}"}*

```diff
@@ -6,15 +6,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
                 "import pandas as pd\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.widgets.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.widgets.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997826086956522%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(3, 'spy.options.compatibility = 189')], delete: [3]}}}"}*

```diff
@@ -9,15 +9,15 @@
                 }
             },
             "outputs": [],
             "source": [
                 "from seeq import spy\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {
                 "pycharm": {
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.workbooks.ipynb` & `seeq-spy-189.0/seeq/spy/docs/Documentation/spy.workbooks.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998883928571429%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(5, 'spy.options.compatibility = 189')], delete: [5]}}}"}*

```diff
@@ -7,15 +7,15 @@
             "outputs": [],
             "source": [
                 "import os\n",
                 "import shutil\n",
                 "from seeq import spy\n",
                 "\n",
                 "# Set the compatibility option so that you maximize the chance that SPy will remain compatible with your notebook/script\n",
-                "spy.options.compatibility = 188"
+                "spy.options.compatibility = 189"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 2,
             "metadata": {},
             "outputs": [
```

### Comparing `seeq-spy-188.3/seeq/spy/docs/_copy.py` & `seeq-spy-189.0/seeq/spy/docs/_copy.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/jobs/_execute.py` & `seeq-spy-189.0/seeq/spy/jobs/_execute.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/jobs/_pull.py` & `seeq-spy-189.0/seeq/spy/jobs/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/jobs/_push.py` & `seeq-spy-189.0/seeq/spy/jobs/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/jobs/_schedule.py` & `seeq-spy-189.0/seeq/spy/jobs/_schedule.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/notifications/_emails.py` & `seeq-spy-189.0/seeq/spy/notifications/_emails.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/utils/__init__.py` & `seeq-spy-189.0/seeq/spy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/widgets/_ipy_utils.py` & `seeq-spy-189.0/seeq/spy/widgets/_ipy_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/widgets/_widgets.py` & `seeq-spy-189.0/seeq/spy/widgets/_widgets.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/__init__.py` & `seeq-spy-189.0/seeq/spy/workbooks/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_annotation.py` & `seeq-spy-189.0/seeq/spy/workbooks/_annotation.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_content.py` & `seeq-spy-189.0/seeq/spy/workbooks/_content.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_data.py` & `seeq-spy-189.0/seeq/spy/workbooks/_data.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_folder.py` & `seeq-spy-189.0/seeq/spy/workbooks/_folder.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_item.py` & `seeq-spy-189.0/seeq/spy/workbooks/_item.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_item_map.py` & `seeq-spy-189.0/seeq/spy/workbooks/_item_map.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_load.py` & `seeq-spy-189.0/seeq/spy/workbooks/_load.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_mustache.py` & `seeq-spy-189.0/seeq/spy/workbooks/_mustache.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_pull.py` & `seeq-spy-189.0/seeq/spy/workbooks/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_push.py` & `seeq-spy-189.0/seeq/spy/workbooks/_push.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
         kwargs=input_args,
         input=workbooks,
         output=new_workbooks,
         datasource=datasource_output,
         item_map=item_map,
         status=status)
 
-    output_df = status.df
+    output_df = status.df.copy()
 
     _common.put_properties_on_df(output_df, output_df_properties)
 
     return output_df
 
 
 def _create_folder_path_if_necessary(session: Session, path, status: Status):
```

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_render.py` & `seeq-spy-189.0/seeq/spy/workbooks/_render.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_report_content_utilities.py` & `seeq-spy-189.0/seeq/spy/workbooks/_report_content_utilities.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_save.py` & `seeq-spy-189.0/seeq/spy/workbooks/_save.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_search.py` & `seeq-spy-189.0/seeq/spy/workbooks/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_template.py` & `seeq-spy-189.0/seeq/spy/workbooks/_template.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_user.py` & `seeq-spy-189.0/seeq/spy/workbooks/_user.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_workbook.py` & `seeq-spy-189.0/seeq/spy/workbooks/_workbook.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_worksheet.py` & `seeq-spy-189.0/seeq/spy/workbooks/_worksheet.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/_workstep.py` & `seeq-spy-189.0/seeq/spy/workbooks/_workstep.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq/spy/workbooks/app.css` & `seeq-spy-189.0/seeq/spy/workbooks/app.css`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/seeq_spy.egg-info/PKG-INFO` & `seeq-spy-189.0/seeq_spy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 188.3
+Version: 189.0
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-spy-188.3/seeq_spy.egg-info/SOURCES.txt` & `seeq-spy-189.0/seeq_spy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.3/setup.py` & `seeq-spy-189.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seeq-spy",
-    version="188.3",
+    version="189.0",
     author="Seeq Corporation",
     author_email="support@seeq.com",
     description="Easy-to-use Python interface for Seeq",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.seeq.com",
     project_urls={
```

