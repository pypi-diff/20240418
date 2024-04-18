# Comparing `tmp/pyconcept-0.1.0.tar.gz` & `tmp/pyconcept-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconcept-0.1.0.tar", last modified: Wed Apr 17 11:42:23 2024, max compression
+gzip compressed data, was "pyconcept-0.1.1.tar", last modified: Wed Apr 17 18:56:45 2024, max compression
```

## Comparing `pyconcept-0.1.0.tar` & `pyconcept-0.1.1.tar`

### file list

```diff
@@ -1,281 +1,281 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.553054 pyconcept-0.1.0/
--rw-rw-rw-   0        0        0     1190 2024-04-16 20:18:58.000000 pyconcept-0.1.0/CMakeLists.txt
--rw-rw-rw-   0        0        0     1101 2024-04-15 19:05:00.000000 pyconcept-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      149 2024-04-17 11:32:07.000000 pyconcept-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      844 2024-04-17 11:42:23.553054 pyconcept-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      115 2024-04-17 11:33:45.000000 pyconcept-0.1.0/README.md
--rw-rw-rw-   0        0        0        5 2024-04-17 11:40:17.000000 pyconcept-0.1.0/VERSION
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.085393 pyconcept-0.1.0/ccl/
--rw-rw-rw-   0        0        0     2133 2024-04-17 08:48:56.000000 pyconcept-0.1.0/ccl/CMakeLists.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.055389 pyconcept-0.1.0/ccl/cclCommons/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.055389 pyconcept-0.1.0/ccl/cclCommons/include/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.101390 pyconcept-0.1.0/ccl/cclCommons/include/ccl/
--rw-rw-rw-   0        0        0    10473 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclCommons/include/ccl/Strings.hpp
--rw-rw-rw-   0        0        0      895 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclCommons/include/ccl/Substitutes.hpp
--rw-rw-rw-   0        0        0     1506 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclCommons/include/ccl/cclChange.hpp
--rw-rw-rw-   0        0        0    11710 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclCommons/include/ccl/cclMeta.hpp
--rw-rw-rw-   0        0        0     6078 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclCommons/include/ccl/cclTypes.hpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.056389 pyconcept-0.1.0/ccl/cclGraph/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.056389 pyconcept-0.1.0/ccl/cclGraph/include/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.102388 pyconcept-0.1.0/ccl/cclGraph/include/ccl/
--rw-rw-rw-   0        0        0     2749 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclGraph/include/ccl/Entity.hpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.103389 pyconcept-0.1.0/ccl/cclGraph/include/ccl/graph/
--rw-rw-rw-   0        0        0     2907 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclGraph/include/ccl/graph/CGraph.h
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.105391 pyconcept-0.1.0/ccl/cclGraph/src/
--rw-rw-rw-   0        0        0     9186 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclGraph/src/CGraph.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.058394 pyconcept-0.1.0/ccl/cclLang/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.057388 pyconcept-0.1.0/ccl/cclLang/include/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.057388 pyconcept-0.1.0/ccl/cclLang/include/ccl/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.115390 pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/
--rw-rw-rw-   0        0        0     1191 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp
--rw-rw-rw-   0        0        0     1941 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/LexicalTerm.h
--rw-rw-rw-   0        0        0      345 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/Literals.h
--rw-rw-rw-   0        0        0     1327 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/ManagedText.h
--rw-rw-rw-   0        0        0     8108 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/Morphology.h
--rw-rw-rw-   0        0        0     2748 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/Reference.h
--rw-rw-rw-   0        0        0     2766 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/RefsManager.h
--rw-rw-rw-   0        0        0      514 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/TextEnvironment.h
--rw-rw-rw-   0        0        0     1278 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/TextProcessor.h
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.122388 pyconcept-0.1.0/ccl/cclLang/src/
--rw-rw-rw-   0        0        0     2111 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/src/LexicalTerm.cpp
--rw-rw-rw-   0        0        0      307 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/src/Literals.cpp
--rw-rw-rw-   0        0        0     2016 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/src/ManagedText.cpp
--rw-rw-rw-   0        0        0     2239 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/src/Morphology.cpp
--rw-rw-rw-   0        0        0     7462 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/src/Reference.cpp
--rw-rw-rw-   0        0        0     6535 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/src/RefsManager.cpp
--rw-rw-rw-   0        0        0      452 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/src/TextEnvironment.cpp
--rw-rw-rw-   0        0        0     1581 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/src/TextProcessor.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.122388 pyconcept-0.1.0/ccl/cclLang/unity/
--rw-rw-rw-   0        0        0      309 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cclLang/unity/cclLang.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.123388 pyconcept-0.1.0/ccl/cmake/
--rw-rw-rw-   0        0        0     1541 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/cmake/CXXTargets.cmake
--rw-rw-rw-   0        0        0       93 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/conanfile.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.063391 pyconcept-0.1.0/ccl/core/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.060393 pyconcept-0.1.0/ccl/core/include/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.125388 pyconcept-0.1.0/ccl/core/include/ccl/
--rw-rw-rw-   0        0        0     2124 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/Operation.hpp
--rw-rw-rw-   0        0        0     5309 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/Source.hpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.126386 pyconcept-0.1.0/ccl/core/include/ccl/api/
--rw-rw-rw-   0        0        0      915 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/api/RSFormJA.h
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.128387 pyconcept-0.1.0/ccl/core/include/ccl/env/
--rw-rw-rw-   0        0        0     2904 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/env/SourceManager.hpp
--rw-rw-rw-   0        0        0      624 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/env/cclEnvironment.h
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.131389 pyconcept-0.1.0/ccl/core/include/ccl/ops/
--rw-rw-rw-   0        0        0     1998 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/ops/EquationOptions.h
--rw-rw-rw-   0        0        0      850 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/ops/RSAggregator.h
--rw-rw-rw-   0        0        0     1187 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/ops/RSEquationProcessor.h
--rw-rw-rw-   0        0        0     3525 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/ops/RSOperations.h
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.137385 pyconcept-0.1.0/ccl/core/include/ccl/oss/
--rw-rw-rw-   0        0        0     4161 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/oss/OSSchema.h
--rw-rw-rw-   0        0        0     1658 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/oss/OperationProcessor.hpp
--rw-rw-rw-   0        0        0      903 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/oss/Pict.hpp
--rw-rw-rw-   0        0        0      934 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/oss/RSSynthesProcessor.h
--rw-rw-rw-   0        0        0     1363 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/oss/ossGraphFacet.h
--rw-rw-rw-   0        0        0     2334 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/oss/ossGridFacet.h
--rw-rw-rw-   0        0        0     2979 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/oss/ossOperationsFacet.h
--rw-rw-rw-   0        0        0     2469 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/oss/ossSourceFacet.h
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.153405 pyconcept-0.1.0/ccl/core/include/ccl/semantic/
--rw-rw-rw-   0        0        0      622 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/ConceptRecord.h
--rw-rw-rw-   0        0        0     1473 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/CstFilters.hpp
--rw-rw-rw-   0        0        0     2367 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/CstList.h
--rw-rw-rw-   0        0        0     2523 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/CstType.hpp
--rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/IdentityManager.h
--rw-rw-rw-   0        0        0      962 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/InterpretationStorage.h
--rw-rw-rw-   0        0        0     1069 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/RSConcept.h
--rw-rw-rw-   0        0        0     3584 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/RSCore.h
--rw-rw-rw-   0        0        0     3437 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/RSForm.h
--rw-rw-rw-   0        0        0     3019 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/RSModel.h
--rw-rw-rw-   0        0        0     5074 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/Schema.h
--rw-rw-rw-   0        0        0     1122 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/TextConcept.h
--rw-rw-rw-   0        0        0     2603 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/TextData.hpp
--rw-rw-rw-   0        0        0     3988 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/Thesaurus.h
--rw-rw-rw-   0        0        0     1577 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/rsCalculationFacet.h
--rw-rw-rw-   0        0        0     1648 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/rsModificationFacet.h
--rw-rw-rw-   0        0        0     1099 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/rsOperationFacet.h
--rw-rw-rw-   0        0        0     1867 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/semantic/rsValuesFacet.h
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.157387 pyconcept-0.1.0/ccl/core/include/ccl/tools/
--rw-rw-rw-   0        0        0      894 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/tools/CstNameGenerator.h
--rw-rw-rw-   0        0        0      523 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/tools/EntityGenerator.h
--rw-rw-rw-   0        0        0     2935 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/tools/EnumJSON.hpp
--rw-rw-rw-   0        0        0     3871 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/ccl/tools/JSON.h
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.158388 pyconcept-0.1.0/ccl/core/include/nlohmann/
--rw-rw-rw-   0        0        0   945021 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/include/nlohmann/json.hpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.160389 pyconcept-0.1.0/ccl/core/src/
--rw-rw-rw-   0        0        0    18448 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/JSON.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.161387 pyconcept-0.1.0/ccl/core/src/api/
--rw-rw-rw-   0        0        0     3026 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/api/RSFormJA.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.162387 pyconcept-0.1.0/ccl/core/src/env/
--rw-rw-rw-   0        0        0      636 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/env/cclEnvironment.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.165387 pyconcept-0.1.0/ccl/core/src/ops/
--rw-rw-rw-   0        0        0     1764 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/ops/EquationOptions.cpp
--rw-rw-rw-   0        0        0     4124 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/ops/RSAggregator.cpp
--rw-rw-rw-   0        0        0     4290 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/ops/RSEquationProcessor.cpp
--rw-rw-rw-   0        0        0    16240 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/ops/RSOperations.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.169390 pyconcept-0.1.0/ccl/core/src/oss/
--rw-rw-rw-   0        0        0     7275 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/oss/OSSchema.cpp
--rw-rw-rw-   0        0        0     2812 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/oss/RSSynthesProcessor.cpp
--rw-rw-rw-   0        0        0     4326 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/oss/ossGraphFacet.cpp
--rw-rw-rw-   0        0        0     3023 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/oss/ossGridFacet.cpp
--rw-rw-rw-   0        0        0    11663 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/oss/ossOperationsFacet.cpp
--rw-rw-rw-   0        0        0    10397 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/oss/ossSourceFacet.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.063391 pyconcept-0.1.0/ccl/core/src/semantic/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.173387 pyconcept-0.1.0/ccl/core/src/semantic/rscore/
--rw-rw-rw-   0        0        0      588 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/rscore/ConceptRecord.cpp
--rw-rw-rw-   0        0        0     3957 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/rscore/CstList.cpp
--rw-rw-rw-   0        0        0     1950 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/rscore/IdentityManager.cpp
--rw-rw-rw-   0        0        0    10261 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/rscore/RSCore.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.175386 pyconcept-0.1.0/ccl/core/src/semantic/rsform/
--rw-rw-rw-   0        0        0     8112 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/rsform/RSForm.cpp
--rw-rw-rw-   0        0        0     1573 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/rsform/rsModificationFacet.cpp
--rw-rw-rw-   0        0        0     2431 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/rsform/rsOperationFacet.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.179389 pyconcept-0.1.0/ccl/core/src/semantic/rsmodel/
--rw-rw-rw-   0        0        0     1591 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp
--rw-rw-rw-   0        0        0     4755 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/rsmodel/RSModel.cpp
--rw-rw-rw-   0        0        0     3954 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp
--rw-rw-rw-   0        0        0     6819 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.180389 pyconcept-0.1.0/ccl/core/src/semantic/schema/
--rw-rw-rw-   0        0        0      830 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/schema/RSConcept.cpp
--rw-rw-rw-   0        0        0    13468 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/schema/Schema.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.182386 pyconcept-0.1.0/ccl/core/src/semantic/thesaurus/
--rw-rw-rw-   0        0        0      919 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/thesaurus/TextConcept.cpp
--rw-rw-rw-   0        0        0    10089 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/semantic/thesaurus/Thesaurus.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.183387 pyconcept-0.1.0/ccl/core/src/tools/
--rw-rw-rw-   0        0        0     2682 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/tools/CstNameGenerator.cpp
--rw-rw-rw-   0        0        0      773 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/src/tools/EntityGenerator.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.184389 pyconcept-0.1.0/ccl/core/unity/
--rw-rw-rw-   0        0        0     1448 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/core/unity/CCL.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.068387 pyconcept-0.1.0/ccl/rslang/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.198388 pyconcept-0.1.0/ccl/rslang/header/
--rw-rw-rw-   0        0        0     1362 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/header/ASTNormalizer.h
--rw-rw-rw-   0        0        0    34735 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/header/AsciiLexerImpl.hpp
--rw-rw-rw-   0        0        0     2359 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/header/GeneratorImplAST.h
--rw-rw-rw-   0        0        0    35507 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/header/MathLexerImpl.hpp
--rw-rw-rw-   0        0        0      958 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/header/NameCollector.h
--rw-rw-rw-   0        0        0    22132 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/header/RSParserImpl.h
--rw-rw-rw-   0        0        0     5452 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/header/SDImplementation.h
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.064391 pyconcept-0.1.0/ccl/rslang/import/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.066390 pyconcept-0.1.0/ccl/rslang/import/reflex/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.065393 pyconcept-0.1.0/ccl/rslang/import/reflex/include/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.265386 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/
--rw-rw-rw-   0        0        0    16072 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/abslexer.h
--rw-rw-rw-   0        0        0    69252 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/absmatcher.h
--rw-rw-rw-   0        0        0    18001 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/bits.h
--rw-rw-rw-   0        0        0    19348 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/boostmatcher.h
--rw-rw-rw-   0        0        0    11147 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/convert.h
--rw-rw-rw-   0        0        0     6862 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/debug.h
--rw-rw-rw-   0        0        0     6978 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/error.h
--rw-rw-rw-   0        0        0    24462 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/flexlexer.h
--rw-rw-rw-   0        0        0    38598 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/input.h
--rw-rw-rw-   0        0        0     6354 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/linematcher.h
--rw-rw-rw-   0        0        0    15401 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/matcher.h
--rw-rw-rw-   0        0        0    45834 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/pattern.h
--rw-rw-rw-   0        0        0    20060 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h
--rw-rw-rw-   0        0        0     2948 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/posix.h
--rw-rw-rw-   0        0        0    37159 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/ranges.h
--rw-rw-rw-   0        0        0    12093 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/setop.h
--rw-rw-rw-   0        0        0     4594 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/simd.h
--rw-rw-rw-   0        0        0    22985 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/stdmatcher.h
--rw-rw-rw-   0        0        0     4244 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/timer.h
--rw-rw-rw-   0        0        0     3159 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/traits.h
--rw-rw-rw-   0        0        0     2997 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/unicode.h
--rw-rw-rw-   0        0        0     9522 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/utf8.h
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.306387 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/
--rw-rw-rw-   0        0        0    78708 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/convert.cpp
--rw-rw-rw-   0        0        0     3792 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/debug.cpp
--rw-rw-rw-   0        0        0     5896 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/error.cpp
--rw-rw-rw-   0        0        0    84320 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/input.cpp
--rw-rw-rw-   0        0        0   116725 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/matcher.cpp
--rw-rw-rw-   0        0        0     2693 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/matcher_avx2.cpp
--rw-rw-rw-   0        0        0     2715 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp
--rw-rw-rw-   0        0        0   155001 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/pattern.cpp
--rw-rw-rw-   0        0        0     4261 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/posix.cpp
--rw-rw-rw-   0        0        0     5046 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/simd_avx2.cpp
--rw-rw-rw-   0        0        0     3478 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp
--rw-rw-rw-   0        0        0     5118 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/unicode.cpp
--rw-rw-rw-   0        0        0     8872 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/lib/utf8.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.335387 pyconcept-0.1.0/ccl/rslang/import/reflex/unicode/
--rw-rw-rw-   0        0        0    38187 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/unicode/block_scripts.cpp
--rw-rw-rw-   0        0        0    30273 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/unicode/composer.cpp
--rw-rw-rw-   0        0        0   223308 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/unicode/language_scripts.cpp
--rw-rw-rw-   0        0        0    23072 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/import/reflex/unicode/letter_scripts.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.067390 pyconcept-0.1.0/ccl/rslang/include/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.068387 pyconcept-0.1.0/ccl/rslang/include/ccl/
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.441392 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/
--rw-rw-rw-   0        0        0     3600 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/ASTInterpreter.h
--rw-rw-rw-   0        0        0     1048 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/AsciiLexer.h
--rw-rw-rw-   0        0        0      963 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/Auditor.h
--rw-rw-rw-   0        0        0      317 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/DataContext.hpp
--rw-rw-rw-   0        0        0     1120 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/Error.hpp
--rw-rw-rw-   0        0        0      555 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/ErrorLogger.h
--rw-rw-rw-   0        0        0      848 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/Interpreter.h
--rw-rw-rw-   0        0        0     2192 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/LexerBase.hpp
--rw-rw-rw-   0        0        0      254 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/Literals.h
--rw-rw-rw-   0        0        0      998 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/MathLexer.h
--rw-rw-rw-   0        0        0      927 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/Parser.h
--rw-rw-rw-   0        0        0     1526 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/ParserState.hpp
--rw-rw-rw-   0        0        0     6805 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp
--rw-rw-rw-   0        0        0     1102 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/RSExpr.h
--rw-rw-rw-   0        0        0     1651 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/RSGenerator.h
--rw-rw-rw-   0        0        0      869 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/RSParser.h
--rw-rw-rw-   0        0        0     4689 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/RSToken.h
--rw-rw-rw-   0        0        0     1117 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/SDataCompact.h
--rw-rw-rw-   0        0        0     1953 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/Structure.hpp
--rw-rw-rw-   0        0        0     4776 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/StructuredData.h
--rw-rw-rw-   0        0        0    12948 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/SyntaxTree.h
--rw-rw-rw-   0        0        0     5270 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/TypeAuditor.h
--rw-rw-rw-   0        0        0     1520 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/TypeContext.hpp
--rw-rw-rw-   0        0        0     3754 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/Typification.h
--rw-rw-rw-   0        0        0     4297 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/ValueAuditor.h
--rw-rw-rw-   0        0        0      314 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/ValueClass.hpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.519641 pyconcept-0.1.0/ccl/rslang/src/
--rw-rw-rw-   0        0        0    19985 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/ASTInterpreter.cpp
--rw-rw-rw-   0        0        0     5997 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/ASTNormalizer.cpp
--rw-rw-rw-   0        0        0     2219 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/AsciiLexer.cpp
--rw-rw-rw-   0        0        0     1238 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/Auditor.cpp
--rw-rw-rw-   0        0        0     1413 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/ErrorLogger.cpp
--rw-rw-rw-   0        0        0     7204 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/GeneratorImplAST.cpp
--rw-rw-rw-   0        0        0     1115 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/Interpreter.cpp
--rw-rw-rw-   0        0        0     2046 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/Literals.cpp
--rw-rw-rw-   0        0        0     2316 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/MathLexer.cpp
--rw-rw-rw-   0        0        0     3273 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/NameCollector.cpp
--rw-rw-rw-   0        0        0     3907 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/Parser.cpp
--rw-rw-rw-   0        0        0     3409 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/RSExpr.cpp
--rw-rw-rw-   0        0        0     8152 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/RSGenerator.cpp
--rw-rw-rw-   0        0        0     8280 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/RSParser.cpp
--rw-rw-rw-   0        0        0    60161 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/RSParserImpl.cpp
--rw-rw-rw-   0        0        0    11051 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/RSToken.cpp
--rw-rw-rw-   0        0        0     6882 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/SDImplementation.cpp
--rw-rw-rw-   0        0        0     7535 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/SDataCompact.cpp
--rw-rw-rw-   0        0        0    10421 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/StructuredData.cpp
--rw-rw-rw-   0        0        0     6353 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/SyntaxTree.cpp
--rw-rw-rw-   0        0        0    29818 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/TypeAuditor.cpp
--rw-rw-rw-   0        0        0     3844 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/Typification.cpp
--rw-rw-rw-   0        0        0     6264 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/src/ValueAuditor.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.539528 pyconcept-0.1.0/ccl/rslang/unity/
--rw-rw-rw-   0        0        0      399 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/unity/RSlang.cpp
--rw-rw-rw-   0        0        0      458 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/unity/RSlang2.cpp
--rw-rw-rw-   0        0        0     1195 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/unity/reflex_unity1.cpp
--rw-rw-rw-   0        0        0     1776 2024-04-15 19:05:00.000000 pyconcept-0.1.0/ccl/rslang/unity/reflex_unity2.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.540069 pyconcept-0.1.0/cmake/
--rw-rw-rw-   0        0        0     1490 2024-04-15 19:05:00.000000 pyconcept-0.1.0/cmake/CXXTargets.cmake
--rw-rw-rw-   0        0        0       96 2024-04-16 20:20:08.000000 pyconcept-0.1.0/conanfile.txt
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.541146 pyconcept-0.1.0/include/
--rw-rw-rw-   0        0        0     1216 2024-04-15 19:05:00.000000 pyconcept-0.1.0/include/pyconcept.h
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.552053 pyconcept-0.1.0/pyconcept.egg-info/
--rw-rw-rw-   0        0        0      844 2024-04-17 11:42:22.000000 pyconcept-0.1.0/pyconcept.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8535 2024-04-17 11:42:23.000000 pyconcept-0.1.0/pyconcept.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 11:42:22.000000 pyconcept-0.1.0/pyconcept.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-17 11:42:22.000000 pyconcept-0.1.0/pyconcept.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      146 2024-04-17 11:29:28.000000 pyconcept-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      751 2024-04-17 11:42:23.554052 pyconcept-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3826 2024-04-17 11:17:40.000000 pyconcept-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.546515 pyconcept-0.1.0/src/
--rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.0/src/pyconcept.cpp
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.548172 pyconcept-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-15 19:05:00.000000 pyconcept-0.1.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.550055 pyconcept-0.1.0/tests/__pycache__/
--rw-rw-rw-   0        0        0      148 2024-04-16 20:55:54.000000 pyconcept-0.1.0/tests/__pycache__/__init__.cpython-312.pyc
--rw-rw-rw-   0        0        0     5074 2024-04-16 20:55:54.000000 pyconcept-0.1.0/tests/__pycache__/testBinding.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-04-17 11:42:23.551054 pyconcept-0.1.0/tests/data/
--rw-rw-rw-   0        0        0     2486 2024-04-15 19:05:00.000000 pyconcept-0.1.0/tests/data/КС начальник-подчиненный.trs
--rw-rw-rw-   0        0        0     2645 2024-04-15 19:05:00.000000 pyconcept-0.1.0/tests/testBinding.py
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.403052 pyconcept-0.1.1/
+-rw-rw-rw-   0        0        0      955 2024-04-17 16:53:26.000000 pyconcept-0.1.1/CMakeLists.txt
+-rw-rw-rw-   0        0        0     1101 2024-04-15 19:05:00.000000 pyconcept-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      149 2024-04-17 11:32:07.000000 pyconcept-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      844 2024-04-17 18:56:45.403052 pyconcept-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2024-04-17 11:33:45.000000 pyconcept-0.1.1/README.md
+-rw-rw-rw-   0        0        0        5 2024-04-17 18:56:08.000000 pyconcept-0.1.1/VERSION
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.193029 pyconcept-0.1.1/ccl/
+-rw-rw-rw-   0        0        0     2133 2024-04-17 08:48:56.000000 pyconcept-0.1.1/ccl/CMakeLists.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.172030 pyconcept-0.1.1/ccl/cclCommons/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.172030 pyconcept-0.1.1/ccl/cclCommons/include/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.197028 pyconcept-0.1.1/ccl/cclCommons/include/ccl/
+-rw-rw-rw-   0        0        0    10473 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclCommons/include/ccl/Strings.hpp
+-rw-rw-rw-   0        0        0      895 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclCommons/include/ccl/Substitutes.hpp
+-rw-rw-rw-   0        0        0     1506 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclCommons/include/ccl/cclChange.hpp
+-rw-rw-rw-   0        0        0    11710 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclCommons/include/ccl/cclMeta.hpp
+-rw-rw-rw-   0        0        0     6078 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclCommons/include/ccl/cclTypes.hpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.173028 pyconcept-0.1.1/ccl/cclGraph/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.172030 pyconcept-0.1.1/ccl/cclGraph/include/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.198027 pyconcept-0.1.1/ccl/cclGraph/include/ccl/
+-rw-rw-rw-   0        0        0     2749 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclGraph/include/ccl/Entity.hpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.198027 pyconcept-0.1.1/ccl/cclGraph/include/ccl/graph/
+-rw-rw-rw-   0        0        0     2907 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclGraph/include/ccl/graph/CGraph.h
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.199030 pyconcept-0.1.1/ccl/cclGraph/src/
+-rw-rw-rw-   0        0        0     9186 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclGraph/src/CGraph.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.174028 pyconcept-0.1.1/ccl/cclLang/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.173028 pyconcept-0.1.1/ccl/cclLang/include/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.173028 pyconcept-0.1.1/ccl/cclLang/include/ccl/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.206033 pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/
+-rw-rw-rw-   0        0        0     1191 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp
+-rw-rw-rw-   0        0        0     1941 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/LexicalTerm.h
+-rw-rw-rw-   0        0        0      345 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/Literals.h
+-rw-rw-rw-   0        0        0     1327 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/ManagedText.h
+-rw-rw-rw-   0        0        0     8108 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/Morphology.h
+-rw-rw-rw-   0        0        0     2748 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/Reference.h
+-rw-rw-rw-   0        0        0     2766 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/RefsManager.h
+-rw-rw-rw-   0        0        0      514 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/TextEnvironment.h
+-rw-rw-rw-   0        0        0     1278 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/TextProcessor.h
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.216029 pyconcept-0.1.1/ccl/cclLang/src/
+-rw-rw-rw-   0        0        0     2111 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/src/LexicalTerm.cpp
+-rw-rw-rw-   0        0        0      307 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/src/Literals.cpp
+-rw-rw-rw-   0        0        0     2016 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/src/ManagedText.cpp
+-rw-rw-rw-   0        0        0     2239 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/src/Morphology.cpp
+-rw-rw-rw-   0        0        0     7462 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/src/Reference.cpp
+-rw-rw-rw-   0        0        0     6535 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/src/RefsManager.cpp
+-rw-rw-rw-   0        0        0      452 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/src/TextEnvironment.cpp
+-rw-rw-rw-   0        0        0     1581 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/src/TextProcessor.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.217029 pyconcept-0.1.1/ccl/cclLang/unity/
+-rw-rw-rw-   0        0        0      309 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cclLang/unity/cclLang.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.218031 pyconcept-0.1.1/ccl/cmake/
+-rw-rw-rw-   0        0        0     1541 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/cmake/CXXTargets.cmake
+-rw-rw-rw-   0        0        0       93 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/conanfile.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.179030 pyconcept-0.1.1/ccl/core/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.176027 pyconcept-0.1.1/ccl/core/include/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.221030 pyconcept-0.1.1/ccl/core/include/ccl/
+-rw-rw-rw-   0        0        0     2124 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/Operation.hpp
+-rw-rw-rw-   0        0        0     5309 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/Source.hpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.223034 pyconcept-0.1.1/ccl/core/include/ccl/api/
+-rw-rw-rw-   0        0        0      915 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/api/RSFormJA.h
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.226032 pyconcept-0.1.1/ccl/core/include/ccl/env/
+-rw-rw-rw-   0        0        0     2904 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/env/SourceManager.hpp
+-rw-rw-rw-   0        0        0      624 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/env/cclEnvironment.h
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.231028 pyconcept-0.1.1/ccl/core/include/ccl/ops/
+-rw-rw-rw-   0        0        0     1998 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/ops/EquationOptions.h
+-rw-rw-rw-   0        0        0      850 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/ops/RSAggregator.h
+-rw-rw-rw-   0        0        0     1187 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/ops/RSEquationProcessor.h
+-rw-rw-rw-   0        0        0     3525 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/ops/RSOperations.h
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.242030 pyconcept-0.1.1/ccl/core/include/ccl/oss/
+-rw-rw-rw-   0        0        0     4161 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/oss/OSSchema.h
+-rw-rw-rw-   0        0        0     1658 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/oss/OperationProcessor.hpp
+-rw-rw-rw-   0        0        0      903 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/oss/Pict.hpp
+-rw-rw-rw-   0        0        0      934 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/oss/RSSynthesProcessor.h
+-rw-rw-rw-   0        0        0     1363 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/oss/ossGraphFacet.h
+-rw-rw-rw-   0        0        0     2334 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/oss/ossGridFacet.h
+-rw-rw-rw-   0        0        0     2979 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/oss/ossOperationsFacet.h
+-rw-rw-rw-   0        0        0     2469 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/oss/ossSourceFacet.h
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.257030 pyconcept-0.1.1/ccl/core/include/ccl/semantic/
+-rw-rw-rw-   0        0        0      622 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/ConceptRecord.h
+-rw-rw-rw-   0        0        0     1473 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/CstFilters.hpp
+-rw-rw-rw-   0        0        0     2367 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/CstList.h
+-rw-rw-rw-   0        0        0     2523 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/CstType.hpp
+-rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/IdentityManager.h
+-rw-rw-rw-   0        0        0      962 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/InterpretationStorage.h
+-rw-rw-rw-   0        0        0     1069 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/RSConcept.h
+-rw-rw-rw-   0        0        0     3584 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/RSCore.h
+-rw-rw-rw-   0        0        0     3437 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/RSForm.h
+-rw-rw-rw-   0        0        0     3019 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/RSModel.h
+-rw-rw-rw-   0        0        0     5074 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/Schema.h
+-rw-rw-rw-   0        0        0     1122 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/TextConcept.h
+-rw-rw-rw-   0        0        0     2603 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/TextData.hpp
+-rw-rw-rw-   0        0        0     3988 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/Thesaurus.h
+-rw-rw-rw-   0        0        0     1577 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/rsCalculationFacet.h
+-rw-rw-rw-   0        0        0     1648 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/rsModificationFacet.h
+-rw-rw-rw-   0        0        0     1099 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/rsOperationFacet.h
+-rw-rw-rw-   0        0        0     1867 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/semantic/rsValuesFacet.h
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.260030 pyconcept-0.1.1/ccl/core/include/ccl/tools/
+-rw-rw-rw-   0        0        0      894 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/tools/CstNameGenerator.h
+-rw-rw-rw-   0        0        0      523 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/tools/EntityGenerator.h
+-rw-rw-rw-   0        0        0     2935 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/tools/EnumJSON.hpp
+-rw-rw-rw-   0        0        0     3871 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/ccl/tools/JSON.h
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.261029 pyconcept-0.1.1/ccl/core/include/nlohmann/
+-rw-rw-rw-   0        0        0   945021 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/include/nlohmann/json.hpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.263030 pyconcept-0.1.1/ccl/core/src/
+-rw-rw-rw-   0        0        0    18448 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/JSON.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.264030 pyconcept-0.1.1/ccl/core/src/api/
+-rw-rw-rw-   0        0        0     3026 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/api/RSFormJA.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.264030 pyconcept-0.1.1/ccl/core/src/env/
+-rw-rw-rw-   0        0        0      636 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/env/cclEnvironment.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.267032 pyconcept-0.1.1/ccl/core/src/ops/
+-rw-rw-rw-   0        0        0     1764 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/ops/EquationOptions.cpp
+-rw-rw-rw-   0        0        0     4124 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/ops/RSAggregator.cpp
+-rw-rw-rw-   0        0        0     4290 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/ops/RSEquationProcessor.cpp
+-rw-rw-rw-   0        0        0    16240 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/ops/RSOperations.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.272033 pyconcept-0.1.1/ccl/core/src/oss/
+-rw-rw-rw-   0        0        0     7275 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/oss/OSSchema.cpp
+-rw-rw-rw-   0        0        0     2812 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/oss/RSSynthesProcessor.cpp
+-rw-rw-rw-   0        0        0     4326 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/oss/ossGraphFacet.cpp
+-rw-rw-rw-   0        0        0     3023 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/oss/ossGridFacet.cpp
+-rw-rw-rw-   0        0        0    11663 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/oss/ossOperationsFacet.cpp
+-rw-rw-rw-   0        0        0    10397 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/oss/ossSourceFacet.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.179030 pyconcept-0.1.1/ccl/core/src/semantic/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.275030 pyconcept-0.1.1/ccl/core/src/semantic/rscore/
+-rw-rw-rw-   0        0        0      588 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/rscore/ConceptRecord.cpp
+-rw-rw-rw-   0        0        0     3957 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/rscore/CstList.cpp
+-rw-rw-rw-   0        0        0     1950 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/rscore/IdentityManager.cpp
+-rw-rw-rw-   0        0        0    10261 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/rscore/RSCore.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.277029 pyconcept-0.1.1/ccl/core/src/semantic/rsform/
+-rw-rw-rw-   0        0        0     8112 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/rsform/RSForm.cpp
+-rw-rw-rw-   0        0        0     1573 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/rsform/rsModificationFacet.cpp
+-rw-rw-rw-   0        0        0     2431 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/rsform/rsOperationFacet.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.280027 pyconcept-0.1.1/ccl/core/src/semantic/rsmodel/
+-rw-rw-rw-   0        0        0     1591 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp
+-rw-rw-rw-   0        0        0     4755 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/rsmodel/RSModel.cpp
+-rw-rw-rw-   0        0        0     3954 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp
+-rw-rw-rw-   0        0        0     6819 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.281028 pyconcept-0.1.1/ccl/core/src/semantic/schema/
+-rw-rw-rw-   0        0        0      830 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/schema/RSConcept.cpp
+-rw-rw-rw-   0        0        0    13468 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/schema/Schema.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.283026 pyconcept-0.1.1/ccl/core/src/semantic/thesaurus/
+-rw-rw-rw-   0        0        0      919 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/thesaurus/TextConcept.cpp
+-rw-rw-rw-   0        0        0    10089 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/semantic/thesaurus/Thesaurus.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.285031 pyconcept-0.1.1/ccl/core/src/tools/
+-rw-rw-rw-   0        0        0     2682 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/tools/CstNameGenerator.cpp
+-rw-rw-rw-   0        0        0      773 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/src/tools/EntityGenerator.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.285031 pyconcept-0.1.1/ccl/core/unity/
+-rw-rw-rw-   0        0        0     1448 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/core/unity/CCL.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.182026 pyconcept-0.1.1/ccl/rslang/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.291027 pyconcept-0.1.1/ccl/rslang/header/
+-rw-rw-rw-   0        0        0     1362 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/header/ASTNormalizer.h
+-rw-rw-rw-   0        0        0    34735 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/header/AsciiLexerImpl.hpp
+-rw-rw-rw-   0        0        0     2359 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/header/GeneratorImplAST.h
+-rw-rw-rw-   0        0        0    35507 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/header/MathLexerImpl.hpp
+-rw-rw-rw-   0        0        0      958 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/header/NameCollector.h
+-rw-rw-rw-   0        0        0    22132 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/header/RSParserImpl.h
+-rw-rw-rw-   0        0        0     5452 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/header/SDImplementation.h
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.180028 pyconcept-0.1.1/ccl/rslang/import/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.181027 pyconcept-0.1.1/ccl/rslang/import/reflex/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.180028 pyconcept-0.1.1/ccl/rslang/import/reflex/include/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.322030 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/
+-rw-rw-rw-   0        0        0    16072 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/abslexer.h
+-rw-rw-rw-   0        0        0    69252 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/absmatcher.h
+-rw-rw-rw-   0        0        0    18001 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/bits.h
+-rw-rw-rw-   0        0        0    19348 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/boostmatcher.h
+-rw-rw-rw-   0        0        0    11147 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/convert.h
+-rw-rw-rw-   0        0        0     6862 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/debug.h
+-rw-rw-rw-   0        0        0     6978 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/error.h
+-rw-rw-rw-   0        0        0    24462 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/flexlexer.h
+-rw-rw-rw-   0        0        0    38598 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/input.h
+-rw-rw-rw-   0        0        0     6354 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/linematcher.h
+-rw-rw-rw-   0        0        0    15401 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/matcher.h
+-rw-rw-rw-   0        0        0    45834 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/pattern.h
+-rw-rw-rw-   0        0        0    20060 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h
+-rw-rw-rw-   0        0        0     2948 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/posix.h
+-rw-rw-rw-   0        0        0    37159 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/ranges.h
+-rw-rw-rw-   0        0        0    12093 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/setop.h
+-rw-rw-rw-   0        0        0     4594 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/simd.h
+-rw-rw-rw-   0        0        0    22985 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/stdmatcher.h
+-rw-rw-rw-   0        0        0     4244 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/timer.h
+-rw-rw-rw-   0        0        0     3159 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/traits.h
+-rw-rw-rw-   0        0        0     2997 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/unicode.h
+-rw-rw-rw-   0        0        0     9522 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/utf8.h
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.342033 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/
+-rw-rw-rw-   0        0        0    78708 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/convert.cpp
+-rw-rw-rw-   0        0        0     3792 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/debug.cpp
+-rw-rw-rw-   0        0        0     5896 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/error.cpp
+-rw-rw-rw-   0        0        0    84320 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/input.cpp
+-rw-rw-rw-   0        0        0   116725 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/matcher.cpp
+-rw-rw-rw-   0        0        0     2693 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/matcher_avx2.cpp
+-rw-rw-rw-   0        0        0     2715 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp
+-rw-rw-rw-   0        0        0   155001 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/pattern.cpp
+-rw-rw-rw-   0        0        0     4261 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/posix.cpp
+-rw-rw-rw-   0        0        0     5046 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/simd_avx2.cpp
+-rw-rw-rw-   0        0        0     3478 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp
+-rw-rw-rw-   0        0        0     5118 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/unicode.cpp
+-rw-rw-rw-   0        0        0     8872 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/lib/utf8.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.346034 pyconcept-0.1.1/ccl/rslang/import/reflex/unicode/
+-rw-rw-rw-   0        0        0    38187 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/unicode/block_scripts.cpp
+-rw-rw-rw-   0        0        0    30273 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/unicode/composer.cpp
+-rw-rw-rw-   0        0        0   223308 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/unicode/language_scripts.cpp
+-rw-rw-rw-   0        0        0    23072 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/import/reflex/unicode/letter_scripts.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.181027 pyconcept-0.1.1/ccl/rslang/include/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.182026 pyconcept-0.1.1/ccl/rslang/include/ccl/
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.369032 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/
+-rw-rw-rw-   0        0        0     3600 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/ASTInterpreter.h
+-rw-rw-rw-   0        0        0     1048 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/AsciiLexer.h
+-rw-rw-rw-   0        0        0      963 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/Auditor.h
+-rw-rw-rw-   0        0        0      317 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/DataContext.hpp
+-rw-rw-rw-   0        0        0     1120 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/Error.hpp
+-rw-rw-rw-   0        0        0      555 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/ErrorLogger.h
+-rw-rw-rw-   0        0        0      848 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/Interpreter.h
+-rw-rw-rw-   0        0        0     2192 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/LexerBase.hpp
+-rw-rw-rw-   0        0        0      254 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/Literals.h
+-rw-rw-rw-   0        0        0      998 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/MathLexer.h
+-rw-rw-rw-   0        0        0      927 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/Parser.h
+-rw-rw-rw-   0        0        0     1526 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/ParserState.hpp
+-rw-rw-rw-   0        0        0     6805 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp
+-rw-rw-rw-   0        0        0     1102 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/RSExpr.h
+-rw-rw-rw-   0        0        0     1651 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/RSGenerator.h
+-rw-rw-rw-   0        0        0      869 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/RSParser.h
+-rw-rw-rw-   0        0        0     4689 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/RSToken.h
+-rw-rw-rw-   0        0        0     1117 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/SDataCompact.h
+-rw-rw-rw-   0        0        0     1953 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/Structure.hpp
+-rw-rw-rw-   0        0        0     4776 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/StructuredData.h
+-rw-rw-rw-   0        0        0    12948 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/SyntaxTree.h
+-rw-rw-rw-   0        0        0     5270 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/TypeAuditor.h
+-rw-rw-rw-   0        0        0     1520 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/TypeContext.hpp
+-rw-rw-rw-   0        0        0     3754 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/Typification.h
+-rw-rw-rw-   0        0        0     4297 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/ValueAuditor.h
+-rw-rw-rw-   0        0        0      314 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/ValueClass.hpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.388039 pyconcept-0.1.1/ccl/rslang/src/
+-rw-rw-rw-   0        0        0    19985 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/ASTInterpreter.cpp
+-rw-rw-rw-   0        0        0     5997 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/ASTNormalizer.cpp
+-rw-rw-rw-   0        0        0     2219 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/AsciiLexer.cpp
+-rw-rw-rw-   0        0        0     1238 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/Auditor.cpp
+-rw-rw-rw-   0        0        0     1413 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/ErrorLogger.cpp
+-rw-rw-rw-   0        0        0     7204 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/GeneratorImplAST.cpp
+-rw-rw-rw-   0        0        0     1115 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/Interpreter.cpp
+-rw-rw-rw-   0        0        0     2046 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/Literals.cpp
+-rw-rw-rw-   0        0        0     2316 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/MathLexer.cpp
+-rw-rw-rw-   0        0        0     3273 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/NameCollector.cpp
+-rw-rw-rw-   0        0        0     3907 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/Parser.cpp
+-rw-rw-rw-   0        0        0     3409 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/RSExpr.cpp
+-rw-rw-rw-   0        0        0     8152 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/RSGenerator.cpp
+-rw-rw-rw-   0        0        0     8280 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/RSParser.cpp
+-rw-rw-rw-   0        0        0    60161 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/RSParserImpl.cpp
+-rw-rw-rw-   0        0        0    11051 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/RSToken.cpp
+-rw-rw-rw-   0        0        0     6882 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/SDImplementation.cpp
+-rw-rw-rw-   0        0        0     7535 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/SDataCompact.cpp
+-rw-rw-rw-   0        0        0    10421 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/StructuredData.cpp
+-rw-rw-rw-   0        0        0     6353 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/SyntaxTree.cpp
+-rw-rw-rw-   0        0        0    29818 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/TypeAuditor.cpp
+-rw-rw-rw-   0        0        0     3844 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/Typification.cpp
+-rw-rw-rw-   0        0        0     6264 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/src/ValueAuditor.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.391031 pyconcept-0.1.1/ccl/rslang/unity/
+-rw-rw-rw-   0        0        0      399 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/unity/RSlang.cpp
+-rw-rw-rw-   0        0        0      458 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/unity/RSlang2.cpp
+-rw-rw-rw-   0        0        0     1195 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/unity/reflex_unity1.cpp
+-rw-rw-rw-   0        0        0     1776 2024-04-15 19:05:00.000000 pyconcept-0.1.1/ccl/rslang/unity/reflex_unity2.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.392029 pyconcept-0.1.1/cmake/
+-rw-rw-rw-   0        0        0     1490 2024-04-15 19:05:00.000000 pyconcept-0.1.1/cmake/CXXTargets.cmake
+-rw-rw-rw-   0        0        0       96 2024-04-16 20:20:08.000000 pyconcept-0.1.1/conanfile.txt
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.392029 pyconcept-0.1.1/include/
+-rw-rw-rw-   0        0        0     1216 2024-04-15 19:05:00.000000 pyconcept-0.1.1/include/pyconcept.h
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.402054 pyconcept-0.1.1/pyconcept.egg-info/
+-rw-rw-rw-   0        0        0      844 2024-04-17 18:56:45.000000 pyconcept-0.1.1/pyconcept.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8496 2024-04-17 18:56:45.000000 pyconcept-0.1.1/pyconcept.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 18:56:45.000000 pyconcept-0.1.1/pyconcept.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-17 18:56:45.000000 pyconcept-0.1.1/pyconcept.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      146 2024-04-17 11:29:28.000000 pyconcept-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      751 2024-04-17 18:56:45.404050 pyconcept-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     3916 2024-04-17 17:59:03.000000 pyconcept-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.396067 pyconcept-0.1.1/src/
+-rw-rw-rw-   0        0        0     1231 2024-04-15 19:05:00.000000 pyconcept-0.1.1/src/pyconcept.cpp
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.397058 pyconcept-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-15 19:05:00.000000 pyconcept-0.1.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.399057 pyconcept-0.1.1/tests/__pycache__/
+-rw-rw-rw-   0        0        0      148 2024-04-16 20:55:54.000000 pyconcept-0.1.1/tests/__pycache__/__init__.cpython-312.pyc
+-rw-rw-rw-   0        0        0     5032 2024-04-17 18:55:51.000000 pyconcept-0.1.1/tests/__pycache__/testBinding.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-04-17 18:56:45.400055 pyconcept-0.1.1/tests/data/
+-rw-rw-rw-   0        0        0     2486 2024-04-15 19:05:00.000000 pyconcept-0.1.1/tests/data/Schema1.trs
+-rw-rw-rw-   0        0        0     2606 2024-04-17 16:14:46.000000 pyconcept-0.1.1/tests/testBinding.py
```

### Comparing `pyconcept-0.1.0/CMakeLists.txt` & `pyconcept-0.1.1/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,26 +22,14 @@
 set(PYBIND11_FINDPYTHON ON)
 find_package(pybind11 REQUIRED)
 
 ##
 ## Project Setup
 ##
 pybind11_add_module(pyconcept MODULE src/pyconcept.cpp)
-# add_library(pyconcept)
-
-# set_target_properties(pyconcept PROPERTIES 
-#   OUTPUT_NAME pyconcept
-#   DEBUG_POSTFIX d
-#   POSITION_INDEPENDENT_CODE ON
-# )
-
-# target_sources(pyconcept
-#   PRIVATE
-#     src/pyconcept.cpp
-# )
 
 target_include_directories(pyconcept
   PUBLIC
     include
   PRIVATE
     header
     import/include
```

### Comparing `pyconcept-0.1.0/LICENSE` & `pyconcept-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/PKG-INFO` & `pyconcept-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconcept
-Version: 0.1.0
+Version: 0.1.1
 Summary: Concept core Python wrapper
 Home-page: https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept
 Author: CIHT CONCEPT, IRBorisov
 Author-email: iborisov@acconcept.ru
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyconcept-0.1.0/ccl/CMakeLists.txt` & `pyconcept-0.1.1/ccl/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclCommons/include/ccl/Strings.hpp` & `pyconcept-0.1.1/ccl/cclCommons/include/ccl/Strings.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclCommons/include/ccl/Substitutes.hpp` & `pyconcept-0.1.1/ccl/cclCommons/include/ccl/Substitutes.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclCommons/include/ccl/cclChange.hpp` & `pyconcept-0.1.1/ccl/cclCommons/include/ccl/cclChange.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclCommons/include/ccl/cclMeta.hpp` & `pyconcept-0.1.1/ccl/cclCommons/include/ccl/cclMeta.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclCommons/include/ccl/cclTypes.hpp` & `pyconcept-0.1.1/ccl/cclCommons/include/ccl/cclTypes.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclGraph/include/ccl/Entity.hpp` & `pyconcept-0.1.1/ccl/cclGraph/include/ccl/Entity.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclGraph/include/ccl/graph/CGraph.h` & `pyconcept-0.1.1/ccl/cclGraph/include/ccl/graph/CGraph.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclGraph/src/CGraph.cpp` & `pyconcept-0.1.1/ccl/cclGraph/src/CGraph.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp` & `pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/EntityTermContext.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/LexicalTerm.h` & `pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/LexicalTerm.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/ManagedText.h` & `pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/ManagedText.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/Morphology.h` & `pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/Morphology.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/Reference.h` & `pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/Reference.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/RefsManager.h` & `pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/RefsManager.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/TextEnvironment.h` & `pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/TextEnvironment.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/include/ccl/lang/TextProcessor.h` & `pyconcept-0.1.1/ccl/cclLang/include/ccl/lang/TextProcessor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/src/LexicalTerm.cpp` & `pyconcept-0.1.1/ccl/cclLang/src/LexicalTerm.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/src/ManagedText.cpp` & `pyconcept-0.1.1/ccl/cclLang/src/ManagedText.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/src/Morphology.cpp` & `pyconcept-0.1.1/ccl/cclLang/src/Morphology.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/src/Reference.cpp` & `pyconcept-0.1.1/ccl/cclLang/src/Reference.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/src/RefsManager.cpp` & `pyconcept-0.1.1/ccl/cclLang/src/RefsManager.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cclLang/src/TextProcessor.cpp` & `pyconcept-0.1.1/ccl/cclLang/src/TextProcessor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/cmake/CXXTargets.cmake` & `pyconcept-0.1.1/ccl/cmake/CXXTargets.cmake`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/Operation.hpp` & `pyconcept-0.1.1/ccl/core/include/ccl/Operation.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/Source.hpp` & `pyconcept-0.1.1/ccl/core/include/ccl/Source.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/api/RSFormJA.h` & `pyconcept-0.1.1/ccl/core/include/ccl/api/RSFormJA.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/env/SourceManager.hpp` & `pyconcept-0.1.1/ccl/core/include/ccl/env/SourceManager.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/env/cclEnvironment.h` & `pyconcept-0.1.1/ccl/core/include/ccl/env/cclEnvironment.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/ops/EquationOptions.h` & `pyconcept-0.1.1/ccl/core/include/ccl/ops/EquationOptions.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/ops/RSAggregator.h` & `pyconcept-0.1.1/ccl/core/include/ccl/ops/RSAggregator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/ops/RSEquationProcessor.h` & `pyconcept-0.1.1/ccl/core/include/ccl/ops/RSEquationProcessor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/ops/RSOperations.h` & `pyconcept-0.1.1/ccl/core/include/ccl/ops/RSOperations.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/oss/OSSchema.h` & `pyconcept-0.1.1/ccl/core/include/ccl/oss/OSSchema.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/oss/OperationProcessor.hpp` & `pyconcept-0.1.1/ccl/core/include/ccl/oss/OperationProcessor.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/oss/Pict.hpp` & `pyconcept-0.1.1/ccl/core/include/ccl/oss/Pict.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/oss/RSSynthesProcessor.h` & `pyconcept-0.1.1/ccl/core/include/ccl/oss/RSSynthesProcessor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/oss/ossGraphFacet.h` & `pyconcept-0.1.1/ccl/core/include/ccl/oss/ossGraphFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/oss/ossGridFacet.h` & `pyconcept-0.1.1/ccl/core/include/ccl/oss/ossGridFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/oss/ossOperationsFacet.h` & `pyconcept-0.1.1/ccl/core/include/ccl/oss/ossOperationsFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/oss/ossSourceFacet.h` & `pyconcept-0.1.1/ccl/core/include/ccl/oss/ossSourceFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/ConceptRecord.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/ConceptRecord.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/CstFilters.hpp` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/CstFilters.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/CstList.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/CstList.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/CstType.hpp` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/CstType.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/IdentityManager.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/IdentityManager.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/InterpretationStorage.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/InterpretationStorage.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/RSConcept.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/RSConcept.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/RSCore.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/RSCore.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/RSForm.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/RSForm.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/RSModel.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/RSModel.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/Schema.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/Schema.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/TextConcept.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/TextConcept.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/TextData.hpp` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/TextData.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/Thesaurus.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/Thesaurus.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/rsCalculationFacet.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/rsCalculationFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/rsModificationFacet.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/rsModificationFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/rsOperationFacet.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/rsOperationFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/semantic/rsValuesFacet.h` & `pyconcept-0.1.1/ccl/core/include/ccl/semantic/rsValuesFacet.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/tools/CstNameGenerator.h` & `pyconcept-0.1.1/ccl/core/include/ccl/tools/CstNameGenerator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/tools/EntityGenerator.h` & `pyconcept-0.1.1/ccl/core/include/ccl/tools/EntityGenerator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/tools/EnumJSON.hpp` & `pyconcept-0.1.1/ccl/core/include/ccl/tools/EnumJSON.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/ccl/tools/JSON.h` & `pyconcept-0.1.1/ccl/core/include/ccl/tools/JSON.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/include/nlohmann/json.hpp` & `pyconcept-0.1.1/ccl/core/include/nlohmann/json.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/JSON.cpp` & `pyconcept-0.1.1/ccl/core/src/JSON.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/api/RSFormJA.cpp` & `pyconcept-0.1.1/ccl/core/src/api/RSFormJA.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/env/cclEnvironment.cpp` & `pyconcept-0.1.1/ccl/core/src/env/cclEnvironment.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/ops/EquationOptions.cpp` & `pyconcept-0.1.1/ccl/core/src/ops/EquationOptions.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/ops/RSAggregator.cpp` & `pyconcept-0.1.1/ccl/core/src/ops/RSAggregator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/ops/RSEquationProcessor.cpp` & `pyconcept-0.1.1/ccl/core/src/ops/RSEquationProcessor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/ops/RSOperations.cpp` & `pyconcept-0.1.1/ccl/core/src/ops/RSOperations.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/oss/OSSchema.cpp` & `pyconcept-0.1.1/ccl/core/src/oss/OSSchema.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/oss/RSSynthesProcessor.cpp` & `pyconcept-0.1.1/ccl/core/src/oss/RSSynthesProcessor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/oss/ossGraphFacet.cpp` & `pyconcept-0.1.1/ccl/core/src/oss/ossGraphFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/oss/ossGridFacet.cpp` & `pyconcept-0.1.1/ccl/core/src/oss/ossGridFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/oss/ossOperationsFacet.cpp` & `pyconcept-0.1.1/ccl/core/src/oss/ossOperationsFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/oss/ossSourceFacet.cpp` & `pyconcept-0.1.1/ccl/core/src/oss/ossSourceFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/rscore/ConceptRecord.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/rscore/ConceptRecord.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/rscore/CstList.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/rscore/CstList.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/rscore/IdentityManager.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/rscore/IdentityManager.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/rscore/RSCore.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/rscore/RSCore.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/rsform/RSForm.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/rsform/RSForm.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/rsform/rsModificationFacet.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/rsform/rsModificationFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/rsform/rsOperationFacet.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/rsform/rsOperationFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/rsmodel/InterpretationStorage.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/rsmodel/RSModel.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/rsmodel/RSModel.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/rsmodel/rsCalculationFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/rsmodel/rsValuesFacet.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/schema/RSConcept.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/schema/RSConcept.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/schema/Schema.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/schema/Schema.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/thesaurus/TextConcept.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/thesaurus/TextConcept.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/semantic/thesaurus/Thesaurus.cpp` & `pyconcept-0.1.1/ccl/core/src/semantic/thesaurus/Thesaurus.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/tools/CstNameGenerator.cpp` & `pyconcept-0.1.1/ccl/core/src/tools/CstNameGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/src/tools/EntityGenerator.cpp` & `pyconcept-0.1.1/ccl/core/src/tools/EntityGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/core/unity/CCL.cpp` & `pyconcept-0.1.1/ccl/core/unity/CCL.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/header/ASTNormalizer.h` & `pyconcept-0.1.1/ccl/rslang/header/ASTNormalizer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/header/AsciiLexerImpl.hpp` & `pyconcept-0.1.1/ccl/rslang/header/AsciiLexerImpl.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/header/GeneratorImplAST.h` & `pyconcept-0.1.1/ccl/rslang/header/GeneratorImplAST.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/header/MathLexerImpl.hpp` & `pyconcept-0.1.1/ccl/rslang/header/MathLexerImpl.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/header/NameCollector.h` & `pyconcept-0.1.1/ccl/rslang/header/NameCollector.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/header/RSParserImpl.h` & `pyconcept-0.1.1/ccl/rslang/header/RSParserImpl.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/header/SDImplementation.h` & `pyconcept-0.1.1/ccl/rslang/header/SDImplementation.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/abslexer.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/abslexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/absmatcher.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/absmatcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/bits.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/bits.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/boostmatcher.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/boostmatcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/convert.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/convert.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/debug.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/debug.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/error.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/error.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/flexlexer.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/flexlexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/input.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/input.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/linematcher.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/linematcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/matcher.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/matcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/pattern.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/pattern.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/pcre2matcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/posix.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/posix.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/ranges.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/ranges.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/setop.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/setop.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/simd.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/simd.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/stdmatcher.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/stdmatcher.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/timer.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/timer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/traits.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/traits.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/unicode.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/unicode.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/include/reflex/utf8.h` & `pyconcept-0.1.1/ccl/rslang/import/reflex/include/reflex/utf8.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/lib/convert.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/lib/convert.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/lib/debug.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/lib/debug.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/lib/error.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/lib/error.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/lib/input.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/lib/input.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/lib/matcher.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/lib/matcher.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/lib/matcher_avx2.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/lib/matcher_avx2.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/lib/matcher_avx512bw.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/lib/pattern.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/lib/pattern.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/lib/posix.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/lib/posix.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/lib/simd_avx2.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/lib/simd_avx2.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/lib/simd_avx512bw.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/lib/unicode.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/lib/unicode.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/lib/utf8.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/lib/utf8.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/unicode/block_scripts.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/unicode/block_scripts.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/unicode/composer.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/unicode/composer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/unicode/language_scripts.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/unicode/language_scripts.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/import/reflex/unicode/letter_scripts.cpp` & `pyconcept-0.1.1/ccl/rslang/import/reflex/unicode/letter_scripts.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/ASTInterpreter.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/ASTInterpreter.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/AsciiLexer.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/AsciiLexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/Auditor.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/Auditor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/Error.hpp` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/Error.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/ErrorLogger.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/ErrorLogger.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/Interpreter.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/Interpreter.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/LexerBase.hpp` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/LexerBase.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/MathLexer.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/MathLexer.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/Parser.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/Parser.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/ParserState.hpp` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/ParserState.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/RSErrorCodes.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/RSExpr.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/RSExpr.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/RSGenerator.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/RSGenerator.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/RSParser.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/RSParser.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/RSToken.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/RSToken.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/SDataCompact.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/SDataCompact.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/Structure.hpp` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/Structure.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/StructuredData.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/StructuredData.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/SyntaxTree.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/SyntaxTree.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/TypeAuditor.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/TypeAuditor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/TypeContext.hpp` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/TypeContext.hpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/Typification.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/Typification.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/include/ccl/rslang/ValueAuditor.h` & `pyconcept-0.1.1/ccl/rslang/include/ccl/rslang/ValueAuditor.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/ASTInterpreter.cpp` & `pyconcept-0.1.1/ccl/rslang/src/ASTInterpreter.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/ASTNormalizer.cpp` & `pyconcept-0.1.1/ccl/rslang/src/ASTNormalizer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/AsciiLexer.cpp` & `pyconcept-0.1.1/ccl/rslang/src/AsciiLexer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/Auditor.cpp` & `pyconcept-0.1.1/ccl/rslang/src/Auditor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/ErrorLogger.cpp` & `pyconcept-0.1.1/ccl/rslang/src/ErrorLogger.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/GeneratorImplAST.cpp` & `pyconcept-0.1.1/ccl/rslang/src/GeneratorImplAST.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/Interpreter.cpp` & `pyconcept-0.1.1/ccl/rslang/src/Interpreter.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/Literals.cpp` & `pyconcept-0.1.1/ccl/rslang/src/Literals.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/MathLexer.cpp` & `pyconcept-0.1.1/ccl/rslang/src/MathLexer.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/NameCollector.cpp` & `pyconcept-0.1.1/ccl/rslang/src/NameCollector.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/Parser.cpp` & `pyconcept-0.1.1/ccl/rslang/src/Parser.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/RSExpr.cpp` & `pyconcept-0.1.1/ccl/rslang/src/RSExpr.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/RSGenerator.cpp` & `pyconcept-0.1.1/ccl/rslang/src/RSGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/RSParser.cpp` & `pyconcept-0.1.1/ccl/rslang/src/RSParser.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/RSParserImpl.cpp` & `pyconcept-0.1.1/ccl/rslang/src/RSParserImpl.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/RSToken.cpp` & `pyconcept-0.1.1/ccl/rslang/src/RSToken.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/SDImplementation.cpp` & `pyconcept-0.1.1/ccl/rslang/src/SDImplementation.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/SDataCompact.cpp` & `pyconcept-0.1.1/ccl/rslang/src/SDataCompact.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/StructuredData.cpp` & `pyconcept-0.1.1/ccl/rslang/src/StructuredData.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/SyntaxTree.cpp` & `pyconcept-0.1.1/ccl/rslang/src/SyntaxTree.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/TypeAuditor.cpp` & `pyconcept-0.1.1/ccl/rslang/src/TypeAuditor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/Typification.cpp` & `pyconcept-0.1.1/ccl/rslang/src/Typification.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/src/ValueAuditor.cpp` & `pyconcept-0.1.1/ccl/rslang/src/ValueAuditor.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/unity/reflex_unity1.cpp` & `pyconcept-0.1.1/ccl/rslang/unity/reflex_unity1.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/ccl/rslang/unity/reflex_unity2.cpp` & `pyconcept-0.1.1/ccl/rslang/unity/reflex_unity2.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/cmake/CXXTargets.cmake` & `pyconcept-0.1.1/cmake/CXXTargets.cmake`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/include/pyconcept.h` & `pyconcept-0.1.1/include/pyconcept.h`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/pyconcept.egg-info/PKG-INFO` & `pyconcept-0.1.1/pyconcept.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyconcept
-Version: 0.1.0
+Version: 0.1.1
 Summary: Concept core Python wrapper
 Home-page: https://github.com/IRBorisov/ConceptCore/tree/main/pyconcept
 Author: CIHT CONCEPT, IRBorisov
 Author-email: iborisov@acconcept.ru
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `pyconcept-0.1.0/pyconcept.egg-info/SOURCES.txt` & `pyconcept-0.1.1/pyconcept.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -213,8 +213,8 @@
 pyconcept.egg-info/dependency_links.txt
 pyconcept.egg-info/top_level.txt
 src/pyconcept.cpp
 tests/__init__.py
 tests/testBinding.py
 tests/__pycache__/__init__.cpython-312.pyc
 tests/__pycache__/testBinding.cpython-312.pyc
-tests/data/КС начальник-подчиненный.trs
+tests/data/Schema1.trs
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyconcept-0.1.0/setup.cfg` & `pyconcept-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/setup.py` & `pyconcept-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         target_fullpath = Path.cwd() / self.get_ext_fullpath(target.name)
         output_folder = target_fullpath.parent.resolve()
 
         debug_flag = int(os.environ.get('DEBUG', 0)) if self.debug is None else self.debug
         build_type = 'Debug' if debug_flag else 'Release'
         cmake_generator = os.environ.get('CMAKE_GENERATOR', '')
         cmake_args = [
-            '--preset conan-default',
+            '--preset conan-release' if self.compiler.compiler_type != 'msvc' else '--preset conan-default',
             f"-DCMAKE_LIBRARY_OUTPUT_DIRECTORY={output_folder}{os.sep}",
             f"-DCMAKE_BUILD_TYPE={build_type}"
         ]
 
         if 'CMAKE_ARGS' in os.environ:
             cmake_args += [item for item in os.environ['CMAKE_ARGS'].split(' ') if item]
 
@@ -77,15 +77,15 @@
 
         # Set CMAKE_BUILD_PARALLEL_LEVEL to control the parallel build level across all generators.
         if 'CMAKE_BUILD_PARALLEL_LEVEL' not in os.environ:
             if hasattr(self, 'parallel') and self.parallel:
                 build_args += [f"-j{self.parallel}"]
 
         subprocess.run(['conan', 'profile', 'detect', '--force'], check=True)
-        subprocess.run(['conan', 'install', '.'], check=True)
+        subprocess.run(['conan', 'install', '.', '--build=missing'], check=True)
         subprocess.run(['cmake', target.source_dir, *cmake_args], check=True)
         subprocess.run(['cmake', '--build', '.', *build_args], check=True)
 
 
 setup(
     ext_modules=[CMakeExtension('pyconcept')],
     cmdclass={'build_ext': CMakeBuild}
```

### Comparing `pyconcept-0.1.0/src/pyconcept.cpp` & `pyconcept-0.1.1/src/pyconcept.cpp`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/tests/__pycache__/testBinding.cpython-312.pyc` & `pyconcept-0.1.1/tests/__pycache__/testBinding.cpython-312.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.12 or newer, timestamp-based, .py timestamp: Mon Apr 15 19:05:00 2024 UTC, .py size: 2645 bytes*

 * *Could not decompile bytecode: tuple index out of range*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: cb0d 0d0a 0000 0000 5c7a 1d66 550a 0000  ........\z.fU...
+00000000: cb0d 0d0a 0000 0000 76f5 1f66 2e0a 0000  ........v..f....
 00000010: e300 0000 0000 0000 0000 0000 0005 0000  ................
 00000020: 0000 0000 00f3 9c00 0000 9700 6400 5a00  ............d.Z.
 00000030: 6401 6402 6c01 5a01 6401 6402 6c02 5a02  d.d.l.Z.d.d.l.Z.
 00000040: 6401 6402 6c03 5a03 6401 6403 6c04 6d05  d.d.l.Z.d.d.l.m.
 00000050: 5a05 0100 6401 6402 6c06 5a07 6404 6508  Z...d.d.l.Z.d.e.
 00000060: 6405 6508 6604 6406 8404 5a09 0200 4700  d.e.f.d...Z...G.
 00000070: 6407 8400 6408 6503 6a14 0000 0000 0000  d...d.e.j.......
@@ -273,46 +273,43 @@
 00001100: d119 39b8 34d5 0840 721b 0000 0072 0500  ..9.4..@r....r..
 00001110: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
 00001120: 0000 0003 0000 00f3 4600 0000 9700 7401  ........F.....t.
 00001130: 0000 0000 0000 0000 6a02 0000 0000 0000  ........j.......
 00001140: 0000 0000 0000 0000 0000 0000 ab00 0000  ................
 00001150: 0000 0000 6401 7a00 0000 7d01 7405 0000  ....d.z...}.t...
 00001160: 0000 0000 0000 7c01 ab01 0000 0000 0000  ......|.........
-00001170: 5300 2902 4e75 3e00 0000 2f74 6573 7473  S.).Nu>.../tests
-00001180: 2f64 6174 612f d09a d0a1 20d0 bdd0 b0d1  /data/.... .....
-00001190: 87d0 b0d0 bbd1 8cd0 bdd0 b8d0 ba2d d0bf  .............-..
-000011a0: d0be d0b4 d187 d0b8 d0bd d0b5 d0bd d0bd  ................
-000011b0: d18b d0b9 2e74 7273 2903 da02 6f73 da06  .....trs)...os..
-000011c0: 6765 7463 7764 720c 0000 0029 0272 1900  getcwdr....).r..
-000011d0: 0000 7204 0000 0073 0200 0000 2020 720b  ..r....s....  r.
-000011e0: 0000 0072 2b00 0000 7a1f 5465 7374 4269  ...r+...z.TestBi
-000011f0: 6e64 696e 672e 5f67 6574 5f64 6566 6175  nding._get_defau
-00001200: 6c74 5f73 6368 656d 6142 0000 0073 1e00  lt_schemaB...s..
-00001210: 0000 8000 dc14 1697 4991 4993 4bd0 2263  ........I.I.K."c
-00001220: d114 6388 09dc 0f18 9819 d30f 23d0 0823  ..c.........#..#
-00001230: 721b 0000 004e 290c da08 5f5f 6e61 6d65  r....N)...__name
-00001240: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
-00001250: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
-00001260: 646f 635f 5f72 1a00 0000 721e 0000 0072  doc__r....r....r
-00001270: 2900 0000 7230 0000 0072 3300 0000 723c  )...r0...r3...r<
-00001280: 0000 00da 0373 7472 722b 0000 00a9 0072  .....strr+.....r
-00001290: 1b00 0000 720b 0000 0072 0e00 0000 720e  ....r....r....r.
-000012a0: 0000 0011 0000 0073 3200 0000 8400 d904  .......s2.......
-000012b0: 25f2 0406 0546 01f2 1005 0545 01f2 0e07  %....F.....E....
-000012c0: 0531 f212 0405 26f2 0c07 0535 f212 0505  .1....&....5....
-000012d0: 4101 f00e 0205 24a0 53f4 0002 0524 721b  A.....$.S....$r.
-000012e0: 0000 0072 0e00 0000 da08 5f5f 6d61 696e  ...r......__main
-000012f0: 5f5f 290e 7243 0000 0072 3e00 0000 7224  __).rC...r>...r$
-00001300: 0000 00da 0875 6e69 7474 6573 74da 077a  .....unittest..z
-00001310: 6970 6669 6c65 7203 0000 00da 0970 7963  ipfiler......pyc
-00001320: 6f6e 6365 7074 7216 0000 0072 4400 0000  onceptr....rD...
-00001330: 720c 0000 00da 0854 6573 7443 6173 6572  r......TestCaser
-00001340: 0e00 0000 7240 0000 00da 046d 6169 6e72  ....r@.....mainr
-00001350: 4500 0000 721b 0000 0072 0b00 0000 fa08  E...r....r......
-00001360: 3c6d 6f64 756c 653e 724c 0000 0001 0000  <module>rL......
-00001370: 0073 5700 0000 f003 0101 01d9 001b db00  .sW.............
-00001380: 09db 000b db00 0fdd 001b e300 16f0 0604  ................
-00001390: 0115 9813 f000 0401 15a0 13f3 0004 0115  ................
-000013a0: f40e 3301 2490 28d7 1223 d112 23f4 0033  ..3.$.(..#..#..3
-000013b0: 0124 f06c 0100 040c 887a d203 19d8 0411  .$.l.....z......
-000013c0: 8048 874d 814d 854f f003 0004 1a72 1b00  .H.M.M.O.....r..
-000013d0: 0000                                     ..
+00001170: 5300 2902 4e7a 172f 7465 7374 732f 6461  S.).Nz./tests/da
+00001180: 7461 2f53 6368 656d 6131 2e74 7273 2903  ta/Schema1.trs).
+00001190: da02 6f73 da06 6765 7463 7764 720c 0000  ..os..getcwdr...
+000011a0: 0029 0272 1900 0000 7204 0000 0073 0200  .).r....r....s..
+000011b0: 0000 2020 720b 0000 0072 2b00 0000 7a1f  ..  r....r+...z.
+000011c0: 5465 7374 4269 6e64 696e 672e 5f67 6574  TestBinding._get
+000011d0: 5f64 6566 6175 6c74 5f73 6368 656d 6142  _default_schemaB
+000011e0: 0000 0073 1e00 0000 8000 dc14 1697 4991  ...s..........I.
+000011f0: 4993 4bd0 223c d114 3c88 09dc 0f18 9819  I.K."<..<.......
+00001200: d30f 23d0 0823 721b 0000 004e 290c da08  ..#..#r....N)...
+00001210: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00001220: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00001230: 5f5f da07 5f5f 646f 635f 5f72 1a00 0000  __..__doc__r....
+00001240: 721e 0000 0072 2900 0000 7230 0000 0072  r....r)...r0...r
+00001250: 3300 0000 723c 0000 00da 0373 7472 722b  3...r<.....strr+
+00001260: 0000 00a9 0072 1b00 0000 720b 0000 0072  .....r....r....r
+00001270: 0e00 0000 720e 0000 0011 0000 0073 3200  ....r........s2.
+00001280: 0000 8400 d904 25f2 0406 0546 01f2 1005  ......%....F....
+00001290: 0545 01f2 0e07 0531 f212 0405 26f2 0c07  .E.....1....&...
+000012a0: 0535 f212 0505 4101 f00e 0205 24a0 53f4  .5....A.....$.S.
+000012b0: 0002 0524 721b 0000 0072 0e00 0000 da08  ...$r....r......
+000012c0: 5f5f 6d61 696e 5f5f 290e 7243 0000 0072  __main__).rC...r
+000012d0: 3e00 0000 7224 0000 00da 0875 6e69 7474  >...r$.....unitt
+000012e0: 6573 74da 077a 6970 6669 6c65 7203 0000  est..zipfiler...
+000012f0: 00da 0970 7963 6f6e 6365 7074 7216 0000  ...pyconceptr...
+00001300: 0072 4400 0000 720c 0000 00da 0854 6573  .rD...r......Tes
+00001310: 7443 6173 6572 0e00 0000 7240 0000 00da  tCaser....r@....
+00001320: 046d 6169 6e72 4500 0000 721b 0000 0072  .mainrE...r....r
+00001330: 0b00 0000 fa08 3c6d 6f64 756c 653e 724c  ......<module>rL
+00001340: 0000 0001 0000 0073 5700 0000 f003 0101  .......sW.......
+00001350: 01d9 001b db00 09db 000b db00 0fdd 001b  ................
+00001360: e300 16f0 0604 0115 9813 f000 0401 15a0  ................
+00001370: 13f3 0004 0115 f40e 3301 2490 28d7 1223  ........3.$.(..#
+00001380: d112 23f4 0033 0124 f06c 0100 040c 887a  ..#..3.$.l.....z
+00001390: d203 19d8 0411 8048 874d 814d 854f f003  .......H.M.M.O..
+000013a0: 0004 1a72 1b00 0000                      ...r....
```

### Comparing `pyconcept-0.1.0/tests/data/КС начальник-подчиненный.trs` & `pyconcept-0.1.1/tests/data/Schema1.trs`

 * *Files identical despite different names*

### Comparing `pyconcept-0.1.0/tests/testBinding.py` & `pyconcept-0.1.1/tests/testBinding.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,13 +60,13 @@
         ''' Test reset aliases in schema '''
         schema = self._get_default_schema()
         fixedSchema = json.loads(pc.reset_aliases(schema))
         self.assertTrue(len(fixedSchema['items']) > 1)
         self.assertEqual(fixedSchema['items'][1]['alias'], 'S1')
 
     def _get_default_schema(self) -> str:
-        file_path = os.getcwd() + r'/tests/data/КС начальник-подчиненный.trs'
+        file_path = os.getcwd() + r'/tests/data/Schema1.trs'
         return _read_trs(file_path)
 
 
 if __name__ == '__main__':
     unittest.main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

