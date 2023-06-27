# Comparing `tmp/langflow-0.2.3.tar.gz` & `tmp/langflow-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-0.2.3.tar", max compression
+gzip compressed data, was "langflow-0.2.4.tar", max compression
```

## Comparing `langflow-0.2.3.tar` & `langflow-0.2.4.tar`

### file list

```diff
@@ -1,156 +1,156 @@
--rw-r--r--   0        0        0     1065 2023-06-27 19:32:58.092799 langflow-0.2.3/LICENSE
--rw-r--r--   0        0        0    10808 2023-06-27 19:32:58.092799 langflow-0.2.3/README.md
--rw-r--r--   0        0        0     2574 2023-06-27 19:32:58.112800 langflow-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      424 2023-06-27 19:32:58.112800 langflow-0.2.3/src/backend/langflow/__init__.py
--rw-r--r--   0        0        0     8333 2023-06-27 19:32:58.112800 langflow-0.2.3/src/backend/langflow/__main__.py
--rw-r--r--   0        0        0       61 2023-06-27 19:32:58.112800 langflow-0.2.3/src/backend/langflow/api/__init__.py
--rw-r--r--   0        0        0      423 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/api/router.py
--rw-r--r--   0        0        0      736 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/api/utils.py
--rw-r--r--   0        0        0      436 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/api/v1/__init__.py
--rw-r--r--   0        0        0     2036 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/api/v1/base.py
--rw-r--r--   0        0        0     1127 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/api/v1/callback.py
--rw-r--r--   0        0        0     4807 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/api/v1/chat.py
--rw-r--r--   0        0        0     2498 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/api/v1/endpoints.py
--rw-r--r--   0        0        0     2691 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/api/v1/flow_styles.py
--rw-r--r--   0        0        0     3868 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/api/v1/flows.py
--rw-r--r--   0        0        0     2164 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/api/v1/schemas.py
--rw-r--r--   0        0        0     1054 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/api/v1/validate.py
--rw-r--r--   0        0        0      152 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/cache/__init__.py
--rw-r--r--   0        0        0     1815 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/cache/base.py
--rw-r--r--   0        0        0     4554 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/cache/flow.py
--rw-r--r--   0        0        0     4481 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/cache/manager.py
--rw-r--r--   0        0        0     5062 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/cache/utils.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/chat/__init__.py
--rw-r--r--   0        0        0       45 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/chat/config.py
--rw-r--r--   0        0        0     8157 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/chat/manager.py
--rw-r--r--   0        0        0     1143 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/chat/utils.py
--rw-r--r--   0        0        0    10540 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/config.yaml
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/custom/__init__.py
--rw-r--r--   0        0        0     1374 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/custom/customs.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/database/__init__.py
--rw-r--r--   0        0        0      442 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/database/base.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/database/models/__init__.py
--rw-r--r--   0        0        0      363 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/database/models/base.py
--rw-r--r--   0        0        0     1705 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/database/models/flow.py
--rw-r--r--   0        0        0      831 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/database/models/flow_style.py
--rw-r--r--   0        0        0      889 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg
--rw-r--r--   0        0        0     2521 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg
--rw-r--r--   0        0        0     3513 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg
--rw-r--r--   0        0        0     1578 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg
--rw-r--r--   0        0        0     1705 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg
--rw-r--r--   0        0        0     7249 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg
--rw-r--r--   0        0        0     1106 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg
--rw-r--r--   0        0        0     2007 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg
--rw-r--r--   0        0        0     2763 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/assets/anthropic_box-60809508.svg
--rw-r--r--   0        0        0     6783 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/assets/bing-60c0c591.svg
--rw-r--r--   0        0        0      622 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/assets/chroma-65ceac37.svg
--rw-r--r--   0        0        0     1450 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/assets/cohere-f09153b9.svg
--rw-r--r--   0        0        0     1667 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg
--rw-r--r--   0        0        0    11568 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/froze-flow-494453cf.png
--rw-r--r--   0        0        0     1111 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg
--rw-r--r--   0        0        0      688 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/assets/google-0cf576a5.svg
--rw-r--r--   0        0        0    35286 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg
--rw-r--r--   0        0        0      789 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg
--rw-r--r--   0        0        0  4237102 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/index-7835bd6e.js
--rw-r--r--   0        0        0   158839 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/index-8af82052.css
--rw-r--r--   0        0        0     2212 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg
--rw-r--r--   0        0        0     1182 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/mongodb-icon-64a21d47.svg
--rw-r--r--   0        0        0     2509 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/openAI-2c85883b.svg
--rw-r--r--   0        0        0     2604 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/pinecone_logo-411e417b.svg
--rw-r--r--   0        0        0     1539 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg
--rw-r--r--   0        0        0     3248 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/supabase-icon-bdc56c95.svg
--rw-r--r--   0        0        0     4310 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
--rw-r--r--   0        0        0   104188 2023-06-27 19:33:56.212743 langflow-0.2.3/src/backend/langflow/frontend/favicon.ico
--rw-r--r--   0        0        0      622 2023-06-27 19:33:56.216743 langflow-0.2.3/src/backend/langflow/frontend/index.html
--rw-r--r--   0        0        0      720 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/graph/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/graph/edge/__init__.py
--rw-r--r--   0        0        0     1887 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/graph/edge/base.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/graph/graph/__init__.py
--rw-r--r--   0        0        0     7521 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/graph/graph/base.py
--rw-r--r--   0        0        0     1893 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/graph/graph/constants.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/graph/graph/utils.py
--rw-r--r--   0        0        0      642 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/graph/utils.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/graph/vertex/__init__.py
--rw-r--r--   0        0        0     9458 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/graph/vertex/base.py
--rw-r--r--   0        0        0        1 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/graph/vertex/constants.py
--rw-r--r--   0        0        0     6436 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/graph/vertex/types.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/__init__.py
--rw-r--r--   0        0        0       84 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/agents/__init__.py
--rw-r--r--   0        0        0     1843 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/agents/base.py
--rw-r--r--   0        0        0    10088 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/agents/custom.py
--rw-r--r--   0        0        0     1447 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/agents/prebuilt.py
--rw-r--r--   0        0        0     4632 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/base.py
--rw-r--r--   0        0        0       84 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/chains/__init__.py
--rw-r--r--   0        0        0     2827 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/chains/base.py
--rw-r--r--   0        0        0     4843 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/chains/custom.py
--rw-r--r--   0        0        0     2235 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/custom_lists.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/document_loaders/__init__.py
--rw-r--r--   0        0        0     1479 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/document_loaders/base.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/embeddings/__init__.py
--rw-r--r--   0        0        0     1445 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/embeddings/base.py
--rw-r--r--   0        0        0      171 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/importing/__init__.py
--rw-r--r--   0        0        0     5015 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/importing/utils.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/initialize/__init__.py
--rw-r--r--   0        0        0    12919 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/initialize/loading.py
--rw-r--r--   0        0        0     7704 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/initialize/vector_store.py
--rw-r--r--   0        0        0     1668 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/listing.py
--rw-r--r--   0        0        0       78 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/llms/__init__.py
--rw-r--r--   0        0        0     1355 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/llms/base.py
--rw-r--r--   0        0        0       88 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/memories/__init__.py
--rw-r--r--   0        0        0     1541 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/memories/base.py
--rw-r--r--   0        0        0       87 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/prompts/__init__.py
--rw-r--r--   0        0        0     2459 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/prompts/base.py
--rw-r--r--   0        0        0     2483 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/prompts/custom.py
--rw-r--r--   0        0        0     2122 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/run.py
--rw-r--r--   0        0        0      106 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/text_splitters/__init__.py
--rw-r--r--   0        0        0     1450 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/text_splitters/base.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/toolkits/__init__.py
--rw-r--r--   0        0        0     2598 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/toolkits/base.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/toolkits/custom.py
--rw-r--r--   0        0        0       81 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/tools/__init__.py
--rw-r--r--   0        0        0     5405 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/tools/base.py
--rw-r--r--   0        0        0      900 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/tools/constants.py
--rw-r--r--   0        0        0     1323 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/tools/custom.py
--rw-r--r--   0        0        0     4328 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/tools/util.py
--rw-r--r--   0        0        0     1813 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/types.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/utilities/__init__.py
--rw-r--r--   0        0        0     2294 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/utilities/base.py
--rw-r--r--   0        0        0     2581 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/utils.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/vector_store/__init__.py
--rw-r--r--   0        0        0     1813 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/vector_store/base.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/wrappers/__init__.py
--rw-r--r--   0        0        0     1056 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/interface/wrappers/base.py
--rw-r--r--   0        0        0       29 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/jcloud.yml
--rw-r--r--   0        0        0      362 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/lcserve.py
--rw-r--r--   0        0        0     2034 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/main.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/processing/__init__.py
--rw-r--r--   0        0        0     2206 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/processing/base.py
--rw-r--r--   0        0        0     8079 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/processing/process.py
--rw-r--r--   0        0        0      579 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/server.py
--rw-r--r--   0        0        0     2350 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/settings.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/template/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/template/field/__init__.py
--rw-r--r--   0        0        0     1190 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/template/field/base.py
--rw-r--r--   0        0        0      375 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/template/frontend_node/__init__.py
--rw-r--r--   0        0        0     6679 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/template/frontend_node/agents.py
--rw-r--r--   0        0        0     8633 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/template/frontend_node/base.py
--rw-r--r--   0        0        0     7665 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/template/frontend_node/chains.py
--rw-r--r--   0        0        0     1033 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/template/frontend_node/constants.py
--rw-r--r--   0        0        0     6148 2023-06-27 19:32:58.116800 langflow-0.2.3/src/backend/langflow/template/frontend_node/documentloaders.py
--rw-r--r--   0        0        0     1680 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/template/frontend_node/embeddings.py
--rw-r--r--   0        0        0     3088 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/template/frontend_node/llms.py
--rw-r--r--   0        0        0     2019 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/template/frontend_node/memories.py
--rw-r--r--   0        0        0     3540 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/template/frontend_node/prompts.py
--rw-r--r--   0        0        0     2128 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/template/frontend_node/textsplitters.py
--rw-r--r--   0        0        0     3983 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/template/frontend_node/tools.py
--rw-r--r--   0        0        0      823 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/template/frontend_node/utilities.py
--rw-r--r--   0        0        0     9337 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/template/frontend_node/vectorstores.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/template/template/__init__.py
--rw-r--r--   0        0        0     1181 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/template/template/base.py
--rw-r--r--   0        0        0        0 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/utils/__init__.py
--rw-r--r--   0        0        0     1758 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/utils/constants.py
--rw-r--r--   0        0        0      914 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/utils/logger.py
--rw-r--r--   0        0        0     3169 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/utils/payload.py
--rw-r--r--   0        0        0    11336 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/utils/util.py
--rw-r--r--   0        0        0     5325 2023-06-27 19:32:58.120800 langflow-0.2.3/src/backend/langflow/utils/validate.py
--rw-r--r--   0        0        0    13643 1970-01-01 00:00:00.000000 langflow-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-27 21:33:37.068634 langflow-0.2.4/LICENSE
+-rw-r--r--   0        0        0    10808 2023-06-27 21:33:37.068634 langflow-0.2.4/README.md
+-rw-r--r--   0        0        0     2574 2023-06-27 21:33:37.088633 langflow-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      424 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/__init__.py
+-rw-r--r--   0        0        0     8333 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/__main__.py
+-rw-r--r--   0        0        0       61 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/api/__init__.py
+-rw-r--r--   0        0        0      423 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/api/router.py
+-rw-r--r--   0        0        0      736 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/api/utils.py
+-rw-r--r--   0        0        0      436 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/api/v1/__init__.py
+-rw-r--r--   0        0        0     2036 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/api/v1/base.py
+-rw-r--r--   0        0        0     1127 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/api/v1/callback.py
+-rw-r--r--   0        0        0     4807 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/api/v1/chat.py
+-rw-r--r--   0        0        0     2498 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/api/v1/endpoints.py
+-rw-r--r--   0        0        0     2691 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/api/v1/flow_styles.py
+-rw-r--r--   0        0        0     3868 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/api/v1/flows.py
+-rw-r--r--   0        0        0     2164 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/api/v1/schemas.py
+-rw-r--r--   0        0        0     1054 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/api/v1/validate.py
+-rw-r--r--   0        0        0      152 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/cache/__init__.py
+-rw-r--r--   0        0        0     1815 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/cache/base.py
+-rw-r--r--   0        0        0     4554 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/cache/flow.py
+-rw-r--r--   0        0        0     4481 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/cache/manager.py
+-rw-r--r--   0        0        0     5062 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/cache/utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/chat/__init__.py
+-rw-r--r--   0        0        0       45 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/chat/config.py
+-rw-r--r--   0        0        0     8157 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/chat/manager.py
+-rw-r--r--   0        0        0     1143 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/chat/utils.py
+-rw-r--r--   0        0        0    10540 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/config.yaml
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/custom/__init__.py
+-rw-r--r--   0        0        0     1374 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/custom/customs.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/database/__init__.py
+-rw-r--r--   0        0        0      442 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/database/base.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/database/models/__init__.py
+-rw-r--r--   0        0        0      363 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/database/models/base.py
+-rw-r--r--   0        0        0     1705 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/database/models/flow.py
+-rw-r--r--   0        0        0      831 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/database/models/flow_style.py
+-rw-r--r--   0        0        0      889 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg
+-rw-r--r--   0        0        0     2521 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg
+-rw-r--r--   0        0        0     3513 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg
+-rw-r--r--   0        0        0     1578 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg
+-rw-r--r--   0        0        0     1705 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg
+-rw-r--r--   0        0        0     7249 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg
+-rw-r--r--   0        0        0     1106 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg
+-rw-r--r--   0        0        0     2007 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg
+-rw-r--r--   0        0        0     2763 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/anthropic_box-60809508.svg
+-rw-r--r--   0        0        0     6783 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/bing-60c0c591.svg
+-rw-r--r--   0        0        0      622 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/chroma-65ceac37.svg
+-rw-r--r--   0        0        0     1450 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/cohere-f09153b9.svg
+-rw-r--r--   0        0        0     1667 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg
+-rw-r--r--   0        0        0    11568 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/froze-flow-494453cf.png
+-rw-r--r--   0        0        0     1111 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg
+-rw-r--r--   0        0        0      688 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/google-0cf576a5.svg
+-rw-r--r--   0        0        0    35286 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg
+-rw-r--r--   0        0        0      789 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg
+-rw-r--r--   0        0        0  4237144 2023-06-27 21:34:43.160042 langflow-0.2.4/src/backend/langflow/frontend/assets/index-51fa86f3.js
+-rw-r--r--   0        0        0   158839 2023-06-27 21:34:43.160042 langflow-0.2.4/src/backend/langflow/frontend/assets/index-8af82052.css
+-rw-r--r--   0        0        0     2212 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg
+-rw-r--r--   0        0        0     1182 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/mongodb-icon-64a21d47.svg
+-rw-r--r--   0        0        0     2509 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/openAI-2c85883b.svg
+-rw-r--r--   0        0        0     2604 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/pinecone_logo-411e417b.svg
+-rw-r--r--   0        0        0     1539 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg
+-rw-r--r--   0        0        0     3248 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/assets/supabase-icon-bdc56c95.svg
+-rw-r--r--   0        0        0     4310 2023-06-27 21:34:43.160042 langflow-0.2.4/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js
+-rw-r--r--   0        0        0   104188 2023-06-27 21:34:43.156042 langflow-0.2.4/src/backend/langflow/frontend/favicon.ico
+-rw-r--r--   0        0        0      622 2023-06-27 21:34:43.160042 langflow-0.2.4/src/backend/langflow/frontend/index.html
+-rw-r--r--   0        0        0      720 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/graph/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/graph/edge/__init__.py
+-rw-r--r--   0        0        0     1887 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/graph/edge/base.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/graph/graph/__init__.py
+-rw-r--r--   0        0        0     7521 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/graph/graph/base.py
+-rw-r--r--   0        0        0     1893 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/graph/graph/constants.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/graph/graph/utils.py
+-rw-r--r--   0        0        0      642 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/graph/utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/graph/vertex/__init__.py
+-rw-r--r--   0        0        0     9458 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/graph/vertex/base.py
+-rw-r--r--   0        0        0        1 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/graph/vertex/constants.py
+-rw-r--r--   0        0        0     6436 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/graph/vertex/types.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/__init__.py
+-rw-r--r--   0        0        0       84 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/agents/__init__.py
+-rw-r--r--   0        0        0     1843 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/agents/base.py
+-rw-r--r--   0        0        0    10088 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/agents/custom.py
+-rw-r--r--   0        0        0     1447 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/agents/prebuilt.py
+-rw-r--r--   0        0        0     4632 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/base.py
+-rw-r--r--   0        0        0       84 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/chains/__init__.py
+-rw-r--r--   0        0        0     2827 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/chains/base.py
+-rw-r--r--   0        0        0     4843 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/chains/custom.py
+-rw-r--r--   0        0        0     2235 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/custom_lists.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/document_loaders/__init__.py
+-rw-r--r--   0        0        0     1479 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/document_loaders/base.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/embeddings/__init__.py
+-rw-r--r--   0        0        0     1445 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/embeddings/base.py
+-rw-r--r--   0        0        0      171 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/importing/__init__.py
+-rw-r--r--   0        0        0     5015 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/importing/utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/initialize/__init__.py
+-rw-r--r--   0        0        0    12919 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/initialize/loading.py
+-rw-r--r--   0        0        0     7704 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/initialize/vector_store.py
+-rw-r--r--   0        0        0     1668 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/listing.py
+-rw-r--r--   0        0        0       78 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/llms/__init__.py
+-rw-r--r--   0        0        0     1355 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/llms/base.py
+-rw-r--r--   0        0        0       88 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/memories/__init__.py
+-rw-r--r--   0        0        0     1541 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/memories/base.py
+-rw-r--r--   0        0        0       87 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/prompts/__init__.py
+-rw-r--r--   0        0        0     2459 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/prompts/base.py
+-rw-r--r--   0        0        0     2483 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/prompts/custom.py
+-rw-r--r--   0        0        0     2122 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/run.py
+-rw-r--r--   0        0        0      106 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/text_splitters/__init__.py
+-rw-r--r--   0        0        0     1450 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/text_splitters/base.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/toolkits/__init__.py
+-rw-r--r--   0        0        0     2598 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/toolkits/base.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/toolkits/custom.py
+-rw-r--r--   0        0        0       81 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/tools/__init__.py
+-rw-r--r--   0        0        0     5405 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/tools/base.py
+-rw-r--r--   0        0        0      900 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/tools/constants.py
+-rw-r--r--   0        0        0     1323 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/tools/custom.py
+-rw-r--r--   0        0        0     4328 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/tools/util.py
+-rw-r--r--   0        0        0     1813 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/types.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/utilities/__init__.py
+-rw-r--r--   0        0        0     2294 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/utilities/base.py
+-rw-r--r--   0        0        0     2581 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/vector_store/__init__.py
+-rw-r--r--   0        0        0     1813 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/vector_store/base.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/wrappers/__init__.py
+-rw-r--r--   0        0        0     1056 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/interface/wrappers/base.py
+-rw-r--r--   0        0        0       29 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/jcloud.yml
+-rw-r--r--   0        0        0      362 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/lcserve.py
+-rw-r--r--   0        0        0     2034 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/main.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/processing/__init__.py
+-rw-r--r--   0        0        0     2206 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/processing/base.py
+-rw-r--r--   0        0        0     8079 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/processing/process.py
+-rw-r--r--   0        0        0      579 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/server.py
+-rw-r--r--   0        0        0     2350 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/settings.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/template/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/template/field/__init__.py
+-rw-r--r--   0        0        0     1190 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/template/field/base.py
+-rw-r--r--   0        0        0      375 2023-06-27 21:33:37.092633 langflow-0.2.4/src/backend/langflow/template/frontend_node/__init__.py
+-rw-r--r--   0        0        0     6679 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/frontend_node/agents.py
+-rw-r--r--   0        0        0     8633 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/frontend_node/base.py
+-rw-r--r--   0        0        0     7665 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/frontend_node/chains.py
+-rw-r--r--   0        0        0     1033 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/frontend_node/constants.py
+-rw-r--r--   0        0        0     6148 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/frontend_node/documentloaders.py
+-rw-r--r--   0        0        0     1680 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/frontend_node/embeddings.py
+-rw-r--r--   0        0        0     3088 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/frontend_node/llms.py
+-rw-r--r--   0        0        0     2019 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/frontend_node/memories.py
+-rw-r--r--   0        0        0     3540 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/frontend_node/prompts.py
+-rw-r--r--   0        0        0     2128 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/frontend_node/textsplitters.py
+-rw-r--r--   0        0        0     3983 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/frontend_node/tools.py
+-rw-r--r--   0        0        0      823 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/frontend_node/utilities.py
+-rw-r--r--   0        0        0     9337 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/frontend_node/vectorstores.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/template/__init__.py
+-rw-r--r--   0        0        0     1181 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/template/template/base.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/utils/__init__.py
+-rw-r--r--   0        0        0     1758 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/utils/constants.py
+-rw-r--r--   0        0        0      914 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/utils/logger.py
+-rw-r--r--   0        0        0     3169 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/utils/payload.py
+-rw-r--r--   0        0        0    11336 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/utils/util.py
+-rw-r--r--   0        0        0     5325 2023-06-27 21:33:37.096633 langflow-0.2.4/src/backend/langflow/utils/validate.py
+-rw-r--r--   0        0        0    13643 1970-01-01 00:00:00.000000 langflow-0.2.4/PKG-INFO
```

### Comparing `langflow-0.2.3/LICENSE` & `langflow-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/README.md` & `langflow-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/pyproject.toml` & `langflow-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "0.2.3"
+version = "0.2.4"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Gustavo Schaedler <gustavopoa@gmail.com>",
     "Lucas Eduoli <lucaseduoli@gmail.com>",
```

### Comparing `langflow-0.2.3/src/backend/langflow/__main__.py` & `langflow-0.2.4/src/backend/langflow/__main__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/api/utils.py` & `langflow-0.2.4/src/backend/langflow/api/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/api/v1/base.py` & `langflow-0.2.4/src/backend/langflow/api/v1/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/api/v1/callback.py` & `langflow-0.2.4/src/backend/langflow/api/v1/callback.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/api/v1/chat.py` & `langflow-0.2.4/src/backend/langflow/api/v1/chat.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/api/v1/endpoints.py` & `langflow-0.2.4/src/backend/langflow/api/v1/endpoints.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/api/v1/flow_styles.py` & `langflow-0.2.4/src/backend/langflow/api/v1/flow_styles.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/api/v1/flows.py` & `langflow-0.2.4/src/backend/langflow/api/v1/flows.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/api/v1/schemas.py` & `langflow-0.2.4/src/backend/langflow/api/v1/schemas.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/api/v1/validate.py` & `langflow-0.2.4/src/backend/langflow/api/v1/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/cache/base.py` & `langflow-0.2.4/src/backend/langflow/cache/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/cache/flow.py` & `langflow-0.2.4/src/backend/langflow/cache/flow.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/cache/manager.py` & `langflow-0.2.4/src/backend/langflow/cache/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/cache/utils.py` & `langflow-0.2.4/src/backend/langflow/cache/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/chat/manager.py` & `langflow-0.2.4/src/backend/langflow/chat/manager.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/chat/utils.py` & `langflow-0.2.4/src/backend/langflow/chat/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/config.yaml` & `langflow-0.2.4/src/backend/langflow/config.yaml`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/custom/customs.py` & `langflow-0.2.4/src/backend/langflow/custom/customs.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/database/models/flow.py` & `langflow-0.2.4/src/backend/langflow/database/models/flow.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/database/models/flow_style.py` & `langflow-0.2.4/src/backend/langflow/database/models/flow_style.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/Facebook_Messenger_logo_2020-d4e5cbf1.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/Gooey Ring-5s-271px-aa2b9199.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/Midjourney_Emblem-3952311f.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/Notion-logo-1b52a185.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/QDrant-517d22b4.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/Searx_logo-24248044.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/Y_Combinator_logo-7356d194.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/airbyte-6aa3c5fa.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/anthropic_box-60809508.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/anthropic_box-60809508.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/bing-60c0c591.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/bing-60c0c591.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/chroma-65ceac37.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/chroma-65ceac37.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/cohere-f09153b9.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/cohere-f09153b9.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/evernote-icon-135bbfd8.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/froze-flow-494453cf.png` & `langflow-0.2.4/src/backend/langflow/frontend/assets/froze-flow-494453cf.png`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/gitbook-svgrepo-com-8beecec7.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/google-0cf576a5.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/google-0cf576a5.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/hf-logo-942cad1c.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/ifixit-seeklogo.com-6846f6e5.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/index-7835bd6e.js` & `langflow-0.2.4/src/backend/langflow/frontend/assets/index-51fa86f3.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -57167,14 +57167,16 @@
                             })
                         })
                     }), H.jsx(mo, {
                         content: e.data.node.documentation === "" ? "Coming Soon" : "Documentation",
                         side: "top",
                         children: H.jsx("a", {
                             className: Gt("hover:dark:hover:bg-[#242f47]  transition-all duration-500 ease-in-out dark:bg-gray-800 dark:text-muted-foreground shadow-md relative -ml-px inline-flex items-center bg-white px-2 py-2  ring-1 ring-inset ring-gray-300 hover:bg-muted focus:z-10" + (e.data.node.documentation === "" ? " text-muted-foreground" : " text-foreground")),
+                            target: "_blank",
+                            rel: "noopener noreferrer",
                             href: e.data.node.documentation,
                             onClick: a => {
                                 e.data.node.documentation === "" && a.preventDefault()
                             },
                             children: H.jsx(gJ, {
                                 className: "w-4 h-4 dark:text-muted-foreground"
                             })
```

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/index-8af82052.css` & `langflow-0.2.4/src/backend/langflow/frontend/assets/index-8af82052.css`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/meta-icon-fc8308c0.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/mongodb-icon-64a21d47.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/mongodb-icon-64a21d47.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/openAI-2c85883b.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/openAI-2c85883b.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/pinecone_logo-411e417b.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/pinecone_logo-411e417b.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/slack-icon-32084c4a.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/supabase-icon-bdc56c95.svg` & `langflow-0.2.4/src/backend/langflow/frontend/assets/supabase-icon-bdc56c95.svg`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js` & `langflow-0.2.4/src/backend/langflow/frontend/assets/web-vitals-60d3425a.js`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/favicon.ico` & `langflow-0.2.4/src/backend/langflow/frontend/favicon.ico`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/frontend/index.html` & `langflow-0.2.4/src/backend/langflow/frontend/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <html lang="en">
 <head>
     <meta charset="UTF-8">
     <meta http-equiv="X-UA-Compatible" content="IE=edge">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <link rel="icon" href="/favicon.ico" />
     <title>LangFlow</title>
-  <script type="module" crossorigin src="/assets/index-7835bd6e.js"></script>
+  <script type="module" crossorigin src="/assets/index-51fa86f3.js"></script>
   <link rel="stylesheet" href="/assets/index-8af82052.css">
 </head>
 <body id='body' style="width: 100%; height:100%">
     <noscript>You need to enable JavaScript to run this app.</noscript>
     <div style="width: 100vw; height:100vh" id='root'></div>
     
 </body>
```

### Comparing `langflow-0.2.3/src/backend/langflow/graph/__init__.py` & `langflow-0.2.4/src/backend/langflow/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/graph/edge/base.py` & `langflow-0.2.4/src/backend/langflow/graph/edge/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/graph/graph/base.py` & `langflow-0.2.4/src/backend/langflow/graph/graph/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/graph/graph/constants.py` & `langflow-0.2.4/src/backend/langflow/graph/graph/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/graph/utils.py` & `langflow-0.2.4/src/backend/langflow/graph/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/graph/vertex/base.py` & `langflow-0.2.4/src/backend/langflow/graph/vertex/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/graph/vertex/types.py` & `langflow-0.2.4/src/backend/langflow/graph/vertex/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/agents/base.py` & `langflow-0.2.4/src/backend/langflow/interface/agents/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/agents/custom.py` & `langflow-0.2.4/src/backend/langflow/interface/agents/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/agents/prebuilt.py` & `langflow-0.2.4/src/backend/langflow/interface/agents/prebuilt.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/base.py` & `langflow-0.2.4/src/backend/langflow/interface/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/chains/base.py` & `langflow-0.2.4/src/backend/langflow/interface/chains/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/chains/custom.py` & `langflow-0.2.4/src/backend/langflow/interface/chains/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/custom_lists.py` & `langflow-0.2.4/src/backend/langflow/interface/custom_lists.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/document_loaders/base.py` & `langflow-0.2.4/src/backend/langflow/interface/document_loaders/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/embeddings/base.py` & `langflow-0.2.4/src/backend/langflow/interface/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/importing/utils.py` & `langflow-0.2.4/src/backend/langflow/interface/importing/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/initialize/loading.py` & `langflow-0.2.4/src/backend/langflow/interface/initialize/loading.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/initialize/vector_store.py` & `langflow-0.2.4/src/backend/langflow/interface/initialize/vector_store.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/listing.py` & `langflow-0.2.4/src/backend/langflow/interface/listing.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/llms/base.py` & `langflow-0.2.4/src/backend/langflow/interface/llms/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/memories/base.py` & `langflow-0.2.4/src/backend/langflow/interface/memories/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/prompts/base.py` & `langflow-0.2.4/src/backend/langflow/interface/prompts/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/prompts/custom.py` & `langflow-0.2.4/src/backend/langflow/interface/prompts/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/run.py` & `langflow-0.2.4/src/backend/langflow/interface/run.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/text_splitters/base.py` & `langflow-0.2.4/src/backend/langflow/interface/text_splitters/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/toolkits/base.py` & `langflow-0.2.4/src/backend/langflow/interface/toolkits/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/tools/base.py` & `langflow-0.2.4/src/backend/langflow/interface/tools/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/tools/constants.py` & `langflow-0.2.4/src/backend/langflow/interface/tools/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/tools/custom.py` & `langflow-0.2.4/src/backend/langflow/interface/tools/custom.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/tools/util.py` & `langflow-0.2.4/src/backend/langflow/interface/tools/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/types.py` & `langflow-0.2.4/src/backend/langflow/interface/types.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/utilities/base.py` & `langflow-0.2.4/src/backend/langflow/interface/utilities/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/utils.py` & `langflow-0.2.4/src/backend/langflow/interface/utils.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/vector_store/base.py` & `langflow-0.2.4/src/backend/langflow/interface/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/interface/wrappers/base.py` & `langflow-0.2.4/src/backend/langflow/interface/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/main.py` & `langflow-0.2.4/src/backend/langflow/main.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/processing/base.py` & `langflow-0.2.4/src/backend/langflow/processing/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/processing/process.py` & `langflow-0.2.4/src/backend/langflow/processing/process.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/server.py` & `langflow-0.2.4/src/backend/langflow/server.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/settings.py` & `langflow-0.2.4/src/backend/langflow/settings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/field/base.py` & `langflow-0.2.4/src/backend/langflow/template/field/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/frontend_node/agents.py` & `langflow-0.2.4/src/backend/langflow/template/frontend_node/agents.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/frontend_node/base.py` & `langflow-0.2.4/src/backend/langflow/template/frontend_node/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/frontend_node/chains.py` & `langflow-0.2.4/src/backend/langflow/template/frontend_node/chains.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/frontend_node/constants.py` & `langflow-0.2.4/src/backend/langflow/template/frontend_node/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/frontend_node/documentloaders.py` & `langflow-0.2.4/src/backend/langflow/template/frontend_node/documentloaders.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/frontend_node/embeddings.py` & `langflow-0.2.4/src/backend/langflow/template/frontend_node/embeddings.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/frontend_node/llms.py` & `langflow-0.2.4/src/backend/langflow/template/frontend_node/llms.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/frontend_node/memories.py` & `langflow-0.2.4/src/backend/langflow/template/frontend_node/memories.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/frontend_node/prompts.py` & `langflow-0.2.4/src/backend/langflow/template/frontend_node/prompts.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/frontend_node/textsplitters.py` & `langflow-0.2.4/src/backend/langflow/template/frontend_node/textsplitters.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/frontend_node/tools.py` & `langflow-0.2.4/src/backend/langflow/template/frontend_node/tools.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/frontend_node/utilities.py` & `langflow-0.2.4/src/backend/langflow/template/frontend_node/utilities.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/frontend_node/vectorstores.py` & `langflow-0.2.4/src/backend/langflow/template/frontend_node/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/template/template/base.py` & `langflow-0.2.4/src/backend/langflow/template/template/base.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/utils/constants.py` & `langflow-0.2.4/src/backend/langflow/utils/constants.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/utils/logger.py` & `langflow-0.2.4/src/backend/langflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/utils/payload.py` & `langflow-0.2.4/src/backend/langflow/utils/payload.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/utils/util.py` & `langflow-0.2.4/src/backend/langflow/utils/util.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/src/backend/langflow/utils/validate.py` & `langflow-0.2.4/src/backend/langflow/utils/validate.py`

 * *Files identical despite different names*

### Comparing `langflow-0.2.3/PKG-INFO` & `langflow-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Cristhian Zanforlin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langflow Version: 0.2.3 Summary: A Python package
+Metadata-Version: 2.1 Name: langflow Version: 0.2.4 Summary: A Python package
 with a built-in web application Home-page: https://github.com/logspace-ai/
 langflow License: MIT Keywords: nlp,langchain,openai,gpt,gui Author: Logspace
 Author-email: contact@logspace.ai Maintainer: Cristhian Zanforlin Maintainer-
 email: cristhian.lousa@gmail.com Requires-Python: >=3.9,<3.12 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

