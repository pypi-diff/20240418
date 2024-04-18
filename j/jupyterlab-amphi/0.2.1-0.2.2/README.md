# Comparing `tmp/jupyterlab_amphi-0.2.1.tar.gz` & `tmp/jupyterlab_amphi-0.2.2.tar.gz`

## Comparing `jupyterlab_amphi-0.2.1.tar` & `jupyterlab_amphi-0.2.2.tar`

### file list

```diff
@@ -1,134 +1,137 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/.yarnrc.yml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/MANIFEST.in
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/install.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/lerna.json
--rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/output.json
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/package.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/setup.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/tsconfig.eslint.json
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/tsconfigbase.json
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/_version.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/package.json
--rw-r--r--   0        0        0   109320 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/static/354.17f2b6e853bc242211f3.js
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/static/432.df81fd96e756f14c54d0.js
--rw-r--r--   0        0        0   542676 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/static/713.a7e0851307239af436d3.js
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/static/713.a7e0851307239af436d3.js.LICENSE.txt
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/static/remoteEntry.f28dd63fd7611d76a5b4.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/static/style.js
--rw-r--r--   0        0        0    24579 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/static/third-party-licenses.json
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/package.json
--rw-r--r--   0        0        0    34980 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js
--rw-r--r--   0        0        0    24459 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/143.c7653d290fba1605b212.js
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/143.c7653d290fba1605b212.js.LICENSE.txt
--rw-r--r--   0        0        0  1436458 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/37.77034b0c839d0f88327f.js
--rw-r--r--   0        0        0    32808 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/37.77034b0c839d0f88327f.js.LICENSE.txt
--rw-r--r--   0        0        0   142152 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/379.1427c0520c9ac5a71632.js
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/379.1427c0520c9ac5a71632.js.LICENSE.txt
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/432.5fd4f051d4b18df45075.js
--rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js
--rw-r--r--   0        0        0    43449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/719.3c5804917b7a839b516d.js
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js.LICENSE.txt
--rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/remoteEntry.34ddf437229e19983422.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/style.js
--rw-r--r--   0        0        0   122507 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/third-party-licenses.json
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-editor/package.json
--rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/121.db61795daabb4d1eb7c3.js
--rw-r--r--   0        0        0    22302 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/219.2f775af86603225cd107.js
--rw-r--r--   0        0        0   152538 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/285.4eef7e98cbfad514e073.js
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/285.4eef7e98cbfad514e073.js.LICENSE.txt
--rw-r--r--   0        0        0    23558 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/550.c5bd7757f7228cea68ce.js
--rw-r--r--   0        0        0   180006 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/636.e37faa04eb8cb39edd7f.js
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/636.e37faa04eb8cb39edd7f.js.LICENSE.txt
--rw-r--r--   0        0        0     8366 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/remoteEntry.44274364debca46ec439.js
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/style.js
--rw-r--r--   0        0        0    44588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/third-party-licenses.json
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/package.json
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/static/432.a6577eba0279cb4b76e3.js
--rw-r--r--   0        0        0   627216 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/static/444.36935dbcd8fc3a74e25f.js
--rw-r--r--   0        0        0    15071 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/static/444.36935dbcd8fc3a74e25f.js.LICENSE.txt
--rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/static/684.2b2213062b13c7490a61.js
--rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/static/remoteEntry.9a28884c4594f181f68a.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/static/style.js
--rw-r--r--   0        0        0    62362 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/static/third-party-licenses.json
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-metadata-panel/package.json
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js
--rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-metadata-panel/static/732.5ee1843a7c6f18d4f9f9.js
--rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-metadata-panel/static/remoteEntry.d15f4d692407bd368832.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-metadata-panel/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi/pipeline-metadata-panel/static/third-party-licenses.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/amphi_extension/_version.py
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/package.json
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/tsconfig.json
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
--rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/CodeGenerator.tsx
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/CustomHandle.tsx
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/PipelineComponent.tsx
--rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/PipelineService.tsx
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/RequestService.tsx
--rw-r--r--   0        0        0    18221 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/configUtils.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/declarations.d.ts
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/icons.ts
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/index.ts
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/rendererUtils.tsx
--rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
--rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/selectColumn.tsx
--rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/selectColumns.tsx
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
--rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/selectRegular.tsx
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
--rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/transferData.tsx
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/base.css
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/index.js
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/crosshair-16.svg
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/minus-16.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/play-16.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/play-circle-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/plus-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/plus-24.svg
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/search-16.svg
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/search-24.svg
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/settings-16.svg
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/settings-24.svg
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/trash-16.svg
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/trash-24.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/x-16.svg
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/x-square-16.svg
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/package.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/pipeline-16.svg
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/pipeline-24.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/tailwind.config.js
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/tsconfig.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/schema/extension.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/schema/plugin copy.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/schema/plugin.json
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/src/Dropzone.tsx
--rw-r--r--   0        0        0    18461 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/src/PipelineEditorWidget.tsx
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/src/customEdge.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/src/declarations.d.ts
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/src/icons.ts
--rw-r--r--   0        0        0    17975 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/src/index.ts
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/canvas.css
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/index.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/index.js
--rw-r--r--   0        0        0    21779 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/output.css
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/pipeline-category-icon.svg
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/react-icon.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/tailwinds_preflight.css
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/icons/api-24.svg
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/icons/file-plus-24.svg
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/icons/file-text-24.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/icons/monitor-24.svg
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/.gitignore
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/LICENSE
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/README.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/.yarnrc.yml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/MANIFEST.in
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/install.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/lerna.json
+-rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/output.json
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/package.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/tsconfig.eslint.json
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/tsconfigbase.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/_version.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/package.json
+-rw-r--r--   0        0        0   109320 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/static/354.17f2b6e853bc242211f3.js
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/static/432.df81fd96e756f14c54d0.js
+-rw-r--r--   0        0        0   542676 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/static/713.a7e0851307239af436d3.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/static/713.a7e0851307239af436d3.js.LICENSE.txt
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/static/remoteEntry.9e880e90f12441f9cd92.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/static/style.js
+-rw-r--r--   0        0        0    24579 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0    34980 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js
+-rw-r--r--   0        0        0    24459 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/143.c7653d290fba1605b212.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/143.c7653d290fba1605b212.js.LICENSE.txt
+-rw-r--r--   0        0        0  1436661 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/37.49e35d770e38d792a11d.js
+-rw-r--r--   0        0        0    32808 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/37.49e35d770e38d792a11d.js.LICENSE.txt
+-rw-r--r--   0        0        0   142152 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/379.1427c0520c9ac5a71632.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/379.1427c0520c9ac5a71632.js.LICENSE.txt
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/432.5fd4f051d4b18df45075.js
+-rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js
+-rw-r--r--   0        0        0    43453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/719.c9d87c8fac95544e1714.js
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js.LICENSE.txt
+-rw-r--r--   0        0        0     8337 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/remoteEntry.eefc39996b3e8a655b2e.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/style.js
+-rw-r--r--   0        0        0   122507 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-editor/package.json
+-rw-r--r--   0        0        0     3501 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/121.db61795daabb4d1eb7c3.js
+-rw-r--r--   0        0        0    22302 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/219.2f775af86603225cd107.js
+-rw-r--r--   0        0        0   152538 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/285.4eef7e98cbfad514e073.js
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/285.4eef7e98cbfad514e073.js.LICENSE.txt
+-rw-r--r--   0        0        0    23558 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/550.c5bd7757f7228cea68ce.js
+-rw-r--r--   0        0        0   180209 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/636.18742a3929885dfb4bfa.js
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/636.18742a3929885dfb4bfa.js.LICENSE.txt
+-rw-r--r--   0        0        0     8366 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/remoteEntry.90789c29a44dad669aa0.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/style.js
+-rw-r--r--   0        0        0    44588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/package.json
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/static/432.a6577eba0279cb4b76e3.js
+-rw-r--r--   0        0        0   627423 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/static/444.35926916905e9c76b8c9.js
+-rw-r--r--   0        0        0    15071 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/static/444.35926916905e9c76b8c9.js.LICENSE.txt
+-rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/static/684.2b2213062b13c7490a61.js
+-rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/static/remoteEntry.de9bf8c4ac18d1151373.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/static/style.js
+-rw-r--r--   0        0        0    62362 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-metadata-panel/package.json
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js
+-rw-r--r--   0        0        0    23320 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-metadata-panel/static/732.5ee1843a7c6f18d4f9f9.js
+-rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-metadata-panel/static/remoteEntry.d7f8174936e132a8b035.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-metadata-panel/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi/pipeline-metadata-panel/static/third-party-licenses.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi_extension/_version.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/install.json
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/tsconfig.json
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/CodeGenerator.tsx
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/CustomHandle.tsx
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/PipelineComponent.tsx
+-rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/PipelineService.tsx
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/RequestService.tsx
+-rw-r--r--   0        0        0    18221 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/configUtils.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/declarations.d.ts
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/icons.ts
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/index.ts
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/rendererUtils.tsx
+-rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/selectColumn.tsx
+-rw-r--r--   0        0        0     4515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/selectColumns.tsx
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/selectRegular.tsx
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
+-rw-r--r--   0        0        0     9992 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/transferData.tsx
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/base.css
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/index.js
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/crosshair-16.svg
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/minus-16.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/play-16.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/play-circle-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/plus-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/plus-24.svg
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/search-16.svg
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/search-24.svg
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/settings-16.svg
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/settings-24.svg
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/trash-16.svg
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/trash-24.svg
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/x-16.svg
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/x-square-16.svg
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/install.json
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/package.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/pipeline-16.svg
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/pipeline-24.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/tailwind.config.js
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/tsconfig.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/schema/extension.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/schema/plugin copy.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/schema/plugin.json
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/src/Dropzone.tsx
+-rw-r--r--   0        0        0    18461 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/src/PipelineEditorWidget.tsx
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/src/customEdge.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/src/declarations.d.ts
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/src/icons.ts
+-rw-r--r--   0        0        0    17975 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/src/index.ts
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/canvas.css
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/index.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/index.js
+-rw-r--r--   0        0        0    21779 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/output.css
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/pipeline-category-icon.svg
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/react-icon.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/tailwinds_preflight.css
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/icons/api-24.svg
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/icons/file-plus-24.svg
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/icons/file-text-24.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/icons/monitor-24.svg
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/.gitignore
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/README.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.2/PKG-INFO
```

### Comparing `jupyterlab_amphi-0.2.1/output.json` & `jupyterlab_amphi-0.2.2/output.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/package.json` & `jupyterlab_amphi-0.2.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -66,15 +66,15 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.yaml}\"",
         "prettier:check": "jlpm prettier:base --check",
         "quickstart": "npm run setup:py && jlpm && jlpm deduplicate && jlpm clean:all && jlpm lint && jlpm build:prod && jlpm dist && jlpm docs && jlpm test",
         "setup:py": "python -m pip install -e \".[dev,lint,test,docs]\"",
         "test": "jlpm test:py",
         "test:py": "pytest"
     },
-    "version": "0.2.1",
+    "version": "0.2.2",
     "workspaces": {
         "packages": [
             "packages/pipeline-editor",
             "packages/pipeline-components-manager",
             "packages/pipeline-components-core",
             "packages/pipeline-console",
             "packages/pipeline-metadata-panel"
```

### Comparing `jupyterlab_amphi-0.2.1/tsconfigbase.json` & `jupyterlab_amphi-0.2.2/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/package.json` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.9e880e90f12441f9cd92.js'}}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -39,15 +39,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.f28dd63fd7611d76a5b4.js",
+            "load": "static/remoteEntry.9e880e90f12441f9cd92.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-core",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
@@ -83,9 +83,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/static/354.17f2b6e853bc242211f3.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/static/354.17f2b6e853bc242211f3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/static/432.df81fd96e756f14c54d0.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/static/432.df81fd96e756f14c54d0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/static/713.a7e0851307239af436d3.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/static/713.a7e0851307239af436d3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/static/713.a7e0851307239af436d3.js.LICENSE.txt` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/static/713.a7e0851307239af436d3.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/static/remoteEntry.f28dd63fd7611d76a5b4.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/static/remoteEntry.9e880e90f12441f9cd92.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -113,15 +113,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@amphi/pipeline-components-core", "0.2.1", (() => Promise.all([P.e(345), P.e(354)]).then((() => () => P(354))))), l("reactflow", "11.7.2", (() => Promise.all([P.e(713), P.e(345), P.e(628)]).then((() => () => P(713)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@amphi/pipeline-components-core", "0.2.2", (() => Promise.all([P.e(345), P.e(354)]).then((() => () => P(354))))), l("reactflow", "11.7.2", (() => Promise.all([P.e(713), P.e(345), P.e(628)]).then((() => () => P(713)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-core/static/third-party-licenses.json` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-core/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.eefc39996b3e8a655b2e.js'}}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -44,15 +44,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.34ddf437229e19983422.js",
+            "load": "static/remoteEntry.eefc39996b3e8a655b2e.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-manager",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundle": false,
@@ -93,9 +93,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/143.c7653d290fba1605b212.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/143.c7653d290fba1605b212.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/37.77034b0c839d0f88327f.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/37.49e35d770e38d792a11d.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 37.77034b0c839d0f88327f.js.LICENSE.txt */
+/*! For license information please see 37.49e35d770e38d792a11d.js.LICENSE.txt */
 (self.webpackChunk_amphi_pipeline_components_manager = self.webpackChunk_amphi_pipeline_components_manager || []).push([
     [37], {
         7037: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 Affix: () => Vo,
                 Alert: () => yi,
@@ -895,23 +895,24 @@
                 return _e.has(t) || _e.set(t, new We(t)), _e.get(t)
             }
             var Ke = new WeakMap,
                 Xe = {},
                 qe = new WeakMap;
 
             function Ge(e) {
-                var t = qe.get(e) || "";
-                return t || (Object.keys(e).forEach((function(n) {
-                    var o = e[n];
-                    t += n, o instanceof We ? t += o.id : o && "object" === (0, p.A)(o) ? t += Ge(o) : t += o
-                })), qe.set(e, t)), t
+                var t = arguments.length > 1 && void 0 !== arguments[1] && arguments[1],
+                    n = qe.get(e) || "";
+                return n || (Object.keys(e).forEach((function(o) {
+                    var r = e[o];
+                    n += o, r instanceof We ? n += r.id : r && "object" === (0, p.A)(r) ? n += Ge(r, t) : n += r
+                })), t && (n = Oe(n)), qe.set(e, n)), n
             }
 
             function Ye(e, t) {
-                return Oe("".concat(t, "_").concat(Ge(e)))
+                return Oe("".concat(t, "_").concat(Ge(e, !0)))
             }
             "random-".concat(Date.now(), "-").concat(Math.random()).replace(/\./g, "");
             var Ue = (0, De.A)();
 
             function Qe(e) {
                 return "number" == typeof e ? "".concat(e, "px") : e
             }
@@ -14953,61 +14954,108 @@
                     E = e.onScroll,
                     k = e.onVirtualScroll,
                     O = e.onVisibleChange,
                     A = e.innerProps,
                     I = e.extraRender,
                     N = e.styles,
                     M = (0, ir.A)(e, $m),
-                    j = !(!1 === C || !c || !s),
-                    P = j && v && (s * v.length > c || !!$),
-                    R = "rtl" === x,
-                    z = a()(r, (0, Ee.A)({}, "".concat(r, "-rtl"), R), i),
-                    T = v || wm,
-                    H = (0, o.useRef)(),
-                    B = (0, o.useRef)(),
-                    D = (0, o.useState)(0),
-                    L = (0, ke.A)(D, 2),
-                    F = L[0],
-                    W = L[1],
-                    _ = (0, o.useState)(0),
-                    V = (0, ke.A)(_, 2),
-                    K = V[0],
-                    X = V[1],
-                    q = (0, o.useState)(!1),
+                    j = o.useCallback((function(e) {
+                        return "function" == typeof y ? y(e) : null == e ? void 0 : e[y]
+                    }), [y]),
+                    P = function(e, t, n) {
+                        var r = o.useState(0),
+                            i = (0, ke.A)(r, 2),
+                            a = i[0],
+                            l = i[1],
+                            c = (0, o.useRef)(new Map),
+                            s = (0, o.useRef)(new hm),
+                            u = (0, o.useRef)();
+
+                        function d() {
+                            Ce.cancel(u.current)
+                        }
+
+                        function p() {
+                            var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
+                            d();
+                            var t = function() {
+                                c.current.forEach((function(e, t) {
+                                    if (e && e.offsetParent) {
+                                        var n = h(e),
+                                            o = n.offsetHeight;
+                                        s.current.get(t) !== o && s.current.set(t, n.offsetHeight)
+                                    }
+                                })), l((function(e) {
+                                    return e + 1
+                                }))
+                            };
+                            e ? t() : u.current = Ce(t)
+                        }
+                        return (0, o.useEffect)((function() {
+                            return d
+                        }), []), [function(t, n) {
+                            var o = e(t);
+                            c.current.get(o);
+                            n ? (c.current.set(o, n), p()) : c.current.delete(o)
+                        }, p, s.current, a]
+                    }(j),
+                    R = (0, ke.A)(P, 4),
+                    z = R[0],
+                    T = R[1],
+                    H = R[2],
+                    B = R[3],
+                    D = !(!1 === C || !c || !s),
+                    L = o.useMemo((function() {
+                        return Object.values(H.maps).reduce((function(e, t) {
+                            return e + t
+                        }), 0)
+                    }), [H.id, H.maps]),
+                    F = D && v && (Math.max(s * v.length, L) > c || !!$),
+                    W = "rtl" === x,
+                    _ = a()(r, (0, Ee.A)({}, "".concat(r, "-rtl"), W), i),
+                    V = v || wm,
+                    K = (0, o.useRef)(),
+                    X = (0, o.useRef)(),
+                    q = (0, o.useState)(0),
                     G = (0, ke.A)(q, 2),
                     Y = G[0],
                     U = G[1],
-                    Q = function() {
-                        U(!0)
+                    Q = (0, o.useState)(0),
+                    Z = (0, ke.A)(Q, 2),
+                    J = Z[0],
+                    ee = Z[1],
+                    te = (0, o.useState)(!1),
+                    ne = (0, ke.A)(te, 2),
+                    oe = ne[0],
+                    re = ne[1],
+                    ie = function() {
+                        re(!0)
                     },
-                    Z = function() {
-                        U(!1)
+                    ae = function() {
+                        re(!1)
                     },
-                    J = o.useCallback((function(e) {
-                        return "function" == typeof y ? y(e) : null == e ? void 0 : e[y]
-                    }), [y]),
-                    ee = {
-                        getKey: J
+                    le = {
+                        getKey: j
                     };
 
-                function te(e) {
-                    W((function(t) {
+                function se(e) {
+                    U((function(t) {
                         var n = function(e) {
                             var t = e;
-                            return Number.isNaN(Ne.current) || (t = Math.min(t, Ne.current)), t = Math.max(t, 0)
+                            return Number.isNaN(Me.current) || (t = Math.min(t, Me.current)), t = Math.max(t, 0)
                         }("function" == typeof e ? e(t) : e);
-                        return H.current.scrollTop = n, n
+                        return K.current.scrollTop = n, n
                     }))
                 }
-                var ne = (0, o.useRef)({
+                var ue = (0, o.useRef)({
                         start: 0,
-                        end: T.length
+                        end: V.length
                     }),
-                    oe = (0, o.useRef)(),
-                    re = function(e, t, n) {
+                    de = (0, o.useRef)(),
+                    pe = function(e, t, n) {
                         var r = o.useState(e),
                             i = (0, ke.A)(r, 2),
                             a = i[0],
                             l = i[1],
                             c = o.useState(null),
                             s = (0, ke.A)(c, 2),
                             u = s[0],
@@ -15035,148 +15083,106 @@
                                 return null === s ? null : {
                                     index: s,
                                     multiple: u
                                 }
                             }(a || [], e || [], t);
                             void 0 !== (null == o ? void 0 : o.index) && (null == n || n(o.index), d(e[o.index])), l(e)
                         }), [e]), [u]
-                    }(T, J),
-                    ie = (0, ke.A)(re, 1)[0];
-                oe.current = ie;
-                var ae = function(e, t, n) {
-                        var r = o.useState(0),
-                            i = (0, ke.A)(r, 2),
-                            a = i[0],
-                            l = i[1],
-                            c = (0, o.useRef)(new Map),
-                            s = (0, o.useRef)(new hm),
-                            u = (0, o.useRef)();
-
-                        function d() {
-                            Ce.cancel(u.current)
-                        }
-
-                        function p() {
-                            var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
-                            d();
-                            var t = function() {
-                                c.current.forEach((function(e, t) {
-                                    if (e && e.offsetParent) {
-                                        var n = h(e),
-                                            o = n.offsetHeight;
-                                        s.current.get(t) !== o && s.current.set(t, n.offsetHeight)
-                                    }
-                                })), l((function(e) {
-                                    return e + 1
-                                }))
-                            };
-                            e ? t() : u.current = Ce(t)
-                        }
-                        return (0, o.useEffect)((function() {
-                            return d
-                        }), []), [function(t, n) {
-                            var o = e(t);
-                            c.current.get(o);
-                            n ? (c.current.set(o, n), p()) : c.current.delete(o)
-                        }, p, s.current, a]
-                    }(J),
-                    le = (0, ke.A)(ae, 4),
-                    se = le[0],
-                    ue = le[1],
-                    de = le[2],
-                    pe = le[3],
-                    fe = o.useMemo((function() {
-                        if (!j) return {
+                    }(V, j),
+                    fe = (0, ke.A)(pe, 1)[0];
+                de.current = fe;
+                var me = o.useMemo((function() {
+                        if (!D) return {
                             scrollHeight: void 0,
                             start: 0,
-                            end: T.length - 1,
+                            end: V.length - 1,
                             offset: void 0
                         };
                         var e;
-                        if (!P) return {
-                            scrollHeight: (null === (e = B.current) || void 0 === e ? void 0 : e.offsetHeight) || 0,
+                        if (!F) return {
+                            scrollHeight: (null === (e = X.current) || void 0 === e ? void 0 : e.offsetHeight) || 0,
                             start: 0,
-                            end: T.length - 1,
+                            end: V.length - 1,
                             offset: void 0
                         };
-                        for (var t, n, o, r = 0, i = T.length, a = 0; a < i; a += 1) {
-                            var l = T[a],
-                                u = J(l),
-                                d = de.get(u),
+                        for (var t, n, o, r = 0, i = V.length, a = 0; a < i; a += 1) {
+                            var l = V[a],
+                                u = j(l),
+                                d = H.get(u),
                                 p = r + (void 0 === d ? s : d);
-                            p >= F && void 0 === t && (t = a, n = r), p > F + c && void 0 === o && (o = a), r = p
+                            p >= Y && void 0 === t && (t = a, n = r), p > Y + c && void 0 === o && (o = a), r = p
                         }
-                        return void 0 === t && (t = 0, n = 0, o = Math.ceil(c / s)), void 0 === o && (o = T.length - 1), {
+                        return void 0 === t && (t = 0, n = 0, o = Math.ceil(c / s)), void 0 === o && (o = V.length - 1), {
                             scrollHeight: r,
                             start: t,
-                            end: o = Math.min(o + 1, T.length - 1),
+                            end: o = Math.min(o + 1, V.length - 1),
                             offset: n
                         }
-                    }), [P, j, F, T, pe, c]),
-                    me = fe.scrollHeight,
-                    ge = fe.start,
-                    he = fe.end,
-                    ve = fe.offset;
-                ne.current.start = ge, ne.current.end = he;
-                var be = o.useState({
+                    }), [F, D, Y, V, B, c]),
+                    ge = me.scrollHeight,
+                    he = me.start,
+                    ve = me.end,
+                    be = me.offset;
+                ue.current.start = he, ue.current.end = ve;
+                var ye = o.useState({
                         width: 0,
                         height: c
                     }),
-                    ye = (0, ke.A)(be, 2),
-                    xe = ye[0],
-                    $e = ye[1],
-                    we = (0, o.useRef)(),
+                    xe = (0, ke.A)(ye, 2),
+                    $e = xe[0],
+                    we = xe[1],
                     Se = (0, o.useRef)(),
-                    Oe = o.useMemo((function() {
-                        return xm(xe.width, $)
-                    }), [xe.width, $]),
+                    Oe = (0, o.useRef)(),
                     Ae = o.useMemo((function() {
-                        return xm(xe.height, me)
-                    }), [xe.height, me]),
-                    Ie = me - c,
-                    Ne = (0, o.useRef)(Ie);
-                Ne.current = Ie;
-                var Me = F <= 0,
-                    je = F >= Ie,
-                    Pe = bm(Me, je),
-                    Re = function() {
+                        return xm($e.width, $)
+                    }), [$e.width, $]),
+                    Ie = o.useMemo((function() {
+                        return xm($e.height, ge)
+                    }), [$e.height, ge]),
+                    Ne = ge - c,
+                    Me = (0, o.useRef)(Ne);
+                Me.current = Ne;
+                var je = Y <= 0,
+                    Pe = Y >= Ne,
+                    Re = bm(je, Pe),
+                    ze = function() {
                         return {
-                            x: R ? -K : K,
-                            y: F
+                            x: W ? -J : J,
+                            y: Y
                         }
                     },
-                    ze = (0, o.useRef)(Re()),
-                    Te = wn((function() {
+                    Te = (0, o.useRef)(ze()),
+                    He = wn((function() {
                         if (k) {
-                            var e = Re();
-                            ze.current.x === e.x && ze.current.y === e.y || (k(e), ze.current = e)
+                            var e = ze();
+                            Te.current.x === e.x && Te.current.y === e.y || (k(e), Te.current = e)
                         }
                     }));
 
-                function He(e, t) {
+                function Be(e, t) {
                     var n = e;
                     t ? ((0, f.flushSync)((function() {
-                        X(n)
-                    })), Te()) : te(n)
+                        ee(n)
+                    })), He()) : se(n)
                 }
-                var Be = function(e) {
+                var De = function(e) {
                         var t = e,
-                            n = $ - xe.width;
+                            n = $ ? $ - $e.width : 0;
                         return t = Math.max(t, 0), Math.min(t, n)
                     },
-                    De = wn((function(e, t) {
+                    Le = wn((function(e, t) {
                         t ? ((0, f.flushSync)((function() {
-                            X((function(t) {
-                                return Be(t + (R ? -e : e))
+                            ee((function(t) {
+                                return De(t + (W ? -e : e))
                             }))
-                        })), Te()) : te((function(t) {
+                        })), He()) : se((function(t) {
                             return t + e
                         }))
                     })),
-                    Le = function(e, t, n, r, i) {
+                    Fe = function(e, t, n, r, i) {
                         var a = (0, o.useRef)(0),
                             l = (0, o.useRef)(null),
                             c = (0, o.useRef)(null),
                             s = (0, o.useRef)(!1),
                             u = bm(t, n),
                             d = (0, o.useRef)(null),
                             p = (0, o.useRef)(null);
@@ -15201,18 +15207,18 @@
                                 }(t, g) : function(e, t) {
                                     i(t, !0), vm || e.preventDefault()
                                 }(t, m)
                             }
                         }, function(t) {
                             e && (s.current = t.detail === c.current)
                         }]
-                    }(j, Me, je, !!$, De),
-                    Fe = (0, ke.A)(Le, 2),
-                    We = Fe[0],
-                    _e = Fe[1];
+                    }(D, je, Pe, !!$, Le),
+                    We = (0, ke.A)(Fe, 2),
+                    _e = We[0],
+                    Ve = We[1];
                 ! function(e, t, n) {
                     var r, i = (0, o.useRef)(!1),
                         a = (0, o.useRef)(0),
                         l = (0, o.useRef)(null),
                         c = (0, o.useRef)(null),
                         s = function(e) {
                             if (i.current) {
@@ -15234,38 +15240,38 @@
                     }, it((function() {
                         return e && t.current.addEventListener("touchstart", d),
                             function() {
                                 var e;
                                 null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", d), r(), clearInterval(c.current)
                             }
                     }), [e])
-                }(j, H, (function(e, t) {
-                    return !Pe(e, t) && (We({
+                }(D, K, (function(e, t) {
+                    return !Re(e, t) && (_e({
                         preventDefault: function() {},
                         deltaY: e
                     }), !0)
                 })), it((function() {
                     function e(e) {
-                        j && e.preventDefault()
+                        D && e.preventDefault()
                     }
-                    var t = H.current;
-                    return t.addEventListener("wheel", We), t.addEventListener("DOMMouseScroll", _e), t.addEventListener("MozMousePixelScroll", e),
+                    var t = K.current;
+                    return t.addEventListener("wheel", _e), t.addEventListener("DOMMouseScroll", Ve), t.addEventListener("MozMousePixelScroll", e),
                         function() {
-                            t.removeEventListener("wheel", We), t.removeEventListener("DOMMouseScroll", _e), t.removeEventListener("MozMousePixelScroll", e)
+                            t.removeEventListener("wheel", _e), t.removeEventListener("DOMMouseScroll", Ve), t.removeEventListener("MozMousePixelScroll", e)
                         }
-                }), [j]), it((function() {
-                    $ && X((function(e) {
-                        return Be(e)
+                }), [D]), it((function() {
+                    $ && ee((function(e) {
+                        return De(e)
                     }))
-                }), [xe.width, $]);
-                var Ve = function() {
+                }), [$e.width, $]);
+                var Ke = function() {
                         var e, t;
-                        null === (e = we.current) || void 0 === e || e.delayHidden(), null === (t = Se.current) || void 0 === t || t.delayHidden()
+                        null === (e = Se.current) || void 0 === e || e.delayHidden(), null === (t = Oe.current) || void 0 === t || t.delayHidden()
                     },
-                    Ke = function(e, t, n, r, i, a, l, c) {
+                    Xe = function(e, t, n, r, i, a, l, c) {
                         var s = o.useRef(),
                             u = o.useState(null),
                             f = (0, ke.A)(u, 2),
                             m = f[0],
                             g = f[1];
                         return it((function() {
                                 if (m && m.times < 10) {
@@ -15331,32 +15337,32 @@
                                             index: n,
                                             offset: void 0 === r ? 0 : r,
                                             originAlign: o
                                         })
                                     }
                                 } else c()
                             }
-                    }(H, T, de, s, J, (function() {
-                        return ue(!0)
-                    }), te, Ve);
+                    }(K, V, H, s, j, (function() {
+                        return T(!0)
+                    }), se, Ke);
                 o.useImperativeHandle(t, (function() {
                     return {
-                        getScrollInfo: Re,
+                        getScrollInfo: ze,
                         scrollTo: function(e) {
                             var t;
-                            (t = e) && "object" === (0, p.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && X(Be(e.left)), Ke(e.top)) : Ke(e)
+                            (t = e) && "object" === (0, p.A)(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && ee(De(e.left)), Xe(e.top)) : Xe(e)
                         }
                     }
                 })), it((function() {
                     if (O) {
-                        var e = T.slice(ge, he + 1);
-                        O(e, T)
+                        var e = V.slice(he, ve + 1);
+                        O(e, V)
                     }
-                }), [ge, he, T]);
-                var Xe = function(e, t, n, r) {
+                }), [he, ve, V]);
+                var qe = function(e, t, n, r) {
                         var i = o.useMemo((function() {
                                 return [new Map, []]
                             }), [e, n.id, r]),
                             a = (0, ke.A)(i, 2),
                             l = a[0],
                             c = a[1];
                         return function(o) {
@@ -15372,25 +15378,25 @@
                                     if (c[d] = (c[d - 1] || 0) + g, m === o && (a = d), m === i && (s = d), void 0 !== a && void 0 !== s) break
                                 }
                             return {
                                 top: c[a - 1] || 0,
                                 bottom: c[s]
                             }
                         }
-                    }(T, J, de, s),
-                    qe = null == I ? void 0 : I({
-                        start: ge,
-                        end: he,
-                        virtual: P,
-                        offsetX: K,
-                        offsetY: ve,
-                        rtl: R,
-                        getSize: Xe
+                    }(V, j, H, s),
+                    Ge = null == I ? void 0 : I({
+                        start: he,
+                        end: ve,
+                        virtual: F,
+                        offsetX: J,
+                        offsetY: be,
+                        rtl: W,
+                        getSize: qe
                     }),
-                    Ge = function(e, t, n, r, i, a, l) {
+                    Ye = function(e, t, n, r, i, a, l) {
                         var c = l.getKey;
                         return e.slice(t, n + 1).map((function(e, n) {
                             var l = a(e, t + n, {
                                     style: {
                                         width: r
                                     }
                                 }),
@@ -15398,74 +15404,74 @@
                             return o.createElement(gm, {
                                 key: s,
                                 setRef: function(t) {
                                     return i(e, t)
                                 }
                             }, l)
                         }))
-                    }(T, ge, he, $, se, b, ee),
-                    Ye = null;
-                c && (Ye = (0, d.A)((0, Ee.A)({}, m ? "height" : "maxHeight", c), Sm), j && (Ye.overflowY = "hidden", $ && (Ye.overflowX = "hidden"), Y && (Ye.pointerEvents = "none")));
-                var Ue = {};
-                return R && (Ue.dir = "rtl"), o.createElement("div", (0, l.A)({
+                    }(V, he, ve, $, z, b, le),
+                    Ue = null;
+                c && (Ue = (0, d.A)((0, Ee.A)({}, m ? "height" : "maxHeight", c), Sm), D && (Ue.overflowY = "hidden", $ && (Ue.overflowX = "hidden"), oe && (Ue.pointerEvents = "none")));
+                var Qe = {};
+                return W && (Qe.dir = "rtl"), o.createElement("div", (0, l.A)({
                     style: (0, d.A)((0, d.A)({}, g), {}, {
                         position: "relative"
                     }),
-                    className: z
-                }, Ue, M), o.createElement(ce, {
+                    className: _
+                }, Qe, M), o.createElement(ce, {
                     onResize: function(e) {
-                        $e({
+                        we({
                             width: e.width || e.offsetWidth,
                             height: e.height || e.offsetHeight
                         })
                     }
                 }, o.createElement(S, {
                     className: "".concat(r, "-holder"),
-                    style: Ye,
-                    ref: H,
+                    style: Ue,
+                    ref: K,
                     onScroll: function(e) {
                         var t = e.currentTarget.scrollTop;
-                        t !== F && te(t), null == E || E(e), Te()
+                        t !== Y && se(t), null == E || E(e), He()
                     },
-                    onMouseEnter: Ve
+                    onMouseEnter: Ke
                 }, o.createElement(dm, {
                     prefixCls: r,
-                    height: me,
-                    offsetX: K,
-                    offsetY: ve,
+                    height: ge,
+                    offsetX: J,
+                    offsetY: be,
                     scrollWidth: $,
-                    onInnerResize: ue,
-                    ref: B,
+                    onInnerResize: T,
+                    ref: X,
                     innerProps: A,
-                    rtl: R,
-                    extra: qe
-                }, Ge))), P && me > c && o.createElement(mm, {
-                    ref: we,
+                    rtl: W,
+                    extra: Ge
+                }, Ye))), F && ge > c && o.createElement(mm, {
+                    ref: Se,
                     prefixCls: r,
-                    scrollOffset: F,
-                    scrollRange: me,
-                    rtl: R,
-                    onScroll: He,
-                    onStartMove: Q,
-                    onStopMove: Z,
-                    spinSize: Ae,
-                    containerSize: xe.height,
+                    scrollOffset: Y,
+                    scrollRange: ge,
+                    rtl: W,
+                    onScroll: Be,
+                    onStartMove: ie,
+                    onStopMove: ae,
+                    spinSize: Ie,
+                    containerSize: $e.height,
                     style: null == N ? void 0 : N.verticalScrollBar,
                     thumbStyle: null == N ? void 0 : N.verticalScrollBarThumb
-                }), P && $ > xe.width && o.createElement(mm, {
-                    ref: Se,
+                }), F && $ > $e.width && o.createElement(mm, {
+                    ref: Oe,
                     prefixCls: r,
-                    scrollOffset: K,
+                    scrollOffset: J,
                     scrollRange: $,
-                    rtl: R,
-                    onScroll: He,
-                    onStartMove: Q,
-                    onStopMove: Z,
-                    spinSize: Oe,
-                    containerSize: xe.width,
+                    rtl: W,
+                    onScroll: Be,
+                    onStartMove: ie,
+                    onStopMove: ae,
+                    spinSize: Ae,
+                    containerSize: $e.width,
                     horizontal: !0,
                     style: null == N ? void 0 : N.horizontalScrollBar,
                     thumbStyle: null == N ? void 0 : N.horizontalScrollBarThumb
                 }))
             }
             var km = o.forwardRef(Em);
             km.displayName = "List";
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/37.77034b0c839d0f88327f.js.LICENSE.txt` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/37.49e35d770e38d792a11d.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/379.1427c0520c9ac5a71632.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/379.1427c0520c9ac5a71632.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/379.1427c0520c9ac5a71632.js.LICENSE.txt` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/379.1427c0520c9ac5a71632.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/432.5fd4f051d4b18df45075.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/432.5fd4f051d4b18df45075.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/719.3c5804917b7a839b516d.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/719.c9d87c8fac95544e1714.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -623,15 +623,15 @@
                         "ok" == e.content.status ? t.sessionContext.session.kernel.requestExecute({
                             code: "print(_amphi_metadatapanel_getcontentof(" + m + "))"
                         }).onIOPub = e => {
                             if ("stream" === e.header.msg_type) {
                                 const t = e;
                                 console.log("receive stream %o", t);
                                 const n = t.content.text,
-                                    a = /(\w+)\s+\(([^,]+),\s*(named|unnamed)\)/g,
+                                    a = /([^\s,]+)\s+\(([^,]+),\s*(named|unnamed)\)/g,
                                     r = [];
                                 let i;
                                 for (; null !== (i = a.exec(n));) {
                                     const [e, t, n, a] = i;
                                     r.push({
                                         value: t,
                                         label: t,
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/remoteEntry.34ddf437229e19983422.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/remoteEntry.eefc39996b3e8a655b2e.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, l, u, c, f, d, s, p, h, m, v, b, g, y, w = {
+    var e, r, t, a, n, o, i, l, f, u, d, c, s, p, h, m, v, b, g, y, w = {
             5548: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(143), t.e(379), t.e(345), t.e(628), t.e(719)]).then((() => () => t(7719))),
                         "./extension": () => Promise.all([t.e(143), t.e(379), t.e(345), t.e(628), t.e(719)]).then((() => () => t(7719))),
                         "./style": () => t.e(432).then((() => () => t(1432)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -44,64 +44,64 @@
     }, P.d = (e, r) => {
         for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
         12: "e1b4412a18535c560cd1",
-        37: "77034b0c839d0f88327f",
+        37: "49e35d770e38d792a11d",
         85: "227e3aea03a3014cd80a",
         143: "c7653d290fba1605b212",
         345: "3292eea9d7af2efbde78",
         379: "1427c0520c9ac5a71632",
         432: "5fd4f051d4b18df45075",
         454: "b60aaa09eed0e7e4a124",
         628: "9846ca5c6c20882d89fe",
-        719: "3c5804917b7a839b516d"
+        719: "c9d87c8fac95544e1714"
     } [e] + ".js?v=" + {
         12: "e1b4412a18535c560cd1",
-        37: "77034b0c839d0f88327f",
+        37: "49e35d770e38d792a11d",
         85: "227e3aea03a3014cd80a",
         143: "c7653d290fba1605b212",
         345: "3292eea9d7af2efbde78",
         379: "1427c0520c9ac5a71632",
         432: "5fd4f051d4b18df45075",
         454: "b60aaa09eed0e7e4a124",
         628: "9846ca5c6c20882d89fe",
-        719: "3c5804917b7a839b516d"
+        719: "c9d87c8fac95544e1714"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), P.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-components-manager:", P.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var i, l;
             if (void 0 !== n)
-                for (var u = document.getElementsByTagName("script"), c = 0; c < u.length; c++) {
-                    var f = u[c];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
-                        i = f;
+                for (var f = document.getElementsByTagName("script"), u = 0; u < f.length; u++) {
+                    var d = f[u];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
+                        i = d;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
-            var d = (r, a) => {
+            var c = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(s);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                s = setTimeout(d.bind(null, void 0, {
+                s = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, P.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -122,16 +122,16 @@
                             l = n[r];
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
-                    u = [];
-                return "default" === t && (l("@amphi/pipeline-components-manager", "0.2.1", (() => Promise.all([P.e(143), P.e(379), P.e(345), P.e(628), P.e(719)]).then((() => () => P(7719))))), l("antd", "5.16.2", (() => Promise.all([P.e(37), P.e(143), P.e(345), P.e(628)]).then((() => () => P(7037))))), l("react-dnd-html5-backend", "16.0.1", (() => P.e(454).then((() => () => P(6454))))), l("react-dnd", "16.0.1", (() => Promise.all([P.e(12), P.e(345), P.e(85)]).then((() => () => P(4631)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    f = [];
+                return "default" === t && (l("@amphi/pipeline-components-manager", "0.2.2", (() => Promise.all([P.e(143), P.e(379), P.e(345), P.e(628), P.e(719)]).then((() => () => P(7719))))), l("antd", "5.16.2", (() => Promise.all([P.e(37), P.e(143), P.e(345), P.e(628)]).then((() => () => P(7037))))), l("react-dnd-html5-backend", "16.0.1", (() => P.e(454).then((() => () => P(6454))))), l("react-dnd", "16.0.1", (() => Promise.all([P.e(12), P.e(345), P.e(85)]).then((() => () => P(4631)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -167,47 +167,47 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
             return t
         }
         var i = [];
         for (o = 1; o < e.length; o++) {
             var l = e[o];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : n(l))
+            i.push(0 === l ? "not(" + f() + ")" : 1 === l ? "(" + f() + " || " + f() + ")" : 2 === l ? i.pop() + " " + i.pop() : n(l))
         }
-        return u();
+        return f();
 
-        function u() {
+        function f() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
-            for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var c, f, d = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (f = (typeof(c = r[i]))[0])) return !u || ("u" == d ? l > a && !n : "" == d != n);
-                if ("u" == f) {
-                    if (!u || "u" != d) return !1
-                } else if (u)
-                    if (d == f)
+            for (var i = 0, l = 1, f = !0;; l++, i++) {
+                var u, d, c = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(u = r[i]))[0])) return !f || ("u" == c ? l > a && !n : "" == c != n);
+                if ("u" == d) {
+                    if (!f || "u" != c) return !1
+                } else if (f)
+                    if (c == d)
                         if (l <= a) {
-                            if (c != e[l]) return !1
+                            if (u != e[l]) return !1
                         } else {
-                            if (n ? c > e[l] : c < e[l]) return !1;
-                            c != e[l] && (u = !1)
+                            if (n ? u > e[l] : u < e[l]) return !1;
+                            u != e[l] && (f = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != c && "n" != c) {
                     if (n || l <= a) return !1;
-                    u = !1, l--
+                    f = !1, l--
                 } else {
-                    if (l <= a || f < d != n) return !1;
-                    u = !1
-                } else "s" != d && "n" != d && (u = !1, l--)
+                    if (l <= a || d < c != n) return !1;
+                    f = !1
+                } else "s" != c && "n" != c && (f = !1, l--)
             }
         }
         var s = [],
             p = s.pop.bind(s);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
@@ -216,27 +216,27 @@
     }, i = (e, r) => {
         var t = P.S[e];
         if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", c = (e, r, t, a) => {
+    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", u = (e, r, t, a) => {
         var n = l(e, t);
-        return o(a, n) || d(u(e, t, n, a)), s(e[t][n])
-    }, f = (e, r, t) => {
+        return o(a, n) || c(f(e, t, n, a)), s(e[t][n])
+    }, d = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, d = e => {
+    }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, s = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
         var o = P.I(r);
         return o && o.then ? o.then(e.bind(e, r, P.S[r], t, a, n)) : e(r, P.S[r], t, a, n)
-    })(((e, r, t, a) => (i(e, t), c(r, 0, t, a)))), m = p(((e, r, t, a, n) => {
-        var o = r && P.o(r, t) && f(r, t, a);
+    })(((e, r, t, a) => (i(e, t), u(r, 0, t, a)))), m = p(((e, r, t, a, n) => {
+        var o = r && P.o(r, t) && d(r, t, a);
         return o ? s(o) : n()
     })), v = {}, b = {
         3345: () => h("default", "react", [1, 18, 2, 0]),
         7628: () => h("default", "react-dom", [1, 18, 2, 0]),
         1029: () => m("default", "react-dnd-html5-backend", [1, 16, 0, 1], (() => P.e(454).then((() => () => P(6454))))),
         2283: () => m("default", "antd", [1, 5, 16, 0], (() => P.e(37).then((() => () => P(7037))))),
         5256: () => h("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
@@ -294,20 +294,20 @@
                         i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", i.name = "ChunkLoadError", i.type = n, i.request = o, a[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
                 var a, n, [o, i, l] = t,
-                    u = 0;
+                    f = 0;
                 if (o.some((r => 0 !== e[r]))) {
                     for (a in i) P.o(i, a) && (P.m[a] = i[a]);
                     l && l(P)
                 }
-                for (r && r(t); u < o.length; u++) n = o[u], P.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); f < o.length; f++) n = o[f], P.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amphi_pipeline_components_manager = self.webpackChunk_amphi_pipeline_components_manager || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), P.nc = void 0;
     var E = P(5548);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amphi/pipeline-components-manager"] = E
 })();
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-components-manager/static/third-party-licenses.json` & `jupyterlab_amphi-0.2.2/amphi/pipeline-components-manager/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986263736263736%*

 * *Differences: {"'packages'": "{1: {'versionInfo': '1.20.0'}, 76: {'versionInfo': '3.11.5'}}"}*

```diff
@@ -6,15 +6,15 @@
             "name": "@ant-design/colors",
             "versionInfo": "7.0.2"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2019-present afc163\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the \"Software\"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@ant-design/cssinjs",
-            "versionInfo": "1.19.1"
+            "versionInfo": "1.20.0"
         },
         {
             "extractedText": "MIT LICENSE\n\nCopyright (c) 2018-present Ant UED, https://xtech.antfin.com/\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@ant-design/icons",
             "versionInfo": "5.3.6"
         },
@@ -456,15 +456,15 @@
             "name": "rc-util",
             "versionInfo": "5.39.1"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-virtual-list",
-            "versionInfo": "3.11.4"
+            "versionInfo": "3.11.5"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react",
             "versionInfo": "18.2.0"
         },
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-editor/package.json` & `jupyterlab_amphi-0.2.2/amphi/pipeline-editor/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.90789c29a44dad669aa0.js'}}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -46,15 +46,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.44274364debca46ec439.js",
+            "load": "static/remoteEntry.90789c29a44dad669aa0.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-editor",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
@@ -102,9 +102,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/121.db61795daabb4d1eb7c3.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/121.db61795daabb4d1eb7c3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/219.2f775af86603225cd107.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/219.2f775af86603225cd107.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/285.4eef7e98cbfad514e073.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/285.4eef7e98cbfad514e073.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/285.4eef7e98cbfad514e073.js.LICENSE.txt` & `jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/285.4eef7e98cbfad514e073.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/550.c5bd7757f7228cea68ce.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/550.c5bd7757f7228cea68ce.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/636.e37faa04eb8cb39edd7f.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/636.18742a3929885dfb4bfa.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 636.e37faa04eb8cb39edd7f.js.LICENSE.txt */
+/*! For license information please see 636.18742a3929885dfb4bfa.js.LICENSE.txt */
 (self.webpackChunk_amphi_pipeline_editor = self.webpackChunk_amphi_pipeline_editor || []).push([
     [636], {
         845: (e, t, n) => {
             "use strict";
 
             function r() {
                 return r = Object.assign ? Object.assign.bind() : function(e) {
@@ -1204,58 +1204,104 @@
                     k = e.onScroll,
                     S = e.onVirtualScroll,
                     C = e.onVisibleChange,
                     _ = e.innerProps,
                     M = e.extraRender,
                     N = e.styles,
                     O = j(e, Qe),
-                    A = !(!1 === y || !l || !u),
-                    T = A && h && (u * h.length > l || !!b),
-                    K = "rtl" === m,
-                    D = E()(i, a({}, "".concat(i, "-rtl"), K), c),
-                    R = h || Ze,
-                    L = (0, P.useRef)(),
-                    I = (0, P.useRef)(),
-                    H = $((0, P.useState)(0), 2),
-                    z = H[0],
-                    B = H[1],
-                    F = $((0, P.useState)(0), 2),
-                    X = F[0],
-                    G = F[1],
-                    q = $((0, P.useState)(!1), 2),
-                    Y = q[0],
-                    Q = q[1],
-                    Z = function() {
-                        Q(!0)
-                    },
-                    J = function() {
-                        Q(!1)
-                    },
-                    ee = P.useCallback((function(e) {
+                    A = P.useCallback((function(e) {
                         return "function" == typeof g ? g(e) : null == e ? void 0 : e[g]
                     }), [g]),
-                    te = {
-                        getKey: ee
+                    T = function(e, t, n) {
+                        var r = $(P.useState(0), 2),
+                            o = r[0],
+                            i = r[1],
+                            a = (0, P.useRef)(new Map),
+                            c = (0, P.useRef)(new Fe),
+                            s = (0, P.useRef)();
+
+                        function l() {
+                            He.cancel(s.current)
+                        }
+
+                        function u() {
+                            var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
+                            l();
+                            var t = function() {
+                                a.current.forEach((function(e, t) {
+                                    if (e && e.offsetParent) {
+                                        var n = V(e),
+                                            r = n.offsetHeight;
+                                        c.current.get(t) !== r && c.current.set(t, n.offsetHeight)
+                                    }
+                                })), i((function(e) {
+                                    return e + 1
+                                }))
+                            };
+                            e ? t() : s.current = He(t)
+                        }
+                        return (0, P.useEffect)((function() {
+                            return l
+                        }), []), [function(t, n) {
+                            var r = e(t);
+                            a.current.get(r);
+                            n ? (a.current.set(r, n), u()) : a.current.delete(r)
+                        }, u, c.current, o]
+                    }(A),
+                    K = $(T, 4),
+                    D = K[0],
+                    R = K[1],
+                    L = K[2],
+                    I = K[3],
+                    H = !(!1 === y || !l || !u),
+                    z = P.useMemo((function() {
+                        return Object.values(L.maps).reduce((function(e, t) {
+                            return e + t
+                        }), 0)
+                    }), [L.id, L.maps]),
+                    B = H && h && (Math.max(u * h.length, z) > l || !!b),
+                    F = "rtl" === m,
+                    X = E()(i, a({}, "".concat(i, "-rtl"), F), c),
+                    G = h || Ze,
+                    q = (0, P.useRef)(),
+                    Y = (0, P.useRef)(),
+                    Q = $((0, P.useState)(0), 2),
+                    Z = Q[0],
+                    J = Q[1],
+                    ee = $((0, P.useState)(0), 2),
+                    te = ee[0],
+                    ne = ee[1],
+                    re = $((0, P.useState)(!1), 2),
+                    oe = re[0],
+                    ie = re[1],
+                    ae = function() {
+                        ie(!0)
+                    },
+                    ce = function() {
+                        ie(!1)
+                    },
+                    se = {
+                        getKey: A
                     };
 
-                function ne(e) {
-                    B((function(t) {
+                function le(e) {
+                    J((function(t) {
                         var n = function(e) {
                             var t = e;
-                            return Number.isNaN(Ce.current) || (t = Math.min(t, Ce.current)), t = Math.max(t, 0)
+                            return Number.isNaN(_e.current) || (t = Math.min(t, _e.current)), t = Math.max(t, 0)
                         }("function" == typeof e ? e(t) : e);
-                        return L.current.scrollTop = n, n
+                        return q.current.scrollTop = n, n
                     }))
                 }
-                var re = (0, P.useRef)({
+                var ue = (0, P.useRef)({
                         start: 0,
-                        end: R.length
+                        end: G.length
                     }),
-                    oe = (0, P.useRef)(),
-                    ie = $(function(e, t, n) {
+                    de = (0, P.useRef)(),
+                    fe = $(function(e, t, n) {
                         var r = $(P.useState(e), 2),
                             o = r[0],
                             i = r[1],
                             a = $(P.useState(null), 2),
                             c = a[0],
                             s = a[1];
                         return P.useEffect((function() {
@@ -1281,145 +1327,104 @@
                                 return null === l ? null : {
                                     index: l,
                                     multiple: u
                                 }
                             }(o || [], e || [], t);
                             void 0 !== (null == r ? void 0 : r.index) && (null == n || n(r.index), s(e[r.index])), i(e)
                         }), [e]), [c]
-                    }(R, ee), 1)[0];
-                oe.current = ie;
-                var ae = function(e, t, n) {
-                        var r = $(P.useState(0), 2),
-                            o = r[0],
-                            i = r[1],
-                            a = (0, P.useRef)(new Map),
-                            c = (0, P.useRef)(new Fe),
-                            s = (0, P.useRef)();
-
-                        function l() {
-                            He.cancel(s.current)
-                        }
-
-                        function u() {
-                            var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
-                            l();
-                            var t = function() {
-                                a.current.forEach((function(e, t) {
-                                    if (e && e.offsetParent) {
-                                        var n = V(e),
-                                            r = n.offsetHeight;
-                                        c.current.get(t) !== r && c.current.set(t, n.offsetHeight)
-                                    }
-                                })), i((function(e) {
-                                    return e + 1
-                                }))
-                            };
-                            e ? t() : s.current = He(t)
-                        }
-                        return (0, P.useEffect)((function() {
-                            return l
-                        }), []), [function(t, n) {
-                            var r = e(t);
-                            a.current.get(r);
-                            n ? (a.current.set(r, n), u()) : a.current.delete(r)
-                        }, u, c.current, o]
-                    }(ee),
-                    ce = $(ae, 4),
-                    se = ce[0],
-                    le = ce[1],
-                    ue = ce[2],
-                    de = ce[3],
-                    fe = P.useMemo((function() {
-                        if (!A) return {
+                    }(G, A), 1)[0];
+                de.current = fe;
+                var pe = P.useMemo((function() {
+                        if (!H) return {
                             scrollHeight: void 0,
                             start: 0,
-                            end: R.length - 1,
+                            end: G.length - 1,
                             offset: void 0
                         };
                         var e;
-                        if (!T) return {
-                            scrollHeight: (null === (e = I.current) || void 0 === e ? void 0 : e.offsetHeight) || 0,
+                        if (!B) return {
+                            scrollHeight: (null === (e = Y.current) || void 0 === e ? void 0 : e.offsetHeight) || 0,
                             start: 0,
-                            end: R.length - 1,
+                            end: G.length - 1,
                             offset: void 0
                         };
-                        for (var t, n, r, o = 0, i = R.length, a = 0; a < i; a += 1) {
-                            var c = R[a],
-                                s = ee(c),
-                                d = ue.get(s),
+                        for (var t, n, r, o = 0, i = G.length, a = 0; a < i; a += 1) {
+                            var c = G[a],
+                                s = A(c),
+                                d = L.get(s),
                                 f = o + (void 0 === d ? u : d);
-                            f >= z && void 0 === t && (t = a, n = o), f > z + l && void 0 === r && (r = a), o = f
+                            f >= Z && void 0 === t && (t = a, n = o), f > Z + l && void 0 === r && (r = a), o = f
                         }
-                        return void 0 === t && (t = 0, n = 0, r = Math.ceil(l / u)), void 0 === r && (r = R.length - 1), {
+                        return void 0 === t && (t = 0, n = 0, r = Math.ceil(l / u)), void 0 === r && (r = G.length - 1), {
                             scrollHeight: o,
                             start: t,
-                            end: r = Math.min(r + 1, R.length - 1),
+                            end: r = Math.min(r + 1, G.length - 1),
                             offset: n
                         }
-                    }), [T, A, z, R, de, l]),
-                    pe = fe.scrollHeight,
-                    he = fe.start,
-                    ve = fe.end,
-                    ge = fe.offset;
-                re.current.start = he, re.current.end = ve;
-                var ye = $(P.useState({
+                    }), [B, H, Z, G, I, l]),
+                    he = pe.scrollHeight,
+                    ve = pe.start,
+                    ge = pe.end,
+                    ye = pe.offset;
+                ue.current.start = ve, ue.current.end = ge;
+                var me = $(P.useState({
                         width: 0,
                         height: l
                     }), 2),
-                    me = ye[0],
-                    be = ye[1],
-                    xe = (0, P.useRef)(),
+                    be = me[0],
+                    xe = me[1],
                     we = (0, P.useRef)(),
-                    ke = P.useMemo((function() {
-                        return Ye(me.width, b)
-                    }), [me.width, b]),
+                    ke = (0, P.useRef)(),
                     Ee = P.useMemo((function() {
-                        return Ye(me.height, pe)
-                    }), [me.height, pe]),
-                    Se = pe - l,
-                    Ce = (0, P.useRef)(Se);
-                Ce.current = Se;
-                var _e = z <= 0,
-                    Me = z >= Se,
-                    Ne = Ge(_e, Me),
-                    Ae = function() {
+                        return Ye(be.width, b)
+                    }), [be.width, b]),
+                    Se = P.useMemo((function() {
+                        return Ye(be.height, he)
+                    }), [be.height, he]),
+                    Ce = he - l,
+                    _e = (0, P.useRef)(Ce);
+                _e.current = Ce;
+                var Me = Z <= 0,
+                    Ne = Z >= Ce,
+                    Ae = Ge(Me, Ne),
+                    Ke = function() {
                         return {
-                            x: K ? -X : X,
-                            y: z
+                            x: F ? -te : te,
+                            y: Z
                         }
                     },
-                    Ke = (0, P.useRef)(Ae()),
-                    De = We((function() {
+                    De = (0, P.useRef)(Ke()),
+                    Re = We((function() {
                         if (S) {
-                            var e = Ae();
-                            Ke.current.x === e.x && Ke.current.y === e.y || (S(e), Ke.current = e)
+                            var e = Ke();
+                            De.current.x === e.x && De.current.y === e.y || (S(e), De.current = e)
                         }
                     }));
 
-                function Re(e, t) {
+                function Le(e, t) {
                     var n = e;
                     t ? ((0, U.flushSync)((function() {
-                        G(n)
-                    })), De()) : ne(n)
+                        ne(n)
+                    })), Re()) : le(n)
                 }
-                var Le = function(e) {
+                var Pe = function(e) {
                         var t = e,
-                            n = b - me.width;
+                            n = b ? b - be.width : 0;
                         return t = Math.max(t, 0), Math.min(t, n)
                     },
-                    Pe = We((function(e, t) {
+                    Ie = We((function(e, t) {
                         t ? ((0, U.flushSync)((function() {
-                            G((function(t) {
-                                return Le(t + (K ? -e : e))
+                            ne((function(t) {
+                                return Pe(t + (F ? -e : e))
                             }))
-                        })), De()) : ne((function(t) {
+                        })), Re()) : le((function(t) {
                             return t + e
                         }))
                     })),
-                    Ie = $(function(e, t, n, r, o) {
+                    ze = $(function(e, t, n, r, o) {
                         var i = (0, P.useRef)(0),
                             a = (0, P.useRef)(null),
                             c = (0, P.useRef)(null),
                             s = (0, P.useRef)(!1),
                             l = Ge(t, n),
                             u = (0, P.useRef)(null),
                             d = (0, P.useRef)(null);
@@ -1444,17 +1449,17 @@
                                 }(t, v) : function(e, t) {
                                     o(t, !0), Xe || e.preventDefault()
                                 }(t, h)
                             }
                         }, function(t) {
                             e && (s.current = t.detail === c.current)
                         }]
-                    }(A, _e, Me, !!b, Pe), 2),
-                    ze = Ie[0],
-                    $e = Ie[1];
+                    }(H, Me, Ne, !!b, Ie), 2),
+                    $e = ze[0],
+                    Ue = ze[1];
                 ! function(e, t, n) {
                     var r, o = (0, P.useRef)(!1),
                         i = (0, P.useRef)(0),
                         a = (0, P.useRef)(null),
                         c = (0, P.useRef)(null),
                         s = function(e) {
                             if (o.current) {
@@ -1476,38 +1481,38 @@
                     }, W((function() {
                         return e && t.current.addEventListener("touchstart", u),
                             function() {
                                 var e;
                                 null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", u), r(), clearInterval(c.current)
                             }
                     }), [e])
-                }(A, L, (function(e, t) {
-                    return !Ne(e, t) && (ze({
+                }(H, q, (function(e, t) {
+                    return !Ae(e, t) && ($e({
                         preventDefault: function() {},
                         deltaY: e
                     }), !0)
                 })), W((function() {
                     function e(e) {
-                        A && e.preventDefault()
+                        H && e.preventDefault()
                     }
-                    var t = L.current;
-                    return t.addEventListener("wheel", ze), t.addEventListener("DOMMouseScroll", $e), t.addEventListener("MozMousePixelScroll", e),
+                    var t = q.current;
+                    return t.addEventListener("wheel", $e), t.addEventListener("DOMMouseScroll", Ue), t.addEventListener("MozMousePixelScroll", e),
                         function() {
-                            t.removeEventListener("wheel", ze), t.removeEventListener("DOMMouseScroll", $e), t.removeEventListener("MozMousePixelScroll", e)
+                            t.removeEventListener("wheel", $e), t.removeEventListener("DOMMouseScroll", Ue), t.removeEventListener("MozMousePixelScroll", e)
                         }
-                }), [A]), W((function() {
-                    b && G((function(e) {
-                        return Le(e)
+                }), [H]), W((function() {
+                    b && ne((function(e) {
+                        return Pe(e)
                     }))
-                }), [me.width, b]);
-                var Ue = function() {
+                }), [be.width, b]);
+                var Ve = function() {
                         var e, t;
-                        null === (e = xe.current) || void 0 === e || e.delayHidden(), null === (t = we.current) || void 0 === t || t.delayHidden()
+                        null === (e = we.current) || void 0 === e || e.delayHidden(), null === (t = ke.current) || void 0 === t || t.delayHidden()
                     },
-                    Ve = function(e, t, n, r, i, a, c, l) {
+                    et = function(e, t, n, r, i, a, c, l) {
                         var u = P.useRef(),
                             d = $(P.useState(null), 2),
                             f = d[0],
                             p = d[1];
                         return W((function() {
                                 if (f && f.times < 10) {
                                     if (!e.current) return void p((function(e) {
@@ -1572,32 +1577,32 @@
                                             index: n,
                                             offset: void 0 === a ? 0 : a,
                                             originAlign: r
                                         })
                                     }
                                 } else l()
                             }
-                    }(L, R, ue, u, ee, (function() {
-                        return le(!0)
-                    }), ne, Ue);
+                    }(q, G, L, u, A, (function() {
+                        return R(!0)
+                    }), le, Ve);
                 P.useImperativeHandle(t, (function() {
                     return {
-                        getScrollInfo: Ae,
+                        getScrollInfo: Ke,
                         scrollTo: function(e) {
                             var t;
-                            (t = e) && "object" === o(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && G(Le(e.left)), Ve(e.top)) : Ve(e)
+                            (t = e) && "object" === o(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && ne(Pe(e.left)), et(e.top)) : et(e)
                         }
                     }
                 })), W((function() {
                     if (C) {
-                        var e = R.slice(he, ve + 1);
-                        C(e, R)
+                        var e = G.slice(ve, ge + 1);
+                        C(e, G)
                     }
-                }), [he, ve, R]);
-                var et = function(e, t, n, r) {
+                }), [ve, ge, G]);
+                var tt = function(e, t, n, r) {
                         var o = $(P.useMemo((function() {
                                 return [new Map, []]
                             }), [e, n.id, r]), 2),
                             i = o[0],
                             a = o[1];
                         return function(o) {
                             var c = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : o,
@@ -1612,25 +1617,25 @@
                                     if (a[d] = (a[d - 1] || 0) + v, h === o && (s = d), h === c && (l = d), void 0 !== s && void 0 !== l) break
                                 }
                             return {
                                 top: a[s - 1] || 0,
                                 bottom: a[l]
                             }
                         }
-                    }(R, ee, ue, u),
-                    tt = null == M ? void 0 : M({
-                        start: he,
-                        end: ve,
-                        virtual: T,
-                        offsetX: X,
-                        offsetY: ge,
-                        rtl: K,
-                        getSize: et
+                    }(G, A, L, u),
+                    nt = null == M ? void 0 : M({
+                        start: ve,
+                        end: ge,
+                        virtual: B,
+                        offsetX: te,
+                        offsetY: ye,
+                        rtl: F,
+                        getSize: tt
                     }),
-                    nt = function(e, t, n, r, o, i, a) {
+                    rt = function(e, t, n, r, o, i, a) {
                         var c = a.getKey;
                         return e.slice(t, n + 1).map((function(e, n) {
                             var a = i(e, t + n, {
                                     style: {
                                         width: r
                                     }
                                 }),
@@ -1638,74 +1643,74 @@
                             return P.createElement(Be, {
                                 key: s,
                                 setRef: function(t) {
                                     return o(e, t)
                                 }
                             }, a)
                         }))
-                    }(R, he, ve, b, se, v, te),
-                    rt = null;
-                l && (rt = s(a({}, f ? "height" : "maxHeight", l), Je), A && (rt.overflowY = "hidden", b && (rt.overflowX = "hidden"), Y && (rt.pointerEvents = "none")));
-                var ot = {};
-                return K && (ot.dir = "rtl"), P.createElement("div", r({
+                    }(G, ve, ge, b, D, v, se),
+                    ot = null;
+                l && (ot = s(a({}, f ? "height" : "maxHeight", l), Je), H && (ot.overflowY = "hidden", b && (ot.overflowX = "hidden"), oe && (ot.pointerEvents = "none")));
+                var it = {};
+                return F && (it.dir = "rtl"), P.createElement("div", r({
                     style: s(s({}, p), {}, {
                         position: "relative"
                     }),
-                    className: D
-                }, ot, O), P.createElement(Oe, {
+                    className: X
+                }, it, O), P.createElement(Oe, {
                     onResize: function(e) {
-                        be({
+                        xe({
                             width: e.width || e.offsetWidth,
                             height: e.height || e.offsetHeight
                         })
                     }
                 }, P.createElement(w, {
                     className: "".concat(i, "-holder"),
-                    style: rt,
-                    ref: L,
+                    style: ot,
+                    ref: q,
                     onScroll: function(e) {
                         var t = e.currentTarget.scrollTop;
-                        t !== z && ne(t), null == k || k(e), De()
+                        t !== Z && le(t), null == k || k(e), Re()
                     },
-                    onMouseEnter: Ue
+                    onMouseEnter: Ve
                 }, P.createElement(Te, {
                     prefixCls: i,
-                    height: pe,
-                    offsetX: X,
-                    offsetY: ge,
+                    height: he,
+                    offsetX: te,
+                    offsetY: ye,
                     scrollWidth: b,
-                    onInnerResize: le,
-                    ref: I,
+                    onInnerResize: R,
+                    ref: Y,
                     innerProps: _,
-                    rtl: K,
-                    extra: tt
-                }, nt))), T && pe > l && P.createElement(je, {
-                    ref: xe,
+                    rtl: F,
+                    extra: nt
+                }, rt))), B && he > l && P.createElement(je, {
+                    ref: we,
                     prefixCls: i,
-                    scrollOffset: z,
-                    scrollRange: pe,
-                    rtl: K,
-                    onScroll: Re,
-                    onStartMove: Z,
-                    onStopMove: J,
-                    spinSize: Ee,
-                    containerSize: me.height,
+                    scrollOffset: Z,
+                    scrollRange: he,
+                    rtl: F,
+                    onScroll: Le,
+                    onStartMove: ae,
+                    onStopMove: ce,
+                    spinSize: Se,
+                    containerSize: be.height,
                     style: null == N ? void 0 : N.verticalScrollBar,
                     thumbStyle: null == N ? void 0 : N.verticalScrollBarThumb
-                }), T && b > me.width && P.createElement(je, {
-                    ref: we,
+                }), B && b > be.width && P.createElement(je, {
+                    ref: ke,
                     prefixCls: i,
-                    scrollOffset: X,
+                    scrollOffset: te,
                     scrollRange: b,
-                    rtl: K,
-                    onScroll: Re,
-                    onStartMove: Z,
-                    onStopMove: J,
-                    spinSize: ke,
-                    containerSize: me.width,
+                    rtl: F,
+                    onScroll: Le,
+                    onStartMove: ae,
+                    onStopMove: ce,
+                    spinSize: Ee,
+                    containerSize: be.width,
                     horizontal: !0,
                     style: null == N ? void 0 : N.horizontalScrollBar,
                     thumbStyle: null == N ? void 0 : N.horizontalScrollBarThumb
                 }))
             }
             var tt = P.forwardRef(et);
             tt.displayName = "List";
@@ -5102,23 +5107,24 @@
                 }(),
                 _o = new Eo,
                 Mo = new WeakMap,
                 No = {},
                 Oo = new WeakMap;
 
             function Ao(e) {
-                var t = Oo.get(e) || "";
-                return t || (Object.keys(e).forEach((function(n) {
-                    var r = e[n];
-                    t += n, r instanceof Co ? t += r.id : r && "object" === o(r) ? t += Ao(r) : t += r
-                })), Oo.set(e, t)), t
+                var t = arguments.length > 1 && void 0 !== arguments[1] && arguments[1],
+                    n = Oo.get(e) || "";
+                return n || (Object.keys(e).forEach((function(r) {
+                    var i = e[r];
+                    n += r, i instanceof Co ? n += i.id : i && "object" === o(i) ? n += Ao(i, t) : n += i
+                })), t && (n = ho(n)), Oo.set(e, n)), n
             }
 
             function To(e, t) {
-                return ho("".concat(t, "_").concat(Ao(e)))
+                return ho("".concat(t, "_").concat(Ao(e, !0)))
             }
             "random-".concat(Date.now(), "-").concat(Math.random()).replace(/\./g, "");
             var Ko = B();
 
             function Do(e) {
                 return "number" == typeof e ? "".concat(e, "px") : e
             }
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/636.e37faa04eb8cb39edd7f.js.LICENSE.txt` & `jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/636.18742a3929885dfb4bfa.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/remoteEntry.44274364debca46ec439.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/remoteEntry.90789c29a44dad669aa0.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, l, u, f, d, s, p, c, h, v, m, b, g, y, w, j, S, P, E = {
+    var e, r, t, a, n, o, i, l, u, f, s, d, p, c, h, v, m, b, g, y, w, j, S, P, E = {
             535: (e, r, t) => {
                 var a = {
                         "./index": () => Promise.all([t.e(636), t.e(550), t.e(638), t.e(219)]).then((() => () => t(219))),
                         "./extension": () => Promise.all([t.e(636), t.e(550), t.e(638), t.e(219)]).then((() => () => t(219))),
                         "./style": () => Promise.all([t.e(550), t.e(121)]).then((() => () => t(631)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -47,53 +47,53 @@
             get: r[t]
         })
     }, _.f = {}, _.e = e => Promise.all(Object.keys(_.f).reduce(((r, t) => (_.f[t](e, r), r)), [])), _.u = e => e + "." + {
         121: "db61795daabb4d1eb7c3",
         219: "2f775af86603225cd107",
         285: "4eef7e98cbfad514e073",
         550: "c5bd7757f7228cea68ce",
-        636: "e37faa04eb8cb39edd7f",
+        636: "18742a3929885dfb4bfa",
         638: "28f4ea302090a6e9a404"
     } [e] + ".js?v=" + {
         121: "db61795daabb4d1eb7c3",
         219: "2f775af86603225cd107",
         285: "4eef7e98cbfad514e073",
         550: "c5bd7757f7228cea68ce",
-        636: "e37faa04eb8cb39edd7f",
+        636: "18742a3929885dfb4bfa",
         638: "28f4ea302090a6e9a404"
     } [e], _.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), _.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-editor:", _.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var i, l;
             if (void 0 !== n)
                 for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var d = u[f];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
-                        i = d;
+                    var s = u[f];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
+                        i = s;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, _.nc && i.setAttribute("nonce", _.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
-            var s = (r, a) => {
+            var d = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                p = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, _.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -115,15 +115,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@amphi/pipeline-editor", "0.2.1", (() => Promise.all([_.e(636), _.e(550), _.e(638), _.e(219)]).then((() => () => _(219))))), l("reactflow", "11.9.4", (() => Promise.all([_.e(285), _.e(638)]).then((() => () => _(285)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@amphi/pipeline-editor", "0.2.2", (() => Promise.all([_.e(636), _.e(550), _.e(638), _.e(219)]).then((() => () => _(219))))), l("reactflow", "11.9.4", (() => Promise.all([_.e(285), _.e(638)]).then((() => () => _(285)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         _.g.importScripts && (e = _.g.location + "");
         var r = _.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -173,33 +173,33 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, d, s = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (d = (typeof(f = r[i]))[0])) return !u || ("u" == s ? l > a && !n : "" == s != n);
-                if ("u" == d) {
-                    if (!u || "u" != s) return !1
+                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == d ? l > a && !n : "" == d != n);
+                if ("u" == s) {
+                    if (!u || "u" != d) return !1
                 } else if (u)
-                    if (s == d)
+                    if (d == s)
                         if (l <= a) {
                             if (f != e[l]) return !1
                         } else {
                             if (n ? f > e[l] : f < e[l]) return !1;
                             f != e[l] && (u = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != d && "n" != d) {
                     if (n || l <= a) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= a || d < s != n) return !1;
+                    if (l <= a || s < d != n) return !1;
                     u = !1
-                } else "s" != s && "n" != s && (u = !1, l--)
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
@@ -211,32 +211,32 @@
         return t
     }, l = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", d = (e, r, t, a) => {
+    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", s = (e, r, t, a) => {
         var n = u(e, t);
         return o(a, n) || c(f(e, t, n, a)), v(e[t][n])
-    }, s = (e, r, t) => {
+    }, d = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, p = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + n(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, h = (e, r, t, a) => {
         c(p(e, r, t, a))
     }, v = e => (e.loaded = 1, e.get()), b = (m = e => function(r, t, a, n) {
         var o = _.I(r);
         return o && o.then ? o.then(e.bind(e, r, _.S[r], t, a, n)) : e(r, _.S[r], t, a, n)
-    })(((e, r, t, a) => (i(e, t), v(s(r, t, a) || h(r, e, t, a) || l(r, t))))), g = m(((e, r, t, a) => (i(e, t), d(r, 0, t, a)))), y = m(((e, r, t, a, n) => {
-        var o = r && _.o(r, t) && s(r, t, a);
+    })(((e, r, t, a) => (i(e, t), v(d(r, t, a) || h(r, e, t, a) || l(r, t))))), g = m(((e, r, t, a) => (i(e, t), s(r, 0, t, a)))), y = m(((e, r, t, a, n) => {
+        var o = r && _.o(r, t) && d(r, t, a);
         return o ? v(o) : n()
     })), w = {}, j = {
         345: () => g("default", "react", [1, 18, 2, 0]),
         628: () => g("default", "react-dom", [1, 18, 2, 0]),
         14: () => g("default", "@jupyterlab/statusbar", [1, 4, 1, 6]),
         221: () => g("default", "@jupyterlab/filebrowser", [1, 4, 1, 6]),
         254: () => g("default", "@amphi/pipeline-components-manager", [0]),
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-editor/static/third-party-licenses.json` & `jupyterlab_amphi-0.2.2/amphi/pipeline-editor/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967948717948718%*

 * *Differences: {"'packages'": "{1: {'versionInfo': '1.20.0'}, 31: {'versionInfo': '3.11.5'}}"}*

```diff
@@ -6,15 +6,15 @@
             "name": "@ant-design/colors",
             "versionInfo": "7.0.2"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2019-present afc163\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the \"Software\"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@ant-design/cssinjs",
-            "versionInfo": "1.19.1"
+            "versionInfo": "1.20.0"
         },
         {
             "extractedText": "MIT LICENSE\n\nCopyright (c) 2018-present Ant UED, https://xtech.antfin.com/\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@ant-design/icons",
             "versionInfo": "5.3.6"
         },
@@ -186,15 +186,15 @@
             "name": "rc-util",
             "versionInfo": "5.39.1"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-virtual-list",
-            "versionInfo": "3.11.4"
+            "versionInfo": "3.11.5"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react-is",
             "versionInfo": "18.2.0"
         },
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/package.json` & `jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.de9bf8c4ac18d1151373.js'}}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -52,15 +52,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9a28884c4594f181f68a.js",
+            "load": "static/remoteEntry.de9bf8c4ac18d1151373.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-log-console",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
@@ -99,9 +99,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/static/432.a6577eba0279cb4b76e3.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/static/432.a6577eba0279cb4b76e3.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/static/444.36935dbcd8fc3a74e25f.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/static/444.35926916905e9c76b8c9.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 444.36935dbcd8fc3a74e25f.js.LICENSE.txt */
+/*! For license information please see 444.35926916905e9c76b8c9.js.LICENSE.txt */
 (self.webpackChunk_amphi_pipeline_log_console = self.webpackChunk_amphi_pipeline_log_console || []).push([
     [444], {
         444: (e, t, n) => {
             "use strict";
             n.d(t, {
                 A: () => RS
             });
@@ -3082,58 +3082,104 @@
                     S = e.onScroll,
                     E = e.onVirtualScroll,
                     $ = e.onVisibleChange,
                     k = e.innerProps,
                     I = e.extraRender,
                     N = e.styles,
                     M = ve(e, Kn),
-                    R = !(!1 === h || !a || !l),
-                    j = R && p && (l * p.length > a || !!x),
-                    T = "rtl" === y,
-                    z = Y()(o, q({}, "".concat(o, "-rtl"), T), i),
-                    B = p || _n,
-                    A = (0, r.useRef)(),
-                    D = (0, r.useRef)(),
-                    H = d((0, r.useState)(0), 2),
-                    L = H[0],
-                    F = H[1],
-                    K = d((0, r.useState)(0), 2),
-                    _ = K[0],
-                    W = K[1],
-                    V = d((0, r.useState)(!1), 2),
-                    X = V[0],
-                    U = V[1],
-                    Q = function() {
-                        U(!0)
-                    },
-                    Z = function() {
-                        U(!1)
-                    },
-                    J = r.useCallback((function(e) {
+                    R = r.useCallback((function(e) {
                         return "function" == typeof g ? g(e) : null == e ? void 0 : e[g]
                     }), [g]),
-                    ee = {
-                        getKey: J
+                    j = function(e, t, n) {
+                        var o = d(r.useState(0), 2),
+                            i = o[0],
+                            a = o[1],
+                            l = (0, r.useRef)(new Map),
+                            c = (0, r.useRef)(new Bn),
+                            s = (0, r.useRef)();
+
+                        function u() {
+                            bn.cancel(s.current)
+                        }
+
+                        function f() {
+                            var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
+                            u();
+                            var t = function() {
+                                l.current.forEach((function(e, t) {
+                                    if (e && e.offsetParent) {
+                                        var n = $e(e),
+                                            r = n.offsetHeight;
+                                        c.current.get(t) !== r && c.current.set(t, n.offsetHeight)
+                                    }
+                                })), a((function(e) {
+                                    return e + 1
+                                }))
+                            };
+                            e ? t() : s.current = bn(t)
+                        }
+                        return (0, r.useEffect)((function() {
+                            return u
+                        }), []), [function(t, n) {
+                            var r = e(t);
+                            l.current.get(r);
+                            n ? (l.current.set(r, n), f()) : l.current.delete(r)
+                        }, f, c.current, i]
+                    }(R),
+                    T = d(j, 4),
+                    z = T[0],
+                    B = T[1],
+                    A = T[2],
+                    D = T[3],
+                    H = !(!1 === h || !a || !l),
+                    L = r.useMemo((function() {
+                        return Object.values(A.maps).reduce((function(e, t) {
+                            return e + t
+                        }), 0)
+                    }), [A.id, A.maps]),
+                    F = H && p && (Math.max(l * p.length, L) > a || !!x),
+                    K = "rtl" === y,
+                    _ = Y()(o, q({}, "".concat(o, "-rtl"), K), i),
+                    W = p || _n,
+                    V = (0, r.useRef)(),
+                    X = (0, r.useRef)(),
+                    U = d((0, r.useState)(0), 2),
+                    Q = U[0],
+                    Z = U[1],
+                    J = d((0, r.useState)(0), 2),
+                    ee = J[0],
+                    te = J[1],
+                    ne = d((0, r.useState)(!1), 2),
+                    re = ne[0],
+                    oe = ne[1],
+                    ie = function() {
+                        oe(!0)
+                    },
+                    ae = function() {
+                        oe(!1)
+                    },
+                    le = {
+                        getKey: R
                     };
 
-                function te(e) {
-                    F((function(t) {
+                function ce(e) {
+                    Z((function(t) {
                         var n = function(e) {
                             var t = e;
-                            return Number.isNaN(ke.current) || (t = Math.min(t, ke.current)), t = Math.max(t, 0)
+                            return Number.isNaN(Oe.current) || (t = Math.min(t, Oe.current)), t = Math.max(t, 0)
                         }("function" == typeof e ? e(t) : e);
-                        return A.current.scrollTop = n, n
+                        return V.current.scrollTop = n, n
                     }))
                 }
-                var ne = (0, r.useRef)({
+                var se = (0, r.useRef)({
                         start: 0,
-                        end: B.length
+                        end: W.length
                     }),
-                    re = (0, r.useRef)(),
-                    oe = d(function(e, t, n) {
+                    ue = (0, r.useRef)(),
+                    de = d(function(e, t, n) {
                         var o = d(r.useState(e), 2),
                             i = o[0],
                             a = o[1],
                             l = d(r.useState(null), 2),
                             c = l[0],
                             s = l[1];
                         return r.useEffect((function() {
@@ -3159,145 +3205,104 @@
                                 return null === s ? null : {
                                     index: s,
                                     multiple: u
                                 }
                             }(i || [], e || [], t);
                             void 0 !== (null == r ? void 0 : r.index) && (null == n || n(r.index), s(e[r.index])), a(e)
                         }), [e]), [c]
-                    }(B, J), 1)[0];
-                re.current = oe;
-                var ie = function(e, t, n) {
-                        var o = d(r.useState(0), 2),
-                            i = o[0],
-                            a = o[1],
-                            l = (0, r.useRef)(new Map),
-                            c = (0, r.useRef)(new Bn),
-                            s = (0, r.useRef)();
-
-                        function u() {
-                            bn.cancel(s.current)
-                        }
-
-                        function f() {
-                            var e = arguments.length > 0 && void 0 !== arguments[0] && arguments[0];
-                            u();
-                            var t = function() {
-                                l.current.forEach((function(e, t) {
-                                    if (e && e.offsetParent) {
-                                        var n = $e(e),
-                                            r = n.offsetHeight;
-                                        c.current.get(t) !== r && c.current.set(t, n.offsetHeight)
-                                    }
-                                })), a((function(e) {
-                                    return e + 1
-                                }))
-                            };
-                            e ? t() : s.current = bn(t)
-                        }
-                        return (0, r.useEffect)((function() {
-                            return u
-                        }), []), [function(t, n) {
-                            var r = e(t);
-                            l.current.get(r);
-                            n ? (l.current.set(r, n), f()) : l.current.delete(r)
-                        }, f, c.current, i]
-                    }(J),
-                    ae = d(ie, 4),
-                    le = ae[0],
-                    ce = ae[1],
-                    se = ae[2],
-                    ue = ae[3],
-                    de = r.useMemo((function() {
-                        if (!R) return {
+                    }(W, R), 1)[0];
+                ue.current = de;
+                var fe = r.useMemo((function() {
+                        if (!H) return {
                             scrollHeight: void 0,
                             start: 0,
-                            end: B.length - 1,
+                            end: W.length - 1,
                             offset: void 0
                         };
                         var e;
-                        if (!j) return {
-                            scrollHeight: (null === (e = D.current) || void 0 === e ? void 0 : e.offsetHeight) || 0,
+                        if (!F) return {
+                            scrollHeight: (null === (e = X.current) || void 0 === e ? void 0 : e.offsetHeight) || 0,
                             start: 0,
-                            end: B.length - 1,
+                            end: W.length - 1,
                             offset: void 0
                         };
-                        for (var t, n, r, o = 0, i = B.length, c = 0; c < i; c += 1) {
-                            var s = B[c],
-                                u = J(s),
-                                d = se.get(u),
+                        for (var t, n, r, o = 0, i = W.length, c = 0; c < i; c += 1) {
+                            var s = W[c],
+                                u = R(s),
+                                d = A.get(u),
                                 f = o + (void 0 === d ? l : d);
-                            f >= L && void 0 === t && (t = c, n = o), f > L + a && void 0 === r && (r = c), o = f
+                            f >= Q && void 0 === t && (t = c, n = o), f > Q + a && void 0 === r && (r = c), o = f
                         }
-                        return void 0 === t && (t = 0, n = 0, r = Math.ceil(a / l)), void 0 === r && (r = B.length - 1), {
+                        return void 0 === t && (t = 0, n = 0, r = Math.ceil(a / l)), void 0 === r && (r = W.length - 1), {
                             scrollHeight: o,
                             start: t,
-                            end: r = Math.min(r + 1, B.length - 1),
+                            end: r = Math.min(r + 1, W.length - 1),
                             offset: n
                         }
-                    }), [j, R, L, B, ue, a]),
-                    fe = de.scrollHeight,
-                    pe = de.start,
-                    me = de.end,
-                    ge = de.offset;
-                ne.current.start = pe, ne.current.end = me;
-                var he = d(r.useState({
+                    }), [F, H, Q, W, D, a]),
+                    pe = fe.scrollHeight,
+                    me = fe.start,
+                    ge = fe.end,
+                    he = fe.offset;
+                se.current.start = me, se.current.end = ge;
+                var be = d(r.useState({
                         width: 0,
                         height: a
                     }), 2),
-                    be = he[0],
-                    ye = he[1],
-                    xe = (0, r.useRef)(),
+                    ye = be[0],
+                    xe = be[1],
                     we = (0, r.useRef)(),
-                    Ce = r.useMemo((function() {
-                        return Fn(be.width, x)
-                    }), [be.width, x]),
+                    Ce = (0, r.useRef)(),
                     Se = r.useMemo((function() {
-                        return Fn(be.height, fe)
-                    }), [be.height, fe]),
-                    Ee = fe - a,
-                    ke = (0, r.useRef)(Ee);
-                ke.current = Ee;
-                var Oe = L <= 0,
-                    Ie = L >= Ee,
-                    Ne = Dn(Oe, Ie),
-                    Me = function() {
+                        return Fn(ye.width, x)
+                    }), [ye.width, x]),
+                    Ee = r.useMemo((function() {
+                        return Fn(ye.height, pe)
+                    }), [ye.height, pe]),
+                    ke = pe - a,
+                    Oe = (0, r.useRef)(ke);
+                Oe.current = ke;
+                var Ie = Q <= 0,
+                    Ne = Q >= ke,
+                    Me = Dn(Ie, Ne),
+                    Pe = function() {
                         return {
-                            x: T ? -_ : _,
-                            y: L
+                            x: K ? -ee : ee,
+                            y: Q
                         }
                     },
-                    Pe = (0, r.useRef)(Me()),
-                    Re = f((function() {
+                    Re = (0, r.useRef)(Pe()),
+                    je = f((function() {
                         if (E) {
-                            var e = Me();
-                            Pe.current.x === e.x && Pe.current.y === e.y || (E(e), Pe.current = e)
+                            var e = Pe();
+                            Re.current.x === e.x && Re.current.y === e.y || (E(e), Re.current = e)
                         }
                     }));
 
-                function je(e, t) {
+                function Te(e, t) {
                     var n = e;
                     t ? ((0, O.flushSync)((function() {
-                        W(n)
-                    })), Re()) : te(n)
+                        te(n)
+                    })), je()) : ce(n)
                 }
-                var Te = function(e) {
+                var ze = function(e) {
                         var t = e,
-                            n = x - be.width;
+                            n = x ? x - ye.width : 0;
                         return t = Math.max(t, 0), Math.min(t, n)
                     },
-                    ze = f((function(e, t) {
+                    Be = f((function(e, t) {
                         t ? ((0, O.flushSync)((function() {
-                            W((function(t) {
-                                return Te(t + (T ? -e : e))
+                            te((function(t) {
+                                return ze(t + (K ? -e : e))
                             }))
-                        })), Re()) : te((function(t) {
+                        })), je()) : ce((function(t) {
                             return t + e
                         }))
                     })),
-                    Be = d(function(e, t, n, o, i) {
+                    Ae = d(function(e, t, n, o, i) {
                         var a = (0, r.useRef)(0),
                             l = (0, r.useRef)(null),
                             c = (0, r.useRef)(null),
                             s = (0, r.useRef)(!1),
                             u = Dn(t, n),
                             d = (0, r.useRef)(null),
                             f = (0, r.useRef)(null);
@@ -3322,17 +3327,17 @@
                                 }(t, g) : function(e, t) {
                                     i(t, !0), An || e.preventDefault()
                                 }(t, m)
                             }
                         }, function(t) {
                             e && (s.current = t.detail === c.current)
                         }]
-                    }(R, Oe, Ie, !!x, ze), 2),
-                    Ae = Be[0],
-                    De = Be[1];
+                    }(H, Ie, Ne, !!x, Be), 2),
+                    De = Ae[0],
+                    He = Ae[1];
                 ! function(e, t, n) {
                     var o, i = (0, r.useRef)(!1),
                         a = (0, r.useRef)(0),
                         l = (0, r.useRef)(null),
                         c = (0, r.useRef)(null),
                         s = function(e) {
                             if (i.current) {
@@ -3354,38 +3359,38 @@
                     }, v((function() {
                         return e && t.current.addEventListener("touchstart", d),
                             function() {
                                 var e;
                                 null === (e = t.current) || void 0 === e || e.removeEventListener("touchstart", d), o(), clearInterval(c.current)
                             }
                     }), [e])
-                }(R, A, (function(e, t) {
-                    return !Ne(e, t) && (Ae({
+                }(H, V, (function(e, t) {
+                    return !Me(e, t) && (De({
                         preventDefault: function() {},
                         deltaY: e
                     }), !0)
                 })), v((function() {
                     function e(e) {
-                        R && e.preventDefault()
+                        H && e.preventDefault()
                     }
-                    var t = A.current;
-                    return t.addEventListener("wheel", Ae), t.addEventListener("DOMMouseScroll", De), t.addEventListener("MozMousePixelScroll", e),
+                    var t = V.current;
+                    return t.addEventListener("wheel", De), t.addEventListener("DOMMouseScroll", He), t.addEventListener("MozMousePixelScroll", e),
                         function() {
-                            t.removeEventListener("wheel", Ae), t.removeEventListener("DOMMouseScroll", De), t.removeEventListener("MozMousePixelScroll", e)
+                            t.removeEventListener("wheel", De), t.removeEventListener("DOMMouseScroll", He), t.removeEventListener("MozMousePixelScroll", e)
                         }
-                }), [R]), v((function() {
-                    x && W((function(e) {
-                        return Te(e)
+                }), [H]), v((function() {
+                    x && te((function(e) {
+                        return ze(e)
                     }))
-                }), [be.width, x]);
-                var He = function() {
+                }), [ye.width, x]);
+                var Le = function() {
                         var e, t;
-                        null === (e = xe.current) || void 0 === e || e.delayHidden(), null === (t = we.current) || void 0 === t || t.delayHidden()
+                        null === (e = we.current) || void 0 === e || e.delayHidden(), null === (t = Ce.current) || void 0 === t || t.delayHidden()
                     },
-                    Le = function(e, t, n, o, i, a, l, c) {
+                    Fe = function(e, t, n, o, i, a, l, c) {
                         var s = r.useRef(),
                             u = d(r.useState(null), 2),
                             f = u[0],
                             p = u[1];
                         return v((function() {
                                 if (f && f.times < 10) {
                                     if (!e.current) return void p((function(e) {
@@ -3450,32 +3455,32 @@
                                             index: n,
                                             offset: void 0 === o ? 0 : o,
                                             originAlign: r
                                         })
                                     }
                                 } else c()
                             }
-                    }(A, B, se, l, J, (function() {
-                        return ce(!0)
-                    }), te, He);
+                    }(V, W, A, l, R, (function() {
+                        return B(!0)
+                    }), ce, Le);
                 r.useImperativeHandle(t, (function() {
                     return {
-                        getScrollInfo: Me,
+                        getScrollInfo: Pe,
                         scrollTo: function(e) {
                             var t;
-                            (t = e) && "object" === b(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && W(Te(e.left)), Le(e.top)) : Le(e)
+                            (t = e) && "object" === b(t) && ("left" in t || "top" in t) ? (void 0 !== e.left && te(ze(e.left)), Fe(e.top)) : Fe(e)
                         }
                     }
                 })), v((function() {
                     if ($) {
-                        var e = B.slice(pe, me + 1);
-                        $(e, B)
+                        var e = W.slice(me, ge + 1);
+                        $(e, W)
                     }
-                }), [pe, me, B]);
-                var Fe = function(e, t, n, o) {
+                }), [me, ge, W]);
+                var Ke = function(e, t, n, o) {
                         var i = d(r.useMemo((function() {
                                 return [new Map, []]
                             }), [e, n.id, o]), 2),
                             a = i[0],
                             l = i[1];
                         return function(r) {
                             var i = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : r,
@@ -3490,25 +3495,25 @@
                                     if (l[d] = (l[d - 1] || 0) + g, m === r && (c = d), m === i && (s = d), void 0 !== c && void 0 !== s) break
                                 }
                             return {
                                 top: l[c - 1] || 0,
                                 bottom: l[s]
                             }
                         }
-                    }(B, J, se, l),
-                    Ke = null == I ? void 0 : I({
-                        start: pe,
-                        end: me,
-                        virtual: j,
-                        offsetX: _,
-                        offsetY: ge,
-                        rtl: T,
-                        getSize: Fe
+                    }(W, R, A, l),
+                    _e = null == I ? void 0 : I({
+                        start: me,
+                        end: ge,
+                        virtual: F,
+                        offsetX: ee,
+                        offsetY: he,
+                        rtl: K,
+                        getSize: Ke
                     }),
-                    _e = function(e, t, n, o, i, a, l) {
+                    We = function(e, t, n, o, i, a, l) {
                         var c = l.getKey;
                         return e.slice(t, n + 1).map((function(e, n) {
                             var l = a(e, t + n, {
                                     style: {
                                         width: o
                                     }
                                 }),
@@ -3516,74 +3521,74 @@
                             return r.createElement(zn, {
                                 key: s,
                                 setRef: function(t) {
                                     return i(e, t)
                                 }
                             }, l)
                         }))
-                    }(B, pe, me, x, le, m, ee),
-                    We = null;
-                a && (We = G(q({}, s ? "height" : "maxHeight", a), Wn), R && (We.overflowY = "hidden", x && (We.overflowX = "hidden"), X && (We.pointerEvents = "none")));
-                var Ve = {};
-                return T && (Ve.dir = "rtl"), r.createElement("div", P({
+                    }(W, me, ge, x, z, m, le),
+                    Ve = null;
+                a && (Ve = G(q({}, s ? "height" : "maxHeight", a), Wn), H && (Ve.overflowY = "hidden", x && (Ve.overflowX = "hidden"), re && (Ve.pointerEvents = "none")));
+                var qe = {};
+                return K && (qe.dir = "rtl"), r.createElement("div", P({
                     style: G(G({}, u), {}, {
                         position: "relative"
                     }),
-                    className: z
-                }, Ve, M), r.createElement(dt, {
+                    className: _
+                }, qe, M), r.createElement(dt, {
                     onResize: function(e) {
-                        ye({
+                        xe({
                             width: e.width || e.offsetWidth,
                             height: e.height || e.offsetHeight
                         })
                     }
                 }, r.createElement(C, {
                     className: "".concat(o, "-holder"),
-                    style: We,
-                    ref: A,
+                    style: Ve,
+                    ref: V,
                     onScroll: function(e) {
                         var t = e.currentTarget.scrollTop;
-                        t !== L && te(t), null == S || S(e), Re()
+                        t !== Q && ce(t), null == S || S(e), je()
                     },
-                    onMouseEnter: He
+                    onMouseEnter: Le
                 }, r.createElement(Pn, {
                     prefixCls: o,
-                    height: fe,
-                    offsetX: _,
-                    offsetY: ge,
+                    height: pe,
+                    offsetX: ee,
+                    offsetY: he,
                     scrollWidth: x,
-                    onInnerResize: ce,
-                    ref: D,
+                    onInnerResize: B,
+                    ref: X,
                     innerProps: k,
-                    rtl: T,
-                    extra: Ke
-                }, _e))), j && fe > a && r.createElement(Tn, {
-                    ref: xe,
+                    rtl: K,
+                    extra: _e
+                }, We))), F && pe > a && r.createElement(Tn, {
+                    ref: we,
                     prefixCls: o,
-                    scrollOffset: L,
-                    scrollRange: fe,
-                    rtl: T,
-                    onScroll: je,
-                    onStartMove: Q,
-                    onStopMove: Z,
-                    spinSize: Se,
-                    containerSize: be.height,
+                    scrollOffset: Q,
+                    scrollRange: pe,
+                    rtl: K,
+                    onScroll: Te,
+                    onStartMove: ie,
+                    onStopMove: ae,
+                    spinSize: Ee,
+                    containerSize: ye.height,
                     style: null == N ? void 0 : N.verticalScrollBar,
                     thumbStyle: null == N ? void 0 : N.verticalScrollBarThumb
-                }), j && x > be.width && r.createElement(Tn, {
-                    ref: we,
+                }), F && x > ye.width && r.createElement(Tn, {
+                    ref: Ce,
                     prefixCls: o,
-                    scrollOffset: _,
+                    scrollOffset: ee,
                     scrollRange: x,
-                    rtl: T,
-                    onScroll: je,
-                    onStartMove: Q,
-                    onStopMove: Z,
-                    spinSize: Ce,
-                    containerSize: be.width,
+                    rtl: K,
+                    onScroll: Te,
+                    onStartMove: ie,
+                    onStopMove: ae,
+                    spinSize: Se,
+                    containerSize: ye.width,
                     horizontal: !0,
                     style: null == N ? void 0 : N.horizontalScrollBar,
                     thumbStyle: null == N ? void 0 : N.horizontalScrollBarThumb
                 }))
             }
             var qn = r.forwardRef(Vn);
             qn.displayName = "List";
@@ -5690,23 +5695,24 @@
                 return di.has(t) || di.set(t, new ui(t)), di.get(t)
             }
             var pi = new WeakMap,
                 mi = {},
                 gi = new WeakMap;
 
             function hi(e) {
-                var t = gi.get(e) || "";
-                return t || (Object.keys(e).forEach((function(n) {
-                    var r = e[n];
-                    t += n, r instanceof ui ? t += r.id : r && "object" === b(r) ? t += hi(r) : t += r
-                })), gi.set(e, t)), t
+                var t = arguments.length > 1 && void 0 !== arguments[1] && arguments[1],
+                    n = gi.get(e) || "";
+                return n || (Object.keys(e).forEach((function(r) {
+                    var o = e[r];
+                    n += r, o instanceof ui ? n += o.id : o && "object" === b(o) ? n += hi(o, t) : n += o
+                })), t && (n = Zo(n)), gi.set(e, n)), n
             }
 
             function vi(e, t) {
-                return Zo("".concat(t, "_").concat(hi(e)))
+                return Zo("".concat(t, "_").concat(hi(e, !0)))
             }
             "random-".concat(Date.now(), "-").concat(Math.random()).replace(/\./g, "");
             var bi = p();
 
             function yi(e) {
                 return "number" == typeof e ? "".concat(e, "px") : e
             }
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/static/444.36935dbcd8fc3a74e25f.js.LICENSE.txt` & `jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/static/444.35926916905e9c76b8c9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/static/684.2b2213062b13c7490a61.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/static/684.2b2213062b13c7490a61.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/static/remoteEntry.9a28884c4594f181f68a.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-metadata-panel/static/remoteEntry.d7f8174936e132a8b035.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, l, u, f, s, p, d, c, h, v, m, g = {
-            383: (e, r, t) => {
+    var e, r, t, n, a, i, o, l, u, p, d, f, s, c, h, v, m, g = {
+            320: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(444), t.e(684)]).then((() => () => t(684))),
-                        "./extension": () => Promise.all([t.e(444), t.e(684)]).then((() => () => t(684))),
+                        "./index": () => t.e(732).then((() => () => t(732))),
+                        "./extension": () => t.e(732).then((() => () => t(732))),
                         "./style": () => t.e(432).then((() => () => t(432)))
                     },
-                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     i = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                o = t.S[n];
-                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                a = t.S[n];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => o,
+                    get: () => a,
                     init: () => i
                 })
             }
         },
         b = {};
 
     function y(e) {
@@ -43,80 +43,78 @@
         }), r
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
-        432: "a6577eba0279cb4b76e3",
-        444: "36935dbcd8fc3a74e25f",
-        684: "2b2213062b13c7490a61"
+        432: "1dff82965ae8eeafd45c",
+        732: "5ee1843a7c6f18d4f9f9"
     } [e] + ".js?v=" + {
-        432: "a6577eba0279cb4b76e3",
-        444: "36935dbcd8fc3a74e25f",
-        684: "2b2213062b13c7490a61"
+        432: "1dff82965ae8eeafd45c",
+        732: "5ee1843a7c6f18d4f9f9"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-log-console:", y.l = (t, n, o, i) => {
+    }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-metadata-panel:", y.l = (t, n, a, i) => {
         if (e[t]) e[t].push(n);
         else {
-            var a, l;
-            if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var s = u[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        a = s;
+            var o, l;
+            if (void 0 !== a)
+                for (var u = document.getElementsByTagName("script"), p = 0; p < u.length; p++) {
+                    var d = u[p];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
+                        o = d;
                         break
                     }
                 }
-            a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, y.nc && a.setAttribute("nonce", y.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
-            var p = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(d);
-                    var o = e[t];
-                    if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
+            o || (l = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, y.nc && o.setAttribute("nonce", y.nc), o.setAttribute("data-webpack", r + a), o.src = t), e[t] = [n];
+            var f = (r, n) => {
+                    o.onerror = o.onload = null, clearTimeout(s);
+                    var a = e[t];
+                    if (delete e[t], o.parentNode && o.parentNode.removeChild(o), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                d = setTimeout(p.bind(null, void 0, {
+                s = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
-                    target: a
+                    target: o
                 }), 12e4);
-            a.onerror = p.bind(null, a.onerror), a.onload = p.bind(null, a.onload), l && document.head.appendChild(a)
+            o.onerror = f.bind(null, o.onerror), o.onload = f.bind(null, o.onload), l && document.head.appendChild(o)
         }
     }, y.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         y.S = {};
         var e = {},
             r = {};
         y.I = (t, n) => {
             n || (n = []);
-            var o = r[t];
-            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
-                if (n.push(o), e[t]) return e[t];
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
+                if (n.push(a), e[t]) return e[t];
                 y.o(y.S, t) || (y.S[t] = {});
                 var i = y.S[t],
-                    a = "@amphi/pipeline-log-console",
+                    o = "@amphi/pipeline-metadata-panel",
                     l = [];
                 return "default" === t && ((e, r, t, n) => {
-                    var o = i[e] = i[e] || {},
-                        l = o[r];
-                    (!l || !l.loaded && (1 != !l.eager ? n : a > l.from)) && (o[r] = {
-                        get: () => Promise.all([y.e(444), y.e(684)]).then((() => () => y(684))),
-                        from: a,
+                    var a = i[e] = i[e] || {},
+                        l = a[r];
+                    (!l || !l.loaded && (1 != !l.eager ? n : o > l.from)) && (a[r] = {
+                        get: () => y.e(732).then((() => () => y(732))),
+                        from: o,
                         eager: !1
                     })
-                })("@amphi/pipeline-log-console", "0.2.1"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@amphi/pipeline-metadata-panel", "0.2.2"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -131,105 +129,104 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var o = e[n],
-                i = (typeof o)[0];
+            var a = e[n],
+                i = (typeof a)[0];
             if (n >= r.length) return "u" == i;
-            var a = r[n],
-                l = (typeof a)[0];
+            var o = r[n],
+                l = (typeof o)[0];
             if (i != l) return "o" == i && "n" == l || "s" == l || "u" == i;
-            if ("o" != i && "u" != i && o != a) return o < a;
+            if ("o" != i && "u" != i && a != o) return a < o;
             n++
         }
-    }, o = e => {
+    }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(l = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
-        var a = [];
+        var o = [];
         for (i = 1; i < e.length; i++) {
             var l = e[i];
-            a.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? a.pop() + " " + a.pop() : o(l))
+            o.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? o.pop() + " " + o.pop() : a(l))
         }
         return u();
 
         function u() {
-            return a.pop().replace(/^\((.+)\)$/, "$1")
+            return o.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                o = n < 0;
-            o && (n = -n - 1);
-            for (var a = 0, l = 1, u = !0;; l++, a++) {
-                var f, s, p = l < e.length ? (typeof e[l])[0] : "";
-                if (a >= r.length || "o" == (s = (typeof(f = r[a]))[0])) return !u || ("u" == p ? l > n && !o : "" == p != o);
-                if ("u" == s) {
-                    if (!u || "u" != p) return !1
+                a = n < 0;
+            a && (n = -n - 1);
+            for (var o = 0, l = 1, u = !0;; l++, o++) {
+                var p, d, f = l < e.length ? (typeof e[l])[0] : "";
+                if (o >= r.length || "o" == (d = (typeof(p = r[o]))[0])) return !u || ("u" == f ? l > n && !a : "" == f != a);
+                if ("u" == d) {
+                    if (!u || "u" != f) return !1
                 } else if (u)
-                    if (p == s)
+                    if (f == d)
                         if (l <= n) {
-                            if (f != e[l]) return !1
+                            if (p != e[l]) return !1
                         } else {
-                            if (o ? f > e[l] : f < e[l]) return !1;
-                            f != e[l] && (u = !1)
+                            if (a ? p > e[l] : p < e[l]) return !1;
+                            p != e[l] && (u = !1)
                         }
-                else if ("s" != p && "n" != p) {
-                    if (o || l <= n) return !1;
+                else if ("s" != f && "n" != f) {
+                    if (a || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || s < p != o) return !1;
+                    if (l <= n || d < f != a) return !1;
                     u = !1
-                } else "s" != p && "n" != p && (u = !1, l--)
+                } else "s" != f && "n" != f && (u = !1, l--)
             }
         }
-        var d = [],
-            c = d.pop.bind(d);
-        for (a = 1; a < e.length; a++) {
-            var h = e[a];
-            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
+        var s = [],
+            c = s.pop.bind(s);
+        for (o = 1; o < e.length; o++) {
+            var h = e[o];
+            s.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
         }
         return !!c()
-    }, a = (e, r) => {
+    }, o = (e, r) => {
         var t = y.S[e];
         if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
-        var o = l(e, t);
-        return i(n, o) || s(u(e, t, o, n)), p(e[t][o])
-    }, s = e => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", p = (e, r, t, n) => {
+        var a = l(e, t);
+        return i(n, a) || d(u(e, t, a, n)), f(e[t][a])
+    }, d = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
+    }, f = e => (e.loaded = 1, e.get()), s = (e => function(r, t, n, a) {
         var i = y.I(r);
-        return i && i.then ? i.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
-    })(((e, r, t, n) => (a(e, t), f(r, 0, t, n)))), c = {}, h = {
-        256: () => d("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
-        262: () => d("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        345: () => d("default", "react", [1, 18, 2, 0]),
-        465: () => d("default", "@jupyterlab/application", [1, 4, 1, 6]),
-        602: () => d("default", "@lumino/signaling", [1, 2, 0, 0]),
-        628: () => d("default", "react-dom", [1, 18, 2, 0]),
-        638: () => d("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
-        664: () => d("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
-        723: () => d("default", "@jupyterlab/rendermime", [1, 4, 1, 6]),
-        881: () => d("default", "@amphi/pipeline-editor", [0])
+        return i && i.then ? i.then(e.bind(e, r, y.S[r], t, n, a)) : e(r, y.S[r], t, n)
+    })(((e, r, t, n) => (o(e, t), p(r, 0, t, n)))), c = {}, h = {
+        44: () => s("default", "@jupyterlab/console", [1, 4, 1, 6]),
+        88: () => s("default", "@lumino/datagrid", [1, 2, 3, 0, , "alpha", 0]),
+        256: () => s("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
+        262: () => s("default", "@lumino/coreutils", [1, 2, 0, 0]),
+        465: () => s("default", "@jupyterlab/application", [1, 4, 1, 6]),
+        602: () => s("default", "@lumino/signaling", [1, 2, 0, 0]),
+        638: () => s("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        664: () => s("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
+        881: () => s("default", "@amphi/pipeline-editor", [0])
     }, v = {
-        684: [256, 262, 345, 465, 602, 628, 638, 664, 723, 881]
+        732: [44, 88, 256, 262, 465, 602, 638, 664, 881]
     }, m = {}, y.f.consumes = (e, r) => {
         y.o(v, e) && v[e].forEach((e => {
             if (y.o(c, e)) return r.push(c[e]);
             if (!m[e]) {
                 var t = r => {
                     c[e] = 0, y.m[e] = t => {
                         delete y.c[e], t.exports = r()
@@ -238,51 +235,51 @@
                 m[e] = !0;
                 var n = r => {
                     delete c[e], y.m[e] = t => {
                         throw delete y.c[e], r
                     }
                 };
                 try {
-                    var o = h[e]();
-                    o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
+                    var a = h[e]();
+                    a.then ? r.push(c[e] = a.then(t).catch(n)) : t(a)
                 } catch (e) {
                     n(e)
                 }
             }
         }))
     }, (() => {
         var e = {
-            96: 0
+            680: 0
         };
         y.f.j = (r, t) => {
             var n = y.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
-                    var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                    t.push(n[2] = o);
+                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
+                    t.push(n[2] = a);
                     var i = y.p + y.u(r),
-                        a = new Error;
+                        o = new Error;
                     y.l(i, (t => {
                         if (y.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var o = t && ("load" === t.type ? "missing" : t.type),
+                            var a = t && ("load" === t.type ? "missing" : t.type),
                                 i = t && t.target && t.target.src;
-                            a.message = "Loading chunk " + r + " failed.\n(" + o + ": " + i + ")", a.name = "ChunkLoadError", a.type = o, a.request = i, n[1](a)
+                            o.message = "Loading chunk " + r + " failed.\n(" + a + ": " + i + ")", o.name = "ChunkLoadError", o.type = a, o.request = i, n[1](o)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, o, [i, a, l] = t,
+                var n, a, [i, o, l] = t,
                     u = 0;
                 if (i.some((r => 0 !== e[r]))) {
-                    for (n in a) y.o(a, n) && (y.m[n] = a[n]);
+                    for (n in o) y.o(o, n) && (y.m[n] = o[n]);
                     l && l(y)
                 }
-                for (r && r(t); u < i.length; u++) o = i[u], y.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); u < i.length; u++) a = i[u], y.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
-            t = self.webpackChunk_amphi_pipeline_log_console = self.webpackChunk_amphi_pipeline_log_console || [];
+            t = self.webpackChunk_amphi_pipeline_metadata_panel = self.webpackChunk_amphi_pipeline_metadata_panel || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), y.nc = void 0;
-    var w = y(383);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amphi/pipeline-log-console"] = w
+    var w = y(320);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amphi/pipeline-metadata-panel"] = w
 })();
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-log-console/static/third-party-licenses.json` & `jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967105263157895%*

 * *Differences: {"'packages'": "{1: {'versionInfo': '1.20.0'}, 32: {'versionInfo': '3.11.5'}}"}*

```diff
@@ -6,15 +6,15 @@
             "name": "@ant-design/colors",
             "versionInfo": "7.0.2"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2019-present afc163\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the \"Software\"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@ant-design/cssinjs",
-            "versionInfo": "1.19.1"
+            "versionInfo": "1.20.0"
         },
         {
             "extractedText": "MIT LICENSE\n\nCopyright (c) 2018-present Ant UED, https://xtech.antfin.com/\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@ant-design/icons",
             "versionInfo": "5.3.6"
         },
@@ -192,15 +192,15 @@
             "name": "rc-util",
             "versionInfo": "5.39.1"
         },
         {
             "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "rc-virtual-list",
-            "versionInfo": "3.11.4"
+            "versionInfo": "3.11.5"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react-is",
             "versionInfo": "18.2.0"
         },
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-metadata-panel/package.json` & `jupyterlab_amphi-0.2.2/amphi/pipeline-metadata-panel/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.d7f8174936e132a8b035.js'}}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -51,15 +51,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.d15f4d692407bd368832.js",
+            "load": "static/remoteEntry.d7f8174936e132a8b035.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-metadata-panel",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
@@ -95,9 +95,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-metadata-panel/static/432.1dff82965ae8eeafd45c.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-metadata-panel/static/732.5ee1843a7c6f18d4f9f9.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-metadata-panel/static/732.5ee1843a7c6f18d4f9f9.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-metadata-panel/static/remoteEntry.d15f4d692407bd368832.js` & `jupyterlab_amphi-0.2.2/amphi/pipeline-log-console/static/remoteEntry.de9bf8c4ac18d1151373.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,31 +1,31 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, i, o, l, u, p, d, f, s, c, h, v, m, g = {
-            320: (e, r, t) => {
+    var e, r, t, n, o, a, i, l, u, s, p, f, d, c, h, v, m, g = {
+            383: (e, r, t) => {
                 var n = {
-                        "./index": () => t.e(732).then((() => () => t(732))),
-                        "./extension": () => t.e(732).then((() => () => t(732))),
+                        "./index": () => Promise.all([t.e(444), t.e(684)]).then((() => () => t(684))),
+                        "./extension": () => Promise.all([t.e(444), t.e(684)]).then((() => () => t(684))),
                         "./style": () => t.e(432).then((() => () => t(432)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    i = (e, r) => {
+                    a = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                o = t.S[n];
+                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
-                    init: () => i
+                    get: () => o,
+                    init: () => a
                 })
             }
         },
         b = {};
 
     function y(e) {
         var r = b[e];
@@ -43,78 +43,80 @@
         }), r
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
-        432: "1dff82965ae8eeafd45c",
-        732: "5ee1843a7c6f18d4f9f9"
+        432: "a6577eba0279cb4b76e3",
+        444: "35926916905e9c76b8c9",
+        684: "2b2213062b13c7490a61"
     } [e] + ".js?v=" + {
-        432: "1dff82965ae8eeafd45c",
-        732: "5ee1843a7c6f18d4f9f9"
+        432: "a6577eba0279cb4b76e3",
+        444: "35926916905e9c76b8c9",
+        684: "2b2213062b13c7490a61"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-metadata-panel:", y.l = (t, n, a, i) => {
+    }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-log-console:", y.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
-            var o, l;
-            if (void 0 !== a)
-                for (var u = document.getElementsByTagName("script"), p = 0; p < u.length; p++) {
-                    var d = u[p];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + a) {
-                        o = d;
+            var i, l;
+            if (void 0 !== o)
+                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
+                    var p = u[s];
+                    if (p.getAttribute("src") == t || p.getAttribute("data-webpack") == r + o) {
+                        i = p;
                         break
                     }
                 }
-            o || (l = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, y.nc && o.setAttribute("nonce", y.nc), o.setAttribute("data-webpack", r + a), o.src = t), e[t] = [n];
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, y.nc && i.setAttribute("nonce", y.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
             var f = (r, n) => {
-                    o.onerror = o.onload = null, clearTimeout(s);
-                    var a = e[t];
-                    if (delete e[t], o.parentNode && o.parentNode.removeChild(o), a && a.forEach((e => e(n))), r) return r(n)
+                    i.onerror = i.onload = null, clearTimeout(d);
+                    var o = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                s = setTimeout(f.bind(null, void 0, {
+                d = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
-                    target: o
+                    target: i
                 }), 12e4);
-            o.onerror = f.bind(null, o.onerror), o.onload = f.bind(null, o.onload), l && document.head.appendChild(o)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, y.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         y.S = {};
         var e = {},
             r = {};
         y.I = (t, n) => {
             n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+            var o = r[t];
+            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
+                if (n.push(o), e[t]) return e[t];
                 y.o(y.S, t) || (y.S[t] = {});
-                var i = y.S[t],
-                    o = "@amphi/pipeline-metadata-panel",
+                var a = y.S[t],
+                    i = "@amphi/pipeline-log-console",
                     l = [];
                 return "default" === t && ((e, r, t, n) => {
-                    var a = i[e] = i[e] || {},
-                        l = a[r];
-                    (!l || !l.loaded && (1 != !l.eager ? n : o > l.from)) && (a[r] = {
-                        get: () => y.e(732).then((() => () => y(732))),
-                        from: o,
+                    var o = a[e] = a[e] || {},
+                        l = o[r];
+                    (!l || !l.loaded && (1 != !l.eager ? n : i > l.from)) && (o[r] = {
+                        get: () => Promise.all([y.e(444), y.e(684)]).then((() => () => y(684))),
+                        from: i,
                         eager: !1
                     })
-                })("@amphi/pipeline-metadata-panel", "0.2.1"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@amphi/pipeline-log-console", "0.2.2"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -129,104 +131,105 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                i = (typeof a)[0];
-            if (n >= r.length) return "u" == i;
-            var o = r[n],
-                l = (typeof o)[0];
-            if (i != l) return "o" == i && "n" == l || "s" == l || "u" == i;
-            if ("o" != i && "u" != i && a != o) return a < o;
+            var o = e[n],
+                a = (typeof o)[0];
+            if (n >= r.length) return "u" == a;
+            var i = r[n],
+                l = (typeof i)[0];
+            if (a != l) return "o" == a && "n" == l || "s" == l || "u" == a;
+            if ("o" != a && "u" != a && o != i) return o < i;
             n++
         }
-    }, a = e => {
+    }, o = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(l = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
+            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(l = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
-        var o = [];
-        for (i = 1; i < e.length; i++) {
-            var l = e[i];
-            o.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? o.pop() + " " + o.pop() : a(l))
+        var i = [];
+        for (a = 1; a < e.length; a++) {
+            var l = e[a];
+            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
         }
         return u();
 
         function u() {
-            return o.pop().replace(/^\((.+)\)$/, "$1")
+            return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, i = (e, r) => {
+    }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
-            for (var o = 0, l = 1, u = !0;; l++, o++) {
-                var p, d, f = l < e.length ? (typeof e[l])[0] : "";
-                if (o >= r.length || "o" == (d = (typeof(p = r[o]))[0])) return !u || ("u" == f ? l > n && !a : "" == f != a);
-                if ("u" == d) {
+                o = n < 0;
+            o && (n = -n - 1);
+            for (var i = 0, l = 1, u = !0;; l++, i++) {
+                var s, p, f = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (p = (typeof(s = r[i]))[0])) return !u || ("u" == f ? l > n && !o : "" == f != o);
+                if ("u" == p) {
                     if (!u || "u" != f) return !1
                 } else if (u)
-                    if (f == d)
+                    if (f == p)
                         if (l <= n) {
-                            if (p != e[l]) return !1
+                            if (s != e[l]) return !1
                         } else {
-                            if (a ? p > e[l] : p < e[l]) return !1;
-                            p != e[l] && (u = !1)
+                            if (o ? s > e[l] : s < e[l]) return !1;
+                            s != e[l] && (u = !1)
                         }
                 else if ("s" != f && "n" != f) {
-                    if (a || l <= n) return !1;
+                    if (o || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || d < f != a) return !1;
+                    if (l <= n || p < f != o) return !1;
                     u = !1
                 } else "s" != f && "n" != f && (u = !1, l--)
             }
         }
-        var s = [],
-            c = s.pop.bind(s);
-        for (o = 1; o < e.length; o++) {
-            var h = e[o];
-            s.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
+        var d = [],
+            c = d.pop.bind(d);
+        for (i = 1; i < e.length; i++) {
+            var h = e[i];
+            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
         return !!c()
-    }, o = (e, r) => {
+    }, i = (e, r) => {
         var t = y.S[e];
         if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", p = (e, r, t, n) => {
-        var a = l(e, t);
-        return i(n, a) || d(u(e, t, a, n)), f(e[t][a])
-    }, d = e => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
+        var o = l(e, t);
+        return a(n, o) || p(u(e, t, o, n)), f(e[t][o])
+    }, p = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, f = e => (e.loaded = 1, e.get()), s = (e => function(r, t, n, a) {
-        var i = y.I(r);
-        return i && i.then ? i.then(e.bind(e, r, y.S[r], t, n, a)) : e(r, y.S[r], t, n)
-    })(((e, r, t, n) => (o(e, t), p(r, 0, t, n)))), c = {}, h = {
-        44: () => s("default", "@jupyterlab/console", [1, 4, 1, 6]),
-        88: () => s("default", "@lumino/datagrid", [1, 2, 3, 0, , "alpha", 0]),
-        256: () => s("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
-        262: () => s("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        465: () => s("default", "@jupyterlab/application", [1, 4, 1, 6]),
-        602: () => s("default", "@lumino/signaling", [1, 2, 0, 0]),
-        638: () => s("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
-        664: () => s("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
-        881: () => s("default", "@amphi/pipeline-editor", [0])
+    }, f = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
+        var a = y.I(r);
+        return a && a.then ? a.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), c = {}, h = {
+        256: () => d("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
+        262: () => d("default", "@lumino/coreutils", [1, 2, 0, 0]),
+        345: () => d("default", "react", [1, 18, 2, 0]),
+        465: () => d("default", "@jupyterlab/application", [1, 4, 1, 6]),
+        602: () => d("default", "@lumino/signaling", [1, 2, 0, 0]),
+        628: () => d("default", "react-dom", [1, 18, 2, 0]),
+        638: () => d("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        664: () => d("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
+        723: () => d("default", "@jupyterlab/rendermime", [1, 4, 1, 6]),
+        881: () => d("default", "@amphi/pipeline-editor", [0])
     }, v = {
-        732: [44, 88, 256, 262, 465, 602, 638, 664, 881]
+        684: [256, 262, 345, 465, 602, 628, 638, 664, 723, 881]
     }, m = {}, y.f.consumes = (e, r) => {
         y.o(v, e) && v[e].forEach((e => {
             if (y.o(c, e)) return r.push(c[e]);
             if (!m[e]) {
                 var t = r => {
                     c[e] = 0, y.m[e] = t => {
                         delete y.c[e], t.exports = r()
@@ -235,51 +238,51 @@
                 m[e] = !0;
                 var n = r => {
                     delete c[e], y.m[e] = t => {
                         throw delete y.c[e], r
                     }
                 };
                 try {
-                    var a = h[e]();
-                    a.then ? r.push(c[e] = a.then(t).catch(n)) : t(a)
+                    var o = h[e]();
+                    o.then ? r.push(c[e] = o.then(t).catch(n)) : t(o)
                 } catch (e) {
                     n(e)
                 }
             }
         }))
     }, (() => {
         var e = {
-            680: 0
+            96: 0
         };
         y.f.j = (r, t) => {
             var n = y.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
-                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                    t.push(n[2] = a);
-                    var i = y.p + y.u(r),
-                        o = new Error;
-                    y.l(i, (t => {
+                    var o = new Promise(((t, o) => n = e[r] = [t, o]));
+                    t.push(n[2] = o);
+                    var a = y.p + y.u(r),
+                        i = new Error;
+                    y.l(a, (t => {
                         if (y.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                            var a = t && ("load" === t.type ? "missing" : t.type),
-                                i = t && t.target && t.target.src;
-                            o.message = "Loading chunk " + r + " failed.\n(" + a + ": " + i + ")", o.name = "ChunkLoadError", o.type = a, o.request = i, n[1](o)
+                            var o = t && ("load" === t.type ? "missing" : t.type),
+                                a = t && t.target && t.target.src;
+                            i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var n, a, [i, o, l] = t,
+                var n, o, [a, i, l] = t,
                     u = 0;
-                if (i.some((r => 0 !== e[r]))) {
-                    for (n in o) y.o(o, n) && (y.m[n] = o[n]);
+                if (a.some((r => 0 !== e[r]))) {
+                    for (n in i) y.o(i, n) && (y.m[n] = i[n]);
                     l && l(y)
                 }
-                for (r && r(t); u < i.length; u++) a = i[u], y.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); u < a.length; u++) o = a[u], y.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
-            t = self.webpackChunk_amphi_pipeline_metadata_panel = self.webpackChunk_amphi_pipeline_metadata_panel || [];
+            t = self.webpackChunk_amphi_pipeline_log_console = self.webpackChunk_amphi_pipeline_log_console || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), y.nc = void 0;
-    var w = y(320);
-    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amphi/pipeline-metadata-panel"] = w
+    var w = y(383);
+    (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amphi/pipeline-log-console"] = w
 })();
```

### Comparing `jupyterlab_amphi-0.2.1/amphi/pipeline-metadata-panel/static/third-party-licenses.json` & `jupyterlab_amphi-0.2.2/amphi/pipeline-metadata-panel/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -88,9 +88,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/tsconfig.json` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/BrowseFileDialog.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/BrowseFileDialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/CodeGenerator.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/CodeGenerator.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/CustomHandle.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/CustomHandle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/PipelineComponent.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/PipelineComponent.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/PipelineService.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/PipelineService.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/RequestService.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/RequestService.tsx`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
           future2.onIOPub = msg => {
             if (msg.header.msg_type === 'stream') {
 
               const streamMsg = msg as KernelMessage.IStreamMsg;
               console.log("receive stream %o", streamMsg)
 
               const output = streamMsg.content.text;
-              
-              const regex = /(\w+)\s+\(([^,]+),\s*(named|unnamed)\)/g;
+
+              const regex = /([^\s,]+)\s+\(([^,]+),\s*(named|unnamed)\)/g;
               const newItems = [];
               
               let match;
               while ((match = regex.exec(output)) !== null) {
                 const [_, name, type, namedStatus] = match;
                 newItems.push({
                   value: name,
```

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/configUtils.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/configUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/icons.ts` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/index.ts` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/rendererUtils.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/rendererUtils.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/keyValueForm.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/keyValueForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/selectColumn.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/selectColumn.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/selectColumns.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/selectColumns.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/selectMultiple.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/selectMultiple.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/selectRegular.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/selectRegular.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/selectTokenization.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/selectTokenization.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/transferData.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/transferData.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/src/forms/valuesListForm.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/src/forms/valuesListForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/settings-16.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/settings-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/settings-24.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/settings-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/trash-16.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/trash-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/trash-24.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/trash-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-components-manager/style/icons/x-square-16.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-components-manager/style/icons/x-square-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/package.json` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761904761904762%*

 * *Differences: {"'version'": "'0.2.2'"}*

```diff
@@ -97,9 +97,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/pipeline-16.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/pipeline-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/pipeline-24.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/pipeline-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/tsconfig.json` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/schema/plugin copy.json` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/schema/plugin copy.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/schema/plugin.json` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/src/Dropzone.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/src/Dropzone.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/src/PipelineEditorWidget.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/src/PipelineEditorWidget.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/src/customEdge.tsx` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/src/customEdge.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/src/icons.ts` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/src/index.ts` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/canvas.css` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/canvas.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/output.css` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/output.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/pipeline-category-icon.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/pipeline-category-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/react-icon.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/react-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/icons/api-24.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/icons/api-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/icons/file-plus-24.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/icons/file-plus-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/icons/file-text-24.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/icons/file-text-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/icons/pipeline-brand-16.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/icons/pipeline-brand-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/packages/pipeline-editor/style/icons/pipeline-brand-24.svg` & `jupyterlab_amphi-0.2.2/packages/pipeline-editor/style/icons/pipeline-brand-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/LICENSE` & `jupyterlab_amphi-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/README.md` & `jupyterlab_amphi-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/pyproject.toml` & `jupyterlab_amphi-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.2.1/PKG-INFO` & `jupyterlab_amphi-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-amphi
-Version: 0.2.1
+Version: 0.2.2
 Dynamic: Keywords
 Summary: Amphi is a micro ETL for Jupyterlab.
 Project-URL: Homepage, https://amphi.ai
 Project-URL: Bug Tracker, https://github.com/amphi-ai/jupyterlab-amphi/issues
 Project-URL: Repository, https://github.com/amphi-ai/jupyterlab-amphi.git
 Author-email: Thibaut Gourdel <tgourdel@amphi.ai>
 License: Elastic License 2.0 \(ELv2\)
```

