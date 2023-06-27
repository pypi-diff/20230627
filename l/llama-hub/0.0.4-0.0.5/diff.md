# Comparing `tmp/llama_hub-0.0.4.tar.gz` & `tmp/llama_hub-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_hub-0.0.4.tar", max compression
+gzip compressed data, was "llama_hub-0.0.5.tar", max compression
```

## Comparing `llama_hub-0.0.4.tar` & `llama_hub-0.0.5.tar`

### file list

```diff
@@ -1,455 +1,464 @@
--rw-r--r--   0        0        0     1064 2023-04-18 06:55:56.425923 llama_hub-0.0.4/LICENSE
--rw-r--r--   0        0        0     6505 2023-05-31 00:19:23.700889 llama_hub-0.0.4/README.md
--rw-r--r--   0        0        0      247 2023-05-31 00:19:23.701017 llama_hub-0.0.4/llama_hub/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.701087 llama_hub-0.0.4/llama_hub/__init__.py
--rwxr-xr-x   0        0        0      119 2023-05-31 00:19:23.701156 llama_hub-0.0.4/llama_hub/add_loader.sh
--rw-r--r--   0        0        0      826 2023-05-31 00:19:23.701312 llama_hub-0.0.4/llama_hub/airtable/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.701382 llama_hub-0.0.4/llama_hub/airtable/__init__.py
--rw-r--r--   0        0        0      901 2023-05-31 00:19:23.701488 llama_hub-0.0.4/llama_hub/airtable/base.py
--rw-r--r--   0        0        0       10 2023-05-31 00:19:23.701580 llama_hub-0.0.4/llama_hub/airtable/requirements.txt
--rw-r--r--   0        0        0     1839 2023-05-31 00:19:23.701803 llama_hub-0.0.4/llama_hub/apify/actor/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.701871 llama_hub-0.0.4/llama_hub/apify/actor/__init__.py
--rw-r--r--   0        0        0     2474 2023-05-31 00:19:23.702257 llama_hub-0.0.4/llama_hub/apify/actor/base.py
--rw-r--r--   0        0        0       13 2023-05-31 00:19:23.702389 llama_hub-0.0.4/llama_hub/apify/actor/requirements.txt
--rw-r--r--   0        0        0     1499 2023-05-31 00:19:23.702551 llama_hub-0.0.4/llama_hub/apify/dataset/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.702623 llama_hub-0.0.4/llama_hub/apify/dataset/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-31 00:19:23.702732 llama_hub-0.0.4/llama_hub/apify/dataset/base.py
--rw-r--r--   0        0        0       13 2023-05-31 00:19:23.702829 llama_hub-0.0.4/llama_hub/apify/dataset/requirements.txt
--rw-r--r--   0        0        0      778 2023-05-31 00:19:23.702978 llama_hub-0.0.4/llama_hub/asana/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.703048 llama_hub-0.0.4/llama_hub/asana/__init__.py
--rw-r--r--   0        0        0     1856 2023-05-31 00:19:23.703120 llama_hub-0.0.4/llama_hub/asana/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.703184 llama_hub-0.0.4/llama_hub/asana/requirements.txt
--rw-r--r--   0        0        0     2200 2023-05-31 00:19:23.703343 llama_hub-0.0.4/llama_hub/azcognitive_search/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.703413 llama_hub-0.0.4/llama_hub/azcognitive_search/__init__.py
--rw-r--r--   0        0        0     2080 2023-05-31 00:19:23.703514 llama_hub-0.0.4/llama_hub/azcognitive_search/base.py
--rw-r--r--   0        0        0       37 2023-05-31 00:19:23.703715 llama_hub-0.0.4/llama_hub/azcognitive_search/requirements.txt
--rw-r--r--   0        0        0     2542 2023-05-31 00:19:23.703897 llama_hub-0.0.4/llama_hub/azstorage_blob/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.703969 llama_hub-0.0.4/llama_hub/azstorage_blob/__init__.py
--rw-r--r--   0        0        0     5419 2023-05-31 00:19:23.704197 llama_hub-0.0.4/llama_hub/azstorage_blob/base.py
--rw-r--r--   0        0        0       34 2023-05-31 00:19:23.704302 llama_hub-0.0.4/llama_hub/azstorage_blob/requirements.txt
--rw-r--r--   0        0        0     1077 2023-05-31 00:19:23.704450 llama_hub-0.0.4/llama_hub/bilibili/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.704513 llama_hub-0.0.4/llama_hub/bilibili/__init__.py
--rw-r--r--   0        0        0     2374 2023-05-31 00:19:23.704590 llama_hub-0.0.4/llama_hub/bilibili/base.py
--rw-r--r--   0        0        0       21 2023-05-31 00:19:23.704655 llama_hub-0.0.4/llama_hub/bilibili/requirements.txt
--rw-r--r--   0        0        0     3373 2023-05-31 00:19:23.705017 llama_hub-0.0.4/llama_hub/boarddocs/BoardDocsReader.ipynb
--rw-r--r--   0        0        0     1402 2023-05-31 00:19:23.705098 llama_hub-0.0.4/llama_hub/boarddocs/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.705155 llama_hub-0.0.4/llama_hub/boarddocs/__init__.py
--rw-r--r--   0        0        0     4430 2023-05-31 00:19:23.705233 llama_hub-0.0.4/llama_hub/boarddocs/base.py
--rw-r--r--   0        0        0    19752 2023-05-31 00:19:23.705373 llama_hub-0.0.4/llama_hub/boarddocs/crawl.ipynb
--rw-r--r--   0        0        0       22 2023-05-31 00:19:23.705450 llama_hub-0.0.4/llama_hub/boarddocs/requirements.txt
--rw-r--r--   0        0        0      921 2023-05-31 00:19:23.705605 llama_hub-0.0.4/llama_hub/chatgpt_plugin/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.705665 llama_hub-0.0.4/llama_hub/chatgpt_plugin/__init__.py
--rw-r--r--   0        0        0     2111 2023-05-31 00:19:23.705774 llama_hub-0.0.4/llama_hub/chatgpt_plugin/base.py
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.705804 llama_hub-0.0.4/llama_hub/chatgpt_plugin/requirements.txt
--rw-r--r--   0        0        0     1056 2023-05-31 00:19:23.705957 llama_hub-0.0.4/llama_hub/chroma/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.705990 llama_hub-0.0.4/llama_hub/chroma/__init__.py
--rw-r--r--   0        0        0     1918 2023-05-31 00:19:23.706083 llama_hub-0.0.4/llama_hub/chroma/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.706141 llama_hub-0.0.4/llama_hub/chroma/requirements.txt
--rw-r--r--   0        0        0     2309 2023-06-24 06:49:58.684812 llama_hub-0.0.4/llama_hub/confluence/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.706342 llama_hub-0.0.4/llama_hub/confluence/__init__.py
--rw-r--r--   0        0        0    11807 2023-06-24 06:49:58.684999 llama_hub-0.0.4/llama_hub/confluence/base.py
--rw-r--r--   0        0        0       80 2023-05-31 00:19:23.706544 llama_hub-0.0.4/llama_hub/confluence/requirements.txt
--rw-r--r--   0        0        0     1052 2023-05-31 00:19:23.706689 llama_hub-0.0.4/llama_hub/couchdb/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.706764 llama_hub-0.0.4/llama_hub/couchdb/__init__.py
--rw-r--r--   0        0        0     2564 2023-05-31 00:19:23.706867 llama_hub-0.0.4/llama_hub/couchdb/base.py
--rw-r--r--   0        0        0        9 2023-05-31 00:19:23.706940 llama_hub-0.0.4/llama_hub/couchdb/requirements.txt
--rw-r--r--   0        0        0      582 2023-05-31 00:19:23.707023 llama_hub-0.0.4/llama_hub/dad_jokes/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.707074 llama_hub-0.0.4/llama_hub/dad_jokes/__init__.py
--rw-r--r--   0        0        0      715 2023-05-31 00:19:23.707121 llama_hub-0.0.4/llama_hub/dad_jokes/base.py
--rw-r--r--   0        0        0     1259 2023-05-31 00:19:23.707209 llama_hub-0.0.4/llama_hub/database/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.707265 llama_hub-0.0.4/llama_hub/database/__init__.py
--rw-r--r--   0        0        0     3328 2023-05-31 00:19:23.707352 llama_hub-0.0.4/llama_hub/database/base.py
--rw-r--r--   0        0        0     1096 2023-05-31 00:19:23.707478 llama_hub-0.0.4/llama_hub/deeplake/README.md
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.707559 llama_hub-0.0.4/llama_hub/deeplake/__init__.py
--rw-r--r--   0        0        0     3457 2023-05-31 00:19:23.707661 llama_hub-0.0.4/llama_hub/deeplake/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.707752 llama_hub-0.0.4/llama_hub/deeplake/requirements.txt
--rw-r--r--   0        0        0      851 2023-05-31 00:19:23.707833 llama_hub-0.0.4/llama_hub/discord/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.707879 llama_hub-0.0.4/llama_hub/discord/__init__.py
--rw-r--r--   0        0        0     4650 2023-05-31 00:19:23.707939 llama_hub-0.0.4/llama_hub/discord/base.py
--rw-r--r--   0        0        0       10 2023-05-31 00:19:23.707985 llama_hub-0.0.4/llama_hub/discord/requirements.txt
--rw-r--r--   0        0        0     4153 2023-05-31 00:19:23.708074 llama_hub-0.0.4/llama_hub/docugami/README.md
--rw-r--r--   0        0        0        4 2023-05-31 00:19:23.708125 llama_hub-0.0.4/llama_hub/docugami/__init__.py
--rw-r--r--   0        0        0    12075 2023-05-31 00:19:23.708201 llama_hub-0.0.4/llama_hub/docugami/base.py
--rw-r--r--   0        0        0    65833 2023-05-31 00:19:23.708412 llama_hub-0.0.4/llama_hub/docugami/docugami.ipynb
--rw-r--r--   0        0        0       20 2023-05-31 00:19:23.708465 llama_hub-0.0.4/llama_hub/docugami/requirements.txt
--rw-r--r--   0        0        0     1042 2023-05-31 00:19:23.708545 llama_hub-0.0.4/llama_hub/elasticsearch/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.708572 llama_hub-0.0.4/llama_hub/elasticsearch/__init__.py
--rw-r--r--   0        0        0     2301 2023-05-31 00:19:23.708639 llama_hub-0.0.4/llama_hub/elasticsearch/base.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.708699 llama_hub-0.0.4/llama_hub/elasticsearch/requirements.txt
--rw-r--r--   0        0        0     1319 2023-05-31 00:19:23.708825 llama_hub-0.0.4/llama_hub/faiss/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.708885 llama_hub-0.0.4/llama_hub/faiss/__init__.py
--rw-r--r--   0        0        0     2126 2023-05-31 00:19:23.708943 llama_hub-0.0.4/llama_hub/faiss/base.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.708986 llama_hub-0.0.4/llama_hub/faiss/requirements.txt
--rw-r--r--   0        0        0      585 2023-05-31 00:19:23.709108 llama_hub-0.0.4/llama_hub/feedly_rss/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.709136 llama_hub-0.0.4/llama_hub/feedly_rss/__init__.py
--rw-r--r--   0        0        0     2100 2023-05-31 00:19:23.709219 llama_hub-0.0.4/llama_hub/feedly_rss/base.py
--rw-r--r--   0        0        0       13 2023-05-31 00:19:23.709288 llama_hub-0.0.4/llama_hub/feedly_rss/requirements.txt
--rw-r--r--   0        0        0     2829 2023-05-31 00:19:23.709504 llama_hub-0.0.4/llama_hub/file/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.709559 llama_hub-0.0.4/llama_hub/file/__init__.py
--rw-r--r--   0        0        0      858 2023-05-31 00:19:23.709669 llama_hub-0.0.4/llama_hub/file/audio/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.709737 llama_hub-0.0.4/llama_hub/file/audio/__init__.py
--rw-r--r--   0        0        0     1486 2023-05-31 00:19:23.709814 llama_hub-0.0.4/llama_hub/file/audio/base.py
--rw-r--r--   0        0        0       20 2023-05-31 00:19:23.709874 llama_hub-0.0.4/llama_hub/file/audio/requirements.txt
--rw-r--r--   0        0        0     1241 2023-05-31 00:19:23.710011 llama_hub-0.0.4/llama_hub/file/audio_gladia/README.md
--rw-r--r--   0        0        0       19 2023-05-31 00:19:23.710082 llama_hub-0.0.4/llama_hub/file/audio_gladia/__init__.py
--rw-r--r--   0        0        0     3274 2023-05-31 00:19:23.710177 llama_hub-0.0.4/llama_hub/file/audio_gladia/base.py
--rw-r--r--   0        0        0       20 2023-05-31 00:19:23.710239 llama_hub-0.0.4/llama_hub/file/audio_gladia/requirements.txt
--rw-r--r--   0        0        0     5552 2023-05-31 00:19:23.710436 llama_hub-0.0.4/llama_hub/file/base.py
--rw-r--r--   0        0        0     1069 2023-05-31 00:19:23.710517 llama_hub-0.0.4/llama_hub/file/cjk_pdf/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.710563 llama_hub-0.0.4/llama_hub/file/cjk_pdf/__init__.py
--rw-r--r--   0        0        0     2584 2023-05-31 00:19:23.710634 llama_hub-0.0.4/llama_hub/file/cjk_pdf/base.py
--rw-r--r--   0        0        0       12 2023-05-31 00:19:23.710693 llama_hub-0.0.4/llama_hub/file/cjk_pdf/requirements.txt
--rw-r--r--   0        0        0      800 2023-05-31 00:19:23.710812 llama_hub-0.0.4/llama_hub/file/deepdoctection/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.710846 llama_hub-0.0.4/llama_hub/file/deepdoctection/__init__.py
--rw-r--r--   0        0        0     1188 2023-05-31 00:19:23.710944 llama_hub-0.0.4/llama_hub/file/deepdoctection/base.py
--rw-r--r--   0        0        0       24 2023-05-31 00:19:23.711015 llama_hub-0.0.4/llama_hub/file/deepdoctection/requirements.txt
--rw-r--r--   0        0        0      800 2023-05-31 00:19:23.711097 llama_hub-0.0.4/llama_hub/file/docx/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.711148 llama_hub-0.0.4/llama_hub/file/docx/__init__.py
--rw-r--r--   0        0        0      624 2023-05-31 00:19:23.711197 llama_hub-0.0.4/llama_hub/file/docx/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.711264 llama_hub-0.0.4/llama_hub/file/docx/requirements.txt
--rw-r--r--   0        0        0      724 2023-05-31 00:19:23.711407 llama_hub-0.0.4/llama_hub/file/epub/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.711459 llama_hub-0.0.4/llama_hub/file/epub/__init__.py
--rw-r--r--   0        0        0     1000 2023-05-31 00:19:23.711525 llama_hub-0.0.4/llama_hub/file/epub/base.py
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.711579 llama_hub-0.0.4/llama_hub/file/epub/requirements.txt
--rw-r--r--   0        0        0     1087 2023-05-31 00:19:23.711703 llama_hub-0.0.4/llama_hub/file/flat_pdf/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.711756 llama_hub-0.0.4/llama_hub/file/flat_pdf/__init__.py
--rw-r--r--   0        0        0     2837 2023-05-31 00:19:23.711854 llama_hub-0.0.4/llama_hub/file/flat_pdf/base.py
--rw-r--r--   0        0        0       15 2023-05-31 00:19:23.711939 llama_hub-0.0.4/llama_hub/file/flat_pdf/requirements.txt
--rw-r--r--   0        0        0     1359 2023-05-31 00:19:23.712052 llama_hub-0.0.4/llama_hub/file/image/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.712114 llama_hub-0.0.4/llama_hub/file/image/__init__.py
--rw-r--r--   0        0        0     3888 2023-05-31 00:19:23.712184 llama_hub-0.0.4/llama_hub/file/image/base.py
--rw-r--r--   0        0        0       63 2023-05-31 00:19:23.712235 llama_hub-0.0.4/llama_hub/file/image/requirements.txt
--rw-r--r--   0        0        0      373 2023-05-31 00:19:23.712359 llama_hub-0.0.4/llama_hub/file/image_blip/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.712384 llama_hub-0.0.4/llama_hub/file/image_blip/__init__.py
--rw-r--r--   0        0        0     3229 2023-06-03 03:50:30.194383 llama_hub-0.0.4/llama_hub/file/image_blip/base.py
--rw-r--r--   0        0        0       40 2023-05-31 00:19:23.712578 llama_hub-0.0.4/llama_hub/file/image_blip/requirements.txt
--rw-r--r--   0        0        0      422 2023-05-31 00:19:23.712697 llama_hub-0.0.4/llama_hub/file/image_blip2/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.712725 llama_hub-0.0.4/llama_hub/file/image_blip2/__init__.py
--rw-r--r--   0        0        0     3331 2023-06-03 03:50:30.194545 llama_hub-0.0.4/llama_hub/file/image_blip2/base.py
--rw-r--r--   0        0        0       40 2023-05-31 00:19:23.712933 llama_hub-0.0.4/llama_hub/file/image_blip2/requirements.txt
--rw-r--r--   0        0        0      417 2023-06-24 06:49:58.685139 llama_hub-0.0.4/llama_hub/file/image_deplot/README.md
--rw-r--r--   0        0        0        0 2023-06-24 06:49:58.685166 llama_hub-0.0.4/llama_hub/file/image_deplot/__init__.py
--rw-r--r--   0        0        0     3073 2023-06-24 06:49:58.685304 llama_hub-0.0.4/llama_hub/file/image_deplot/base.py
--rw-r--r--   0        0        0       40 2023-06-24 06:49:58.685736 llama_hub-0.0.4/llama_hub/file/image_deplot/requirements.txt
--rw-r--r--   0        0        0      457 2023-05-31 00:19:23.713074 llama_hub-0.0.4/llama_hub/file/ipynb/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.713111 llama_hub-0.0.4/llama_hub/file/ipynb/__init__.py
--rw-r--r--   0        0        0     1296 2023-05-31 00:19:23.713224 llama_hub-0.0.4/llama_hub/file/ipynb/base.py
--rw-r--r--   0        0        0        9 2023-05-31 00:19:23.713320 llama_hub-0.0.4/llama_hub/file/ipynb/requirements.txt
--rw-r--r--   0        0        0      735 2023-05-31 00:19:23.713712 llama_hub-0.0.4/llama_hub/file/json/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.713821 llama_hub-0.0.4/llama_hub/file/json/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-31 00:19:23.713925 llama_hub-0.0.4/llama_hub/file/json/base.py
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.713956 llama_hub-0.0.4/llama_hub/file/json/requirements.txt
--rw-r--r--   0        0        0      744 2023-05-31 00:19:23.714073 llama_hub-0.0.4/llama_hub/file/markdown/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.714150 llama_hub-0.0.4/llama_hub/file/markdown/__init__.py
--rw-r--r--   0        0        0     3633 2023-05-31 00:19:23.714275 llama_hub-0.0.4/llama_hub/file/markdown/base.py
--rw-r--r--   0        0        0      680 2023-05-31 00:19:23.714381 llama_hub-0.0.4/llama_hub/file/mbox/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.714447 llama_hub-0.0.4/llama_hub/file/mbox/__init__.py
--rw-r--r--   0        0        0     3604 2023-05-31 00:19:23.714680 llama_hub-0.0.4/llama_hub/file/mbox/base.py
--rw-r--r--   0        0        0       14 2023-05-31 00:19:23.714754 llama_hub-0.0.4/llama_hub/file/mbox/requirements.txt
--rw-r--r--   0        0        0      929 2023-05-31 00:19:23.714899 llama_hub-0.0.4/llama_hub/file/paged_csv/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.714940 llama_hub-0.0.4/llama_hub/file/paged_csv/__init__.py
--rw-r--r--   0        0        0      929 2023-05-31 00:19:23.715096 llama_hub-0.0.4/llama_hub/file/paged_csv/base.py
--rw-r--r--   0        0        0      786 2023-05-31 00:19:23.715234 llama_hub-0.0.4/llama_hub/file/pandas_csv/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.715305 llama_hub-0.0.4/llama_hub/file/pandas_csv/__init__.py
--rw-r--r--   0        0        0     2271 2023-05-31 00:19:23.715402 llama_hub-0.0.4/llama_hub/file/pandas_csv/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.715462 llama_hub-0.0.4/llama_hub/file/pandas_csv/requirements.txt
--rw-r--r--   0        0        0     1334 2023-05-31 00:19:23.715614 llama_hub-0.0.4/llama_hub/file/pandas_excel/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.715680 llama_hub-0.0.4/llama_hub/file/pandas_excel/__init__.py
--rw-r--r--   0        0        0     2219 2023-05-31 00:19:23.715753 llama_hub-0.0.4/llama_hub/file/pandas_excel/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.715809 llama_hub-0.0.4/llama_hub/file/pandas_excel/requirements.txt
--rw-r--r--   0        0        0      790 2023-05-31 00:19:23.715925 llama_hub-0.0.4/llama_hub/file/pdf/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.715984 llama_hub-0.0.4/llama_hub/file/pdf/__init__.py
--rw-r--r--   0        0        0     1165 2023-05-31 00:19:23.716042 llama_hub-0.0.4/llama_hub/file/pdf/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.716096 llama_hub-0.0.4/llama_hub/file/pdf/requirements.txt
--rw-r--r--   0        0        0      904 2023-06-10 07:58:38.772384 llama_hub-0.0.4/llama_hub/file/pdf_miner/README.md
--rw-r--r--   0        0        0       17 2023-06-10 07:58:38.772474 llama_hub-0.0.4/llama_hub/file/pdf_miner/__init__.py
--rw-r--r--   0        0        0     2005 2023-06-10 07:58:38.772566 llama_hub-0.0.4/llama_hub/file/pdf_miner/base.py
--rw-r--r--   0        0        0       13 2023-06-10 07:58:38.772654 llama_hub-0.0.4/llama_hub/file/pdf_miner/requirements.txt
--rw-r--r--   0        0        0     1120 2023-05-31 00:19:23.716188 llama_hub-0.0.4/llama_hub/file/pptx/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.716252 llama_hub-0.0.4/llama_hub/file/pptx/__init__.py
--rw-r--r--   0        0        0     3447 2023-05-31 00:19:23.716338 llama_hub-0.0.4/llama_hub/file/pptx/base.py
--rw-r--r--   0        0        0       49 2023-05-31 00:19:23.716404 llama_hub-0.0.4/llama_hub/file/pptx/requirements.txt
--rw-r--r--   0        0        0     1160 2023-05-31 00:19:23.716683 llama_hub-0.0.4/llama_hub/file/pymu_pdf/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.716754 llama_hub-0.0.4/llama_hub/file/pymu_pdf/__init__.py
--rw-r--r--   0        0        0     2415 2023-05-31 00:19:23.716819 llama_hub-0.0.4/llama_hub/file/pymu_pdf/base.py
--rw-r--r--   0        0        0        7 2023-05-31 00:19:23.716870 llama_hub-0.0.4/llama_hub/file/pymu_pdf/requirements.txt
--rw-r--r--   0        0        0      890 2023-05-31 00:19:23.716967 llama_hub-0.0.4/llama_hub/file/rdf/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717033 llama_hub-0.0.4/llama_hub/file/rdf/__init__.py
--rw-r--r--   0        0        0     2203 2023-05-31 00:19:23.717110 llama_hub-0.0.4/llama_hub/file/rdf/base.py
--rw-r--r--   0        0        0       13 2023-05-31 00:19:23.717167 llama_hub-0.0.4/llama_hub/file/rdf/requirements.txt
--rw-r--r--   0        0        0      792 2023-05-31 00:19:23.717279 llama_hub-0.0.4/llama_hub/file/simple_csv/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717342 llama_hub-0.0.4/llama_hub/file/simple_csv/__init__.py
--rw-r--r--   0        0        0     1234 2023-05-31 00:19:23.717441 llama_hub-0.0.4/llama_hub/file/simple_csv/base.py
--rw-r--r--   0        0        0     2531 2023-05-31 00:19:23.717561 llama_hub-0.0.4/llama_hub/file/unstructured/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717635 llama_hub-0.0.4/llama_hub/file/unstructured/__init__.py
--rw-r--r--   0        0        0     1305 2023-05-31 00:19:23.717707 llama_hub-0.0.4/llama_hub/file/unstructured/base.py
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717763 llama_hub-0.0.4/llama_hub/file/unstructured/requirements.txt
--rw-r--r--   0        0        0     1498 2023-06-10 07:58:38.772778 llama_hub-0.0.4/llama_hub/firestore/README.md
--rw-r--r--   0        0        0       17 2023-06-10 07:58:38.772830 llama_hub-0.0.4/llama_hub/firestore/__init__.py
--rw-r--r--   0        0        0     2225 2023-06-10 07:58:38.772918 llama_hub-0.0.4/llama_hub/firestore/base.py
--rw-r--r--   0        0        0       23 2023-06-10 07:58:38.772997 llama_hub-0.0.4/llama_hub/firestore/requirements.txt
--rw-r--r--   0        0        0     3141 2023-06-10 07:58:38.773157 llama_hub-0.0.4/llama_hub/github_repo/README.md
--rw-r--r--   0        0        0      153 2023-05-31 00:19:23.717979 llama_hub-0.0.4/llama_hub/github_repo/__init__.py
--rw-r--r--   0        0        0    20914 2023-06-03 03:50:30.194900 llama_hub-0.0.4/llama_hub/github_repo/base.py
--rw-r--r--   0        0        0    12721 2023-05-31 00:19:23.718674 llama_hub-0.0.4/llama_hub/github_repo/github_client.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.718740 llama_hub-0.0.4/llama_hub/github_repo/requirements.txt
--rw-r--r--   0        0        0     5709 2023-06-03 03:50:30.195070 llama_hub-0.0.4/llama_hub/github_repo/utils.py
--rw-r--r--   0        0        0      948 2023-05-31 00:19:23.719165 llama_hub-0.0.4/llama_hub/gmail/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.719238 llama_hub-0.0.4/llama_hub/gmail/__init__.py
--rw-r--r--   0        0        0     5302 2023-05-31 00:19:23.719342 llama_hub-0.0.4/llama_hub/gmail/base.py
--rw-r--r--   0        0        0       81 2023-05-31 00:19:23.719438 llama_hub-0.0.4/llama_hub/gmail/requirements.txt
--rw-r--r--   0        0        0     1364 2023-05-31 00:19:23.719568 llama_hub-0.0.4/llama_hub/google_calendar/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.719630 llama_hub-0.0.4/llama_hub/google_calendar/__init__.py
--rw-r--r--   0        0        0     4755 2023-05-31 00:19:23.719707 llama_hub-0.0.4/llama_hub/google_calendar/base.py
--rw-r--r--   0        0        0       66 2023-05-31 00:19:23.719771 llama_hub-0.0.4/llama_hub/google_calendar/requirements.txt
--rw-r--r--   0        0        0     2571 2023-05-31 00:19:23.719884 llama_hub-0.0.4/llama_hub/google_docs/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.719942 llama_hub-0.0.4/llama_hub/google_docs/__init__.py
--rw-r--r--   0        0        0     5290 2023-06-24 06:49:58.686032 llama_hub-0.0.4/llama_hub/google_docs/base.py
--rw-r--r--   0        0        0       66 2023-05-31 00:19:23.720074 llama_hub-0.0.4/llama_hub/google_docs/requirements.txt
--rw-r--r--   0        0        0     1807 2023-05-31 00:19:23.720187 llama_hub-0.0.4/llama_hub/google_drive/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.720244 llama_hub-0.0.4/llama_hub/google_drive/__init__.py
--rw-r--r--   0        0        0    13454 2023-06-03 03:50:30.195254 llama_hub-0.0.4/llama_hub/google_drive/base.py
--rw-r--r--   0        0        0       76 2023-05-31 00:19:23.720583 llama_hub-0.0.4/llama_hub/google_drive/requirements.txt
--rw-r--r--   0        0        0     1150 2023-05-31 00:19:23.720701 llama_hub-0.0.4/llama_hub/google_sheets/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.720755 llama_hub-0.0.4/llama_hub/google_sheets/__init__.py
--rw-r--r--   0        0        0     4989 2023-05-31 00:19:23.720863 llama_hub-0.0.4/llama_hub/google_sheets/base.py
--rw-r--r--   0        0        0       66 2023-05-31 00:19:23.720914 llama_hub-0.0.4/llama_hub/google_sheets/requirements.txt
--rw-r--r--   0        0        0      809 2023-05-31 00:19:23.721050 llama_hub-0.0.4/llama_hub/gpt_repo/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.721109 llama_hub-0.0.4/llama_hub/gpt_repo/__init__.py
--rw-r--r--   0        0        0     5488 2023-05-31 00:19:23.721217 llama_hub-0.0.4/llama_hub/gpt_repo/base.py
--rw-r--r--   0        0        0     1595 2023-05-31 00:19:23.721376 llama_hub-0.0.4/llama_hub/graphdb_cypher/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.721443 llama_hub-0.0.4/llama_hub/graphdb_cypher/__init__.py
--rw-r--r--   0        0        0     1788 2023-05-31 00:19:23.721561 llama_hub-0.0.4/llama_hub/graphdb_cypher/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.721683 llama_hub-0.0.4/llama_hub/graphdb_cypher/requirements.txt
--rw-r--r--   0        0        0     1215 2023-05-31 00:19:23.721834 llama_hub-0.0.4/llama_hub/graphql/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.721886 llama_hub-0.0.4/llama_hub/graphql/__init__.py
--rw-r--r--   0        0        0     2204 2023-05-31 00:19:23.721979 llama_hub-0.0.4/llama_hub/graphql/base.py
--rw-r--r--   0        0        0       21 2023-05-31 00:19:23.722048 llama_hub-0.0.4/llama_hub/graphql/requirements.txt
--rw-r--r--   0        0        0      969 2023-05-31 00:19:23.722173 llama_hub-0.0.4/llama_hub/hatena_blog/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.722225 llama_hub-0.0.4/llama_hub/hatena_blog/__init__.py
--rw-r--r--   0        0        0     2624 2023-05-31 00:19:23.722316 llama_hub-0.0.4/llama_hub/hatena_blog/base.py
--rw-r--r--   0        0        0       28 2023-05-31 00:19:23.722405 llama_hub-0.0.4/llama_hub/hatena_blog/requirements.txt
--rw-r--r--   0        0        0      916 2023-05-31 00:19:23.722570 llama_hub-0.0.4/llama_hub/hubspot/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.722654 llama_hub-0.0.4/llama_hub/hubspot/__init__.py
--rw-r--r--   0        0        0     1286 2023-05-31 00:19:23.722744 llama_hub-0.0.4/llama_hub/hubspot/base.py
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.722823 llama_hub-0.0.4/llama_hub/hubspot/requirements.txt
--rw-r--r--   0        0        0     1035 2023-05-31 00:19:23.722974 llama_hub-0.0.4/llama_hub/huggingface/fs/README.md
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.723070 llama_hub-0.0.4/llama_hub/huggingface/fs/__init__.py
--rw-r--r--   0        0        0     1827 2023-05-31 00:19:23.723162 llama_hub-0.0.4/llama_hub/huggingface/fs/base.py
--rw-r--r--   0        0        0       15 2023-05-31 00:19:23.723269 llama_hub-0.0.4/llama_hub/huggingface/fs/requirements.txt
--rw-r--r--   0        0        0      797 2023-05-31 00:19:23.723369 llama_hub-0.0.4/llama_hub/intercom/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.723425 llama_hub-0.0.4/llama_hub/intercom/__init__.py
--rw-r--r--   0        0        0     2416 2023-05-31 00:19:23.723490 llama_hub-0.0.4/llama_hub/intercom/base.py
--rw-r--r--   0        0        0       39 2023-05-31 00:19:23.723542 llama_hub-0.0.4/llama_hub/intercom/requirements.txt
--rw-r--r--   0        0        0      808 2023-06-10 07:58:38.773924 llama_hub-0.0.4/llama_hub/jira/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.723719 llama_hub-0.0.4/llama_hub/jira/__init__.py
--rw-r--r--   0        0        0     3383 2023-05-31 00:19:23.723801 llama_hub-0.0.4/llama_hub/jira/base.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.723892 llama_hub-0.0.4/llama_hub/jira/requirements.txt
--rw-r--r--   0        0        0     1362 2023-05-31 00:19:23.724041 llama_hub-0.0.4/llama_hub/joplin/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.724074 llama_hub-0.0.4/llama_hub/joplin/__init__.py
--rw-r--r--   0        0        0     5183 2023-05-31 00:19:23.724310 llama_hub-0.0.4/llama_hub/joplin/base.py
--rw-r--r--   0        0        0      698 2023-05-31 00:19:23.724418 llama_hub-0.0.4/llama_hub/jsondata/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.724463 llama_hub-0.0.4/llama_hub/jsondata/__init__.py
--rw-r--r--   0        0        0     1633 2023-05-31 00:19:23.724551 llama_hub-0.0.4/llama_hub/jsondata/base.py
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.724577 llama_hub-0.0.4/llama_hub/jsondata/requirements.txt
--rw-r--r--   0        0        0     7206 2023-05-31 00:19:23.724774 llama_hub-0.0.4/llama_hub/kaltura/esearch/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.724845 llama_hub-0.0.4/llama_hub/kaltura/esearch/__init__.py
--rw-r--r--   0        0        0    12019 2023-05-31 00:19:23.724953 llama_hub-0.0.4/llama_hub/kaltura/esearch/base.py
--rw-r--r--   0        0        0       24 2023-05-31 00:19:23.725038 llama_hub-0.0.4/llama_hub/kaltura/esearch/requirements.txt
--rw-r--r--   0        0        0      785 2023-06-24 06:49:58.686157 llama_hub-0.0.4/llama_hub/kibela/README.md
--rw-r--r--   0        0        0       17 2023-06-24 06:49:58.686207 llama_hub-0.0.4/llama_hub/kibela/__init__.py
--rw-r--r--   0        0        0     3137 2023-06-24 06:49:58.686313 llama_hub-0.0.4/llama_hub/kibela/base.py
--rw-r--r--   0        0        0        4 2023-06-24 06:49:58.686394 llama_hub-0.0.4/llama_hub/kibela/requirements.txt
--rw-r--r--   0        0        0    11884 2023-06-24 06:49:58.686539 llama_hub-0.0.4/llama_hub/library.json
--rw-r--r--   0        0        0     1117 2023-05-31 00:19:23.725289 llama_hub-0.0.4/llama_hub/make_com/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.725348 llama_hub-0.0.4/llama_hub/make_com/__init__.py
--rw-r--r--   0        0        0     1721 2023-05-31 00:19:23.725434 llama_hub-0.0.4/llama_hub/make_com/base.py
--rw-r--r--   0        0        0      810 2023-05-31 00:19:23.725515 llama_hub-0.0.4/llama_hub/mangoapps_guides/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.725566 llama_hub-0.0.4/llama_hub/mangoapps_guides/__init__.py
--rw-r--r--   0        0        0     4752 2023-05-31 00:19:23.725645 llama_hub-0.0.4/llama_hub/mangoapps_guides/base.py
--rw-r--r--   0        0        0       39 2023-05-31 00:19:23.725706 llama_hub-0.0.4/llama_hub/mangoapps_guides/requirements.txt
--rw-r--r--   0        0        0     2740 2023-05-31 00:19:23.725850 llama_hub-0.0.4/llama_hub/maps/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.725903 llama_hub-0.0.4/llama_hub/maps/__init__.py
--rw-r--r--   0        0        0     4599 2023-05-31 00:19:23.726215 llama_hub-0.0.4/llama_hub/maps/base.py
--rw-r--r--   0        0        0       15 2023-05-31 00:19:23.726327 llama_hub-0.0.4/llama_hub/maps/requirements.txt
--rw-r--r--   0        0        0      870 2023-05-31 00:19:23.726449 llama_hub-0.0.4/llama_hub/memos/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.726502 llama_hub-0.0.4/llama_hub/memos/__init__.py
--rw-r--r--   0        0        0     1465 2023-05-31 00:19:23.726557 llama_hub-0.0.4/llama_hub/memos/base.py
--rw-r--r--   0        0        0      952 2023-05-31 00:19:23.726641 llama_hub-0.0.4/llama_hub/metal/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.726693 llama_hub-0.0.4/llama_hub/metal/__init__.py
--rw-r--r--   0        0        0     2326 2023-05-31 00:19:23.726764 llama_hub-0.0.4/llama_hub/metal/base.py
--rw-r--r--   0        0        0       10 2023-05-31 00:19:23.726825 llama_hub-0.0.4/llama_hub/metal/requirements.txt
--rw-r--r--   0        0        0     1174 2023-05-31 00:19:23.726943 llama_hub-0.0.4/llama_hub/milvus/README.md
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.727017 llama_hub-0.0.4/llama_hub/milvus/__init__.py
--rw-r--r--   0        0        0     4588 2023-05-31 00:19:23.727112 llama_hub-0.0.4/llama_hub/milvus/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.727182 llama_hub-0.0.4/llama_hub/milvus/requirements.txt
--rw-r--r--   0        0        0      853 2023-05-31 00:19:23.727268 llama_hub-0.0.4/llama_hub/mondaydotcom/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.727321 llama_hub-0.0.4/llama_hub/mondaydotcom/__init__.py
--rw-r--r--   0        0        0     2658 2023-05-31 00:19:23.727383 llama_hub-0.0.4/llama_hub/mondaydotcom/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.727432 llama_hub-0.0.4/llama_hub/mondaydotcom/requirements.txt
--rw-r--r--   0        0        0      973 2023-05-31 00:19:23.727516 llama_hub-0.0.4/llama_hub/mongo/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.727566 llama_hub-0.0.4/llama_hub/mongo/__init__.py
--rw-r--r--   0        0        0     2260 2023-05-31 00:19:23.727656 llama_hub-0.0.4/llama_hub/mongo/base.py
--rw-r--r--   0        0        0        7 2023-05-31 00:19:23.727743 llama_hub-0.0.4/llama_hub/mongo/requirements.txt
--rw-r--r--   0        0        0      916 2023-05-31 00:19:23.727849 llama_hub-0.0.4/llama_hub/notion/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.727909 llama_hub-0.0.4/llama_hub/notion/__init__.py
--rw-r--r--   0        0        0     6102 2023-05-31 00:19:23.727971 llama_hub-0.0.4/llama_hub/notion/base.py
--rw-r--r--   0        0        0      395 2023-06-01 05:01:36.458116 llama_hub-0.0.4/llama_hub/notion/tool.py
--rw-r--r--   0        0        0      688 2023-05-31 00:19:23.728057 llama_hub-0.0.4/llama_hub/obsidian/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.728106 llama_hub-0.0.4/llama_hub/obsidian/__init__.py
--rw-r--r--   0        0        0     1583 2023-05-31 00:19:23.728167 llama_hub-0.0.4/llama_hub/obsidian/base.py
--rw-r--r--   0        0        0     1050 2023-05-31 00:19:23.728304 llama_hub-0.0.4/llama_hub/opendal_reader/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.728335 llama_hub-0.0.4/llama_hub/opendal_reader/__init__.py
--rw-r--r--   0        0        0      980 2023-05-31 00:19:23.728466 llama_hub-0.0.4/llama_hub/opendal_reader/azblob/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.728521 llama_hub-0.0.4/llama_hub/opendal_reader/azblob/__init__.py
--rw-r--r--   0        0        0     2476 2023-05-31 00:19:23.728643 llama_hub-0.0.4/llama_hub/opendal_reader/azblob/base.py
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.728751 llama_hub-0.0.4/llama_hub/opendal_reader/azblob/requirements.txt
--rw-r--r--   0        0        0     2979 2023-05-31 00:19:23.728891 llama_hub-0.0.4/llama_hub/opendal_reader/base.py
--rw-r--r--   0        0        0      999 2023-05-31 00:19:23.729020 llama_hub-0.0.4/llama_hub/opendal_reader/gcs/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.729087 llama_hub-0.0.4/llama_hub/opendal_reader/gcs/__init__.py
--rw-r--r--   0        0        0     2294 2023-05-31 00:19:23.729212 llama_hub-0.0.4/llama_hub/opendal_reader/gcs/base.py
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729283 llama_hub-0.0.4/llama_hub/opendal_reader/gcs/requirements.txt
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729358 llama_hub-0.0.4/llama_hub/opendal_reader/requirements.txt
--rw-r--r--   0        0        0     1397 2023-05-31 00:19:23.729481 llama_hub-0.0.4/llama_hub/opendal_reader/s3/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.729530 llama_hub-0.0.4/llama_hub/opendal_reader/s3/__init__.py
--rw-r--r--   0        0        0     2605 2023-05-31 00:19:23.729641 llama_hub-0.0.4/llama_hub/opendal_reader/s3/base.py
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729714 llama_hub-0.0.4/llama_hub/opendal_reader/s3/requirements.txt
--rw-r--r--   0        0        0     2147 2023-05-31 00:19:23.729798 llama_hub-0.0.4/llama_hub/outlook_localcalendar/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729846 llama_hub-0.0.4/llama_hub/outlook_localcalendar/__init__,py
--rw-r--r--   0        0        0     3838 2023-05-31 00:19:23.729934 llama_hub-0.0.4/llama_hub/outlook_localcalendar/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.730022 llama_hub-0.0.4/llama_hub/outlook_localcalendar/requirements.txt
--rw-r--r--   0        0        0     1801 2023-05-31 00:19:23.730149 llama_hub-0.0.4/llama_hub/pandas_ai/README.md
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.730219 llama_hub-0.0.4/llama_hub/pandas_ai/__init__.py
--rw-r--r--   0        0        0     3932 2023-05-31 00:19:23.730347 llama_hub-0.0.4/llama_hub/pandas_ai/base.py
--rw-r--r--   0        0        0        8 2023-05-31 00:19:23.730434 llama_hub-0.0.4/llama_hub/pandas_ai/requirements.txt
--rw-r--r--   0        0        0     1484 2023-05-31 00:19:23.730555 llama_hub-0.0.4/llama_hub/papers/arxiv/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.730614 llama_hub-0.0.4/llama_hub/papers/arxiv/__init__.py
--rw-r--r--   0        0        0     6441 2023-05-31 00:19:23.730749 llama_hub-0.0.4/llama_hub/papers/arxiv/base.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.730795 llama_hub-0.0.4/llama_hub/papers/arxiv/requirements.txt
--rw-r--r--   0        0        0      931 2023-05-31 00:19:23.730889 llama_hub-0.0.4/llama_hub/papers/pubmed/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.730947 llama_hub-0.0.4/llama_hub/papers/pubmed/__init__.py
--rw-r--r--   0        0        0     6168 2023-05-31 00:19:23.731053 llama_hub-0.0.4/llama_hub/papers/pubmed/base.py
--rw-r--r--   0        0        0     1279 2023-05-31 00:19:23.731154 llama_hub-0.0.4/llama_hub/pinecone/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.731210 llama_hub-0.0.4/llama_hub/pinecone/__init__.py
--rw-r--r--   0        0        0     2587 2023-05-31 00:19:23.731290 llama_hub-0.0.4/llama_hub/pinecone/base.py
--rw-r--r--   0        0        0       15 2023-05-31 00:19:23.731346 llama_hub-0.0.4/llama_hub/pinecone/requirements.txt
--rw-r--r--   0        0        0     1157 2023-05-31 00:19:23.731448 llama_hub-0.0.4/llama_hub/qdrant/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.731505 llama_hub-0.0.4/llama_hub/qdrant/__init__.py
--rw-r--r--   0        0        0     6920 2023-05-31 00:19:23.731618 llama_hub-0.0.4/llama_hub/qdrant/base.py
--rw-r--r--   0        0        0       13 2023-05-31 00:19:23.731674 llama_hub-0.0.4/llama_hub/qdrant/requirements.txt
--rw-r--r--   0        0        0     1551 2023-05-31 00:19:23.731776 llama_hub-0.0.4/llama_hub/readwise/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.731833 llama_hub-0.0.4/llama_hub/readwise/__init__.py
--rw-r--r--   0        0        0     1800 2023-05-31 00:19:23.731903 llama_hub-0.0.4/llama_hub/readwise/base.py
--rw-r--r--   0        0        0     2707 2023-05-31 00:19:23.732014 llama_hub-0.0.4/llama_hub/reddit/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.732079 llama_hub-0.0.4/llama_hub/reddit/__init__.py
--rw-r--r--   0        0        0     1914 2023-05-31 00:19:23.732143 llama_hub-0.0.4/llama_hub/reddit/base.py
--rw-r--r--   0        0        0       81 2023-05-31 00:19:23.732202 llama_hub-0.0.4/llama_hub/reddit/requirements.txt
--rw-r--r--   0        0        0     1330 2023-05-31 00:19:23.732308 llama_hub-0.0.4/llama_hub/remote/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.732382 llama_hub-0.0.4/llama_hub/remote/__init__.py
--rw-r--r--   0        0        0     3165 2023-05-31 00:19:23.732529 llama_hub-0.0.4/llama_hub/remote/base.py
--rw-r--r--   0        0        0     1383 2023-05-31 00:19:23.732627 llama_hub-0.0.4/llama_hub/remote_depth/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.732655 llama_hub-0.0.4/llama_hub/remote_depth/__init__.py
--rw-r--r--   0        0        0     3829 2023-05-31 00:19:23.732820 llama_hub-0.0.4/llama_hub/remote_depth/base.py
--rw-r--r--   0        0        0       31 2023-05-31 00:19:23.732887 llama_hub-0.0.4/llama_hub/remote_depth/requirements.txt
--rw-r--r--   0        0        0     1669 2023-05-31 00:19:23.732997 llama_hub-0.0.4/llama_hub/s3/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.733053 llama_hub-0.0.4/llama_hub/s3/__init__.py
--rw-r--r--   0        0        0     3985 2023-05-31 00:19:23.733196 llama_hub-0.0.4/llama_hub/s3/base.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.733253 llama_hub-0.0.4/llama_hub/s3/requirements.txt
--rw-r--r--   0        0        0      821 2023-05-31 00:19:23.733394 llama_hub-0.0.4/llama_hub/slack/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.733459 llama_hub-0.0.4/llama_hub/slack/__init__.py
--rw-r--r--   0        0        0     7499 2023-05-31 00:19:23.733536 llama_hub-0.0.4/llama_hub/slack/base.py
--rw-r--r--   0        0        0        9 2023-05-31 00:19:23.733594 llama_hub-0.0.4/llama_hub/slack/requirements.txt
--rw-r--r--   0        0        0      690 2023-05-31 00:19:23.733754 llama_hub-0.0.4/llama_hub/snscrape_twitter/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.733815 llama_hub-0.0.4/llama_hub/snscrape_twitter/__init__.py
--rw-r--r--   0        0        0     1156 2023-05-31 00:19:23.733911 llama_hub-0.0.4/llama_hub/snscrape_twitter/base.py
--rw-r--r--   0        0        0       56 2023-05-31 00:19:23.734041 llama_hub-0.0.4/llama_hub/snscrape_twitter/requirements.txt
--rw-r--r--   0        0        0     1662 2023-05-31 00:19:23.734145 llama_hub-0.0.4/llama_hub/spotify/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.734204 llama_hub-0.0.4/llama_hub/spotify/__init__.py
--rw-r--r--   0        0        0     2287 2023-05-31 00:19:23.734275 llama_hub-0.0.4/llama_hub/spotify/base.py
--rw-r--r--   0        0        0        7 2023-05-31 00:19:23.734331 llama_hub-0.0.4/llama_hub/spotify/requirements.txt
--rw-r--r--   0        0        0      846 2023-05-31 00:19:23.734458 llama_hub-0.0.4/llama_hub/stackoverflow/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.734518 llama_hub-0.0.4/llama_hub/stackoverflow/__init__.py
--rw-r--r--   0        0        0     6263 2023-05-31 00:19:23.734626 llama_hub-0.0.4/llama_hub/stackoverflow/base.py
--rw-r--r--   0        0        0       21 2023-05-31 00:19:23.734708 llama_hub-0.0.4/llama_hub/stackoverflow/requirements.txt
--rw-r--r--   0        0        0      936 2023-05-31 00:19:23.734832 llama_hub-0.0.4/llama_hub/steamship/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.734866 llama_hub-0.0.4/llama_hub/steamship/__init__.py
--rw-r--r--   0        0        0     3498 2023-05-31 00:19:23.734974 llama_hub-0.0.4/llama_hub/steamship/base.py
--rw-r--r--   0        0        0        9 2023-05-31 00:19:23.735057 llama_hub-0.0.4/llama_hub/steamship/requirements.txt
--rw-r--r--   0        0        0      726 2023-05-31 00:19:23.735154 llama_hub-0.0.4/llama_hub/string_iterable/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.735234 llama_hub-0.0.4/llama_hub/string_iterable/__init__.py
--rw-r--r--   0        0        0      969 2023-05-31 00:19:23.735290 llama_hub-0.0.4/llama_hub/string_iterable/base.py
--rw-r--r--   0        0        0      676 2023-05-31 00:19:23.735435 llama_hub-0.0.4/llama_hub/trello/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.735493 llama_hub-0.0.4/llama_hub/trello/__init__.py
--rw-r--r--   0        0        0     1429 2023-05-31 00:19:23.735587 llama_hub-0.0.4/llama_hub/trello/base.py
--rw-r--r--   0        0        0       10 2023-05-31 00:19:23.735672 llama_hub-0.0.4/llama_hub/trello/requirements.txt
--rw-r--r--   0        0        0      924 2023-05-31 00:19:23.735778 llama_hub-0.0.4/llama_hub/twitter/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.735847 llama_hub-0.0.4/llama_hub/twitter/__init__.py
--rw-r--r--   0        0        0     1777 2023-05-31 00:19:23.735917 llama_hub-0.0.4/llama_hub/twitter/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.735976 llama_hub-0.0.4/llama_hub/twitter/requirements.txt
--rw-r--r--   0        0        0      637 2023-05-31 00:19:23.736279 llama_hub-0.0.4/llama_hub/utils.py
--rw-r--r--   0        0        0     1162 2023-05-31 00:19:23.736420 llama_hub-0.0.4/llama_hub/weather/README.md
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.736481 llama_hub-0.0.4/llama_hub/weather/__init__.py
--rw-r--r--   0        0        0     2779 2023-05-31 00:19:23.736578 llama_hub-0.0.4/llama_hub/weather/base.py
--rw-r--r--   0        0        0        5 2023-05-31 00:19:23.736662 llama_hub-0.0.4/llama_hub/weather/requirements.txt
--rw-r--r--   0        0        0     1525 2023-05-31 00:19:23.736765 llama_hub-0.0.4/llama_hub/weaviate/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.736823 llama_hub-0.0.4/llama_hub/weaviate/__init__.py
--rw-r--r--   0        0        0     3697 2023-05-31 00:19:23.736889 llama_hub-0.0.4/llama_hub/weaviate/base.py
--rw-r--r--   0        0        0       15 2023-05-31 00:19:23.736940 llama_hub-0.0.4/llama_hub/weaviate/requirements.txt
--rw-r--r--   0        0        0      415 2023-05-31 00:19:23.737101 llama_hub-0.0.4/llama_hub/web/async_web/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.737136 llama_hub-0.0.4/llama_hub/web/async_web/__init__.py
--rw-r--r--   0        0        0     2554 2023-05-31 00:19:23.737236 llama_hub-0.0.4/llama_hub/web/async_web/base.py
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.737325 llama_hub-0.0.4/llama_hub/web/async_web/requirements.txt
--rw-r--r--   0        0        0     3446 2023-05-31 00:19:23.737437 llama_hub-0.0.4/llama_hub/web/beautiful_soup_web/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.737504 llama_hub-0.0.4/llama_hub/web/beautiful_soup_web/__init__.py
--rw-r--r--   0        0        0     6747 2023-05-31 00:19:23.737610 llama_hub-0.0.4/llama_hub/web/beautiful_soup_web/base.py
--rw-r--r--   0        0        0       31 2023-05-31 00:19:23.737666 llama_hub-0.0.4/llama_hub/web/beautiful_soup_web/requirements.txt
--rw-r--r--   0        0        0     3672 2023-05-31 00:19:23.737782 llama_hub-0.0.4/llama_hub/web/knowledge_base/README.md
--rw-r--r--   0        0        0        1 2023-05-31 00:19:23.737843 llama_hub-0.0.4/llama_hub/web/knowledge_base/__init__.py
--rw-r--r--   0        0        0     5611 2023-05-31 00:19:23.737918 llama_hub-0.0.4/llama_hub/web/knowledge_base/base.py
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.737968 llama_hub-0.0.4/llama_hub/web/knowledge_base/requirements.txt
--rw-r--r--   0        0        0     2681 2023-05-31 00:19:23.738073 llama_hub-0.0.4/llama_hub/web/readability_web/README.md
--rw-r--r--   0        0        0    83319 2023-05-31 00:19:23.738443 llama_hub-0.0.4/llama_hub/web/readability_web/Readability.js
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.738513 llama_hub-0.0.4/llama_hub/web/readability_web/__init__.py
--rw-r--r--   0        0        0     4531 2023-05-31 00:19:23.738613 llama_hub-0.0.4/llama_hub/web/readability_web/base.py
--rw-r--r--   0        0        0       18 2023-05-31 00:19:23.738660 llama_hub-0.0.4/llama_hub/web/readability_web/requirements.txt
--rw-r--r--   0        0        0      489 2023-05-31 00:19:23.738734 llama_hub-0.0.4/llama_hub/web/rss/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.738780 llama_hub-0.0.4/llama_hub/web/rss/__init__.py
--rw-r--r--   0        0        0     1986 2023-05-31 00:19:23.738829 llama_hub-0.0.4/llama_hub/web/rss/base.py
--rw-r--r--   0        0        0     1994 2023-05-31 00:19:23.738914 llama_hub-0.0.4/llama_hub/web/simple_web/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.738959 llama_hub-0.0.4/llama_hub/web/simple_web/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-31 00:19:23.739036 llama_hub-0.0.4/llama_hub/web/simple_web/base.py
--rw-r--r--   0        0        0        9 2023-05-31 00:19:23.739081 llama_hub-0.0.4/llama_hub/web/simple_web/requirements.txt
--rw-r--r--   0        0        0     2009 2023-05-31 00:19:23.739158 llama_hub-0.0.4/llama_hub/web/trafilatura_web/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739207 llama_hub-0.0.4/llama_hub/web/trafilatura_web/__init__.py
--rw-r--r--   0        0        0      889 2023-05-31 00:19:23.739262 llama_hub-0.0.4/llama_hub/web/trafilatura_web/base.py
--rw-r--r--   0        0        0       16 2023-05-31 00:19:23.739305 llama_hub-0.0.4/llama_hub/web/trafilatura_web/requirements.txt
--rw-r--r--   0        0        0     1075 2023-05-31 00:19:23.739438 llama_hub-0.0.4/llama_hub/web/unstructured_web/README.md
--rw-r--r--   0        0        0        0 2023-05-31 00:19:23.739468 llama_hub-0.0.4/llama_hub/web/unstructured_web/__init__.py
--rw-r--r--   0        0        0     2250 2023-05-31 00:19:23.739541 llama_hub-0.0.4/llama_hub/web/unstructured_web/base.py
--rw-r--r--   0        0        0       12 2023-05-31 00:19:23.739609 llama_hub-0.0.4/llama_hub/web/unstructured_web/requirements.txt
--rw-r--r--   0        0        0     1315 2023-05-31 00:19:23.739686 llama_hub-0.0.4/llama_hub/whatsapp/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739729 llama_hub-0.0.4/llama_hub/whatsapp/__init__.py
--rw-r--r--   0        0        0     1509 2023-05-31 00:19:23.739776 llama_hub-0.0.4/llama_hub/whatsapp/base.py
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739818 llama_hub-0.0.4/llama_hub/whatsapp/requirements.txt
--rw-r--r--   0        0        0      895 2023-05-31 00:19:23.739897 llama_hub-0.0.4/llama_hub/wikipedia/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739946 llama_hub-0.0.4/llama_hub/wikipedia/__init__.py
--rw-r--r--   0        0        0      818 2023-05-31 00:19:23.740017 llama_hub-0.0.4/llama_hub/wikipedia/base.py
--rw-r--r--   0        0        0       14 2023-05-31 00:19:23.740060 llama_hub-0.0.4/llama_hub/wikipedia/requirements.txt
--rw-r--r--   0        0        0     1042 2023-05-31 00:19:23.740135 llama_hub-0.0.4/llama_hub/wordpress/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.740190 llama_hub-0.0.4/llama_hub/wordpress/__init__.py
--rw-r--r--   0        0        0     2546 2023-05-31 00:19:23.740248 llama_hub-0.0.4/llama_hub/wordpress/base.py
--rw-r--r--   0        0        0       39 2023-05-31 00:19:23.740291 llama_hub-0.0.4/llama_hub/wordpress/requirements.txt
--rw-r--r--   0        0        0      774 2023-05-31 00:19:23.740378 llama_hub-0.0.4/llama_hub/youtube_transcript/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.740429 llama_hub-0.0.4/llama_hub/youtube_transcript/__init__.py
--rw-r--r--   0        0        0     1687 2023-05-31 00:19:23.740509 llama_hub-0.0.4/llama_hub/youtube_transcript/base.py
--rw-r--r--   0        0        0       29 2023-05-31 00:19:23.740552 llama_hub-0.0.4/llama_hub/youtube_transcript/requirements.txt
--rw-r--r--   0        0        0      884 2023-05-31 00:19:23.740654 llama_hub-0.0.4/llama_hub/zendesk/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.740708 llama_hub-0.0.4/llama_hub/zendesk/__init__.py
--rw-r--r--   0        0        0     2323 2023-05-31 00:19:23.740795 llama_hub-0.0.4/llama_hub/zendesk/base.py
--rw-r--r--   0        0        0       24 2023-05-31 00:19:23.740869 llama_hub-0.0.4/llama_hub/zendesk/requirements.txt
--rw-r--r--   0        0        0     1304 2023-05-31 00:19:23.740971 llama_hub-0.0.4/llama_hub/zulip/README.md
--rw-r--r--   0        0        0       17 2023-05-31 00:19:23.741018 llama_hub-0.0.4/llama_hub/zulip/__init__.py
--rw-r--r--   0        0        0     2432 2023-05-31 00:19:23.741092 llama_hub-0.0.4/llama_hub/zulip/base.py
--rw-r--r--   0        0        0        6 2023-05-31 00:19:23.741155 llama_hub-0.0.4/llama_hub/zulip/requirements.txt
--rw-r--r--   0        0        0      868 2023-06-24 06:50:17.515585 llama_hub-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     7267 1970-01-01 00:00:00.000000 llama_hub-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-18 06:55:56.425923 llama_hub-0.0.5/LICENSE
+-rw-r--r--   0        0        0     6722 2023-06-27 01:05:04.198482 llama_hub-0.0.5/README.md
+-rw-r--r--   0        0        0      247 2023-05-31 00:19:23.701017 llama_hub-0.0.5/llama_hub/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.701087 llama_hub-0.0.5/llama_hub/__init__.py
+-rwxr-xr-x   0        0        0      119 2023-05-31 00:19:23.701156 llama_hub-0.0.5/llama_hub/add_loader.sh
+-rw-r--r--   0        0        0      826 2023-05-31 00:19:23.701312 llama_hub-0.0.5/llama_hub/airtable/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.701382 llama_hub-0.0.5/llama_hub/airtable/__init__.py
+-rw-r--r--   0        0        0      898 2023-06-27 01:05:04.199169 llama_hub-0.0.5/llama_hub/airtable/base.py
+-rw-r--r--   0        0        0       10 2023-05-31 00:19:23.701580 llama_hub-0.0.5/llama_hub/airtable/requirements.txt
+-rw-r--r--   0        0        0     1844 2023-06-27 01:05:04.199286 llama_hub-0.0.5/llama_hub/apify/actor/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.701871 llama_hub-0.0.5/llama_hub/apify/actor/__init__.py
+-rw-r--r--   0        0        0     2475 2023-06-27 01:05:04.199382 llama_hub-0.0.5/llama_hub/apify/actor/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:19:23.702389 llama_hub-0.0.5/llama_hub/apify/actor/requirements.txt
+-rw-r--r--   0        0        0     1504 2023-06-27 01:05:04.199484 llama_hub-0.0.5/llama_hub/apify/dataset/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.702623 llama_hub-0.0.5/llama_hub/apify/dataset/__init__.py
+-rw-r--r--   0        0        0     1373 2023-06-27 01:05:04.199596 llama_hub-0.0.5/llama_hub/apify/dataset/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:19:23.702829 llama_hub-0.0.5/llama_hub/apify/dataset/requirements.txt
+-rw-r--r--   0        0        0      778 2023-05-31 00:19:23.702978 llama_hub-0.0.5/llama_hub/asana/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.703048 llama_hub-0.0.5/llama_hub/asana/__init__.py
+-rw-r--r--   0        0        0     1861 2023-06-27 01:05:04.199732 llama_hub-0.0.5/llama_hub/asana/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.703184 llama_hub-0.0.5/llama_hub/asana/requirements.txt
+-rw-r--r--   0        0        0     2200 2023-05-31 00:19:23.703343 llama_hub-0.0.5/llama_hub/azcognitive_search/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.703413 llama_hub-0.0.5/llama_hub/azcognitive_search/__init__.py
+-rw-r--r--   0        0        0     2076 2023-06-27 01:05:04.199856 llama_hub-0.0.5/llama_hub/azcognitive_search/base.py
+-rw-r--r--   0        0        0       37 2023-05-31 00:19:23.703715 llama_hub-0.0.5/llama_hub/azcognitive_search/requirements.txt
+-rw-r--r--   0        0        0     2542 2023-05-31 00:19:23.703897 llama_hub-0.0.5/llama_hub/azstorage_blob/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.703969 llama_hub-0.0.5/llama_hub/azstorage_blob/__init__.py
+-rw-r--r--   0        0        0     5579 2023-06-27 01:05:04.199993 llama_hub-0.0.5/llama_hub/azstorage_blob/base.py
+-rw-r--r--   0        0        0       34 2023-05-31 00:19:23.704302 llama_hub-0.0.5/llama_hub/azstorage_blob/requirements.txt
+-rw-r--r--   0        0        0     1077 2023-05-31 00:19:23.704450 llama_hub-0.0.5/llama_hub/bilibili/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.704513 llama_hub-0.0.5/llama_hub/bilibili/__init__.py
+-rw-r--r--   0        0        0     2379 2023-06-27 01:05:04.200376 llama_hub-0.0.5/llama_hub/bilibili/base.py
+-rw-r--r--   0        0        0       21 2023-05-31 00:19:23.704655 llama_hub-0.0.5/llama_hub/bilibili/requirements.txt
+-rw-r--r--   0        0        0     3373 2023-05-31 00:19:23.705017 llama_hub-0.0.5/llama_hub/boarddocs/BoardDocsReader.ipynb
+-rw-r--r--   0        0        0     1402 2023-05-31 00:19:23.705098 llama_hub-0.0.5/llama_hub/boarddocs/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.705155 llama_hub-0.0.5/llama_hub/boarddocs/__init__.py
+-rw-r--r--   0        0        0     4358 2023-06-27 01:05:04.200537 llama_hub-0.0.5/llama_hub/boarddocs/base.py
+-rw-r--r--   0        0        0    19752 2023-05-31 00:19:23.705373 llama_hub-0.0.5/llama_hub/boarddocs/crawl.ipynb
+-rw-r--r--   0        0        0       22 2023-05-31 00:19:23.705450 llama_hub-0.0.5/llama_hub/boarddocs/requirements.txt
+-rw-r--r--   0        0        0      921 2023-05-31 00:19:23.705605 llama_hub-0.0.5/llama_hub/chatgpt_plugin/README.md
+-rw-r--r--   0        0        0       17 2023-06-27 01:05:04.202292 llama_hub-0.0.5/llama_hub/chatgpt_plugin/__init__.py
+-rw-r--r--   0        0        0     2111 2023-05-31 00:19:23.705774 llama_hub-0.0.5/llama_hub/chatgpt_plugin/base.py
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.705804 llama_hub-0.0.5/llama_hub/chatgpt_plugin/requirements.txt
+-rw-r--r--   0        0        0     1056 2023-05-31 00:19:23.705957 llama_hub-0.0.5/llama_hub/chroma/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.705990 llama_hub-0.0.5/llama_hub/chroma/__init__.py
+-rw-r--r--   0        0        0     1803 2023-06-27 01:05:04.202393 llama_hub-0.0.5/llama_hub/chroma/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.706141 llama_hub-0.0.5/llama_hub/chroma/requirements.txt
+-rw-r--r--   0        0        0     3039 2023-06-27 01:05:04.203110 llama_hub-0.0.5/llama_hub/confluence/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.706342 llama_hub-0.0.5/llama_hub/confluence/__init__.py
+-rw-r--r--   0        0        0    16558 2023-06-27 01:05:04.203316 llama_hub-0.0.5/llama_hub/confluence/base.py
+-rw-r--r--   0        0        0       89 2023-06-27 01:05:04.203462 llama_hub-0.0.5/llama_hub/confluence/requirements.txt
+-rw-r--r--   0        0        0     1052 2023-05-31 00:19:23.706689 llama_hub-0.0.5/llama_hub/couchdb/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.706764 llama_hub-0.0.5/llama_hub/couchdb/__init__.py
+-rw-r--r--   0        0        0     2660 2023-06-27 01:05:04.203585 llama_hub-0.0.5/llama_hub/couchdb/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:19:23.706940 llama_hub-0.0.5/llama_hub/couchdb/requirements.txt
+-rw-r--r--   0        0        0      582 2023-05-31 00:19:23.707023 llama_hub-0.0.5/llama_hub/dad_jokes/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.707074 llama_hub-0.0.5/llama_hub/dad_jokes/__init__.py
+-rw-r--r--   0        0        0      720 2023-06-27 01:05:04.203682 llama_hub-0.0.5/llama_hub/dad_jokes/base.py
+-rw-r--r--   0        0        0     1259 2023-05-31 00:19:23.707209 llama_hub-0.0.5/llama_hub/database/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.707265 llama_hub-0.0.5/llama_hub/database/__init__.py
+-rw-r--r--   0        0        0     3333 2023-06-27 01:05:04.203791 llama_hub-0.0.5/llama_hub/database/base.py
+-rw-r--r--   0        0        0     1096 2023-05-31 00:19:23.707478 llama_hub-0.0.5/llama_hub/deeplake/README.md
+-rw-r--r--   0        0        0       19 2023-06-27 01:05:04.203876 llama_hub-0.0.5/llama_hub/deeplake/__init__.py
+-rw-r--r--   0        0        0     3457 2023-05-31 00:19:23.707661 llama_hub-0.0.5/llama_hub/deeplake/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.707752 llama_hub-0.0.5/llama_hub/deeplake/requirements.txt
+-rw-r--r--   0        0        0      851 2023-05-31 00:19:23.707833 llama_hub-0.0.5/llama_hub/discord/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.707879 llama_hub-0.0.5/llama_hub/discord/__init__.py
+-rw-r--r--   0        0        0     4655 2023-06-27 01:05:04.203994 llama_hub-0.0.5/llama_hub/discord/base.py
+-rw-r--r--   0        0        0       10 2023-05-31 00:19:23.707985 llama_hub-0.0.5/llama_hub/discord/requirements.txt
+-rw-r--r--   0        0        0     4221 2023-06-25 18:53:37.869509 llama_hub-0.0.5/llama_hub/docugami/README.md
+-rw-r--r--   0        0        0        5 2023-06-27 01:05:04.204081 llama_hub-0.0.5/llama_hub/docugami/__init__.py
+-rw-r--r--   0        0        0    12087 2023-06-27 01:05:04.204227 llama_hub-0.0.5/llama_hub/docugami/base.py
+-rw-r--r--   0        0        0    65833 2023-05-31 00:19:23.708412 llama_hub-0.0.5/llama_hub/docugami/docugami.ipynb
+-rw-r--r--   0        0        0       20 2023-05-31 00:19:23.708465 llama_hub-0.0.5/llama_hub/docugami/requirements.txt
+-rw-r--r--   0        0        0     1042 2023-05-31 00:19:23.708545 llama_hub-0.0.5/llama_hub/elasticsearch/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.708572 llama_hub-0.0.5/llama_hub/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     2190 2023-06-27 01:05:04.204393 llama_hub-0.0.5/llama_hub/elasticsearch/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.708699 llama_hub-0.0.5/llama_hub/elasticsearch/requirements.txt
+-rw-r--r--   0        0        0     1319 2023-05-31 00:19:23.708825 llama_hub-0.0.5/llama_hub/faiss/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.708885 llama_hub-0.0.5/llama_hub/faiss/__init__.py
+-rw-r--r--   0        0        0     2126 2023-05-31 00:19:23.708943 llama_hub-0.0.5/llama_hub/faiss/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.708986 llama_hub-0.0.5/llama_hub/faiss/requirements.txt
+-rw-r--r--   0        0        0      585 2023-05-31 00:19:23.709108 llama_hub-0.0.5/llama_hub/feedly_rss/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.709136 llama_hub-0.0.5/llama_hub/feedly_rss/__init__.py
+-rw-r--r--   0        0        0     2128 2023-06-27 01:05:04.204556 llama_hub-0.0.5/llama_hub/feedly_rss/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:19:23.709288 llama_hub-0.0.5/llama_hub/feedly_rss/requirements.txt
+-rw-r--r--   0        0        0     2829 2023-05-31 00:19:23.709504 llama_hub-0.0.5/llama_hub/file/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.709559 llama_hub-0.0.5/llama_hub/file/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-31 00:19:23.709669 llama_hub-0.0.5/llama_hub/file/audio/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.709737 llama_hub-0.0.5/llama_hub/file/audio/__init__.py
+-rw-r--r--   0        0        0     1491 2023-06-27 01:05:04.204764 llama_hub-0.0.5/llama_hub/file/audio/base.py
+-rw-r--r--   0        0        0       20 2023-05-31 00:19:23.709874 llama_hub-0.0.5/llama_hub/file/audio/requirements.txt
+-rw-r--r--   0        0        0     1241 2023-05-31 00:19:23.710011 llama_hub-0.0.5/llama_hub/file/audio_gladia/README.md
+-rw-r--r--   0        0        0       19 2023-05-31 00:19:23.710082 llama_hub-0.0.5/llama_hub/file/audio_gladia/__init__.py
+-rw-r--r--   0        0        0     3273 2023-06-27 01:05:04.204876 llama_hub-0.0.5/llama_hub/file/audio_gladia/base.py
+-rw-r--r--   0        0        0       20 2023-05-31 00:19:23.710239 llama_hub-0.0.5/llama_hub/file/audio_gladia/requirements.txt
+-rw-r--r--   0        0        0     5553 2023-06-27 01:05:04.204981 llama_hub-0.0.5/llama_hub/file/base.py
+-rw-r--r--   0        0        0     1069 2023-05-31 00:19:23.710517 llama_hub-0.0.5/llama_hub/file/cjk_pdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.710563 llama_hub-0.0.5/llama_hub/file/cjk_pdf/__init__.py
+-rw-r--r--   0        0        0     2594 2023-06-27 01:05:04.205064 llama_hub-0.0.5/llama_hub/file/cjk_pdf/base.py
+-rw-r--r--   0        0        0       12 2023-05-31 00:19:23.710693 llama_hub-0.0.5/llama_hub/file/cjk_pdf/requirements.txt
+-rw-r--r--   0        0        0      800 2023-05-31 00:19:23.710812 llama_hub-0.0.5/llama_hub/file/deepdoctection/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.710846 llama_hub-0.0.5/llama_hub/file/deepdoctection/__init__.py
+-rw-r--r--   0        0        0     1164 2023-06-27 01:05:04.205154 llama_hub-0.0.5/llama_hub/file/deepdoctection/base.py
+-rw-r--r--   0        0        0       24 2023-05-31 00:19:23.711015 llama_hub-0.0.5/llama_hub/file/deepdoctection/requirements.txt
+-rw-r--r--   0        0        0      800 2023-05-31 00:19:23.711097 llama_hub-0.0.5/llama_hub/file/docx/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.711148 llama_hub-0.0.5/llama_hub/file/docx/__init__.py
+-rw-r--r--   0        0        0      629 2023-06-27 01:05:04.205232 llama_hub-0.0.5/llama_hub/file/docx/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.711264 llama_hub-0.0.5/llama_hub/file/docx/requirements.txt
+-rw-r--r--   0        0        0      724 2023-05-31 00:19:23.711407 llama_hub-0.0.5/llama_hub/file/epub/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.711459 llama_hub-0.0.5/llama_hub/file/epub/__init__.py
+-rw-r--r--   0        0        0     1005 2023-06-27 01:05:04.205315 llama_hub-0.0.5/llama_hub/file/epub/base.py
+-rw-r--r--   0        0        0       18 2023-05-31 00:19:23.711579 llama_hub-0.0.5/llama_hub/file/epub/requirements.txt
+-rw-r--r--   0        0        0     1087 2023-05-31 00:19:23.711703 llama_hub-0.0.5/llama_hub/file/flat_pdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.711756 llama_hub-0.0.5/llama_hub/file/flat_pdf/__init__.py
+-rw-r--r--   0        0        0     2978 2023-06-27 01:05:04.205404 llama_hub-0.0.5/llama_hub/file/flat_pdf/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:19:23.711939 llama_hub-0.0.5/llama_hub/file/flat_pdf/requirements.txt
+-rw-r--r--   0        0        0     1359 2023-05-31 00:19:23.712052 llama_hub-0.0.5/llama_hub/file/image/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.712114 llama_hub-0.0.5/llama_hub/file/image/__init__.py
+-rw-r--r--   0        0        0     3888 2023-05-31 00:19:23.712184 llama_hub-0.0.5/llama_hub/file/image/base.py
+-rw-r--r--   0        0        0       63 2023-05-31 00:19:23.712235 llama_hub-0.0.5/llama_hub/file/image/requirements.txt
+-rw-r--r--   0        0        0      373 2023-05-31 00:19:23.712359 llama_hub-0.0.5/llama_hub/file/image_blip/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.712384 llama_hub-0.0.5/llama_hub/file/image_blip/__init__.py
+-rw-r--r--   0        0        0     3374 2023-06-27 01:05:04.206094 llama_hub-0.0.5/llama_hub/file/image_blip/base.py
+-rw-r--r--   0        0        0       40 2023-05-31 00:19:23.712578 llama_hub-0.0.5/llama_hub/file/image_blip/requirements.txt
+-rw-r--r--   0        0        0      422 2023-05-31 00:19:23.712697 llama_hub-0.0.5/llama_hub/file/image_blip2/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.712725 llama_hub-0.0.5/llama_hub/file/image_blip2/__init__.py
+-rw-r--r--   0        0        0     3416 2023-06-27 01:05:04.206233 llama_hub-0.0.5/llama_hub/file/image_blip2/base.py
+-rw-r--r--   0        0        0       40 2023-05-31 00:19:23.712933 llama_hub-0.0.5/llama_hub/file/image_blip2/requirements.txt
+-rw-r--r--   0        0        0      417 2023-06-24 06:49:58.685139 llama_hub-0.0.5/llama_hub/file/image_deplot/README.md
+-rw-r--r--   0        0        0        0 2023-06-24 06:49:58.685166 llama_hub-0.0.5/llama_hub/file/image_deplot/__init__.py
+-rw-r--r--   0        0        0     3140 2023-06-27 01:05:04.206336 llama_hub-0.0.5/llama_hub/file/image_deplot/base.py
+-rw-r--r--   0        0        0       40 2023-06-24 06:49:58.685736 llama_hub-0.0.5/llama_hub/file/image_deplot/requirements.txt
+-rw-r--r--   0        0        0      457 2023-05-31 00:19:23.713074 llama_hub-0.0.5/llama_hub/file/ipynb/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.713111 llama_hub-0.0.5/llama_hub/file/ipynb/__init__.py
+-rw-r--r--   0        0        0     1292 2023-06-27 01:05:04.206427 llama_hub-0.0.5/llama_hub/file/ipynb/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:19:23.713320 llama_hub-0.0.5/llama_hub/file/ipynb/requirements.txt
+-rw-r--r--   0        0        0      735 2023-05-31 00:19:23.713712 llama_hub-0.0.5/llama_hub/file/json/README.md
+-rw-r--r--   0        0        0       17 2023-06-27 01:05:04.206504 llama_hub-0.0.5/llama_hub/file/json/__init__.py
+-rw-r--r--   0        0        0     2696 2023-06-27 01:05:04.206596 llama_hub-0.0.5/llama_hub/file/json/base.py
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.713956 llama_hub-0.0.5/llama_hub/file/json/requirements.txt
+-rw-r--r--   0        0        0      744 2023-05-31 00:19:23.714073 llama_hub-0.0.5/llama_hub/file/markdown/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.714150 llama_hub-0.0.5/llama_hub/file/markdown/__init__.py
+-rw-r--r--   0        0        0     3638 2023-06-27 01:05:04.206699 llama_hub-0.0.5/llama_hub/file/markdown/base.py
+-rw-r--r--   0        0        0      680 2023-05-31 00:19:23.714381 llama_hub-0.0.5/llama_hub/file/mbox/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.714447 llama_hub-0.0.5/llama_hub/file/mbox/__init__.py
+-rw-r--r--   0        0        0     3647 2023-06-27 01:05:04.206809 llama_hub-0.0.5/llama_hub/file/mbox/base.py
+-rw-r--r--   0        0        0       14 2023-05-31 00:19:23.714754 llama_hub-0.0.5/llama_hub/file/mbox/requirements.txt
+-rw-r--r--   0        0        0      929 2023-05-31 00:19:23.714899 llama_hub-0.0.5/llama_hub/file/paged_csv/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.714940 llama_hub-0.0.5/llama_hub/file/paged_csv/__init__.py
+-rw-r--r--   0        0        0      983 2023-06-27 01:05:04.206911 llama_hub-0.0.5/llama_hub/file/paged_csv/base.py
+-rw-r--r--   0        0        0      786 2023-05-31 00:19:23.715234 llama_hub-0.0.5/llama_hub/file/pandas_csv/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.715305 llama_hub-0.0.5/llama_hub/file/pandas_csv/__init__.py
+-rw-r--r--   0        0        0     2309 2023-06-27 01:05:04.207028 llama_hub-0.0.5/llama_hub/file/pandas_csv/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.715462 llama_hub-0.0.5/llama_hub/file/pandas_csv/requirements.txt
+-rw-r--r--   0        0        0     1334 2023-05-31 00:19:23.715614 llama_hub-0.0.5/llama_hub/file/pandas_excel/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.715680 llama_hub-0.0.5/llama_hub/file/pandas_excel/__init__.py
+-rw-r--r--   0        0        0     2366 2023-06-27 01:05:04.207130 llama_hub-0.0.5/llama_hub/file/pandas_excel/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.715809 llama_hub-0.0.5/llama_hub/file/pandas_excel/requirements.txt
+-rw-r--r--   0        0        0      790 2023-05-31 00:19:23.715925 llama_hub-0.0.5/llama_hub/file/pdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.715984 llama_hub-0.0.5/llama_hub/file/pdf/__init__.py
+-rw-r--r--   0        0        0     1135 2023-06-27 01:05:04.207213 llama_hub-0.0.5/llama_hub/file/pdf/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.716096 llama_hub-0.0.5/llama_hub/file/pdf/requirements.txt
+-rw-r--r--   0        0        0      904 2023-06-10 07:58:38.772384 llama_hub-0.0.5/llama_hub/file/pdf_miner/README.md
+-rw-r--r--   0        0        0       17 2023-06-10 07:58:38.772474 llama_hub-0.0.5/llama_hub/file/pdf_miner/__init__.py
+-rw-r--r--   0        0        0     2037 2023-06-27 01:05:04.207657 llama_hub-0.0.5/llama_hub/file/pdf_miner/base.py
+-rw-r--r--   0        0        0       13 2023-06-10 07:58:38.772654 llama_hub-0.0.5/llama_hub/file/pdf_miner/requirements.txt
+-rw-r--r--   0        0        0     1120 2023-05-31 00:19:23.716188 llama_hub-0.0.5/llama_hub/file/pptx/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.716252 llama_hub-0.0.5/llama_hub/file/pptx/__init__.py
+-rw-r--r--   0        0        0     3477 2023-06-27 01:05:04.207756 llama_hub-0.0.5/llama_hub/file/pptx/base.py
+-rw-r--r--   0        0        0       49 2023-05-31 00:19:23.716404 llama_hub-0.0.5/llama_hub/file/pptx/requirements.txt
+-rw-r--r--   0        0        0     1160 2023-05-31 00:19:23.716683 llama_hub-0.0.5/llama_hub/file/pymu_pdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.716754 llama_hub-0.0.5/llama_hub/file/pymu_pdf/__init__.py
+-rw-r--r--   0        0        0     2415 2023-05-31 00:19:23.716819 llama_hub-0.0.5/llama_hub/file/pymu_pdf/base.py
+-rw-r--r--   0        0        0        7 2023-05-31 00:19:23.716870 llama_hub-0.0.5/llama_hub/file/pymu_pdf/requirements.txt
+-rw-r--r--   0        0        0      890 2023-05-31 00:19:23.716967 llama_hub-0.0.5/llama_hub/file/rdf/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717033 llama_hub-0.0.5/llama_hub/file/rdf/__init__.py
+-rw-r--r--   0        0        0     2200 2023-06-27 01:05:04.207859 llama_hub-0.0.5/llama_hub/file/rdf/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:19:23.717167 llama_hub-0.0.5/llama_hub/file/rdf/requirements.txt
+-rw-r--r--   0        0        0      792 2023-05-31 00:19:23.717279 llama_hub-0.0.5/llama_hub/file/simple_csv/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717342 llama_hub-0.0.5/llama_hub/file/simple_csv/__init__.py
+-rw-r--r--   0        0        0     1244 2023-06-27 01:05:04.207963 llama_hub-0.0.5/llama_hub/file/simple_csv/base.py
+-rw-r--r--   0        0        0     2531 2023-05-31 00:19:23.717561 llama_hub-0.0.5/llama_hub/file/unstructured/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717635 llama_hub-0.0.5/llama_hub/file/unstructured/__init__.py
+-rw-r--r--   0        0        0     1345 2023-06-27 01:05:04.208090 llama_hub-0.0.5/llama_hub/file/unstructured/base.py
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.717763 llama_hub-0.0.5/llama_hub/file/unstructured/requirements.txt
+-rw-r--r--   0        0        0     1498 2023-06-10 07:58:38.772778 llama_hub-0.0.5/llama_hub/firestore/README.md
+-rw-r--r--   0        0        0       17 2023-06-10 07:58:38.772830 llama_hub-0.0.5/llama_hub/firestore/__init__.py
+-rw-r--r--   0        0        0     2236 2023-06-27 01:05:04.208204 llama_hub-0.0.5/llama_hub/firestore/base.py
+-rw-r--r--   0        0        0       23 2023-06-10 07:58:38.772997 llama_hub-0.0.5/llama_hub/firestore/requirements.txt
+-rw-r--r--   0        0        0     3141 2023-06-10 07:58:38.773157 llama_hub-0.0.5/llama_hub/github_repo/README.md
+-rw-r--r--   0        0        0      153 2023-05-31 00:19:23.717979 llama_hub-0.0.5/llama_hub/github_repo/__init__.py
+-rw-r--r--   0        0        0    20914 2023-06-03 03:50:30.194900 llama_hub-0.0.5/llama_hub/github_repo/base.py
+-rw-r--r--   0        0        0    12720 2023-06-27 01:05:04.208341 llama_hub-0.0.5/llama_hub/github_repo/github_client.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.718740 llama_hub-0.0.5/llama_hub/github_repo/requirements.txt
+-rw-r--r--   0        0        0     5663 2023-06-27 01:05:04.208451 llama_hub-0.0.5/llama_hub/github_repo/utils.py
+-rw-r--r--   0        0        0     2280 2023-06-27 01:05:04.208604 llama_hub-0.0.5/llama_hub/github_repo_issues/README.md
+-rw-r--r--   0        0        0      177 2023-06-27 01:05:04.208667 llama_hub-0.0.5/llama_hub/github_repo_issues/__init__.py
+-rw-r--r--   0        0        0     7714 2023-06-27 01:05:04.208747 llama_hub-0.0.5/llama_hub/github_repo_issues/base.py
+-rw-r--r--   0        0        0     6497 2023-06-27 01:05:04.208818 llama_hub-0.0.5/llama_hub/github_repo_issues/github_client.py
+-rw-r--r--   0        0        0        5 2023-06-27 01:05:04.208872 llama_hub-0.0.5/llama_hub/github_repo_issues/requirements.txt
+-rw-r--r--   0        0        0      948 2023-05-31 00:19:23.719165 llama_hub-0.0.5/llama_hub/gmail/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.719238 llama_hub-0.0.5/llama_hub/gmail/__init__.py
+-rw-r--r--   0        0        0     5289 2023-06-27 01:05:04.209018 llama_hub-0.0.5/llama_hub/gmail/base.py
+-rw-r--r--   0        0        0       81 2023-05-31 00:19:23.719438 llama_hub-0.0.5/llama_hub/gmail/requirements.txt
+-rw-r--r--   0        0        0     1364 2023-05-31 00:19:23.719568 llama_hub-0.0.5/llama_hub/google_calendar/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.719630 llama_hub-0.0.5/llama_hub/google_calendar/__init__.py
+-rw-r--r--   0        0        0     4760 2023-06-27 01:05:04.209147 llama_hub-0.0.5/llama_hub/google_calendar/base.py
+-rw-r--r--   0        0        0       66 2023-05-31 00:19:23.719771 llama_hub-0.0.5/llama_hub/google_calendar/requirements.txt
+-rw-r--r--   0        0        0     2571 2023-05-31 00:19:23.719884 llama_hub-0.0.5/llama_hub/google_docs/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.719942 llama_hub-0.0.5/llama_hub/google_docs/__init__.py
+-rw-r--r--   0        0        0     5295 2023-06-27 01:05:04.209374 llama_hub-0.0.5/llama_hub/google_docs/base.py
+-rw-r--r--   0        0        0       66 2023-05-31 00:19:23.720074 llama_hub-0.0.5/llama_hub/google_docs/requirements.txt
+-rw-r--r--   0        0        0     1807 2023-05-31 00:19:23.720187 llama_hub-0.0.5/llama_hub/google_drive/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.720244 llama_hub-0.0.5/llama_hub/google_drive/__init__.py
+-rw-r--r--   0        0        0    14112 2023-06-27 01:05:04.209675 llama_hub-0.0.5/llama_hub/google_drive/base.py
+-rw-r--r--   0        0        0       76 2023-05-31 00:19:23.720583 llama_hub-0.0.5/llama_hub/google_drive/requirements.txt
+-rw-r--r--   0        0        0     1150 2023-05-31 00:19:23.720701 llama_hub-0.0.5/llama_hub/google_sheets/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.720755 llama_hub-0.0.5/llama_hub/google_sheets/__init__.py
+-rw-r--r--   0        0        0     4994 2023-06-27 01:05:04.209852 llama_hub-0.0.5/llama_hub/google_sheets/base.py
+-rw-r--r--   0        0        0       66 2023-05-31 00:19:23.720914 llama_hub-0.0.5/llama_hub/google_sheets/requirements.txt
+-rw-r--r--   0        0        0      809 2023-05-31 00:19:23.721050 llama_hub-0.0.5/llama_hub/gpt_repo/README.md
+-rw-r--r--   0        0        0       17 2023-06-27 01:05:04.209962 llama_hub-0.0.5/llama_hub/gpt_repo/__init__.py
+-rw-r--r--   0        0        0     5493 2023-06-27 01:05:04.210066 llama_hub-0.0.5/llama_hub/gpt_repo/base.py
+-rw-r--r--   0        0        0     1595 2023-05-31 00:19:23.721376 llama_hub-0.0.5/llama_hub/graphdb_cypher/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.721443 llama_hub-0.0.5/llama_hub/graphdb_cypher/__init__.py
+-rw-r--r--   0        0        0     1786 2023-06-27 01:05:04.210177 llama_hub-0.0.5/llama_hub/graphdb_cypher/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.721683 llama_hub-0.0.5/llama_hub/graphdb_cypher/requirements.txt
+-rw-r--r--   0        0        0     1215 2023-05-31 00:19:23.721834 llama_hub-0.0.5/llama_hub/graphql/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.721886 llama_hub-0.0.5/llama_hub/graphql/__init__.py
+-rw-r--r--   0        0        0     2119 2023-06-27 01:05:04.210415 llama_hub-0.0.5/llama_hub/graphql/base.py
+-rw-r--r--   0        0        0       21 2023-05-31 00:19:23.722048 llama_hub-0.0.5/llama_hub/graphql/requirements.txt
+-rw-r--r--   0        0        0      969 2023-05-31 00:19:23.722173 llama_hub-0.0.5/llama_hub/hatena_blog/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.722225 llama_hub-0.0.5/llama_hub/hatena_blog/__init__.py
+-rw-r--r--   0        0        0     2770 2023-06-27 01:05:04.210532 llama_hub-0.0.5/llama_hub/hatena_blog/base.py
+-rw-r--r--   0        0        0       28 2023-05-31 00:19:23.722405 llama_hub-0.0.5/llama_hub/hatena_blog/requirements.txt
+-rw-r--r--   0        0        0      916 2023-05-31 00:19:23.722570 llama_hub-0.0.5/llama_hub/hubspot/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.722654 llama_hub-0.0.5/llama_hub/hubspot/__init__.py
+-rw-r--r--   0        0        0     1411 2023-06-27 01:05:04.210631 llama_hub-0.0.5/llama_hub/hubspot/base.py
+-rw-r--r--   0        0        0       18 2023-05-31 00:19:23.722823 llama_hub-0.0.5/llama_hub/hubspot/requirements.txt
+-rw-r--r--   0        0        0     1035 2023-05-31 00:19:23.722974 llama_hub-0.0.5/llama_hub/huggingface/fs/README.md
+-rw-r--r--   0        0        0       19 2023-06-27 01:05:04.210725 llama_hub-0.0.5/llama_hub/huggingface/fs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-06-27 01:05:04.210825 llama_hub-0.0.5/llama_hub/huggingface/fs/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:19:23.723269 llama_hub-0.0.5/llama_hub/huggingface/fs/requirements.txt
+-rw-r--r--   0        0        0      797 2023-05-31 00:19:23.723369 llama_hub-0.0.5/llama_hub/intercom/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.723425 llama_hub-0.0.5/llama_hub/intercom/__init__.py
+-rw-r--r--   0        0        0     2390 2023-06-27 01:05:04.210929 llama_hub-0.0.5/llama_hub/intercom/base.py
+-rw-r--r--   0        0        0       39 2023-05-31 00:19:23.723542 llama_hub-0.0.5/llama_hub/intercom/requirements.txt
+-rw-r--r--   0        0        0      808 2023-06-10 07:58:38.773924 llama_hub-0.0.5/llama_hub/jira/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.723719 llama_hub-0.0.5/llama_hub/jira/__init__.py
+-rw-r--r--   0        0        0     3545 2023-06-27 01:05:04.211048 llama_hub-0.0.5/llama_hub/jira/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.723892 llama_hub-0.0.5/llama_hub/jira/requirements.txt
+-rw-r--r--   0        0        0     1362 2023-05-31 00:19:23.724041 llama_hub-0.0.5/llama_hub/joplin/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.724074 llama_hub-0.0.5/llama_hub/joplin/__init__.py
+-rw-r--r--   0        0        0     5179 2023-06-27 01:05:04.211155 llama_hub-0.0.5/llama_hub/joplin/base.py
+-rw-r--r--   0        0        0      698 2023-05-31 00:19:23.724418 llama_hub-0.0.5/llama_hub/jsondata/README.md
+-rw-r--r--   0        0        0       17 2023-06-27 01:05:04.211259 llama_hub-0.0.5/llama_hub/jsondata/__init__.py
+-rw-r--r--   0        0        0     1617 2023-06-27 01:05:04.211365 llama_hub-0.0.5/llama_hub/jsondata/base.py
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.724577 llama_hub-0.0.5/llama_hub/jsondata/requirements.txt
+-rw-r--r--   0        0        0     7206 2023-05-31 00:19:23.724774 llama_hub-0.0.5/llama_hub/kaltura/esearch/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.724845 llama_hub-0.0.5/llama_hub/kaltura/esearch/__init__.py
+-rw-r--r--   0        0        0    12207 2023-06-27 01:05:04.211499 llama_hub-0.0.5/llama_hub/kaltura/esearch/base.py
+-rw-r--r--   0        0        0       24 2023-05-31 00:19:23.725038 llama_hub-0.0.5/llama_hub/kaltura/esearch/requirements.txt
+-rw-r--r--   0        0        0      785 2023-06-24 06:49:58.686157 llama_hub-0.0.5/llama_hub/kibela/README.md
+-rw-r--r--   0        0        0       17 2023-06-24 06:49:58.686207 llama_hub-0.0.5/llama_hub/kibela/__init__.py
+-rw-r--r--   0        0        0     3103 2023-06-27 01:05:04.211707 llama_hub-0.0.5/llama_hub/kibela/base.py
+-rw-r--r--   0        0        0        4 2023-06-24 06:49:58.686394 llama_hub-0.0.5/llama_hub/kibela/requirements.txt
+-rw-r--r--   0        0        0    12236 2023-06-27 01:05:04.211840 llama_hub-0.0.5/llama_hub/library.json
+-rw-r--r--   0        0        0     1117 2023-05-31 00:19:23.725289 llama_hub-0.0.5/llama_hub/make_com/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.725348 llama_hub-0.0.5/llama_hub/make_com/__init__.py
+-rw-r--r--   0        0        0     1708 2023-06-27 01:05:04.211941 llama_hub-0.0.5/llama_hub/make_com/base.py
+-rw-r--r--   0        0        0      810 2023-05-31 00:19:23.725515 llama_hub-0.0.5/llama_hub/mangoapps_guides/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.725566 llama_hub-0.0.5/llama_hub/mangoapps_guides/__init__.py
+-rw-r--r--   0        0        0     4784 2023-06-27 01:05:04.212048 llama_hub-0.0.5/llama_hub/mangoapps_guides/base.py
+-rw-r--r--   0        0        0       39 2023-05-31 00:19:23.725706 llama_hub-0.0.5/llama_hub/mangoapps_guides/requirements.txt
+-rw-r--r--   0        0        0     2740 2023-05-31 00:19:23.725850 llama_hub-0.0.5/llama_hub/maps/README.md
+-rw-r--r--   0        0        0       17 2023-06-27 01:05:04.212139 llama_hub-0.0.5/llama_hub/maps/__init__.py
+-rw-r--r--   0        0        0     4603 2023-06-27 01:05:04.212241 llama_hub-0.0.5/llama_hub/maps/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:19:23.726327 llama_hub-0.0.5/llama_hub/maps/requirements.txt
+-rw-r--r--   0        0        0      870 2023-05-31 00:19:23.726449 llama_hub-0.0.5/llama_hub/memos/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.726502 llama_hub-0.0.5/llama_hub/memos/__init__.py
+-rw-r--r--   0        0        0     1470 2023-06-27 01:05:04.212330 llama_hub-0.0.5/llama_hub/memos/base.py
+-rw-r--r--   0        0        0      952 2023-05-31 00:19:23.726641 llama_hub-0.0.5/llama_hub/metal/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.726693 llama_hub-0.0.5/llama_hub/metal/__init__.py
+-rw-r--r--   0        0        0     2326 2023-05-31 00:19:23.726764 llama_hub-0.0.5/llama_hub/metal/base.py
+-rw-r--r--   0        0        0       10 2023-05-31 00:19:23.726825 llama_hub-0.0.5/llama_hub/metal/requirements.txt
+-rw-r--r--   0        0        0     1174 2023-05-31 00:19:23.726943 llama_hub-0.0.5/llama_hub/milvus/README.md
+-rw-r--r--   0        0        0       19 2023-06-27 01:05:04.212408 llama_hub-0.0.5/llama_hub/milvus/__init__.py
+-rw-r--r--   0        0        0     4588 2023-05-31 00:19:23.727112 llama_hub-0.0.5/llama_hub/milvus/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.727182 llama_hub-0.0.5/llama_hub/milvus/requirements.txt
+-rw-r--r--   0        0        0      853 2023-05-31 00:19:23.727268 llama_hub-0.0.5/llama_hub/mondaydotcom/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.727321 llama_hub-0.0.5/llama_hub/mondaydotcom/__init__.py
+-rw-r--r--   0        0        0     2703 2023-06-27 01:05:04.212512 llama_hub-0.0.5/llama_hub/mondaydotcom/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.727432 llama_hub-0.0.5/llama_hub/mondaydotcom/requirements.txt
+-rw-r--r--   0        0        0      973 2023-05-31 00:19:23.727516 llama_hub-0.0.5/llama_hub/mongo/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.727566 llama_hub-0.0.5/llama_hub/mongo/__init__.py
+-rw-r--r--   0        0        0     2265 2023-06-27 01:05:04.212611 llama_hub-0.0.5/llama_hub/mongo/base.py
+-rw-r--r--   0        0        0        7 2023-05-31 00:19:23.727743 llama_hub-0.0.5/llama_hub/mongo/requirements.txt
+-rw-r--r--   0        0        0      916 2023-05-31 00:19:23.727849 llama_hub-0.0.5/llama_hub/notion/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.727909 llama_hub-0.0.5/llama_hub/notion/__init__.py
+-rw-r--r--   0        0        0     6126 2023-06-27 01:05:04.212712 llama_hub-0.0.5/llama_hub/notion/base.py
+-rw-r--r--   0        0        0      395 2023-06-01 05:01:36.458116 llama_hub-0.0.5/llama_hub/notion/tool.py
+-rw-r--r--   0        0        0      688 2023-05-31 00:19:23.728057 llama_hub-0.0.5/llama_hub/obsidian/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.728106 llama_hub-0.0.5/llama_hub/obsidian/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-31 00:19:23.728167 llama_hub-0.0.5/llama_hub/obsidian/base.py
+-rw-r--r--   0        0        0     1050 2023-05-31 00:19:23.728304 llama_hub-0.0.5/llama_hub/opendal_reader/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.728335 llama_hub-0.0.5/llama_hub/opendal_reader/__init__.py
+-rw-r--r--   0        0        0      980 2023-05-31 00:19:23.728466 llama_hub-0.0.5/llama_hub/opendal_reader/azblob/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.728521 llama_hub-0.0.5/llama_hub/opendal_reader/azblob/__init__.py
+-rw-r--r--   0        0        0     2472 2023-06-27 01:05:04.212815 llama_hub-0.0.5/llama_hub/opendal_reader/azblob/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.728751 llama_hub-0.0.5/llama_hub/opendal_reader/azblob/requirements.txt
+-rw-r--r--   0        0        0     2970 2023-06-27 01:05:04.212918 llama_hub-0.0.5/llama_hub/opendal_reader/base.py
+-rw-r--r--   0        0        0      999 2023-05-31 00:19:23.729020 llama_hub-0.0.5/llama_hub/opendal_reader/gcs/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.729087 llama_hub-0.0.5/llama_hub/opendal_reader/gcs/__init__.py
+-rw-r--r--   0        0        0     2290 2023-06-27 01:05:04.213008 llama_hub-0.0.5/llama_hub/opendal_reader/gcs/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729283 llama_hub-0.0.5/llama_hub/opendal_reader/gcs/requirements.txt
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729358 llama_hub-0.0.5/llama_hub/opendal_reader/requirements.txt
+-rw-r--r--   0        0        0     1397 2023-05-31 00:19:23.729481 llama_hub-0.0.5/llama_hub/opendal_reader/s3/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.729530 llama_hub-0.0.5/llama_hub/opendal_reader/s3/__init__.py
+-rw-r--r--   0        0        0     2601 2023-06-27 01:05:04.213107 llama_hub-0.0.5/llama_hub/opendal_reader/s3/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729714 llama_hub-0.0.5/llama_hub/opendal_reader/s3/requirements.txt
+-rw-r--r--   0        0        0     2147 2023-05-31 00:19:23.729798 llama_hub-0.0.5/llama_hub/outlook_localcalendar/README.md
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.729846 llama_hub-0.0.5/llama_hub/outlook_localcalendar/__init__,py
+-rw-r--r--   0        0        0     3944 2023-06-27 01:05:04.213216 llama_hub-0.0.5/llama_hub/outlook_localcalendar/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.730022 llama_hub-0.0.5/llama_hub/outlook_localcalendar/requirements.txt
+-rw-r--r--   0        0        0     1801 2023-05-31 00:19:23.730149 llama_hub-0.0.5/llama_hub/pandas_ai/README.md
+-rw-r--r--   0        0        0       19 2023-06-27 01:05:04.213297 llama_hub-0.0.5/llama_hub/pandas_ai/__init__.py
+-rw-r--r--   0        0        0     3904 2023-06-27 01:05:04.213395 llama_hub-0.0.5/llama_hub/pandas_ai/base.py
+-rw-r--r--   0        0        0        8 2023-05-31 00:19:23.730434 llama_hub-0.0.5/llama_hub/pandas_ai/requirements.txt
+-rw-r--r--   0        0        0     1484 2023-05-31 00:19:23.730555 llama_hub-0.0.5/llama_hub/papers/arxiv/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.730614 llama_hub-0.0.5/llama_hub/papers/arxiv/__init__.py
+-rw-r--r--   0        0        0     6442 2023-06-27 01:05:04.213521 llama_hub-0.0.5/llama_hub/papers/arxiv/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.730795 llama_hub-0.0.5/llama_hub/papers/arxiv/requirements.txt
+-rw-r--r--   0        0        0      931 2023-05-31 00:19:23.730889 llama_hub-0.0.5/llama_hub/papers/pubmed/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.730947 llama_hub-0.0.5/llama_hub/papers/pubmed/__init__.py
+-rw-r--r--   0        0        0     6178 2023-06-27 01:05:04.213656 llama_hub-0.0.5/llama_hub/papers/pubmed/base.py
+-rw-r--r--   0        0        0     1279 2023-05-31 00:19:23.731154 llama_hub-0.0.5/llama_hub/pinecone/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.731210 llama_hub-0.0.5/llama_hub/pinecone/__init__.py
+-rw-r--r--   0        0        0     2587 2023-05-31 00:19:23.731290 llama_hub-0.0.5/llama_hub/pinecone/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:19:23.731346 llama_hub-0.0.5/llama_hub/pinecone/requirements.txt
+-rw-r--r--   0        0        0     1157 2023-05-31 00:19:23.731448 llama_hub-0.0.5/llama_hub/qdrant/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.731505 llama_hub-0.0.5/llama_hub/qdrant/__init__.py
+-rw-r--r--   0        0        0     6920 2023-05-31 00:19:23.731618 llama_hub-0.0.5/llama_hub/qdrant/base.py
+-rw-r--r--   0        0        0       13 2023-05-31 00:19:23.731674 llama_hub-0.0.5/llama_hub/qdrant/requirements.txt
+-rw-r--r--   0        0        0     1551 2023-05-31 00:19:23.731776 llama_hub-0.0.5/llama_hub/readwise/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.731833 llama_hub-0.0.5/llama_hub/readwise/__init__.py
+-rw-r--r--   0        0        0     1901 2023-06-27 01:05:04.213771 llama_hub-0.0.5/llama_hub/readwise/base.py
+-rw-r--r--   0        0        0     2707 2023-05-31 00:19:23.732014 llama_hub-0.0.5/llama_hub/reddit/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.732079 llama_hub-0.0.5/llama_hub/reddit/__init__.py
+-rw-r--r--   0        0        0     1924 2023-06-27 01:05:04.213875 llama_hub-0.0.5/llama_hub/reddit/base.py
+-rw-r--r--   0        0        0       81 2023-05-31 00:19:23.732202 llama_hub-0.0.5/llama_hub/reddit/requirements.txt
+-rw-r--r--   0        0        0     1330 2023-05-31 00:19:23.732308 llama_hub-0.0.5/llama_hub/remote/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.732382 llama_hub-0.0.5/llama_hub/remote/__init__.py
+-rw-r--r--   0        0        0     3170 2023-06-27 01:05:04.214197 llama_hub-0.0.5/llama_hub/remote/base.py
+-rw-r--r--   0        0        0     1383 2023-05-31 00:19:23.732627 llama_hub-0.0.5/llama_hub/remote_depth/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.732655 llama_hub-0.0.5/llama_hub/remote_depth/__init__.py
+-rw-r--r--   0        0        0     3830 2023-06-27 01:05:04.214339 llama_hub-0.0.5/llama_hub/remote_depth/base.py
+-rw-r--r--   0        0        0       31 2023-05-31 00:19:23.732887 llama_hub-0.0.5/llama_hub/remote_depth/requirements.txt
+-rw-r--r--   0        0        0     1669 2023-05-31 00:19:23.732997 llama_hub-0.0.5/llama_hub/s3/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.733053 llama_hub-0.0.5/llama_hub/s3/__init__.py
+-rw-r--r--   0        0        0     3984 2023-06-27 01:05:04.214456 llama_hub-0.0.5/llama_hub/s3/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.733253 llama_hub-0.0.5/llama_hub/s3/requirements.txt
+-rw-r--r--   0        0        0      821 2023-05-31 00:19:23.733394 llama_hub-0.0.5/llama_hub/slack/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.733459 llama_hub-0.0.5/llama_hub/slack/__init__.py
+-rw-r--r--   0        0        0     7494 2023-06-27 01:05:04.214578 llama_hub-0.0.5/llama_hub/slack/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:19:23.733594 llama_hub-0.0.5/llama_hub/slack/requirements.txt
+-rw-r--r--   0        0        0      690 2023-05-31 00:19:23.733754 llama_hub-0.0.5/llama_hub/snscrape_twitter/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.733815 llama_hub-0.0.5/llama_hub/snscrape_twitter/__init__.py
+-rw-r--r--   0        0        0     1176 2023-06-27 01:05:04.214673 llama_hub-0.0.5/llama_hub/snscrape_twitter/base.py
+-rw-r--r--   0        0        0       56 2023-05-31 00:19:23.734041 llama_hub-0.0.5/llama_hub/snscrape_twitter/requirements.txt
+-rw-r--r--   0        0        0     1662 2023-05-31 00:19:23.734145 llama_hub-0.0.5/llama_hub/spotify/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.734204 llama_hub-0.0.5/llama_hub/spotify/__init__.py
+-rw-r--r--   0        0        0     2302 2023-06-27 01:05:04.214758 llama_hub-0.0.5/llama_hub/spotify/base.py
+-rw-r--r--   0        0        0        7 2023-05-31 00:19:23.734331 llama_hub-0.0.5/llama_hub/spotify/requirements.txt
+-rw-r--r--   0        0        0      846 2023-05-31 00:19:23.734458 llama_hub-0.0.5/llama_hub/stackoverflow/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.734518 llama_hub-0.0.5/llama_hub/stackoverflow/__init__.py
+-rw-r--r--   0        0        0     6486 2023-06-27 01:05:04.214885 llama_hub-0.0.5/llama_hub/stackoverflow/base.py
+-rw-r--r--   0        0        0       21 2023-05-31 00:19:23.734708 llama_hub-0.0.5/llama_hub/stackoverflow/requirements.txt
+-rw-r--r--   0        0        0      936 2023-05-31 00:19:23.734832 llama_hub-0.0.5/llama_hub/steamship/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.734866 llama_hub-0.0.5/llama_hub/steamship/__init__.py
+-rw-r--r--   0        0        0     3498 2023-05-31 00:19:23.734974 llama_hub-0.0.5/llama_hub/steamship/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:19:23.735057 llama_hub-0.0.5/llama_hub/steamship/requirements.txt
+-rw-r--r--   0        0        0      726 2023-05-31 00:19:23.735154 llama_hub-0.0.5/llama_hub/string_iterable/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.735234 llama_hub-0.0.5/llama_hub/string_iterable/__init__.py
+-rw-r--r--   0        0        0      974 2023-06-27 01:05:04.214972 llama_hub-0.0.5/llama_hub/string_iterable/base.py
+-rw-r--r--   0        0        0      676 2023-05-31 00:19:23.735435 llama_hub-0.0.5/llama_hub/trello/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.735493 llama_hub-0.0.5/llama_hub/trello/__init__.py
+-rw-r--r--   0        0        0     1441 2023-06-27 01:05:04.215067 llama_hub-0.0.5/llama_hub/trello/base.py
+-rw-r--r--   0        0        0       10 2023-05-31 00:19:23.735672 llama_hub-0.0.5/llama_hub/trello/requirements.txt
+-rw-r--r--   0        0        0      924 2023-05-31 00:19:23.735778 llama_hub-0.0.5/llama_hub/twitter/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.735847 llama_hub-0.0.5/llama_hub/twitter/__init__.py
+-rw-r--r--   0        0        0     1782 2023-06-27 01:05:04.215155 llama_hub-0.0.5/llama_hub/twitter/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.735976 llama_hub-0.0.5/llama_hub/twitter/requirements.txt
+-rw-r--r--   0        0        0      629 2023-06-27 01:05:04.215231 llama_hub-0.0.5/llama_hub/utils.py
+-rw-r--r--   0        0        0     1162 2023-05-31 00:19:23.736420 llama_hub-0.0.5/llama_hub/weather/README.md
+-rw-r--r--   0        0        0       17 2023-06-27 01:05:04.215312 llama_hub-0.0.5/llama_hub/weather/__init__.py
+-rw-r--r--   0        0        0     2873 2023-06-27 01:05:04.215403 llama_hub-0.0.5/llama_hub/weather/base.py
+-rw-r--r--   0        0        0        5 2023-05-31 00:19:23.736662 llama_hub-0.0.5/llama_hub/weather/requirements.txt
+-rw-r--r--   0        0        0     1525 2023-05-31 00:19:23.736765 llama_hub-0.0.5/llama_hub/weaviate/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.736823 llama_hub-0.0.5/llama_hub/weaviate/__init__.py
+-rw-r--r--   0        0        0     3697 2023-05-31 00:19:23.736889 llama_hub-0.0.5/llama_hub/weaviate/base.py
+-rw-r--r--   0        0        0       15 2023-05-31 00:19:23.736940 llama_hub-0.0.5/llama_hub/weaviate/requirements.txt
+-rw-r--r--   0        0        0     1163 2023-06-27 01:05:04.215535 llama_hub-0.0.5/llama_hub/web/async_web/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.737136 llama_hub-0.0.5/llama_hub/web/async_web/__init__.py
+-rw-r--r--   0        0        0     2559 2023-06-27 01:05:04.215642 llama_hub-0.0.5/llama_hub/web/async_web/base.py
+-rw-r--r--   0        0        0       18 2023-05-31 00:19:23.737325 llama_hub-0.0.5/llama_hub/web/async_web/requirements.txt
+-rw-r--r--   0        0        0     3446 2023-05-31 00:19:23.737437 llama_hub-0.0.5/llama_hub/web/beautiful_soup_web/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.737504 llama_hub-0.0.5/llama_hub/web/beautiful_soup_web/__init__.py
+-rw-r--r--   0        0        0     6793 2023-06-27 01:05:04.215772 llama_hub-0.0.5/llama_hub/web/beautiful_soup_web/base.py
+-rw-r--r--   0        0        0       31 2023-05-31 00:19:23.737666 llama_hub-0.0.5/llama_hub/web/beautiful_soup_web/requirements.txt
+-rw-r--r--   0        0        0     3672 2023-05-31 00:19:23.737782 llama_hub-0.0.5/llama_hub/web/knowledge_base/README.md
+-rw-r--r--   0        0        0        1 2023-05-31 00:19:23.737843 llama_hub-0.0.5/llama_hub/web/knowledge_base/__init__.py
+-rw-r--r--   0        0        0     5616 2023-06-27 01:05:04.215894 llama_hub-0.0.5/llama_hub/web/knowledge_base/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.737968 llama_hub-0.0.5/llama_hub/web/knowledge_base/requirements.txt
+-rw-r--r--   0        0        0     2681 2023-05-31 00:19:23.738073 llama_hub-0.0.5/llama_hub/web/readability_web/README.md
+-rw-r--r--   0        0        0    83319 2023-05-31 00:19:23.738443 llama_hub-0.0.5/llama_hub/web/readability_web/Readability.js
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.738513 llama_hub-0.0.5/llama_hub/web/readability_web/__init__.py
+-rw-r--r--   0        0        0     4627 2023-06-27 01:05:04.216041 llama_hub-0.0.5/llama_hub/web/readability_web/base.py
+-rw-r--r--   0        0        0       18 2023-05-31 00:19:23.738660 llama_hub-0.0.5/llama_hub/web/readability_web/requirements.txt
+-rw-r--r--   0        0        0      489 2023-05-31 00:19:23.738734 llama_hub-0.0.5/llama_hub/web/rss/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.738780 llama_hub-0.0.5/llama_hub/web/rss/__init__.py
+-rw-r--r--   0        0        0     1991 2023-06-27 01:05:04.216216 llama_hub-0.0.5/llama_hub/web/rss/base.py
+-rw-r--r--   0        0        0     1994 2023-05-31 00:19:23.738914 llama_hub-0.0.5/llama_hub/web/simple_web/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.738959 llama_hub-0.0.5/llama_hub/web/simple_web/__init__.py
+-rw-r--r--   0        0        0     1262 2023-06-27 01:05:04.216373 llama_hub-0.0.5/llama_hub/web/simple_web/base.py
+-rw-r--r--   0        0        0        9 2023-05-31 00:19:23.739081 llama_hub-0.0.5/llama_hub/web/simple_web/requirements.txt
+-rw-r--r--   0        0        0     1731 2023-06-27 01:05:04.216507 llama_hub-0.0.5/llama_hub/web/sitemap/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 01:05:04.216547 llama_hub-0.0.5/llama_hub/web/sitemap/__init__.py
+-rw-r--r--   0        0        0     2110 2023-06-27 01:05:04.216636 llama_hub-0.0.5/llama_hub/web/sitemap/base.py
+-rw-r--r--   0        0        0        0 2023-06-27 01:05:04.216672 llama_hub-0.0.5/llama_hub/web/sitemap/requirements.txt
+-rw-r--r--   0        0        0     2009 2023-05-31 00:19:23.739158 llama_hub-0.0.5/llama_hub/web/trafilatura_web/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739207 llama_hub-0.0.5/llama_hub/web/trafilatura_web/__init__.py
+-rw-r--r--   0        0        0      894 2023-06-27 01:05:04.216806 llama_hub-0.0.5/llama_hub/web/trafilatura_web/base.py
+-rw-r--r--   0        0        0       16 2023-05-31 00:19:23.739305 llama_hub-0.0.5/llama_hub/web/trafilatura_web/requirements.txt
+-rw-r--r--   0        0        0     1075 2023-05-31 00:19:23.739438 llama_hub-0.0.5/llama_hub/web/unstructured_web/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 00:19:23.739468 llama_hub-0.0.5/llama_hub/web/unstructured_web/__init__.py
+-rw-r--r--   0        0        0     2255 2023-06-27 01:05:04.216918 llama_hub-0.0.5/llama_hub/web/unstructured_web/base.py
+-rw-r--r--   0        0        0       12 2023-05-31 00:19:23.739609 llama_hub-0.0.5/llama_hub/web/unstructured_web/requirements.txt
+-rw-r--r--   0        0        0     1315 2023-05-31 00:19:23.739686 llama_hub-0.0.5/llama_hub/whatsapp/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739729 llama_hub-0.0.5/llama_hub/whatsapp/__init__.py
+-rw-r--r--   0        0        0     1586 2023-06-27 01:05:04.217028 llama_hub-0.0.5/llama_hub/whatsapp/base.py
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739818 llama_hub-0.0.5/llama_hub/whatsapp/requirements.txt
+-rw-r--r--   0        0        0      895 2023-05-31 00:19:23.739897 llama_hub-0.0.5/llama_hub/wikipedia/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.739946 llama_hub-0.0.5/llama_hub/wikipedia/__init__.py
+-rw-r--r--   0        0        0      837 2023-06-27 01:05:04.217152 llama_hub-0.0.5/llama_hub/wikipedia/base.py
+-rw-r--r--   0        0        0       14 2023-05-31 00:19:23.740060 llama_hub-0.0.5/llama_hub/wikipedia/requirements.txt
+-rw-r--r--   0        0        0     1042 2023-05-31 00:19:23.740135 llama_hub-0.0.5/llama_hub/wordpress/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.740190 llama_hub-0.0.5/llama_hub/wordpress/__init__.py
+-rw-r--r--   0        0        0     2546 2023-05-31 00:19:23.740248 llama_hub-0.0.5/llama_hub/wordpress/base.py
+-rw-r--r--   0        0        0       39 2023-05-31 00:19:23.740291 llama_hub-0.0.5/llama_hub/wordpress/requirements.txt
+-rw-r--r--   0        0        0      774 2023-05-31 00:19:23.740378 llama_hub-0.0.5/llama_hub/youtube_transcript/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.740429 llama_hub-0.0.5/llama_hub/youtube_transcript/__init__.py
+-rw-r--r--   0        0        0     1681 2023-06-27 01:05:04.217272 llama_hub-0.0.5/llama_hub/youtube_transcript/base.py
+-rw-r--r--   0        0        0       29 2023-05-31 00:19:23.740552 llama_hub-0.0.5/llama_hub/youtube_transcript/requirements.txt
+-rw-r--r--   0        0        0      884 2023-05-31 00:19:23.740654 llama_hub-0.0.5/llama_hub/zendesk/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.740708 llama_hub-0.0.5/llama_hub/zendesk/__init__.py
+-rw-r--r--   0        0        0     2328 2023-06-27 01:05:04.217395 llama_hub-0.0.5/llama_hub/zendesk/base.py
+-rw-r--r--   0        0        0       24 2023-05-31 00:19:23.740869 llama_hub-0.0.5/llama_hub/zendesk/requirements.txt
+-rw-r--r--   0        0        0     1304 2023-05-31 00:19:23.740971 llama_hub-0.0.5/llama_hub/zulip/README.md
+-rw-r--r--   0        0        0       17 2023-05-31 00:19:23.741018 llama_hub-0.0.5/llama_hub/zulip/__init__.py
+-rw-r--r--   0        0        0     2458 2023-06-27 01:05:04.217525 llama_hub-0.0.5/llama_hub/zulip/base.py
+-rw-r--r--   0        0        0        6 2023-05-31 00:19:23.741155 llama_hub-0.0.5/llama_hub/zulip/requirements.txt
+-rw-r--r--   0        0        0      883 2023-06-27 01:05:27.618116 llama_hub-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7508 1970-01-01 00:00:00.000000 llama_hub-0.0.5/PKG-INFO
```

### Comparing `llama_hub-0.0.4/LICENSE` & `llama_hub-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/README.md` & `llama_hub-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -133,14 +133,18 @@
 python3.9 -m venv .venv
 source .venv/bin/activate 
 pip3 install -r test_requirements.txt
 
 poetry run pytest tests 
 ```
 
+## Changelog
+
+If you want to track the latest version updates / see which loaders are added to each release, take a look at our [full changelog here](https://github.com/emptycrown/llama-hub/blob/main/CHANGELOG.md)! 
+
 ## FAQ
 
 ### How do I test my loader before it's merged?
 
 There is an argument called `loader_hub_url` in [`download_loader`](https://github.com/jerryjliu/llama_index/blob/main/llama_index/readers/download.py) that defaults to the main branch of this repo. You can set it to your branch or fork to test your new loader.
 
 ### Should I create a PR against LlamaHub or the LlamaIndex repo directly?
```

### Comparing `llama_hub-0.0.4/llama_hub/airtable/README.md` & `llama_hub-0.0.5/llama_hub/airtable/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/airtable/base.py` & `llama_hub-0.0.5/llama_hub/airtable/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 
 class AirtableReader(BaseReader):
     """Airtable reader. Reads data from a table in a base.
 
     Args:
         api_key (str): Airtable API key.
     """
-    
+
     def __init__(self, api_key: str) -> None:
         """Initialize Airtable reader."""
-        
 
         self.api_key = api_key
 
-    def load_data(self, base_id: str,table_id: str) -> List[Document]:
+    def load_data(self, base_id: str, table_id: str) -> List[Document]:
         """Load data from a table in a base
 
         Args:
             table_id (str): Table ID.
             base_id (str): Base ID.
         Returns:
             List[Document]: List of documents.
         """
         from pyairtable import Table
+
         table = Table(self.api_key, base_id, table_id)
-        all_records=table.all()
-        return [Document(f"{all_records}", extra_info={})]
+        all_records = table.all()
+        return [Document(text=f"{all_records}", extra_info={})]
```

### Comparing `llama_hub-0.0.4/llama_hub/apify/actor/README.md` & `llama_hub-0.0.5/llama_hub/apify/actor/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ```python
 from llama_index import download_loader
 from llama_index.readers.schema.base import Document
 
 # Converts a single record from the Actor's resulting dataset to the LlamaIndex format
 def tranform_dataset_item(item):
     return Document(
-        item.get("text"),
+        text=item.get("text"),
         extra_info={
             "url": item.get("url"),
         },
     )
 
 ApifyActor = download_loader("ApifyActor")
```

### Comparing `llama_hub-0.0.4/llama_hub/apify/actor/base.py` & `llama_hub-0.0.5/llama_hub/apify/actor/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
             build=build,
             memory_mbytes=memory_mbytes,
             timeout_secs=timeout_secs,
         )
 
         try:
             from llama_hub.utils import import_loader
+
             ApifyDataset = import_loader("ApifyDataset")
         except ImportError:
             ApifyDataset = download_loader("ApifyDataset")
 
         reader = ApifyDataset(self.apify_api_token)
         documents = reader.load_data(
             dataset_id=actor_call.get("defaultDatasetId"),
```

### Comparing `llama_hub-0.0.4/llama_hub/apify/dataset/README.md` & `llama_hub-0.0.5/llama_hub/apify/dataset/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 ```python
 from llama_index import download_loader
 from llama_index.readers.schema.base import Document
 
 # Converts a single record from the Apify dataset to the LlamaIndex format
 def tranform_dataset_item(item):
     return Document(
-        item.get("text"),
+        text=item.get("text"),
         extra_info={
             "url": item.get("url"),
         },
     )
 
 ApifyDataset = download_loader("ApifyDataset")
```

### Comparing `llama_hub-0.0.4/llama_hub/apify/dataset/base.py` & `llama_hub-0.0.5/llama_hub/apify/dataset/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Apify dataset reader"""
-from typing import Any, Callable, Dict, List
+from typing import Callable, Dict, List
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 
 class ApifyDataset(BaseReader):
     """Apify Dataset reader.
```

### Comparing `llama_hub-0.0.4/llama_hub/asana/README.md` & `llama_hub-0.0.5/llama_hub/asana/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/asana/base.py` & `llama_hub-0.0.5/llama_hub/asana/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             for task in tasks:
                 stories = self.client.tasks.stories(task["gid"], opt_fields="type,text")
                 comments = "\n".join(
                     [story["text"] for story in stories if story["type"] == "comment"]
                 )
                 results.append(
                     Document(
-                        task["name"] + " " + task["notes"] + " " + comments,
+                        text=task["name"] + " " + task["notes"] + " " + comments,
                         extra_info={
                             "task_id": task["gid"],
                             "name": task["name"],
                             "assignee": task["assignee"],
                             "project": project["name"],
                         },
                     )
```

### Comparing `llama_hub-0.0.4/llama_hub/azcognitive_search/README.md` & `llama_hub-0.0.5/llama_hub/azcognitive_search/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/azcognitive_search/base.py` & `llama_hub-0.0.5/llama_hub/azcognitive_search/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class AzCognitiveSearchReader(BaseReader):
     """General reader for any Azure Cognitive Search index reader.
 
     Args:
         service_name (str): the name of azure cognitive search service.
         search_key (str): provide azure search access key directly.
         index (str): index name
-    
+
     """
 
     def __init__(self, service_name: str, searck_key: str, index: str) -> None:
         """Initialize Azure cognitive search service using the search key."""
         import logging
 
         from azure.core.credentials import AzureKeyCredential
```

### Comparing `llama_hub-0.0.4/llama_hub/azstorage_blob/README.md` & `llama_hub-0.0.5/llama_hub/azstorage_blob/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/azstorage_blob/base.py` & `llama_hub-0.0.5/llama_hub/azstorage_blob/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 import tempfile
 import time
 import math
 from pathlib import Path
 from typing import Any, List, Optional, Union, Dict
 
 
-
 from llama_index import download_loader
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 logger = logging.getLogger(__name__)
 
+
 class AzStorageBlobReader(BaseReader):
-    """General reader for any Azure Storage Blob file or directory. 
+    """General reader for any Azure Storage Blob file or directory.
 
     Args:
         container_name (str): name of the container for the blob.
-        blob (Optional[str]): name of the file to download. If none specified          
+        blob (Optional[str]): name of the file to download. If none specified
             this loader will iterate through list of blobs in the container.
-        name_starts_with (Optional[str]): filter the list of blobs to download 
+        name_starts_with (Optional[str]): filter the list of blobs to download
             to only those whose names begin with the specified string.
-        include: (Union[str, List[str], None]): Specifies one or more additional 
-            datasets to include in the response. Options include: 'snapshots', 
-            'metadata', 'uncommittedblobs', 'copy', 'deleted', 
-            'deletedwithversions', 'tags', 'versions', 'immutabilitypolicy', 
+        include: (Union[str, List[str], None]): Specifies one or more additional
+            datasets to include in the response. Options include: 'snapshots',
+            'metadata', 'uncommittedblobs', 'copy', 'deleted',
+            'deletedwithversions', 'tags', 'versions', 'immutabilitypolicy',
             'legalhold'.
         file_extractor (Optional[Dict[str, Union[str, BaseReader]]]): A mapping of file
             extension to a BaseReader class that specifies how to convert that file
             to text. See `SimpleDirectoryReader` for more details.
         account_url (str): URI to the storage account, may include SAS token.
         credential (Union[str, Dict[str, str], AzureNamedKeyCredential, AzureSasCredential, TokenCredential, None] = None):
             The credentials with which to authenticate. This is optional if the account URL already has a SAS token.
@@ -42,81 +42,90 @@
 
     def __init__(
         self,
         *args: Any,
         container_name: str,
         blob: Optional[str] = None,
         name_starts_with: Optional[str] = None,
-        include: Optional[Any] = None, 
+        include: Optional[Any] = None,
         file_extractor: Optional[Dict[str, Union[str, BaseReader]]] = None,
         account_url: str,
         credential: Optional[Any] = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> None:
-        """Initializes Azure Storage Account
-        """
+        """Initializes Azure Storage Account"""
         super().__init__(*args, **kwargs)
 
         self.container_name = container_name
         self.blob = blob
         self.name_starts_with = name_starts_with
         self.include = include
 
         self.file_extractor = file_extractor
 
         self.account_url = account_url
         self.credential = credential
 
     def load_data(self) -> List[Document]:
         """Load file(s) from Azure Storage Blob"""
-        #from azure.core.credentials import AzureNamedKeyCredential, AzureSasCredential, TokenCredential
-        #from azure.storage.blob import BlobServiceClient, BlobClient, ContainerClient
+        # from azure.core.credentials import AzureNamedKeyCredential, AzureSasCredential, TokenCredential
+        # from azure.storage.blob import BlobServiceClient, BlobClient, ContainerClient
         from azure.storage.blob import ContainerClient
 
-
-        container_client = ContainerClient(self.account_url, self.container_name, credential=self.credential)
+        container_client = ContainerClient(
+            self.account_url, self.container_name, credential=self.credential
+        )
         total_download_start_time = time.time()
 
         with tempfile.TemporaryDirectory() as temp_dir:
             if self.blob:
                 extension = Path(self.blob).suffix
-                download_file_path = f"{temp_dir}/{next(tempfile._get_candidate_names())}{extension}"
+                download_file_path = (
+                    f"{temp_dir}/{next(tempfile._get_candidate_names())}{extension}"
+                )
                 logger.info(f"Start download of {self.blob}")
                 start_time = time.time()
                 stream = container_client.download_blob(self.blob)
                 with open(file=download_file_path, mode="wb") as download_file:
                     stream.readinto(download_file)
                 end_time = time.time()
                 logger.info(
                     f"{self.blob} downloaded in {end_time - start_time} seconds."
                 )
             else:
-                logger.info(f"Listing blobs")
-                blobs_list = container_client.list_blobs(self.name_starts_with, self.include)
+                logger.info("Listing blobs")
+                blobs_list = container_client.list_blobs(
+                    self.name_starts_with, self.include
+                )
                 for obj in blobs_list:
                     extension = Path(obj.name).suffix
-                    download_file_path = f"{temp_dir}/{next(tempfile._get_candidate_names())}{extension}"
+                    download_file_path = (
+                        f"{temp_dir}/{next(tempfile._get_candidate_names())}{extension}"
+                    )
                     logger.info(f"Start download of {obj.name}")
                     start_time = time.time()
                     stream = container_client.download_blob(obj)
                     with open(file=download_file_path, mode="wb") as download_file:
                         stream.readinto(download_file)
                     end_time = time.time()
                     logger.info(
                         f"{obj.name} downloaded in {end_time - start_time} seconds."
                     )
-            
+
             total_download_end_time = time.time()
-            total_elapsed_time = math.ceil(total_download_end_time - total_download_start_time)
-            logger.info(f"Downloading completed in approximately {total_elapsed_time // 60}min {total_elapsed_time % 60}s.")
-            logger.info(f"Document creation starting")
+            total_elapsed_time = math.ceil(
+                total_download_end_time - total_download_start_time
+            )
+            logger.info(
+                f"Downloading completed in approximately {total_elapsed_time // 60}min {total_elapsed_time % 60}s."
+            )
+            logger.info("Document creation starting")
 
             try:
                 from llama_hub.utils import import_loader
+
                 SimpleDirectoryReader = import_loader("SimpleDirectoryReader")
             except ImportError:
                 SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
             loader = SimpleDirectoryReader(temp_dir, file_extractor=self.file_extractor)
 
-            return loader.load_data()         
-
-
+            return loader.load_data()
```

### Comparing `llama_hub-0.0.4/llama_hub/bilibili/README.md` & `llama_hub-0.0.5/llama_hub/bilibili/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/bilibili/base.py` & `llama_hub-0.0.5/llama_hub/bilibili/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,13 +52,13 @@
         Returns:
             List[Document]: A list of Document objects, each containing the transcript for a Bilibili video.
         """
         results = []
         for bili_url in video_urls:
             try:
                 transcript = self.get_bilibili_info_and_subs(bili_url)
-                results.append(Document(transcript))
+                results.append(Document(text=transcript))
             except Exception as e:
                 warnings.warn(
                     f"Error loading transcript for video {bili_url}: {str(e)}. Skipping video."
                 )
         return results
```

### Comparing `llama_hub-0.0.4/llama_hub/boarddocs/BoardDocsReader.ipynb` & `llama_hub-0.0.5/llama_hub/boarddocs/BoardDocsReader.ipynb`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/boarddocs/README.md` & `llama_hub-0.0.5/llama_hub/boarddocs/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/boarddocs/base.py` & `llama_hub-0.0.5/llama_hub/boarddocs/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,46 +3,47 @@
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 import json
 import requests
 
+
 class BoardDocsReader(BaseReader):
     """BoardDocs doc reader.
 
     Read public agendas included on a BoardDocs site.
 
     Args:
         site (str): The BoardDocs site you'd like to index, e.g. "ca/redwood"
         committee_id (str): The committee on the site you want to index
     """
 
     def __init__(
         self,
-        site:str,
-        committee_id:str,
+        site: str,
+        committee_id: str,
     ) -> None:
         """Initialize with parameters."""
         self.site = site
         self.committee_id = committee_id
         self.base_url = "https://go.boarddocs.com/" + site + "/Board.nsf"
 
         # set up the headers required for the server to answer
         self.headers = {
             "accept": "application/json, text/javascript, */*; q=0.01",
             "accept-language": "en-US,en;q=0.9",
             "content-type": "application/x-www-form-urlencoded; charset=UTF-8",
-            "sec-ch-ua": "\"Google Chrome\";v=\"113\", \"Chromium\";v=\"113\", \"Not-A.Brand\";v=\"24\"",
+            "sec-ch-ua": '"Google Chrome";v="113", "Chromium";v="113", "Not-A.Brand";v="24"',
             "sec-ch-ua-mobile": "?0",
-            "sec-ch-ua-platform": "\"macOS\"",
+            "sec-ch-ua-platform": '"macOS"',
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "same-origin",
-            "x-requested-with": "XMLHttpRequest"
+            "x-requested-with": "XMLHttpRequest",
         }
         super().__init__()
 
     def get_meeting_list(self) -> List[dict]:
         """
         Returns a list of meetings for the committee
 
@@ -53,23 +54,27 @@
         """
         meeting_list_url = self.base_url + "/BD-GetMeetingsList?open"
 
         data = "current_committee_id=" + self.committee_id
         response = requests.post(meeting_list_url, headers=self.headers, data=data)
         meetingsData = json.loads(response.text)
 
-        meetings = [{"meetingID": meeting.get('unique', None),
-                    "date": meeting.get('numberdate', None),
-                    "unid": meeting.get('unid', None)} for meeting in meetingsData]
+        meetings = [
+            {
+                "meetingID": meeting.get("unique", None),
+                "date": meeting.get("numberdate", None),
+                "unid": meeting.get("unid", None),
+            }
+            for meeting in meetingsData
+        ]
         return meetings
 
-
-    def process_meeting(self,
-                       meeting_id:str,
-                       index_pdfs:bool = True) -> List[Document]:
+    def process_meeting(
+        self, meeting_id: str, index_pdfs: bool = True
+    ) -> List[Document]:
         """
         Returns documents from the given meeting
         """
 
         agenda_url = self.base_url + "/PRINT-AgendaDetailed"
 
         # set the meetingID & committee
@@ -79,47 +84,50 @@
         response = requests.post(agenda_url, headers=self.headers, data=data)
 
         import html2text
         from bs4 import BeautifulSoup
 
         # parse the returned HTML
         soup = BeautifulSoup(response.content, "html.parser")
-        agenda_date = soup.find("div", {"class":"print-meeting-date"}).string
-        agenda_title = soup.find("div", {"class":"print-meeting-name"}).string
-        agenda_files = [fd.a.get('href') for fd in soup.find_all("div", {"class":"public-file"})]
+        agenda_date = soup.find("div", {"class": "print-meeting-date"}).string
+        agenda_title = soup.find("div", {"class": "print-meeting-name"}).string
+        [
+            fd.a.get("href") for fd in soup.find_all("div", {"class": "public-file"})
+        ]
         agenda_data = html2text.html2text(response.text)
 
         # TODO: index the linked PDFs in agenda_files!
 
         docs = []
-        agenda_doc = Document(text=agenda_data,
-                              doc_id=meeting_id,
-                              extra_info={
-                                    "committee": self.committee_id,
-                                    "title": agenda_title,
-                                    "date": agenda_date,
-                                    "url": agenda_url,
-                              })
+        agenda_doc = Document(
+            text=agenda_data,
+            doc_id=meeting_id,
+            extra_info={
+                "committee": self.committee_id,
+                "title": agenda_title,
+                "date": agenda_date,
+                "url": agenda_url,
+            },
+        )
         docs.append(agenda_doc)
         return docs
 
-
     def load_data(
-        self,
-        meeting_ids: Optional[List[str]] = None,
-        **load_kwargs: Any
+        self, meeting_ids: Optional[List[str]] = None, **load_kwargs: Any
     ) -> List[Document]:
         """Load all meetings of the committee.
 
         Args:
             meeting_ids (List[str]): A list of meeting IDs to load. If None, load all meetings.
         """
 
         # if a list of meetings wasn't provided, enumerate them all
         if not meeting_ids:
-            meeting_ids = [meeting.get('meetingID') for meeting in self.get_meeting_list()]
+            meeting_ids = [
+                meeting.get("meetingID") for meeting in self.get_meeting_list()
+            ]
 
         # process all relevant meetings & return the documents
         docs = []
         for meeting_id in meeting_ids:
             docs.extend(self.process_meeting(meeting_id))
         return docs
```

### Comparing `llama_hub-0.0.4/llama_hub/boarddocs/crawl.ipynb` & `llama_hub-0.0.5/llama_hub/boarddocs/crawl.ipynb`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/chatgpt_plugin/README.md` & `llama_hub-0.0.5/llama_hub/chatgpt_plugin/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/chatgpt_plugin/base.py` & `llama_hub-0.0.5/llama_hub/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/chroma/README.md` & `llama_hub-0.0.5/llama_hub/chroma/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/chroma/base.py` & `llama_hub-0.0.5/llama_hub/chroma/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 
     def __init__(
         self,
         collection_name: str,
         persist_directory: str,
     ) -> None:
         """Initialize with parameters."""
-        import_err_msg = (
-            "`chromadb` package not found, please run `pip install chromadb`"
-        )
         import chromadb  # noqa: F401
         from chromadb.config import Settings
 
         if (collection_name is None) or (persist_directory is None):
             raise ValueError("Please provide a collection name and persist directory.")
 
         self._client = chromadb.Client(
```

### Comparing `llama_hub-0.0.4/llama_hub/confluence/README.md` & `llama_hub-0.0.5/llama_hub/confluence/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,42 @@
 OAuth 2.0 credentials to authenticate with the Confluence instance. If no credentials are specified, the loader will
 look for `CONFLUENCE_API_TOKEN` or `CONFLUENCE_USERNAME`/`CONFLUENCE_PASSWORD` environment variables to proceed with basic authentication.
 
 For more on authenticating using OAuth 2.0, checkout:
 - https://atlassian-python-api.readthedocs.io/index.html
 - https://developer.atlassian.com/cloud/confluence/oauth-2-3lo-apps/
 
-User then specify a list of `page_ids` and/or `space_key` to load in the corresponding pages into Document objects, if 
-both are specified the union of both sets will be returned. User can also specify a boolean `include_attachments` to 
+Confluence pages are obtained through one of 4 four mutually exclusive ways:
+
+1. `page_ids`: Load all pages from a list of page ids
+2. `space_key`: Load all pages from a space
+3. `label`: Load all pages with a given label
+4. `cql`: Load all pages that match a given CQL query (Confluence Query Language https://developer.atlassian.com/cloud/confluence/advanced-searching-using-cql/ ).
+
+When `page_ids` is specified, `include_children` will cause the loader to also load all descendent pages.
+When `space_key` is specified, `page_status` further specifies the status of pages to load: None, 'current', 'archived', 'draft'.
+
+limit (int): Deprecated, use `max_num_results` instead.
+
+max_num_results (int): Maximum number of results to return.  If None, return all results.  Requests are made in batches to achieve the desired number of results.
+
+User can also specify a boolean `include_attachments` to 
 include attachments, this is set to `False` by default, if set to `True` all attachments will be downloaded and 
-ConfluenceReader will extract the text from the attachments and add it to the Document object. Currently supported attachment types are: PDF, PNG, JPEG/JPG, SVG, Word and Excel. 
+ConfluenceReader will extract the text from the attachments and add it to the Document object.
+Currently supported attachment types are: PDF, PNG, JPEG/JPG, SVG, Word and Excel. 
 
 Hint: `space_key` and `page_id` can both be found in the URL of a page in Confluence - https://yoursite.atlassian.com/wiki/spaces/<space_key>/pages/<page_id>
 
 ## Usage
 
 Here's an example usage of the ConfluenceReader.
 
 ```python
-from llama_index import download_loader
 
-ConfluenceReader = download_loader('ConfluenceReader')
+from llama_hub.confluence.base import ConfluenceReader
 
 token = {
     access_token: "<access_token>",
     token_type: "<token_type>"
 }
 oauth2_dict = {
     "client_id": "<client_id>",
@@ -36,11 +49,12 @@
 
 base_url = "https://yoursite.atlassian.com/wiki"
 
 page_ids = ["<page_id_1>", "<page_id_2>", "<page_id_3"]
 space_key = "<space_key>"
 
 reader = ConfluenceReader(base_url=base_url, oauth2=oauth2_dict)
-documents = reader.load_data(space_key=space_key, page_ids=page_ids, include_attachments=True)
+documents = reader.load_data(space_key=space_key, include_attachments=True, page_status="current")
+documents.extend(reader.load_data(page_ids=page_ids, include_children=True, include_attachments=True))
 ```
 
 This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/jerryjliu/gpt_index/tree/main/gpt_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent. See [here](https://github.com/emptycrown/llama-hub/tree/main) for examples.
```

### Comparing `llama_hub-0.0.4/llama_hub/couchdb/README.md` & `llama_hub-0.0.5/llama_hub/couchdb/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/couchdb/base.py` & `llama_hub-0.0.5/llama_hub/couchdb/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,74 +2,83 @@
 
 from typing import Dict, List, Optional
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 import logging
 import json
 
+
 class SimpleCouchDBReader(BaseReader):
     """Simple CouchDB reader.
 
     Concatenates each CouchDB doc into Document used by LlamaIndex.
 
     Args:
         couchdb_url (str): CouchDB Full URL.
         max_docs (int): Maximum number of documents to load.
 
     """
 
-    def __init__(self, user: str, pwd: str, host: str, port: int, couchdb_url: Optional[Dict] = None, max_docs: int = 1000) -> None:
+    def __init__(
+        self,
+        user: str,
+        pwd: str,
+        host: str,
+        port: int,
+        couchdb_url: Optional[Dict] = None,
+        max_docs: int = 1000,
+    ) -> None:
         """Initialize with parameters."""
         import couchdb3
 
         if couchdb_url is not None:
             self.client: CouchDBClient = couchdb3.Server(couchdb_url)
         else:
-            self.client: CouchDBClient = couchdb3.Server(f'http://{user}:{pwd}@{host}:{port}')
+            self.client: CouchDBClient = couchdb3.Server(
+                f"http://{user}:{pwd}@{host}:{port}"
+            )
         self.max_docs = max_docs
 
-    def load_data(
-        self, db_name: str, query: Optional[str] = None
-    ) -> List[Document]:
+    def load_data(self, db_name: str, query: Optional[str] = None) -> List[Document]:
         """Load data from the input directory.
 
         Args:
             db_name (str): name of the database.
             query (Optional[str]): query to filter documents.
                 Defaults to None
 
         Returns:
             List[Document]: A list of documents.
 
         """
         documents = []
         db = self.client.get(db_name)
         if query is None:
-            #if no query is specified, return all docs in database
-            logging.debug('showing all docs')
-            results = db.view('_all_docs',include_docs=True)
+            # if no query is specified, return all docs in database
+            logging.debug("showing all docs")
+            results = db.view("_all_docs", include_docs=True)
         else:
-            logging.debug('executing query')
+            logging.debug("executing query")
             results = db.find(query)
 
         if type(results) is not dict:
             logging.debug(results.rows)
         else:
             logging.debug(results)
 
-        #check if more than one result
+        # check if more than one result
         if type(results) is not dict and results.rows is not None:
             for row in results.rows:
-                #check that the id field exists
+                # check that the id field exists
                 if "id" not in row:
                     raise ValueError("`id` field not found in CouchDB document.")
-                documents.append(Document(json.dumps(row.doc)))
+                documents.append(Document(text=json.dumps(row.doc)))
         else:
-            #only one result
-            if results.get('docs') is not None:
-                for item in results.get('docs'):
-                    #check that the _id field exists
+            # only one result
+            if results.get("docs") is not None:
+                for item in results.get("docs"):
+                    # check that the _id field exists
                     if "_id" not in item:
                         raise ValueError("`_id` field not found in CouchDB document.")
-                    documents.append(Document(json.dumps(item)))
+                    documents.append(Document(text=json.dumps(item)))
 
         return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/dad_jokes/README.md` & `llama_hub-0.0.5/llama_hub/dad_jokes/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/dad_jokes/base.py` & `llama_hub-0.0.5/llama_hub/dad_jokes/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,8 +25,8 @@
     def load_data(self) -> List[Document]:
         """Return a random dad joke.
 
         Args:
             None.
 
         """
-        return [Document(self._get_random_dad_joke())]
+        return [Document(text=self._get_random_dad_joke())]
```

### Comparing `llama_hub-0.0.4/llama_hub/database/README.md` & `llama_hub-0.0.5/llama_hub/database/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/database/base.py` & `llama_hub-0.0.5/llama_hub/database/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,9 +89,9 @@
                 raise ValueError("A query parameter is necessary to filter the data")
             else:
                 result = connection.execute(text(query))
 
             for item in result.fetchall():
                 # fetch each item
                 doc_str = ", ".join([str(entry) for entry in item])
-                documents.append(Document(doc_str))
+                documents.append(Document(text=doc_str))
         return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/deeplake/README.md` & `llama_hub-0.0.5/llama_hub/deeplake/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/deeplake/base.py` & `llama_hub-0.0.5/llama_hub/deeplake/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/discord/README.md` & `llama_hub-0.0.5/llama_hub/discord/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/discord/base.py` & `llama_hub-0.0.5/llama_hub/discord/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
                     f"Channel id {channel_id} must be an integer, "
                     f"not {type(channel_id)}."
                 )
             channel_content = self._read_channel(
                 channel_id, limit=limit, oldest_first=oldest_first
             )
             results.append(
-                Document(channel_content, extra_info={"channel": channel_id})
+                Document(text=channel_content, extra_info={"channel": channel_id})
             )
         return results
 
 
 if __name__ == "__main__":
     reader = DiscordReader()
     print("initialized reader")
```

### Comparing `llama_hub-0.0.4/llama_hub/docugami/README.md` & `llama_hub-0.0.5/llama_hub/docugami/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 
 loader = DocugamiReader()
 documents = loader.load_data(docset_id=docset_id, document_ids=document_ids)
 ```
 
 This loader is designed to be used as a way to load data into [LlamaIndex](https://github.com/jerryjliu/gpt_index/tree/main/gpt_index) and/or subsequently used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent. See [here](https://github.com/emptycrown/llama-hub/tree/main) for examples.
 
-See more information about how to use Docugami with LangChain in the [LangChain docs](https://python.langchain.com/en/latest/ecosystem/docugami.html).
+See more information about how to use Docugami with LangChain in the [LangChain docs](https://python.langchain.com/docs/ecosystem/integrations/docugami).
 
 # Advantages vs Other Chunking Techniques
 
 Appropriate chunking of your documents is critical for retrieval from documents. Many chunking techniques exist, including simple ones that rely on whitespace and recursive chunk splitting based on character length. Docugami offers a different approach:
 
 1.	**Intelligent Chunking:** Docugami breaks down every document into a hierarchical semantic XML tree of chunks of varying sizes, from single words or numerical values to entire sections. These chunks follow the semantic contours of the document, providing a more meaningful representation than arbitrary length or simple whitespace-based chunking.
 2.	**Structured Representation:** In addition, the XML tree indicates the structural contours of every document, using attributes denoting headings, paragraphs, lists, tables, and other common elements, and does that consistently across all supported document formats, such as scanned PDFs or DOCX files. It appropriately handles long-form document characteristics like page headers/footers or multi-column flows for clean text extraction.
 3.	**Semantic Annotations:** Chunks are annotated with semantic tags that are coherent across the document set, facilitating consistent hierarchical queries across multiple documents, even if they are written and formatted differently. For example, in set of lease agreements, you can easily identify key provisions like the Landlord, Tenant, or Renewal Date, as well as more complex information such as the wording of any sub-lease provision or whether a specific jurisdiction has an exception section within a Termination Clause.
-4.	**Additional Metadata:** Chunks are also annotated with additional metadata, if a user has been using Docugami. This additional metadata can be used for high-accuracy Document QA without context window restrictions. See detailed code walk-through in [this notebook](./docugami.ipynb).
+4.	**Additional Metadata:** Chunks are also annotated with additional metadata, if a user has been using Docugami. This additional metadata can be used for high-accuracy Document QA without context window restrictions. See detailed code walk-through in [this notebook](https://github.com/docugami/llama-hub/blob/main/llama_hub/docugami/docugami.ipynb).
```

### Comparing `llama_hub-0.0.4/llama_hub/docugami/base.py` & `llama_hub-0.0.5/llama_hub/docugami/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,15 @@
 
         per_file_metadata = {}
         for artifact in all_artifacts:
             artifact_name = artifact.get("name")
             artifact_url = artifact.get("url")
             artifact_doc = artifact.get("document")
 
-            if artifact_name == f"{project_id}.xml" and artifact_url and artifact_doc:
+            if artifact_name == "report-values.xml" and artifact_url and artifact_doc:
                 doc_id = artifact_doc["id"]
                 metadata: Dict = {}
 
                 # the evaluated XML for each document is named after the project
                 response = requests.request(
                     "GET",
                     f"{artifact_url}/content",
@@ -243,19 +243,19 @@
                         raise ValueError(
                             "Could not import lxml python package. "
                             "Please install it with `pip install lxml`."
                         )
                     artifact_tree = etree.parse(io.BytesIO(response.content))
                     artifact_root = artifact_tree.getroot()
                     ns = artifact_root.nsmap
-                    entries = artifact_root.xpath("//wp:Entry", namespaces=ns)
+                    entries = artifact_root.xpath("//pr:Entry", namespaces=ns)
                     for entry in entries:
-                        heading = entry.xpath("./wp:Heading", namespaces=ns)[0].text
+                        heading = entry.xpath("./pr:Heading", namespaces=ns)[0].text
                         value = " ".join(
-                            entry.xpath("./wp:Value", namespaces=ns)[0].itertext()
+                            entry.xpath("./pr:Value", namespaces=ns)[0].itertext()
                         ).strip()
                         metadata[heading] = value
                     per_file_metadata[doc_id] = metadata
                 else:
                     raise Exception(
                         f"Failed to download {artifact_url}/content "
                         + "(status: {response.status_code})"
@@ -281,32 +281,35 @@
             return self._parse_dgml(document, response.content, doc_metadata)
         else:
             raise Exception(
                 f"Failed to download {url} (status: {response.status_code})"
             )
 
     def load_data(
-            self,
-            docset_id: str,
-            document_ids: Optional[List[str]] = None,
-            access_token: Optional[str] = None) -> List[Document]:
+        self,
+        docset_id: str,
+        document_ids: Optional[List[str]] = None,
+        access_token: Optional[str] = None,
+    ) -> List[Document]:
         """Load data the given docset_id in Docugami
 
         Args:
             docset_id (str): Document set ID to load data for.
             document_ids (Optional[List[str]]): Optional list of document ids to load data for.
                                     If not specified, all documents from docset_id are loaded.
         """
         chunks: List[Document] = []
 
         if access_token:
             self.access_token = access_token
 
         if not self.access_token:
-            raise Exception("Please specify access token as argument or set the DOCUGAMI_API_KEY env var.")
+            raise Exception(
+                "Please specify access token as argument or set the DOCUGAMI_API_KEY env var."
+            )
 
         _document_details = self._document_details_for_docset_id(docset_id)
         if document_ids:
             _document_details = [
                 d for d in _document_details if d["id"] in document_ids
             ]
 
@@ -316,19 +319,19 @@
             # if there are any projects for this docset, load project metadata
             for project in _project_details:
                 metadata = self._metadata_for_project(project)
                 combined_project_metadata.update(metadata)
 
         for doc in _document_details:
             doc_metadata = combined_project_metadata.get(doc["id"])
-            chunks += self._load_chunks_for_document(
-                docset_id, doc, doc_metadata
-            )
+            chunks += self._load_chunks_for_document(docset_id, doc, doc_metadata)
 
         return chunks
 
 
 if __name__ == "__main__":
     reader = DocugamiReader()
     print(
-        reader.load_data(docset_id="ecxqpipcoe2p", document_ids=["43rj0ds7s0ur", "bpc1vibyeke2"])
+        reader.load_data(
+            docset_id="ecxqpipcoe2p", document_ids=["43rj0ds7s0ur", "bpc1vibyeke2"]
+        )
     )
```

### Comparing `llama_hub-0.0.4/llama_hub/docugami/docugami.ipynb` & `llama_hub-0.0.5/llama_hub/docugami/docugami.ipynb`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/elasticsearch/README.md` & `llama_hub-0.0.5/llama_hub/elasticsearch/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/elasticsearch/base.py` & `llama_hub-0.0.5/llama_hub/elasticsearch/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,16 @@
         httpx_client_args (dict): Optional additional args to pass to the `httpx.Client`
     """
 
     def __init__(
         self, endpoint: str, index: str, httpx_client_args: Optional[dict] = None
     ):
         """Initialize with parameters."""
-        import_err_msg = """
-            `httpx` package not found. Install via `pip install httpx`
-        """
         import httpx  # noqa: F401
+
         self._client = httpx.Client(base_url=endpoint, **(httpx_client_args or {}))
         self._index = index
         self._endpoint = endpoint
 
     def load_data(
         self,
         field: str,
```

### Comparing `llama_hub-0.0.4/llama_hub/faiss/README.md` & `llama_hub-0.0.5/llama_hub/faiss/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/faiss/base.py` & `llama_hub-0.0.5/llama_hub/faiss/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/feedly_rss/README.md` & `llama_hub-0.0.5/llama_hub/feedly_rss/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/feedly_rss/base.py` & `llama_hub-0.0.5/llama_hub/feedly_rss/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,60 +2,64 @@
 
 from pathlib import Path
 import json
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
+
 class FeedlyRssReader(BaseReader):
     """Feedly Rss Reader.
 
     Get entries from Feedly Rss Reader
 
     Uses Feedly Official python-api-client: https://github.com/feedly/python-api-client
     """
 
     def __init__(self, bearer_token: str) -> None:
         """Initialize with parameters."""
         super().__init__()
         self.bearer_token = bearer_token
 
-    def setup_auth(self, directory: Path = Path.home() / ".config/feedly", overwrite: bool = False):
+    def setup_auth(
+        self, directory: Path = Path.home() / ".config/feedly", overwrite: bool = False
+    ):
         """Modified from python-api-client/feedly/api_client/utils.py
         Instead promopting for user input, we take the token as an argument
         """
         directory.mkdir(exist_ok=True, parents=True)
 
         auth_file = directory / "access.token"
 
         if not auth_file.exists() or overwrite:
             auth = self.bearer_token
-            auth_file.write_text(auth.strip()) 
+            auth_file.write_text(auth.strip())
 
-    def load_data(self, category_name, max_count = 100):
-        """Get the entries from a feedly category
-        """
+    def load_data(self, category_name, max_count=100):
+        """Get the entries from a feedly category"""
 
         from feedly.api_client.session import FeedlySession
         from feedly.api_client.stream import StreamOptions
 
         self.setup_auth(overwrite=True)
         sess = FeedlySession()
         category = sess.user.user_categories.get(category_name)
 
         documents = []
-        for article in category.stream_contents(options = StreamOptions(max_count = max_count)):
+        for article in category.stream_contents(
+            options=StreamOptions(max_count=max_count)
+        ):
             # doc for available fields: https://developer.feedly.com/v3/streams/
             entry = {
-                'title': article["title"],
-                'published': article["published"],
-                'summary': article["summary"],
-                'author': article["author"],
-                'content': article["content"],
-                'keywords': article["keywords"],
-                'commonTopics': article["commonTopics"]
+                "title": article["title"],
+                "published": article["published"],
+                "summary": article["summary"],
+                "author": article["author"],
+                "content": article["content"],
+                "keywords": article["keywords"],
+                "commonTopics": article["commonTopics"],
             }
 
             text = json.dumps(entry, ensure_ascii=False)
 
-            documents.append(Document(text))
-        return documents
+            documents.append(Document(text=text))
+        return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/file/README.md` & `llama_hub-0.0.5/llama_hub/file/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/audio/README.md` & `llama_hub-0.0.5/llama_hub/file/audio/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/audio/base.py` & `llama_hub-0.0.5/llama_hub/file/audio/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,8 +48,8 @@
             audio.export(file_str, format="mp3")
 
         model = cast(whisper.Whisper, self.parser_config["model"])
         result = model.transcribe(str(file))
 
         transcript = result["text"]
 
-        return [Document(transcript, extra_info=extra_info)]
+        return [Document(text=transcript, extra_info=extra_info)]
```

### Comparing `llama_hub-0.0.4/llama_hub/file/audio_gladia/README.md` & `llama_hub-0.0.5/llama_hub/file/audio_gladia/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/audio_gladia/base.py` & `llama_hub-0.0.5/llama_hub/file/audio_gladia/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Audio Transcriber.
 
 A transcriber for the audio of mp3, mp4 files using Gladia's OpenAI Whisper.
 
 """
 from pathlib import Path
-from typing import Any, Dict, List, Optional, cast
+from typing import Any, Dict, List, Optional
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 
 class GladiaAudioTranscriber(BaseReader):
     """Audio parser.
@@ -90,8 +90,8 @@
             "https://api.gladia.io/audio/text/audio-transcription/",
             headers=headers,
             files=files,
         )
         response_dict = response.json()
         transcript = response_dict["prediction"]
 
-        return [Document(transcript, extra_info=extra_info)]
+        return [Document(text=transcript, extra_info=extra_info)]
```

### Comparing `llama_hub-0.0.4/llama_hub/file/base.py` & `llama_hub-0.0.5/llama_hub/file/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,24 +131,25 @@
 
             if input_file.suffix in self.file_extractor:
                 reader = self.file_extractor[input_file.suffix]
 
                 if isinstance(reader, str):
                     try:
                         from llama_hub.utils import import_loader
+
                         reader = import_loader(reader)()
-                    except ImportError as e:
+                    except ImportError:
                         reader = download_loader(reader)()
 
                 extracted_documents = reader.load_data(
                     file=input_file, extra_info=metadata
                 )
                 documents.extend(extracted_documents)
             else:
                 data = ""
                 # do standard read
                 with open(input_file, "r", errors=self.errors) as f:
                     data = f.read()
-                document = Document(data, extra_info=metadata)
+                document = Document(text=data, extra_info=metadata)
                 documents.append(document)
 
         return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/file/cjk_pdf/README.md` & `llama_hub-0.0.5/llama_hub/file/cjk_pdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/cjk_pdf/base.py` & `llama_hub-0.0.5/llama_hub/file/cjk_pdf/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,10 +68,10 @@
         self, file: Path, extra_info: Optional[Dict] = None
     ) -> List[Document]:
         """Parse file."""
 
         text_list = self._extract_text_by_page(file)
 
         if self._concat_pages:
-            return [Document("\n".join(text_list), extra_info=extra_info)]
+            return [Document(text="\n".join(text_list), extra_info=extra_info)]
         else:
-            return [Document(text, extra_info=extra_info) for text in text_list]
+            return [Document(text=text, extra_info=extra_info) for text in text_list]
```

### Comparing `llama_hub-0.0.4/llama_hub/file/deepdoctection/README.md` & `llama_hub-0.0.5/llama_hub/file/deepdoctection/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/deepdoctection/base.py` & `llama_hub-0.0.5/llama_hub/file/deepdoctection/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     Uses deepdoctection as a library to parse PDF files.
 
     """
 
     def __init__(self, attrs_as_metadata: Optional[Set] = None) -> None:
         """Init params."""
         import deepdoctection as dd
+
         self.analyzer = dd.get_dd_analyzer()
         self.attrs_as_metadata = attrs_as_metadata or set()
 
     def load_data(
         self, file: Path, extra_info: Optional[Dict] = None
     ) -> List[Document]:
         """Parse file."""
@@ -29,11 +30,9 @@
         doc = iter(df)
         result_docs = []
         for page in doc:
             doc_text = page.text
             extra_info = {
                 k: getattr(page, k) for k in self.attrs_as_metadata if hasattr(page, k)
             }
-            result_docs.append(
-                Document(doc_text, extra_info=extra_info)
-            )
+            result_docs.append(Document(text=doc_text, extra_info=extra_info))
         return result_docs
```

### Comparing `llama_hub-0.0.4/llama_hub/file/docx/README.md` & `llama_hub-0.0.5/llama_hub/file/docx/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/docx/base.py` & `llama_hub-0.0.5/llama_hub/file/docx/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
         text = docx2txt.process(file)
         metadata = {"file_name": file.name}
 
         if extra_info is not None:
             metadata.update(extra_info)
 
-        return [Document(text, extra_info=metadata)]
+        return [Document(text=text, extra_info=metadata)]
```

### Comparing `llama_hub-0.0.4/llama_hub/file/epub/README.md` & `llama_hub-0.0.5/llama_hub/file/epub/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/epub/base.py` & `llama_hub-0.0.5/llama_hub/file/epub/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,8 +29,8 @@
             # Chapters are typically located in epub documents items.
             if item.get_type() == ebooklib.ITEM_DOCUMENT:
                 text_list.append(
                     html2text.html2text(item.get_content().decode("utf-8"))
                 )
 
         text = "\n".join(text_list)
-        return [Document(text, extra_info=extra_info)]
+        return [Document(text=text, extra_info=extra_info)]
```

### Comparing `llama_hub-0.0.4/llama_hub/file/flat_pdf/README.md` & `llama_hub-0.0.5/llama_hub/file/flat_pdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/flat_pdf/base.py` & `llama_hub-0.0.5/llama_hub/file/flat_pdf/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,50 +26,61 @@
 
 
         :param self: Represent the instance of the class
         :param file: Path: The file that we want to load
         :return: A document object
         """
         import shutil
+
         try:
 
             if not file.is_file() and file.suffix != ".pdf":
                 raise Exception("Invalid file")
 
             pdf_dir: Path = file
-            work_dir: str = str(pathlib.Path().resolve()) + "/flat_pdf/{file_name}".format(
-                file_name=file.name.replace(file.suffix, ""))
+            work_dir: str = str(
+                pathlib.Path().resolve()
+            ) + "/flat_pdf/{file_name}".format(
+                file_name=file.name.replace(file.suffix, "")
+            )
             pdf_content: str = ""
 
-            shutil.rmtree(str(pathlib.Path().resolve()) + f"/flat_pdf", ignore_errors=True)
+            shutil.rmtree(
+                str(pathlib.Path().resolve()) + "/flat_pdf", ignore_errors=True
+            )
             os.makedirs(work_dir)
 
-            pdf_pages_count: int = self.convert_pdf_in_images(pdf_dir=pdf_dir, work_dir=work_dir)
+            pdf_pages_count: int = self.convert_pdf_in_images(
+                pdf_dir=pdf_dir, work_dir=work_dir
+            )
 
             for page_number in range(0, pdf_pages_count):
-                document = self.image_loader.load_data(file=Path(work_dir + f"/page-{page_number}.png"))
+                document = self.image_loader.load_data(
+                    file=Path(work_dir + f"/page-{page_number}.png")
+                )
                 pdf_content += document[0].text
             return Document(text=pdf_content)
 
         except Exception as e:
-            warnings.warn(
-                f"{str(e)}"
-            )
+            warnings.warn(f"{str(e)}")
         finally:
-            shutil.rmtree(str(pathlib.Path().resolve()) + f"/flat_pdf", ignore_errors=True)
+            shutil.rmtree(
+                str(pathlib.Path().resolve()) + "/flat_pdf", ignore_errors=True
+            )
 
     def convert_pdf_in_images(self, pdf_dir: Path, work_dir: str) -> int:
         """
         The convert_pdf_in_images function converts a PDF file into images.
 
         :param pdf_dir: Path: Specify the path of the pdf file to be converted
         :param work_dir: str: Specify the directory where the images will be saved
         :return: The number of pages in the pdf file
         """
         import fitz
+
         zoom_x = 2.0  # horizontal zoom
         zoom_y = 2.0  # vertical zoom
         mat = fitz.Matrix(zoom_x, zoom_y)
         pages = fitz.open(pdf_dir)
         for page in pages:  # iterate through the pages
             image = page.get_pixmap(matrix=mat)  # render page to an image
             image.save(f"{work_dir}/page-{page.number}.png")
```

### Comparing `llama_hub-0.0.4/llama_hub/file/image/README.md` & `llama_hub-0.0.5/llama_hub/file/image/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/image/base.py` & `llama_hub-0.0.5/llama_hub/file/image/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/image_blip/base.py` & `llama_hub-0.0.5/llama_hub/file/image_blip/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,22 +48,33 @@
                 raise ImportError(
                     "PIL is required to read image files: " "`pip install Pillow`"
                 )
 
             device = "cuda" if torch.cuda.is_available() else "cpu"
             dtype = torch.float16 if torch.cuda.is_available() else torch.float32
 
-            processor = BlipProcessor.from_pretrained("Salesforce/blip-image-captioning-large")
-            model = BlipForConditionalGeneration.from_pretrained("Salesforce/blip-image-captioning-large", torch_dtype=dtype)
-
-            parser_config = {"processor": processor, "model": model, "device": device, "dtype": dtype}
+            processor = BlipProcessor.from_pretrained(
+                "Salesforce/blip-image-captioning-large"
+            )
+            model = BlipForConditionalGeneration.from_pretrained(
+                "Salesforce/blip-image-captioning-large", torch_dtype=dtype
+            )
+
+            parser_config = {
+                "processor": processor,
+                "model": model,
+                "device": device,
+                "dtype": dtype,
+            }
 
         self._parser_config = parser_config
 
-    def load_data(self, file: Path, extra_info: Optional[Dict] = None) -> List[Document]:
+    def load_data(
+        self, file: Path, extra_info: Optional[Dict] = None
+    ) -> List[Document]:
         """Parse file."""
         from PIL import Image
 
         from llama_index.img_utils import img_2_b64
 
         # load document image
         image = Image.open(file)
@@ -80,15 +91,15 @@
         processor = self._parser_config["processor"]
 
         device = self._parser_config["device"]
         dtype = self._parser_config["dtype"]
         model.to(device)
 
         # unconditional image captioning
-        
+
         inputs = processor(image, self._prompt, return_tensors="pt").to(device, dtype)
 
         out = model.generate(**inputs)
         text_str = processor.decode(out[0], skip_special_tokens=True)
 
         return ImageDocument(
             text=text_str,
```

### Comparing `llama_hub-0.0.4/llama_hub/file/image_blip2/base.py` & `llama_hub-0.0.5/llama_hub/file/image_blip2/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,20 +48,27 @@
                 )
             device = "cuda" if torch.cuda.is_available() else "cpu"
             dtype = torch.float16 if torch.cuda.is_available() else torch.float32
             processor = Blip2Processor.from_pretrained("Salesforce/blip2-opt-2.7b")
             model = Blip2ForConditionalGeneration.from_pretrained(
                 "Salesforce/blip2-opt-2.7b", torch_dtype=dtype
             )
-            parser_config = {"processor": processor, "model": model, "device": device, "dtype": dtype}
+            parser_config = {
+                "processor": processor,
+                "model": model,
+                "device": device,
+                "dtype": dtype,
+            }
         self._parser_config = parser_config
         self._keep_image = keep_image
         self._prompt = prompt
 
-    def load_data(self, file: Path, extra_info: Optional[Dict] = None) -> List[Document]:
+    def load_data(
+        self, file: Path, extra_info: Optional[Dict] = None
+    ) -> List[Document]:
         """Parse file."""
         from PIL import Image
 
         from llama_index.img_utils import img_2_b64
 
         # load document image
         image = Image.open(file)
@@ -78,15 +85,15 @@
         processor = self._parser_config["processor"]
 
         device = self._parser_config["device"]
         dtype = self._parser_config["dtype"]
         model.to(device)
 
         # unconditional image captioning
-        
+
         inputs = processor(image, self._prompt, return_tensors="pt").to(device, dtype)
 
         out = model.generate(**inputs)
         text_str = processor.decode(out[0], skip_special_tokens=True)
 
         return ImageDocument(
             text=text_str,
```

### Comparing `llama_hub-0.0.4/llama_hub/file/image_deplot/base.py` & `llama_hub-0.0.5/llama_hub/file/image_deplot/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,36 +12,40 @@
 
     """
 
     def __init__(
         self,
         parser_config: Optional[Dict] = None,
         keep_image: bool = False,
-        max_output_tokens = 512,
+        max_output_tokens=512,
         prompt: str = "Generate underlying data table of the figure below:",
     ):
         """Init params."""
 
         if parser_config is None:
             try:
                 import torch  # noqa: F401
                 from PIL import Image  # noqa: F401
-                from transformers import (Pix2StructForConditionalGeneration,
-                                          Pix2StructProcessor)
+                from transformers import (
+                    Pix2StructForConditionalGeneration,
+                    Pix2StructProcessor,
+                )
             except ImportError:
                 raise ImportError(
                     "Please install extra dependencies that are required for "
                     "the ImageCaptionReader: "
                     "`pip install torch transformers Pillow`"
                 )
 
             device = "cuda" if torch.cuda.is_available() else "cpu"
             dtype = torch.float16 if torch.cuda.is_available() else torch.float32
-            processor = Pix2StructProcessor.from_pretrained('google/deplot')
-            model = Pix2StructForConditionalGeneration.from_pretrained('google/deplot', torch_dtype=dtype)
+            processor = Pix2StructProcessor.from_pretrained("google/deplot")
+            model = Pix2StructForConditionalGeneration.from_pretrained(
+                "google/deplot", torch_dtype=dtype
+            )
             parser_config = {
                 "processor": processor,
                 "model": model,
                 "device": device,
                 "dtype": dtype,
             }
 
@@ -77,15 +81,17 @@
         model.to(device)
 
         # unconditional image captioning
 
         inputs = processor(image, self._prompt, return_tensors="pt").to(device, dtype)
 
         out = model.generate(**inputs, max_new_tokens=self._max_output_tokens)
-        text_str = "Figure or chart with tabular data: " + processor.decode(out[0], skip_special_tokens=True)
+        text_str = "Figure or chart with tabular data: " + processor.decode(
+            out[0], skip_special_tokens=True
+        )
 
         return [
             ImageDocument(
                 text=text_str,
                 image=image_str,
                 extra_info=extra_info,
             )
```

### Comparing `llama_hub-0.0.4/llama_hub/file/ipynb/base.py` & `llama_hub-0.0.5/llama_hub/file/ipynb/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-
 import re
 from pathlib import Path
 from typing import Dict, Optional, List
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 
 class IPYNBReader(BaseReader):
     """Ipynb file loader.
 
-    Reads jupyter notebook files. 
+    Reads jupyter notebook files.
 
     """
 
     def __init__(
         self,
         parser_config: Optional[Dict] = None,
         concatenate: bool = False,
     ):
         """Init params."""
         self._parser_config = parser_config
         self._concatenate = concatenate
 
-    def load_data(self, file: Path, extra_info: Optional[Dict] = None) -> List[Document]:
+    def load_data(
+        self, file: Path, extra_info: Optional[Dict] = None
+    ) -> List[Document]:
         """Parse file."""
-        
+
         if file.name.endswith(".ipynb"):
             try:
                 import nbconvert  # noqa: F401
             except ImportError:
                 raise ImportError("Please install nbconvert 'pip install nbconvert' ")
         string = nbconvert.exporters.ScriptExporter().from_file(file)[0]
         # split each In[] cell into a separate string
-        splits = re.split(r'In\[\d+\]:', string)
+        splits = re.split(r"In\[\d+\]:", string)
         # remove the first element, which is empty
         splits.pop(0)
-        
+
         if self._concatenate:
             docs = [Document(text="\n\n".join(splits))]
         else:
             docs = [Document(text=s) for s in splits]
         return docs
```

### Comparing `llama_hub-0.0.4/llama_hub/file/json/README.md` & `llama_hub-0.0.5/llama_hub/file/json/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/json/base.py` & `llama_hub-0.0.5/llama_hub/file/json/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,17 +47,15 @@
 
     def __init__(self, levels_back: Optional[int] = None) -> None:
         """Initialize with arguments."""
         super().__init__()
         self.levels_back = levels_back
 
     def load_data(
-        self, 
-        file: Path, 
-        extra_info: Optional[Dict] = None
+        self, file: Path, extra_info: Optional[Dict] = None
     ) -> List[Document]:
         """Load data from the input file."""
         # TODO: change Path typing for file in all load_data calls
         if not isinstance(file, Path):
             file = Path(file)
         with open(file, "r") as f:
             data = json.load(f)
@@ -65,13 +63,13 @@
                 # If levels_back isn't set, we just format and make each
                 # line an embedding
                 json_output = json.dumps(data, indent=0)
                 lines = json_output.split("\n")
                 useful_lines = [
                     line for line in lines if not re.match(r"^[{}\[\],]*$", line)
                 ]
-                return [Document("\n".join(useful_lines), extra_info=extra_info)]
+                return [Document(text="\n".join(useful_lines), extra_info=extra_info)]
             elif self.levels_back is not None:
                 # If levels_back is set, we make the embeddings contain the labels
                 # from further up the JSON tree
                 lines = [*_depth_first_yield(data, self.levels_back, [])]
-                return [Document("\n".join(lines), extra_info=extra_info)]
+                return [Document(text="\n".join(lines), extra_info=extra_info)]
```

### Comparing `llama_hub-0.0.4/llama_hub/file/markdown/README.md` & `llama_hub-0.0.5/llama_hub/file/markdown/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/markdown/base.py` & `llama_hub-0.0.5/llama_hub/file/markdown/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,8 +103,8 @@
         extra_info: Optional[Dict] = None,
         content: Optional[str] = None,
     ) -> List[Document]:
         """Parse file into string.
         If content is provided, use that instead of reading from file."""
         tups = self.parse_tups(file, content=content)
         # TODO: don't include headers right now
-        return [Document(value, extra_info=extra_info) for _, value in tups]
+        return [Document(text=value, extra_info=extra_info) for _, value in tups]
```

### Comparing `llama_hub-0.0.4/llama_hub/file/mbox/README.md` & `llama_hub-0.0.5/llama_hub/file/mbox/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/mbox/base.py` & `llama_hub-0.0.5/llama_hub/file/mbox/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,17 @@
                         content = part.get_payload(decode=True)  # decode
                         break
             # Get plain message payload for non-multipart messages
             else:
                 content = msg.get_payload(decode=True)
 
             if not content:
-                print("WARNING llama_hub.file.mbox found messages with content that stayed None. Skipping entry...")
+                print(
+                    "WARNING llama_hub.file.mbox found messages with content that stayed None. Skipping entry..."
+                )
                 continue
 
             # Parse message HTML content and remove unneeded whitespace
             soup = BeautifulSoup(content)
             stripped_content = " ".join(soup.get_text().split())
             # Format message to include date, sender, receiver and subject
             msg_string = self.message_format.format(
@@ -103,9 +105,9 @@
         load_kwargs:
             max_count (int): Maximum amount of messages to read.
             message_format (str): Message format overriding default.
         """
         docs: List[Document] = []
         content = self.parse_file(file)
         for msg in content:
-            docs.append(Document(msg, extra_info=extra_info))
+            docs.append(Document(text=msg, extra_info=extra_info))
         return docs
```

### Comparing `llama_hub-0.0.4/llama_hub/file/paged_csv/README.md` & `llama_hub-0.0.5/llama_hub/file/paged_csv/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/paged_csv/base.py` & `llama_hub-0.0.5/llama_hub/file/paged_csv/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Paged CSV reader.
 
 A parser for tabular data files.
 
 """
 from pathlib import Path
-from typing import Any, Dict, List, Optional
+from typing import Dict, List, Optional
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 
 class PagedCSVReader(BaseReader):
     """Paged CSV parser.
@@ -24,12 +24,14 @@
 
         docs = []
         with open(file, "r") as fp:
             csv_reader = csv.DictReader(fp)  # type: ignore
             for row in csv_reader:
                 docs.append(
                     Document(
-                        "\n".join(f"{k.strip()}: {v.strip()}" for k, v in row.items()),
+                        text="\n".join(
+                            f"{k.strip()}: {v.strip()}" for k, v in row.items()
+                        ),
                         extra_info=extra_info,
                     )
                 )
         return docs
```

### Comparing `llama_hub-0.0.4/llama_hub/file/pandas_csv/README.md` & `llama_hub-0.0.5/llama_hub/file/pandas_csv/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/pandas_csv/base.py` & `llama_hub-0.0.5/llama_hub/file/pandas_csv/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,10 +61,12 @@
         df = pd.read_csv(file, **self._pandas_config)
 
         text_list = df.apply(
             lambda row: (self._col_joiner).join(row.astype(str).tolist()), axis=1
         ).tolist()
 
         if self._concat_rows:
-            return [Document((self._row_joiner).join(text_list), extra_info=extra_info)]
+            return [
+                Document(text=self._row_joiner.join(text_list), extra_info=extra_info)
+            ]
         else:
-            return [Document(text, extra_info=extra_info) for text in text_list]
+            return [Document(text=text, extra_info=extra_info) for text in text_list]
```

### Comparing `llama_hub-0.0.4/llama_hub/file/pandas_excel/README.md` & `llama_hub-0.0.5/llama_hub/file/pandas_excel/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/pandas_excel/base.py` & `llama_hub-0.0.5/llama_hub/file/pandas_excel/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,45 +25,54 @@
     """
 
     def __init__(
         self,
         *args: Any,
         pandas_config: dict = {},
         concat_rows: bool = True,
+        row_joiner: str = "\n",
         **kwargs: Any
     ) -> None:
         """Init params."""
         super().__init__(*args, **kwargs)
         self._pandas_config = pandas_config
         self._concat_rows = concat_rows
+        self._row_joiner = row_joiner
 
     def load_data(
-        self, file: Path, sheet_name: Optional[Union[str, int]] = None, extra_info: Optional[Dict] = None
+        self,
+        file: Path,
+        sheet_name: Optional[Union[str, int]] = None,
+        extra_info: Optional[Dict] = None,
     ) -> List[Document]:
         """Parse file and extract values from a specific column.
 
         Args:
             file (Path): The path to the Excel file to read.
             column_name (str): The name of the column to use when creating the Document objects.
         Returns:
             List[Document]: A list of`Document objects containing the values from the specified column in the Excel file.
         """
         import itertools
 
         import pandas as pd
-        
+
         df = pd.read_excel(file, sheet_name=sheet_name, **self._pandas_config)
 
         keys = df.keys()
 
         df_sheets = []
 
         for key in keys:
             sheet = df[key].values.astype(str).tolist()
             df_sheets.append(sheet)
 
-        text_list = list(itertools.chain.from_iterable(df_sheets))  # flatten list of lists
+        text_list = list(
+            itertools.chain.from_iterable(df_sheets)
+        )  # flatten list of lists
 
         if self._concat_rows:
-            return [Document((self._row_joiner).join(text_list), extra_info=extra_info)]
+            return [
+                Document(text=self._row_joiner.join(text_list), extra_info=extra_info)
+            ]
         else:
-            return [Document(text, extra_info=extra_info) for text in text_list]
+            return [Document(text=text, extra_info=extra_info) for text in text_list]
```

### Comparing `llama_hub-0.0.4/llama_hub/file/pdf/README.md` & `llama_hub-0.0.5/llama_hub/file/pdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/pdf/base.py` & `llama_hub-0.0.5/llama_hub/file/pdf/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,14 +25,14 @@
 
             # Iterate over every page
             docs = []
             for page in range(num_pages):
                 # Extract the text from the page
                 page_text = pdf.pages[page].extract_text()
                 page_label = pdf.page_labels[page]
-                metadata = {"page_label": page_label, "file_name":file.name}
-                
+                metadata = {"page_label": page_label, "file_name": file.name}
+
                 if extra_info is not None:
                     metadata.update(extra_info)
-                    
-                docs.append(Document(page_text, extra_info=metadata))
+
+                docs.append(Document(text=page_text, extra_info=metadata))
             return docs
```

### Comparing `llama_hub-0.0.4/llama_hub/file/pdf_miner/README.md` & `llama_hub-0.0.5/llama_hub/file/pdf_miner/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/pdf_miner/base.py` & `llama_hub-0.0.5/llama_hub/file/pdf_miner/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from pathlib import Path
 from typing import Dict, List, Optional
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
+
 class PDFMinerReader(BaseReader):
     """PDF parser based on pdfminer.six."""
 
     def load_data(
         self, file: Path, extra_info: Optional[Dict] = None
     ) -> List[Document]:
         """Parse file."""
@@ -19,36 +20,38 @@
             from pdfminer.converter import TextConverter
             from pdfminer.layout import LAParams
             from io import StringIO
 
             def _extract_text_from_page(page):
                 resource_manager = PDFResourceManager()
                 output_string = StringIO()
-                codec = 'utf-8'
+                codec = "utf-8"
                 laparams = LAParams()
-                device = TextConverter(resource_manager, output_string, codec=codec, laparams=laparams)
+                device = TextConverter(
+                    resource_manager, output_string, codec=codec, laparams=laparams
+                )
                 interpreter = PDFPageInterpreter(resource_manager, device)
                 interpreter.process_page(page)
                 text = output_string.getvalue()
                 device.close()
                 output_string.close()
                 return text
-            
+
         except ImportError:
             raise ImportError(
                 "pdfminer.six is required to read PDF files: `pip install pypdf`"
             )
-        with open(file, 'rb') as fp:
+        with open(file, "rb") as fp:
             reader = PDF_Page.get_pages(fp)
 
             # Iterate over every page
             docs = []
             for i, page in enumerate(reader):
                 # Extract the text from the page
                 page_text = _extract_text_from_page(page)
 
                 metadata = {"page_label": i, "file_name": file.name}
                 if extra_info is not None:
                     metadata.update(extra_info)
 
-                docs.append(Document(page_text, extra_info=metadata))
+                docs.append(Document(text=page_text, extra_info=metadata))
             return docs
```

### Comparing `llama_hub-0.0.4/llama_hub/file/pptx/README.md` & `llama_hub-0.0.5/llama_hub/file/pptx/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/pptx/base.py` & `llama_hub-0.0.5/llama_hub/file/pptx/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,19 @@
 
     """
 
     def __init__(self, caption_images: Optional[bool] = False) -> None:
         """Init reader."""
         self.caption_images = caption_images
         if caption_images:
-            from transformers import (AutoTokenizer, VisionEncoderDecoderModel,
-                                      ViTFeatureExtractor)
+            from transformers import (
+                AutoTokenizer,
+                VisionEncoderDecoderModel,
+                ViTFeatureExtractor,
+            )
 
             model = VisionEncoderDecoderModel.from_pretrained(
                 "nlpconnect/vit-gpt2-image-captioning"
             )
             feature_extractor = ViTFeatureExtractor.from_pretrained(
                 "nlpconnect/vit-gpt2-image-captioning"
             )
@@ -96,8 +99,8 @@
                         f"\n Image: {self.generate_image_caption(image_filename)}\n\n"
                     )
 
                     os.remove(image_filename)
                 if hasattr(shape, "text"):
                     result += f"{shape.text}\n"
 
-        return [Document(result, extra_info=extra_info)]
+        return [Document(text=result, extra_info=extra_info)]
```

### Comparing `llama_hub-0.0.4/llama_hub/file/pymu_pdf/README.md` & `llama_hub-0.0.5/llama_hub/file/pymu_pdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/pymu_pdf/base.py` & `llama_hub-0.0.5/llama_hub/file/pymu_pdf/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/rdf/README.md` & `llama_hub-0.0.5/llama_hub/file/rdf/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/rdf/base.py` & `llama_hub-0.0.5/llama_hub/file/rdf/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         """Initialize loader."""
         super().__init__(*args, **kwargs)
 
-        from rdflib import Graph, URIRef
+        from rdflib import Graph
         from rdflib.namespace import RDF, RDFS
 
         self.Graph = Graph
         self.RDF = RDF
         self.RDFS = RDFS
 
     def fetch_labels(self, uri: Any, graph: Any, lang: str):
@@ -72,8 +72,8 @@
                 f"<{self.fetch_label_in_graphs(p, lang=lang)}> "
                 f"<{self.fetch_label_in_graphs(o, lang=lang)}>"
             )
             text_list.append(triple)
 
         text = "\n".join(text_list)
 
-        return [Document(text, extra_info=extra_info)]
+        return [Document(text=text, extra_info=extra_info)]
```

### Comparing `llama_hub-0.0.4/llama_hub/file/simple_csv/README.md` & `llama_hub-0.0.5/llama_hub/file/simple_csv/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/simple_csv/base.py` & `llama_hub-0.0.5/llama_hub/file/simple_csv/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def load_data(
         self, file: Path, extra_info: Optional[Dict] = None
     ) -> List[Document]:
         """Parse file."""
         import csv
 
         text_list = []
-        with open(file, "r", encoding='utf-8') as fp:
+        with open(file, "r", encoding="utf-8") as fp:
             csv_reader = csv.reader(fp)
             for row in csv_reader:
                 text_list.append(", ".join(row))
         if self._concat_rows:
-            return [Document("\n".join(text_list), extra_info=extra_info)]
+            return [Document(text="\n".join(text_list), extra_info=extra_info)]
         else:
-            return [Document(text, extra_info=extra_info) for text in text_list]
+            return [Document(text=text, extra_info=extra_info) for text in text_list]
```

### Comparing `llama_hub-0.0.4/llama_hub/file/unstructured/README.md` & `llama_hub-0.0.5/llama_hub/file/unstructured/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/file/unstructured/base.py` & `llama_hub-0.0.5/llama_hub/file/unstructured/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,10 +33,12 @@
         """Parse file."""
         from unstructured.partition.auto import partition
 
         elements = partition(str(file))
         text_chunks = [" ".join(str(el).split()) for el in elements]
 
         if split_documents:
-            return [Document(chunk, extra_info=extra_info) for chunk in text_chunks]
+            return [
+                Document(text=chunk, extra_info=extra_info) for chunk in text_chunks
+            ]
         else:
-            return [Document("\n\n".join(text_chunks), extra_info=extra_info)]
+            return [Document(text="\n\n".join(text_chunks), extra_info=extra_info)]
```

### Comparing `llama_hub-0.0.4/llama_hub/firestore/README.md` & `llama_hub-0.0.5/llama_hub/firestore/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/firestore/base.py` & `llama_hub-0.0.5/llama_hub/firestore/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         self,
         project_id: str,
         *args: Optional[Any],
         **kwargs: Optional[Any],
     ) -> None:
         """Initialize with parameters."""
         from google.cloud import firestore
+
         self.db = firestore.Client(project=project_id)
 
     def load_data(self, collection: str) -> List[Document]:
         """Load data from a Firestore collection, returning a list of Documents.
 
         Args:
             collection (str): The name of the Firestore collection to read from.
@@ -36,15 +37,15 @@
         Returns:
             List[Document]: A list of Document objects.
         """
         documents = []
         col_ref = self.db.collection(collection)
         for doc in col_ref.stream():
             doc_str = ", ".join([f"{k}: {v}" for k, v in doc.to_dict().items()])
-            documents.append(Document(doc_str))
+            documents.append(Document(text=doc_str))
         return documents
 
     def load_document(self, document_url: str) -> Document:
         """Load a single document from Firestore.
 
         Args:
             document_url (str): The absolute path to the Firestore document to read.
@@ -63,8 +64,8 @@
             else:
                 ref = ref.document(parts[i])
 
         doc = ref.get()
         if not doc.exists:
             raise ValueError(f"No such document: {document_url}")
         doc_str = ", ".join([f"{k}: {v}" for k, v in doc.to_dict().items()])
-        return Document(doc_str)
+        return Document(text=doc_str)
```

### Comparing `llama_hub-0.0.4/llama_hub/github_repo/README.md` & `llama_hub-0.0.5/llama_hub/github_repo/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/github_repo/base.py` & `llama_hub-0.0.5/llama_hub/github_repo/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/github_repo/github_client.py` & `llama_hub-0.0.5/llama_hub/github_repo/github_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 
         tree: Tree
 
     commit: Commit
     url: str
     sha: str
 
+
 @dataclass
 class GitBranchResponseModel(DataClassJsonMixin):
     """
     Dataclass for the response from the Github API's getBranch endpoint.
 
     Attributes:
         - commit (Commit): Commit object for the branch.
@@ -141,15 +142,15 @@
     @dataclass
     class Links(DataClassJsonMixin):
         self: str
         html: str
 
     commit: Commit
     name: str
-    _links: Links  
+    _links: Links
 
 
 from typing import Protocol
 
 
 class BaseGithubClient(Protocol):
     def get_all_endpoints(self) -> Dict[str, str]:
```

### Comparing `llama_hub-0.0.4/llama_hub/github_repo/utils.py` & `llama_hub-0.0.5/llama_hub/github_repo/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,22 +160,19 @@
                     start:end
                 ]  # TODO: use batch_size instead of buffer_size for concurrent requests
             ]
         )
         if self._verbose:
             end_t = time.time()
             blob_names_and_sizes = [
-                (blob.path, blob.size)
-                for blob, _ in self._blobs_and_paths[start:end]
+                (blob.path, blob.size) for blob, _ in self._blobs_and_paths[start:end]
             ]
             print(
                 "Time to get blobs ("
                 + f"{blob_names_and_sizes}"
                 + f"): {end_t - start_t:.2f} seconds"
             )
 
         self._buffer = [
             (result, path)
-            for result, (_, path) in zip(
-                results, self._blobs_and_paths[start:end]
-            )
+            for result, (_, path) in zip(results, self._blobs_and_paths[start:end])
         ]
```

### Comparing `llama_hub-0.0.4/llama_hub/gmail/README.md` & `llama_hub-0.0.5/llama_hub/gmail/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/gmail/base.py` & `llama_hub-0.0.5/llama_hub/gmail/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,37 +14,35 @@
 
     Reads emails
 
     Args:
         query (str): Gmail query. Defaults to None.
         max_results (int): Max number of results. Defaults to 10.
     """
+
     query: str = None
     use_iterative_parser: bool = False
     max_results: int = 10
     service: Any
 
-    def load_data(
-        self
-    ) -> List[Document]:
-        """Load emails from the user's account
-        """
+    def load_data(self) -> List[Document]:
+        """Load emails from the user's account"""
         from googleapiclient.discovery import build
 
         credentials = self._get_credentials()
         if not self.service:
-            self.service = build('gmail', 'v1', credentials=credentials)
+            self.service = build("gmail", "v1", credentials=credentials)
 
         messsages = self.search_messages()
 
         results = []
         for message in messsages:
-            text = message.pop('body')
+            text = message.pop("body")
             extra_info = message
-            results.append(Document(text, extra_info=extra_info))
+            results.append(Document(text=text, extra_info=extra_info))
 
         return results
 
     def _get_credentials(self) -> Any:
         """Get valid user credentials from storage.
 
         The file token.json stores the user's access and refresh tokens, and is
@@ -78,86 +76,89 @@
         return creds
 
     def search_messages(self):
         query = self.query
 
         max_results = self.max_results
 
-        messages = self.service.users().messages().list(
-            userId='me',
-            q=query,
-            maxResults=int(max_results)
-        ).execute().get('messages', [])
+        messages = (
+            self.service.users()
+            .messages()
+            .list(userId="me", q=query, maxResults=int(max_results))
+            .execute()
+            .get("messages", [])
+        )
 
         result = []
         try:
             for message in messages:
                 message_data = self.get_message_data(message)
                 if not message_data:
                     continue
                 result.append(message_data)
         except Exception as e:
             raise Exception("Can't get message data" + str(e))
 
         return result
 
     def get_message_data(self, message):
-        message_id = message['id']
-        message_data = self.service.users().messages().get(
-            format="raw",
-            userId='me',
-            id=message_id).execute()
+        message_id = message["id"]
+        message_data = (
+            self.service.users()
+            .messages()
+            .get(format="raw", userId="me", id=message_id)
+            .execute()
+        )
         if self.use_iterative_parser:
             body = self.extract_message_body_iterative(message_data)
         else:
             body = self.extract_message_body(message_data)
 
         if not body:
             return None
 
         return {
-            "id": message_data['id'],
-            "threadId": message_data['threadId'],
-            "snippet": message_data['snippet'],
+            "id": message_data["id"],
+            "threadId": message_data["threadId"],
+            "snippet": message_data["snippet"],
             "body": body,
         }
-    
-    def extract_message_body_iterative(self, message:dict):
-        if message['raw']:
-            body = base64.urlsafe_b64decode(message['raw'].encode('utf8'))
+
+    def extract_message_body_iterative(self, message: dict):
+        if message["raw"]:
+            body = base64.urlsafe_b64decode(message["raw"].encode("utf8"))
             mime_msg = email.message_from_bytes(body)
         else:
             mime_msg = message
-        
-        body_text = ''
-        if mime_msg.get_content_type() == 'text/plain':
+
+        body_text = ""
+        if mime_msg.get_content_type() == "text/plain":
             plain_text = mime_msg.get_payload(decode=True)
-            charset = mime_msg.get_content_charset('utf-8')
-            body_text = plain_text.decode(charset).encode('utf-8').decode('utf-8')
-            
-        elif mime_msg.get_content_maintype() == 'multipart':
+            charset = mime_msg.get_content_charset("utf-8")
+            body_text = plain_text.decode(charset).encode("utf-8").decode("utf-8")
+
+        elif mime_msg.get_content_maintype() == "multipart":
             msg_parts = mime_msg.get_payload()
             for msg_part in msg_parts:
                 body_text += self.extract_message_body_iterative(msg_part)
-                
+
         return body_text
 
     def extract_message_body(self, message: dict):
         from bs4 import BeautifulSoup
+
         try:
-            body = base64.urlsafe_b64decode(message['raw'].encode('ASCII'))
+            body = base64.urlsafe_b64decode(message["raw"].encode("ASCII"))
             mime_msg = email.message_from_bytes(body)
 
             # If the message body contains HTML, parse it with BeautifulSoup
-            if 'text/html' in mime_msg:
-                soup = BeautifulSoup(body, 'html.parser')
+            if "text/html" in mime_msg:
+                soup = BeautifulSoup(body, "html.parser")
                 body = soup.get_text()
             return body.decode("ascii")
         except Exception as e:
             raise Exception("Can't parse message body" + str(e))
 
 
 if __name__ == "__main__":
     reader = GmailReader(query="from:me after:2023-01-01")
-    print(
-        reader.load_data()
-    )
+    print(reader.load_data())
```

### Comparing `llama_hub-0.0.4/llama_hub/google_calendar/README.md` & `llama_hub-0.0.5/llama_hub/google_calendar/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/google_calendar/base.py` & `llama_hub-0.0.5/llama_hub/google_calendar/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             display_name = organizer.get("displayName", "N/A")
             email = organizer.get("email", "N/A")
             if display_name != "N/A":
                 event_string += f"Organizer: {display_name} ({email})"
             else:
                 event_string += f"Organizer: {email}"
 
-            results.append(Document(event_string))
+            results.append(Document(text=event_string))
 
         return results
 
     def _get_credentials(self) -> Any:
         """Get valid user credentials from storage.
 
         The file token.json stores the user's access and refresh tokens, and is
```

### Comparing `llama_hub-0.0.4/llama_hub/google_docs/README.md` & `llama_hub-0.0.5/llama_hub/google_docs/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/google_docs/base.py` & `llama_hub-0.0.5/llama_hub/google_docs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         """
         if document_ids is None:
             raise ValueError('Must specify a "document_ids" in `load_kwargs`.')
 
         results = []
         for document_id in document_ids:
             doc = self._load_doc(document_id)
-            results.append(Document(doc, extra_info={"document_id": document_id}))
+            results.append(Document(text=doc, extra_info={"document_id": document_id}))
         return results
 
     def _load_doc(self, document_id: str) -> str:
         """Load a document from Google Docs.
 
         Args:
             document_id: the document id.
```

### Comparing `llama_hub-0.0.4/llama_hub/google_drive/README.md` & `llama_hub-0.0.5/llama_hub/google_drive/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/google_drive/base.py` & `llama_hub-0.0.5/llama_hub/google_drive/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -102,15 +102,18 @@
         gauth.SaveCredentialsFile(self.pydrive_creds_path)
 
         drive = GoogleDrive(gauth)
 
         return creds, drive
 
     def _get_fileids_meta(
-        self, folder_id: Optional[str] = None, file_id: Optional[str] = None, mime_types: Optional[list] = None
+        self,
+        folder_id: Optional[str] = None,
+        file_id: Optional[str] = None,
+        mime_types: Optional[list] = None,
     ) -> List[List[str]]:
         """Get file ids present in folder/ file id
         Args:
             folder_id: folder id of the folder in google drive.
             file_id: file id of the file in google drive
             mime_types: the mimeTypes you want to allow e.g.: "application/vnd.google-apps.document"
         Returns:
@@ -121,55 +124,75 @@
         try:
             service = build("drive", "v3", credentials=self._creds)
             fileids_meta = []
             if folder_id:
                 folder_mime_type = "application/vnd.google-apps.folder"
                 query = "'" + folder_id + "' in parents"
 
-                #Add mimeType filter to query
+                # Add mimeType filter to query
                 if mime_types:
                     if folder_mime_type not in mime_types:
-                        mime_types.append(folder_mime_type) #keep the recursiveness
-                    mime_query = " or ".join([f"mimeType='{mime_type}'" for mime_type in mime_types])
+                        mime_types.append(folder_mime_type)  # keep the recursiveness
+                    mime_query = " or ".join(
+                        [f"mimeType='{mime_type}'" for mime_type in mime_types]
+                    )
                     query += f" and ({mime_query})"
 
-                results = service.files().list(
-                    q=query, 
-                    includeItemsFromAllDrives=True,
-                    supportsAllDrives=True, 
-                    fields="*"
-                ).execute()
+                results = (
+                    service.files()
+                    .list(
+                        q=query,
+                        includeItemsFromAllDrives=True,
+                        supportsAllDrives=True,
+                        fields="*",
+                    )
+                    .execute()
+                )
                 items = results.get("files", [])
                 for item in items:
                     if item["mimeType"] == folder_mime_type:
                         fileids_meta.extend(
-                            self._get_fileids_meta(folder_id=item["id"], mime_types=mime_types)
+                            self._get_fileids_meta(
+                                folder_id=item["id"], mime_types=mime_types
+                            )
                         )
                     else:
                         # Check if file doesn't belong to a Shared Drive. "owners" doesn't exist in a Shared Drive
-                        is_shared_drive = 'driveId' in item
-                        author = item["owners"][0]["displayName"] if not is_shared_drive else "Shared Drive"
+                        is_shared_drive = "driveId" in item
+                        author = (
+                            item["owners"][0]["displayName"]
+                            if not is_shared_drive
+                            else "Shared Drive"
+                        )
 
                         fileids_meta.append(
                             (
                                 item["id"],
                                 author,
                                 item["name"],
                                 item["createdTime"],
                                 item["modifiedTime"],
                             )
                         )
 
             else:
                 # Get the file details
-                file = service.files().get(fileId=file_id, supportsAllDrives=True, fields="*").execute()
+                file = (
+                    service.files()
+                    .get(fileId=file_id, supportsAllDrives=True, fields="*")
+                    .execute()
+                )
                 # Get metadata of the file
                 # Check if file doesn't belong to a Shared Drive. "owners" doesn't exist in a Shared Drive
-                is_shared_drive = 'driveId' in file
-                author = file["owners"][0]["displayName"] if not is_shared_drive else "Shared Drive"
+                is_shared_drive = "driveId" in file
+                author = (
+                    file["owners"][0]["displayName"]
+                    if not is_shared_drive
+                    else "Shared Drive"
+                )
 
                 fileids_meta.append(
                     (
                         file["id"],
                         author,
                         file["name"],
                         file["createdTime"],
@@ -197,21 +220,23 @@
         from googleapiclient.discovery import build
 
         try:
             # Get file details
             service = build("drive", "v3", credentials=self._creds)
             file = service.files().get(fileId=fileid, supportsAllDrives=True).execute()
 
-            if file['mimeType'] in self._mimetypes:
-                download_mimetype = self._mimetypes[file['mimeType']]['mimetype']
-                download_extension = self._mimetypes[file['mimeType']]['extension']
+            if file["mimeType"] in self._mimetypes:
+                download_mimetype = self._mimetypes[file["mimeType"]]["mimetype"]
+                download_extension = self._mimetypes[file["mimeType"]]["extension"]
                 new_file_name = filename + download_extension
 
                 # Download and convert file
-                request = service.files().export_media(fileId=fileid, mimeType=download_mimetype)
+                request = service.files().export_media(
+                    fileId=fileid, mimeType=download_mimetype
+                )
             else:
                 new_file_name = filename
 
                 # Download file without conversion
                 request = service.files().get_media(fileId=fileid)
 
             # Download file data
@@ -219,15 +244,15 @@
             downloader = MediaIoBaseDownload(file_data, request)
             done = False
 
             while not done:
                 status, done = downloader.next_chunk()
 
             # Save the downloaded file
-            with open(new_file_name, 'wb') as f:
+            with open(new_file_name, "wb") as f:
                 f.write(file_data.getvalue())
 
             return new_file_name
         except Exception as e:
             logger.error("An error occurred while downloading file: {}".format(e))
 
     def _load_data_fileids_meta(self, fileids_meta: List[List[str]]) -> List[Document]:
@@ -258,38 +283,43 @@
                         "author": fileid_meta[1],
                         "file name": fileid_meta[2],
                         "created at": fileid_meta[3],
                         "modified at": fileid_meta[4],
                     }
                 try:
                     from llama_hub.utils import import_loader
+
                     SimpleDirectoryReader = import_loader("SimpleDirectoryReader")
                 except ImportError:
                     SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
                 loader = SimpleDirectoryReader(temp_dir, file_metadata=get_metadata)
                 documents = loader.load_data()
 
             return documents
         except Exception as e:
             logger.error(
                 "An error occurred while loading data from fileids meta: {}".format(e)
             )
 
-    def _load_from_file_ids(self, file_ids: List[str], mime_types: list) -> List[Document]:
+    def _load_from_file_ids(
+        self, file_ids: List[str], mime_types: list
+    ) -> List[Document]:
         """Load data from file ids
         Args:
             file_ids: file ids of the files in google drive.
         Returns:
             Document: List of Documents of text.
         """
 
         try:
             fileids_meta = []
             for file_id in file_ids:
-                fileids_meta.extend(self._get_fileids_meta(file_id=file_id, mime_types=mime_types))
+                fileids_meta.extend(
+                    self._get_fileids_meta(file_id=file_id, mime_types=mime_types)
+                )
             documents = self._load_data_fileids_meta(fileids_meta)
 
             return documents
         except Exception as e:
             logger.error("An error occurred while loading with fileid: {}".format(e))
 
     def _load_from_folder(self, folder_id: str, mime_types: list) -> List[Document]:
@@ -297,22 +327,27 @@
         Args:
             folder_id: folder id of the folder in google drive.
             mime_types: the mimeTypes you want to allow e.g.: "application/vnd.google-apps.document"
         Returns:
             Document: List of Documents of text.
         """
         try:
-            fileids_meta = self._get_fileids_meta(folder_id=folder_id,mime_types=mime_types)
+            fileids_meta = self._get_fileids_meta(
+                folder_id=folder_id, mime_types=mime_types
+            )
             documents = self._load_data_fileids_meta(fileids_meta)
             return documents
         except Exception as e:
             logger.error("An error occurred while loading from folder: {}".format(e))
 
     def load_data(
-        self, folder_id: str = None, file_ids: List[str] = None, mime_types: List[str] = None
+        self,
+        folder_id: str = None,
+        file_ids: List[str] = None,
+        mime_types: List[str] = None,
     ) -> List[Document]:
         """Load data from the folder id and file ids.
         Args:
             folder_id: folder id of the folder in google drive.
             file_ids: file ids of the files in google drive.
             mime_types: the mimeTypes you want to allow e.g.: "application/vnd.google-apps.document"
         Returns:
```

### Comparing `llama_hub-0.0.4/llama_hub/google_sheets/README.md` & `llama_hub-0.0.5/llama_hub/google_sheets/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/google_sheets/base.py` & `llama_hub-0.0.5/llama_hub/google_sheets/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         if spreadsheet_ids is None:
             raise ValueError('Must specify a "spreadsheet_ids" in `load_kwargs`.')
 
         results = []
         for spreadsheet_id in spreadsheet_ids:
             sheet = self._load_sheet(spreadsheet_id)
             results.append(
-                Document(sheet, extra_info={"spreadsheet_id": spreadsheet_id})
+                Document(text=sheet, extra_info={"spreadsheet_id": spreadsheet_id})
             )
         return results
 
     def _load_sheet(self, spreadsheet_id: str) -> str:
         """Load a sheet from Google Sheets.
 
         Args:
```

### Comparing `llama_hub-0.0.4/llama_hub/gpt_repo/README.md` & `llama_hub-0.0.5/llama_hub/gpt_repo/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/gpt_repo/base.py` & `llama_hub-0.0.5/llama_hub/gpt_repo/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,10 +146,10 @@
             )
         text_list = process_repository(
             repo_path, ignore_list, concatenate=self.concatenate, extensions=extensions
         )
         docs = []
         for text in text_list:
             doc_text = output_text + text + "\n--END--\n"
-            docs.append(Document(doc_text))
+            docs.append(Document(text=doc_text))
 
         return docs
```

### Comparing `llama_hub-0.0.4/llama_hub/graphdb_cypher/README.md` & `llama_hub-0.0.5/llama_hub/graphdb_cypher/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/graphdb_cypher/base.py` & `llama_hub-0.0.5/llama_hub/graphdb_cypher/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,47 +3,44 @@
 from typing import Dict, List, Optional
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 import yaml
 
+
 class GraphDBCypherReader(BaseReader):
     """Graph database Cypher reader.
 
     Combines all Cypher query results into the Document type used by LlamaIndex.
 
     Args:
         uri (str): Graph Database URI
         username (str): Username
-        password (str): Password 
+        password (str): Password
 
     """
 
-    def __init__(
-        self,
-        uri: str,
-        username: str,
-        password: str,
-        database: str
-    ) -> None:
+    def __init__(self, uri: str, username: str, password: str, database: str) -> None:
         """Initialize with parameters."""
         try:
             from neo4j import GraphDatabase, basic_auth
 
         except ImportError:
             raise ImportError(
                 "`neo4j` package not found, please run `pip install neo4j`"
             )
         if uri:
             if uri is None:
                 raise ValueError("`uri` must be provided.")
-            self.client = GraphDatabase.driver(uri=uri, auth=basic_auth(username, password))
+            self.client = GraphDatabase.driver(
+                uri=uri, auth=basic_auth(username, password)
+            )
             self.database = database
-            
+
     def load_data(
         self, query: str, parameters: Optional[Dict] = None
     ) -> List[Document]:
         """Run the Cypher with optional parameters and turn results into documents
 
         Args:
             query (str): Graph Cypher query string.
@@ -52,12 +49,14 @@
         Returns:
             List[Document]: A list of documents.
 
         """
         if parameters is None:
             parameters = {}
 
-        records, summary, keys = self.client.execute_query(query, parameters, database_ = self.database)
+        records, summary, keys = self.client.execute_query(
+            query, parameters, database_=self.database
+        )
 
-        documents = [Document(yaml.dump(entry.data())) for entry in records]
+        documents = [Document(text=yaml.dump(entry.data())) for entry in records]
 
-        return documents
+        return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/graphql/README.md` & `llama_hub-0.0.5/llama_hub/graphql/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/graphql/base.py` & `llama_hub-0.0.5/llama_hub/graphql/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,53 +25,47 @@
     ) -> None:
         """Initialize with parameters."""
         try:
             from gql import Client
             from gql.transport.requests import RequestsHTTPTransport
 
         except ImportError:
-            raise ImportError(
-                "`gql` package not found, please run `pip install gql`"
-            )
+            raise ImportError("`gql` package not found, please run `pip install gql`")
         if uri:
             if uri is None:
                 raise ValueError("`uri` must be provided.")
             if headers is None:
                 headers = {}
             transport = RequestsHTTPTransport(url=uri, headers=headers)
             self.client = Client(transport=transport, fetch_schema_from_transport=True)
-            
-    def load_data(
-        self, query: str, variables: Optional[Dict] = None
-    ) -> List[Document]:
+
+    def load_data(self, query: str, variables: Optional[Dict] = None) -> List[Document]:
         """Run query with optional variables and turn results into documents
 
         Args:
             query (str): GraphQL query string.
             variables (Optional[Dict]): optional query parameters.
 
         Returns:
             List[Document]: A list of documents.
 
         """
         try:
             from gql import gql
 
         except ImportError:
-            raise ImportError(
-                "`gql` package not found, please run `pip install gql`"
-            )
+            raise ImportError("`gql` package not found, please run `pip install gql`")
         if variables is None:
             variables = {}
 
         documents = []
-        
-        result = self.client.execute(gql(query), variable_values = variables)
+
+        result = self.client.execute(gql(query), variable_values=variables)
 
         for key in result:
             entry = result[key]
             if type(entry) == list:
-                documents.extend([Document(yaml.dump(v)) for v in entry])
+                documents.extend([Document(text=yaml.dump(v)) for v in entry])
             else:
-                documents.append(Document(yaml.dump(entry)))
+                documents.append(Document(text=yaml.dump(entry)))
 
-        return documents
+        return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/hatena_blog/README.md` & `llama_hub-0.0.5/llama_hub/hatena_blog/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/hatena_blog/base.py` & `llama_hub-0.0.5/llama_hub/hatena_blog/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Hatena Blog reader."""
 
 from typing import List, Dict
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
-ATOM_PUB_ENTRY_URL = '{root_endpoint}/entry'
+ATOM_PUB_ENTRY_URL = "{root_endpoint}/entry"
 
 
 class Article:
     def __init__(self) -> None:
-        self.title = ''
-        self.content = ''
-        self.published = ''
+        self.title = ""
+        self.content = ""
+        self.published = ""
 
 
 class HatenaBlogReader(BaseReader):
     """Hatena Blog reader.
 
     Args:
         root_endpoint (str): AtomPub root endpoint.
@@ -30,53 +30,60 @@
         self.username = username
 
     def load_data(self) -> List[Document]:
         results = []
         articles = self.get_all_articles()
         for a in articles:
             results.append(
-                Document(a.content, extra_info={'title': a.title, 'published': a.published})
+                Document(
+                    text=a.content,
+                    extra_info={"title": a.title, "published": a.published},
+                )
             )
 
         return results
 
     def get_all_articles(self) -> List[Article]:
         articles: List[Article] = []
         page_url = ATOM_PUB_ENTRY_URL.format(root_endpoint=self.root_endpoint)
 
         while True:
             res = self.get_articles(page_url)
-            articles += res.get('articles')
-            page_url = res.get('next_page')
+            articles += res.get("articles")
+            page_url = res.get("next_page")
             if page_url is None:
                 break
 
         return articles
 
     def get_articles(self, url: str) -> Dict:
         import requests
         from requests.auth import HTTPBasicAuth
         from bs4 import BeautifulSoup
 
         articles: List[Article] = []
         next_page = None
 
         res = requests.get(url, auth=HTTPBasicAuth(self.username, self.api_key))
-        soup = BeautifulSoup(res.text, 'xml')
-        for entry in soup.find_all('entry'):
-            if entry.find('app:control').find('app:draft').string == 'yes':
+        soup = BeautifulSoup(res.text, "xml")
+        for entry in soup.find_all("entry"):
+            if entry.find("app:control").find("app:draft").string == "yes":
                 continue
             article = Article()
-            article.title = entry.find('title').string
-            article.published = entry.find('published').string
-            content = entry.find('content')
-            if content.get('type') == 'text/html':
-                article.content = BeautifulSoup(entry.find('content').string, 'html.parser').get_text().strip()
+            article.title = entry.find("title").string
+            article.published = entry.find("published").string
+            content = entry.find("content")
+            if content.get("type") == "text/html":
+                article.content = (
+                    BeautifulSoup(entry.find("content").string, "html.parser")
+                    .get_text()
+                    .strip()
+                )
             else:
-                article.content = entry.find('content').string.strip()
+                article.content = entry.find("content").string.strip()
             articles.append(article)
 
-        next = soup.find('link', attrs={'rel': 'next'})
+        next = soup.find("link", attrs={"rel": "next"})
         if next:
-            next_page = next.get('href')
+            next_page = next.get("href")
 
-        return {'articles': articles, 'next_page': next_page}
+        return {"articles": articles, "next_page": next_page}
```

### Comparing `llama_hub-0.0.4/llama_hub/hubspot/README.md` & `llama_hub-0.0.5/llama_hub/hubspot/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/hubspot/base.py` & `llama_hub-0.0.5/llama_hub/hubspot/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,32 +7,39 @@
 
 class HubspotReader(BaseReader):
     """Hubspot reader. Reads data from a Hubspot account.
 
     Args:
         access_token(str): Hubspot API key.
     """
-    
+
     def __init__(self, access_token: str) -> None:
         """Initialize Hubspot reader."""
-        
 
         self.access_token = access_token
 
-
     def load_data(self) -> List[Document]:
         """Load deals, contacts and companies data from Hubspot
-        
+
         Returns:
             List[Document]: List of documents, where each document represensts a list of Hubspot objects
         """
         from hubspot import HubSpot
+
         api_client = HubSpot(access_token=self.access_token)
         all_deals = api_client.crm.deals.get_all()
         all_contacts = api_client.crm.contacts.get_all()
         all_companies = api_client.crm.companies.get_all()
         results = [
-            Document(f"{all_deals}".replace("\n", ""), extra_info={type: "deals"}), 
-            Document(f"{all_contacts}".replace("\n", ""), extra_info={type: "contacts"}),
-            Document(f"{all_companies}".replace("\n", ""), extra_info={type: "companies"})
+            Document(
+                text=f"{all_deals}".replace("\n", ""), extra_info={"type": "deals"}
+            ),
+            Document(
+                text=f"{all_contacts}".replace("\n", ""),
+                extra_info={"type": "contacts"},
+            ),
+            Document(
+                text=f"{all_companies}".replace("\n", ""),
+                extra_info={"type": "companies"},
+            ),
         ]
-        return results
+        return results
```

### Comparing `llama_hub-0.0.4/llama_hub/huggingface/fs/README.md` & `llama_hub-0.0.5/llama_hub/huggingface/fs/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/huggingface/fs/base.py` & `llama_hub-0.0.5/llama_hub/huggingface/fs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 A parser for HF files.
 
 """
 import json
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import Any, Dict, List, Optional
+from typing import Dict, List
 
 import pandas as pd
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 
 class HuggingFaceFSReader(BaseReader):
@@ -63,9 +63,9 @@
         return pd.DataFrame(self.load_dicts(path))
 
     def load_data(self, path: str) -> List[Document]:
         """Load data."""
         json_dicts = self.load_dicts(path)
         docs = []
         for d in json_dicts:
-            docs.append(Document(str(d)))
+            docs.append(Document(text=str(d)))
         return docs
```

### Comparing `llama_hub-0.0.4/llama_hub/intercom/README.md` & `llama_hub-0.0.5/llama_hub/intercom/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/intercom/base.py` & `llama_hub-0.0.5/llama_hub/zendesk/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,94 +1,85 @@
-"""Intercom reader."""
-from typing import List
+"""Zendesk reader."""
 import json
+from typing import List
+
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 
-class IntercomReader(BaseReader):
-    """Intercom reader. Reads data from a Intercom workspace.
+class ZendeskReader(BaseReader):
+    """Zendesk reader. Reads data from a Zendesk workspace.
 
     Args:
-        personal_access_token (str): Intercom token.
+        zendesk_subdomain (str): Zendesk subdomain
+        locale (str): Locale of articles
     """
 
-    def __init__(self, intercom_access_token: str) -> None:
-        """Initialize Intercom reader."""
-
-        self.intercom_access_token = intercom_access_token
+    def __init__(self, zendesk_subdomain: str, locale: str = "en-us") -> None:
+        """Initialize Zendesk reader."""
+        self.zendesk_subdomain = zendesk_subdomain
+        self.locale = locale
 
     def load_data(self) -> List[Document]:
         """Load data from the workspace.
 
         Args:
             workspace_id (str): Workspace ID.
         Returns:
             List[Document]: List of documents.
         """
         from bs4 import BeautifulSoup
 
         results = []
 
         articles = self.get_all_articles()
-
         for article in articles:
-
-            body = article['body']
-            soup = BeautifulSoup(body, 'html.parser')
+            body = article["body"]
+            soup = BeautifulSoup(body, "html.parser")
             body = soup.get_text()
-
             extra_info = {
-                "id": article['id'],
-                "title": article['title'],
-                "url": article['url'],
-                "updated_at": article['updated_at']
+                "id": article["id"],
+                "title": article["title"],
+                "url": article["html_url"],
+                "updated_at": article["updated_at"],
             }
 
             results.append(
                 Document(
-                    body,
+                    text=body,
                     extra_info=extra_info,
                 )
             )
 
         return results
 
     def get_all_articles(self):
         articles = []
         next_page = None
 
         while True:
             response = self.get_articles_page(next_page)
-            articles.extend(response['articles'])
-            next_page = response['next_page']
+            articles.extend(response["articles"])
+            next_page = response["next_page"]
 
             if next_page is None:
                 break
 
         return articles
 
     def get_articles_page(self, next_page: str = None):
         import requests
+
         if next_page is None:
-            url = "https://api.intercom.io/articles"
+            url = f"https://{self.zendesk_subdomain}.zendesk.com/api/v2/help_center/{self.locale}/articles?per_page=100"
         else:
             url = next_page
 
-        headers = {
-            "accept": "application/json",
-            "Intercom-Version": "2.8",
-            "authorization": f"Bearer {self.intercom_access_token}"
-        }
-
-        response = requests.get(url, headers=headers)
+        response = requests.get(url)
 
         response_json = json.loads(response.text)
 
-        next_page = response_json.get('pages', {}).get('next', None)
+        next_page = response_json.get("next_page", None)
 
-        articles = response_json.get('data', [])
+        articles = response_json.get("articles", [])
 
-        return {
-            "articles": articles,
-            "next_page": next_page
-        }
+        return {"articles": articles, "next_page": next_page}
```

### Comparing `llama_hub-0.0.4/llama_hub/jira/README.md` & `llama_hub-0.0.5/llama_hub/jira/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/jira/base.py` & `llama_hub-0.0.5/llama_hub/jira/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,90 +1,94 @@
 from typing import List
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
+
 def safe_value_dict(dict_obj):
     for key, value in dict_obj.items():
         if isinstance(value, (str, int, float)):
             dict_obj[key] = value
         elif isinstance(value, list):
             # Convert lists to strings
-            dict_obj[key] = ', '.join(map(str, value))
+            dict_obj[key] = ", ".join(map(str, value))
         elif value is None:
             # Replace None with a default string
-            dict_obj[key] = ''
+            dict_obj[key] = ""
         else:
             # Convert other types to strings
             dict_obj[key] = str(value)
     return dict_obj
 
+
 class JiraReader(BaseReader):
     """Jira reader. Reads data from Jira issues from passed query.
 
     Args:
         email (str): Jira email.
         api_token (str): Jira API token.
         server_url (str): Jira server url.
     """
 
     def __init__(self, email: str, api_token: str, server_url: str) -> None:
 
         from jira import JIRA
 
-        self.jira = JIRA(
-            basic_auth=(email, api_token),
-            server=f'https://{server_url}'
-        )
+        self.jira = JIRA(basic_auth=(email, api_token), server=f"https://{server_url}")
 
     def load_data(self, query: str) -> List[Document]:
         relevant_issues = self.jira.search_issues(query)
 
         issues = []
 
         for issue in relevant_issues:
             # Iterates through only issues and not epics
-            if 'parent' in (issue.raw['fields']):
-                assignee = ''
-                reporter = ''
-                epic_key = ''
-                epic_summary = ''
-                epic_descripton = ''
+            if "parent" in (issue.raw["fields"]):
+                assignee = ""
+                reporter = ""
+                epic_key = ""
+                epic_summary = ""
+                epic_descripton = ""
 
                 if issue.fields.assignee:
                     assignee = issue.fields.assignee.displayName
 
                 if issue.fields.reporter:
                     reporter = issue.fields.reporter.displayName
 
-                if issue.raw['fields']['parent']['key']:
-                    epic_key = issue.raw['fields']['parent']['key']
+                if issue.raw["fields"]["parent"]["key"]:
+                    epic_key = issue.raw["fields"]["parent"]["key"]
 
-                if issue.raw['fields']['parent']['fields']['summary']:
-                    epic_summary = issue.raw['fields']['parent']['fields']['summary']
+                if issue.raw["fields"]["parent"]["fields"]["summary"]:
+                    epic_summary = issue.raw["fields"]["parent"]["fields"]["summary"]
 
-                if issue.raw['fields']['parent']['fields']['status']['description']:
-                    epic_descripton = issue.raw['fields']['parent']['fields']['status']['description']
+                if issue.raw["fields"]["parent"]["fields"]["status"]["description"]:
+                    epic_descripton = issue.raw["fields"]["parent"]["fields"]["status"][
+                        "description"
+                    ]
 
                 issues.append(
                     Document(
-                        f"{issue.fields.summary} \n {issue.fields.description}",
-                        extra_info = safe_value_dict({
-                            'id': issue.id,
-                            'title': issue.fields.summary,
-                            'url': issue.permalink(),
-                            'created_at': issue.fields.created,
-                            'updated_at': issue.fields.updated,
-                            'labels': issue.fields.labels,
-                            'status': issue.fields.status.name,
-                            'assignee': assignee,
-                            'reporter': reporter,
-                            'project': issue.fields.project.name,
-                            'issue_type': issue.fields.issuetype.name,
-                            'priority': issue.fields.priority.name,
-                            'epic_key': epic_key,
-                            'epic_summary': epic_summary,
-                            'epic_description': epic_descripton})
+                        text=f"{issue.fields.summary} \n {issue.fields.description}",
+                        extra_info=safe_value_dict(
+                            {
+                                "id": issue.id,
+                                "title": issue.fields.summary,
+                                "url": issue.permalink(),
+                                "created_at": issue.fields.created,
+                                "updated_at": issue.fields.updated,
+                                "labels": issue.fields.labels,
+                                "status": issue.fields.status.name,
+                                "assignee": assignee,
+                                "reporter": reporter,
+                                "project": issue.fields.project.name,
+                                "issue_type": issue.fields.issuetype.name,
+                                "priority": issue.fields.priority.name,
+                                "epic_key": epic_key,
+                                "epic_summary": epic_summary,
+                                "epic_description": epic_descripton,
+                            }
+                        ),
                     )
                 )
 
         return issues
```

### Comparing `llama_hub-0.0.4/llama_hub/joplin/README.md` & `llama_hub-0.0.5/llama_hub/joplin/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/joplin/base.py` & `llama_hub-0.0.5/llama_hub/joplin/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 When Joplin is installed and running it will parse all markdown
 files into a List of Documents.
 
 """
 from datetime import datetime
 import json
 import os
-from typing import Any, Iterator, List, Optional
+from typing import Iterator, List, Optional
 import urllib
 
 from llama_index import download_loader
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 LINK_NOTE_TEMPLATE = "joplin://x-callback-url/openNote?id={id}"
@@ -49,14 +49,15 @@
             port (int): The port on which Joplin's Web Clipper service is running. Default is 41184.
             host (str): The host on which Joplin's Web Clipper service is running. Default is "localhost".
         """
         self.parse_markdown = parse_markdown
         if parse_markdown:
             try:
                 from llama_hub.utils import import_loader
+
                 mr = import_loader("MarkdownReader")
             except:
                 mr = download_loader("MarkdownReader")
             self.parser = mr()
 
         access_token = access_token or self._get_token_from_env()
         base_url = f"http://{host}:{port}"
```

### Comparing `llama_hub-0.0.4/llama_hub/jsondata/README.md` & `llama_hub-0.0.5/llama_hub/jsondata/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/jsondata/base.py` & `llama_hub-0.0.5/llama_hub/jsondata/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import json
 import re
 from typing import Dict, Generator, List, Union
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
+
 def _depth_first_yield(json_data: Dict, path: List[str]) -> Generator[str, None, None]:
     """Do depth first yield of all of the leaf nodes of a JSON.
 
     Combines keys in the JSON tree using spaces.
 
     """
     if isinstance(json_data, dict):
@@ -44,11 +45,9 @@
         """Load data from the input file."""
         if isinstance(input_data, str):
             data = json.loads(input_data)
         else:
             data = input_data
         json_output = json.dumps(data, indent=0)
         lines = json_output.split("\n")
-        useful_lines = [
-            line for line in lines if not re.match(r"^[{}\[\],]*$", line)
-        ]
-        return [Document("\n".join(useful_lines))]
+        useful_lines = [line for line in lines if not re.match(r"^[{}\[\],]*$", line)]
+        return [Document(text="\n".join(useful_lines))]
```

### Comparing `llama_hub-0.0.4/llama_hub/kaltura/esearch/README.md` & `llama_hub-0.0.5/llama_hub/kaltura/esearch/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/kaltura/esearch/base.py` & `llama_hub-0.0.5/llama_hub/kaltura/esearch/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 import json
 from typing import Optional, List, Dict, Any
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 logger = logging.getLogger(__name__)
 
+
 class KalturaESearchReader(BaseReader):
     """Kaltura eSearch API Reader."""
 
     def __init__(
         self,
-        partner_id: int = 0,  
-        api_secret: str = "INSERT_YOUR_ADMIN_SECRET", 
-        user_id: str = "INSERT_YOUR_USER_ID", 
+        partner_id: int = 0,
+        api_secret: str = "INSERT_YOUR_ADMIN_SECRET",
+        user_id: str = "INSERT_YOUR_USER_ID",
         ks_type: int = 2,
-        ks_expiry: int = 86400, 
-        ks_privileges: str = "disableentitlement", 
+        ks_expiry: int = 86400,
+        ks_privileges: str = "disableentitlement",
         kaltura_api_endpoint: str = "https://cdnapi-ev.kaltura.com/",
-        request_timeout: int = 500, 
-        should_log_api_calls: bool = False 
+        request_timeout: int = 500,
+        should_log_api_calls: bool = False,
     ) -> None:
         """
         Initialize a new instance of KalturaESearchReader.
 
         Args:
             partner_id (int): The Kaltura Account ID. Default is 0.
             api_secret (str): The Kaltura API Admin Secret. Default is "INSERT_YOUR_ADMIN_SECRET".
@@ -70,173 +71,186 @@
                 self.ks_type = KalturaSessionType.ADMIN
             self.ks = self.client.generateSessionV2(
                 self.api_secret,
                 self.user_id,
                 self.ks_type,
                 self.partner_id,
                 self.ks_expiry,
-                self.ks_privileges
+                self.ks_privileges,
             )
             self.client.setKs(self.ks)
             self._kaltura_loaded = True
-        except Exception as e:
-            logger.error(f'Kaltura Auth failed, check your credentials')
-    
+        except Exception:
+            logger.error("Kaltura Auth failed, check your credentials")
+
     def _load_from_search_params(
-        self, 
-        search_params, 
-        with_captions: bool = True, 
-        max_entries: int = 10
+        self, search_params, with_captions: bool = True, max_entries: int = 10
     ) -> List[Dict[str, Any]]:
         """Load search parameters and returns a list of entries.
 
         Args:
             search_params: Search parameters for Kaltura eSearch.
             with_captions (bool): If True, the entries will include captions.
             max_entries (int): Maximum number of entries to return.
 
         Returns:
-            list: A list of entries as dictionaries, 
-            if captions required entry_info will include all metadata and text will include transcript, 
+            list: A list of entries as dictionaries,
+            if captions required entry_info will include all metadata and text will include transcript,
             otherwise info is just entry_id and text is all metadata.
         """
         from KalturaClient.Plugins.Core import KalturaPager
 
         try:
             entries = []
             pager = KalturaPager()
             pager.pageIndex = 1
             pager.pageSize = max_entries
-            response = self.client.elasticSearch.eSearch.searchEntry(search_params, pager)
+            response = self.client.elasticSearch.eSearch.searchEntry(
+                search_params, pager
+            )
 
             for search_result in response.objects:
                 entry = search_result.object
                 items_data = search_result.itemsData
 
                 entry_info = {
-                    'entry_id': str(entry.id),
-                    'entry_name': str(entry.name),
-                    'entry_description': str(entry.description or ''),
-                    'entry_media_type': int(entry.mediaType.value or 0),
-                    'entry_media_date': int(entry.createdAt or 0),
-                    'entry_ms_duration': int(entry.msDuration or 0),
-                    'entry_last_played_at': int(entry.lastPlayedAt or 0),
-                    'entry_application': str(entry.application or ''),
-                    'entry_tags': str(entry.tags or ''),
-                    'entry_reference_id': str(entry.referenceId or '')
+                    "entry_id": str(entry.id),
+                    "entry_name": str(entry.name),
+                    "entry_description": str(entry.description or ""),
+                    "entry_media_type": int(entry.mediaType.value or 0),
+                    "entry_media_date": int(entry.createdAt or 0),
+                    "entry_ms_duration": int(entry.msDuration or 0),
+                    "entry_last_played_at": int(entry.lastPlayedAt or 0),
+                    "entry_application": str(entry.application or ""),
+                    "entry_tags": str(entry.tags or ""),
+                    "entry_reference_id": str(entry.referenceId or ""),
                 }
 
                 if with_captions:
                     caption_search_result = items_data[0].items[0]
-                    if hasattr(caption_search_result, 'captionAssetId'):
+                    if hasattr(caption_search_result, "captionAssetId"):
                         # TODO: change this to fetch captions per language, or as for a specific language code
                         caption_asset_id = caption_search_result.captionAssetId
-                        entry_dict = {'video_transcript': self._get_json_transcript(caption_asset_id)}
+                        entry_dict = {
+                            "video_transcript": self._get_json_transcript(
+                                caption_asset_id
+                            )
+                        }
                     else:
                         entry_dict = entry_info.copy()
-                        entry_info = {'entry_id': str(entry.id)}
+                        entry_info = {"entry_id": str(entry.id)}
                 else:
                     entry_dict = entry_info.copy()
-                    entry_info = {'entry_id': str(entry.id)}
+                    entry_info = {"entry_id": str(entry.id)}
 
                 entry_doc = Document(text=json.dumps(entry_dict), extra_info=entry_info)
                 entries.append(entry_doc)
 
             return entries
 
         except Exception as e:
             if e.code == "INVALID_KS":
-                raise ValueError(f'Kaltura Auth failed, check your credentials: {e}')
-            logger.error(f'An error occurred while loading with search params: {e}')
+                raise ValueError(f"Kaltura Auth failed, check your credentials: {e}")
+            logger.error(f"An error occurred while loading with search params: {e}")
             return []
 
-
     def _get_json_transcript(self, caption_asset_id):
         """Fetch json transcript/captions from a given caption_asset_id
-        
+
         Args:
             caption_asset_id: The ID of the caption asset that includes the captions to fetch json transcript for
 
         Returns:
             A JSON transcript of the captions, or an empty dictionary if none found or an error occurred.
         """
         # TODO: change this to fetch captions per language, or as for a specific language code
         try:
-            cap_json_url = self.client.caption.captionAsset.serveAsJson(caption_asset_id)
+            cap_json_url = self.client.caption.captionAsset.serveAsJson(
+                caption_asset_id
+            )
             cap_json = requests.get(cap_json_url).json()
             return cap_json
         except Exception as e:
-            logger.error(f'An error occurred while getting captions: {e}')
+            logger.error(f"An error occurred while getting captions: {e}")
             return {}
 
-  
-    def load_data(self, 
-              search_params: Any = None,
-              search_operator_and: bool = True, 
-              free_text: Optional[str] = None, 
-              category_ids: Optional[str] = None, 
-              with_captions: bool = True, 
-              max_entries: int = 5
-             ) -> List[Dict[str, Any]]:
-        """Load data from the Kaltura based on search parameters. 
-        The function returns a list of dictionaries. 
+    def load_data(
+        self,
+        search_params: Any = None,
+        search_operator_and: bool = True,
+        free_text: Optional[str] = None,
+        category_ids: Optional[str] = None,
+        with_captions: bool = True,
+        max_entries: int = 5,
+    ) -> List[Dict[str, Any]]:
+        """Load data from the Kaltura based on search parameters.
+        The function returns a list of dictionaries.
         Each dictionary represents a media entry, where the keys are strings (field names) and the values can be of any type.
 
         Args:
             search_params: search parameters of type KalturaESearchEntryParams with pre-set search queries. If not provided, the other parameters will be used to construct the search query.
             search_operator_and: if True, the constructed search query will have AND operator between query filters, if False, the operator will be OR.
             free_text: if provided, will be used as the free text query of the search in Kaltura.
             category_ids: if provided, will only search for entries that are found inside these category ids.
             withCaptions: determines whether or not to also download captions/transcript contents from Kaltura.
             maxEntries: sets the maximum number of entries to pull from Kaltura, between 0 to 500 (max pageSize in Kaltura).
 
         Returns:
-            List[Dict[str, Any]]: A list of dictionaries representing Kaltura Media Entries with the following fields: 
-            entry_id:str, entry_name:str, entry_description:str, entry_captions:JSON, 
-            entry_media_type:int, entry_media_date:int, entry_ms_duration:int, entry_last_played_at:int, 
-            entry_application:str, entry_tags:str, entry_reference_id:str. 
+            List[Dict[str, Any]]: A list of dictionaries representing Kaltura Media Entries with the following fields:
+            entry_id:str, entry_name:str, entry_description:str, entry_captions:JSON,
+            entry_media_type:int, entry_media_date:int, entry_ms_duration:int, entry_last_played_at:int,
+            entry_application:str, entry_tags:str, entry_reference_id:str.
             If with_captions is False, it sets entry_info to only include the entry_id and entry_dict to include all other entry information.
             If with_captions is True, it sets entry_info to include all entry information and entry_dict to only include the entry transcript fetched via self._get_captions(items_data).
         """
         from KalturaClient.Plugins.ElasticSearch import (
-            KalturaESearchCaptionItem, KalturaESearchCaptionFieldName, KalturaESearchUnifiedItem, 
-            KalturaESearchEntryParams, KalturaESearchCategoryEntryItem, KalturaESearchEntryOperator, 
-            KalturaESearchOperatorType, KalturaESearchItemType, KalturaCategoryEntryStatus, KalturaESearchCategoryEntryFieldName
+            KalturaESearchCaptionItem,
+            KalturaESearchCaptionFieldName,
+            KalturaESearchUnifiedItem,
+            KalturaESearchEntryParams,
+            KalturaESearchCategoryEntryItem,
+            KalturaESearchEntryOperator,
+            KalturaESearchOperatorType,
+            KalturaESearchItemType,
+            KalturaCategoryEntryStatus,
+            KalturaESearchCategoryEntryFieldName,
         )
 
         # Load and initialize the Kaltura client
         if not self._kaltura_loaded:
             self._load_kaltura()
 
         # Validate input parameters:
         if search_params is None:
             search_params = KalturaESearchEntryParams()
-            # Create an AND/OR relationship between the following search queries - 
+            # Create an AND/OR relationship between the following search queries -
             search_params.searchOperator = KalturaESearchEntryOperator()
             if search_operator_and:
-                search_params.searchOperator.operator = KalturaESearchOperatorType.AND_OP
+                search_params.searchOperator.operator = (
+                    KalturaESearchOperatorType.AND_OP
+                )
             else:
                 search_params.searchOperator.operator = KalturaESearchOperatorType.OR_OP
             search_params.searchOperator.searchItems = []
             # Find only entries that have captions -
             if with_captions:
                 caption_item = KalturaESearchCaptionItem()
                 caption_item.fieldName = KalturaESearchCaptionFieldName.CONTENT
                 caption_item.itemType = KalturaESearchItemType.EXISTS
                 search_params.searchOperator.searchItems.append(caption_item)
-            # Find only entries that are inside these category IDs - 
+            # Find only entries that are inside these category IDs -
             if category_ids is not None:
                 category_item = KalturaESearchCategoryEntryItem()
                 category_item.categoryEntryStatus = KalturaCategoryEntryStatus.ACTIVE
                 category_item.fieldName = KalturaESearchCategoryEntryFieldName.FULL_IDS
                 category_item.addHighlight = False
                 category_item.itemType = KalturaESearchItemType.EXACT_MATCH
                 category_item.searchTerm = category_ids
                 search_params.searchOperator.searchItems.append(category_item)
             # Find only entries that has this freeText found in them -
             if free_text is not None:
                 unified_item = KalturaESearchUnifiedItem()
                 unified_item.searchTerm = free_text
                 unified_item.itemType = KalturaESearchItemType.PARTIAL
                 search_params.searchOperator.searchItems.append(unified_item)
-        
+
         return self._load_from_search_params(search_params, with_captions, max_entries)
```

### Comparing `llama_hub-0.0.4/llama_hub/kibela/README.md` & `llama_hub-0.0.5/llama_hub/kibela/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/kibela/base.py` & `llama_hub-0.0.5/llama_hub/kibela/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,16 +48,15 @@
         """Initialize with parameters."""
         from gql.transport.aiohttp import AIOHTTPTransport
         from gql import Client
 
         self.url = f"https://{team}.kibe.la/api/v1"
         self.headers = {"Authorization": f"Bearer {token}"}
         transport = AIOHTTPTransport(url=self.url, headers=self.headers)
-        self.client = Client(transport=transport,
-                             fetch_schema_from_transport=True)
+        self.client = Client(transport=transport, fetch_schema_from_transport=True)
 
     def request(self, query: str, params: dict) -> Dict:
         from gql import gql
 
         q = gql(query)
         return self.client.execute(q, variable_values=params)
 
@@ -85,23 +84,22 @@
                 title
                 content
               }
             }
           }
         }
         """
-        after = ""
-        params = {"after": after}
+        params = {"after": ""}
         has_next = True
         documents = []
         # Due to the request limit of 10 requests per second on the Kibela API, we do not process in parallel.
         # See https://github.com/kibela/kibela-api-v1-document#1%E7%A7%92%E3%81%82%E3%81%9F%E3%82%8A%E3%81%AE%E3%83%AA%E3%82%AF%E3%82%A8%E3%82%B9%E3%83%88%E6%95%B0
         while has_next:
             res = self.request(query, params)
             note_conn = parse_obj_as(Connection[Note], res["notes"])
             for note in note_conn.edges:
                 doc = f"---\nurl: {note.node.url}\ntitle: {note.node.title}\n---\ncontent:\n{note.node.content}\n"
-                documents.append(Document(doc))
+                documents.append(Document(text=doc))
             has_next = note_conn.pageInfo.hasNextPage
-            after = note_conn.pageInfo.endCursor
+            params = {"after": note_conn.pageInfo.endCursor}
 
         return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/library.json` & `llama_hub-0.0.5/llama_hub/library.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9821428571428571%*

 * *Differences: {"'GitHubRepositoryIssuesReader'": "OrderedDict([('id', 'github_repo_issues'), ('author', "*

 * *                                   "'moncho'), ('keywords', ['github', 'repository', 'issues']), "*

 * *                                   "('extra_files', ['github_client.py', '__init__.py'])])",*

 * * "'SitemapReader'": "OrderedDict([('id', 'web/sitemap'), ('author', 'selamanse'), ('keywords', "*

 * *                    "['sitemap', 'website', 'seo'])])"}*

```diff
@@ -180,14 +180,27 @@
             "flattened"
         ]
     },
     "GPTRepoReader": {
         "author": "mpoon",
         "id": "gpt_repo"
     },
+    "GitHubRepositoryIssuesReader": {
+        "author": "moncho",
+        "extra_files": [
+            "github_client.py",
+            "__init__.py"
+        ],
+        "id": "github_repo_issues",
+        "keywords": [
+            "github",
+            "repository",
+            "issues"
+        ]
+    },
     "GithubRepositoryReader": {
         "author": "ahmetkca",
         "extra_files": [
             "github_client.py",
             "utils.py",
             "__init__.py"
         ],
@@ -609,14 +622,23 @@
         "author": "jerryjliu",
         "id": "mongo"
     },
     "SimpleWebPageReader": {
         "author": "thejessezhang",
         "id": "web/simple_web"
     },
+    "SitemapReader": {
+        "author": "selamanse",
+        "id": "web/sitemap",
+        "keywords": [
+            "sitemap",
+            "website",
+            "seo"
+        ]
+    },
     "SlackReader": {
         "author": "jerryjliu",
         "id": "slack"
     },
     "SnscrapeTwitterReader": {
         "author": "smyja",
         "id": "snscrape_twitter"
```

### Comparing `llama_hub-0.0.4/llama_hub/make_com/README.md` & `llama_hub-0.0.5/llama_hub/make_com/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/make_com/base.py` & `llama_hub-0.0.5/llama_hub/make_com/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from typing import Any, List, Optional
 
 import requests
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 from llama_index.response.schema import Response
-from llama_index.data_structs.node import Node, NodeWithScore
+from llama_index.schema import TextNode, NodeWithScore
 
 
 class MakeWrapper(BaseReader):
     """Make reader."""
 
     def load_data(self, *args: Any, **load_kwargs: Any) -> List[Document]:
         """Load data from the input directory.
@@ -47,15 +47,15 @@
 
 
 if __name__ == "__main__":
     wrapper = MakeWrapper()
     test_response = Response(
         response="test response",
         source_nodes=[
-            NodeWithScore(node=Node(source_text="test source", doc_id="test id"))
+            NodeWithScore(node=TextNode(text="test source", id_="test id"))
         ],
     )
     wrapper.pass_response_to_webhook(
         "https://hook.us1.make.com/asdfadsfasdfasdfd",
         test_response,
         "Test query",
     )
```

### Comparing `llama_hub-0.0.4/llama_hub/mangoapps_guides/README.md` & `llama_hub-0.0.5/llama_hub/mangoapps_guides/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/mangoapps_guides/base.py` & `llama_hub-0.0.5/llama_hub/mangoapps_guides/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,28 +26,30 @@
         import requests
         from bs4 import BeautifulSoup
 
         self.domain_url = domain_url
         self.limit = limit
         self.start_url = f"{self.domain_url}/home/"
 
-        fetched_urls = self.crawl_urls()[:self.limit]
+        fetched_urls = self.crawl_urls()[: self.limit]
 
         results = []
 
         guides_pages = {}
         for url in fetched_urls:
             try:
                 response = requests.get(url)
-                soup = BeautifulSoup(response.content, 'html.parser')
+                soup = BeautifulSoup(response.content, "html.parser")
 
-                page_title = soup.find('title').text
+                page_title = soup.find("title").text
 
                 # Remove the div with aria-label="Table of contents"
-                table_of_contents_div = soup.find("div", {"aria-label": "Table of contents"})
+                table_of_contents_div = soup.find(
+                    "div", {"aria-label": "Table of contents"}
+                )
                 if table_of_contents_div:
                     table_of_contents_div.decompose()
 
                 # Remove header and footer
                 header = soup.find("header")
                 if header:
                     header.decompose()
@@ -61,54 +63,53 @@
 
                 # Remove empty elements from the main content
                 for element in soup.find_all():
                     if element.get_text(strip=True) == "":
                         element.decompose()
 
                 # Find the main element containing the desired content
-                main_element = soup.find("main")  # Replace "main" with the appropriate element tag or CSS class
+                main_element = soup.find(
+                    "main"
+                )  # Replace "main" with the appropriate element tag or CSS class
 
                 # Extract the text content from the main element
                 if main_element:
                     text_content = main_element.get_text("\n")
                     # Remove multiple consecutive newlines and keep only one newline
-                    text_content = re.sub(r'\n+', '\n', text_content)
+                    text_content = re.sub(r"\n+", "\n", text_content)
                 else:
                     text_content = ""
 
                 page_text = text_content
 
                 guides_page = {}
-                guides_page['title'] =page_title
+                guides_page["title"] = page_title
                 guides_page["text"] = page_text
                 guides_pages[url] = guides_page
             except Exception as e:
                 print(f"Failed for {url} => {e}")
 
         for k, v in guides_pages.items():
-            extra_info = {
-                "url": k,
-                "title": v["title"]
-            }
+            extra_info = {"url": k, "title": v["title"]}
             results.append(
                 Document(
-                    v["text"],
+                    text=v["text"],
                     extra_info=extra_info,
                 )
             )
 
         return results
 
     def crawl_urls(self) -> List[str]:
         """Crawls all the urls from given domain"""
 
         self.visited = []
 
         fetched_urls = self.fetch_url(self.start_url)
-        fetched_urls = (list(set(fetched_urls)))
+        fetched_urls = list(set(fetched_urls))
 
         return fetched_urls
 
     def fetch_url(self, url):
         """Fetch the urls from given domain"""
 
         import requests
@@ -132,15 +133,16 @@
                 newurl not in self.visited
                 and not newurl.startswith("#")
                 and f"https://{urlparse(newurl).netloc}" == self.domain_url
                 and len(self.visited) <= self.limit
             ):
                 newurls = newurls + self.fetch_url(newurl)
 
-        newurls = (list(set(newurls)))
+        newurls = list(set(newurls))
         return newurls
 
+
 if __name__ == "__main__":
     reader = MangoppsGuidesReader()
     print("Initialized MangoppsGuidesReader")
-    output = reader.load_data( domain_url="https://guides.mangoapps.com", limit=5 )
+    output = reader.load_data(domain_url="https://guides.mangoapps.com", limit=5)
     print(output)
```

### Comparing `llama_hub-0.0.4/llama_hub/maps/README.md` & `llama_hub-0.0.5/llama_hub/maps/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/maps/base.py` & `llama_hub-0.0.5/llama_hub/maps/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,126 +1,129 @@
 """Simple reader that reads OSMmap data from overpass API"""
 
-from typing import List,Optional,Literal
+from typing import List, Optional
 import random
 import string
 import warnings
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
-warnings.filterwarnings('ignore')
-
 
+warnings.filterwarnings("ignore")
 
 
 class OpenMap(BaseReader):
     """OpenMap Reader.
 
-    Get the map Features from the overpass api(osm) for the given location/area 
+    Get the map Features from the overpass api(osm) for the given location/area
 
 
     Args:
-        localarea(str) -  Area or location you are seaching for 
-        tag_values(str) -  filter for the give area 
+        localarea(str) -  Area or location you are seaching for
+        tag_values(str) -  filter for the give area
         search_tag(str)  - Tag that you are looking for
 
-        if you not sure about the search_tag and tag_values visit https://taginfo.openstreetmap.org/tags 
+        if you not sure about the search_tag and tag_values visit https://taginfo.openstreetmap.org/tags
 
-        remove_keys(list) - list of keys that need to be removed from the response 
+        remove_keys(list) - list of keys that need to be removed from the response
                             by default  following keys will be removed ['nodes','geometry','members']
 
     """
 
     def __init__(self) -> None:
         """Initialize with parameters."""
         super().__init__()
-    
+
     @staticmethod
-    def _get_user()->str:
+    def _get_user() -> str:
         # choose from all lowercase letter
         letters = string.ascii_lowercase
-        result_str = ''.join(random.choice(letters) for i in range(10))
+        result_str = "".join(random.choice(letters) for i in range(10))
         return result_str
-    
-    @staticmethod    
-    def _get_latlon(locarea:str,user_agent:str)->tuple:
+
+    @staticmethod
+    def _get_latlon(locarea: str, user_agent: str) -> tuple:
         try:
-            from geopy.geocoders import Nominatim 
+            from geopy.geocoders import Nominatim
         except:
-            raise ImportError('install geopy using `pip3 install geopy`')
+            raise ImportError("install geopy using `pip3 install geopy`")
 
         geolocator = Nominatim(user_agent=user_agent)
         location = geolocator.geocode(locarea)
-        return(location.latitude,location.longitude) if location else (None, None)
-    
+        return (location.latitude, location.longitude) if location else (None, None)
+
     def load_data(
-        self, 
-        localarea:str,
-        search_tag:Optional[str] = 'amenity',
-        remove_keys : Optional [List]= ['nodes','geometry','members'],
-        tag_only:Optional[bool]=True ,
-        tag_values:Optional[List]=[''],
-        local_area_buffer : Optional[int] = 2000,
+        self,
+        localarea: str,
+        search_tag: Optional[str] = "amenity",
+        remove_keys: Optional[List] = ["nodes", "geometry", "members"],
+        tag_only: Optional[bool] = True,
+        tag_values: Optional[List] = [""],
+        local_area_buffer: Optional[int] = 2000,
     ) -> List[Document]:
-        
+
         """
         This loader will bring you the all the node values from the open street maps for the given location
 
         Args:
 
-        localarea(str) -  Area or location you are seaching for 
+        localarea(str) -  Area or location you are seaching for
         search_tag(str)  - Tag that you are looking for
-        if you not sure about the search_tag and tag_values visit https://taginfo.openstreetmap.org/tags 
+        if you not sure about the search_tag and tag_values visit https://taginfo.openstreetmap.org/tags
 
-        remove_keys(list) - list of keys that need to be removed from the response 
+        remove_keys(list) - list of keys that need to be removed from the response
                             by default it those keys will be removed ['nodes','geometry','members']
 
-        tag_only(bool) - if True it  return the nodes which has tags if False returns all the nodes  
-        tag_values(str) -  filter for the give area 
+        tag_only(bool) - if True it  return the nodes which has tags if False returns all the nodes
+        tag_values(str) -  filter for the give area
         local_area_buffer(int) - range that you wish to cover (Default 2000(2km))
         """
         try:
-            from osmxtract import overpass, location 
+            from osmxtract import overpass, location
             from osmxtract.errors import OverpassBadRequest
         except:
-            raise ImportError('install osmxtract using `pip3 install osmxtract`')
-        
-        null_list=['','null','none',None]
-        extra_info={}
-        local_area=localarea
-
-        if (local_area.lower().strip() in null_list):
-            raise Exception('The Area should not be null')
-        
-        user=self._get_user()
-        lat, lon = self._get_latlon(local_area,user)
+            raise ImportError("install osmxtract using `pip3 install osmxtract`")
+
+        null_list = ["", "null", "none", None]
+        extra_info = {}
+        local_area = localarea
+
+        if local_area.lower().strip() in null_list:
+            raise Exception("The Area should not be null")
+
+        user = self._get_user()
+        lat, lon = self._get_latlon(local_area, user)
         try:
             bounds = location.from_buffer(lat, lon, buffer_size=int(local_area_buffer))
         except TypeError:
-            raise TypeError('Please give valid location name or check for spelling')
-    
-        #overpass query generation and execution
-        tag_values=[str(i).lower().strip() for i in tag_values ]
-        query = overpass.ql_query(bounds, tag=search_tag.lower(), values=tag_values,timeout=500)
+            raise TypeError("Please give valid location name or check for spelling")
 
-        extra_info['overpass_query']=query
+        # overpass query generation and execution
+        tag_values = [str(i).lower().strip() for i in tag_values]
+        query = overpass.ql_query(
+            bounds, tag=search_tag.lower(), values=tag_values, timeout=500
+        )
+
+        extra_info["overpass_query"] = query
         try:
             response = overpass.request(query)
-            
-        except OverpassBadRequest : 
-            raise TypeError(f'Error while executing the Query {query} please check the Args')
-        
-        res=response['elements']
-
-        _meta=response.copy()
-        del _meta['elements']
-        extra_info['overpass_meta']=str(_meta)
-        extra_info['lat']=lat
-        extra_info['lon']=lon
-        # filtering for only the tag values 
-        filtered=[i for i in res if 'tags' in i.keys()] if tag_only else res
+
+        except OverpassBadRequest:
+            raise TypeError(
+                f"Error while executing the Query {query} please check the Args"
+            )
+
+        res = response["elements"]
+
+        _meta = response.copy()
+        del _meta["elements"]
+        extra_info["overpass_meta"] = str(_meta)
+        extra_info["lat"] = lat
+        extra_info["lon"] = lon
+        # filtering for only the tag values
+        filtered = [i for i in res if "tags" in i.keys()] if tag_only else res
 
         for key in remove_keys:
-            extras_poped =[i.pop(key,None) for i in filtered ]
+            [i.pop(key, None) for i in filtered]
         if filtered:
-            return Document(str(filtered),extra_info=extra_info)
+            return Document(text=str(filtered), extra_info=extra_info)
         else:
-            return Document(str(res),extra_info=extra_info)
+            return Document(text=str(res), extra_info=extra_info)
```

### Comparing `llama_hub-0.0.4/llama_hub/memos/README.md` & `llama_hub-0.0.5/llama_hub/memos/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/memos/base.py` & `llama_hub-0.0.5/llama_hub/memos/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,21 +39,21 @@
 
         try:
             req = requests.get(realUrl, params)
             res = req.json()
         except:
             raise ValueError("Your Memo URL is not valid")
 
-        if not "data" in res:
+        if "data" not in res:
             raise ValueError("Invalid Memo response")
 
         memos = res["data"]
         for memo in memos:
             content = memo["content"]
             extra_info = {
                 "creator": memo["creator"],
                 "resource_list": memo["resourceList"],
                 id: memo["id"],
             }
-            documents.append(Document(content, extra_info=extra_info))
+            documents.append(Document(text=content, extra_info=extra_info))
 
         return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/metal/README.md` & `llama_hub-0.0.5/llama_hub/metal/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/metal/base.py` & `llama_hub-0.0.5/llama_hub/metal/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/milvus/README.md` & `llama_hub-0.0.5/llama_hub/milvus/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/milvus/base.py` & `llama_hub-0.0.5/llama_hub/milvus/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/mondaydotcom/README.md` & `llama_hub-0.0.5/llama_hub/mondaydotcom/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/mondaydotcom/base.py` & `llama_hub-0.0.5/llama_hub/mondaydotcom/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,62 @@
 """monday.com reader."""
 from typing import Dict, List
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
-import json
 import requests
 
+
 class MondayReader(BaseReader):
     """monday.com reader. Reads board's data by a GraphQL query.
 
     Args:
         api_key (str): monday.com API key.
     """
-    
+
     def __init__(self, api_key: str) -> None:
         """Initialize monday.com reader."""
-        
+
         self.api_key = api_key
         self.api_url = "https://api.monday.com/v2"
 
     def _parse_item_values(self, cv) -> Dict[str, str]:
         data = {}
-        data["title"]= cv["title"]
-        data["value"]= cv["text"]
+        data["title"] = cv["title"]
+        data["value"] = cv["text"]
 
         return data
 
     def _parse_data(self, item) -> Dict[str, str]:
         data = {}
         data["id"] = item["id"]
         data["name"] = item["name"]
         data["values"] = list(map(self._parse_item_values, list(item["column_values"])))
 
         return data
 
-    def _perform_request(self,board_id) -> Dict[str, str]:
-        headers = {"Authorization" : self.api_key}
+    def _perform_request(self, board_id) -> Dict[str, str]:
+        headers = {"Authorization": self.api_key}
         query = """
             query{
                 boards(ids: [%d]){
                     name,
                     items{
                         id,
                         name,
                         column_values{
                             title,
                             text
                         }
                     }
                 }
-            } """ % (board_id)
-        data = {'query' : query}
+            } """ % (
+            board_id
+        )
+        data = {"query": query}
 
         response = requests.post(url=self.api_url, json=data, headers=headers)
         return response.json()
 
     def load_data(self, board_id: int) -> List[Document]:
         """Load board data by board_id
 
@@ -62,28 +64,30 @@
             board_id (int): monday.com board id.
         Returns:
             List[Document]: List of items as documents.
             [{id, name, values: [{title, value}]}]
         """
 
         json_response = self._perform_request(board_id)
-        board_data = json_response['data']['boards'][0]
+        board_data = json_response["data"]["boards"][0]
 
-        board_name = board_data["name"]
+        board_data["name"]
         items_array = list(board_data["items"])
         parsed_items = list(map(self._parse_data, list(items_array)))
         result = []
         for item in parsed_items:
             text = f"name: {item['name']}"
             for item_value in item["values"]:
-                if item_value['value']: 
+                if item_value["value"]:
                     text += f", {item_value['title']}: {item_value['value']}"
-            result.append(Document(text, extra_info={"board_id": board_id, "item_id": item["id"]}))
+            result.append(
+                Document(
+                    text=text, extra_info={"board_id": board_id, "item_id": item["id"]}
+                )
+            )
 
         return result
 
 
 if __name__ == "__main__":
-    reader = MondayReader('api_key')
-    print(
-        reader.load_data(12345)
-    )
+    reader = MondayReader("api_key")
+    print(reader.load_data(12345))
```

### Comparing `llama_hub-0.0.4/llama_hub/mongo/README.md` & `llama_hub-0.0.5/llama_hub/mongo/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/mongo/base.py` & `llama_hub-0.0.5/llama_hub/mongo/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,9 +64,9 @@
             cursor = db[collection_name].find()
         else:
             cursor = db[collection_name].find(query_dict)
 
         for item in cursor:
             if "text" not in item:
                 raise ValueError("`text` field not found in Mongo document.")
-            documents.append(Document(item["text"]))
+            documents.append(Document(text=item["text"]))
         return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/notion/README.md` & `llama_hub-0.0.5/llama_hub/notion/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/notion/base.py` & `llama_hub-0.0.5/llama_hub/notion/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,17 @@
         result_lines = "\n".join(result_lines_arr)
         return result_lines
 
     def read_page(self, page_id: str) -> str:
         """Read a page."""
         return self._read_block(page_id)
 
-    def query_database(self, database_id: str, query_dict: Dict[str, Any] = {"page_size": 100}) -> List[str]:
+    def query_database(
+        self, database_id: str, query_dict: Dict[str, Any] = {"page_size": 100}
+    ) -> List[str]:
         """Get all the pages from a Notion database."""
         pages = []
 
         res = requests.post(
             DATABASE_URL_TMPL.format(database_id=database_id),
             headers=self.headers,
             json=query_dict,
@@ -159,19 +161,19 @@
             raise ValueError("Must specify either `page_ids` or `database_id`.")
         docs = []
         if database_id is not None:
             # get all the pages in the database
             page_ids = self.query_database(database_id)
             for page_id in page_ids:
                 page_text = self.read_page(page_id)
-                docs.append(Document(page_text, extra_info={"page_id": page_id}))
+                docs.append(Document(text=page_text, extra_info={"page_id": page_id}))
         else:
             for page_id in page_ids:
                 page_text = self.read_page(page_id)
-                docs.append(Document(page_text, extra_info={"page_id": page_id}))
+                docs.append(Document(text=page_text, extra_info={"page_id": page_id}))
 
         return docs
 
 
 if __name__ == "__main__":
     reader = NotionPageReader()
     print(reader.search("What I"))
```

### Comparing `llama_hub-0.0.4/llama_hub/obsidian/README.md` & `llama_hub-0.0.5/llama_hub/obsidian/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/obsidian/base.py` & `llama_hub-0.0.5/llama_hub/obsidian/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/opendal_reader/README.md` & `llama_hub-0.0.5/llama_hub/opendal_reader/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/opendal_reader/azblob/README.md` & `llama_hub-0.0.5/llama_hub/opendal_reader/azblob/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/opendal_reader/azblob/base.py` & `llama_hub-0.0.5/llama_hub/opendal_reader/azblob/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Azblob file and directory reader.
 
 A loader that fetches a file or iterates through a directory on Azblob or.
 
 """
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 from llama_index import download_loader
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 
 class OpendalAzblobReader(BaseReader):
@@ -53,14 +53,15 @@
         }
 
     def load_data(self) -> List[Document]:
         """Load file(s) from OpenDAL."""
 
         try:
             from llama_hub.utils import import_loader
+
             OpendalReader = import_loader("OpendalReader")
         except ImportError:
             OpendalReader = download_loader("OpendalReader")
 
         loader = OpendalReader(
             scheme="azblob",
             path=self.path,
```

### Comparing `llama_hub-0.0.4/llama_hub/opendal_reader/base.py` & `llama_hub-0.0.5/llama_hub/opendal_reader/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,41 +50,40 @@
             if not self.path.endswith("/"):
                 asyncio.run(download_file_from_opendal(self.op, temp_dir, self.path))
             else:
                 asyncio.run(download_dir_from_opendal(self.op, temp_dir, self.path))
 
             try:
                 from llama_hub.utils import import_loader
+
                 SimpleDirectoryReader = import_loader("SimpleDirectoryReader")
             except ImportError:
                 SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
             loader = SimpleDirectoryReader(temp_dir, file_extractor=self.file_extractor)
 
             return loader.load_data()
 
 
-async def download_file_from_opendal(
-    op: Any, temp_dir: str, path: str
-) -> str:
+async def download_file_from_opendal(op: Any, temp_dir: str, path: str) -> str:
     """Download file from OpenDAL."""
     import opendal
+
     op = cast(opendal.AsyncOperator, op)
 
     suffix = Path(path).suffix
     filepath = f"{temp_dir}/{next(tempfile._get_candidate_names())}{suffix}"
 
     async with op.open_reader(path) as r:
         with open(filepath, "wb") as w:
             w.write(await r.read())
 
     return filepath
 
 
-async def download_dir_from_opendal(
-    op: Any, temp_dir: str, dir: str
-) -> str:
+async def download_dir_from_opendal(op: Any, temp_dir: str, dir: str) -> str:
     """Download directory from opendal."""
 
     import opendal
+
     op = cast(opendal.AsyncOperator, op)
     async for obj in await op.scan(dir):
         await download_file_from_opendal(op, temp_dir, obj.path)
```

### Comparing `llama_hub-0.0.4/llama_hub/opendal_reader/gcs/README.md` & `llama_hub-0.0.5/llama_hub/opendal_reader/gcs/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/opendal_reader/gcs/base.py` & `llama_hub-0.0.5/llama_hub/opendal_reader/gcs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Gcs file and directory reader.
 
 A loader that fetches a file or iterates through a directory on Gcs.
 
 """
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 from llama_index import download_loader
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 
 class OpendalGcsReader(BaseReader):
@@ -50,14 +50,15 @@
         }
 
     def load_data(self) -> List[Document]:
         """Load file(s) from OpenDAL."""
 
         try:
             from llama_hub.utils import import_loader
+
             OpendalReader = import_loader("OpendalReader")
         except ImportError:
             OpendalReader = download_loader("OpendalReader")
         loader = OpendalReader(
             scheme="gcs",
             path=self.path,
             file_extractor=self.file_extractor,
```

### Comparing `llama_hub-0.0.4/llama_hub/opendal_reader/s3/README.md` & `llama_hub-0.0.5/llama_hub/opendal_reader/s3/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/opendal_reader/s3/base.py` & `llama_hub-0.0.5/llama_hub/opendal_reader/s3/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """S3 file and directory reader.
 
 A loader that fetches a file or iterates through a directory on AWS S3 or other compatible service.
 
 """
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 from llama_index import download_loader
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 
 class OpendalS3Reader(BaseReader):
@@ -55,14 +55,15 @@
         }
 
     def load_data(self) -> List[Document]:
         """Load file(s) from OpenDAL."""
 
         try:
             from llama_hub.utils import import_loader
+
             OpendalReader = import_loader("OpendalReader")
         except ImportError:
             OpendalReader = download_loader("OpendalReader")
         loader = OpendalReader(
             scheme="s3",
             path=self.path,
             file_extractor=self.file_extractor,
```

### Comparing `llama_hub-0.0.4/llama_hub/outlook_localcalendar/README.md` & `llama_hub-0.0.5/llama_hub/outlook_localcalendar/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/outlook_localcalendar/base.py` & `llama_hub-0.0.5/llama_hub/outlook_localcalendar/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,25 @@
 """
 Created on Sun Apr 16 12:03:19 2023
 
 @author: tevslin
 """
 
 
-
 import datetime
 import importlib
 import platform
 
 
 from typing import List, Optional, Union
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 
-
 # Copyright 2023 Evslin Consulting
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -41,66 +39,71 @@
     """
 
     def load_data(
         self,
         number_of_results: Optional[int] = 100,
         start_date: Optional[Union[str, datetime.date]] = None,
         end_date: Optional[Union[str, datetime.date]] = None,
-        more_attributes: Optional [ List[str]]=None
+        more_attributes: Optional[List[str]] = None,
     ) -> List[Document]:
 
         """Load data from user's local calendar.
         Args:
             number_of_results (Optional[int]): the number of events to return. Defaults to 100.
             start_date (Optional[Union[str, datetime.date]]): the start date to return events from. Defaults to today.
             end_date (Optional[Union[str, datetime.date]]): the last date (inclusive) to return events from. Defaults to 2199-01-01.
             more_attributes (Optional[ List[str]]): additional attributes to be retrieved from calendar entries. Non-existnat attributes are ignored.
-            
+
         Returns a list of documents sutitable for indexing by llam_index. Always returns Start, End, Subject, Location, and Organizer
         attributes and optionally returns additional attributes specified in the more_attributes parameter.
         """
         if platform.system().lower() != "windows":
-            return([])
-        attributes=["Start","End","Subject","Location","Organizer"] # base attrubutes to return
-        if not more_attributes is None: #if the user has specified more attributes
-            attributes+=more_attributes
+            return []
+        attributes = [
+            "Start",
+            "End",
+            "Subject",
+            "Location",
+            "Organizer",
+        ]  # base attrubutes to return
+        if more_attributes is not None:  # if the user has specified more attributes
+            attributes += more_attributes
         if start_date is None:
             start_date = datetime.date.today()
         elif isinstance(start_date, str):
             start_date = datetime.date.fromisoformat(start_date)
 
-
         # Initialize the Outlook application
-        winstuff=importlib.import_module("win32com.client")
+        winstuff = importlib.import_module("win32com.client")
         outlook = winstuff.Dispatch("Outlook.Application").GetNamespace("MAPI")
 
         # Get the Calendar folder
         calendar_folder = outlook.GetDefaultFolder(9)
 
         # Retrieve calendar items
         events = calendar_folder.Items
 
         if not events:
             return []
-        events.Sort('[Start]')  # Sort items by start time
-        numberReturned=0
+        events.Sort("[Start]")  # Sort items by start time
+        numberReturned = 0
         results = []
         for event in events:
-            converted_date = datetime.date(event.Start.year, event.Start.month, event.Start.day)
-            if converted_date>start_date: #if past start date
-                numberReturned+=1
-                eventstring=''
+            converted_date = datetime.date(
+                event.Start.year, event.Start.month, event.Start.day
+            )
+            if converted_date > start_date:  # if past start date
+                numberReturned += 1
+                eventstring = ""
                 for attribute in attributes:
-                    if hasattr(event,attribute):
-                        eventstring+=f"{attribute}: {getattr(event,attribute)}, "
-                results.append(Document(eventstring))
-            if numberReturned>=number_of_results:
+                    if hasattr(event, attribute):
+                        eventstring += f"{attribute}: {getattr(event,attribute)}, "
+                results.append(Document(text=eventstring))
+            if numberReturned >= number_of_results:
                 break
 
         return results
-        
 
-   
 
 if __name__ == "__main__":
     reader = OutlookLocalCalendarReader()
     print(reader.load_data())
```

### Comparing `llama_hub-0.0.4/llama_hub/pandas_ai/README.md` & `llama_hub-0.0.5/llama_hub/pandas_ai/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/pandas_ai/base.py` & `llama_hub-0.0.5/llama_hub/pandas_ai/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Pandas AI loader."""
 
 from pathlib import Path
-from typing import Dict, List, Optional, Any
+from typing import List, Optional, Any
 import pandas as pd
 import numpy as np
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 from llama_index.readers.download import download_loader
 from tempfile import TemporaryDirectory
@@ -63,15 +63,14 @@
     def run_pandas_ai(
         self,
         initial_df: pd.DataFrame,
         query: str,
         is_conversational_answer: bool = False,
     ) -> Any:
         """Load dataframe."""
-        import pandasai
 
         return self._pandas_ai.run(
             initial_df, prompt=query, is_conversational_answer=is_conversational_answer
         )
 
     def load_data(
         self,
@@ -93,14 +92,15 @@
                 pass
             else:
                 raise ValueError("Unexpected type for result: {}".format(type(result)))
             # if not conversational answer, use Pandas CSV Reader
 
             try:
                 from llama_hub.utils import import_loader
+
                 PandasCSVReader = import_loader("PandasCSVReader")
             except ImportError:
                 PandasCSVReader = download_loader("PandasCSVReader")
 
             reader = PandasCSVReader(
                 concat_rows=self._concat_rows,
                 col_joiner=self._col_joiner,
@@ -111,8 +111,8 @@
             with TemporaryDirectory() as tmpdir:
                 outpath = Path(tmpdir) / "out.csv"
                 with outpath.open("w") as f:
                     # TODO: add option to specify index=False
                     result.to_csv(f, index=False)
 
                 docs = reader.load_data(outpath)
-                return docs
+                return docs
```

### Comparing `llama_hub-0.0.4/llama_hub/papers/arxiv/README.md` & `llama_hub-0.0.5/llama_hub/papers/arxiv/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/papers/arxiv/base.py` & `llama_hub-0.0.5/llama_hub/papers/arxiv/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,29 +76,28 @@
         arxiv_documents = SimpleDirectoryReader(
             papers_dir, file_metadata=get_paper_metadata
         ).load_data()
         # Include extra documents containing the abstracts
         abstract_documents = []
         for paper in search_results:
             d = f"The following is a summary of the paper: {paper.title}\n\nSummary: {paper.summary}"
-            abstract_documents.append(Document(d))
+            abstract_documents.append(Document(text=d))
 
         # Delete downloaded papers
         try:
             for f in os.listdir(papers_dir):
                 os.remove(os.path.join(papers_dir, f))
                 logging.debug(f"> Deleted file: {f}")
             os.rmdir(papers_dir)
             logging.debug(f"> Deleted directory: {papers_dir}")
         except OSError:
             print("Unable to delete files or directory")
 
         return arxiv_documents + abstract_documents
-    
-    
+
     def load_papers_and_abstracts(
         self,
         search_query: str,
         papers_dir: Optional[str] = ".papers",
         max_results: Optional[int] = 10,
     ) -> Tuple[List[Document], List[Document]]:
         """Search for a topic on Arxiv, download the PDFs of the top results locally, then read them.
@@ -141,25 +140,26 @@
             logging.debug(f"> Downloading {filename}...")
 
         def get_paper_metadata(filename):
             return paper_lookup[filename]
 
         try:
             from llama_hub.utils import import_loader
+
             SimpleDirectoryReader = import_loader("SimpleDirectoryReader")
-        except ImportError: 
+        except ImportError:
             SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
         arxiv_documents = SimpleDirectoryReader(
             papers_dir, file_metadata=get_paper_metadata
         ).load_data()
         # Include extra documents containing the abstracts
         abstract_documents = []
         for paper in search_results:
             d = f"The following is a summary of the paper: {paper.title}\n\nSummary: {paper.summary}"
-            abstract_documents.append(Document(d))
+            abstract_documents.append(Document(text=d))
 
         # Delete downloaded papers
         try:
             for f in os.listdir(papers_dir):
                 os.remove(os.path.join(papers_dir, f))
                 logging.debug(f"> Deleted file: {f}")
             os.rmdir(papers_dir)
```

### Comparing `llama_hub-0.0.4/llama_hub/papers/pubmed/README.md` & `llama_hub-0.0.5/llama_hub/papers/pubmed/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/papers/pubmed/base.py` & `llama_hub-0.0.5/llama_hub/papers/pubmed/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         # Then get documents from Pubmed text, which includes abstracts
         pubmed_documents = []
         for paper in pubmed_search:
             for d in paper["documents"]:
                 text = "\n".join([p["text"] for p in d["passages"]])
                 pubmed_documents.append(
                     Document(
-                        text,
+                        text=text,
                         extra_info={
                             "Title of this paper": paper["title"],
                             "URL": paper["url"],
                             "Date published": datetime.strptime(
                                 paper["date"], "%Y%m%d"
                             ).strftime("%m/%d/%Y"),
                         },
@@ -152,15 +152,15 @@
                     pass
 
         # Then get documents from Pubmed text, which includes abstracts
         pubmed_documents = []
         for paper in pubmed_search:
             pubmed_documents.append(
                 Document(
-                    paper["text"],
+                    text=paper["text"],
                     extra_info={
                         "Title of this paper": paper["title"],
                         "Journal it was published in:": paper["journal"],
                         "URL": paper["url"],
                     },
                 )
             )
```

### Comparing `llama_hub-0.0.4/llama_hub/pinecone/README.md` & `llama_hub-0.0.5/llama_hub/pinecone/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/pinecone/base.py` & `llama_hub-0.0.5/llama_hub/pinecone/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/qdrant/README.md` & `llama_hub-0.0.5/llama_hub/qdrant/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/qdrant/base.py` & `llama_hub-0.0.5/llama_hub/qdrant/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/readwise/README.md` & `llama_hub-0.0.5/llama_hub/readwise/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/readwise/base.py` & `llama_hub-0.0.5/llama_hub/readwise/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,55 +4,58 @@
 import datetime
 from typing import List, Optional
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 
-def _get_readwise_data(api_key: str,
-                       updated_after: Optional[datetime.datetime] = None):
-  """
-  Uses Readwise's export API to export all highlights, optionally after a specified date.
-
-  See https://readwise.io/api_deets for details.
-
-  Args:
-      updated_after (datetime.datetime): The datetime to load highlights after. Useful for updating indexes over time.
-  """
-  result = []
-  next_page = None
-  while True:
-    response = requests.get(
-      url="https://readwise.io/api/v2/export/",
-      params={
-        "pageCursor": next_page,
-        "updatedAfter": updated_after.isoformat() if updated_after else None
-      },
-      headers={"Authorization": f"Token {api_key}"})
-    response.raise_for_status()
-    result.extend(response.json()["results"])
-    next_page = response.json().get("nextPageCursor")
-    if not next_page: break
-  return result
+def _get_readwise_data(api_key: str, updated_after: Optional[datetime.datetime] = None):
+    """
+    Uses Readwise's export API to export all highlights, optionally after a specified date.
+
+    See https://readwise.io/api_deets for details.
+
+    Args:
+        updated_after (datetime.datetime): The datetime to load highlights after. Useful for updating indexes over time.
+    """
+    result = []
+    next_page = None
+    while True:
+        response = requests.get(
+            url="https://readwise.io/api/v2/export/",
+            params={
+                "pageCursor": next_page,
+                "updatedAfter": updated_after.isoformat() if updated_after else None,
+            },
+            headers={"Authorization": f"Token {api_key}"},
+        )
+        response.raise_for_status()
+        result.extend(response.json()["results"])
+        next_page = response.json().get("nextPageCursor")
+        if not next_page:
+            break
+    return result
+
 
 class ReadwiseReader(BaseReader):
-  """
+    """
     Reader for Readwise highlights.
     """
 
-  def __init__(self, api_key: str):
-    self._api_key = api_key
+    def __init__(self, api_key: str):
+        self._api_key = api_key
 
-  def load_data(
-    self,
-    updated_after: Optional[datetime.datetime] = None,
-  ) -> List[Document]:
-    """
+    def load_data(
+        self,
+        updated_after: Optional[datetime.datetime] = None,
+    ) -> List[Document]:
+        """
         Load your Readwise.io highlights.
 
         Args:
             updated_after (datetime.datetime): The datetime to load highlights after. Useful for updating indexes over time.
         """
-    readwise_response = _get_readwise_data(api_key=self._api_key,
-                                           updated_after=updated_after)
-    result = [Document(json.dumps(d)) for d in readwise_response]
-    return result
+        readwise_response = _get_readwise_data(
+            api_key=self._api_key, updated_after=updated_after
+        )
+        result = [Document(text=json.dumps(d)) for d in readwise_response]
+        return result
```

### Comparing `llama_hub-0.0.4/llama_hub/reddit/README.md` & `llama_hub-0.0.5/llama_hub/reddit/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/reddit/base.py` & `llama_hub-0.0.5/llama_hub/reddit/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,14 @@
         for sr in subreddits:
             ml_subreddit = reddit.subreddit(sr)
 
             for kw in search_keys:
                 relevant_posts = ml_subreddit.search(kw, limit=post_limit)
 
                 for post in relevant_posts:
-                    posts.append(Document(post.selftext))
+                    posts.append(Document(text=post.selftext))
                     for top_level_comment in post.comments:
                         if isinstance(top_level_comment, MoreComments):
                             continue
-                        posts.append(Document(top_level_comment.body))
+                        posts.append(Document(text=top_level_comment.body))
 
         return posts
```

### Comparing `llama_hub-0.0.4/llama_hub/remote/README.md` & `llama_hub-0.0.5/llama_hub/remote/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/remote/base.py` & `llama_hub-0.0.5/llama_hub/remote/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,24 +49,25 @@
         """Parse whatever is at the URL."""
         import tempfile
         from urllib.parse import urlparse
         from urllib.request import urlopen, Request
 
         extra_info = {"Source": url}
 
-        req = Request(url, headers={'User-Agent' : "Magic Browser"})
+        req = Request(url, headers={"User-Agent": "Magic Browser"})
         result = urlopen(req)
         url_type = result.info().get_content_type()
         documents = []
         if url_type == "text/html" or url_type == "text/plain":
             text = "\n\n".join([str(el.decode("utf-8-sig")) for el in result])
-            documents = [Document(text, extra_info=extra_info)]
+            documents = [Document(text=text, extra_info=extra_info)]
         elif self._is_youtube_video(url):
             try:
                 from llama_hub.utils import import_loader
+
                 YoutubeTranscriptReader = import_loader("YoutubeTranscriptReader")
             except ImportError:
                 YoutubeTranscriptReader = download_loader("YoutubeTranscriptReader")
             youtube_reader = YoutubeTranscriptReader()
             # TODO should we have another langauge, like english / french?
             documents = youtube_reader.load_data([url])
         else:
```

### Comparing `llama_hub-0.0.4/llama_hub/remote_depth/README.md` & `llama_hub-0.0.5/llama_hub/remote_depth/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/remote_depth/base.py` & `llama_hub-0.0.5/llama_hub/remote_depth/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,38 +27,39 @@
 
     def load_data(self, url: str) -> List[Document]:
         from tqdm.auto import tqdm
 
         """Parse whatever is at the URL.""" ""
         try:
             from llama_hub.utils import import_loader
+
             RemoteReader = import_loader("RemoteReader")
         except ImportError:
             RemoteReader = download_loader("RemoteReader")
         remote_reader = RemoteReader(file_extractor=self.file_extractor)
         documents = []
         links = self.get_links(url)
         urls = {-1: [url]}  # -1 is the starting point
         links_visited = []
         for i in range(self.depth + 1):
             urls[i] = []
             new_links = []
             print(f"Reading links at depth {i}...")
             for link in tqdm(links):
-                """Checking if the link belongs the provided domain. """
-                if ((self.domain_lock and link.find(url)>-1) or (not self.domain_lock)):
+                """Checking if the link belongs the provided domain."""
+                if (self.domain_lock and link.find(url) > -1) or (not self.domain_lock):
                     print("Loading link: " + link)
                     if link in links_visited:
                         continue
                     if link:
                         urls[i].append(link)
                         new_links.extend(self.get_links(link))
                     links_visited.append(link)
                 else:
-                    print("Link ignored: " +link)
+                    print("Link ignored: " + link)
             new_links = list(set(new_links))
             links = new_links
         print(f"Found {len(urls)} links at depth {self.depth}.")
         for depth_i in urls:
             for url in urls[depth_i]:
                 try:
                     documents.extend(remote_reader.load_data(url))
```

### Comparing `llama_hub-0.0.4/llama_hub/s3/README.md` & `llama_hub-0.0.5/llama_hub/s3/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/s3/base.py` & `llama_hub-0.0.5/llama_hub/s3/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,18 +64,18 @@
 
         s3 = boto3.resource("s3")
         s3_client = boto3.client("s3")
         if self.aws_access_id:
             session = boto3.Session(
                 aws_access_key_id=self.aws_access_id,
                 aws_secret_access_key=self.aws_access_secret,
-                aws_session_token=self.aws_session_token, 
+                aws_session_token=self.aws_session_token,
             )
             s3 = session.resource("s3")
-            s3_client = session.client("s3", endpoint_url=self.s3_endpoint_url )
+            s3_client = session.client("s3", endpoint_url=self.s3_endpoint_url)
 
         with tempfile.TemporaryDirectory() as temp_dir:
             if self.key:
                 suffix = Path(self.key).suffix
                 filepath = f"{temp_dir}/{next(tempfile._get_candidate_names())}{suffix}"
                 s3_client.download_file(self.bucket, self.key, filepath)
             else:
@@ -87,13 +87,14 @@
                     filepath = (
                         f"{temp_dir}/{next(tempfile._get_candidate_names())}{suffix}"
                     )
                     s3_client.download_file(self.bucket, obj.key, filepath)
 
             try:
                 from llama_hub.utils import import_loader
+
                 SimpleDirectoryReader = import_loader("SimpleDirectoryReader")
             except ImportError:
                 SimpleDirectoryReader = download_loader("SimpleDirectoryReader")
             loader = SimpleDirectoryReader(temp_dir, file_extractor=self.file_extractor)
 
             return loader.load_data()
```

### Comparing `llama_hub-0.0.4/llama_hub/slack/README.md` & `llama_hub-0.0.5/llama_hub/slack/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/slack/base.py` & `llama_hub-0.0.5/llama_hub/slack/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,27 +123,29 @@
                     )
                 else:
                     result = self.client.conversations_history(
                         channel=channel_id,
                         cursor=next_cursor,
                         oldest=str(self.earliest_date_timestamp),
                         latest=str(self.latest_date_timestamp),
-                    )                    
+                    )
                 conversation_history = result["messages"]
                 # Print results
                 logger.info(
                     "{} messages found in {}".format(len(conversation_history), id)
                 )
-                # 'reply_count' is present if there are replies in the 
+                # 'reply_count' is present if there are replies in the
                 # conversation thread otherwise not.
                 # using it to reduce number of slack api calls.
-                result_messages.extend(self._read_message(channel_id, message["ts"]) 
-                            if 'reply_count' in message 
-                            else message['text'] 
-                            for message in conversation_history)
+                result_messages.extend(
+                    self._read_message(channel_id, message["ts"])
+                    if "reply_count" in message
+                    else message["text"]
+                    for message in conversation_history
+                )
                 if not result["has_more"]:
                     break
                 next_cursor = result["response_metadata"]["next_cursor"]
 
             except SlackApiError as e:
                 if e.response["error"] == "ratelimited":
                     logger.error(
@@ -173,15 +175,15 @@
         """
         results = []
         for channel_id in channel_ids:
             channel_content = self._read_channel(
                 channel_id, reverse_chronological=reverse_chronological
             )
             results.append(
-                Document(channel_content, extra_info={"channel": channel_id})
+                Document(text=channel_content, extra_info={"channel": channel_id})
             )
         return results
 
 
 if __name__ == "__main__":
     reader = SlackReader()
     logging.info(reader.load_data(channel_ids=["C04DC2VUY3F"]))
```

### Comparing `llama_hub-0.0.4/llama_hub/snscrape_twitter/README.md` & `llama_hub-0.0.5/llama_hub/snscrape_twitter/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/snscrape_twitter/base.py` & `llama_hub-0.0.5/llama_hub/snscrape_twitter/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 class SnscrapeTwitterReader(BaseReader):
     """SnscrapeTwitter reader. Reads data from a twitter profile.
 
     Args:
         username (str): Twitter Username.
         num_tweets (int): Number of tweets to fetch.
     """
-    
+
     def __init__(self):
         """Initialize SnscrapeTwitter reader."""
 
-  
     def load_data(self, username: str, num_tweets: int) -> List[Document]:
         """Load data from a twitter profile.
 
         Args:
-            username (str): Twitter Username. 
+            username (str): Twitter Username.
             num_tweets (int): Number of tweets to fetch.
         Returns:
             List[Document]: List of documents.
         """
         import snscrape.modules.twitter as sntwitter
+
         attributes_container = []
-        for i,tweet in enumerate(sntwitter.TwitterSearchScraper(f'from:{username}').get_items()):
-            if i>num_tweets:
+        for i, tweet in enumerate(
+            sntwitter.TwitterSearchScraper(f"from:{username}").get_items()
+        ):
+            if i > num_tweets:
                 break
             attributes_container.append(tweet.rawContent)
-        return [Document(text=attributes_container,extra_info={"username": username})]
+        return [Document(text=attributes_container, extra_info={"username": username})]
```

### Comparing `llama_hub-0.0.4/llama_hub/spotify/README.md` & `llama_hub-0.0.5/llama_hub/spotify/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/spotify/base.py` & `llama_hub-0.0.5/llama_hub/spotify/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,32 +32,32 @@
             response = sp.current_user_saved_albums()
             items = response["items"]
             for item in items:
                 album = item["album"]
                 album_name = album["name"]
                 artist_name = album["artists"][0]["name"]
                 album_string = f"Album {album_name} by Artist {artist_name}\n"
-                results.append(Document(album_string))
+                results.append(Document(text=album_string))
         elif collection == "tracks":
             response = sp.current_user_saved_tracks()
             items = response["items"]
             for item in items:
                 track = item["track"]
                 track_name = track["name"]
                 artist_name = track["artists"][0]["name"]
                 artist_string = f"Track {track_name} by Artist {artist_name}\n"
-                results.append(Document(artist_string))
+                results.append(Document(text=artist_string))
         elif collection == "playlists":
             response = sp.current_user_playlists()
             items = response["items"]
             for item in items:
                 playlist_name = item["name"]
                 owner_name = item["owner"]["display_name"]
                 playlist_string = f"Playlist {playlist_name} created by {owner_name}\n"
-                results.append(Document(playlist_string))
+                results.append(Document(text=playlist_string))
         else:
             raise ValueError(
                 "Invalid collection parameter value. Allowed values are 'albums', 'tracks', or 'playlists'."
             )
 
         return results
```

### Comparing `llama_hub-0.0.4/llama_hub/stackoverflow/README.md` & `llama_hub-0.0.5/llama_hub/stackoverflow/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/stackoverflow/base.py` & `llama_hub-0.0.5/llama_hub/stackoverflow/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,21 +27,22 @@
     owner_account_id: Optional[int] = None
     owner_reputation: Optional[int] = None
     owner_user_id: Optional[int] = None
     owner_user_type: Optional[str] = None
     owner_profile_image: Optional[str] = None
     owner_display_name: Optional[str] = None
     owner_link: Optional[str] = None
-    title:  Optional[str] = None
-    last_edit_date:  Optional[str] = None
+    title: Optional[str] = None
+    last_edit_date: Optional[str] = None
     tags: Optional[List[str]] = None
     view_count: Optional[int] = None
     article_id: Optional[int] = None
     article_type: Optional[str] = None
 
+
 def rate_limit(*, allowed_per_second: int):
     max_period = 1.0 / allowed_per_second
     last_call = [time.perf_counter()]
     lock = threading.Lock()
 
     def decorate(func):
         @wraps(func)
@@ -50,104 +51,125 @@
                 elapsed = time.perf_counter() - last_call[0]
                 hold = max_period - elapsed
                 if hold > 0:
                     time.sleep(hold)
                 result = func(*args, **kwargs)
                 last_call[0] = time.perf_counter()
             return result
+
         return limit
+
     return decorate
 
+
 @rate_limit(allowed_per_second=15)
 def rate_limited_get(url, headers):
-    '''
+    """
     https://api.stackoverflowteams.com/docs/throttle
     https://api.stackexchange.com/docs/throttle
     Every application is subject to an IP based concurrent request throttle.
     If a single IP is making more than 30 requests a second, new requests will be dropped.
     The exact ban period is subject to change, but will be on the order of 30 seconds to a few minutes typically.
     Note that exactly what response an application gets (in terms of HTTP code, text, and so on)
     is undefined when subject to this ban; we consider > 30 request/sec per IP to be very abusive and thus cut the requests off very harshly.
-    '''
+    """
     resp = requests.get(url, headers=headers)
     if resp.status_code == 429:
-        logger.warning('Rate limited, sleeping for 5 minutes')
+        logger.warning("Rate limited, sleeping for 5 minutes")
         time.sleep(300)
         return rate_limited_get(url, headers)
     return resp
 
 
 class StackoverflowReader(BaseReader):
-
-    def __init__(self, api_key: str = None, team_name: str = None, cache_dir: str = None) -> None:
-        self._api_key = api_key or os.environ.get('STACKOVERFLOW_PAT')
-        self._team_name = team_name or os.environ.get('STACKOVERFLOW_TEAM_NAME')
-        self._last_index_time = None # TODO
+    def __init__(
+        self, api_key: str = None, team_name: str = None, cache_dir: str = None
+    ) -> None:
+        self._api_key = api_key or os.environ.get("STACKOVERFLOW_PAT")
+        self._team_name = team_name or os.environ.get("STACKOVERFLOW_TEAM_NAME")
+        self._last_index_time = None  # TODO
         self._cache_dir = cache_dir
         if self._cache_dir:
             os.makedirs(self._cache_dir, exist_ok=True)
 
-    def load_data(self, page: int = 1, doc_type: str = 'posts', limit: int = 50) -> List[Document]:
+    def load_data(
+        self, page: int = 1, doc_type: str = "posts", limit: int = 50
+    ) -> List[Document]:
         data = []
         has_more = True
 
         while has_more:
             url = self.build_url(page, doc_type)
-            headers = {'X-API-Access-Token': self._api_key}
-            fp = os.path.join(self._cache_dir, f'{doc_type}_{page}.json')
+            headers = {"X-API-Access-Token": self._api_key}
+            fp = os.path.join(self._cache_dir, f"{doc_type}_{page}.json")
             response = {}
             if self._cache_dir and os.path.exists(fp) and os.path.getsize(fp) > 0:
                 try:
-                    with open(fp, 'r') as f:
+                    with open(fp, "r") as f:
                         response = f.read()
                         response = json.loads(response)
                 except Exception as e:
                     logger.error(e)
             if not response:
                 response = rate_limited_get(url, headers)
                 response.raise_for_status()
                 if self._cache_dir:
-                    with open(os.path.join(self._cache_dir, f'{doc_type}_{page}.json'), 'w') as f:
-                        f.write(response.content.decode('utf-8'))
-                    logger.info(f'Wrote {fp} to cache')
+                    with open(
+                        os.path.join(self._cache_dir, f"{doc_type}_{page}.json"), "w"
+                    ) as f:
+                        f.write(response.content.decode("utf-8"))
+                    logger.info(f"Wrote {fp} to cache")
                 response = response.json()
-            has_more = response['has_more']
-            items = response['items']
-            logger.info(f'Fetched {len(items)} {doc_type} from Stack Overflow')
+            has_more = response["has_more"]
+            items = response["items"]
+            logger.info(f"Fetched {len(items)} {doc_type} from Stack Overflow")
 
             for item_dict in items:
                 owner_fields = {}
-                if 'owner' in item_dict:
-                    owner_fields = {f"owner_{k}": v for k, v in item_dict.pop('owner').items()}
-                if 'title' not in item_dict:
-                    item_dict['title'] = item_dict['link']
+                if "owner" in item_dict:
+                    owner_fields = {
+                        f"owner_{k}": v for k, v in item_dict.pop("owner").items()
+                    }
+                if "title" not in item_dict:
+                    item_dict["title"] = item_dict["link"]
                 post = StackOverflowPost(**item_dict, **owner_fields)
                 # TODO: filter out old posts
                 # last_modified = datetime.fromtimestamp(post.last_edit_date or post.last_activity_date)
                 # if last_modified < self._last_index_time:
                 #     return data
 
-                post_document = Document(text=post.body_markdown, doc_id=post.post_id,
-                                         extra_info={"title": post.title, "author": post.owner_display_name,
-                                                     "timestamp": datetime.fromtimestamp(post.creation_date), "location": post.link,
-                                                     "url": post.link, "author_image_url": post.owner_profile_image,
-                                                     "type": post.post_type})
+                post_document = Document(
+                    text=post.body_markdown,
+                    doc_id=post.post_id,
+                    extra_info={
+                        "title": post.title,
+                        "author": post.owner_display_name,
+                        "timestamp": datetime.fromtimestamp(post.creation_date),
+                        "location": post.link,
+                        "url": post.link,
+                        "author_image_url": post.owner_profile_image,
+                        "type": post.post_type,
+                    },
+                )
                 data.append(post_document)
 
             if has_more:
                 page += 1
 
         return data
 
     def build_url(self, page: int, doc_type: str) -> str:
-        team_fragment = f'&team={self._team_name}'
+        team_fragment = f"&team={self._team_name}"
         # not sure if this filter is shared globally, or only to a particular team
-        filter_fragment = '&filter=!nOedRLbqzB'
-        page_fragment = f'&page={page}'
-        url = f'https://api.stackoverflowteams.com/2.3/{doc_type}?{team_fragment}{filter_fragment}{page_fragment}'
+        filter_fragment = "&filter=!nOedRLbqzB"
+        page_fragment = f"&page={page}"
+        url = f"https://api.stackoverflowteams.com/2.3/{doc_type}?{team_fragment}{filter_fragment}{page_fragment}"
         return url
 
 
-
 if __name__ == "__main__":
-    reader = StackoverflowReader(os.environ.get('STACKOVERFLOW_PAT'), os.environ.get('STACKOVERFLOW_TEAM_NAME'), cache_dir='./stackoverflow_cache')
-    # reader.load_data()
+    reader = StackoverflowReader(
+        os.environ.get("STACKOVERFLOW_PAT"),
+        os.environ.get("STACKOVERFLOW_TEAM_NAME"),
+        cache_dir="./stackoverflow_cache",
+    )
+    # reader.load_data()
```

### Comparing `llama_hub-0.0.4/llama_hub/steamship/README.md` & `llama_hub-0.0.5/llama_hub/steamship/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/steamship/base.py` & `llama_hub-0.0.5/llama_hub/steamship/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/string_iterable/README.md` & `llama_hub-0.0.5/llama_hub/string_iterable/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/string_iterable/base.py` & `llama_hub-0.0.5/llama_hub/string_iterable/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,10 +23,10 @@
             # response should be something like "You bought an apple."
     """
 
     def load_data(self, texts: List[str]) -> List[Document]:
         """Load the data."""
         results = []
         for text in texts:
-            results.append(Document(text))
+            results.append(Document(text=text))
 
         return results
```

### Comparing `llama_hub-0.0.4/llama_hub/trello/README.md` & `llama_hub-0.0.5/llama_hub/trello/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/trello/base.py` & `llama_hub-0.0.5/llama_hub/trello/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,20 +31,19 @@
         client = TrelloClient(api_key=self.api_key, token=self.api_token)
         board = client.get_board(board_id)
         cards = board.get_cards()
 
         documents = []
         for card in cards:
             document = Document(
-                card.name,
-                card.description,
+                doc_id=card.name,
+                text=card.description,
                 extra_info={
                     "id": card.id,
                     "url": card.url,
                     "due_date": card.due_date,
                     "labels": [label.name for label in card.labels],
-                }
+                },
             )
             documents.append(document)
 
         return documents
-
```

### Comparing `llama_hub-0.0.4/llama_hub/twitter/README.md` & `llama_hub-0.0.5/llama_hub/twitter/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/twitter/base.py` & `llama_hub-0.0.5/llama_hub/twitter/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,9 +46,9 @@
         for username in twitterhandles:
             # tweets = api.user_timeline(screen_name=user, count=self.num_tweets)
             user = client.get_user(username=username)
             tweets = client.get_users_tweets(user.data.id, max_results=self.num_tweets)
             response = " "
             for tweet in tweets.data:
                 response = response + tweet.text + "\n"
-            results.append(Document(response))
+            results.append(Document(text=response))
         return results
```

### Comparing `llama_hub-0.0.4/llama_hub/utils.py` & `llama_hub-0.0.5/llama_hub/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 LIBRARY_JSON_PATH = Path(__file__).parent / "library.json"
 
 
 def import_loader(reader_str: str) -> Type[BaseReader]:
     """Import or download loader."""
 
     # read library json file
-    json_dict = json.load(open(LIBRARY_JSON_PATH, 'r'))
+    json_dict = json.load(open(LIBRARY_JSON_PATH, "r"))
     dir_name = str(json_dict[reader_str]["id"])
 
-    fmt_dir_name = dir_name.replace('/', '.')
+    fmt_dir_name = dir_name.replace("/", ".")
     module = importlib.import_module("llama_hub." + fmt_dir_name + ".base")
     reader_cls = getattr(module, reader_str)
     return reader_cls
-
```

### Comparing `llama_hub-0.0.4/llama_hub/weather/README.md` & `llama_hub-0.0.5/llama_hub/weather/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/weather/base.py` & `llama_hub-0.0.5/llama_hub/weather/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,65 +22,71 @@
         token: str,
     ) -> None:
         """Initialize with parameters."""
         super().__init__()
         self.token = token
 
     def load_data(
-        self, 
-        places: List[str], 
+        self,
+        places: List[str],
     ) -> List[Document]:
-        
-        """Load weather data for the given locations. 
+
+        """Load weather data for the given locations.
         OWM's One Call API provides the following weather data for any geographical coordinate:
         - Current weather
         - Hourly forecast for 48 hours
         - Daily forecast for 7 days
 
         Args:
             places (List[str]) - places you want the weather data for.
         """
 
         try:
             import pyowm
         except:
-            raise ImportError('install pyowm using `pip install pyowm`')
+            raise ImportError("install pyowm using `pip install pyowm`")
 
         owm = pyowm.OWM(api_key=self.token)
         mgr = owm.weather_manager()
 
         reg = owm.city_id_registry()
 
-        
         results = []
         for place in places:
             info_dict = {}
             extra_info = {}
             list_of_locations = reg.locations_for(city_name=place)
 
             try:
                 city = list_of_locations[0]
             except:
-                raise ValueError(f"Unable to find {place}, try checking the spelling and try again")
+                raise ValueError(
+                    f"Unable to find {place}, try checking the spelling and try again"
+                )
             lat = city.lat
             lon = city.lon
-    
-            res = mgr.one_call(lat=lat,lon=lon)
-            
-            
-            extra_info['latitude'] = lat
-            extra_info['longitude'] = lon
-            extra_info['timezone'] = res.timezone
-            info_dict['location'] = place
-            info_dict['current weather'] = res.current.to_dict()
+
+            res = mgr.one_call(lat=lat, lon=lon)
+
+            extra_info["latitude"] = lat
+            extra_info["longitude"] = lon
+            extra_info["timezone"] = res.timezone
+            info_dict["location"] = place
+            info_dict["current weather"] = res.current.to_dict()
             if res.forecast_daily:
-                info_dict['daily forecast'] = [i.to_dict() for i in res.forecast_daily]
+                info_dict["daily forecast"] = [i.to_dict() for i in res.forecast_daily]
             if res.forecast_hourly:
-                info_dict['hourly forecast'] = [i.to_dict() for i in res.forecast_hourly]
+                info_dict["hourly forecast"] = [
+                    i.to_dict() for i in res.forecast_hourly
+                ]
             if res.forecast_minutely:
-                info_dict['minutely forecast'] = [i.to_dict() for i in res.forecast_minutely]
+                info_dict["minutely forecast"] = [
+                    i.to_dict() for i in res.forecast_minutely
+                ]
             if res.national_weather_alerts:
-                info_dict['national weather alerts'] = [i.to_dict() for i in res.national_weather_alerts]
-            
-            results.append(Document(text=str(info_dict),extra_info=extra_info))
+                info_dict["national weather alerts"] = [
+                    i.to_dict() for i in res.national_weather_alerts
+                ]
+
+            results.append(Document(text=str(info_dict), extra_info=extra_info))
 
-        return results
+        return results
```

### Comparing `llama_hub-0.0.4/llama_hub/weaviate/README.md` & `llama_hub-0.0.5/llama_hub/weaviate/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/weaviate/base.py` & `llama_hub-0.0.5/llama_hub/weaviate/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/web/async_web/base.py` & `llama_hub-0.0.5/llama_hub/web/async_web/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,10 +71,10 @@
             if isinstance(response, Exception):
                 raise ValueError(f"One of the inputs is not a valid url: {urls[i]}")
             if self._html_to_text:
                 import html2text
 
                 response = html2text.html2text(response)
 
-            documents.append(Document(response))
+            documents.append(Document(text=response))
 
         return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/web/beautiful_soup_web/README.md` & `llama_hub-0.0.5/llama_hub/web/beautiful_soup_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/web/beautiful_soup_web/base.py` & `llama_hub-0.0.5/llama_hub/web/beautiful_soup_web/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,17 @@
         except IndexError:
             text = None
         if text:
             texts.append("\n".join([t for t in text.split("\n") if t]))
     return "\n".join(texts), {}
 
 
-def _readmedocs_reader(soup: Any, url: str, include_url_in_text: bool = True) -> Tuple[str, Dict[str, Any]]:
+def _readmedocs_reader(
+    soup: Any, url: str, include_url_in_text: bool = True
+) -> Tuple[str, Dict[str, Any]]:
     """Extract text from a ReadMe documentation site"""
     import requests
     from bs4 import BeautifulSoup
 
     links = soup.find_all("a")
     docs_links = [link["href"] for link in links if "/docs/" in link["href"]]
     docs_links = list(set(docs_links))
@@ -71,26 +73,31 @@
                 for child in element.descendants:
                     if child.name == "a" and child.has_attr("href"):
                         if include_url_in_text:
                             url = child.get("href")
                             if url is not None and "edit" in url:
                                 text += child.text
                             else:
-                                text += f"{child.text} (Reference url: {doc_link}{url}) "
+                                text += (
+                                    f"{child.text} (Reference url: {doc_link}{url}) "
+                                )
                     elif child.string and child.string.strip():
-                        text += child.string.strip() + " "  
-                            
+                        text += child.string.strip() + " "
+
         except IndexError:
             text = None
             logger.error(f"Could not extract text from {doc_link}")
             continue
         texts.append("\n".join([t for t in text.split("\n") if t]))
     return "\n".join(texts), {}
 
-def _gitbook_reader(soup: Any, url: str, include_url_in_text: bool = True) -> Tuple[str, Dict[str, Any]]:
+
+def _gitbook_reader(
+    soup: Any, url: str, include_url_in_text: bool = True
+) -> Tuple[str, Dict[str, Any]]:
     """Extract text from a ReadMe documentation site"""
     import requests
     from bs4 import BeautifulSoup
 
     links = soup.find_all("a")
     docs_links = [link["href"] for link in links if "/docs/" in link["href"]]
     docs_links = list(set(docs_links))
@@ -140,15 +147,18 @@
         self,
         website_extractor: Optional[Dict[str, Callable]] = None,
     ) -> None:
         """Initialize with parameters."""
         self.website_extractor = website_extractor or DEFAULT_WEBSITE_EXTRACTOR
 
     def load_data(
-        self, urls: List[str], custom_hostname: Optional[str] = None,include_url_in_text: Optional[bool] = True
+        self,
+        urls: List[str],
+        custom_hostname: Optional[str] = None,
+        include_url_in_text: Optional[bool] = True,
     ) -> List[Document]:
         """Load data from the urls.
 
         Args:
             urls (List[str]): List of URLs to scrape.
             custom_hostname (Optional[str]): Force a certain hostname in the case
                 a website is displayed under custom URLs (e.g. Substack blogs)
@@ -174,19 +184,17 @@
 
             soup = BeautifulSoup(page.content, "html.parser")
 
             data = ""
             extra_info = {"URL": url}
             if hostname in self.website_extractor:
                 data, metadata = self.website_extractor[hostname](
-                    soup=soup,
-                    url=url,
-                    include_url_in_text=include_url_in_text
+                    soup=soup, url=url, include_url_in_text=include_url_in_text
                 )
                 extra_info.update(metadata)
 
             else:
                 data = soup.getText()
 
-            documents.append(Document(data, extra_info=extra_info))
+            documents.append(Document(text=data, extra_info=extra_info))
 
         return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/web/knowledge_base/README.md` & `llama_hub-0.0.5/llama_hub/web/knowledge_base/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/web/knowledge_base/base.py` & `llama_hub-0.0.5/llama_hub/web/knowledge_base/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                     url,
                 )
                 extra_info = {
                     "title": article["title"],
                     "subtitle": article["subtitle"],
                     "url": article["url"],
                 }
-                documents.append(Document(article["body"], extra_info=extra_info))
+                documents.append(Document(text=article["body"], extra_info=extra_info))
 
             browser.close()
 
             return documents
 
     def scrape_article(
         self,
```

### Comparing `llama_hub-0.0.4/llama_hub/web/readability_web/README.md` & `llama_hub-0.0.5/llama_hub/web/readability_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/web/readability_web/Readability.js` & `llama_hub-0.0.5/llama_hub/web/readability_web/Readability.js`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/web/readability_web/base.py` & `llama_hub-0.0.5/llama_hub/web/readability_web/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 from llama_index.langchain_helpers.text_splitter import TextSplitter
 
 import unicodedata
 
 from pathlib import Path
+
 path = Path(__file__).parent / "Readability.js"
 
 readabilityjs = ""
 with open(path, "r") as f:
     readabilityjs = f.read()
 
 inject_readability = f"""
@@ -19,16 +20,18 @@
       function executor() {{
         return new Readability({{}}, document).parse();
       }}
       return executor();
     }}())
 """
 
+
 def nfkc_normalize(text: str) -> str:
-    return unicodedata.normalize('NFKC', text)
+    return unicodedata.normalize("NFKC", text)
+
 
 class ReadabilityWebPageReader(BaseReader):
     """Readability Webpage Loader
 
     Extracting relevant information from a fully rendered web page.
     During the processing, it is always assumed that web pages used as data sources contain textual content.
 
@@ -38,19 +41,22 @@
     Args:
         proxy (Optional[str], optional): Proxy server. Defaults to None.
         wait_until (Optional[Literal["commit", "domcontentloaded", "load", "networkidle"]], optional): Wait until the page is loaded. Defaults to "domcontentloaded".
         text_splitter (TextSplitter, optional): Text splitter. Defaults to None.
         normalizer (Optional[Callable[[str], str]], optional): Text normalizer. Defaults to nfkc_normalize.
     """
 
-    def __init__(self, proxy: Optional[str] = None, wait_until: Optional[
+    def __init__(
+        self,
+        proxy: Optional[str] = None,
+        wait_until: Optional[
             Literal["commit", "domcontentloaded", "load", "networkidle"]
-        ] = "domcontentloaded", 
+        ] = "domcontentloaded",
         text_splitter: Optional[TextSplitter] = None,
-        normalize: Optional[Callable[[str], str]] = nfkc_normalize
+        normalize: Optional[Callable[[str], str]] = nfkc_normalize,
     ) -> None:
         self._launch_options = {
             "headless": True,
         }
         self._wait_until = wait_until
         if proxy:
             self._launch_options["proxy"] = {
@@ -74,35 +80,38 @@
         with sync_playwright() as p:
             browser = p.chromium.launch(**self._launch_options)
 
             article = self.scrape_page(
                 browser,
                 url,
             )
-            extra_info = {key: article[key] for key in [
-                "title",
-                "length",
-                "excerpt",
-                "byline",
-                "dir",
-                "lang",
-                "siteName",
-            ]}
+            extra_info = {
+                key: article[key]
+                for key in [
+                    "title",
+                    "length",
+                    "excerpt",
+                    "byline",
+                    "dir",
+                    "lang",
+                    "siteName",
+                ]
+            }
 
             if self._normalize is not None:
                 article["textContent"] = self._normalize(article["textContent"])
             texts = []
             if self._text_splitter is not None:
                 texts = self._text_splitter.split_text(article["textContent"])
             else:
                 texts = [article["textContent"]]
-                
+
             browser.close()
 
-            return [Document(x, extra_info=extra_info) for x in texts]
+            return [Document(text=x, extra_info=extra_info) for x in texts]
 
     def scrape_page(
         self,
         browser: Any,
         url: str,
     ) -> Dict[str, str]:
         """Scrape a single article url.
@@ -121,14 +130,15 @@
             byline: author metadata;
             dir: content direction;
             siteName: name of the site.
             lang: content language
 
         """
         from playwright.sync_api._generated import Browser
+
         browser = cast(Browser, browser)
         page = browser.new_page(ignore_https_errors=True)
         page.set_default_timeout(60000)
         page.goto(url, wait_until=self._wait_until)
 
         r = page.evaluate(inject_readability)
```

### Comparing `llama_hub-0.0.4/llama_hub/web/rss/base.py` & `llama_hub-0.0.5/llama_hub/web/rss/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,10 +64,10 @@
 
                 if self._html_to_text:
                     import html2text
 
                     data = html2text.html2text(data)
 
                 extra_info = {"title": entry.title, "link": entry.link}
-                documents.append(Document(data, extra_info=extra_info))
+                documents.append(Document(text=data, extra_info=extra_info))
 
         return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/web/simple_web/README.md` & `llama_hub-0.0.5/llama_hub/web/simple_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/web/simple_web/base.py` & `llama_hub-0.0.5/llama_hub/web/simple_web/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,10 +38,10 @@
         for url in urls:
             response = requests.get(url)
             if self._html_to_text:
                 import html2text
 
                 response = html2text.html2text(response)
 
-            documents.append(Document(response))
+            documents.append(Document(text=response))
 
         return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/web/trafilatura_web/README.md` & `llama_hub-0.0.5/llama_hub/web/trafilatura_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/web/trafilatura_web/base.py` & `llama_hub-0.0.5/llama_hub/web/trafilatura_web/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,10 +26,10 @@
 
         if not isinstance(urls, list):
             raise ValueError("urls must be a list of strings.")
         documents = []
         for url in urls:
             downloaded = trafilatura.fetch_url(url)
             response = trafilatura.extract(downloaded)
-            documents.append(Document(response))
+            documents.append(Document(text=response))
 
         return documents
```

### Comparing `llama_hub-0.0.4/llama_hub/web/unstructured_web/README.md` & `llama_hub-0.0.5/llama_hub/web/unstructured_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/web/unstructured_web/base.py` & `llama_hub-0.0.5/llama_hub/web/unstructured_web/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,14 @@
             try:
                 if self.__is_headers_available():
                     elements = partition_html(url=url, headers=self.headers)
                 else:
                     elements = partition_html(url=url)
                 text = "\n\n".join([str(el) for el in elements])
                 metadata = {"source": url}
-                docs.append(Document(text, extra_info=metadata))
+                docs.append(Document(text=text, extra_info=metadata))
             except Exception as e:
                 if self.continue_on_failure:
                     logger.error(f"Error fetching or processing {url}, exeption: {e}")
                 else:
                     raise e
         return docs
```

### Comparing `llama_hub-0.0.4/llama_hub/whatsapp/README.md` & `llama_hub-0.0.5/llama_hub/whatsapp/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/whatsapp/base.py` & `llama_hub-0.0.5/llama_hub/whatsapp/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         self.file_path = path
 
     def load_data(self) -> List[Document]:
         """
         Parse Whatsapp file into Documents
         """
 
-        import pandas as pd
         from chatminer.chatparsers import WhatsAppParser
 
         path = Path(self.file_path)
 
         parser = WhatsAppParser(path)
         parser.parse_file()
         df = parser.parsed_messages.get_df()
@@ -44,15 +43,20 @@
                 "source": str(path).split("/")[-1].replace(".txt", ""),
                 "author": row.author,
                 "timestamp": str(row.timestamp),
             }
 
             docs.append(
                 Document(
-                    str(row.timestamp) + " " + row.author + ":" + " " + row.message,
+                    text=str(row.timestamp)
+                    + " "
+                    + row.author
+                    + ":"
+                    + " "
+                    + row.message,
                     extra_info=extra_info,
                 )
             )
 
             n += 1
             logging.debug(f"Added {n} of {len(df)} messages.")
```

### Comparing `llama_hub-0.0.4/llama_hub/wikipedia/README.md` & `llama_hub-0.0.5/llama_hub/wikipedia/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/wikipedia/base.py` & `llama_hub-0.0.5/llama_hub/wikipedia/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,22 +8,24 @@
 class WikipediaReader(BaseReader):
     """Wikipedia reader.
 
     Reads a page.
 
     """
 
-    def load_data(self, pages: List[str], lang: str = "en", **load_kwargs: Any) -> List[Document]:
+    def load_data(
+        self, pages: List[str], lang: str = "en", **load_kwargs: Any
+    ) -> List[Document]:
         """Load data from the input directory.
 
         Args:
             pages (List[str]): List of pages to read.
             lang  (str): language of wikipedia texts (default English)
         """
         import wikipedia
 
         results = []
         for page in pages:
             wikipedia.set_lang(lang)
             page_content = wikipedia.page(page, **load_kwargs).content
-            results.append(Document(page_content))
+            results.append(Document(text=page_content))
         return results
```

### Comparing `llama_hub-0.0.4/llama_hub/wordpress/README.md` & `llama_hub-0.0.5/llama_hub/wordpress/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/wordpress/base.py` & `llama_hub-0.0.5/llama_hub/wordpress/base.py`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/youtube_transcript/README.md` & `llama_hub-0.0.5/llama_hub/youtube_transcript/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/youtube_transcript/base.py` & `llama_hub-0.0.5/llama_hub/youtube_transcript/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,19 @@
 
 class YoutubeTranscriptReader(BaseReader):
     """Youtube Transcript reader."""
 
     @staticmethod
     def _extract_video_id(yt_link) -> Optional[str]:
         # regular expressions to match the different syntax of YouTube links
-        patterns = [r'^https?://(?:www\.)?youtube\.com/watch\?v=([\w-]+)',
-                    r'^https?://(?:www\.)?youtube\.com/embed/([\w-]+)',
-                    r'^https?://youtu\.be/([\w-]+)',]  # youtu.be does not use www
+        patterns = [
+            r"^https?://(?:www\.)?youtube\.com/watch\?v=([\w-]+)",
+            r"^https?://(?:www\.)?youtube\.com/embed/([\w-]+)",
+            r"^https?://youtu\.be/([\w-]+)",
+        ]  # youtu.be does not use www
 
         for pattern in patterns:
             match = re.search(pattern, yt_link)
             if match:
                 return match.group(1)
 
         # return None if no match is found
@@ -38,14 +40,13 @@
 
         """
         from youtube_transcript_api import YouTubeTranscriptApi
 
         results = []
         for link in ytlinks:
             video_id = self._extract_video_id(link)
-            srt = YouTubeTranscriptApi.get_transcript(
-                video_id, languages=languages)
+            srt = YouTubeTranscriptApi.get_transcript(video_id, languages=languages)
             transcript = ""
             for chunk in srt:
                 transcript = transcript + chunk["text"] + "\n"
-            results.append(Document(transcript))
+            results.append(Document(text=transcript))
         return results
```

### Comparing `llama_hub-0.0.4/llama_hub/zendesk/README.md` & `llama_hub-0.0.5/llama_hub/zendesk/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/zendesk/base.py` & `llama_hub-0.0.5/llama_hub/intercom/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,56 @@
-"""Zendesk reader."""
-import json
+"""Intercom reader."""
 from typing import List
-
+import json
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 
-class ZendeskReader(BaseReader):
-    """Zendesk reader. Reads data from a Zendesk workspace.
+class IntercomReader(BaseReader):
+    """Intercom reader. Reads data from a Intercom workspace.
 
     Args:
-        zendesk_subdomain (str): Zendesk subdomain
-        locale (str): Locale of articles
+        personal_access_token (str): Intercom token.
     """
 
-    def __init__(self, zendesk_subdomain: str, locale: str = "en-us") -> None:
-        """Initialize Zendesk reader."""
-        self.zendesk_subdomain = zendesk_subdomain
-        self.locale = locale
+    def __init__(self, intercom_access_token: str) -> None:
+        """Initialize Intercom reader."""
+
+        self.intercom_access_token = intercom_access_token
 
     def load_data(self) -> List[Document]:
         """Load data from the workspace.
 
         Args:
             workspace_id (str): Workspace ID.
         Returns:
             List[Document]: List of documents.
         """
         from bs4 import BeautifulSoup
 
         results = []
 
         articles = self.get_all_articles()
+
         for article in articles:
+
             body = article["body"]
             soup = BeautifulSoup(body, "html.parser")
             body = soup.get_text()
+
             extra_info = {
                 "id": article["id"],
                 "title": article["title"],
-                "url": article["html_url"],
+                "url": article["url"],
                 "updated_at": article["updated_at"],
             }
 
             results.append(
                 Document(
-                    body,
+                    text=body,
                     extra_info=extra_info,
                 )
             )
 
         return results
 
     def get_all_articles(self):
@@ -66,20 +67,26 @@
 
         return articles
 
     def get_articles_page(self, next_page: str = None):
         import requests
 
         if next_page is None:
-            url = f"https://{self.zendesk_subdomain}.zendesk.com/api/v2/help_center/{self.locale}/articles?per_page=100"
+            url = "https://api.intercom.io/articles"
         else:
             url = next_page
 
-        response = requests.get(url)
+        headers = {
+            "accept": "application/json",
+            "Intercom-Version": "2.8",
+            "authorization": f"Bearer {self.intercom_access_token}",
+        }
+
+        response = requests.get(url, headers=headers)
 
         response_json = json.loads(response.text)
 
-        next_page = response_json.get("next_page", None)
+        next_page = response_json.get("pages", {}).get("next", None)
 
-        articles = response_json.get("articles", [])
+        articles = response_json.get("data", [])
 
         return {"articles": articles, "next_page": next_page}
```

### Comparing `llama_hub-0.0.4/llama_hub/zulip/README.md` & `llama_hub-0.0.5/llama_hub/zulip/README.md`

 * *Files identical despite different names*

### Comparing `llama_hub-0.0.4/llama_hub/zulip/base.py` & `llama_hub-0.0.5/llama_hub/zulip/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,35 +3,38 @@
 from datetime import datetime
 import os
 from llama_index.readers.base import BaseReader
 from llama_index.readers.schema.base import Document
 
 logger = logging.getLogger(__name__)
 
+
 class ZulipReader(BaseReader):
     """Zulip reader."""
 
     def __init__(
-            self,
-            zulip_email: str,
-            zulip_domain: str,
-            earliest_date: Optional[datetime] = None,
-            latest_date: Optional[datetime] = None,
-        ) -> None:
-            import zulip
-
-            """Initialize with parameters."""
-            # Read the Zulip token from the environment variable
-            zulip_token = os.environ.get("ZULIP_TOKEN")
-
-            if zulip_token is None:
-                raise ValueError("ZULIP_TOKEN environment variable not set.")
-
-            # Initialize Zulip client with provided parameters
-            self.client = zulip.Client(api_key=zulip_token, email=zulip_email, site=zulip_domain)
+        self,
+        zulip_email: str,
+        zulip_domain: str,
+        earliest_date: Optional[datetime] = None,
+        latest_date: Optional[datetime] = None,
+    ) -> None:
+        import zulip
+
+        """Initialize with parameters."""
+        # Read the Zulip token from the environment variable
+        zulip_token = os.environ.get("ZULIP_TOKEN")
+
+        if zulip_token is None:
+            raise ValueError("ZULIP_TOKEN environment variable not set.")
+
+        # Initialize Zulip client with provided parameters
+        self.client = zulip.Client(
+            api_key=zulip_token, email=zulip_email, site=zulip_domain
+        )
 
     def _read_stream(self, stream_name: str, reverse_chronological: bool) -> str:
         """Read a stream."""
         params = {
             "narrow": [{"operator": "stream", "operand": stream_name}],
             "anchor": "newest",
             "num_before": 100,
@@ -47,21 +50,27 @@
         self, streams: List[str], reverse_chronological: bool = True
     ) -> List[Document]:
         """Load data from the input streams."""
         # Load data logic here
         data = []
         for stream_name in streams:
             stream_content = self._read_stream(stream_name, reverse_chronological)
-            data.append(Document(stream_content, extra_info={"stream": stream_name}))
+            data.append(
+                Document(text=stream_content, extra_info={"stream": stream_name})
+            )
         return data
 
     def get_all_streams(self) -> list:
         # Fetch all streams
         response = self.client.get_streams()
         streams_data = response["streams"]
         # Collect the stream IDs
-        stream_names = [stream['name'] for stream in streams_data]
+        stream_names = [stream["name"] for stream in streams_data]
         return stream_names
 
+
 if __name__ == "__main__":
-    reader = ZulipReader(zulip_email="ianita-bot@plurigrid.zulipchat.com", zulip_domain="plurigrid.zulipchat.com")
+    reader = ZulipReader(
+        zulip_email="ianita-bot@plurigrid.zulipchat.com",
+        zulip_domain="plurigrid.zulipchat.com",
+    )
     logging.info(reader.load_data(reader.get_all_streams()))
```

### Comparing `llama_hub-0.0.4/pyproject.toml` & `llama_hub-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "llama-hub"
-version = "0.0.4"
+version = "0.0.5"
 description = "A library of community-driven data loaders for LLMs. Use with LlamaIndex and/or LangChain. "
 authors = ["Jerry Liu", "Jesse Zhang"]
 # New attributes
 license = "MIT"
 readme = "README.md"
 homepage = "https://llamahub.ai"
 repository = "https://github.com/emptycrown/llama-hub"
@@ -16,14 +16,15 @@
 [tool.poetry.dependencies]
 # Updated Python version
 python = ">=3.8.1,<4.0"
 llama-index = ">=0.6.9"
 atlassian-python-api = "*"
 html2text = "*"
 psutil = "*"
+retrying = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.2.1"
 pytest-dotenv = "0.5.2"
 typing-inspect = "0.8.0"
 typing_extensions = "4.5.0"
 types-requests = "2.28.11.8"
```

### Comparing `llama_hub-0.0.4/PKG-INFO` & `llama_hub-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-hub
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library of community-driven data loaders for LLMs. Use with LlamaIndex and/or LangChain. 
 Home-page: https://llamahub.ai
 License: MIT
 Keywords: llama-index,llama-hub,llama
 Author: Jerry Liu
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: atlassian-python-api
 Requires-Dist: html2text
 Requires-Dist: llama-index (>=0.6.9)
 Requires-Dist: psutil
+Requires-Dist: retrying
 Project-URL: Repository, https://github.com/emptycrown/llama-hub
 Description-Content-Type: text/markdown
 
 # LlamaHub 🦙
 
 This is a simple library of all the data loaders / readers that have been created by the community. The goal is to make it extremely easy to connect large language models to a large variety of knowledge sources. These are general-purpose utilities that are meant to be used in [LlamaIndex](https://github.com/jerryjliu/llama_index) (e.g. when building a index) and [LangChain](https://github.com/hwchase17/langchain) (e.g. when building different tools an agent can use). For example, there are loaders to parse Google Docs, SQL Databases, PDF files, PowerPoints, Notion, Slack, Obsidian, and many more. Note that because different loaders produce the same types of Documents, you can easily use them together in the same index.
 
@@ -154,14 +155,18 @@
 python3.9 -m venv .venv
 source .venv/bin/activate 
 pip3 install -r test_requirements.txt
 
 poetry run pytest tests 
 ```
 
+## Changelog
+
+If you want to track the latest version updates / see which loaders are added to each release, take a look at our [full changelog here](https://github.com/emptycrown/llama-hub/blob/main/CHANGELOG.md)! 
+
 ## FAQ
 
 ### How do I test my loader before it's merged?
 
 There is an argument called `loader_hub_url` in [`download_loader`](https://github.com/jerryjliu/llama_index/blob/main/llama_index/readers/download.py) that defaults to the main branch of this repo. You can set it to your branch or fork to test your new loader.
 
 ### Should I create a PR against LlamaHub or the LlamaIndex repo directly?
```

