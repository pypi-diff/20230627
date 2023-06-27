# Comparing `tmp/jupyterlab_nodeeditor-1.0.1.tar.gz` & `tmp/jupyterlab_nodeeditor-1.0.2.tar.gz`

## Comparing `jupyterlab_nodeeditor-1.0.1.tar` & `jupyterlab_nodeeditor-1.0.2.tar`

### file list

```diff
@@ -1,435 +1,435 @@
--rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/.copier-answers.yml
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/.gitmodules
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/.prettierignore
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/.yarnrc.yml
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/CHANGELOG.md
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/RELEASE.md
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/dev.sh
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/init.sh
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/install.json
--rwxr-xr-x   0        0        0     6214 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/package.json
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/setup.py
--rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/tsconfig.json
--rwxr-xr-x   0        0        0   215226 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/yarn.lock
--rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/.copier-answers.yml
--rwxr-xr-x   0        0        0     1587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/.gitignore
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/.prettierignore
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/.yarnrc.yml
--rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/CHANGELOG.md
--rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/LICENSE
--rwxr-xr-x   0        0        0     2571 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/README.md
--rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/RELEASE.md
--rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/install.json
--rwxr-xr-x   0        0        0     5198 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/package.json
--rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/pyproject.toml
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/setup.py
--rwxr-xr-x   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/tsconfig.json
--rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/jupyterlab_nodeeditor/__init__.py
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/schema/plugin.json
--rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/src/index.ts
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/style/base.css
--rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/style/index.css
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/_temp_extension/style/index.js
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/.babelrc
--rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/.editorconfig
--rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/.eslintrc
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/.git
--rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/.gitignore
--rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/.npmignore
--rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/.nvmrc
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/.travis.yml
--rwxr-xr-x   0        0        0     3369 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/CODE_OF_CONDUCT.md
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/LICENSE
--rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/README.md
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/cypress.json
--rwxr-xr-x   0        0        0   533606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/logo.ai
--rwxr-xr-x   0        0        0    15873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/logo.png
--rwxr-xr-x   0        0        0     3123 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/logo.svg
--rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/package.json
--rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/rollup.config.js
--rwxr-xr-x   0        0        0   675825 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/yarn.lock
--rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/cypress/fixtures/example.json
--rwxr-xr-x   0        0        0     4389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/cypress/integration/NodeEditorSpec.js
--rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/cypress/plugins/index.js
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/cypress/support/commands.js
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/cypress/support/index.js
--rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/.gitignore
--rwxr-xr-x   0        0        0      721 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/README.md
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/babel.config.js
--rwxr-xr-x   0        0        0     3301 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docusaurus.config.js
--rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/package.json
--rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/sidebars.js
--rwxr-xr-x   0        0        0   428509 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/yarn.lock
--rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/blog/2019-05-28-hola.md
--rwxr-xr-x   0        0        0      428 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/blog/2019-05-29-hello-world.md
--rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/blog/2019-05-30-welcome.md
--rwxr-xr-x   0        0        0     4098 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/components/AnatomyExample.js
--rwxr-xr-x   0        0        0     1446 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/components/Colors.js
--rwxr-xr-x   0        0        0     5622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/components/ControlExamples.js
--rwxr-xr-x   0        0        0     5735 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/components/DynamicNodesExamples.js
--rwxr-xr-x   0        0        0     2495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/components/DynamicThemingExample.js
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/components/FlexRow.js
--rwxr-xr-x   0        0        0    16960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/components/GettingStartedExample.js
--rwxr-xr-x   0        0        0     6137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/NodeEditor.mdx
--rwxr-xr-x   0        0        0     5303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/RootEngine.mdx
--rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/anatomy.mdx
--rwxr-xr-x   0        0        0     8565 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/basic-config.mdx
--rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/colors.mdx
--rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/comments.mdx
--rwxr-xr-x   0        0        0     8897 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/controls.mdx
--rwxr-xr-x   0        0        0      525 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/defining-nodes.mdx
--rwxr-xr-x   0        0        0     4129 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/doc1.md
--rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/doc2.md
--rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/doc3.md
--rwxr-xr-x   0        0        0     5038 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/dynamic-nodes.mdx
--rwxr-xr-x   0        0        0     7241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/faq.mdx
--rwxr-xr-x   0        0        0    10532 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/flume-config.mdx
--rwxr-xr-x   0        0        0     4261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/logic-nodes.mdx
--rwxr-xr-x   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/mdx.md
--rwxr-xr-x   0        0        0     2232 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/node-editor.mdx
--rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/overview.mdx
--rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/quick-start.mdx
--rwxr-xr-x   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/root-engine.mdx
--rwxr-xr-x   0        0        0     2978 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/root-node.mdx
--rwxr-xr-x   0        0        0     2981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/running-logic.mdx
--rwxr-xr-x   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/saving-nodes.mdx
--rwxr-xr-x   0        0        0     1929 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/theming.mdx
--rwxr-xr-x   0        0        0     2296 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/type-safety.mdx
--rwxr-xr-x   0        0        0     4178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/using-with-react.mdx
--rwxr-xr-x   0        0        0     1818 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/docs/using-without-react.mdx
--rwxr-xr-x   0        0        0     8877 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/src/exampleFlumeConfig.js
--rwxr-xr-x   0        0        0    49415 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/src/components/TypeSafe.js
--rwxr-xr-x   0        0        0     1304 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/src/css/custom.css
--rwxr-xr-x   0        0        0    15622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/src/pages/index.js
--rwxr-xr-x   0        0        0    11943 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/src/pages/styles.module.css
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/.nojekyll
--rwxr-xr-x   0        0        0     4297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/60fps.svg
--rwxr-xr-x   0        0        0     5914 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/android-chrome-192x192.png
--rwxr-xr-x   0        0        0    17474 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/android-chrome-512x512.png
--rwxr-xr-x   0        0        0     5337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/apple-touch-icon.png
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/arrow-right-blue.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/arrow-right-green.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/arrow-right-red.svg
--rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/arrow-right-red_1.svg
--rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/arrow-right.svg
--rwxr-xr-x   0        0        0     3193 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/controls.svg
--rwxr-xr-x   0        0        0   539930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/example_editors.png
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/favicon-16x16.png
--rwxr-xr-x   0        0        0      765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/favicon-32x32.png
--rwxr-xr-x   0        0        0    15406 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/favicon.ico
--rwxr-xr-x   0        0        0   127864 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/fb-img.png
--rwxr-xr-x   0        0        0   737734 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/flume-short-web.mp4
--rwxr-xr-x   0        0        0     5893 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/friends-graph.svg
--rwxr-xr-x   0        0        0    48634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/hero-nodes.svg
--rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/logo-dark.svg
--rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/logo.svg
--rwxr-xr-x   0        0        0     5626 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/netlify.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/page-curve-blue.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/page-curve-dark.svg
--rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/page-curve.svg
--rwxr-xr-x   0        0        0     1588 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/performance-tile.svg
--rwxr-xr-x   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/play-icon.svg
--rwxr-xr-x   0        0        0     2880 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/react-tile.svg
--rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/size-tile.svg
--rwxr-xr-x   0        0        0     2330 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/theme-tile.svg
--rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/theme.svg
--rwxr-xr-x   0        0        0    41674 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/type-safe-node.svg
--rwxr-xr-x   0        0        0    21728 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/type-safe-nodes.svg
--rwxr-xr-x   0        0        0    31457 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/undraw_docusaurus_mountain.svg
--rwxr-xr-x   0        0        0    35968 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/undraw_docusaurus_react.svg
--rwxr-xr-x   0        0        0    11784 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/undraw_docusaurus_tree.svg
--rwxr-xr-x   0        0        0   146113 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/valid_port_types.png
--rwxr-xr-x   0        0        0      499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/wordmark_white.svg
--rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/.eslintrc
--rwxr-xr-x   0        0        0   105919 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/README.md
--rwxr-xr-x   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/package.json
--rwxr-xr-x   0        0        0   913821 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/yarn.lock
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/public/index.html
--rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/public/manifest.json
--rwxr-xr-x   0        0        0    18960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/App.js
--rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/index.css
--rwxr-xr-x   0        0        0     1503 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/index.js
--rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/TestRoutes/TestEditor.js
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/TestRoutes/nodes.js
--rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/components/Checkbox.js
--rwxr-xr-x   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/components/FloatingNavigation.js
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/components/Header.js
--rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/components/LogicEditor.js
--rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/components/Modal.js
--rwxr-xr-x   0        0        0     2000 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/components/OptionsEditor.js
--rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/icons/BoxIcon.js
--rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/icons/FormIcon.js
--rwxr-xr-x   0        0        0     3783 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/icons/GearIcon.js
--rwxr-xr-x   0        0        0     6066 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/Attributes.js
--rwxr-xr-x   0        0        0     2886 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/Body.js
--rwxr-xr-x   0        0        0     2020 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/Field.js
--rwxr-xr-x   0        0        0    10739 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/Form.css
--rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/Form.js
--rwxr-xr-x   0        0        0     1834 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/InputTypes.js
--rwxr-xr-x   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/NodeTypes.js
--rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/PreviewField.js
--rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/Sidebar.js
--rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/defaultNodes.js
--rwxr-xr-x   0        0        0      815 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/designerReducer.js
--rwxr-xr-x   0        0        0     1261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/fieldTypes.js
--rwxr-xr-x   0        0        0     1560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/fieldsReducer.js
--rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/formHandler.js
--rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/previewFieldsReducer.js
--rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/resolveLogic.js
--rwxr-xr-x   0        0        0     8710 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/wizardLogic/logicTypes.js
--rwxr-xr-x   0        0        0     1910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Forms/Forms.css
--rwxr-xr-x   0        0        0     1854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Forms/Forms.js
--rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Records/Records.css
--rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Records/Records.js
--rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/.eslintrc
--rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/Cache.js
--rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/RootEngine.js
--rwxr-xr-x   0        0        0     1377 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/commentsReducer.js
--rwxr-xr-x   0        0        0     6241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/connectionCalculator.js
--rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/constants.js
--rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/context.js
--rwxr-xr-x   0        0        0     9569 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/index.js
--rwxr-xr-x   0        0        0    13868 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/nodesReducer.js
--rwxr-xr-x   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/stageReducer.js
--rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/styles.css
--rwxr-xr-x   0        0        0     1191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/toastsReducer.js
--rwxr-xr-x   0        0        0     8905 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/typeBuilders.js
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/utilities.js
--rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Checkbox/Checkbox.css
--rwxr-xr-x   0        0        0      651 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Checkbox/Checkbox.js
--rwxr-xr-x   0        0        0     1134 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/ColorPicker/ColorPicker.css
--rwxr-xr-x   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/ColorPicker/ColorPicker.js
--rwxr-xr-x   0        0        0     2159 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Comment/Comment.css
--rwxr-xr-x   0        0        0     5506 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Comment/Comment.js
--rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Connection/Connection.css
--rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Connection/Connection.js
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Connections/Connections.css
--rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Connections/Connections.js
--rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/ContextMenu/ContextMenu.css
--rwxr-xr-x   0        0        0     7010 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/ContextMenu/ContextMenu.js
--rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Control/Control.css
--rwxr-xr-x   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Control/Control.js
--rwxr-xr-x   0        0        0     3751 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Draggable/Draggable.js
--rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/IoPorts/IoPorts.css
--rwxr-xr-x   0        0        0    12769 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/IoPorts/IoPorts.js
--rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Node/Node.css
--rwxr-xr-x   0        0        0     7392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Node/Node.js
--rwxr-xr-x   0        0        0     2001 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Select/Select.css
--rwxr-xr-x   0        0        0     3645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Select/Select.js
--rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Stage/Stage.css
--rwxr-xr-x   0        0        0     8901 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Stage/Stage.js
--rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/TextInput/TextInput.css
--rwxr-xr-x   0        0        0     3063 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/TextInput/TextInput.js
--rwxr-xr-x   0        0        0     2223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Toaster/Toaster.css
--rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/components/Toaster/Toaster.js
--rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/hooks/usePrevious.js
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/img/grid.png
--rwxr-xr-x   0        0        0     8912 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/tests/dynamic.test.js
--rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/tests/nodes.js
--rwxr-xr-x   0        0        0     1409 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/tests/ssr.test.js
--rwxr-xr-x   0        0        0     1397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/flume/src/tests/test.js
--rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/__init__.py
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/_version.py
--rwxr-xr-x   0        0        0     5542 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/package.json
--rwxr-xr-x   0        0        0     6214 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig
--rwxr-xr-x   0        0        0     9120 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json
--rwxr-xr-x   0        0        0     3987 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js.LICENSE.txt
--rwxr-xr-x   0        0        0     6292 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js.LICENSE.txt
--rwxr-xr-x   0        0        0    18679 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3638 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js.LICENSE.txt
--rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7685 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js.LICENSE.txt
--rwxr-xr-x   0        0        0    11356 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1849 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4595 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js.LICENSE.txt
--rwxr-xr-x   0        0        0    10308 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5078 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1183 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5424 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js
--rwxr-xr-x   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js.LICENSE.txt
--rwxr-xr-x   0        0        0     9725 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4055 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     9126 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js.LICENSE.txt
--rwxr-xr-x   0        0        0  3246909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js
--rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2846 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4006 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1927 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1892 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4030 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js.LICENSE.txt
--rwxr-xr-x   0        0        0    17021 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2459 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2519 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7231 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1911 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js.LICENSE.txt
--rwxr-xr-x   0        0        0     6491 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js.LICENSE.txt
--rwxr-xr-x   0        0        0    32283 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js.LICENSE.txt
--rwxr-xr-x   0        0        0    32835 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js.LICENSE.txt
--rwxr-xr-x   0        0        0     6820 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1951 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js.LICENSE.txt
--rwxr-xr-x   0        0        0    16144 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3065 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3470 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js.LICENSE.txt
--rwxr-xr-x   0        0        0    11882 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2342 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js.LICENSE.txt
--rwxr-xr-x   0        0        0    38168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js.LICENSE.txt
--rwxr-xr-x   0        0        0     5447 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2567 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3657 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3351 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3653 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js.LICENSE.txt
--rwxr-xr-x   0        0        0    10379 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8109 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js.LICENSE.txt
--rwxr-xr-x   0        0        0    73464 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf
--rwxr-xr-x   0        0        0     3654 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js
--rwxr-xr-x   0        0        0     8337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js.LICENSE.txt
--rwxr-xr-x   0        0        0     7938 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js.LICENSE.txt
--rwxr-xr-x   0        0        0    22618 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js
--rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js.LICENSE.txt
--rwxr-xr-x   0        0        0    14242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2658 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3155 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js.LICENSE.txt
--rwxr-xr-x   0        0        0   195262 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8863.946765f359766002d15a.js
--rwxr-xr-x   0        0        0     2899 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     1501 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4332 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js.LICENSE.txt
--rwxr-xr-x   0        0        0     3017 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js.LICENSE.txt
--rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js.LICENSE.txt
--rwxr-xr-x   0        0        0     8202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js
--rwxr-xr-x   0        0        0     4099 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js
--rwxr-xr-x   0        0        0     5873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js.LICENSE.txt
--rwxr-xr-x   0        0        0    13543 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js
--rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js.LICENSE.txt
--rwxr-xr-x   0        0        0    12832 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/remoteEntry.120bf7f984546f850c8d.js
--rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/style.js
--rwxr-xr-x   0        0        0     8629 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json
--rwxr-xr-x   0        0        0     9120 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/schema/plugin.json
--rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/ReRunIcon.tsx
--rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/arrownIcon.tsx
--rwxr-xr-x   0        0        0     1455 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/clearIcon.tsx
--rwxr-xr-x   0        0        0      954 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/deleteIcon.tsx
--rwxr-xr-x   0        0        0     1505 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/exportIcon.tsx
--rwxr-xr-x   0        0        0     1310 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/factory.ts
--rwxr-xr-x   0        0        0    37158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/flumeConfig.tsx
--rwxr-xr-x   0        0        0     7454 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/imageViewer.tsx
--rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/index.ts
--rwxr-xr-x   0        0        0     2268 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/lockIcon.tsx
--rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/model.ts
--rwxr-xr-x   0        0        0      807 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/newIcon.tsx
--rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/runIcon.tsx
--rwxr-xr-x   0        0        0     1778 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/utils.tsx
--rwxr-xr-x   0        0        0   139943 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/widget.tsx
--rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/src/yesIcon.tsx
--rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/style/base.css
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/style/index.css
--rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/style/index.js
--rwxr-xr-x   0        0        0     1596 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/.gitignore
--rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/LICENSE
--rwxr-xr-x   0        0        0     2557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/README.md
--rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/.copier-answers.yml
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/.gitmodules
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/.prettierignore
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/.yarnrc.yml
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/CHANGELOG.md
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/RELEASE.md
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/dev.sh
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/init.sh
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/install.json
+-rwxr-xr-x   0        0        0     6214 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/package.json
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/setup.py
+-rwxr-xr-x   0        0        0      583 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/tsconfig.json
+-rwxr-xr-x   0        0        0   215226 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/yarn.lock
+-rwxr-xr-x   0        0        0      456 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/.copier-answers.yml
+-rwxr-xr-x   0        0        0     1587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/.gitignore
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/.prettierignore
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/.yarnrc.yml
+-rwxr-xr-x   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/LICENSE
+-rwxr-xr-x   0        0        0     2571 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/README.md
+-rwxr-xr-x   0        0        0     2314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/RELEASE.md
+-rwxr-xr-x   0        0        0      203 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/install.json
+-rwxr-xr-x   0        0        0     5198 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/package.json
+-rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/pyproject.toml
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/setup.py
+-rwxr-xr-x   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/tsconfig.json
+-rwxr-xr-x   0        0        0      600 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/jupyterlab_nodeeditor/__init__.py
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/schema/plugin.json
+-rwxr-xr-x   0        0        0      920 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/src/index.ts
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/style/base.css
+-rwxr-xr-x   0        0        0       20 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/style/index.css
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/_temp_extension/style/index.js
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/.babelrc
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/.editorconfig
+-rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/.eslintrc
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/.git
+-rwxr-xr-x   0        0        0      376 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/.gitignore
+-rwxr-xr-x   0        0        0       37 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/.npmignore
+-rwxr-xr-x   0        0        0        6 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/.nvmrc
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/.travis.yml
+-rwxr-xr-x   0        0        0     3369 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/LICENSE
+-rwxr-xr-x   0        0        0     2069 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/README.md
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/cypress.json
+-rwxr-xr-x   0        0        0   533606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/logo.ai
+-rwxr-xr-x   0        0        0    15873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/logo.png
+-rwxr-xr-x   0        0        0     3123 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/logo.svg
+-rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/package.json
+-rwxr-xr-x   0        0        0      857 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/rollup.config.js
+-rwxr-xr-x   0        0        0   675825 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/yarn.lock
+-rwxr-xr-x   0        0        0      154 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/cypress/fixtures/example.json
+-rwxr-xr-x   0        0        0     4389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/cypress/integration/NodeEditorSpec.js
+-rwxr-xr-x   0        0        0      718 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/cypress/plugins/index.js
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/cypress/support/commands.js
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/cypress/support/index.js
+-rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/.gitignore
+-rwxr-xr-x   0        0        0      721 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/README.md
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/babel.config.js
+-rwxr-xr-x   0        0        0     3301 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docusaurus.config.js
+-rwxr-xr-x   0        0        0      837 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/package.json
+-rwxr-xr-x   0        0        0      497 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/sidebars.js
+-rwxr-xr-x   0        0        0   428509 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/yarn.lock
+-rwxr-xr-x   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/blog/2019-05-28-hola.md
+-rwxr-xr-x   0        0        0      428 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/blog/2019-05-29-hello-world.md
+-rwxr-xr-x   0        0        0      452 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/blog/2019-05-30-welcome.md
+-rwxr-xr-x   0        0        0     4098 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/components/AnatomyExample.js
+-rwxr-xr-x   0        0        0     1446 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/components/Colors.js
+-rwxr-xr-x   0        0        0     5622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/components/ControlExamples.js
+-rwxr-xr-x   0        0        0     5735 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/components/DynamicNodesExamples.js
+-rwxr-xr-x   0        0        0     2495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/components/DynamicThemingExample.js
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/components/FlexRow.js
+-rwxr-xr-x   0        0        0    16960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/components/GettingStartedExample.js
+-rwxr-xr-x   0        0        0     6137 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/NodeEditor.mdx
+-rwxr-xr-x   0        0        0     5303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/RootEngine.mdx
+-rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/anatomy.mdx
+-rwxr-xr-x   0        0        0     8565 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/basic-config.mdx
+-rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/colors.mdx
+-rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/comments.mdx
+-rwxr-xr-x   0        0        0     8897 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/controls.mdx
+-rwxr-xr-x   0        0        0      525 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/defining-nodes.mdx
+-rwxr-xr-x   0        0        0     4129 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/doc1.md
+-rwxr-xr-x   0        0        0      153 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/doc2.md
+-rwxr-xr-x   0        0        0     2173 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/doc3.md
+-rwxr-xr-x   0        0        0     5038 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/dynamic-nodes.mdx
+-rwxr-xr-x   0        0        0     7241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/faq.mdx
+-rwxr-xr-x   0        0        0    10532 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/flume-config.mdx
+-rwxr-xr-x   0        0        0     4261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/logic-nodes.mdx
+-rwxr-xr-x   0        0        0      521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/mdx.md
+-rwxr-xr-x   0        0        0     2232 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/node-editor.mdx
+-rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/overview.mdx
+-rwxr-xr-x   0        0        0      898 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/quick-start.mdx
+-rwxr-xr-x   0        0        0     4650 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/root-engine.mdx
+-rwxr-xr-x   0        0        0     2978 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/root-node.mdx
+-rwxr-xr-x   0        0        0     2981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/running-logic.mdx
+-rwxr-xr-x   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/saving-nodes.mdx
+-rwxr-xr-x   0        0        0     1929 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/theming.mdx
+-rwxr-xr-x   0        0        0     2296 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/type-safety.mdx
+-rwxr-xr-x   0        0        0     4178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/using-with-react.mdx
+-rwxr-xr-x   0        0        0     1818 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/docs/using-without-react.mdx
+-rwxr-xr-x   0        0        0     8877 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/src/exampleFlumeConfig.js
+-rwxr-xr-x   0        0        0    49415 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/src/components/TypeSafe.js
+-rwxr-xr-x   0        0        0     1304 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/src/css/custom.css
+-rwxr-xr-x   0        0        0    15622 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/src/pages/index.js
+-rwxr-xr-x   0        0        0    11943 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/src/pages/styles.module.css
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/.nojekyll
+-rwxr-xr-x   0        0        0     4297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/60fps.svg
+-rwxr-xr-x   0        0        0     5914 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/android-chrome-192x192.png
+-rwxr-xr-x   0        0        0    17474 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/android-chrome-512x512.png
+-rwxr-xr-x   0        0        0     5337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/apple-touch-icon.png
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/arrow-right-blue.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/arrow-right-green.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/arrow-right-red.svg
+-rwxr-xr-x   0        0        0      439 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/arrow-right-red_1.svg
+-rwxr-xr-x   0        0        0      436 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/arrow-right.svg
+-rwxr-xr-x   0        0        0     3193 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/controls.svg
+-rwxr-xr-x   0        0        0   539930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/example_editors.png
+-rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/favicon-16x16.png
+-rwxr-xr-x   0        0        0      765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/favicon-32x32.png
+-rwxr-xr-x   0        0        0    15406 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/favicon.ico
+-rwxr-xr-x   0        0        0   127864 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/fb-img.png
+-rwxr-xr-x   0        0        0   737734 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/flume-short-web.mp4
+-rwxr-xr-x   0        0        0     5893 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/friends-graph.svg
+-rwxr-xr-x   0        0        0    48634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/hero-nodes.svg
+-rwxr-xr-x   0        0        0     1860 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/logo-dark.svg
+-rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/logo.svg
+-rwxr-xr-x   0        0        0     5626 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/netlify.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/page-curve-blue.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/page-curve-dark.svg
+-rwxr-xr-x   0        0        0      274 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/page-curve.svg
+-rwxr-xr-x   0        0        0     1588 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/performance-tile.svg
+-rwxr-xr-x   0        0        0      377 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/play-icon.svg
+-rwxr-xr-x   0        0        0     2880 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/react-tile.svg
+-rwxr-xr-x   0        0        0     1823 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/size-tile.svg
+-rwxr-xr-x   0        0        0     2330 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/theme-tile.svg
+-rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/theme.svg
+-rwxr-xr-x   0        0        0    41674 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/type-safe-node.svg
+-rwxr-xr-x   0        0        0    21728 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/type-safe-nodes.svg
+-rwxr-xr-x   0        0        0    31457 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/undraw_docusaurus_mountain.svg
+-rwxr-xr-x   0        0        0    35968 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/undraw_docusaurus_react.svg
+-rwxr-xr-x   0        0        0    11784 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/undraw_docusaurus_tree.svg
+-rwxr-xr-x   0        0        0   146113 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/valid_port_types.png
+-rwxr-xr-x   0        0        0      499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/wordmark_white.svg
+-rwxr-xr-x   0        0        0       28 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/.eslintrc
+-rwxr-xr-x   0        0        0   105919 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/README.md
+-rwxr-xr-x   0        0        0     1168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/package.json
+-rwxr-xr-x   0        0        0   913821 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/yarn.lock
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/public/index.html
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/public/manifest.json
+-rwxr-xr-x   0        0        0    18960 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/App.js
+-rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/index.css
+-rwxr-xr-x   0        0        0     1503 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/index.js
+-rwxr-xr-x   0        0        0     1795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/TestRoutes/TestEditor.js
+-rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/TestRoutes/nodes.js
+-rwxr-xr-x   0        0        0      557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/components/Checkbox.js
+-rwxr-xr-x   0        0        0     1895 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/components/FloatingNavigation.js
+-rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/components/Header.js
+-rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/components/LogicEditor.js
+-rwxr-xr-x   0        0        0      380 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/components/Modal.js
+-rwxr-xr-x   0        0        0     2000 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/components/OptionsEditor.js
+-rwxr-xr-x   0        0        0      736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/icons/BoxIcon.js
+-rwxr-xr-x   0        0        0     1223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/icons/FormIcon.js
+-rwxr-xr-x   0        0        0     3783 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/icons/GearIcon.js
+-rwxr-xr-x   0        0        0     6066 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/Attributes.js
+-rwxr-xr-x   0        0        0     2886 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/Body.js
+-rwxr-xr-x   0        0        0     2020 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/Field.js
+-rwxr-xr-x   0        0        0    10739 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/Form.css
+-rwxr-xr-x   0        0        0     5639 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/Form.js
+-rwxr-xr-x   0        0        0     1834 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/InputTypes.js
+-rwxr-xr-x   0        0        0     6297 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/NodeTypes.js
+-rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/PreviewField.js
+-rwxr-xr-x   0        0        0      795 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/Sidebar.js
+-rwxr-xr-x   0        0        0      287 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/defaultNodes.js
+-rwxr-xr-x   0        0        0      815 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/designerReducer.js
+-rwxr-xr-x   0        0        0     1261 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/fieldTypes.js
+-rwxr-xr-x   0        0        0     1560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/fieldsReducer.js
+-rwxr-xr-x   0        0        0      345 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/formHandler.js
+-rwxr-xr-x   0        0        0      580 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/previewFieldsReducer.js
+-rwxr-xr-x   0        0        0     3568 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/resolveLogic.js
+-rwxr-xr-x   0        0        0     8710 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/wizardLogic/logicTypes.js
+-rwxr-xr-x   0        0        0     1910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Forms/Forms.css
+-rwxr-xr-x   0        0        0     1854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Forms/Forms.js
+-rwxr-xr-x   0        0        0      754 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Records/Records.css
+-rwxr-xr-x   0        0        0     1716 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Records/Records.js
+-rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/.eslintrc
+-rwxr-xr-x   0        0        0      105 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/Cache.js
+-rwxr-xr-x   0        0        0     4158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/RootEngine.js
+-rwxr-xr-x   0        0        0     1377 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/commentsReducer.js
+-rwxr-xr-x   0        0        0     6241 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/connectionCalculator.js
+-rwxr-xr-x   0        0        0      176 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/constants.js
+-rwxr-xr-x   0        0        0      579 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/context.js
+-rwxr-xr-x   0        0        0     9569 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/index.js
+-rwxr-xr-x   0        0        0    13868 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/nodesReducer.js
+-rwxr-xr-x   0        0        0      460 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/stageReducer.js
+-rwxr-xr-x   0        0        0      179 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/styles.css
+-rwxr-xr-x   0        0        0     1191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/toastsReducer.js
+-rwxr-xr-x   0        0        0     8905 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/typeBuilders.js
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/utilities.js
+-rwxr-xr-x   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Checkbox/Checkbox.css
+-rwxr-xr-x   0        0        0      651 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Checkbox/Checkbox.js
+-rwxr-xr-x   0        0        0     1134 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/ColorPicker/ColorPicker.css
+-rwxr-xr-x   0        0        0     1934 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/ColorPicker/ColorPicker.js
+-rwxr-xr-x   0        0        0     2159 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Comment/Comment.css
+-rwxr-xr-x   0        0        0     5506 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Comment/Comment.js
+-rwxr-xr-x   0        0        0      125 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Connection/Connection.css
+-rwxr-xr-x   0        0        0      847 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Connection/Connection.js
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Connections/Connections.css
+-rwxr-xr-x   0        0        0      285 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Connections/Connections.js
+-rwxr-xr-x   0        0        0     1547 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/ContextMenu/ContextMenu.css
+-rwxr-xr-x   0        0        0     7010 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/ContextMenu/ContextMenu.js
+-rwxr-xr-x   0        0        0      314 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Control/Control.css
+-rwxr-xr-x   0        0        0     2731 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Control/Control.js
+-rwxr-xr-x   0        0        0     3751 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Draggable/Draggable.js
+-rwxr-xr-x   0        0        0     2499 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/IoPorts/IoPorts.css
+-rwxr-xr-x   0        0        0    12769 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/IoPorts/IoPorts.js
+-rwxr-xr-x   0        0        0      468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Node/Node.css
+-rwxr-xr-x   0        0        0     7392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Node/Node.js
+-rwxr-xr-x   0        0        0     2001 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Select/Select.css
+-rwxr-xr-x   0        0        0     3645 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Select/Select.js
+-rwxr-xr-x   0        0        0     1284 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Stage/Stage.css
+-rwxr-xr-x   0        0        0     8901 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Stage/Stage.js
+-rwxr-xr-x   0        0        0      435 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/TextInput/TextInput.css
+-rwxr-xr-x   0        0        0     3063 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/TextInput/TextInput.js
+-rwxr-xr-x   0        0        0     2223 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Toaster/Toaster.css
+-rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/components/Toaster/Toaster.js
+-rwxr-xr-x   0        0        0      212 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/hooks/usePrevious.js
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/img/grid.png
+-rwxr-xr-x   0        0        0     8912 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/tests/dynamic.test.js
+-rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/tests/nodes.js
+-rwxr-xr-x   0        0        0     1409 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/tests/ssr.test.js
+-rwxr-xr-x   0        0        0     1397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/flume/src/tests/test.js
+-rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/__init__.py
+-rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/_version.py
+-rwxr-xr-x   0        0        0     5542 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/package.json
+-rwxr-xr-x   0        0        0     6214 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig
+-rwxr-xr-x   0        0        0     9220 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json
+-rwxr-xr-x   0        0        0     3987 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     6292 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    18679 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3638 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2267 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8495 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7397 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7685 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5560 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    11356 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1849 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4595 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3213 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    10308 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2736 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5078 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1183 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5424 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4910 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js
+-rwxr-xr-x   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3888 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     9725 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4055 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3672 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1765 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     9126 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js.LICENSE.txt
+-rwxr-xr-x   0        0        0  3246909 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js
+-rwxr-xr-x   0        0        0      576 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2846 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4006 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1927 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1892 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4030 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    17021 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2459 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2519 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7231 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1911 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     6491 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    32283 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    32835 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3981 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     6820 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1951 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    16144 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2634 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3077 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3065 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3470 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    11882 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2342 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7468 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    38168 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     5447 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3303 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2567 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3657 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3351 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3653 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    10379 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8109 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    73464 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf
+-rwxr-xr-x   0        0        0     3654 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js
+-rwxr-xr-x   0        0        0     8337 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     7938 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    22618 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js
+-rwxr-xr-x   0        0        0     6060 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    14242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2658 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3155 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4242 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4606 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0   196018 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8863.3c02516ff41cbeccb48c.js
+-rwxr-xr-x   0        0        0     2899 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     1501 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4332 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     4994 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     3017 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     2484 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8587 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js.LICENSE.txt
+-rwxr-xr-x   0        0        0     8202 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js
+-rwxr-xr-x   0        0        0     4099 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js
+-rwxr-xr-x   0        0        0     5873 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    13543 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js
+-rwxr-xr-x   0        0        0      387 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js.LICENSE.txt
+-rwxr-xr-x   0        0        0    12832 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/remoteEntry.e064f53aae017c82fa69.js
+-rwxr-xr-x   0        0        0      164 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/style.js
+-rwxr-xr-x   0        0        0     8629 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json
+-rwxr-xr-x   0        0        0     9220 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/schema/plugin.json
+-rwxr-xr-x   0        0        0      830 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/ReRunIcon.tsx
+-rwxr-xr-x   0        0        0      926 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/arrownIcon.tsx
+-rwxr-xr-x   0        0        0     1455 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/clearIcon.tsx
+-rwxr-xr-x   0        0        0      954 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/deleteIcon.tsx
+-rwxr-xr-x   0        0        0     1505 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/exportIcon.tsx
+-rwxr-xr-x   0        0        0     1310 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/factory.ts
+-rwxr-xr-x   0        0        0    37158 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/flumeConfig.tsx
+-rwxr-xr-x   0        0        0     7454 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/imageViewer.tsx
+-rwxr-xr-x   0        0        0     2243 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/index.ts
+-rwxr-xr-x   0        0        0     2268 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/lockIcon.tsx
+-rwxr-xr-x   0        0        0      111 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/model.ts
+-rwxr-xr-x   0        0        0      807 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/newIcon.tsx
+-rwxr-xr-x   0        0        0      854 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/runIcon.tsx
+-rwxr-xr-x   0        0        0     1778 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/utils.tsx
+-rwxr-xr-x   0        0        0   141102 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/widget.tsx
+-rwxr-xr-x   0        0        0      856 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/src/yesIcon.tsx
+-rwxr-xr-x   0        0        0      191 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/style/base.css
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/style/index.css
+-rwxr-xr-x   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/style/index.js
+-rwxr-xr-x   0        0        0     1596 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/.gitignore
+-rwxr-xr-x   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/LICENSE
+-rwxr-xr-x   0        0        0     2557 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/README.md
+-rwxr-xr-x   0        0        0     2350 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5392 2020-02-02 00:00:00.000000 jupyterlab_nodeeditor-1.0.2/PKG-INFO
```

### Comparing `jupyterlab_nodeeditor-1.0.1/RELEASE.md` & `jupyterlab_nodeeditor-1.0.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/package.json` & `jupyterlab_nodeeditor-1.0.2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.0.2'"}*

```diff
@@ -174,9 +174,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.0.2"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.1/tsconfig.json` & `jupyterlab_nodeeditor-1.0.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/yarn.lock` & `jupyterlab_nodeeditor-1.0.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/_temp_extension/.gitignore` & `jupyterlab_nodeeditor-1.0.2/_temp_extension/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/_temp_extension/LICENSE` & `jupyterlab_nodeeditor-1.0.2/_temp_extension/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/_temp_extension/README.md` & `jupyterlab_nodeeditor-1.0.2/_temp_extension/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/_temp_extension/RELEASE.md` & `jupyterlab_nodeeditor-1.0.2/_temp_extension/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/_temp_extension/package.json` & `jupyterlab_nodeeditor-1.0.2/_temp_extension/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/_temp_extension/pyproject.toml` & `jupyterlab_nodeeditor-1.0.2/_temp_extension/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/_temp_extension/tsconfig.json` & `jupyterlab_nodeeditor-1.0.2/_temp_extension/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/_temp_extension/jupyterlab_nodeeditor/__init__.py` & `jupyterlab_nodeeditor-1.0.2/_temp_extension/jupyterlab_nodeeditor/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/_temp_extension/src/index.ts` & `jupyterlab_nodeeditor-1.0.2/_temp_extension/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/CODE_OF_CONDUCT.md` & `jupyterlab_nodeeditor-1.0.2/flume/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/LICENSE` & `jupyterlab_nodeeditor-1.0.2/flume/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/README.md` & `jupyterlab_nodeeditor-1.0.2/flume/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/logo.ai` & `jupyterlab_nodeeditor-1.0.2/flume/logo.ai`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/logo.png` & `jupyterlab_nodeeditor-1.0.2/flume/logo.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/logo.svg` & `jupyterlab_nodeeditor-1.0.2/flume/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/package.json` & `jupyterlab_nodeeditor-1.0.2/flume/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/rollup.config.js` & `jupyterlab_nodeeditor-1.0.2/flume/rollup.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/yarn.lock` & `jupyterlab_nodeeditor-1.0.2/flume/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/cypress/integration/NodeEditorSpec.js` & `jupyterlab_nodeeditor-1.0.2/flume/cypress/integration/NodeEditorSpec.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/cypress/plugins/index.js` & `jupyterlab_nodeeditor-1.0.2/flume/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/cypress/support/commands.js` & `jupyterlab_nodeeditor-1.0.2/flume/cypress/support/commands.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/cypress/support/index.js` & `jupyterlab_nodeeditor-1.0.2/flume/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/README.md` & `jupyterlab_nodeeditor-1.0.2/flume/docs/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docusaurus.config.js` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docusaurus.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/package.json` & `jupyterlab_nodeeditor-1.0.2/flume/docs/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/yarn.lock` & `jupyterlab_nodeeditor-1.0.2/flume/docs/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/components/AnatomyExample.js` & `jupyterlab_nodeeditor-1.0.2/flume/docs/components/AnatomyExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/components/Colors.js` & `jupyterlab_nodeeditor-1.0.2/flume/docs/components/Colors.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/components/ControlExamples.js` & `jupyterlab_nodeeditor-1.0.2/flume/docs/components/ControlExamples.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/components/DynamicNodesExamples.js` & `jupyterlab_nodeeditor-1.0.2/flume/docs/components/DynamicNodesExamples.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/components/DynamicThemingExample.js` & `jupyterlab_nodeeditor-1.0.2/flume/docs/components/DynamicThemingExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/components/GettingStartedExample.js` & `jupyterlab_nodeeditor-1.0.2/flume/docs/components/GettingStartedExample.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/NodeEditor.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/NodeEditor.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/RootEngine.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/RootEngine.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/anatomy.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/anatomy.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/basic-config.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/basic-config.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/colors.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/colors.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/comments.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/comments.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/controls.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/controls.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/defining-nodes.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/defining-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/doc1.md` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/doc1.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/doc3.md` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/doc3.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/dynamic-nodes.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/dynamic-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/faq.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/faq.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/flume-config.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/flume-config.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/logic-nodes.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/logic-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/mdx.md` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/mdx.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/node-editor.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/node-editor.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/overview.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/overview.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/quick-start.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/quick-start.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/root-engine.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/root-engine.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/root-node.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/root-node.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/running-logic.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/running-logic.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/saving-nodes.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/saving-nodes.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/theming.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/theming.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/type-safety.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/type-safety.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/using-with-react.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/using-with-react.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/docs/using-without-react.mdx` & `jupyterlab_nodeeditor-1.0.2/flume/docs/docs/using-without-react.mdx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/src/exampleFlumeConfig.js` & `jupyterlab_nodeeditor-1.0.2/flume/docs/src/exampleFlumeConfig.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/src/components/TypeSafe.js` & `jupyterlab_nodeeditor-1.0.2/flume/docs/src/components/TypeSafe.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/src/css/custom.css` & `jupyterlab_nodeeditor-1.0.2/flume/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/src/pages/index.js` & `jupyterlab_nodeeditor-1.0.2/flume/docs/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/src/pages/styles.module.css` & `jupyterlab_nodeeditor-1.0.2/flume/docs/src/pages/styles.module.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/60fps.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/60fps.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/android-chrome-192x192.png` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/android-chrome-512x512.png` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/apple-touch-icon.png` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/controls.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/controls.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/example_editors.png` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/example_editors.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/favicon-32x32.png` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/favicon.ico` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/fb-img.png` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/fb-img.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/flume-short-web.mp4` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/flume-short-web.mp4`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/friends-graph.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/friends-graph.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/hero-nodes.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/hero-nodes.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/logo-dark.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/logo-dark.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/logo.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/netlify.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/netlify.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/performance-tile.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/performance-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/react-tile.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/react-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/size-tile.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/size-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/theme-tile.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/theme-tile.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/theme.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/theme.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/type-safe-node.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/type-safe-node.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/type-safe-nodes.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/type-safe-nodes.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/undraw_docusaurus_mountain.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/undraw_docusaurus_mountain.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/undraw_docusaurus_react.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/undraw_docusaurus_react.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/undraw_docusaurus_tree.svg` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/undraw_docusaurus_tree.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/docs/static/img/valid_port_types.png` & `jupyterlab_nodeeditor-1.0.2/flume/docs/static/img/valid_port_types.png`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/README.md` & `jupyterlab_nodeeditor-1.0.2/flume/example/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/package.json` & `jupyterlab_nodeeditor-1.0.2/flume/example/package.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/yarn.lock` & `jupyterlab_nodeeditor-1.0.2/flume/example/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/public/index.html` & `jupyterlab_nodeeditor-1.0.2/flume/example/public/index.html`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/App.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/App.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/index.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/TestRoutes/TestEditor.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/TestRoutes/TestEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/TestRoutes/nodes.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/TestRoutes/nodes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/components/Checkbox.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/components/Checkbox.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/components/FloatingNavigation.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/components/FloatingNavigation.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/components/LogicEditor.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/components/LogicEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/components/OptionsEditor.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/components/OptionsEditor.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/icons/BoxIcon.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/icons/BoxIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/icons/FormIcon.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/icons/FormIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/icons/GearIcon.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/icons/GearIcon.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/Attributes.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/Attributes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/Body.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/Body.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/Field.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/Field.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/Form.css` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/Form.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/Form.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/Form.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/InputTypes.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/InputTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/NodeTypes.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/NodeTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/PreviewField.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/PreviewField.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/Sidebar.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/Sidebar.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/designerReducer.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/designerReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/fieldTypes.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/fieldTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/fieldsReducer.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/fieldsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/previewFieldsReducer.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/previewFieldsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/resolveLogic.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/resolveLogic.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Form/wizardLogic/logicTypes.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Form/wizardLogic/logicTypes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Forms/Forms.css` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Forms/Forms.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Forms/Forms.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Forms/Forms.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Records/Records.css` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Records/Records.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/example/src/pages/Records/Records.js` & `jupyterlab_nodeeditor-1.0.2/flume/example/src/pages/Records/Records.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/RootEngine.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/RootEngine.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/commentsReducer.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/commentsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/connectionCalculator.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/connectionCalculator.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/context.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/context.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/index.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/index.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/nodesReducer.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/nodesReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/toastsReducer.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/toastsReducer.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/typeBuilders.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/typeBuilders.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/utilities.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/utilities.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/Checkbox/Checkbox.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/Checkbox/Checkbox.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/ColorPicker/ColorPicker.css` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/ColorPicker/ColorPicker.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/ColorPicker/ColorPicker.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/ColorPicker/ColorPicker.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/Comment/Comment.css` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/Comment/Comment.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/Comment/Comment.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/Comment/Comment.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/Connection/Connection.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/Connection/Connection.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/ContextMenu/ContextMenu.css` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/ContextMenu/ContextMenu.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/ContextMenu/ContextMenu.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/ContextMenu/ContextMenu.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/Control/Control.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/Control/Control.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/Draggable/Draggable.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/Draggable/Draggable.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/IoPorts/IoPorts.css` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/IoPorts/IoPorts.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/IoPorts/IoPorts.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/IoPorts/IoPorts.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/Node/Node.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/Node/Node.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/Select/Select.css` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/Select/Select.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/Select/Select.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/Select/Select.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/Stage/Stage.css` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/Stage/Stage.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/Stage/Stage.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/Stage/Stage.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/TextInput/TextInput.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/TextInput/TextInput.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/Toaster/Toaster.css` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/Toaster/Toaster.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/components/Toaster/Toaster.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/components/Toaster/Toaster.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/tests/dynamic.test.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/tests/dynamic.test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/tests/nodes.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/tests/nodes.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/tests/ssr.test.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/tests/ssr.test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/flume/src/tests/test.js` & `jupyterlab_nodeeditor-1.0.2/flume/src/tests/test.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/package.json` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9787326388888888%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e064f53aae017c82fa69.js'}}",*

 * * "'version'": "'1.0.2'"}*

```diff
@@ -106,15 +106,15 @@
         "schema/**/*.json",
         "style/index.js"
     ],
     "homepage": "https://github.com/github_username/jupyterlab_nodeeditor",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.120bf7f984546f850c8d.js",
+            "load": "static/remoteEntry.e064f53aae017c82fa69.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_nodeeditor/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -179,9 +179,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.0.2"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/package.json.orig`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'1.0.2'"}*

```diff
@@ -174,9 +174,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.1"
+    "version": "1.0.2"
 }
```

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/schemas/jupyterlab_nodeeditor/plugin.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998139880952381%*

 * *Differences: {"'jupyter.lab.menus'": "{'main': {0: {'items': {insert: [(27, OrderedDict([('command', "*

 * *                        "'nd-set-as-default')]))]}}}}"}*

```diff
@@ -82,14 +82,17 @@
                         "command": "nd-cell-redo"
                     },
                     {
                         "command": "nd-edit-pre-cell"
                     },
                     {
                         "command": "nd-edit-next-cell"
+                    },
+                    {
+                        "command": "nd-set-as-default"
                     }
                 ],
                 "label": "\u8282\u70b9\u7f16\u8f91\u5668",
                 "rank": 100
             }
         ]
     },
```

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1065.9fc232a423740f88d7f7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1134.0798a6e0f0b366f5ec0e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1147.39b1dbd1dc9f44484129.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1156.51b1cd7d3c43a2460f5b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1259.c5ce71099876a9077b0e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1448.4cd0d08640480a20e1be.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/147.aabb9a95aeaa104ea87c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1471.24c2d2410c69af549513.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/180.35121b49922e87b1c149.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1886.2db2df6f572ece29c0f7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1960.6ec8e86cd017816e8b19.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/1961.6e20f8f707b02ce1cbf8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2060.6bd80005c2f229b0b503.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2075.90a652d1054519d81c67.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2140.f56f1b33eac3015d6da6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2240.a66fd83c780910cfc59d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/249.29fd18b4c942cb74c119.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2571.258bf39d2f3203873c1c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2798.b3bdec92cfa37d47a39a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2814.cb00521a567e09d78d65.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2892.ca540f68ece31947bfc2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2911.eabbf735a43bd0f8f3c5.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/2954.08455b7095d1bc5a62a0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3036.b46a950d8500a6fedb99.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3585.225d1e4e8e91981f6e1f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3632.3178d68a5ee8038d9902.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3682.c29ad46de27c1bfa667e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3760.345604e300cce0d33af3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3837.9c89b698d6aee3df1d54.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/3919.5f7472017a7efdcdae88.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4028.8946573a3bc6851d9836.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4129.23cb6a9a14f87b1d6e32.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4188.8f04d6771e801c8133a2.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4368.55a0be85488d830a88d8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4386.4cd2e0e3046587a32df9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4407.0e49511df47493a41294.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4902.d9a95a926e1babc1af71.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4912.4b183a2e104bb3790b0f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/4946.d33a125321ac0d97ed9e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5062.cf7ab2340467395b8b0b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/525.efd83915541f187fe395.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5288.76cfac5d7da6016bcff7.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5377.8010f4ced2972da327c4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5593.d3d93e1343ca6222ef6a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5703.ea7a26b511d042c9e12d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5849.be4b19eaf4160df7c6b3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5880.88af74925009377e72f6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/5962.4440afe1a5ce11bb01f4.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6082.e47fdc5d826cdd28a7c6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6241.4ede6f570c01e76fab1a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6423.868934ee650d15b2be1e.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6424.4094750d6016604fd3ea.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6449.e29241378f0a62c863db.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6489.0e5448d89dadd7c7a137.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6587.3673bd53fb7d44fbeb2c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/665.df23ff272e3e4d9b2ae1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/6717.132ed63d276f40b99880.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7043.2209cf023190531f3998.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7131.da877c0347b0bbcb4343.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7287.2b85f10dbc3e23c93a0d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7562.67b7fb0bfc56ec0a2cb9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7637.cfee4e5fb8812dc83492.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7778.0eb819ee3d38e06c1c2f.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/7835.64016ba198a8163a5dcb.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/79f233d057d658d1789d.ttf`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8.b10d47f837675650f39c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8070.a8bd6d66f871fce6d53d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8084.dda9b009ce099df0bb96.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8180.a3d01aa0d2f10b552dd3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8401.d14444e38cb7aa24efdd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8424.3938b0f02a27846d3fcd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/848.52559abadf17bbbe08ce.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/854.569d991fc0455bf6780d.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8670.e60df217bf8cf5c38364.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8715.815f4104f6ed5438c593.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8719.e05fefc4bcc2bc7ab0d6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8863.946765f359766002d15a.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8863.3c02516ff41cbeccb48c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,15 @@
         6037: (e, t, n) => {
             "use strict";
             n.d(t, {
                 BC: () => nr,
                 VB: () => or,
                 ZX: () => Io,
                 a2: () => tr,
-                ik: () => Ao,
+                ik: () => So,
                 it: () => ar,
                 oP: () => rr,
                 wL: () => Ro,
                 xV: () => he
             });
             var o = n(6029),
                 r = n.n(o),
@@ -282,27 +282,27 @@
                 }, t.exports), t.exports
             }
             var N = "object" == typeof M && M && M.Object === Object && M,
                 T = "object" == typeof self && self && self.Object === Object && self,
                 I = N || T || Function("return this")(),
                 R = I.Symbol,
                 k = Object.prototype,
-                A = k.hasOwnProperty,
-                S = k.toString,
+                S = k.hasOwnProperty,
+                A = k.toString,
                 L = R ? R.toStringTag : void 0,
                 B = Object.prototype.toString,
                 W = R ? R.toStringTag : void 0,
                 K = function(e) {
                     return null == e ? void 0 === e ? "[object Undefined]" : "[object Null]" : W && W in Object(e) ? function(e) {
-                        var t = A.call(e, L),
+                        var t = S.call(e, L),
                             n = e[L];
                         try {
                             e[L] = void 0
                         } catch (e) {}
-                        var o = S.call(e);
+                        var o = A.call(e);
                         return t ? e[L] = n : delete e[L], o
                     }(e) : function(e) {
                         return B.call(e)
                     }(e)
                 },
                 U = function(e) {
                     return null != e && "object" == typeof e
@@ -447,44 +447,44 @@
                         N = de(P, 2),
                         T = N[0],
                         I = N[1],
                         R = r().useRef(Y(10)),
                         k = function(e) {
                             s(e), a()
                         },
-                        A = r().useCallback((function(e) {
-                            g.current && !g.current.contains(e.target) && (a(), document.removeEventListener("click", A, {
+                        S = r().useCallback((function(e) {
+                            g.current && !g.current.contains(e.target) && (a(), document.removeEventListener("click", S, {
                                 capture: !0
-                            }), document.removeEventListener("contextmenu", A, {
+                            }), document.removeEventListener("contextmenu", S, {
                                 capture: !0
                             }))
                         }), [g, a]),
-                        S = r().useCallback((function(e) {
-                            27 === e.keyCode && (a(), document.removeEventListener("keydown", S, {
+                        A = r().useCallback((function(e) {
+                            27 === e.keyCode && (a(), document.removeEventListener("keydown", A, {
                                 capture: !0
                             }))
                         }), [a]);
                     r().useEffect((function() {
-                        return E.current && E.current.focus(), M(g.current.getBoundingClientRect().width), document.addEventListener("keydown", S, {
+                        return E.current && E.current.focus(), M(g.current.getBoundingClientRect().width), document.addEventListener("keydown", A, {
                                 capture: !0
-                            }), document.addEventListener("click", A, {
+                            }), document.addEventListener("click", S, {
                                 capture: !0
-                            }), document.addEventListener("contextmenu", A, {
+                            }), document.addEventListener("contextmenu", S, {
                                 capture: !0
                             }),
                             function() {
-                                document.removeEventListener("click", A, {
+                                document.removeEventListener("click", S, {
                                     capture: !0
-                                }), document.removeEventListener("contextmenu", A, {
+                                }), document.removeEventListener("contextmenu", S, {
                                     capture: !0
-                                }), document.removeEventListener("keydown", S, {
+                                }), document.removeEventListener("keydown", A, {
                                     capture: !0
                                 })
                             }
-                    }), [A, S]);
+                    }), [S, A]);
                     var L = r().useState([]),
                         B = de(L, 2),
                         W = B[0],
                         K = B[1];
 
                     function U(e, t) {
                         var n = e.toLowerCase();
@@ -719,50 +719,50 @@
                 Te = Pe.toString,
                 Ie = Ne.hasOwnProperty,
                 Re = RegExp("^" + Te.call(Ie).replace(/[\\^$.*+?()[\]{}|]/g, "\\$&").replace(/hasOwnProperty|(function).*?(?=\\\()| for .+?(?=\\\])/g, "$1.*?") + "$"),
                 ke = function(e) {
                     return !(!D(e) || (t = e, we && we in t)) && (xe(e) ? Re : Me).test(De(e));
                     var t
                 },
-                Ae = function(e, t) {
+                Se = function(e, t) {
                     var n = function(e, t) {
                         return null == e ? void 0 : e[t]
                     }(e, t);
                     return ke(n) ? n : void 0
                 },
-                Se = Ae(Object, "create"),
+                Ae = Se(Object, "create"),
                 Le = Object.prototype.hasOwnProperty,
                 Be = Object.prototype.hasOwnProperty;
 
             function We(e) {
                 var t = -1,
                     n = null == e ? 0 : e.length;
                 for (this.clear(); ++t < n;) {
                     var o = e[t];
                     this.set(o[0], o[1])
                 }
             }
             We.prototype.clear = function() {
-                this.__data__ = Se ? Se(null) : {}, this.size = 0
+                this.__data__ = Ae ? Ae(null) : {}, this.size = 0
             }, We.prototype.delete = function(e) {
                 var t = this.has(e) && delete this.__data__[e];
                 return this.size -= t ? 1 : 0, t
             }, We.prototype.get = function(e) {
                 var t = this.__data__;
-                if (Se) {
+                if (Ae) {
                     var n = t[e];
                     return "__lodash_hash_undefined__" === n ? void 0 : n
                 }
                 return Le.call(t, e) ? t[e] : void 0
             }, We.prototype.has = function(e) {
                 var t = this.__data__;
-                return Se ? void 0 !== t[e] : Be.call(t, e)
+                return Ae ? void 0 !== t[e] : Be.call(t, e)
             }, We.prototype.set = function(e, t) {
                 var n = this.__data__;
-                return this.size += this.has(e) ? 0 : 1, n[e] = Se && void 0 === t ? "__lodash_hash_undefined__" : t, this
+                return this.size += this.has(e) ? 0 : 1, n[e] = Ae && void 0 === t ? "__lodash_hash_undefined__" : t, this
             };
             var Ke = We,
                 Ue = function(e, t) {
                     return e === t || e != e && t != t
                 },
                 je = function(e, t) {
                     for (var n = e.length; n--;)
@@ -793,15 +793,15 @@
                 return je(this.__data__, e) > -1
             }, $e.prototype.set = function(e, t) {
                 var n = this.__data__,
                     o = je(n, e);
                 return o < 0 ? (++this.size, n.push([e, t])) : n[o][1] = t, this
             };
             var ze = $e,
-                Fe = Ae(I, "Map"),
+                Fe = Se(I, "Map"),
                 qe = function(e, t) {
                     var n, o, r = e.__data__;
                     return ("string" == (o = typeof(n = t)) || "number" == o || "symbol" == o || "boolean" == o ? "__proto__" !== n : null === n) ? r["string" == typeof t ? "string" : "hash"] : r.map
                 };
 
             function Xe(e) {
                 var t = -1,
@@ -1016,15 +1016,15 @@
                     return !!(t = null == t ? 9007199254740991 : t) && ("number" == n || "symbol" != n && Tt.test(e)) && e > -1 && e % 1 == 0 && e < t
                 },
                 Rt = function(e) {
                     return "number" == typeof e && e > -1 && e % 1 == 0 && e <= 9007199254740991
                 },
                 kt = {};
             kt["[object Float32Array]"] = kt["[object Float64Array]"] = kt["[object Int8Array]"] = kt["[object Int16Array]"] = kt["[object Int32Array]"] = kt["[object Uint8Array]"] = kt["[object Uint8ClampedArray]"] = kt["[object Uint16Array]"] = kt["[object Uint32Array]"] = !0, kt["[object Arguments]"] = kt["[object Array]"] = kt["[object ArrayBuffer]"] = kt["[object Boolean]"] = kt["[object DataView]"] = kt["[object Date]"] = kt["[object Error]"] = kt["[object Function]"] = kt["[object Map]"] = kt["[object Number]"] = kt["[object Object]"] = kt["[object RegExp]"] = kt["[object Set]"] = kt["[object String]"] = kt["[object WeakMap]"] = !1;
-            var At, St, Lt = function(e) {
+            var St, At, Lt = function(e) {
                     return function(t) {
                         return e(t)
                     }
                 },
                 Bt = P((function(e, t) {
                     var n = t && !t.nodeType && t,
                         o = n && e && !e.nodeType && e,
@@ -1052,16 +1052,16 @@
                             return o
                         }(e.length, String) : [],
                         l = s.length;
                     for (var u in e) !t && !Ut.call(e, u) || a && ("length" == u || r && ("offset" == u || "parent" == u) || i && ("buffer" == u || "byteLength" == u || "byteOffset" == u) || It(u, l)) || s.push(u);
                     return s
                 },
                 Vt = Object.prototype,
-                $t = (At = Object.keys, St = Object, function(e) {
-                    return At(St(e))
+                $t = (St = Object.keys, At = Object, function(e) {
+                    return St(At(e))
                 }),
                 zt = Object.prototype.hasOwnProperty,
                 Ft = function(e) {
                     if (n = (t = e) && t.constructor, t !== ("function" == typeof n && n.prototype || Vt)) return $t(e);
                     var t, n, o = [];
                     for (var r in Object(e)) zt.call(e, r) && "constructor" != r && o.push(r);
                     return o
@@ -1078,18 +1078,18 @@
                         return ye(e) ? o : function(e, t) {
                             for (var n = -1, o = t.length, r = e.length; ++n < o;) e[r + n] = t[n];
                             return e
                         }(o, n(e))
                     }(e, Xt, xt)
                 },
                 Zt = Object.prototype.hasOwnProperty,
-                Ht = Ae(I, "DataView"),
-                Jt = Ae(I, "Promise"),
-                Gt = Ae(I, "Set"),
-                Qt = Ae(I, "WeakMap"),
+                Ht = Se(I, "DataView"),
+                Jt = Se(I, "Promise"),
+                Gt = Se(I, "Set"),
+                Qt = Se(I, "WeakMap"),
                 en = "[object Map]",
                 tn = "[object Promise]",
                 nn = "[object Set]",
                 on = "[object WeakMap]",
                 rn = "[object DataView]",
                 an = De(Ht),
                 sn = De(Fe),
@@ -1353,17 +1353,17 @@
                             }
                             return e.index - t.index
                         }(e, t, n)
                     }))
                 },
                 Rn = "__node_editor_stage__",
                 kn = "__node_editor_drag_connection__",
-                An = "__node_editor_connections__";
+                Sn = "__node_editor_connections__";
 
-            function Sn(e) {
+            function An(e) {
                 return {
                     value: e.type,
                     label: e.label,
                     description: e.description,
                     sortIndex: e.sortIndex,
                     node: e
                 }
@@ -1402,24 +1402,24 @@
                     T = r().useRef({
                         x: 0,
                         y: 0
                     }),
                     I = r().useState(!1),
                     R = de(I, 2),
                     k = R[0],
-                    A = R[1],
-                    S = r().useCallback((function() {
+                    S = R[1],
+                    A = r().useCallback((function() {
                         u.current = y.current.getBoundingClientRect()
                     }), []);
                 r().useEffect((function() {
-                    return u.current = y.current.getBoundingClientRect(), window.addEventListener("resize", S),
+                    return u.current = y.current.getBoundingClientRect(), window.addEventListener("resize", A),
                         function() {
-                            window.removeEventListener("resize", S)
+                            window.removeEventListener("resize", A)
                         }
-                }), [u, S]);
+                }), [u, A]);
                 var L = r().useCallback((function(e) {
                         ("TEXTAREA" === e.target.nodeName || e.target.dataset.comment) && e.target.clientHeight < e.target.scrollHeight || (e.preventDefault(), 0 !== l && i((function(t) {
                             var n = t.scale,
                                 o = t.translate,
                                 r = e.deltaY,
                                 i = X(n - .005 * X(r, -10, 10), .1, 7),
                                 a = function(e) {
@@ -1466,28 +1466,28 @@
                             type: "ADD_NODE",
                             x: i,
                             y: a,
                             nodeType: t.type
                         })
                     },
                     U = function e(t) {
-                        32 === t.which && (A(!1), document.removeEventListener("keyup", e))
+                        32 === t.which && (S(!1), document.removeEventListener("keyup", e))
                     };
                 r().useEffect((function() {
                     if (!h) {
                         var e = y.current;
                         return e.addEventListener("wheel", L),
                             function() {
                                 e.removeEventListener("wheel", L)
                             }
                     }
                 }), [L, h]);
                 var j, V, $, z, F, q = (V = Object.values(m).filter((function(e) {
                     return !1 !== e.addable
-                })).map(Sn), $ = ["sortIndex", "label"], j = null == V ? [] : (ye($) || ($ = null == $ ? [] : [$]), ye(z = F ? void 0 : z) || (z = null == z ? [] : [z]), In(V, $, z)), d || j.push({
+                })).map(An), $ = ["sortIndex", "label"], j = null == V ? [] : (ye($) || ($ = null == $ ? [] : [$]), ye(z = F ? void 0 : z) || (z = null == z ? [] : [z]), In(V, $, z)), d || j.push({
                     value: "comment",
                     label: "Comment",
                     description: "A comment for documenting nodes",
                     internalType: "comment"
                 }), j);
                 return f && f.outOptions && f.outOptions({
                     addNode: K,
@@ -1536,15 +1536,15 @@
                                     x: o.x + t,
                                     y: o.y + n
                                 }
                             }
                         }))
                     },
                     onKeyDown: c ? function(e) {
-                        32 === e.which && document.activeElement === y.current && (e.preventDefault(), e.stopPropagation(), A(!0), document.addEventListener("keyup", U))
+                        32 === e.which && document.activeElement === y.current && (e.preventDefault(), e.stopPropagation(), S(!0), document.addEventListener("keyup", U))
                     } : null,
                     tabIndex: -1,
                     stageState: {
                         scale: t,
                         translate: n
                     },
                     style: {
@@ -1894,15 +1894,15 @@
                 },
                 so = function(e) {
                     var t = e.id,
                         n = document.querySelector('[data-connection-id="' + t + '"]');
                     n && n.parentNode.remove()
                 },
                 lo = function(e) {
-                    return document.getElementById("" + An + e)
+                    return document.getElementById("" + Sn + e)
                 },
                 uo = Bn,
                 co = "IoPorts_transput__1wbHA",
                 _o = "IoPorts_portLabel__qOE7y";
             h('.IoPorts_wrapper__3d2hh{\n  display: flex;\n  flex-direction: column;\n  margin-top: auto;\n  width: 100%;\n  padding: 3px;\n}\n.IoPorts_inputs__2etkb{\n  display: flex;\n  flex-direction: column;\n  justify-content: flex-end;\n  width: 100%;\n  margin-bottom: 10px;\n}\n.IoPorts_inputs__2etkb:last-child{\n    margin-bottom: 0px;\n  }\n.IoPorts_inputs__2etkb .IoPorts_transput__1wbHA:first-child .IoPorts_portLabel__qOE7y, .IoPorts_inputs__2etkb .IoPorts_transput__1wbHA:first-child .IoPorts_port__1_a6J{\n        margin-top: 3px;\n      }\n.IoPorts_inputs__2etkb .IoPorts_transput__1wbHA:last-child .IoPorts_portLabel__qOE7y, .IoPorts_inputs__2etkb .IoPorts_transput__1wbHA:last-child .IoPorts_port__1_a6J{\n        margin-bottom: 3px;\n      }\n.IoPorts_outputs__3JGh-{\n  display: flex;\n  flex-direction: column;\n  margin-left: auto;\n  justify-content: flex-end;\n  align-items: flex-end;\n  width: 100%;\n}\n.IoPorts_outputs__3JGh- .IoPorts_transput__1wbHA:last-child .IoPorts_portLabel__qOE7y, .IoPorts_outputs__3JGh- .IoPorts_transput__1wbHA:last-child .IoPorts_port__1_a6J{\n        margin-bottom: 2px;\n      }\n.IoPorts_outputs__3JGh-:first-child{\n    margin-top: 2px;\n  }\n.IoPorts_transput__1wbHA{\n  width: auto;\n  display: flex;\n  align-items: center;\n  margin-top: 2px;\n  margin-bottom: 2px;\n}\n.IoPorts_transput__1wbHA:first-child{\n    margin-top: 0px;\n  }\n.IoPorts_transput__1wbHA[data-controlless="true"]{\n    margin-top: 2px;\n    margin-bottom: 2px;\n  }\n.IoPorts_transput__1wbHA[data-controlless="true"]:first-child{\n      margin-top: 0px;\n    }\n.IoPorts_transput__1wbHA[data-controlless="false"]{\n    margin-top: 2px;\n    margin-bottom: 2px;\n  }\n.IoPorts_controls__1dKFt{\n  display: flex;\n  flex-direction: column;\n  width: 100%;\n}\n.IoPorts_portLabel__qOE7y{\n  font-size: 16px;\n  font-weight: 400;\n  width: 100%;\n}\n.IoPorts_port__1_a6J{\n  width: 14px;\n  height: 14px;\n  background: linear-gradient(to bottom, #acb1b4, #919699);\n  border-radius: 100%;\n  margin-right: 5px;\n  margin-left: -11px;\n  flex: 0 0 auto;\n  box-shadow: 0px 2px 1px 0px rgba(0,0,0,.6);\n}\n.IoPorts_port__1_a6J:last-child{\n    margin-right: -11px;\n    margin-left: 5px;\n  }\n.IoPorts_port__1_a6J[data-port-color="red"]{\n    background: linear-gradient(to bottom, #fa4a6f, #c22e4d);\n  }\n.IoPorts_port__1_a6J[data-port-color="purple"]{\n    background: linear-gradient(to bottom, #9e55fb, #6024b6);\n  }\n.IoPorts_port__1_a6J[data-port-color="blue"]{\n    background: linear-gradient(to bottom, #4284f7, #2867d4);\n  }\n.IoPorts_port__1_a6J[data-port-color="green"]{\n    background: linear-gradient(to bottom, #31dd9f, #11ad7a);\n  }\n.IoPorts_port__1_a6J[data-port-color="yellow"]{\n    background: linear-gradient(to bottom, #d6bf47, #9d8923);\n  }\n.IoPorts_port__1_a6J[data-port-color="orange"]{\n    background: linear-gradient(to bottom, #fa7841, #c94b23);\n  }\n.IoPorts_port__1_a6J[data-port-color="pink"]{\n    background: linear-gradient(to bottom, #fe8aeb, #e046c3);\n  }\n.IoPorts_port__1_a6J[data-port-color="tuple"]{\n    background: linear-gradient(to bottom, #bf00ff, #bf00ff);\n  }\n.IoPorts_port__1_a6J[data-port-color="dict"]{\n    background: linear-gradient(to bottom, #8fc409, #00e1ff);\n  }\n.IoPorts_port__1_a6J[data-port-color="control"]{\n    background: linear-gradient(to bottom, #ffffff, #ffffff);\n  }\n');
             h(".Control_wrapper__VZIiC {\n  width: 100%;\n  padding-right: 3px;\n  padding-top: 3px;\n  padding-bottom: 5px;\n  display: flex;\n}\n\n.Control_label__1OX-Q {\n  font-size: 18px;\n}\n\n.Control_controlLabel__3ga2- {\n  display: flex;\n  align-items: center;\n  font-size: 16px;\n  margin-left: 0px;\n  margin-right: 5px;\n  margin-top: 0px;\n  margin-bottom: 0px;\n  flex: none;\n}");
             h(".Checkbox_wrapper__aSqyY{\n  display: flex;\n  align-items: center;\n}\n.Checkbox_checkbox__Qv5gn{\n  background: linear-gradient(to bottom, #5b5f62, #6f7477);\n  border: 1px solid #3c3e40;\n  border-radius: 4px;\n  margin-right: 8px;\n}\n.Checkbox_label__2RxP-{\n  padding-top: 2px;\n  font-size: 13px;\n}\n");
@@ -2632,78 +2632,78 @@
                                         !i && c.return && c.return()
                                     } finally {
                                         if (a) throw l
                                     }
                                 }
                             }
                         },
-                        A = function() {
+                        S = function() {
                             l && (k(l.inputs), k(l.outputs, !0))
                         },
-                        S = function(e) {
+                        A = function(e) {
                             return e.preventDefault(), e.stopPropagation(), I({
                                 x: e.clientX,
                                 y: e.clientY
                             }), P(!0), !1
                         },
                         L = r().useRef(null);
-                    return h && h.outOptions && h.outOptions((ue(t = {}, "updateNodeConnections_" + n, A), ue(t, "nodeDraggable_" + n, O), ue(t, "startDragDelay_" + n, L), t)), r().createElement(me, {
+                    return h && h.outOptions && h.outOptions((ue(t = {}, "updateNodeConnections_" + n, S), ue(t, "nodeDraggable_" + n, O), ue(t, "startDragDelay_" + n, L), t)), r().createElement(me, {
                         className: "Node_wrapper__3SmT7",
                         style: {
                             width: o,
                             transform: "translate(" + i + "px, " + a + "px)"
                         },
                         onDragStart: function(e) {
                             d(), h && h.onNodeStartDrag && h.onNodeStartDrag(n, O.current)
                         },
                         onDrag: function(e) {
                             var t = e.x,
                                 n = e.y;
-                            O.current.style.transform = "translate(" + t + "px," + n + "px)", A()
+                            O.current.style.transform = "translate(" + t + "px," + n + "px)", S()
                         },
                         onDragEnd: function(e, t) {
                             g(ce({
                                 type: "SET_NODE_COORDINATES"
                             }, t, {
                                 nodeId: n
                             }))
                         },
                         innerRef: O,
                         id: n,
                         "data-node-id": n,
                         "data-flume-component": "node",
                         "data-flume-node-type": E.type,
                         "data-flume-component-is-root": !!_,
-                        onContextMenu: S,
+                        onContextMenu: A,
                         stageState: y,
                         stageRect: s,
                         onMouseDown: function(e) {
                             h && h.onNodeMouseDown && h.onNodeMouseDown(e, n, O.current)
                         },
                         onMouseUp: function(e) {
                             h && h.onNodeMouseUp && h.onNodeMouseUp(e, n, O.current)
                         },
                         startDragDelayRef: L
                     }, p ? p(Po, E, {
-                        openMenu: S,
+                        openMenu: A,
                         closeMenu: function() {
                             P(!1)
                         },
                         deleteNode: function() {
                             g({
                                 type: "REMOVE_NODE",
                                 nodeId: n
                             })
                         }
                     }, n) : r().createElement(Po, null, b), r().createElement(Co, {
                         nodeId: n,
                         inputs: x,
                         outputs: w,
                         connections: l,
-                        updateNodeConnections: A,
+                        updateNodeConnections: S,
                         inputData: c
                     }))
                 },
                 Po = function(e) {
                     var t = e.children,
                         n = e.className,
                         o = void 0 === n ? "" : n,
@@ -2815,15 +2815,15 @@
                                 color: e.color || t.color,
                                 hidePort: No(e.hidePort, t.hidePort),
                                 controls: No(e.controls, t.controls)
                             }
                         }, e
                     }), {})
                 },
-                Ao = function() {
+                So = function() {
                     function e(t) {
                         se(this, e), t ? (this.nodeTypes = ce({}, t.nodeTypes), this.portTypes = ce({}, t.portTypes)) : (this.nodeTypes = {}, this.portTypes = {})
                     }
                     return le(e, [{
                         key: "addRootNodeType",
                         value: function(e) {
                             return this.addNodeType(ce({}, e, {
@@ -2924,15 +2924,15 @@
                                     i = (r[e], _e(r, [e]));
                                 this.portTypes = i
                             } else console.error('Non-existent port type "' + e + '" cannot be removed.');
                             return this
                         }
                     }]), e
                 }(),
-                So = function(e) {
+                Ao = function(e) {
                     var t = e.x,
                         n = e.y,
                         o = e.onColorPicked,
                         i = e.onRequestClose,
                         a = r().useRef(),
                         s = r().useCallback((function(e) {
                             a.current && !a.current.contains(e.target) && (i(), document.removeEventListener("click", s), document.removeEventListener("contextmenu", s))
@@ -3010,17 +3010,17 @@
                         T = de(N, 2),
                         I = T[0],
                         R = T[1],
                         k = r().useState({
                             x: 0,
                             y: 0
                         }),
-                        A = de(k, 2),
-                        S = A[0],
-                        L = A[1],
+                        S = de(k, 2),
+                        A = S[0],
+                        L = S[1],
                         B = function() {
                             E(!0)
                         };
                     return r().useEffect((function() {
                         d && (E(!0), t({
                             type: "REMOVE_COMMENT_NEW",
                             id: n
@@ -3143,17 +3143,17 @@
                                     t({
                                         type: "DELETE_COMMENT",
                                         id: n
                                     })
                             }
                         },
                         from: "comment"
-                    })) : null, C ? r().createElement(b, null, r().createElement(So, {
-                        x: S.x,
-                        y: S.y,
+                    })) : null, C ? r().createElement(b, null, r().createElement(Ao, {
+                        x: A.x,
+                        y: A.y,
                         onRequestClose: function() {
                             return w(!1)
                         },
                         onColorPicked: function(e) {
                             t({
                                 type: "SET_COMMENT_COLOR",
                                 id: n,
@@ -3268,15 +3268,15 @@
                 };
             h(".Connections_svgWrapper__3mXcU{\n  position: absolute;\n  left: 0px;\n  height: 0px;\n}\n");
             var Uo = function(e) {
                     e.nodes;
                     var t = e.editorId;
                     return r().createElement("div", {
                         className: "Connections_svgWrapper__3mXcU",
-                        id: "" + An + t
+                        id: "" + Sn + t
                     })
                 },
                 jo = function(e, t, n) {
                     var o, r = e[t.nodeId],
                         i = r.connections.inputs,
                         a = (i[t.portName], _e(i, [t.portName])),
                         s = ce({}, r, {
@@ -3558,42 +3558,42 @@
                                 P = t.nodeType,
                                 N = t.id,
                                 T = t.defaultNode,
                                 I = t.node,
                                 R = void 0 === I ? null : I;
                             if (null == R) {
                                 var k = N || Y(10),
-                                    A = {
+                                    S = {
                                         id: k,
                                         x: D,
                                         y: M,
                                         type: P,
                                         width: o[P].initialWidth || 200,
                                         connections: {
                                             inputs: {},
                                             outputs: {}
                                         },
                                         inputData: {}
                                     };
-                                return A.inputData = qo({
-                                    node: A,
+                                return S.inputData = qo({
+                                    node: S,
                                     nodeType: o[P],
                                     portTypes: r,
                                     context: s
-                                }), T && (A.defaultNode = !0), o[P].root && (A.root = !0), ce({}, e, ue({}, k, A))
+                                }), T && (S.defaultNode = !0), o[P].root && (S.root = !0), ce({}, e, ue({}, k, S))
                             }
                             return p(ce({}, e, ue({}, R.id, R)), R);
                         case "ADD_NODES":
-                            var S = t.nodes,
+                            var A = t.nodes,
                                 L = e,
                                 B = !0,
                                 W = !1,
                                 K = void 0;
                             try {
-                                for (var U, j = S[Symbol.iterator](); !(B = (U = j.next()).done); B = !0) {
+                                for (var U, j = A[Symbol.iterator](); !(B = (U = j.next()).done); B = !0) {
                                     var V = U.value;
                                     L = p(ce({}, L, ue({}, V.id, V)), V)
                                 }
                             } catch (e) {
                                 W = !0, K = e
                             } finally {
                                 try {
@@ -3898,15 +3898,15 @@
                                 }
                             }));
                         return n.onlyResolveConnected ? a : ce({}, i, a)
                     }
                     return console.error("A root node was not found. The Root Engine requires that exactly one node be marked as the root node."), {}
                 }
             }]);
-            var tr = Sn,
+            var tr = An,
                 nr = ie,
                 or = lo,
                 rr = uo,
                 ir = {},
                 ar = function(e, t) {
                     var n = e.comments,
                         i = e.nodes,
@@ -3931,26 +3931,26 @@
                         M = void 0 !== D && D,
                         P = e.disablePan,
                         N = void 0 !== P && P,
                         T = e.circularBehavior,
                         I = e.renderNodeHeader,
                         R = e.debug,
                         k = (0, o.useContext)(ie),
-                        A = function(e) {
+                        S = function(e) {
                             var t = _ ? p() : null,
                                 n = (0, o.useState)(t),
                                 r = n[0],
                                 i = n[1];
                             return u((function() {
                                 null === r && i(p())
                             }), []), (0, o.useEffect)((function() {
                                 !1 === _ && (_ = !0)
                             }), []), null != r ? String(r) : void 0
                         }(),
-                        S = r().useRef(new Go),
+                        A = r().useRef(new Go),
                         L = r().useRef(),
                         B = r().useState(),
                         W = de(B, 2),
                         K = W[0],
                         U = W[1],
                         j = r().useReducer(Ho, []),
                         V = de(j, 2),
@@ -3959,15 +3959,15 @@
                         F = r().useReducer(function(e, t, n) {
                             return function(o, r) {
                                 return e(o, r, t, n)
                             }
                         }(Xo, {
                             nodeTypes: s,
                             portTypes: c,
-                            cache: S,
+                            cache: A,
                             circularBehavior: T,
                             context: m,
                             owner: k
                         }, U), {}, (function() {
                             return Fo(i, h, s, c, m)
                         })),
                         q = de(F, 2),
@@ -4060,19 +4060,19 @@
                                                         stage: r
                                                     })
                                                 }
                                             }))
                                         }))
                                     }))
                                 }
-                            }(Z, Ee, A)
-                        }), [Z, A, Ee]),
+                            }(Z, Ee, S)
+                        }), [Z, S, Ee]),
                         xe = r().useCallback((function() {
-                            L.current = document.getElementById("" + Rn + A).getBoundingClientRect()
-                        }), [A]);
+                            L.current = document.getElementById("" + Rn + S).getBoundingClientRect()
+                        }), [S]);
                     r().useLayoutEffect((function() {
                         fe && (ve(), me(!1))
                     }), [fe, ve]);
                     var Ce = r().useCallback((function() {
                         me(!0)
                     }), []);
                     r().useImperativeHandle(t, (function() {
@@ -4092,39 +4092,39 @@
                     var Oe = vo(ue);
                     return r().useEffect((function() {
                         Oe && y && ue !== Oe && y(ue)
                     }), [ue, Oe, y]), r().useEffect((function() {
                         K && (z(K), U(null))
                     }), [K]), k && k.outOptions && k.outOptions({
                         refreshCache: function() {
-                            S.current = new Go
+                            A.current = new Go
                         },
                         recalculateStageRect: xe,
                         nanoid: Y,
-                        editorId: A
+                        editorId: S
                     }), r().createElement(J.Provider, {
                         value: c
                     }, r().createElement(H.Provider, {
                         value: s
                     }, r().createElement(G.Provider, {
                         value: ae
                     }, r().createElement(Q.Provider, {
                         value: Ce
                     }, r().createElement(ee.Provider, {
                         value: m
                     }, r().createElement(te.Provider, {
                         value: Ee
                     }, r().createElement(ne.Provider, {
-                        value: S
-                    }, r().createElement(re.Provider, {
                         value: A
+                    }, r().createElement(re.Provider, {
+                        value: S
                     }, r().createElement(oe.Provider, {
                         value: xe
                     }, r().createElement(Ln, {
-                        editorId: A,
+                        editorId: S,
                         scale: Ee.scale,
                         translate: Ee.translate,
                         spaceToPan: v,
                         disablePan: N,
                         disableZoom: M,
                         dispatchStageState: be,
                         dispatchComments: _e,
@@ -4165,18 +4165,18 @@
                             onDragEnd: Ce,
                             onDragStart: xe,
                             renderNodeHeader: I,
                             key: e.id
                         }))
                     })), r().createElement(Uo, {
                         nodes: Z,
-                        editorId: A
+                        editorId: S
                     }), r().createElement("div", {
                         className: Qo.dragWrapper,
-                        id: "" + kn + A
+                        id: "" + kn + S
                     })), k && k.refreshNodeBoxShadow())))))))))
                 };
             ar = r().forwardRef(ar)
         },
         8327: (e, t, n) => {
             "use strict";
             var o = n(5377);
@@ -5622,15 +5622,15 @@
                 nodeErrorBoxShadow = "rgb(255 38 227) 0px 0px 10px 10px",
                 kernelStateMap = {
                     idle: "空闲",
                     busy: "繁忙"
                 };
             class NodeEditorWidget extends _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.ReactWidget {
                 constructor(e, t, n, o) {
-                    super(), this._isReady = !1, this._stopCreateNodeType = !1, this._internal_options = [], this._isSaveNodes = !0, this._curNodesId = "", this._loadingNodes = !1, this._nodeTypes = {}, this._redoList = [], this._redoListIndex = 0, this._redoListMaxLength = 200, this._redoing = null, this._renderCache = null, this._dragging = !1, this._dragStartPos = null, this._dragXDistance = 0, this._dragYDistance = 0, this._scaling = !1, this._scaleStartPos = null, this._scaleDistance = 0, this._scaleXDistance = 0, this._scaleYDistance = 0, this._preAction = null, this._copyedNodes = null, this._containerRef = null, this._editorContainerRef = null, this._draggingSelectedNodes = !1, this._stageDragging = !1, this._selectRectRef = null, this._drawStartPos = null, this._lockedNodes = new Set, this._headRenderCache = {}, this._runCache = {}, this._runCheckCache = !0, this._outputAreaAutoScroll = !0, this._runningNodeId = null, this._runningError = !1, this._exportingCodeNodeId = null, this._exportRet = [], this._exportIndent = "", this._showMsgToNotebook = !0, this._codeEditorValueCache = "", this._saveCode = null, this._curEditingCellIndex = -1, this._stopFilterCell = !1, this._codeEditor = null, this._codeDiffEditor = null, this._renameCache = "", this._interruptingKernel = !1, this.scaleSpeed = .01, this.selectedNodes = new Set, this.keyEventFilter = new Set, this.editorOptions = {}, this.curNodeName = "", this.editorNodes = {}, this._context = e, this._app = t, this._palette = n, this._settings = o;
+                    super(), this._isReady = !1, this._stopCreateNodeType = !1, this._internal_options = [], this._isSaveNodes = !0, this._curNodesId = "", this._loadingNodes = !1, this._nodeTypes = {}, this._redoList = [], this._redoListIndex = 0, this._redoListMaxLength = 200, this._redoing = null, this._renderCache = null, this._dragging = !1, this._dragStartPos = null, this._dragXDistance = 0, this._dragYDistance = 0, this._scaling = !1, this._scaleStartPos = null, this._scaleDistance = 0, this._scaleXDistance = 0, this._scaleYDistance = 0, this._preAction = null, this._copyedNodes = null, this._containerRef = null, this._editorContainerRef = null, this._draggingSelectedNodes = !1, this._stageDragging = !1, this._selectRectRef = null, this._drawStartPos = null, this._lockedNodes = new Set, this._headRenderCache = {}, this._runCache = {}, this._runCheckCache = !0, this._outputAreaAutoScroll = !0, this._runningNodeId = null, this._runningError = !1, this._exportingCodeNodeId = null, this._exportRet = [], this._exportIndent = "", this._showMsgToNotebook = !0, this._codeEditorValueCache = "", this._saveCode = null, this._curEditingCellIndex = -1, this._stopFilterCell = !1, this._codeEditor = null, this._codeDiffEditor = null, this._renameCache = "", this._interruptingKernel = !1, this._curNodesIsDefault = !1, this.scaleSpeed = .01, this.selectedNodes = new Set, this.keyEventFilter = new Set, this.editorOptions = {}, this.curNodeName = "", this.editorNodes = {}, this._context = e, this._app = t, this._palette = n, this._settings = o;
                     let r = this;
                     this._context.model.sharedModel.changed.connect(((e, t) => {
                         this.onContentChanged(e, t)
                     })), this._context.sessionContext.ready.then((async e => {
                         await r.onReady()
                     })), this._context.saveState.connect((() => {
                         r.onSaveState()
@@ -5939,15 +5939,17 @@
                             }
                         }, react__WEBPACK_IMPORTED_MODULE_8___default().createElement("label", null, "名称:(", c, ")"), react__WEBPACK_IMPORTED_MODULE_8___default().createElement("br", null), react__WEBPACK_IMPORTED_MODULE_8___default().createElement("label", {
                             "data-name": "node-editor-kernel-state-label",
                             style: {
                                 height: "100%",
                                 backgroundColor: "rgba(0, 0, 0, 0)"
                             }
-                        }, "空闲"))), e && react__WEBPACK_IMPORTED_MODULE_8___default().createElement("div", {
+                        }, "空闲"), react__WEBPACK_IMPORTED_MODULE_8___default().createElement("br", null), react__WEBPACK_IMPORTED_MODULE_8___default().createElement("label", {
+                            id: "id-default-node-label"
+                        }))), e && react__WEBPACK_IMPORTED_MODULE_8___default().createElement("div", {
                             style: {
                                 position: "absolute",
                                 left: "0px",
                                 top: "0px",
                                 width: "100%",
                                 height: "100%"
                             }
@@ -6827,15 +6829,15 @@
                         const n = this.cellGet(t);
                         if ("code" == n.type) {
                             let t = this._get_node_data(n);
                             if (!t) continue;
                             e.push(t)
                         }
                     }
-                    return e
+                    return e.length > 0 && (e[0].data.default = !0), e
                 }
                 async _saveNodes(e) {
                     if (!this._isSaveNodes) return;
                     "" == this._curNodesId && (this._curNodesId = (0, uuid__WEBPACK_IMPORTED_MODULE_9__.v4)());
                     let t = {
                         id: this._curNodesId,
                         name: this.curNodeName,
@@ -6894,26 +6896,30 @@
                                             } catch (e) {}
                                             e.type == n.type && (o = !0)
                                         }
                                     }
                                 }
                                 if (!o) return !1
                             }
-                            return e.locked && (this._lockedNodes = new Set([...e.locked])), await this._readRunCache(e), this.setEditorConfig(this.editorConfig), this._clearNodes(), this.dispatchNodes({
+                            return e.locked && (this._lockedNodes = new Set([...e.locked])), await this._readRunCache(e), this._curNodesIsDefault = e.default, this.setEditorConfig(this.editorConfig), this._clearNodes(), this.dispatchNodes({
                                 type: "RE_INIT",
                                 nodes: e.nodes
                             }), this.setEditorNodes(e.nodes), this.setCurNodeName(e.name), this._curNodesId = e.id, this._isSaveNodes = !0, this._clearRedoList(), setTimeout((() => {
-                                this._focusToAllNodes()
+                                this._focusToAllNodes(), this._updateNodesDefaultShow()
                             })), !0
                         } catch (e) {} finally {
                             this._loadingNodes = !1
                         }
                         return !1
                     }
                 }
+                _updateNodesDefaultShow() {
+                    const e = document.getElementById("id-default-node-label");
+                    e && (e.innerText = this._curNodesIsDefault ? "默认" : "非默认")
+                }
                 async _checkSessionAndKernel(e) {
                     var t;
                     const n = (e = e || _jupyterlab_translation__WEBPACK_IMPORTED_MODULE_2__.nullTranslator).load("jupyterlab");
                     let o = this._context.sessionContext;
                     if (o && o.isTerminating) {
                         let e = (null === (t = o.session) || void 0 === t ? void 0 : t.path) || "";
                         return (0, _jupyterlab_apputils__WEBPACK_IMPORTED_MODULE_1__.showDialog)({
@@ -7722,14 +7728,21 @@
                         })), this._createCommand("nd-cell-redo", "nd-cell-redo(重做Cell)", (() => {
                             this.cellRedo(), this._editCell(this._curEditingCellIndex)
                         })), this._createCommand("nd-edit-pre-cell", "nd-edit-pre-cell(编辑上一个Cell)", (() => {
                             this._editCell(Math.max(this._curEditingCellIndex - 1, 0))
                         })), this._createCommand("nd-edit-next-cell", "nd-edit-next-cell(编辑下一个Cell)", (() => {
                             const e = this._context.model.cells;
                             this._editCell(Math.min(this._curEditingCellIndex + 1, e.length - 1))
+                        })), this._createCommand("nd-set-as-default", "nd-set-as-default(设置为默认)", (() => {
+                            const e = this._getCurNodeCellModel();
+                            if (e) {
+                                const t = this.cellGet(0),
+                                    n = e.sharedModel.getSource();
+                                e.sharedModel.setSource(t.sharedModel.getSource()), t.sharedModel.setSource(n), this._curNodesIsDefault = !0, this._updateNodesDefaultShow()
+                            }
                         }))
                     } catch (e) {}
                 }
             }
             const NOTEBOOK_PANEL_TOOLBAR_CLASS = "jp-NotebookPanel-toolbar";
             class NodeEditorDocumentWidget extends _jupyterlab_docregistry__WEBPACK_IMPORTED_MODULE_0__.DocumentWidget {
                 constructor(e) {
```

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8906.b9ef8e8fbada8f634ff8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/8946.e37c54e493ef0fcd3129.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/911.54d4e2a70d9237abc6dd.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9343.68df0c5454cb71b71ac8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9398.e709c53f5309c556391b.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9400.af8212185e81be7c179c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9537.5b34dc2ee55a5048c2a8.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9684.31d4865e5191437dcb69.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9687.0805ace94c0cdeaabf35.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9747.77aa0e73ef6f7f90faff.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/9907.d82be9ce7f1b2830eed6.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/996.66980e5a835d45afb0e9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/remoteEntry.120bf7f984546f850c8d.js` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/remoteEntry.e064f53aae017c82fa69.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -120,15 +120,15 @@
         8084: "dda9b009ce099df0bb96",
         8180: "a3d01aa0d2f10b552dd3",
         8401: "d14444e38cb7aa24efdd",
         8424: "3938b0f02a27846d3fcd",
         8670: "e60df217bf8cf5c38364",
         8715: "815f4104f6ed5438c593",
         8719: "e05fefc4bcc2bc7ab0d6",
-        8863: "946765f359766002d15a",
+        8863: "3c02516ff41cbeccb48c",
         8906: "b9ef8e8fbada8f634ff8",
         8946: "e37c54e493ef0fcd3129",
         9343: "68df0c5454cb71b71ac8",
         9398: "e709c53f5309c556391b",
         9400: "af8212185e81be7c179c",
         9537: "5b34dc2ee55a5048c2a8",
         9684: "31d4865e5191437dcb69",
@@ -209,15 +209,15 @@
         8084: "dda9b009ce099df0bb96",
         8180: "a3d01aa0d2f10b552dd3",
         8401: "d14444e38cb7aa24efdd",
         8424: "3938b0f02a27846d3fcd",
         8670: "e60df217bf8cf5c38364",
         8715: "815f4104f6ed5438c593",
         8719: "e05fefc4bcc2bc7ab0d6",
-        8863: "946765f359766002d15a",
+        8863: "3c02516ff41cbeccb48c",
         8906: "b9ef8e8fbada8f634ff8",
         8946: "e37c54e493ef0fcd3129",
         9343: "68df0c5454cb71b71ac8",
         9398: "e709c53f5309c556391b",
         9400: "af8212185e81be7c179c",
         9537: "5b34dc2ee55a5048c2a8",
         9684: "31d4865e5191437dcb69",
@@ -279,15 +279,15 @@
                         (!b || !b.loaded && (!f != !b.eager ? f : t > b.from)) && (c[a] = {
                             get: d,
                             from: t,
                             eager: !!f
                         })
                     },
                     o = [];
-                return "default" === d && (b("jupyterlab_nodeeditor", "1.0.1", (() => P.e(8863).then((() => () => P(8863))))), b("monaco-editor", "0.39.0", (() => Promise.all([P.e(3837), P.e(8)]).then((() => () => P(3837))))), b("uuid", "9.0.0", (() => P.e(9687).then((() => () => P(9687)))))), e[d] = o.length ? Promise.all(o).then((() => e[d] = 1)) : 1
+                return "default" === d && (b("jupyterlab_nodeeditor", "1.0.2", (() => P.e(8863).then((() => () => P(8863))))), b("monaco-editor", "0.39.0", (() => Promise.all([P.e(3837), P.e(8)]).then((() => () => P(3837))))), b("uuid", "9.0.0", (() => P.e(9687).then((() => () => P(9687)))))), e[d] = o.length ? Promise.all(o).then((() => e[d] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var a = P.g.document;
         if (!e && a && (a.currentScript && (e = a.currentScript.src), !e)) {
```

### Comparing `jupyterlab_nodeeditor-1.0.1/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json` & `jupyterlab_nodeeditor-1.0.2/jupyterlab_nodeeditor/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/schema/plugin.json` & `jupyterlab_nodeeditor-1.0.2/schema/plugin.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998139880952381%*

 * *Differences: {"'jupyter.lab.menus'": "{'main': {0: {'items': {insert: [(27, OrderedDict([('command', "*

 * *                        "'nd-set-as-default')]))]}}}}"}*

```diff
@@ -82,14 +82,17 @@
                         "command": "nd-cell-redo"
                     },
                     {
                         "command": "nd-edit-pre-cell"
                     },
                     {
                         "command": "nd-edit-next-cell"
+                    },
+                    {
+                        "command": "nd-set-as-default"
                     }
                 ],
                 "label": "\u8282\u70b9\u7f16\u8f91\u5668",
                 "rank": 100
             }
         ]
     },
```

### Comparing `jupyterlab_nodeeditor-1.0.1/src/ReRunIcon.tsx` & `jupyterlab_nodeeditor-1.0.2/src/ReRunIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/src/arrownIcon.tsx` & `jupyterlab_nodeeditor-1.0.2/src/arrownIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/src/clearIcon.tsx` & `jupyterlab_nodeeditor-1.0.2/src/clearIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/src/deleteIcon.tsx` & `jupyterlab_nodeeditor-1.0.2/src/deleteIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/src/exportIcon.tsx` & `jupyterlab_nodeeditor-1.0.2/src/exportIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/src/factory.ts` & `jupyterlab_nodeeditor-1.0.2/src/factory.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/src/flumeConfig.tsx` & `jupyterlab_nodeeditor-1.0.2/src/flumeConfig.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/src/imageViewer.tsx` & `jupyterlab_nodeeditor-1.0.2/src/imageViewer.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/src/index.ts` & `jupyterlab_nodeeditor-1.0.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/src/lockIcon.tsx` & `jupyterlab_nodeeditor-1.0.2/src/lockIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/src/newIcon.tsx` & `jupyterlab_nodeeditor-1.0.2/src/newIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/src/runIcon.tsx` & `jupyterlab_nodeeditor-1.0.2/src/runIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/src/utils.tsx` & `jupyterlab_nodeeditor-1.0.2/src/utils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/src/widget.tsx` & `jupyterlab_nodeeditor-1.0.2/src/widget.tsx`

 * *Files 0% similar despite different names*

```diff
@@ -123,14 +123,15 @@
     private _curEditingCellIndex = -1
     private _stopFilterCell = false
     private _codeEditor: monaco.editor.IStandaloneCodeEditor | null = null
     private _codeDiffEditor: monaco.editor.IStandaloneDiffEditor | null = null
     private _cellIndexInputRef
     private _renameCache = ""
     private _interruptingKernel = false
+    private _curNodesIsDefault = false
 
 
     scaleSpeed = 0.01 // 缩放的速度，_scaleDistance * scaleSpeed 就是新的缩放值
     selectedNodes = new Set<string>() // 选择的节点
     keyEventFilter = new Set<string>()// 按键过滤器，用于过滤键盘操作
     editorOptions = {} // 有flume导出的函数变量等。。
     setShowImg: any // 用于设置是否打开图片查看器 setShowImg(true/false)
@@ -706,14 +707,16 @@
                             }}>
                                 <label>名称:({nodesName})</label>
                                 <br />
                                 <label data-name="node-editor-kernel-state-label" style={{
                                     height: "100%",
                                     backgroundColor: "rgba(0, 0, 0, 0)"
                                 }}>空闲</label>
+                                <br />
+                                <label id="id-default-node-label"></label>
                             </span>
                         </div>
                         {/* 图片浏览器 */}
                         {showImg && <div style={{
                             position: "absolute", left: "0px", top: "0px",
                             width: "100%",
                             height: "100%",
@@ -2254,14 +2257,19 @@
                 let data: any = this._get_node_data(cell as CodeCellModel)
                 if (!data) {
                     continue
                 }
                 ret.push(data)
             }
         }
+
+        if (ret.length > 0) {
+            ret[0].data.default = true
+        }
+
         return ret
     }
 
     private async _saveNodes(nodes: NodeMap) {
         if (!this._isSaveNodes) return
         if (this._curNodesId == "") {
             this._curNodesId = uuidv4()
@@ -2378,38 +2386,46 @@
             // 3.锁定的节点
             if (data.locked) {
                 this._lockedNodes = new Set([...data.locked])
             }
 
             // 4.运行缓存
             await this._readRunCache(data)
-
+            this._curNodesIsDefault = data.default
             this.setEditorConfig(this.editorConfig)
             // 清除当前数据
             this._clearNodes()
             // 加载node数据
             this.dispatchNodes({ type: "RE_INIT", nodes: data.nodes })
             this.setEditorNodes(data.nodes)
             this.setCurNodeName(data.name)
             this._curNodesId = data.id
             this._isSaveNodes = true
             // 清除redolist
             this._clearRedoList()
 
             setTimeout(() => {
                 this._focusToAllNodes()
+                this._updateNodesDefaultShow()
             })
             return true
         } catch (error) {
         } finally {
             this._loadingNodes = false
         }
         return false
     }
 
+    private _updateNodesDefaultShow(){
+        const element = document.getElementById("id-default-node-label")
+        if (element) {
+            element.innerText = this._curNodesIsDefault ? "默认" : "非默认"
+        }
+    }
+
     private async _checkSessionAndKernel(translator: ITranslator | null) {
         translator = translator || nullTranslator;
         const trans = translator.load('jupyterlab');
         let sessionContext = this._context.sessionContext
         // 检查是否正在打断执行
         if (sessionContext) {
             if (sessionContext.isTerminating) {
@@ -3896,14 +3912,26 @@
             })
 
             this._createCommand("nd-edit-next-cell", "nd-edit-next-cell(编辑下一个Cell)", () => {
                 const cells = this._context.model.cells
                 this._editCell(Math.min(this._curEditingCellIndex + 1, cells.length - 1))
             })
 
+            this._createCommand("nd-set-as-default", "nd-set-as-default(设置为默认)", () => {
+                const curModel = this._getCurNodeCellModel()
+                if (curModel) {
+                    const firstModel = this.cellGet(0)
+                    const temp = curModel.sharedModel.getSource()
+                    curModel.sharedModel.setSource(firstModel.sharedModel.getSource())
+                    firstModel.sharedModel.setSource(temp)
+                    this._curNodesIsDefault = true
+                    this._updateNodesDefaultShow()
+                }
+            })
+
         } catch (error) {
 
         }
     }
 }
 
 const NOTEBOOK_PANEL_TOOLBAR_CLASS = 'jp-NotebookPanel-toolbar';
```

### Comparing `jupyterlab_nodeeditor-1.0.1/src/yesIcon.tsx` & `jupyterlab_nodeeditor-1.0.2/src/yesIcon.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/.gitignore` & `jupyterlab_nodeeditor-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/LICENSE` & `jupyterlab_nodeeditor-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/README.md` & `jupyterlab_nodeeditor-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/pyproject.toml` & `jupyterlab_nodeeditor-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_nodeeditor-1.0.1/PKG-INFO` & `jupyterlab_nodeeditor-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_nodeeditor
-Version: 1.0.1
+Version: 1.0.2
 Summary: 一个节点编辑器
 Project-URL: Homepage, https://github.com/github_username/jupyterlab_nodeeditor
 Project-URL: Bug Tracker, https://github.com/github_username/jupyterlab_nodeeditor/issues
 Project-URL: Repository, https://github.com/github_username/jupyterlab_nodeeditor.git
 Author-email: l0n0l <cenlan@hotmail.com>
 License: BSD 3-Clause License
```

