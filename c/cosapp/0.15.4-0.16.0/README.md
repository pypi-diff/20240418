# Comparing `tmp/cosapp-0.15.4.tar.gz` & `tmp/cosapp-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosapp-0.15.4.tar", last modified: Wed Feb 28 13:39:09 2024, max compression
+gzip compressed data, was "cosapp-0.16.0.tar", last modified: Thu Apr 18 14:27:43 2024, max compression
```

## Comparing `cosapp-0.15.4.tar` & `cosapp-0.16.0.tar`

### file list

```diff
@@ -1,497 +1,498 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.219464 cosapp-0.15.4/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2024-02-28 13:38:49.000000 cosapp-0.15.4/AUTHORS.md
--rw-rw-rw-   0 root         (0) root         (0)     3579 2024-02-28 13:38:49.000000 cosapp-0.15.4/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)    45800 2024-02-28 13:38:49.000000 cosapp-0.15.4/HISTORY.md
--rw-rw-rw-   0 root         (0) root         (0)     6572 2024-02-28 13:38:49.000000 cosapp-0.15.4/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      754 2024-02-28 13:38:49.000000 cosapp-0.15.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    49049 2024-02-28 13:39:09.219464 cosapp-0.15.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1480 2024-02-28 13:38:49.000000 cosapp-0.15.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.126465 cosapp-0.15.4/cosapp/
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.127465 cosapp-0.15.4/cosapp/base/
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.129465 cosapp-0.15.4/cosapp/core/
--rw-rw-rw-   0 root         (0) root         (0)      231 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     5176 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/configuration_schema.json
--rw-rw-rw-   0 root         (0) root         (0)    18908 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/eval_str.py
--rw-rw-rw-   0 root         (0) root         (0)    16116 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/module.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.131465 cosapp-0.15.4/cosapp/core/numerics/
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/numerics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    27814 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/numerics/basics.py
--rw-rw-rw-   0 root         (0) root         (0)    28991 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/numerics/boundary.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/numerics/enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2948 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/numerics/mathematicalproblem.schema.json
--rw-rw-rw-   0 root         (0) root         (0)    13455 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/numerics/residues.py
--rw-rw-rw-   0 root         (0) root         (0)    19400 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/numerics/root.py
--rw-rw-rw-   0 root         (0) root         (0)    15550 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/numerics/sobol_seq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.131465 cosapp-0.15.4/cosapp/core/signal/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/signal/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4972 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/signal/signal.py
--rw-rw-rw-   0 root         (0) root         (0)     1812 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/signal/slot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.133465 cosapp-0.15.4/cosapp/core/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8079 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    15027 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/tests/test_AssignString.py
--rw-rw-rw-   0 root         (0) root         (0)    12270 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/tests/test_CoSAppConfiguration.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/tests/test_ContextLocals.py
--rw-rw-rw-   0 root         (0) root         (0)    12783 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/tests/test_EvalString.py
--rw-rw-rw-   0 root         (0) root         (0)    14154 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/tests/test_Module.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/tests/test_time.py
--rw-rw-rw-   0 root         (0) root         (0)     2013 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/core/variableref.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.136465 cosapp-0.15.4/cosapp/drivers/
--rw-rw-rw-   0 root         (0) root         (0)      936 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3030 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/abstractsetofcases.py
--rw-rw-rw-   0 root         (0) root         (0)    11978 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/abstractsolver.py
--rw-rw-rw-   0 root         (0) root         (0)     8692 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/driver.py
--rw-rw-rw-   0 root         (0) root         (0)     9499 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/influence.py
--rw-rw-rw-   0 root         (0) root         (0)     2214 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/iterativecase.py
--rw-rw-rw-   0 root         (0) root         (0)     2867 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/lineardoe.py
--rw-rw-rw-   0 root         (0) root         (0)     3131 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/metasystembuilder.py
--rw-rw-rw-   0 root         (0) root         (0)    10683 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/montecarlo.py
--rw-rw-rw-   0 root         (0) root         (0)    29314 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/nonlinearsolver.py
--rw-rw-rw-   0 root         (0) root         (0)    21794 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/optimizer.py
--rw-rw-rw-   0 root         (0) root         (0)     1589 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/optionaldriver.py
--rw-rw-rw-   0 root         (0) root         (0)     6674 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/runonce.py
--rw-rw-rw-   0 root         (0) root         (0)    12912 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/runsinglecase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.137465 cosapp-0.15.4/cosapp/drivers/time/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1017 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/euler.py
--rw-rw-rw-   0 root         (0) root         (0)    20082 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/interfaces.py
--rw-rw-rw-   0 root         (0) root         (0)     3457 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/runge_kutta.py
--rw-rw-rw-   0 root         (0) root         (0)    14133 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/scenario.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.141465 cosapp-0.15.4/cosapp/drivers/time/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15016 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     6501 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_BouncingBall.py
--rw-rw-rw-   0 root         (0) root         (0)     2599 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_DiscreteStepper.py
--rw-rw-rw-   0 root         (0) root         (0)     4202 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_EulerExplicit.py
--rw-rw-rw-   0 root         (0) root         (0)    21059 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_ExplicitTimeDriver.py
--rw-rw-rw-   0 root         (0) root         (0)     1501 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_InterpolAssignString.py
--rw-rw-rw-   0 root         (0) root         (0)     2419 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_Interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     5336 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_NewtonPendulum.py
--rw-rw-rw-   0 root         (0) root         (0)    25908 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_RungeKutta.py
--rw-rw-rw-   0 root         (0) root         (0)    22357 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_Scenario.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_SystemInterpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     1633 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_TimeAssignString.py
--rw-rw-rw-   0 root         (0) root         (0)     4551 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_TimeStepManager.py
--rw-rw-rw-   0 root         (0) root         (0)     8108 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_TimeUnknownDict.py
--rw-rw-rw-   0 root         (0) root         (0)     4478 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_TimeUnknownStack.py
--rw-rw-rw-   0 root         (0) root         (0)     2914 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_TimeVarManager.py
--rw-rw-rw-   0 root         (0) root         (0)      608 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_TwoPointCubicInterpolator.py
--rw-rw-rw-   0 root         (0) root         (0)      771 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_TwoPointCubicPolynomial.py
--rw-rw-rw-   0 root         (0) root         (0)     9926 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_event_cascades.py
--rw-rw-rw-   0 root         (0) root         (0)     1483 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/tests/test_modevar_init.py
--rw-rw-rw-   0 root         (0) root         (0)    21544 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/time/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    15033 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1657 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/drivers/validitycheck.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.142465 cosapp-0.15.4/cosapp/multimode/
--rw-rw-rw-   0 root         (0) root         (0)      158 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/multimode/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5937 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/multimode/discreteStepper.py
--rw-rw-rw-   0 root         (0) root         (0)    11879 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/multimode/event.py
--rw-rw-rw-   0 root         (0) root         (0)     2503 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/multimode/zeroCrossing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.143465 cosapp-0.15.4/cosapp/patterns/
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/patterns/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3411 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/patterns/observer.py
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/patterns/singleton.py
--rw-rw-rw-   0 root         (0) root         (0)      713 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/patterns/visitor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.145465 cosapp-0.15.4/cosapp/ports/
--rw-rw-rw-   0 root         (0) root         (0)      494 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/ports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16179 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/ports/connectors.py
--rw-rw-rw-   0 root         (0) root         (0)     1040 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/ports/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/ports/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4022 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/ports/mode_variable.py
--rw-rw-rw-   0 root         (0) root         (0)    34280 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/ports/port.py
--rw-rw-rw-   0 root         (0) root         (0)     5865 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/ports/unit_library.ini
--rw-rw-rw-   0 root         (0) root         (0)    33349 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/ports/units.py
--rw-rw-rw-   0 root         (0) root         (0)    31417 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/ports/variable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.146465 cosapp-0.15.4/cosapp/recorders/
--rw-rw-rw-   0 root         (0) root         (0)      169 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/recorders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4628 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/recorders/dataframe_recorder.py
--rw-rw-rw-   0 root         (0) root         (0)     7847 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/recorders/dsv_recorder.py
--rw-rw-rw-   0 root         (0) root         (0)    14620 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/recorders/recorder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.148465 cosapp-0.15.4/cosapp/systems/
--rw-rw-rw-   0 root         (0) root         (0)      741 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/systems/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6451 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/systems/externalsystem.py
--rw-rw-rw-   0 root         (0) root         (0)    13327 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/systems/metamodels.py
--rw-rw-rw-   0 root         (0) root         (0)     1237 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/systems/processsystem.py
--rw-rw-rw-   0 root         (0) root         (0)     5246 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/systems/structure.schema.json
--rw-rw-rw-   0 root         (0) root         (0)   134097 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/systems/system.py
--rw-rw-rw-   0 root         (0) root         (0)     3095 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/systems/system.schema.json
--rw-rw-rw-   0 root         (0) root         (0)     3004 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/systems/systemConnector.py
--rw-rw-rw-   0 root         (0) root         (0)    15658 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/systems/systemSurrogate.py
--rw-rw-rw-   0 root         (0) root         (0)     5515 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/systems/systemfamily.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.150465 cosapp-0.15.4/cosapp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/all_tests.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.154465 cosapp-0.15.4/cosapp/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)      356 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/default_dataframe.json
--rw-rw-rw-   0 root         (0) root         (0)      214 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/export_doe.cs
--rw-rw-rw-   0 root         (0) root         (0)      214 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/export_doe.csv
--rw-rw-rw-   0 root         (0) root         (0)      887 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/export_doe.json
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/export_doe.txt
--rw-rw-rw-   0 root         (0) root         (0)     1701 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/system_config.json
--rw-rw-rw-   0 root         (0) root         (0)      738 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/system_config_ducts.json
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss.json
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss1.json
--rw-rw-rw-   0 root         (0) root         (0)      453 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss11.json
--rw-rw-rw-   0 root         (0) root         (0)      932 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss11bis.json
--rw-rw-rw-   0 root         (0) root         (0)      623 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss12.json
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss121.json
--rw-rw-rw-   0 root         (0) root         (0)      922 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss131.json
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss2.json
--rw-rw-rw-   0 root         (0) root         (0)      809 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss22.json
--rw-rw-rw-   0 root         (0) root         (0)     2537 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss222.json
--rw-rw-rw-   0 root         (0) root         (0)      708 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss2tank.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.154465 cosapp-0.15.4/cosapp/tests/library/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/library/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1790 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/library/ports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.156465 cosapp-0.15.4/cosapp/tests/library/systems/
--rw-rw-rw-   0 root         (0) root         (0)     1150 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/library/systems/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7259 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/library/systems/basicalgebra.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/library/systems/dynamics.py
--rw-rw-rw-   0 root         (0) root         (0)     3257 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/library/systems/elec.py
--rw-rw-rw-   0 root         (0) root         (0)     8536 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/library/systems/multiply.py
--rw-rw-rw-   0 root         (0) root         (0)    11780 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/library/systems/others.py
--rw-rw-rw-   0 root         (0) root         (0)     4826 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/library/systems/pressurelossvarious.py
--rw-rw-rw-   0 root         (0) root         (0)     1986 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/library/systems/vectors.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/test_ComplexDuct.py
--rw-rw-rw-   0 root         (0) root         (0)    10011 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/test_MathematicalProblem_integration.py
--rw-rw-rw-   0 root         (0) root         (0)    10653 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/test_Turbofan.py
--rw-rw-rw-   0 root         (0) root         (0)     3971 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/test_dynamics.py
--rw-rw-rw-   0 root         (0) root         (0)     6650 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/test_electric_circuit.py
--rw-rw-rw-   0 root         (0) root         (0)     9223 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/test_multimode.py
--rw-rw-rw-   0 root         (0) root         (0)     8225 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/test_system_pressureloss.py
--rw-rw-rw-   0 root         (0) root         (0)     1524 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/test_tutorials.py
--rw-rw-rw-   0 root         (0) root         (0)    11905 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/test_unknown_aliasing.py
--rw-rw-rw-   0 root         (0) root         (0)     5540 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tests/test_visitor_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.156465 cosapp-0.15.4/cosapp/tools/
--rw-rw-rw-   0 root         (0) root         (0)      655 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.157465 cosapp-0.15.4/cosapp/tools/fmu/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/fmu/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22336 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/fmu/exporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3204 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/fmu/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.158465 cosapp-0.15.4/cosapp/tools/fmu/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/fmu/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2606 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/fmu/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    13858 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/fmu/tests/test_exporter.py
--rw-rw-rw-   0 root         (0) root         (0)     1686 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/fmu/tests/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     4117 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/help.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.158465 cosapp-0.15.4/cosapp/tools/module_parser/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/module_parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4279 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/module_parser/package_metadata.schema.json
--rw-rw-rw-   0 root         (0) root         (0)    14905 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/module_parser/parseModule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.159465 cosapp-0.15.4/cosapp/tools/problem_viewer/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7945 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/problem_viewer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.160465 cosapp-0.15.4/cosapp/tools/problem_viewer/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   250263 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/tests/test_viewmodeldata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.160465 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/
--rw-rw-rw-   0 root         (0) root         (0)     9254 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.161465 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/libs/
--rw-rw-rw-   0 root         (0) root         (0)     9483 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/libs/awesomplete.js
--rw-rw-rw-   0 root         (0) root         (0)   211120 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/libs/d3.v4.min.js
--rw-rw-rw-   0 root         (0) root         (0)      925 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/libs/http.js
--rw-rw-rw-   0 root         (0) root         (0)    86659 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/libs/jquery-3.2.1.min.js
--rw-rw-rw-   0 root         (0) root         (0)     4679 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/libs/vkBeautify.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.163465 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/
--rw-rw-rw-   0 root         (0) root         (0)      921 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/constants.js
--rw-rw-rw-   0 root         (0) root         (0)    16285 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/draw.js
--rw-rw-rw-   0 root         (0) root         (0)     5771 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/legend.js
--rw-rw-rw-   0 root         (0) root         (0)      647 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/modal.js
--rw-rw-rw-   0 root         (0) root         (0)    70307 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/ptN2.js
--rw-rw-rw-   0 root         (0) root         (0)     9486 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/search.js
--rw-rw-rw-   0 root         (0) root         (0)     4155 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/svg.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.164465 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/style/
--rw-rw-rw-   0 root         (0) root         (0)     1815 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/style/awesomplete.css
--rw-rw-rw-   0 root         (0) root         (0)     5612 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/style/fontello.woff
--rw-rw-rw-   0 root         (0) root         (0)     5815 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/style/partition_tree.css
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/problem_viewer/webview.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.165465 cosapp-0.15.4/cosapp/tools/templates/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.166465 cosapp-0.15.4/cosapp/tools/templates/lib/
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/templates/lib/Readme.txt
--rw-rw-rw-   0 root         (0) root         (0)   236746 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/templates/lib/d3.min.js
--rw-rw-rw-   0 root         (0) root         (0)    23777 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/templates/lib/vis.min.css
--rw-rw-rw-   0 root         (0) root         (0)   663624 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/templates/lib/vis.min.js
--rw-rw-rw-   0 root         (0) root         (0)     3800 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/templates/pythonfmu.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.167465 cosapp-0.15.4/cosapp/tools/templates/src/
--rw-rw-rw-   0 root         (0) root         (0)     4751 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/templates/src/d3_draw.js
--rw-rw-rw-   0 root         (0) root         (0)      451 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/templates/src/d3_styles.css
--rw-rw-rw-   0 root         (0) root         (0)      213 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/templates/system_d3.html
--rw-rw-rw-   0 root         (0) root         (0)     8155 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/templates/system_repr.html
--rw-rw-rw-   0 root         (0) root         (0)     6675 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.168465 cosapp-0.15.4/cosapp/tools/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2583 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/views/baseRenderer.py
--rw-rw-rw-   0 root         (0) root         (0)     6755 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/views/d3js.py
--rw-rw-rw-   0 root         (0) root         (0)     4753 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/views/markdown.py
--rw-rw-rw-   0 root         (0) root         (0)    20440 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/views/prettyprint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.169465 cosapp-0.15.4/cosapp/tools/views/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/views/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3951 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/views/tests/test_VisJsRenderer.py
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/views/tests/test_d3.py
--rw-rw-rw-   0 root         (0) root         (0)     7927 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/views/tests/test_markdown.py
--rw-rw-rw-   0 root         (0) root         (0)     5912 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/views/tests/test_prettyprint.py
--rw-rw-rw-   0 root         (0) root         (0)    15789 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tools/views/visjs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.176465 cosapp-0.15.4/cosapp/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)     3288 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/00-Introduction.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    20810 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/01-Systems.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    15181 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/02-Ports.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    18919 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/03-Drivers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2711 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/04-Triggers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    18216 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/05-Validation.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10391 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/06-Visibility.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     8547 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/07-Metamodels.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    23655 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/08-Multipoints-Design.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    14617 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/09-MonteCarlo.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5749 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/10-Recorders.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10256 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/11-DesignMethods.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    11006 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/CustomConnectors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     3536 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/FMI.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    28157 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/Guidelines.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    15090 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/HybridSimulations.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    13505 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/Logging.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4336 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/Optimization.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     7358 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/SwapSystems.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    17402 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/SystemSurrogates.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    21247 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/SystemSurrogatesAdvanced.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19955 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/Targets.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19043 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/TimeDriver.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    16726 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/TimeDriverAdvanced.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    20413 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/TipsAndTricks.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10059 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/Visitors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10359 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/aa-SimpleCircuit.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      610 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/exprampode_fmu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.181465 cosapp-0.15.4/cosapp/tutorials/images/
--rw-rw-rw-   0 root         (0) root         (0)     3204 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/cosapp.svg
--rw-rw-rw-   0 root         (0) root         (0)    17745 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/design_circuit.svg
--rw-rw-rw-   0 root         (0) root         (0)    23419 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/drivers_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     6953 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/drivers_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     7366 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/drivers_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    40831 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/drivers_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     8450 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/drivers_5.svg
--rw-rw-rw-   0 root         (0) root         (0)     4537 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/drivers_nonlinear.svg
--rw-rw-rw-   0 root         (0) root         (0)     2309 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/experimental.svg
--rw-rw-rw-   0 root         (0) root         (0)    10190 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/in_progress.svg
--rw-rw-rw-   0 root         (0) root         (0)    26687 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/ports_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    19983 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/ports_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    30601 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/ports_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    16538 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/simple_circuit.svg
--rw-rw-rw-   0 root         (0) root         (0)     9156 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/systems_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    18904 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/systems_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    18945 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/systems_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    24136 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/systems_4.svg
--rw-rw-rw-   0 root         (0) root         (0)    28090 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/systems_5.svg
--rw-rw-rw-   0 root         (0) root         (0)     5070 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/tanks.svg
--rw-rw-rw-   0 root         (0) root         (0)    27536 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/triggers_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    24504 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/triggers_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6961 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/validity.svg
--rw-rw-rw-   0 root         (0) root         (0)    85431 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/images/visibility.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.182465 cosapp-0.15.4/cosapp/tutorials/multimode/
--rw-rw-rw-   0 root         (0) root         (0)     7025 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/multimode/BouncingBall.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4001 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/multimode/MultimodeOde.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5205 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/multimode/NewtonPendulum.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.182465 cosapp-0.15.4/cosapp/tutorials/optimization/
--rw-rw-rw-   0 root         (0) root         (0)     7559 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/optimization/BetzLimit.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     8420 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/optimization/Sellar.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4315 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/quickstart.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     3233 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/tutorials/time_solutions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.185465 cosapp-0.15.4/cosapp/utils/
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.186465 cosapp-0.15.4/cosapp/utils/distributions/
--rw-rw-rw-   0 root         (0) root         (0)      195 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/distributions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4555 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/distributions/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)     2693 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/distributions/normal.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.187465 cosapp-0.15.4/cosapp/utils/distributions/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/distributions/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1809 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/distributions/tests/test_distribution.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/distributions/tests/test_normal.py
--rw-rw-rw-   0 root         (0) root         (0)     2912 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/distributions/tests/test_triangular.py
--rw-rw-rw-   0 root         (0) root         (0)     1219 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/distributions/tests/test_uniform.py
--rw-rw-rw-   0 root         (0) root         (0)     4207 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/distributions/triangular.py
--rw-rw-rw-   0 root         (0) root         (0)     2193 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/distributions/uniform.py
--rw-rw-rw-   0 root         (0) root         (0)     8441 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/find_variables.py
--rw-rw-rw-   0 root         (0) root         (0)     3677 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/graph_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)     4604 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/json.py
--rw-rw-rw-   0 root         (0) root         (0)    16769 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     3694 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/naming.py
--rw-rw-rw-   0 root         (0) root         (0)    14038 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/options_dictionary.py
--rw-rw-rw-   0 root         (0) root         (0)     5169 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     3928 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/pull_variables.py
--rw-rw-rw-   0 root         (0) root         (0)     1761 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/state_io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.188465 cosapp-0.15.4/cosapp/utils/surrogate_models/
--rw-rw-rw-   0 root         (0) root         (0)     1399 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     9528 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/kriging.py
--rw-rw-rw-   0 root         (0) root         (0)    39321 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/multifi_cokriging.py
--rw-rw-rw-   0 root         (0) root         (0)     5292 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/nearest_neighbor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.189465 cosapp-0.15.4/cosapp/utils/surrogate_models/nn_interpolators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/nn_interpolators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5286 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/nn_interpolators/linear_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     3158 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/nn_interpolators/nn_base.py
--rw-rw-rw-   0 root         (0) root         (0)    18553 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/nn_interpolators/rbf_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     5287 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/nn_interpolators/weighted_interpolator.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/response_surface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.190465 cosapp-0.15.4/cosapp/utils/surrogate_models/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4611 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/tests/test_kriging.py
--rw-rw-rw-   0 root         (0) root         (0)     6925 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/tests/test_multifi_cokriging.py
--rw-rw-rw-   0 root         (0) root         (0)    16140 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/tests/test_nearest_neighbor.py
--rw-rw-rw-   0 root         (0) root         (0)     3709 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/surrogate_models/tests/test_response_surface.py
--rw-rw-rw-   0 root         (0) root         (0)     2992 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/swap_system.py
--rw-rw-rw-   0 root         (0) root         (0)     7400 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/testing.py
--rw-rw-rw-   0 root         (0) root         (0)     1334 2024-02-28 13:38:49.000000 cosapp-0.15.4/cosapp/utils/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.127465 cosapp-0.15.4/cosapp.egg-info/
--rw-r--r--   0 root         (0) root         (0)    49049 2024-02-28 13:39:09.000000 cosapp-0.15.4/cosapp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    16093 2024-02-28 13:39:09.000000 cosapp-0.15.4/cosapp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 13:39:09.000000 cosapp-0.15.4/cosapp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-28 13:39:09.000000 cosapp-0.15.4/cosapp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      244 2024-02-28 13:39:09.000000 cosapp-0.15.4/cosapp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-28 13:39:09.000000 cosapp-0.15.4/cosapp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.192465 cosapp-0.15.4/docs/
--rw-rw-rw-   0 root         (0) root         (0)     6810 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/authors.rst
--rw-rw-rw-   0 root         (0) root         (0)    11509 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/contributing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.193465 cosapp-0.15.4/docs/cosapp_theme/
--rw-rw-rw-   0 root         (0) root         (0)     2422 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/layout.html
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/searchbox.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.193465 cosapp-0.15.4/docs/cosapp_theme/static/
--rw-rw-rw-   0 root         (0) root         (0)     8997 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/cosapp.css_t
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.196465 cosapp-0.15.4/docs/cosapp_theme/static/css/
--rw-rw-rw-   0 root         (0) root         (0)     1033 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/css/custom.css
--rw-rw-rw-   0 root         (0) root         (0)    31000 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/css/font-awesome.min.css
--rw-rw-rw-   0 root         (0) root         (0)     1466 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/css/font.css
--rw-rw-rw-   0 root         (0) root         (0)      776 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/css/highlight.css
--rw-rw-rw-   0 root         (0) root         (0)    40062 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/css/kube.css
--rw-rw-rw-   0 root         (0) root         (0)     8764 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/css/kube.demo.css
--rw-rw-rw-   0 root         (0) root         (0)     9250 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/css/kube.legenda.css
--rw-rw-rw-   0 root         (0) root         (0)    30268 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/css/kube.min.css
--rw-rw-rw-   0 root         (0) root         (0)    26211 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/css/master.css
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/css/mermaid.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.198464 cosapp-0.15.4/docs/cosapp_theme/static/font/
--rw-rw-rw-   0 root         (0) root         (0)   297272 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/font/Lato-Black.woff
--rw-rw-rw-   0 root         (0) root         (0)   328952 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/font/Lato-Bold.woff
--rw-rw-rw-   0 root         (0) root         (0)   347092 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/font/Lato-BoldItalic.woff
--rw-rw-rw-   0 root         (0) root         (0)   343528 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/font/Lato-Italic.woff
--rw-rw-rw-   0 root         (0) root         (0)   323172 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/font/Lato-Regular.woff
--rw-rw-rw-   0 root         (0) root         (0)   326132 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/font/Lato-Semibold.woff
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.199465 cosapp-0.15.4/docs/cosapp_theme/static/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    98024 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/fonts/fontawesome-webfont.woff
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.199465 cosapp-0.15.4/docs/cosapp_theme/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     5930 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/img/cosapp.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.200465 cosapp-0.15.4/docs/cosapp_theme/static/js/
--rw-rw-rw-   0 root         (0) root         (0)    84380 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/js/jquery-2.1.4.min.js
--rw-rw-rw-   0 root         (0) root         (0)    56646 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/js/kube.js
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/js/kube.legenda.js
--rw-rw-rw-   0 root         (0) root         (0)    31683 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/js/kube.min.js
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/js/master.js
--rw-rw-rw-   0 root         (0) root         (0)    12047 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/js/tocbot.min.js
--rw-rw-rw-   0 root         (0) root         (0)     5219 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/static/sidebar.js_t
--rw-rw-rw-   0 root         (0) root         (0)      736 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/cosapp_theme/theme.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.201465 cosapp-0.15.4/docs/developer/
--rw-rw-rw-   0 root         (0) root         (0)     2923 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/developer/installation_cases.rst
--rw-rw-rw-   0 root         (0) root         (0)     8633 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/developer/logger.rst
--rw-rw-rw-   0 root         (0) root         (0)     1846 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/developer/project_structure.rst
--rw-rw-rw-   0 root         (0) root         (0)    12553 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/developer/scenarii.rst
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/history.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.202465 cosapp-0.15.4/docs/img/
--rw-rw-rw-   0 root         (0) root         (0)     2475 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/img/gitlab-cosapp-f4950f.svg
--rw-rw-rw-   0 root         (0) root         (0)     4393 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/img/website-docs-blue.svg
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2237 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)       59 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/license.rst
--rw-rw-rw-   0 root         (0) root         (0)     6499 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.123465 cosapp-0.15.4/docs/nb_thumbnails/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.204465 cosapp-0.15.4/docs/nb_thumbnails/_images/
--rw-rw-rw-   0 root         (0) root         (0)      299 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/nb_thumbnails/_images/desktop-download.svg
--rw-rw-rw-   0 root         (0) root         (0)      327 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/nb_thumbnails/_images/eye.svg
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/nb_thumbnails/_images/file-code.svg
--rw-rw-rw-   0 root         (0) root         (0)      225 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/nb_thumbnails/_images/file-text.svg
--rw-rw-rw-   0 root         (0) root         (0)      329 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/nb_thumbnails/_images/fold.svg
--rw-rw-rw-   0 root         (0) root         (0)      444 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/nb_thumbnails/_images/package.svg
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/nb_thumbnails/_images/pencil.svg
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/nb_thumbnails/_images/play.svg
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/nb_thumbnails/_images/plug.svg
--rw-rw-rw-   0 root         (0) root         (0)      205 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/nb_thumbnails/_images/pulse.svg
--rw-rw-rw-   0 root         (0) root         (0)      729 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/nb_thumbnails/_images/verified.svg
--rw-rw-rw-   0 root         (0) root         (0)      148 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/nb_thumbnails/_images/zap.svg
--rw-rw-rw-   0 root         (0) root         (0)      238 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/readme.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.204465 cosapp-0.15.4/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)     3759 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/source/modules.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.205464 cosapp-0.15.4/docs/tools/
--rw-rw-rw-   0 root         (0) root         (0)    13384 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tools/mermaid.py
--rw-rw-rw-   0 root         (0) root         (0)    10131 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tools/mermaid_inheritance.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.211465 cosapp-0.15.4/docs/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)     3288 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/00-Introduction.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    20810 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/01-Systems.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    15181 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/02-Ports.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    18919 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/03-Drivers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2711 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/04-Triggers.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    18216 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/05-Validation.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10391 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/06-Visibility.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     8547 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/07-Metamodels.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    23655 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/08-Multipoints-Design.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    14617 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/09-MonteCarlo.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5749 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/10-Recorders.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10256 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/11-DesignMethods.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    11006 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/CustomConnectors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     3536 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/FMI.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    28157 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/Guidelines.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    15090 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/HybridSimulations.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    13505 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/Logging.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4336 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/Optimization.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     7358 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/SwapSystems.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    17402 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/SystemSurrogates.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    21247 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/SystemSurrogatesAdvanced.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19955 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/Targets.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    19043 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/TimeDriver.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    16726 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/TimeDriverAdvanced.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    20413 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/TipsAndTricks.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10059 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/Visitors.ipynb
--rw-rw-rw-   0 root         (0) root         (0)    10359 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/aa-SimpleCircuit.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      610 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/exprampode_fmu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.216464 cosapp-0.15.4/docs/tutorials/images/
--rw-rw-rw-   0 root         (0) root         (0)    84424 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/Moise_tables_loi.jpg
--rw-rw-rw-   0 root         (0) root         (0)     3204 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/cosapp.svg
--rw-rw-rw-   0 root         (0) root         (0)    17745 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/design_circuit.svg
--rw-rw-rw-   0 root         (0) root         (0)    23419 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/drivers_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     6953 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/drivers_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     7366 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/drivers_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    40831 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/drivers_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     8450 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/drivers_5.svg
--rw-rw-rw-   0 root         (0) root         (0)     4537 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/drivers_nonlinear.svg
--rw-rw-rw-   0 root         (0) root         (0)     2309 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/experimental.svg
--rw-rw-rw-   0 root         (0) root         (0)    10190 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/in_progress.svg
--rw-rw-rw-   0 root         (0) root         (0)    26687 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/ports_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    19983 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/ports_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    30601 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/ports_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    16538 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/simple_circuit.svg
--rw-rw-rw-   0 root         (0) root         (0)     9156 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/systems_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    18904 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/systems_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    18945 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/systems_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    24136 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/systems_4.svg
--rw-rw-rw-   0 root         (0) root         (0)    28090 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/systems_5.svg
--rw-rw-rw-   0 root         (0) root         (0)     5070 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/tanks.svg
--rw-rw-rw-   0 root         (0) root         (0)    27536 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/triggers_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    24504 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/triggers_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6961 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/validity.svg
--rw-rw-rw-   0 root         (0) root         (0)    85431 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/images/visibility.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.217464 cosapp-0.15.4/docs/tutorials/multimode/
--rw-rw-rw-   0 root         (0) root         (0)     7025 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/multimode/BouncingBall.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4001 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/multimode/MultimodeOde.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5205 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/multimode/NewtonPendulum.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-28 13:39:09.217464 cosapp-0.15.4/docs/tutorials/optimization/
--rw-rw-rw-   0 root         (0) root         (0)     7559 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/optimization/BetzLimit.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     8420 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/optimization/Sellar.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4315 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/quickstart.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     3233 2024-02-28 13:38:49.000000 cosapp-0.15.4/docs/tutorials/time_solutions.py
--rw-rw-rw-   0 root         (0) root         (0)     1956 2024-02-28 13:39:09.220464 cosapp-0.15.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1071 2024-02-28 13:38:49.000000 cosapp-0.15.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.539381 cosapp-0.16.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2024-04-18 14:27:24.000000 cosapp-0.16.0/AUTHORS.md
+-rw-rw-rw-   0 root         (0) root         (0)     3579 2024-04-18 14:27:24.000000 cosapp-0.16.0/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)    47689 2024-04-18 14:27:24.000000 cosapp-0.16.0/HISTORY.md
+-rw-rw-rw-   0 root         (0) root         (0)     6572 2024-04-18 14:27:24.000000 cosapp-0.16.0/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      754 2024-04-18 14:27:24.000000 cosapp-0.16.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    51587 2024-04-18 14:27:43.539381 cosapp-0.16.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2024-04-18 14:27:24.000000 cosapp-0.16.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.446382 cosapp-0.16.0/cosapp/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.447382 cosapp-0.16.0/cosapp/base/
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.449382 cosapp-0.16.0/cosapp/core/
+-rw-rw-rw-   0 root         (0) root         (0)      231 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5176 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/configuration_schema.json
+-rw-rw-rw-   0 root         (0) root         (0)    18908 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/eval_str.py
+-rw-rw-rw-   0 root         (0) root         (0)    16116 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.451382 cosapp-0.16.0/cosapp/core/numerics/
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/numerics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    32490 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/numerics/basics.py
+-rw-rw-rw-   0 root         (0) root         (0)    28991 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/numerics/boundary.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/numerics/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2948 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/numerics/mathematicalproblem.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)    13455 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/numerics/residues.py
+-rw-rw-rw-   0 root         (0) root         (0)    19400 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/numerics/root.py
+-rw-rw-rw-   0 root         (0) root         (0)    15550 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/numerics/sobol_seq.py
+-rw-rw-rw-   0 root         (0) root         (0)     5497 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/numerics/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.452382 cosapp-0.16.0/cosapp/core/signal/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/signal/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4972 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/signal/signal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1812 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/signal/slot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.453382 cosapp-0.16.0/cosapp/core/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8079 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    15027 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/tests/test_AssignString.py
+-rw-rw-rw-   0 root         (0) root         (0)    12270 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/tests/test_CoSAppConfiguration.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/tests/test_ContextLocals.py
+-rw-rw-rw-   0 root         (0) root         (0)    12783 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/tests/test_EvalString.py
+-rw-rw-rw-   0 root         (0) root         (0)    14154 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/tests/test_Module.py
+-rw-rw-rw-   0 root         (0) root         (0)     2078 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/tests/test_time.py
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/core/variableref.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.456382 cosapp-0.16.0/cosapp/drivers/
+-rw-rw-rw-   0 root         (0) root         (0)      936 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3030 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/abstractsetofcases.py
+-rw-rw-rw-   0 root         (0) root         (0)    12356 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/abstractsolver.py
+-rw-rw-rw-   0 root         (0) root         (0)     8692 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/driver.py
+-rw-rw-rw-   0 root         (0) root         (0)     9499 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/influence.py
+-rw-rw-rw-   0 root         (0) root         (0)     2214 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/iterativecase.py
+-rw-rw-rw-   0 root         (0) root         (0)     2867 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/lineardoe.py
+-rw-rw-rw-   0 root         (0) root         (0)     3131 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/metasystembuilder.py
+-rw-rw-rw-   0 root         (0) root         (0)    10683 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/montecarlo.py
+-rw-rw-rw-   0 root         (0) root         (0)    29100 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/nonlinearsolver.py
+-rw-rw-rw-   0 root         (0) root         (0)    21207 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/optimizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1589 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/optionaldriver.py
+-rw-rw-rw-   0 root         (0) root         (0)     6789 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/runonce.py
+-rw-rw-rw-   0 root         (0) root         (0)    13004 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/runsinglecase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.457382 cosapp-0.16.0/cosapp/drivers/time/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/euler.py
+-rw-rw-rw-   0 root         (0) root         (0)    20495 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/interfaces.py
+-rw-rw-rw-   0 root         (0) root         (0)     3457 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/runge_kutta.py
+-rw-rw-rw-   0 root         (0) root         (0)    14133 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/scenario.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.462382 cosapp-0.16.0/cosapp/drivers/time/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15016 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     9212 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_BouncingBall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2599 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_DiscreteStepper.py
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_EulerExplicit.py
+-rw-rw-rw-   0 root         (0) root         (0)    21059 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_ExplicitTimeDriver.py
+-rw-rw-rw-   0 root         (0) root         (0)     1501 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_InterpolAssignString.py
+-rw-rw-rw-   0 root         (0) root         (0)     2419 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_Interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5336 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_NewtonPendulum.py
+-rw-rw-rw-   0 root         (0) root         (0)    25908 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_RungeKutta.py
+-rw-rw-rw-   0 root         (0) root         (0)    22357 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_Scenario.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_SystemInterpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1633 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_TimeAssignString.py
+-rw-rw-rw-   0 root         (0) root         (0)     4551 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_TimeStepManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     8108 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_TimeUnknownDict.py
+-rw-rw-rw-   0 root         (0) root         (0)     4516 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_TimeUnknownStack.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_TimeVarManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_TwoPointCubicInterpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)      771 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_TwoPointCubicPolynomial.py
+-rw-rw-rw-   0 root         (0) root         (0)     9926 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_event_cascades.py
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/tests/test_modevar_init.py
+-rw-rw-rw-   0 root         (0) root         (0)    21661 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/time/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    15033 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1657 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/drivers/validitycheck.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.462382 cosapp-0.16.0/cosapp/multimode/
+-rw-rw-rw-   0 root         (0) root         (0)      158 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/multimode/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6537 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/multimode/discreteStepper.py
+-rw-rw-rw-   0 root         (0) root         (0)    12822 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/multimode/event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2517 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/multimode/zeroCrossing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.463382 cosapp-0.16.0/cosapp/patterns/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/patterns/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3411 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/patterns/observer.py
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/patterns/singleton.py
+-rw-rw-rw-   0 root         (0) root         (0)      713 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/patterns/visitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.465382 cosapp-0.16.0/cosapp/ports/
+-rw-rw-rw-   0 root         (0) root         (0)      494 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/ports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16179 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/ports/connectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     1040 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/ports/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/ports/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4022 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/ports/mode_variable.py
+-rw-rw-rw-   0 root         (0) root         (0)    34280 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/ports/port.py
+-rw-rw-rw-   0 root         (0) root         (0)     5865 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/ports/unit_library.ini
+-rw-rw-rw-   0 root         (0) root         (0)    33349 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/ports/units.py
+-rw-rw-rw-   0 root         (0) root         (0)    31417 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/ports/variable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.466382 cosapp-0.16.0/cosapp/recorders/
+-rw-rw-rw-   0 root         (0) root         (0)      169 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/recorders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4628 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/recorders/dataframe_recorder.py
+-rw-rw-rw-   0 root         (0) root         (0)     7847 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/recorders/dsv_recorder.py
+-rw-rw-rw-   0 root         (0) root         (0)    14620 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/recorders/recorder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.468382 cosapp-0.16.0/cosapp/systems/
+-rw-rw-rw-   0 root         (0) root         (0)      741 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/systems/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6451 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/systems/externalsystem.py
+-rw-rw-rw-   0 root         (0) root         (0)    13327 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/systems/metamodels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1237 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/systems/processsystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     5246 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/systems/structure.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)   136481 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/systems/system.py
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/systems/system.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/systems/systemConnector.py
+-rw-rw-rw-   0 root         (0) root         (0)    15653 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/systems/systemSurrogate.py
+-rw-rw-rw-   0 root         (0) root         (0)     5515 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/systems/systemfamily.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.470382 cosapp-0.16.0/cosapp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/all_tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.474382 cosapp-0.16.0/cosapp/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/default_dataframe.json
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/export_doe.cs
+-rw-rw-rw-   0 root         (0) root         (0)      214 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/export_doe.csv
+-rw-rw-rw-   0 root         (0) root         (0)      887 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/export_doe.json
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/export_doe.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/system_config.json
+-rw-rw-rw-   0 root         (0) root         (0)      738 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/system_config_ducts.json
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss.json
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss1.json
+-rw-rw-rw-   0 root         (0) root         (0)      453 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss11.json
+-rw-rw-rw-   0 root         (0) root         (0)      932 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss11bis.json
+-rw-rw-rw-   0 root         (0) root         (0)      623 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss12.json
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss121.json
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss131.json
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss2.json
+-rw-rw-rw-   0 root         (0) root         (0)      809 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss22.json
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss222.json
+-rw-rw-rw-   0 root         (0) root         (0)      708 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss2tank.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.474382 cosapp-0.16.0/cosapp/tests/library/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/library/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/library/ports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.476382 cosapp-0.16.0/cosapp/tests/library/systems/
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/library/systems/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7259 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/library/systems/basicalgebra.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/library/systems/dynamics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3257 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/library/systems/elec.py
+-rw-rw-rw-   0 root         (0) root         (0)     8536 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/library/systems/multiply.py
+-rw-rw-rw-   0 root         (0) root         (0)    11780 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/library/systems/others.py
+-rw-rw-rw-   0 root         (0) root         (0)     4826 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/library/systems/pressurelossvarious.py
+-rw-rw-rw-   0 root         (0) root         (0)     1986 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/library/systems/vectors.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/test_ComplexDuct.py
+-rw-rw-rw-   0 root         (0) root         (0)    10011 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/test_MathematicalProblem_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)    10653 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/test_Turbofan.py
+-rw-rw-rw-   0 root         (0) root         (0)     3971 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/test_dynamics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6650 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/test_electric_circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     9221 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/test_multimode.py
+-rw-rw-rw-   0 root         (0) root         (0)     8237 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/test_system_pressureloss.py
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/test_tutorials.py
+-rw-rw-rw-   0 root         (0) root         (0)    11905 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/test_unknown_aliasing.py
+-rw-rw-rw-   0 root         (0) root         (0)     5540 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tests/test_visitor_integration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.476382 cosapp-0.16.0/cosapp/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      655 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.477382 cosapp-0.16.0/cosapp/tools/fmu/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/fmu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22336 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/fmu/exporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3204 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/fmu/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.478382 cosapp-0.16.0/cosapp/tools/fmu/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/fmu/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/fmu/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    13858 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/fmu/tests/test_exporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/fmu/tests/test_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     4117 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/help.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.478382 cosapp-0.16.0/cosapp/tools/module_parser/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/module_parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4344 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/module_parser/package_metadata.schema.json
+-rw-rw-rw-   0 root         (0) root         (0)    14977 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/module_parser/parseModule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.479382 cosapp-0.16.0/cosapp/tools/problem_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7945 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/problem_viewer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.479382 cosapp-0.16.0/cosapp/tools/problem_viewer/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   250263 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/tests/test_viewmodeldata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.480382 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/
+-rw-rw-rw-   0 root         (0) root         (0)     9254 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.481382 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/libs/
+-rw-rw-rw-   0 root         (0) root         (0)     9483 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/libs/awesomplete.js
+-rw-rw-rw-   0 root         (0) root         (0)   211120 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/libs/d3.v4.min.js
+-rw-rw-rw-   0 root         (0) root         (0)      925 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/libs/http.js
+-rw-rw-rw-   0 root         (0) root         (0)    86659 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/libs/jquery-3.2.1.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     4679 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/libs/vkBeautify.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.482382 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/
+-rw-rw-rw-   0 root         (0) root         (0)      921 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/constants.js
+-rw-rw-rw-   0 root         (0) root         (0)    16285 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/draw.js
+-rw-rw-rw-   0 root         (0) root         (0)     5771 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/legend.js
+-rw-rw-rw-   0 root         (0) root         (0)      647 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/modal.js
+-rw-rw-rw-   0 root         (0) root         (0)    70307 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/ptN2.js
+-rw-rw-rw-   0 root         (0) root         (0)     9486 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/search.js
+-rw-rw-rw-   0 root         (0) root         (0)     4155 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/svg.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.483382 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/style/
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/style/awesomplete.css
+-rw-rw-rw-   0 root         (0) root         (0)     5612 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/style/fontello.woff
+-rw-rw-rw-   0 root         (0) root         (0)     5815 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/style/partition_tree.css
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/problem_viewer/webview.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.484382 cosapp-0.16.0/cosapp/tools/templates/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.485382 cosapp-0.16.0/cosapp/tools/templates/lib/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/templates/lib/Readme.txt
+-rw-rw-rw-   0 root         (0) root         (0)   236746 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/templates/lib/d3.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    23777 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/templates/lib/vis.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   663624 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/templates/lib/vis.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     3798 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/templates/pythonfmu.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.486382 cosapp-0.16.0/cosapp/tools/templates/src/
+-rw-rw-rw-   0 root         (0) root         (0)     4751 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/templates/src/d3_draw.js
+-rw-rw-rw-   0 root         (0) root         (0)      451 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/templates/src/d3_styles.css
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/templates/system_d3.html
+-rw-rw-rw-   0 root         (0) root         (0)     8155 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/templates/system_repr.html
+-rw-rw-rw-   0 root         (0) root         (0)     6675 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.487382 cosapp-0.16.0/cosapp/tools/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2583 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/views/baseRenderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6755 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/views/d3js.py
+-rw-rw-rw-   0 root         (0) root         (0)     4753 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/views/markdown.py
+-rw-rw-rw-   0 root         (0) root         (0)    20440 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/views/prettyprint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.488382 cosapp-0.16.0/cosapp/tools/views/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/views/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3951 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/views/tests/test_VisJsRenderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/views/tests/test_d3.py
+-rw-rw-rw-   0 root         (0) root         (0)     7927 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/views/tests/test_markdown.py
+-rw-rw-rw-   0 root         (0) root         (0)     5912 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/views/tests/test_prettyprint.py
+-rw-rw-rw-   0 root         (0) root         (0)    15789 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tools/views/visjs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.495382 cosapp-0.16.0/cosapp/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)     3288 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/00-Introduction.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    20810 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/01-Systems.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    15181 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/02-Ports.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    18919 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/03-Drivers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2711 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/04-Triggers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    18216 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/05-Validation.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10391 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/06-Visibility.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     8547 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/07-Metamodels.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    23655 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/08-Multipoints-Design.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    14617 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/09-MonteCarlo.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5749 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/10-Recorders.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10256 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/11-DesignMethods.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    11006 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/CustomConnectors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     3536 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/FMI.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    28157 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/Guidelines.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    15090 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/HybridSimulations.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    13505 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/Logging.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4336 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/Optimization.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     7358 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/SwapSystems.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    17402 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/SystemSurrogates.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    21247 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/SystemSurrogatesAdvanced.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19955 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/Targets.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19043 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/TimeDriver.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    16726 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/TimeDriverAdvanced.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    20413 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/TipsAndTricks.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10059 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/Visitors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10359 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/aa-SimpleCircuit.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/exprampode_fmu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.500382 cosapp-0.16.0/cosapp/tutorials/images/
+-rw-rw-rw-   0 root         (0) root         (0)     3204 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/cosapp.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17745 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/design_circuit.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23419 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/drivers_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6953 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/drivers_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7366 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/drivers_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    40831 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/drivers_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8450 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/drivers_5.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4537 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/drivers_nonlinear.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/experimental.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10190 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/in_progress.svg
+-rw-rw-rw-   0 root         (0) root         (0)    26687 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/ports_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19983 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/ports_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    30601 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/ports_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16538 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/simple_circuit.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9156 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/systems_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18904 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/systems_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18945 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/systems_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24136 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/systems_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)    28090 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/systems_5.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/tanks.svg
+-rw-rw-rw-   0 root         (0) root         (0)    27536 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/triggers_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24504 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/triggers_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6961 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/validity.svg
+-rw-rw-rw-   0 root         (0) root         (0)    85431 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/images/visibility.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.500382 cosapp-0.16.0/cosapp/tutorials/multimode/
+-rw-rw-rw-   0 root         (0) root         (0)     7025 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/multimode/BouncingBall.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/multimode/MultimodeOde.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5205 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/multimode/NewtonPendulum.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.501382 cosapp-0.16.0/cosapp/tutorials/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)     7559 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/optimization/BetzLimit.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     8420 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/optimization/Sellar.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/quickstart.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/tutorials/time_solutions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.504382 cosapp-0.16.0/cosapp/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.505382 cosapp-0.16.0/cosapp/utils/distributions/
+-rw-rw-rw-   0 root         (0) root         (0)      195 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/distributions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4555 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/distributions/distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     2693 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/distributions/normal.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.506382 cosapp-0.16.0/cosapp/utils/distributions/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/distributions/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1809 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/distributions/tests/test_distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/distributions/tests/test_normal.py
+-rw-rw-rw-   0 root         (0) root         (0)     2912 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/distributions/tests/test_triangular.py
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/distributions/tests/test_uniform.py
+-rw-rw-rw-   0 root         (0) root         (0)     4207 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/distributions/triangular.py
+-rw-rw-rw-   0 root         (0) root         (0)     2193 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/distributions/uniform.py
+-rw-rw-rw-   0 root         (0) root         (0)     7929 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/find_variables.py
+-rw-rw-rw-   0 root         (0) root         (0)     3682 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/graph_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4604 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/json.py
+-rw-rw-rw-   0 root         (0) root         (0)    16769 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     3694 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/naming.py
+-rw-rw-rw-   0 root         (0) root         (0)    14038 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/options_dictionary.py
+-rw-rw-rw-   0 root         (0) root         (0)     5169 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/parsing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3928 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/pull_variables.py
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/state_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.507382 cosapp-0.16.0/cosapp/utils/surrogate_models/
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     9528 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/kriging.py
+-rw-rw-rw-   0 root         (0) root         (0)    39321 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/multifi_cokriging.py
+-rw-rw-rw-   0 root         (0) root         (0)     5292 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/nearest_neighbor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.508382 cosapp-0.16.0/cosapp/utils/surrogate_models/nn_interpolators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/nn_interpolators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5286 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/nn_interpolators/linear_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3158 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/nn_interpolators/nn_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    18553 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/nn_interpolators/rbf_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     5287 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/nn_interpolators/weighted_interpolator.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/response_surface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.510382 cosapp-0.16.0/cosapp/utils/surrogate_models/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4611 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/tests/test_kriging.py
+-rw-rw-rw-   0 root         (0) root         (0)     6925 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/tests/test_multifi_cokriging.py
+-rw-rw-rw-   0 root         (0) root         (0)    16140 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/tests/test_nearest_neighbor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3709 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/surrogate_models/tests/test_response_surface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2992 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/swap_system.py
+-rw-rw-rw-   0 root         (0) root         (0)     7400 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/testing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1334 2024-04-18 14:27:24.000000 cosapp-0.16.0/cosapp/utils/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.537381 cosapp-0.16.0/cosapp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    51587 2024-04-18 14:27:43.000000 cosapp-0.16.0/cosapp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    16123 2024-04-18 14:27:43.000000 cosapp-0.16.0/cosapp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 14:27:43.000000 cosapp-0.16.0/cosapp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 14:27:43.000000 cosapp-0.16.0/cosapp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      244 2024-04-18 14:27:43.000000 cosapp-0.16.0/cosapp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-18 14:27:43.000000 cosapp-0.16.0/cosapp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.511382 cosapp-0.16.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     6810 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/authors.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11509 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/contributing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.512382 cosapp-0.16.0/docs/cosapp_theme/
+-rw-rw-rw-   0 root         (0) root         (0)     2422 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/layout.html
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/searchbox.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.513382 cosapp-0.16.0/docs/cosapp_theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)     8997 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/cosapp.css_t
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.515382 cosapp-0.16.0/docs/cosapp_theme/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/css/custom.css
+-rw-rw-rw-   0 root         (0) root         (0)    31000 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/css/font-awesome.min.css
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/css/font.css
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/css/highlight.css
+-rw-rw-rw-   0 root         (0) root         (0)    40062 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/css/kube.css
+-rw-rw-rw-   0 root         (0) root         (0)     8764 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/css/kube.demo.css
+-rw-rw-rw-   0 root         (0) root         (0)     9250 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/css/kube.legenda.css
+-rw-rw-rw-   0 root         (0) root         (0)    30268 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/css/kube.min.css
+-rw-rw-rw-   0 root         (0) root         (0)    26211 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/css/master.css
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/css/mermaid.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.517382 cosapp-0.16.0/docs/cosapp_theme/static/font/
+-rw-rw-rw-   0 root         (0) root         (0)   297272 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/font/Lato-Black.woff
+-rw-rw-rw-   0 root         (0) root         (0)   328952 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/font/Lato-Bold.woff
+-rw-rw-rw-   0 root         (0) root         (0)   347092 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/font/Lato-BoldItalic.woff
+-rw-rw-rw-   0 root         (0) root         (0)   343528 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/font/Lato-Italic.woff
+-rw-rw-rw-   0 root         (0) root         (0)   323172 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/font/Lato-Regular.woff
+-rw-rw-rw-   0 root         (0) root         (0)   326132 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/font/Lato-Semibold.woff
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.518381 cosapp-0.16.0/docs/cosapp_theme/static/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    98024 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/fonts/fontawesome-webfont.woff
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.518381 cosapp-0.16.0/docs/cosapp_theme/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/img/cosapp.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.520382 cosapp-0.16.0/docs/cosapp_theme/static/js/
+-rw-rw-rw-   0 root         (0) root         (0)    84380 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/js/jquery-2.1.4.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    56646 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/js/kube.js
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/js/kube.legenda.js
+-rw-rw-rw-   0 root         (0) root         (0)    31683 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/js/kube.min.js
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/js/master.js
+-rw-rw-rw-   0 root         (0) root         (0)    12047 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/js/tocbot.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     5219 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/static/sidebar.js_t
+-rw-rw-rw-   0 root         (0) root         (0)      736 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/cosapp_theme/theme.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.520382 cosapp-0.16.0/docs/developer/
+-rw-rw-rw-   0 root         (0) root         (0)     2923 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/developer/installation_cases.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8633 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/developer/logger.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/developer/project_structure.rst
+-rw-rw-rw-   0 root         (0) root         (0)    12549 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/developer/scenarii.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/history.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.521381 cosapp-0.16.0/docs/img/
+-rw-rw-rw-   0 root         (0) root         (0)     2475 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/img/gitlab-cosapp-f4950f.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4393 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/img/website-docs-blue.svg
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2237 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/license.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6499 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.443382 cosapp-0.16.0/docs/nb_thumbnails/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.523382 cosapp-0.16.0/docs/nb_thumbnails/_images/
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/nb_thumbnails/_images/desktop-download.svg
+-rw-rw-rw-   0 root         (0) root         (0)      327 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/nb_thumbnails/_images/eye.svg
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/nb_thumbnails/_images/file-code.svg
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/nb_thumbnails/_images/file-text.svg
+-rw-rw-rw-   0 root         (0) root         (0)      329 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/nb_thumbnails/_images/fold.svg
+-rw-rw-rw-   0 root         (0) root         (0)      444 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/nb_thumbnails/_images/package.svg
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/nb_thumbnails/_images/pencil.svg
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/nb_thumbnails/_images/play.svg
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/nb_thumbnails/_images/plug.svg
+-rw-rw-rw-   0 root         (0) root         (0)      205 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/nb_thumbnails/_images/pulse.svg
+-rw-rw-rw-   0 root         (0) root         (0)      729 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/nb_thumbnails/_images/verified.svg
+-rw-rw-rw-   0 root         (0) root         (0)      148 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/nb_thumbnails/_images/zap.svg
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/readme.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.523382 cosapp-0.16.0/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)     3759 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/source/modules.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.524381 cosapp-0.16.0/docs/tools/
+-rw-rw-rw-   0 root         (0) root         (0)    13384 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tools/mermaid.py
+-rw-rw-rw-   0 root         (0) root         (0)    10131 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tools/mermaid_inheritance.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.530381 cosapp-0.16.0/docs/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)     3288 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/00-Introduction.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    20810 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/01-Systems.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    15181 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/02-Ports.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    18919 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/03-Drivers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2711 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/04-Triggers.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    18216 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/05-Validation.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10391 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/06-Visibility.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     8547 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/07-Metamodels.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    23655 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/08-Multipoints-Design.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    14617 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/09-MonteCarlo.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5749 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/10-Recorders.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10256 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/11-DesignMethods.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    11006 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/CustomConnectors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     3536 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/FMI.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    28157 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/Guidelines.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    15090 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/HybridSimulations.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    13505 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/Logging.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4336 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/Optimization.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     7358 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/SwapSystems.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    17402 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/SystemSurrogates.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    21247 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/SystemSurrogatesAdvanced.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19955 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/Targets.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    19043 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/TimeDriver.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    16726 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/TimeDriverAdvanced.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    20413 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/TipsAndTricks.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10059 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/Visitors.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)    10359 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/aa-SimpleCircuit.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/exprampode_fmu.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.535381 cosapp-0.16.0/docs/tutorials/images/
+-rw-rw-rw-   0 root         (0) root         (0)    84424 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/Moise_tables_loi.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     3204 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/cosapp.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17745 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/design_circuit.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23419 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/drivers_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6953 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/drivers_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7366 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/drivers_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    40831 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/drivers_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8450 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/drivers_5.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4537 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/drivers_nonlinear.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2309 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/experimental.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10190 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/in_progress.svg
+-rw-rw-rw-   0 root         (0) root         (0)    26687 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/ports_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19983 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/ports_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    30601 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/ports_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16538 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/simple_circuit.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9156 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/systems_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18904 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/systems_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18945 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/systems_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24136 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/systems_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)    28090 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/systems_5.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5070 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/tanks.svg
+-rw-rw-rw-   0 root         (0) root         (0)    27536 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/triggers_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24504 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/triggers_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6961 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/validity.svg
+-rw-rw-rw-   0 root         (0) root         (0)    85431 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/images/visibility.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.536381 cosapp-0.16.0/docs/tutorials/multimode/
+-rw-rw-rw-   0 root         (0) root         (0)     7025 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/multimode/BouncingBall.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/multimode/MultimodeOde.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5205 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/multimode/NewtonPendulum.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 14:27:43.537381 cosapp-0.16.0/docs/tutorials/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)     7559 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/optimization/BetzLimit.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     8420 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/optimization/Sellar.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4315 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/quickstart.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     3233 2024-04-18 14:27:24.000000 cosapp-0.16.0/docs/tutorials/time_solutions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2024-04-18 14:27:43.540381 cosapp-0.16.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-04-18 14:27:24.000000 cosapp-0.16.0/setup.py
```

### Comparing `cosapp-0.15.4/AUTHORS.md` & `cosapp-0.16.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/CONTRIBUTING.md` & `cosapp-0.16.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/HISTORY.md` & `cosapp-0.16.0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,31 @@
 # History
 
 
+## 0.16.0 (2024-04-18)
+
+### Bug fixes and code quality
+
+- Primary events triggered within the same time step are now correctly captured (MR [#287](https://gitlab.com/cosapp/cosapp/-/merge_requests/287)).
+  A bug persists when several primary events occur at the exact same time, though, as only one will be retained.
+- Fix bug preventing events from occurring during the first time step of a simulation (MR [#288](https://gitlab.com/cosapp/cosapp/-/merge_requests/288)).
+- Fix a bug causing recorders to crash when inspecting ports with properties (MR [#282](https://gitlab.com/cosapp/cosapp/-/merge_requests/282)).
+- Algebraic and time-dependent problems are now dissociated (MR [#284](https://gitlab.com/cosapp/cosapp/-/merge_requests/284)). As a consequence, invoking `self.problem.clear()` during transitions, for instance, no longer affects time-dependent unknowns such as transients.
+- Fix ambiguous warning message raised by `RunSingleCase` (MR [#279](https://gitlab.com/cosapp/cosapp/-/merge_requests/279)).
+- Various refactoring passes (MRs [#283](https://gitlab.com/cosapp/cosapp/-/merge_requests/283) and [#286](https://gitlab.com/cosapp/cosapp/-/merge_requests/286)).
+
+### Maintenance
+
+- Updated description inside the conda recipe (MR [#276](https://gitlab.com/cosapp/cosapp/-/merge_requests/276)).
+- Pin `pytest` version due to a bug in version 8.1 (MR [#280](https://gitlab.com/cosapp/cosapp/-/merge_requests/280)).
+- Add a "Citing" section in the main README file (MR [#281](https://gitlab.com/cosapp/cosapp/-/merge_requests/281)).
+- The module parser was updated (MR [#285](https://gitlab.com/cosapp/cosapp/-/merge_requests/285)).
+- Force `sphinx` < 7.3 in the documentation building environment, owing to an incompatibility with `sphinx-mdinclude` (MR [#289](https://gitlab.com/cosapp/cosapp/-/merge_requests/289)). This is a temporary patch until root cause is fixed.
+
+
 ## 0.15.4 (2024-02-28)
 
 ### Bug fixes and code quality
 
 - Fix bug raised in `NonLinearSolver` for systems with rates (MR [#268](https://gitlab.com/cosapp/cosapp/-/merge_requests/268)).
 - Minor refactoring pass (MR [#274](https://gitlab.com/cosapp/cosapp/-/merge_requests/274)).
```

### Comparing `cosapp-0.15.4/LICENSE.rst` & `cosapp-0.16.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/MANIFEST.in` & `cosapp-0.16.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/PKG-INFO` & `cosapp-0.16.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosapp
-Version: 0.15.4
+Version: 0.16.0
 Summary: CoSApp, the Collaborative System Approach.
 Home-page: https://cosapp.readthedocs.io
 Author: CoSApp Development Team
 License: Apache-2.0
 Keywords: cosapp,system simulation,system design
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -68,23 +68,56 @@
 CoSApp solvers can be combined into versatile, customized workflows that fit specific simulation intents.
 
 Have a look at the [introduction](https://cosapp.readthedocs.io/en/stable/tutorials/00-Introduction.html#), containing many tutorials!
 
 This code is the property of Safran SA.
 It uses code coming from various open-source projects (see [LICENSE](https://gitlab.com/cosapp/cosapp/blob/master/LICENSE.rst) file).
 
+# Citing
+
+If you use CoSApp, please cite us!
+
+Lac *et al.* (2024), [CoSApp: a Python library to create, simulate and design complex systems](https://doi.org/10.21105/joss.06292), Journal of Open Source Software 9(94), 6292. 
+
+BibTeX entry:
+
+```bibtex
+@article{Lac.etal:joss2024, author={Étienne Lac and Guy {De Spiegeleer} and Adrien Delsalle and Frédéric Collonval and Duc-Trung Lê and Mathias Malandain}, title={CoSApp: a Python library to create, simulate and design complex systems}, journal={Journal of Open Source Software}, year={2024}, volume={9}, number={94}, pages={6292}, doi={10.21105/joss.06292}, publisher={The Open Journal}}
+```
+
 # Try it now!
 
 Run a Jupyter Lab instance with binder to try out CoSApp features through examples.
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/cosapp%2Fcosapp/master?urlpath=lab/tree/docs/tutorials)
 
 # History
 
 
+## 0.16.0 (2024-04-18)
+
+### Bug fixes and code quality
+
+- Primary events triggered within the same time step are now correctly captured (MR [#287](https://gitlab.com/cosapp/cosapp/-/merge_requests/287)).
+  A bug persists when several primary events occur at the exact same time, though, as only one will be retained.
+- Fix bug preventing events from occurring during the first time step of a simulation (MR [#288](https://gitlab.com/cosapp/cosapp/-/merge_requests/288)).
+- Fix a bug causing recorders to crash when inspecting ports with properties (MR [#282](https://gitlab.com/cosapp/cosapp/-/merge_requests/282)).
+- Algebraic and time-dependent problems are now dissociated (MR [#284](https://gitlab.com/cosapp/cosapp/-/merge_requests/284)). As a consequence, invoking `self.problem.clear()` during transitions, for instance, no longer affects time-dependent unknowns such as transients.
+- Fix ambiguous warning message raised by `RunSingleCase` (MR [#279](https://gitlab.com/cosapp/cosapp/-/merge_requests/279)).
+- Various refactoring passes (MRs [#283](https://gitlab.com/cosapp/cosapp/-/merge_requests/283) and [#286](https://gitlab.com/cosapp/cosapp/-/merge_requests/286)).
+
+### Maintenance
+
+- Updated description inside the conda recipe (MR [#276](https://gitlab.com/cosapp/cosapp/-/merge_requests/276)).
+- Pin `pytest` version due to a bug in version 8.1 (MR [#280](https://gitlab.com/cosapp/cosapp/-/merge_requests/280)).
+- Add a "Citing" section in the main README file (MR [#281](https://gitlab.com/cosapp/cosapp/-/merge_requests/281)).
+- The module parser was updated (MR [#285](https://gitlab.com/cosapp/cosapp/-/merge_requests/285)).
+- Force `sphinx` < 7.3 in the documentation building environment, owing to an incompatibility with `sphinx-mdinclude` (MR [#289](https://gitlab.com/cosapp/cosapp/-/merge_requests/289)). This is a temporary patch until root cause is fixed.
+
+
 ## 0.15.4 (2024-02-28)
 
 ### Bug fixes and code quality
 
 - Fix bug raised in `NonLinearSolver` for systems with rates (MR [#268](https://gitlab.com/cosapp/cosapp/-/merge_requests/268)).
 - Minor refactoring pass (MR [#274](https://gitlab.com/cosapp/cosapp/-/merge_requests/274)).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cosapp-0.15.4/README.md` & `cosapp-0.16.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,12 +20,24 @@
 CoSApp solvers can be combined into versatile, customized workflows that fit specific simulation intents.
 
 Have a look at the [introduction](https://cosapp.readthedocs.io/en/stable/tutorials/00-Introduction.html#), containing many tutorials!
 
 This code is the property of Safran SA.
 It uses code coming from various open-source projects (see [LICENSE](https://gitlab.com/cosapp/cosapp/blob/master/LICENSE.rst) file).
 
+# Citing
+
+If you use CoSApp, please cite us!
+
+Lac *et al.* (2024), [CoSApp: a Python library to create, simulate and design complex systems](https://doi.org/10.21105/joss.06292), Journal of Open Source Software 9(94), 6292. 
+
+BibTeX entry:
+
+```bibtex
+@article{Lac.etal:joss2024, author={Étienne Lac and Guy {De Spiegeleer} and Adrien Delsalle and Frédéric Collonval and Duc-Trung Lê and Mathias Malandain}, title={CoSApp: a Python library to create, simulate and design complex systems}, journal={Journal of Open Source Software}, year={2024}, volume={9}, number={94}, pages={6292}, doi={10.21105/joss.06292}, publisher={The Open Journal}}
+```
+
 # Try it now!
 
 Run a Jupyter Lab instance with binder to try out CoSApp features through examples.
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/cosapp%2Fcosapp/master?urlpath=lab/tree/docs/tutorials)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cosapp-0.15.4/cosapp/core/config.py` & `cosapp-0.16.0/cosapp/core/config.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/configuration_schema.json` & `cosapp-0.16.0/cosapp/core/configuration_schema.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/eval_str.py` & `cosapp-0.16.0/cosapp/core/eval_str.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/module.py` & `cosapp-0.16.0/cosapp/core/module.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/numerics/basics.py` & `cosapp-0.16.0/cosapp/core/numerics/basics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 from __future__ import annotations
+import abc
 import logging
+import numpy
+from itertools import chain
 from collections import OrderedDict
 from numbers import Number
 from dataclasses import dataclass, field
 from typing import (
-    Any, Dict, Iterable, Optional,
-    Sequence, Union, Tuple, List,
-    Set, Callable, NamedTuple,
+    Any, Union, Iterable, Optional,
+    Dict, Tuple, List, Set,
+    Callable, NamedTuple,
+    TYPE_CHECKING, TypeVar,
 )
-
-import numpy
+if TYPE_CHECKING:
+    from cosapp.systems import System
 
 from cosapp.core.variableref import VariableReference
 from cosapp.core.numerics.boundary import Boundary, Unknown, TimeUnknown, TimeDerivative
 from cosapp.core.numerics.residues import Residue, DeferredResidue
+from cosapp.core.numerics.utils import TransferHelper
 from cosapp.utils.naming import natural_varname
 from cosapp.utils.helpers import check_arg
 
 logger = logging.getLogger(__name__)
 
 
+Self = TypeVar("Self", bound="BaseProblem")
+TimeVar = TypeVar("TimeVar", TimeUnknown, TimeDerivative)
+
+
 def default_array_factory(shape=0, dtype=float):
     """Default factory for dataclass fields."""
     def factory():
         return numpy.empty(shape, dtype=dtype)
     return factory
 
 
@@ -75,15 +84,15 @@
 
     @property
     def target(self) -> str:
         """str: targetted quantity"""
         return self.deferred.target
 
     @property
-    def context(self):
+    def context(self) -> System:
         """System: evaluation context of residue"""
         return self.deferred.context
 
     @property
     def variables(self) -> Set[str]:
         """Set[str]: names of variables involved in residue"""
         return self.deferred.variables
@@ -97,34 +106,128 @@
         return self.deferred.equation()
 
     def make_residue(self, reference=None) -> Residue:
         """Generates the residue corresponding to equation 'target == value(target)'"""
         return self.deferred.make_residue(reference)
 
 
-class MathematicalProblem:
+class BaseProblem(abc.ABC):
     """Container object for unknowns and equations.
 
     Parameters
     ----------
     name : str
         Name of the mathematical problem
     context : cosapp.systems.System
         Context in which the mathematical problem will be evaluated.
     """
-    def __init__(self, name: str, context: Optional["System"]) -> None:
+    def __init__(self, name: str, context: Optional[System]) -> None:
         from cosapp.systems import System
         check_arg(context, 'context', (System, type(None)))
-        # TODO add point label to associate set of equations with Single Case
         self._name = name  # type: str
         self._context: System = context
+
+    @property
+    def name(self) -> str:
+        """str : Mathematical system name."""
+        return self._name
+
+    @property
+    def context(self) -> System:
+        """cosapp.systems.System or None: Context in which mathematical objects are evaluated."""
+        return self._context
+
+    @context.setter
+    def context(self, context: Optional[System]):
+        if self._context is None:
+            from cosapp.systems import System
+            check_arg(context, 'context', (System, type(None)))
+            self._context = context
+        elif context is not self._context:
+            raise ValueError(f"Context is already set to {self._context.name!r}.")
+
+    def _check_context(self, attr_name: str) -> None:
+        if self._context is None:
+            raise AttributeError(f"Owner System is required to define {attr_name}.")
+
+    @abc.abstractmethod
+    def is_empty(self) -> bool:
+        pass
+
+    @abc.abstractmethod
+    def extend(
+        self: Self,
+        other: Self,
+        copy = True,
+        overwrite = False,
+        **kwargs,
+    ) -> Self:
+        """Extend the current problem with another one.
+
+        Parameters
+        ----------
+        - other [BaseProblem]:
+            The other mathematical system to add
+        - copy [bool, optional]:
+            Should the objects be copied; default is `True`.
+        - overwrite [bool, optional]:
+            If `False` (default), common attributes raise `ValueError`.
+            If `True`, attributes are silently overwritten.
+
+        Returns
+        -------
+        BaseProblem
+            The resulting problem
+        """
+        return self
+
+    @abc.abstractmethod
+    def clear(self) -> None:
+        """Clear all mathematical elements in problem."""
+        pass
+
+    def copy(self: Self) -> Self:
+        """Copy the problem into a new one.
+
+        Returns
+        -------
+        BaseProblem
+            The duplicated problem.
+        """
+        new = type(self)(self.name, self.context)
+        new.extend(self, copy=True)
+        return new
+
+    @abc.abstractmethod
+    def to_dict(self) -> Dict[str, Any]:
+        """Returns a JSONable representation of the problem.
+        
+        Returns
+        -------
+        dict[str, Any]
+            JSONable representation
+        """
+        pass
+
+
+class MathematicalProblem(BaseProblem):
+    """Container object for unknowns and equations.
+
+    Parameters
+    ----------
+    name : str
+        Name of the mathematical problem
+    context : cosapp.systems.System
+        Context in which the mathematical problem will be evaluated.
+    """
+    def __init__(self, name: str, context: Optional[System]) -> None:
+        super().__init__(name, context)
+        # TODO add point label to associate set of equations with Single Case
         self._unknowns = OrderedDict()  # type: Dict[str, Unknown]
         self._residues = OrderedDict()  # type: Dict[str, Residue]
-        self._transients = OrderedDict()  # type: Dict[str, TimeUnknown]
-        self._rates = OrderedDict()  # type: Dict[str, TimeDerivative]
         self._targets = OrderedDict()  # type: Dict[str, WeakDeferredResidue]
 
     def __repr__(self) -> str:
         lines = []
         indent = "  "
         def format_unknown(items: Tuple[str, Unknown]) -> str:
             key, unknown = items
@@ -147,31 +250,14 @@
             lines.extend(
                 f"{indent}{deferred.equation()} (target)"
                 for deferred in self.deferred_residues.values()
             )
         return "\n".join(lines) if lines else "empty problem"
 
     @property
-    def name(self) -> str:
-        """str : Mathematical system name."""
-        return self._name
-
-    @property
-    def context(self) -> Optional['cosapp.systems.System']:
-        """cosapp.systems.System or None: Context in which mathematical objects are evaluated."""
-        return self._context
-
-    @context.setter
-    def context(self, context: Optional['cosapp.systems.System']):
-        if self._context is None:
-            self._context = context
-        elif context is not self._context:
-            raise ValueError(f"Context is already set to {self._context.name!r}.")
-
-    @property
     def residues(self) -> Dict[str, Residue]:
         """Dict[str, Residue]: Residue dictionary defined in problem."""
         return self._residues
 
     @property
     def unknowns(self) -> Dict[str, Unknown]:
         """Dict[str, Unknown]: Unknown dictionary defined in problem."""
@@ -181,15 +267,15 @@
         """numpy.ndarray: Residue values stacked into a vector."""
         return self.__as_vector(self.residues)
 
     def unknown_vector(self):
         """numpy.ndarray: Unknown values stacked into a vector."""
         return self.__as_vector(self.unknowns)
 
-    def __as_vector(self, collection: dict):
+    def __as_vector(self, collection: dict[str, Union[Unknown, Residue]]):
         values = tuple(
             numpy.ravel(element.value) for element in collection.values()
         )
         return numpy.concatenate(values) if values else numpy.empty(0)
 
     def residue_names(self) -> Tuple[str]:
         """Tuple[str]: Names of residues, flattened to have the same size as `residue_vector()`."""
@@ -239,15 +325,15 @@
 
     @property
     def shape(self) -> Tuple[int, int]:
         """(int, int) : Number of unknowns and equations."""
         return (self.n_unknowns, self.n_equations)
 
     def is_empty(self) -> bool:
-        return self.shape == (0, 0)
+        return self.n_unknowns == self.n_equations == 0
 
     def add_unknown(self,
         name: Union[str, Iterable[Union[dict, str, Unknown]]],
         max_abs_step: Number = numpy.inf,
         max_rel_step: Number = numpy.inf,
         lower_bound: Number = -numpy.inf,
         upper_bound: Number = numpy.inf,
@@ -274,16 +360,16 @@
             Mask of unknown values in the vector variable
 
         Returns
         -------
         MathematicalProblem
             The modified MathematicalSystem
         """
-        self.__check_context("unknowns")
-        context = self.context
+        self._check_context("unknowns")
+        context = self._context
 
         def add_unknown(
             name: str,
             max_abs_step: Number = numpy.inf,
             max_rel_step: Number = numpy.inf,
             lower_bound: Number = -numpy.inf,
             upper_bound: Number = numpy.inf,
@@ -362,15 +448,15 @@
             If value is "norm", actual reference value is estimated from order of magnitude.
 
         Returns
         -------
         MathematicalProblem
             The modified MathematicalSystem
         """
-        self.__check_context("equations")
+        self._check_context("equations")
         context = self.context
 
         def add_residue(equation, name=None, reference=1):
             """Add residue from equation."""
             residue = Residue(context, equation, name, reference)
             self._residues[residue.name] = residue
 
@@ -405,15 +491,15 @@
             If True, the target is disregarded if the corresponding variable is connected; default is `False`.
 
         Returns
         -------
         MathematicalProblem
             The modified MathematicalSystem
         """
-        self.__check_context("targets")
+        self._check_context("targets")
         context = self.context
 
         def register(name, reference=1):
             deferred = DeferredResidue(context, name, reference)
             if len(deferred.variables) > 1:
                 raise NotImplementedError(
                     f"Targets are only supported for single variables; got {deferred.variables}"
@@ -457,26 +543,218 @@
         return f"{target} (target)"
 
     @property
     def deferred_residues(self) -> Dict[str, WeakDeferredResidue]:
         """Dict[str, WeakDeferredResidue]: Dict of deferred residues defined for this system."""
         return self._targets
 
+    def extend(self,
+        other: MathematicalProblem,
+        copy = True,
+        overwrite = False,
+        unknowns = True,
+        equations = True,
+        unknown_wrapper: Optional[Callable[[str], str]] = None,
+        residue_wrapper: Optional[Callable[[str], str]] = None,
+    ) -> MathematicalProblem:
+        """Extend the current mathematical problem with another one.
+
+        Parameters
+        ----------
+        - other [MathematicalProblem]:
+            The other mathematical system to add
+        - copy [bool, optional]:
+            Should the objects be copied; default is `True`.
+        - overwrite [bool, optional]:
+            If `False` (default), common unknowns/equations raise `ValueError`.
+            If `True`, attributes are silently overwritten.
+        - unknowns [bool, optional]:
+            If `False`, unknowns are discarded; default is `True`.
+        - equations [bool, optional]:
+            If `False`, equations are discarded; default is `True`.
+
+        Returns
+        -------
+        MathematicalProblem
+            The merged mathematical problem
+        """
+        no_wrapping = (unknown_wrapper is residue_wrapper is None)
+        if other is self and not copy and no_wrapping:
+            return self  # quick return
+
+        if unknown_wrapper is None:
+            unknown_wrapper = lambda key: key
+        if residue_wrapper is None:
+            residue_wrapper = lambda key: key
+
+        context: System = self.context
+        other_context: System = other.context
+
+        helper = TransferHelper(context)
+        var_key_format = TransferHelper.variable_key_format
+
+        def transfer(attr_name: str, transfer_func: Callable, name_wrapper: Callable[[str], str]):
+            source: dict = getattr(other, attr_name)
+            destination: dict = getattr(self, attr_name)
+            transferred = transfer_func(
+                source.values(),
+                name_wrapper=name_wrapper,
+                copy=copy,
+            )
+            if not overwrite:
+                common = set(destination).intersection(transferred)
+                if common:
+                    if len(common) == 1:
+                        message = f"{common.pop()!r} already exists"
+                    else:
+                        message = f"{sorted(common)} already exist"
+                    raise ValueError(f"{message} in {self.name!r}.")
+            destination.update(transferred)
+
+        if unknowns:
+            transfer('unknowns', helper.transfer_unknowns, unknown_wrapper)
+
+        if equations:
+            transfer('residues', helper.transfer_residues, residue_wrapper)
+
+            connectors = list(context.incoming_connectors())
+            name2variable = other_context.name2variable
+            path = helper.path_finder.get_path(other_context)
+
+            for deferred in other._targets.values():
+                targetted = list(deferred.variables)[0]
+                name = deferred.target.replace(targetted, var_key_format(path, targetted))  # default
+                ref = name2variable[targetted]
+                port, varname = ref.mapping, ref.key
+                # Check if targetted variable is a pulled output
+                if port.is_output:
+                    for connector in connectors:
+                        pulled = (
+                            connector.source is port
+                            and varname in connector.source_variables()
+                        )
+                        if pulled:
+                            alias_name = natural_varname(
+                                f"{connector.sink.name}.{connector.sink_variable(varname)}"
+                            )
+                            original = name
+                            if deferred.target == targetted:
+                                name = alias_name
+                            else:
+                                # target is an expression involving `targetted`
+                                name = name.replace(var_key_format(path, targetted), alias_name)
+                            logger.info(
+                                f"Target on {original!r} will be based on {name!r} in the context of {context.full_name()!r}"
+                            )
+                            break
+                self.add_target(name, weak=deferred.weak)
+
+        return self
+
+    def clear(self) -> None:
+        """Clear all mathematical elements in this problem."""
+        self._unknowns.clear()
+        self._residues.clear()
+        self._targets.clear()
+
+    def copy(self, activate_targets=False) -> MathematicalProblem:
+        """Copy the `MathematicalProblem` object.
+
+        Returns
+        -------
+        MathematicalProblem
+            The duplicated mathematical problem.
+        """
+        new = super().copy()
+        if activate_targets:
+            new.activate_targets()
+        return new
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Returns a JSONable representation of the mathematical problem.
+        
+        Returns
+        -------
+        dict[str, Any]
+            JSONable representation
+        """
+        def value_to_dict(items: tuple[str, Union[Unknown, Residue]]):
+            return items[0], items[1].to_dict()
+
+        return {
+            "unknowns": dict(map(value_to_dict, self.unknowns.items())),
+            "equations": dict(map(value_to_dict, self.residues.items()))
+        }
+
+    def validate(self) -> None:
+        """Verifies that there are as many unknowns as equations defined.
+
+        Raises
+        ------
+        ArithmeticError
+            If the mathematical problem is not square.
+        """
+        n_unknowns, n_equations = self.shape
+        if n_unknowns != n_equations:
+            msg = "Nonlinear problem {} error: Mismatch between numbers of params [{}] and residues [{}]".format(
+                self.name, n_unknowns, n_equations
+            )
+            logger.error(msg)
+            logger.error(f"Residues: {list(self.residues) + list(self.deferred_residues)}")
+            logger.error(f"Variables: {list(self.unknowns)}")
+            raise ArithmeticError(msg)
+
+
+class TimeProblem(BaseProblem):
+    """Container object for time-dependent variables.
+
+    Parameters
+    ----------
+    name : str
+        Name of the mathematical problem
+    context : cosapp.systems.System
+        Context in which the mathematical problem will be evaluated.
+    """
+    def __init__(self, name: str, context: Optional[System]) -> None:
+        super().__init__(name, context)
+        self._transients = OrderedDict()  # type: Dict[str, TimeUnknown]
+        self._rates = OrderedDict()  # type: Dict[str, TimeDerivative]
+
+    def __repr__(self) -> str:
+        lines = []
+        indent = "  "
+        if self._transients:
+            lines.append(f"Transients")
+            lines.extend(
+                f"{indent}{transient.name} (derivative: {transient.der})"
+                for transient in self._transients.values()
+            )
+        if self._rates:
+            lines.append(f"Rates")
+            lines.extend(
+                f"{indent}{rate.name} (source: {rate.source_expr})"
+                for rate in self._rates.values()
+            )
+        return "\n".join(lines) if lines else "empty time problem"
+
     @property
     def transients(self) -> Dict[str, TimeUnknown]:
         """Dict[str, TimeUnknown] : Unknown time-dependent numerical features defined for this system."""
         return self._transients
 
+    def is_empty(self) -> bool:
+        return len(self._transients) == len(self._rates) == 0
+
     def add_transient(self,
         name: str,
         der: Any,
         max_time_step: Union[Number, str] = numpy.inf,
         max_abs_step: Union[Number, str] = numpy.inf,
         pulled_from: Optional[VariableReference] = None,
-    ) -> MathematicalProblem:
+    ) -> TimeProblem:
         """Add a time-dependent unknown.
 
         Parameters
         ----------
         name : str
             Name of the new time-dependent (transient) variable
         der : Any
@@ -489,18 +767,20 @@
             Original time unknown before pulling; None by default.
 
         Returns
         -------
         MathematicalProblem
             The modified MathematicalSystem
         """
-        self.__check_context("transient unknowns")
+        self._check_context("transient unknowns")
 
         if name in self._transients:
-            raise ArithmeticError(f"Variable {name!r} is already defined as a time-dependent unknown of {self.name!r}.")
+            raise ArithmeticError(
+                f"Variable {name!r} is already defined as a time-dependent unknown of {self.name!r}."
+            )
 
         self._transients[name] = TimeUnknown(
             self.context,
             name,
             der,
             max_time_step,
             max_abs_step,
@@ -509,50 +789,52 @@
         return self
 
     @property
     def rates(self) -> Dict[str, TimeDerivative]:
         """Dict[str, TimeDerivative] : Time derivatives computed during system evolution."""
         return self._rates
 
-    def add_rate(self, name: str, source: Any, initial_value: Any = None) -> MathematicalProblem:
+    def add_rate(self, name: str, source: Any, initial_value: Any = None) -> TimeProblem:
         """Add a time derivative.
 
         Parameters
         ----------
         name : str
             Name of the new time-dependent (transient) variable
         source : Any
             Name of the variable or evaluable expression whose time derivative will be computed
 
         Returns
         -------
         MathematicalProblem
             The modified MathematicalSystem
         """
-        self.__check_context("rates")
+        self._check_context("rates")
 
         if name in self._rates:
-            raise ArithmeticError(f"Variable {name!r} is already defined as a time-dependent unknown of {self.name!r}.")
+            raise ArithmeticError(
+                f"Variable {name!r} is already defined as a time-dependent unknown of {self.name!r}."
+            )
 
         self._rates[name] = TimeDerivative(self.context, name, source, initial_value)
         return self
 
-    def __check_context(self, name: str):
-        if self.context is None:
-            raise AttributeError(f"Owner System is required to define {name}.")
+    @property
+    def n_unknowns(self) -> int:
+        """int: Number of unknowns."""
+        return sum(
+            numpy.size(unknown.value) 
+            for unknown in chain(self._transients.values(), self._rates.values())
+        )
 
     def extend(self,
-        other: MathematicalProblem,
+        other: TimeProblem,
         copy = True,
-        unknowns = True,
-        equations = True,
         overwrite = False,
-        unknown_wrapper: Optional[Callable[[str], str]] = None,
-        residue_wrapper: Optional[Callable[[str], str]] = None,
-    ) -> MathematicalProblem:
+    ) -> TimeProblem:
         """Extend the current mathematical system with the other one.
 
         Parameters
         ----------
         - other [MathematicalProblem]:
             The other mathematical system to add
         - copy [bool, optional]:
@@ -566,163 +848,48 @@
             If `True`, attributes are silently overwritten.
 
         Returns
         -------
         MathematicalProblem
             The resulting mathematical system
         """
-        no_wrapping = (unknown_wrapper is residue_wrapper is None)
-        if other is self and not copy and no_wrapping:
+        if other is self and not copy:
             return self  # quick return
 
-        if unknown_wrapper is None:
-            unknown_wrapper = lambda key: key
-        if residue_wrapper is None:
-            residue_wrapper = lambda key: key
-
-        from cosapp.systems import System
-        context: System = self.context
-
-        sys_paths: Dict[int, str] = dict()
+        helper = TransferHelper(self.context)
 
-        def get_path(system: System) -> str:
-            nonlocal sys_paths
-            key = id(system)
-            try:
-                path = sys_paths[key]
-            except KeyError:
-                sys_paths[key] = path = context.get_path_to_child(system)
-            return path
-
-        def var_key_format(path: str, varname: str):
-            return f"{path}.{varname}" if path else varname
-
-        def res_key_format(path: str, eqname: str):
-            return f"{path}: {eqname}" if path else eqname
-
-        def make_key(obj: Union[Boundary, Residue], key_format, wrapper) -> str:
-            """Generic key formatter for unknowns and residues."""
-            path = get_path(obj.context)
-            key = key_format(path, obj.name)
-            return wrapper(key)
-
-        def variable_key(variable: Boundary) -> str:
-            """Generate dict key from `variable` context."""
-            return make_key(variable, var_key_format, unknown_wrapper)
-
-        def residue_key(residue: Residue) -> str:
-            """Generate dict key from `residue` context."""
-            return make_key(residue, res_key_format, residue_wrapper)
-
-        get = (lambda obj: obj.copy()) if copy else (lambda obj: obj)
-
-        def transfer_unknowns(kind: str):
-            """Transfer unknowns from other mathematical problem"""
-            source = getattr(other, kind)
-            destination = getattr(self, kind)
-            for unknown in source.values():
-                key = variable_key(unknown)
-                if not overwrite and key in destination:
-                    raise ValueError(f"{key!r} already exists in {self.name!r}.")
-                destination[key] = get(unknown)
+        def transfer_unknowns(attr_name: str):
+            """Transfer unknowns from other time problem"""
+            source: Dict[str, TimeVar] = getattr(other, attr_name)
+            unknowns: Dict[str, TimeVar] = getattr(self, attr_name)
+            transferred_unknowns = helper.transfer_unknowns(source.values(), copy=copy)
+            if not overwrite:
+                common = set(unknowns).intersection(transferred_unknowns)
+                if common:
+                    raise ValueError(f"{sorted(common)} already exist in {self.name!r}.")
+            unknowns.update(transferred_unknowns)
 
-        if unknowns:
-            transfer_unknowns('unknowns')
-            transfer_unknowns('transients')
-            transfer_unknowns('rates')
-
-        if equations:
-            residues = self._residues
-            for name, residue in other.residues.items():
-                key = residue_key(residue)
-                if not overwrite and key in residues:
-                    raise ValueError(f"{key!r} already exists in {self.name!r}.")
-                residues[key] = get(residue)
-
-            connectors = list(self.context.incoming_connectors())
-            name2variable = other.context.name2variable
-            path = get_path(other.context)
-
-            for deferred in other._targets.values():
-                targetted = list(deferred.variables)[0]
-                name = deferred.target.replace(targetted, var_key_format(path, targetted))  # default
-                ref = name2variable[targetted]
-                port, varname = ref.mapping, ref.key
-                # Check if targetted variable is a pulled output
-                if port.is_output:
-                    for connector in connectors:
-                        pulled = (
-                            connector.source is port
-                            and varname in connector.source_variables()
-                        )
-                        if pulled:
-                            alias_name = natural_varname(
-                                f"{connector.sink.name}.{connector.sink_variable(varname)}"
-                            )
-                            original = name
-                            if deferred.target == targetted:
-                                name = alias_name
-                            else:
-                                # target is an expression involving `targetted`
-                                name = name.replace(var_key_format(path, targetted), alias_name)
-                            logger.info(
-                                f"Target on {original!r} will be based on {name!r} in the context of {self.context.full_name()!r}"
-                            )
-                            break
-                self.add_target(name, weak=deferred.weak)
+        transfer_unknowns('transients')
+        transfer_unknowns('rates')
 
         return self
 
     def clear(self) -> None:
         """Clear all mathematical elements in this problem."""
-        self._unknowns.clear()
-        self._residues.clear()
         self._transients.clear()
         self._rates.clear()
-        self._targets.clear()
-
-    def copy(self, activate_targets=False) -> MathematicalProblem:
-        """Copy the `MathematicalSystem` object.
-
-        Returns
-        -------
-        MathematicalProblem
-            The duplicated mathematical problem.
-        """
-        new = MathematicalProblem(self.name, self.context)
-        new.extend(self, copy=True)
-        if activate_targets:
-            new.activate_targets()
-        return new
 
     def to_dict(self) -> Dict[str, Any]:
         """Returns a JSONable representation of the mathematical problem.
         
         Returns
         -------
         Dict[str, Any]
             JSONable representation
         """
+        def value_to_dict(items: tuple[str, TimeVar]):
+            return items[0], items[1].to_dict()
+
         return {
-            "unknowns": dict((name, unknown.to_dict()) for name, unknown in self.unknowns.items()),
-            "equations": dict((name, equation.to_dict()) for name, equation in self.residues.items()),
-            "transients": dict((name, transient.to_dict()) for name, transient in self.transients.items()),
-            "rates": dict((name, rate.to_dict()) for name, rate in self.rates.items())
+            "transients": dict(map(value_to_dict, self._transients.items())),
+            "rates": dict(map(value_to_dict, self._rates.items()))
         }
-
-    def validate(self) -> None:
-        """Verifies that there are as much unknowns as equations defined.
-
-        Raises
-        ------
-        ArithmeticError
-            If the mathematical system is not closed.
-        """
-        n_unknowns, n_equations = self.shape
-        if n_unknowns != n_equations:
-            msg = "Nonlinear problem {} error: Mismatch between numbers of params [{}] and residues [{}]".format(
-                self.name, n_unknowns, n_equations
-            )
-            logger.error(msg)
-            logger.error(f"Residues: {list(self.residues) + list(self.deferred_residues)}")
-            logger.error(f"Variables: {list(self.unknowns)}")
-            raise ArithmeticError(msg)
```

### Comparing `cosapp-0.15.4/cosapp/core/numerics/boundary.py` & `cosapp-0.16.0/cosapp/core/numerics/boundary.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/numerics/enum.py` & `cosapp-0.16.0/cosapp/core/numerics/enum.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/numerics/mathematicalproblem.schema.json` & `cosapp-0.16.0/cosapp/core/numerics/mathematicalproblem.schema.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/numerics/residues.py` & `cosapp-0.16.0/cosapp/core/numerics/residues.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/numerics/root.py` & `cosapp-0.16.0/cosapp/core/numerics/root.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/numerics/sobol_seq.py` & `cosapp-0.16.0/cosapp/core/numerics/sobol_seq.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/signal/signal.py` & `cosapp-0.16.0/cosapp/core/signal/signal.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/signal/slot.py` & `cosapp-0.16.0/cosapp/core/signal/slot.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/tests/conftest.py` & `cosapp-0.16.0/cosapp/core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/tests/test_AssignString.py` & `cosapp-0.16.0/cosapp/core/tests/test_AssignString.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/tests/test_CoSAppConfiguration.py` & `cosapp-0.16.0/cosapp/core/tests/test_CoSAppConfiguration.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/tests/test_ContextLocals.py` & `cosapp-0.16.0/cosapp/core/tests/test_ContextLocals.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/tests/test_EvalString.py` & `cosapp-0.16.0/cosapp/core/tests/test_EvalString.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/tests/test_Module.py` & `cosapp-0.16.0/cosapp/core/tests/test_Module.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/tests/test_time.py` & `cosapp-0.16.0/cosapp/core/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/time.py` & `cosapp-0.16.0/cosapp/core/time.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/core/variableref.py` & `cosapp-0.16.0/cosapp/core/variableref.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/__init__.py` & `cosapp-0.16.0/cosapp/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/abstractsetofcases.py` & `cosapp-0.16.0/cosapp/drivers/abstractsetofcases.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/abstractsolver.py` & `cosapp-0.16.0/cosapp/drivers/abstractsolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,23 @@
 
                 self._postcompute()
                 self.computed.emit()
             
             else:
                 logger.debug(f"Skip {self.name} execution - Inactive")
 
+    def _update_system(self) -> None:
+        """Update owner system by executing sub-drivers, if any, or owner's subsystem drivers"""
+        if self.children:
+            for subdriver in self.children.values():
+                logger.debug(f"Call {subdriver.name}.run_once()")
+                subdriver.run_once()
+        else:
+            self.owner.run_children_drivers()
+
     def _precompute(self) -> None:
         # TODO we should check that all variables are of numerical types
         super()._precompute()
         self.touch_unknowns()
 
     def touch_unknowns(self):
         for unknown in self.problem.unknowns.values():
```

### Comparing `cosapp-0.15.4/cosapp/drivers/driver.py` & `cosapp-0.16.0/cosapp/drivers/driver.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/influence.py` & `cosapp-0.16.0/cosapp/drivers/influence.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/iterativecase.py` & `cosapp-0.16.0/cosapp/drivers/iterativecase.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/lineardoe.py` & `cosapp-0.16.0/cosapp/drivers/lineardoe.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/metasystembuilder.py` & `cosapp-0.16.0/cosapp/drivers/metasystembuilder.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/montecarlo.py` & `cosapp-0.16.0/cosapp/drivers/montecarlo.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/nonlinearsolver.py` & `cosapp-0.16.0/cosapp/drivers/nonlinearsolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,22 +279,15 @@
         -------
         numpy.ndarray
             The list of residues of the `System`
         """
         x = numpy.asarray(x)
         logger.debug(f"Call fresidues with x = {x!r}")
         self.set_iteratives(x)
-
-        if self.children:
-            for subdriver in self.children.values():
-                logger.debug(f"Call {subdriver.name}.run_once()")
-                subdriver.run_once()
-        else:
-            self.owner.run_children_drivers()
-
+        self._update_system()
         self.__builder.update_residues()
         residues = self.problem.residue_vector()
         logger.debug(f"Residues: {residues!r}")
         return residues
 
     def set_iteratives(self, x: Sequence[float]) -> None:
         x = numpy.asarray(x)
```

### Comparing `cosapp-0.15.4/cosapp/drivers/optimizer.py` & `cosapp-0.16.0/cosapp/drivers/optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import (
     Union, Iterable, Callable, Optional,
     Any, Sequence, Dict, List, Set, Tuple,
 )
 from collections.abc import Collection
 
 from cosapp.core.eval_str import EvalString
-from cosapp.core.numerics.basics import MathematicalProblem, SolverResults
+from cosapp.core.numerics.basics import SolverResults
 from cosapp.core.numerics.boundary import Unknown
 from cosapp.drivers.abstractsolver import AbstractSolver
 from cosapp.drivers.optionaldriver import OptionalDriver
 from cosapp.drivers.utils import ConstraintParser, dealias_problem
 from cosapp.recorders.recorder import BaseRecorder
 from cosapp.utils.options_dictionary import OptionsDictionary
 from cosapp.utils.helpers import check_arg
@@ -204,20 +204,20 @@
             return None
 
     @property
     def objective_expr(self) -> str:
         return str(self._objective) if self._objective else None
 
     def add_unknown(self,
-            name: Union[str, Iterable[Union[dict, str, Unknown]]],
-            max_abs_step: Number = numpy.inf,
-            max_rel_step: Number = numpy.inf,
-            lower_bound: Number = -numpy.inf,
-            upper_bound: Number = numpy.inf
-    ) -> "MathematicalProblem":
+        name: Union[str, Iterable[Union[dict, str, Unknown]]],
+        max_abs_step: Number = numpy.inf,
+        max_rel_step: Number = numpy.inf,
+        lower_bound: Number = -numpy.inf,
+        upper_bound: Number = numpy.inf
+    ) -> None:
         """Add unknown variables.
 
         You can set variable one by one or provide a list of dictionary to set multiple variable at once. The
         dictionary key are the arguments of this method.
 
         Parameters
         ----------
@@ -292,41 +292,32 @@
         self.__current_x = numpy.empty(0)
         
         # Resolve unknown aliasing and connected unknowns
         self.problem = dealias_problem(self._raw_problem)
         self.touch_unknowns()
 
     def _expression_wrapper(self, expression: EvalString) -> Callable[[numpy.ndarray], float]:
-        """Wrapper around objective and constraint expression to propagate the x values in the
-            `System` owner.
+        """Wrapper around objective and constraint expression to propagate
+        the unknown x values in the owner system.
 
         Parameters
         ----------
         expression : EvalString
             The expression to be evaluated.
 
         Returns
         -------
         Callable[[numpy.ndarray], float]
             Callable objective function usable by scipy.optimize.minimize
         """
-        if self.children:
-            def wrapper(x: numpy.ndarray, *args) -> float:
-                modified = self._update_unknowns(x)
-                if modified:
-                    for driver in self.children.values():
-                        driver.run_once()
-                return expression.eval()
-
-        else:
-            def wrapper(x: numpy.ndarray, *args) -> float:
-                modified = self._update_unknowns(x)
-                if modified:
-                    self.owner.run_children_drivers()
-                return expression.eval()
+        def wrapper(x: numpy.ndarray, *args) -> float:
+            modified = self._update_unknowns(x)
+            if modified:
+                self._update_system()
+            return expression.eval()
 
         return wrapper
 
     def _fresidues(self, x: numpy.ndarray) -> float:
         """
         Method used by the solver to take free variables values as input and values of the objective function (after
         running the System).
@@ -340,47 +331,40 @@
         -------
         float
             Objective function value
         """
         x = numpy.asarray(x)
         logger.debug(f"Call fresidues with x = {x!r}")
         self.set_iteratives(x)
-
-        if self.children:
-            for subdriver in self.children.values():
-                subdriver.run_once()
-        else:
-            self.owner.run_children_drivers()
+        self._update_system()
 
         objective = self._objective.eval()
         logger.debug(f"Objective: {objective!r}")
         return objective
 
     def set_iteratives(self, x: Sequence[float]) -> None:
         self._update_unknowns(x)
 
     def _update_unknowns(self, x: Sequence[float]) -> bool:
         modified = not numpy.array_equal(x, self.__current_x)
 
         if modified:
-            x = numpy.asarray(x)
+            self.__current_x = x = numpy.array(x)  # force copy
             counter = 0
             for unknown in self.problem.unknowns.values():
                 if unknown.mask is None:
                     unknown.set_default_value(x[counter])
                     counter += 1
                 else:
                     n = numpy.count_nonzero(unknown.mask)
                     unknown.set_default_value(x[counter : counter + n])
                     counter += n
                 # Set variable to new x
                 unknown.set_to_default()
 
-            self.__current_x = numpy.array(x)  # force copy
-
         return modified
 
     def resolution_method(self,
         fresidues: Callable[[Sequence[float]], float],
         x0: numpy.ndarray,
         args: Tuple[Union[float, str], bool] = (),
         options: Optional[OptionsDictionary] = None,
```

### Comparing `cosapp-0.15.4/cosapp/drivers/optionaldriver.py` & `cosapp-0.16.0/cosapp/drivers/optionaldriver.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/runonce.py` & `cosapp-0.16.0/cosapp/drivers/runonce.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,21 +143,22 @@
     def setup_run(self):
         """Method called once before starting any simulation."""
         super().setup_run()
         owner = self.owner
 
         if not owner.is_standalone() and owner.parent is None:
             owner.open_loops()  # Force loops opening to test if the owner needs a solver
+            problem = self.get_problem()
 
-            if not self.get_problem().is_empty():
+            if not problem.is_empty():
                 logger.warning(
-                    "Required iterations detected, not taken into account in {} driver.".format(
-                        type(self).__qualname__
-                    )
+                    f"A mathematical problem on system {owner.full_name()!r} was detetected,"
+                    f" but will not be solved by {type(self).__qualname__} driver {self.full_name()!r}."
                 )
+                logger.debug(f"Problem:\n{problem}")
 
             owner.close_loops()
 
     def _precompute(self):
         """Set execution order and start the recorder."""
         super()._precompute()
         # Solution cannot be cleared in setup_run otherwise it won't be available when get_init is called.
```

### Comparing `cosapp-0.15.4/cosapp/drivers/runsinglecase.py` & `cosapp-0.16.0/cosapp/drivers/runsinglecase.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,16 +125,23 @@
             return handler.merged_problem(name=name, offdesign_prefix=None, copy=copy)
         except ValueError as error:
             error.args = (f"{error.args[0]} in {name!r}",)
             raise
 
     def setup_run(self):
         """Method called once before starting any simulation."""
+        self.problem = None
         super().setup_run()
-        
+        if self.problem is None:
+            self._assemble_problem()
+
+    def _assemble_problem(self) -> None:
+        """Create the mathematical problem defined on case,
+        by assembling the owner problem with locally defined constraints.
+        """
         raw = self.__raw_problem
         # Transfer problem copies from `raw` to `processed`
         processed = raw.copy(prune=False)
 
         # Add owner off-design problem to `processed.offdesign`
         owner_problem = self.owner.assembled_problem()
         processed.offdesign.extend(owner_problem)
@@ -166,16 +173,15 @@
         super()._precompute()
 
         # Set boundary conditions
         self.apply_values()
 
         # Set offdesign variables
         design_unknowns = set(self.design.unknowns)
-        problem = self.get_problem()
-        for name, unknown in problem.unknowns.items():
+        for name, unknown in self.problem.unknowns.items():
             if name in design_unknowns:
                 continue
             if not numpy.array_equal(unknown.value, unknown.default_value):
                 unknown.set_to_default()
 
     def apply_values(self) -> None:
         owner_changed = False
@@ -196,18 +202,16 @@
 
         Returns
         -------
         MathematicalProblem
             The full mathematical problem to solve for the case
         """
         if self.problem is None:
-            logger.warning("RunSingleCase.get_problem called with no prior call to RunSingleCase.setup_run.")
-            return MathematicalProblem(self.name, self.owner)
-        else:
-            return self.problem
+            self._assemble_problem()
+        return self.problem
 
     def set_values(self, modifications: Dict[str, Any]) -> None:
         """Enter the set of variables defining the case, from a dictionary of the kind {'variable1': value1, ...}
         Note: will erase all previously defined values. Use 'add_values' to append new case values.
 
         The variable can be contextual `child1.port2.var`. The only rule is that it should belong to
         the owner `System` of this driver or any of its descendants.
```

### Comparing `cosapp-0.15.4/cosapp/drivers/time/euler.py` & `cosapp-0.16.0/cosapp/drivers/time/euler.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/interfaces.py` & `cosapp-0.16.0/cosapp/drivers/time/interfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,47 +319,52 @@
                             xs = (t, t + dt),
                             ys = data[0::2],  # values
                             dy = data[1::2],  # derivatives
                         )
                         for name, data in tr_data.items()
                     }
                 )
-                occur = stepper.first_discrete_step()  # first step: root finding + non-primitive events
+                occurring = stepper.first_discrete_step()  # first step: root finding + non-primitive events
                 record_data()
                 record_event()
                 stepper.reevaluate_primitive_events()
                 self.transition()
-                record_event(occur.event.contextual_name)
-                record = EventRecord(occur.time, [occur.event])
-                all_events = set(stepper.present_events())
+                record_event(occurring.event.contextual_name)
+                record = EventRecord(occurring.time, [occurring.event])
+                event_cascade = set(stepper.present_events())
                 stepper.tick()
                 stepper.set_events()
 
-                while stepper.event_detected(): # following steps: event cascade
+                while stepper.event_detected():  # following steps: event cascade
                     events = stepper.discrete_step()
-                    all_events.update(events)
+                    event_cascade.update(events)
                     self.transition()
                     stamp = ", ".join(event.contextual_name for event in events)
                     record_event(stamp)
                     stepper.tick()
                     stepper.set_events()
 
-                record.events.extend(all_events - {occur.event})
+                record.events.extend(event_cascade - {occurring.event})
                 self.__recorded_events.append(record)
                 for transient in self._transients.values():
                     transient.touch()
                 for event in record.events:
                     event.context.set_dirty(PortType.IN)
-                self._set_time(occur.time)
+                self._set_time(occurring.time)
                 self._synch_transients()
-                record_data(occur.event.contextual_name)
-                must_stop = any(event.final for event in all_events)
-                next_t = occur.time
+                record_data(occurring.event.contextual_name)
+                must_stop = any(event.final for event in event_cascade)
+                next_t = occurring.time
                 dt = next_t - t
 
+                # Reevaluate transient values and derivatives @ occur.time,
+                # in case one or more primitive events were dropped
+                for key, var in owner_transients.items():
+                    tr_data[key][2:4] = value_and_derivative(var)
+            
             else:
                 next_t = t + dt
                 stepper.reevaluate_primitive_events()
                 stepper.shift()
                 must_stop = False
 
             record_dt(dt)
@@ -411,15 +416,15 @@
         for driver in self.children.values():
             driver.call_setup_run()
 
     def _set_time(self, t: Number) -> None:
         dt = t - self.time
         self.__clock.time = t
         self.__scenario.update_values()
-        self._update_children()
+        self._update_system()
         self._update_rates(dt)
 
     def __reset_time(self) -> None:
         """Reset clock time to driver start time"""
         time = self.__time_interval[0]
         logger.debug(f"Reset time to {time}")
         self.__clock.reset(time)
@@ -429,15 +434,15 @@
         self.__scenario.apply_init_values()
         self.__scenario.update_values()
         self.__init_modevars()
         self._synch_transients()
         logger.debug("Reset rates")
         for rate in self._rates.values():
             rate.reset()
-        self.__stepper.reset()
+        self.__stepper.initialize()
     
     def __init_modevars(self):
         """Force init value of output mode vars or owner system."""
         from cosapp.systems import System
         
         for system in self.owner.tree():
             system.retrieve_incoming_data()
@@ -451,18 +456,19 @@
                     )
 
     def _synch_transients(self):
         """Re-synch stacked unknowns with root variables"""
         for transient in self._transients.values():
             transient.reset()
 
-    def _update_children(self) -> None:
-        """Execute sub-drivers, if any, or owner's subsystem drivers"""
+    def _update_system(self) -> None:
+        """Update owner system by executing sub-drivers, if any, or owner's subsystem drivers"""
         if self.children:
             for driver in self.children.values():
+                logger.debug(f"Call {driver.name}.run_once()")
                 driver.run_once()
         else:
             self.owner.run_children_drivers()
 
     def _update_rates(self, dt: Number) -> None:
         """Update rate-of-changes over time interval dt"""
         if dt == 0:
@@ -470,15 +476,15 @@
         synch_needed = False
         for rate in self._rates.values():
             rate.update(dt)
             synch_needed = True
         if synch_needed:
             # Re-run dynamic system with updated (synchronized) rates
             # Equivalent to a single step fixed-point solver
-            self._update_children()
+            self._update_system()
 
     @abc.abstractmethod
     def _update_transients(self, dt: Number) -> None:
         """
         Time integration of transient variables over time step `dt`.
         Actual implementation depends on chosen numerical scheme.
         """
```

### Comparing `cosapp-0.15.4/cosapp/drivers/time/runge_kutta.py` & `cosapp-0.16.0/cosapp/drivers/time/runge_kutta.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/scenario.py` & `cosapp-0.16.0/cosapp/drivers/time/scenario.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/conftest.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_DiscreteStepper.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_DiscreteStepper.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_EulerExplicit.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_EulerExplicit.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_ExplicitTimeDriver.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_ExplicitTimeDriver.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_InterpolAssignString.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_InterpolAssignString.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_Interpolator.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_Interpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_NewtonPendulum.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_NewtonPendulum.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_RungeKutta.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_RungeKutta.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_Scenario.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_Scenario.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_SystemInterpolator.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_SystemInterpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_TimeAssignString.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_TimeAssignString.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_TimeStepManager.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_TimeStepManager.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_TimeUnknownDict.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_TimeUnknownDict.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_TimeUnknownStack.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_TimeUnknownStack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import pytest
 
 import numpy as np
+from typing import Type
 from cosapp.drivers.time.utils import TimeUnknownStack, TimeVarManager
 from cosapp.systems import System
 from .conftest import PointMass, PointMassWithPorts, DevilCase
 
 
 @pytest.fixture(scope="function")
 def make_case():
-    def factory(cls, name, **options):
+    def factory(cls: Type[System], name, **options):
         system = cls(name, **options)
         manager = TimeVarManager(system)
         return system, manager
     return factory
 
 
 @pytest.mark.parametrize("cls, branch, name", [
```

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_TimeVarManager.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_TimeVarManager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 import pytest
 
 import numpy as np
 
 from cosapp.systems import System
 from cosapp.drivers.time.utils import TimeVarManager
-from cosapp.core.numerics.basics import MathematicalProblem
-from .conftest import (
-    ScalarOde, VectorOde,
-    PointMass, PointMassWithPorts,
-    ExpRampOde, DampedMassSpring,
-    CoupledTanks,
-    )
+from cosapp.core.numerics.basics import TimeProblem
+from .conftest import PointMass, PointMassWithPorts
 
 
 @pytest.mark.parametrize("ders, expected", [
     ({}, {}),
     ({'h': 'Q / A'}, {'h': ['h', 'Q / A']}),
     ({'x': 'v'}, {'x': ['x', 'v']}),
     ({'v': 'a', 'x': 'v'}, {'x': ['x', 'v', 'a']}),
@@ -30,15 +25,15 @@
 @pytest.mark.parametrize("system, expected", [
     (PointMass('point'), dict(transients=["[x, v]"])),
     (PointMassWithPorts('point'), dict(transients=["[position.x, kinematics.v]"])),
 ])
 def test_TimeVarManager__init__(system, expected):
     m = TimeVarManager(system)
     assert m.context is system
-    assert isinstance(m.problem, MathematicalProblem)
+    assert isinstance(m.problem, TimeProblem)
     assert m.problem.context is system
     assert set(m.transients.keys()) == set(expected.get("transients", []))
     assert set(m.rates.keys()) == set(expected.get("rates", []))
 
 
 def test_TimeVarManager_context():
     a = PointMass("A")
```

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_TwoPointCubicInterpolator.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_TwoPointCubicInterpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_TwoPointCubicPolynomial.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_TwoPointCubicPolynomial.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_event_cascades.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_event_cascades.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/tests/test_modevar_init.py` & `cosapp-0.16.0/cosapp/drivers/time/tests/test_modevar_init.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/time/utils.py` & `cosapp-0.16.0/cosapp/drivers/time/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+from __future__ import annotations
 from collections.abc import MutableMapping
 from numbers import Number
 from typing import (
     Any, Dict, List, Optional, Callable,
     Iterator, TypeVar, Union, Tuple,
+    TYPE_CHECKING,
 )
 
 import numpy, numpy.polynomial
 
 from cosapp.core.eval_str import EvalString
 from cosapp.core.variableref import VariableReference
-from cosapp.core.numerics.boundary import AbstractTimeUnknown, TimeUnknown
+from cosapp.core.numerics.boundary import AbstractTimeUnknown, TimeUnknown, TimeDerivative
 from cosapp.ports.port import ExtensiblePort
 from cosapp.systems.system import System
 from cosapp.utils.helpers import check_arg
 from cosapp.drivers.time.scenario import TimeAssignString
+if TYPE_CHECKING:
+    from cosapp.drivers.time.interfaces import ExplicitTimeDriver
+
 
 T = TypeVar('T')
 
 
 class TimeUnknownStack(AbstractTimeUnknown):
     """
     Class representing a group of variables [a, b, c, ...] jointly solved by a time driver, with
@@ -117,15 +122,15 @@
         size = self.__var_size
         for i, unknown in enumerate(self.__transients):
             offset = i * size
             unknown.value = self.__sub_value(offset)
 
     def reset(self) -> None:
         """Reset stack value from original system variables"""
-        self.__value = numpy.array(list(map(lambda t: t.value, self.__transients))).ravel()
+        self.__value = numpy.ravel([var.value for var in self.__transients])
         self.touch()
 
     def touch(self) -> None:
         """Set owner systems as 'dirty'."""
         for unknown in self.__transients:
             unknown.touch()
 
@@ -284,15 +289,15 @@
     @property
     def context(self) -> System:
         """System handled by manager"""
         return self.__context
 
     @property
     def problem(self):
-        """Mathematical problem handled by manager"""
+        """Time problem handled by manager"""
         return self.__problem
 
     @context.setter
     def context(self, context: System):
         if not isinstance(context, System):
             raise TypeError("TimeVarManager context must be a system")
         self.__context = context
@@ -305,25 +310,25 @@
         variable (key) to its associated time unknown (value).
         For stand-alone, order-1 derivatives, transient unknowns are of type `TimeUnknown`.
         For higher-order derivatives, related variables are gathered into a `TimeUnknownStack` object.
         """
         return self.__transients
 
     @property
-    def rates(self) -> Dict[str, "TimeDerivative"]:
+    def rates(self) -> Dict[str, TimeDerivative]:
         """
         Dictionary of all rate variables in current system, linking each
         variable (key) to its associated TimeDerivative object (value).
         """
         return self.__problem.rates
 
     def update_transients(self) -> None:
         """Update the transient variable dictionary (see property `transients` for details)"""
         context = self.__context
-        problem = context.assembled_problem()
+        problem = context.assembled_time_problem()
         context_transients = problem.transients
         ders = dict()
         reference2name = dict()
         for name, unknown in context_transients.items():
             reference = unknown.pulled_from or unknown.context.name2variable[unknown.name]
             reference2name[reference] = name
             der_context = unknown.der.eval_context
@@ -344,16 +349,15 @@
                 root_stack_name = ", ".join(branches).join("[]")
                 context_name = context.get_path_to_child(stack_context)
                 stack_name = f"{context_name}{root_stack_name}"
                 transients_stack = map(
                     lambda name: context_transients[name], 
                     map(lambda reference: reference2name[reference], branch[:-1])
                 )
-                transients[stack_name] = TimeUnknownStack(
-                    stack_context, stack_name, list(transients_stack))
+                transients[stack_name] = TimeUnknownStack(stack_context, stack_name, list(transients_stack))
             else:  # first-order time derivative -> use current unknown
                 root_name = reference2name[root]
                 transients[root_name] = context_transients[root_name]
 
         self.__transients = transients
         self.__problem = problem
 
@@ -554,20 +558,20 @@
     return ndpoly
 
 
 class SystemInterpolator:
     """Class providing a continuous time view on a system,
     by replacing transient variables by time functions.
     """
-    def __init__(self, driver: "ExplicitTimeDriver"):
+    def __init__(self, driver: ExplicitTimeDriver):
         from cosapp.drivers.time.interfaces import ExplicitTimeDriver
         check_arg(driver, 'driver', ExplicitTimeDriver)
         self.__owner = driver
         self.__system = system = driver.owner
-        problem = system.assembled_problem()
+        problem = system.assembled_time_problem()
         self.__transients = transients = problem.transients
         self.__interp = dict.fromkeys(transients, None)
 
     @property
     def system(self) -> System:
         """System modified by interpolator"""
         return self.__system
```

### Comparing `cosapp-0.15.4/cosapp/drivers/utils.py` & `cosapp-0.16.0/cosapp/drivers/utils.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/drivers/validitycheck.py` & `cosapp-0.16.0/cosapp/drivers/validitycheck.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/multimode/discreteStepper.py` & `cosapp-0.16.0/cosapp/multimode/discreteStepper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """
 Event handling and discrete stepping
 """
+from __future__ import annotations
 import scipy.optimize
 from math import inf
 
-from typing import NamedTuple, Iterator, List, Dict, Tuple
+from typing import NamedTuple, Iterator, List, Dict, Tuple, TYPE_CHECKING
 from cosapp.multimode.event import Event
 from cosapp.utils import partition
+if TYPE_CHECKING:
+    from cosapp.drivers import Driver
+    from cosapp.drivers.time.utils import SystemInterpolator
 
 
 class TimedEvent(NamedTuple):
     """Named tuple associating an event and its occurrence time"""
     event: Event
     time: float
 
@@ -22,15 +26,15 @@
 class DiscreteStepper():
 
     __slots__ = (
         '_owner', '_state', '_system', '_sysview',
         '_interval', '_nonprimitives', '_primitives',
     )
 
-    def __init__(self, driver: "Driver"):
+    def __init__(self, driver: Driver):
         # Local import to avoid cyclic dependency
         from cosapp.drivers.time.utils import SystemInterpolator
 
         self._owner = driver
         self._system = driver.owner
         self._sysview = SystemInterpolator(driver)
         self._interval = None
@@ -50,25 +54,31 @@
 
     def reset(self) -> None:
         """Update event list, and reset all events"""
         self.set_events()
         for event in self.events():
             event.reset()
 
+    def initialize(self) -> None:
+        """Update event list, and initialize all events"""
+        self.set_events()
+        for event in self.events():
+            event.initialize()
+
     def events(self) -> Iterator[Event]:
         """Iterator on handled events"""
         return self._state.keys()
 
     def present_events(self) -> Iterator[Event]:
         """Returns an iterator on all present events"""
         return filter(lambda event: event.present, self.events())
 
     @property
-    def sysview(self) -> "SystemInterpolator":
-        """SystemInterpolator: system interpolator"""
+    def sysview(self) -> SystemInterpolator:
+        """SystemInterpolator: system interpolator used for event time finding"""
         return self._sysview
 
     @property
     def interval(self) -> Tuple[float, float]:
         """Tuple[float, float]: time interval"""
         return self._interval
 
@@ -99,22 +109,27 @@
         """Returns a `TimedEvent` named tuple containing the first primitive event triggered,
         together with its occurrence date ((None, inf) if no primitive event is triggered).
         The internal state is only updated if an event is triggered.
         This method should only be called at the first microstep of the first discrete time step.
         """
         # TODO: Possibility of several events at the same time (up to rounding errors)?
         # For instance, if an event occurs every 0.2s and another event every s...
-        triggered_events = list(filter(lambda e: e.present, self._primitives))
+        triggered_events = list(filter(lambda event: event.present, self._primitives))
         primal = TimedEvent.empty()
         for event in triggered_events:
             time = self.trigger_time(event)
             if time < primal.time:
                 primal = TimedEvent(event, time)
         self._state[primal.event] = True
         self._sysview.exec(primal.time)
+        # Cancel primitive events that occured after primal event
+        for event in triggered_events:
+            if event is not primal.event:
+                event.cancel()
+                event.reevaluate()
         return primal
 
     def event_detected(self) -> bool:
         """Tests all primitive events and returns a Boolean value indicating
         whether at least one of these events is to be triggered."""
         return any(event.to_trigger() for event in self._primitives)
 
@@ -156,8 +171,8 @@
     def shift(self) -> None:
         """Performs a time shift of all primitive events."""
         for event in self._primitives:
             event.tick()
 
     def reevaluate_primitive_events(self) -> None:
         for event in self._primitives:
-            event.reevaluate()
+            event.reevaluate()
```

### Comparing `cosapp-0.15.4/cosapp/multimode/event.py` & `cosapp-0.16.0/cosapp/multimode/event.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from __future__ import annotations
 import abc
 import logging, warnings
 from numpy import bool_ as numpy_bool
-from typing import Any, Union, Optional
+from typing import Any, Union, Optional, TYPE_CHECKING
 
 from .zeroCrossing import ZeroCrossing
 from cosapp.core.eval_str import EvalString
 from cosapp.utils.naming import NameChecker, CommonPorts
 from cosapp.utils.helpers import check_arg
+if TYPE_CHECKING:
+    from cosapp.systems import System
 
 logger = logging.getLogger(__name__)
 
 
 class EventState(abc.ABC):
     """Interface describing the inner state of an event
     """
@@ -25,20 +28,23 @@
         """Returns value associated with event.
         By default, equivalent to `must_emit()`.
         """
         return self.must_emit()
 
     @property
     def is_primitive(self) -> bool:
-        """bool: `True` if event triggering is self contained, `False` otherwise"""
+        """bool: `True` if event triggering condition is self-contained, `False` otherwise"""
         return False
 
     def reset(self) -> None:
         pass
 
+    def initialize(self) -> None:
+        pass
+
     def reevaluate(self) -> None:
         pass
 
     def tick(self) -> None:
         pass
 
     def lock(self) -> None:
@@ -59,17 +65,17 @@
         "_final",
     )
     __name_check = NameChecker(excluded=CommonPorts.names())
 
     def __init__(
         self,
         name: str,
-        context: "cosapp.systems.System",
+        context: System,
         desc: str = "",
-        trigger: Optional[Union[str, ZeroCrossing, EventState, "Event"]] = None,
+        trigger: Optional[Union[str, ZeroCrossing, EventState, Event]] = None,
         final: bool = False,
     ):
         """`Event` constructor.
 
         Parameters
         ----------
         - name [str]:
@@ -100,20 +106,20 @@
 
     @classmethod
     def name_check(cls, name: str):
         return cls.__name_check(name)
 
     @property
     def name(self) -> str:
-        """str : Event name"""
+        """str: Event name"""
         return self._name
 
     @property
     def contextual_name(self) -> str:
-        """str : Join context system name and event name.
+        """str: Join context system name and event name.
 
         If the event has no context, only its name is returned.
         """
         context = self._context
         return self._name if context is None else f"{context.name}.{self._name}"
 
     def __repr__(self) -> str:
@@ -138,28 +144,29 @@
             path = context.path_namelist()
             if trim_root:
                 path = path[1:]
         path.append(self.name)
         return ".".join(path)
 
     @property
-    def context(self) -> "cosapp.systems.System":
+    def context(self) -> System:
+        """System: context in which the event is defined"""
         return self._context
 
     @property
     def desc(self) -> str:
-        """str : Event description"""
+        """str: Event description"""
         return self._desc
 
     @property
-    def trigger(self) -> Union[ZeroCrossing, EventState, "Event"]:
+    def trigger(self) -> Union[ZeroCrossing, EventState, Event]:
         return self._trigger
 
     @trigger.setter
-    def trigger(self, trigger: Union[EventState, ZeroCrossing, str, "Event"]):
+    def trigger(self, trigger: Union[EventState, ZeroCrossing, str, Event]):
         state = None
         if isinstance(trigger, str):
             trigger = ZeroCrossing.from_comparison(trigger)
         if isinstance(trigger, ZeroCrossing):
             state = ZeroCrossingEvent(self, trigger)
         elif isinstance(trigger, Event):
             state = SynchronizedEvent(trigger)
@@ -204,14 +211,22 @@
         self._present = False
 
     def reset(self) -> None:
         """Resets the event."""
         self._state.reset()
         self._present = False
 
+    def cancel(self) -> None:
+        """Cancels the event."""
+        self._present = False
+
+    def initialize(self) -> None:
+        """Initialize the event using current state of owner system."""
+        self._state.initialize()
+
     def reevaluate(self) -> None:
         """Reevaluates the current state of the event; used to update information
         about zero-crossing events after an integration time step was interrupted by
         the triggering of an event."""
         self._state.reevaluate()
 
     def step(self) -> bool:
@@ -224,15 +239,15 @@
         # return True whenever the event has been emitted in this step
         return old ^ self._present
 
     def to_trigger(self) -> bool:
         """bool : Indicates whether the event has to be triggered in the next discrete step"""
         return self._present ^ self._state.to_emit()
 
-    def filter(self, condition: str) -> "FilteredEvent":
+    def filter(self, condition: str) -> FilteredEvent:
         """Filters event with an additional boolean condition.
         
         Parameters:
         -----------
         - condition [str]:
             Evaluable boolean condition.
         
@@ -240,15 +255,15 @@
         --------
         - trigger [FilteredEvent]:
             The filtered event state, to be used as trigger.
         """
         return FilteredEvent(self, condition)
 
     @staticmethod
-    def merge(*events: "Event") -> "MergedEvents":
+    def merge(*events: Event) -> MergedEvents:
         """Merges events into a trigger condition.
         
         Parameters:
         -----------
         - *events [Event]:
             Enumeration of events to be merged.
         
@@ -279,17 +294,29 @@
             )
         self._expr = expr
         self._direction = zeroxing.direction
         self._event = event
         self.reset()
 
     def reset(self) -> None:
+        """Reset the event, in such a way that the event will not occur
+        after the next zero-crossing function evaluation.
+        """
         self._prev = self._curr = None
         self._locked = False
 
+    def initialize(self) -> None:
+        """Initialize the event using the current value of the zero-crossing function.
+        If the value is nil, it is discarded, and the event is simply reset.
+        This prevents the event from occurring at the beginning of a simulation.
+        """
+        self.reset()
+        if (value := self.value()) != 0.:
+            self._prev = value
+
     def value(self) -> float:
         """Evaluates and returns the zero-crossing function defining the event."""
         return self._expr.eval()
 
     def zero_detected(self, next_value) -> bool:
         """Is a zero detected between previous value and `next_value`?"""
         return self._prev is not None and self._direction.zero_detected(self._prev, next_value)
@@ -303,15 +330,15 @@
 
     def to_emit(self) -> bool:
         """Checks whether the event will have to be triggered in a new discrete step"""
         if not self._locked and self._curr is None and not self._event.present:
             next_value = self.value()
             return self.zero_detected(next_value)
         return False
-        
+
     def lock(self) -> None:
         """Locks the event"""
         self._locked = True
 
     def reevaluate(self):
         """Forces the reevaluation of the zero-crossing function"""
         self._curr = self.value()
@@ -319,14 +346,15 @@
     def tick(self):
         """Performs a tick and checks whether the event can be unlocked"""
         if self._locked:
             self._locked = (self._curr == self._prev)
         self._prev = self._curr
         self._curr = None
 
+    @property
     def is_primitive(self) -> bool:
         return True
 
 
 class FilteredEvent(EventState):
     """Inner state of an event triggered by another event,
     filtered by a Boolean condition.
```

### Comparing `cosapp-0.15.4/cosapp/multimode/zeroCrossing.py` & `cosapp-0.16.0/cosapp/multimode/zeroCrossing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from __future__ import annotations
 import enum
-import re
 from typing import Dict, NamedTuple
 from cosapp.utils.helpers import check_arg
 
 
 @enum.unique
 class EventDirection(enum.Enum):
     """Enum covering zero-crossing directions"""
@@ -26,27 +26,27 @@
 
 
 class ZeroCrossing(NamedTuple):
     expression: str
     direction: EventDirection
 
     @classmethod
-    def up(cls, expression: str) -> "ZeroCrossing":
+    def up(cls, expression: str) -> ZeroCrossing:
         return cls(expression, EventDirection.UP)
- 
+
     @classmethod
-    def down(cls, expression: str) -> "ZeroCrossing":
+    def down(cls, expression: str) -> ZeroCrossing:
         return cls(expression, EventDirection.DOWN)
- 
+
     @classmethod
-    def updown(cls, expression: str) -> "ZeroCrossing":
+    def updown(cls, expression: str) -> ZeroCrossing:
         return cls(expression, EventDirection.UPDOWN)
- 
+
     @classmethod
-    def from_comparison(cls, expression: str) -> "ZeroCrossing":
+    def from_comparison(cls, expression: str) -> ZeroCrossing:
         """Interpret an expression of the kind 'lhs <op> rhs'
         as a `ZeroCrossing` object, where <op> is one of
         comparison operators:
         - `<`, `<=`
         - `==`
         - `>`, `>=`
         """
```

### Comparing `cosapp-0.15.4/cosapp/patterns/observer.py` & `cosapp-0.16.0/cosapp/patterns/observer.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/patterns/singleton.py` & `cosapp-0.16.0/cosapp/patterns/singleton.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/patterns/visitor.py` & `cosapp-0.16.0/cosapp/patterns/visitor.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/ports/connectors.py` & `cosapp-0.16.0/cosapp/ports/connectors.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/ports/enum.py` & `cosapp-0.16.0/cosapp/ports/enum.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/ports/mode_variable.py` & `cosapp-0.16.0/cosapp/ports/mode_variable.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/ports/port.py` & `cosapp-0.16.0/cosapp/ports/port.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/ports/unit_library.ini` & `cosapp-0.16.0/cosapp/ports/unit_library.ini`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/ports/units.py` & `cosapp-0.16.0/cosapp/ports/units.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/ports/variable.py` & `cosapp-0.16.0/cosapp/ports/variable.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/recorders/dataframe_recorder.py` & `cosapp-0.16.0/cosapp/recorders/dataframe_recorder.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/recorders/dsv_recorder.py` & `cosapp-0.16.0/cosapp/recorders/dsv_recorder.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/recorders/recorder.py` & `cosapp-0.16.0/cosapp/recorders/recorder.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/systems/__init__.py` & `cosapp-0.16.0/cosapp/systems/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/systems/externalsystem.py` & `cosapp-0.16.0/cosapp/systems/externalsystem.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/systems/metamodels.py` & `cosapp-0.16.0/cosapp/systems/metamodels.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/systems/processsystem.py` & `cosapp-0.16.0/cosapp/systems/processsystem.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/systems/structure.schema.json` & `cosapp-0.16.0/cosapp/systems/structure.schema.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/systems/system.py` & `cosapp-0.16.0/cosapp/systems/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import numpy
 import pandas
 
 from cosapp.patterns.visitor import Visitor
 from cosapp.core.module import Module, CommonPorts
 from cosapp.core.eval_str import EvalString
 from cosapp.core.variableref import VariableReference
-from cosapp.core.numerics.basics import MathematicalProblem
+from cosapp.core.numerics.basics import MathematicalProblem, TimeProblem
 from cosapp.core.numerics.boundary import TimeDerivative, TimeUnknown, Unknown
 from cosapp.core.time import TimeObserver
 from cosapp.ports.enum import PortType, Scope, Validity
 from cosapp.ports.port import BasePort, ExtensiblePort, ModeVarPort, Port
 from cosapp.ports.units import UnitError
 from cosapp.ports.variable import RangeValue, Types, Variable
 from cosapp.ports.connectors import BaseConnector, Connector, ConnectorError
@@ -158,15 +158,15 @@
     >>>             self.max_roots.x = max(self.roots)
     >>>         else:
     >>>             self.roots = None
     >>>             self.max_roots.x = np.nan
     """
 
     __slots__ = (
-        '__context_lock', '_is_tree_clean', '_locked', '_math',
+        '__context_lock', '_is_tree_clean', '_locked', '_math', '_time_pb',
         'design_methods', 'drivers', 'inputs', 'outputs', 'name2variable',
         '__readonly', '__events', '_meta', '__runner', '__input_mapping',
         '__loop_problem', '__child_connectors', '__pulling_connectors',
         '__free_problem',
     )
 
     INWARDS = CommonPorts.INWARDS.value  # type: ClassVar[str]
@@ -226,14 +226,15 @@
             System name
         """
         Module.__init__(self, name)
         TimeObserver.__init__(self, sign_in=False)
         from cosapp.drivers import Driver
 
         self._math = self.new_problem(name)
+        self._time_pb = TimeProblem(name, self)
         self.__loop_problem = self.new_problem('loop')
         self.drivers = collections.OrderedDict()  # type: Dict[str, Driver]
         self.design_methods = dict()  # type: Dict[str, MathematicalProblem]
         self.__readonly = dict()  # type: Dict[str, Any]
         self.__ctor_kwargs = kwargs.copy()
 
         self.__context_lock = ContextLock()
@@ -1146,15 +1147,15 @@
                 str_der = self.str_der(1)
                 desc = f"Transient variable defined as {str_der(name)} = {der}"
 
             # Need to copy the value to avoid vector linked by reference between variable and its derivative
             #  See https://gitlab.safrantech.safran/cosapp/cosapp/issues/179
             self.add_inward(name, value=deepcopy(value), desc=desc, dtype=dtype)
 
-        self._math.add_transient(name, der, max_time_step, max_abs_step)
+        self._time_pb.add_transient(name, der, max_time_step, max_abs_step)
 
     def add_rate(self,
             name: str,
             source: Any,  # `name` is the time derivative of `source`
             initial_value: Union[Number, numpy.ndarray, str] = None,
             desc: str = None,
         ) -> None:
@@ -1236,15 +1237,15 @@
                 value = None
                 dtype = (dtype, type(None))
             else:
                 value = cast(initial_value)
             
             self.add_inward(name, value=value, desc=desc, dtype=dtype)
 
-        self._math.add_rate(name, source, initial_value)
+        self._time_pb.add_rate(name, source, initial_value)
 
     def is_input_var(self, name: str) -> bool:
         """Returns `True` if `name` is the name of an input variable, `False` otherwise"""
         return self.__check_var(name, PortType.IN)
 
     def is_output_var(self, name: str) -> bool:
         """Returns `True` if `name` is the name of an output variable, `False` otherwise"""
@@ -1276,15 +1277,15 @@
         if order == 1:
             return lambda s: f"d({s})/dt"
         elif order > 1:
             return lambda s: "d^{0}({1})/dt^{0}".format(s, order)
         return lambda s: s
 
     def _precompute(self) -> None:
-        for rate in self._math.rates.values():
+        for rate in self._time_pb.rates.values():
             rate.touch()  # ensured that system is recomputed at first time step
 
     def check(self, name: Optional[str] = None) -> Union[Dict[str, Validity], Validity]:
         """Get variable value validity for a given variable, port or system or all of them.
 
         If `name` is not provided, returns a dictionary with the validity of all `System` variables;
         i.e. all variables in input and output ports including inwards and outwards of this system and
@@ -1355,21 +1356,21 @@
         # MappingProxyType forbids external modification
         return MappingProxyType(self._math.unknowns)
 
     @property
     def transients(self):
         """Returns a dictionary containing all transient unknowns in current system tree"""
         # MappingProxyType forbids external modification
-        return MappingProxyType(self._math.transients)
+        return MappingProxyType(self._time_pb.transients)
 
     @property
     def rates(self):
         """Returns a dictionary containing all time derivatives (rates) in current system tree"""
         # MappingProxyType forbids external modification
-        return MappingProxyType(self._math.rates)
+        return MappingProxyType(self._time_pb.rates)
 
     def events(self) -> Iterator[Event]:
         """Iterator on all events locally defined on system."""
         yield from self.__events.values()
 
     def all_events(self) -> Iterator[Event]:
         """Recursive iterator on all events in complete system tree."""
@@ -1422,92 +1423,149 @@
         -------
         MathematicalProblem
             The assembled mathematical problem.
         """
         problem = self.new_problem('off-design')
 
         # Make shallow copy of `self._math` properties
-        for name in ('residues', 'deferred_residues', 'unknowns', 'transients', 'rates'):
+        for name in ('residues', 'deferred_residues', 'unknowns'):
             attr = getattr(problem, name)
             attr.update(getattr(self._math, name))
 
-        def transfer_unknown(unknown, name):
+        def transfer_unknown(unknown: Unknown, new_name: str):
             options = {
                 attr: getattr(unknown, attr)
                 for attr in ('max_abs_step', 'max_rel_step', 'lower_bound', 'upper_bound')
             }
-            problem.add_unknown(name, **options)
+            problem.add_unknown(new_name, **options)
 
-        def transfer_transient(unknown, name):
-            ref = unknown.context.name2variable[unknown.basename]
+        children: dict[str, System] = self.children
+
+        for child in children.values():
+            if child.is_standalone():
+                continue
+
+            child_problem = child.assembled_problem()
+            connectors = self.__child_connectors.get(child.name, [])
+            unknowns = child_problem.unknowns
+
+            for connector in connectors:
+                # Transfer unknowns to parent (when necessary)
+                for name in list(unknowns.keys()):
+                    unknown = unknowns[name]
+                    port = unknown.port
+                    connected = (
+                        port.owner in self.children.values()
+                        and port is connector.sink 
+                        and unknown.variable in connector.sink_variables()
+                    )
+                    if connected:
+                        # Port is connected => remove unknown
+                        unknowns.pop(name)
+                        pulled = connector.source.owner is self
+                        if pulled:
+                            # Transfer unknown to parent level
+                            src = connector.source_variable(unknown.variable)
+                            transfer_unknown(unknown, f"{connector.source.name}.{src}")
+
+                # Prune target equations defined as weak if target is connected
+                origin = connector.source.owner
+                deferred_residues = origin._math.deferred_residues.values()
+
+                for deferred in filter(lambda target: target.weak, deferred_residues):
+                    targetted = list(deferred.variables)[0]
+                    ref = origin.name2variable[targetted]
+                    port = ref.mapping
+                    name = ref.key
+                    connected = (
+                        port.owner in self.children.values()
+                        and port is connector.source 
+                        and name in connector.source_variables()
+                    )
+                    if connected:
+                        # Remove deferred equation
+                        key = MathematicalProblem.target_key(f"{origin.name}.{targetted}")
+                        problem.deferred_residues.pop(key)
+
+            problem.extend(child_problem, copy=False)
+
+        return problem.extend(self.__loop_problem)
+
+    def assembled_time_problem(self) -> TimeProblem:
+        """Returns the consolidated transient problem, assembled from the entire system tree.
+
+        Returns
+        -------
+        TimeProblem
+            The assembled time problem.
+        """
+        problem = TimeProblem('off-design', self)
+
+        # Make shallow copy of `self._math` properties
+        for name in ('transients', 'rates'):
+            attr: dict = getattr(problem, name)
+            attr.update(getattr(self._time_pb, name))
+
+        def transfer_transient(transient: TimeUnknown, name: str):
+            ref = transient.context.name2variable[transient.basename]
             problem.add_transient(name, 
-                der = unknown.der,
-                max_time_step = unknown.max_time_step_expr,
-                pulled_from = unknown.pulled_from or ref,
+                der = transient.der,
+                max_time_step = transient.max_time_step_expr,
+                pulled_from = transient.pulled_from or ref,
             )
 
-        def transfer_rate(unknown, name):
+        def transfer_rate(rate: TimeDerivative, name: str):
             problem.add_rate(name,
-                source = unknown.source_expr,
-                initial_value = unknown.initial_value_expr,
+                source = rate.source_expr,
+                initial_value = rate.initial_value_expr,
             )
 
-        for child in self.children.values():
-            if child.is_standalone():
-                continue
+        popped: list[tuple[str, str]] = list()
 
-            child_problem = child.assembled_problem()
+        for child in self.children.values():
+            child_problem = child.assembled_time_problem()
             connectors = self.__child_connectors.get(child.name, [])
             transfer_items = [
-                (child_problem.unknowns, transfer_unknown),
                 (child_problem.transients, transfer_transient),
                 (child_problem.rates, transfer_rate),
             ]
 
             for connector in connectors:
-                # Transfer unknowns, transients and rates to parent (when necessary)
+                # Transfer transients and rates to parent (when necessary)
                 for unknowns, transfer in transfer_items:
                     for name in list(unknowns.keys()):
-                        unknown = unknowns[name]
+                        unknown: Unknown = unknowns[name]
                         port = unknown.port
                         connected = (
                             port.owner in self.children.values()
                             and port is connector.sink 
                             and unknown.variable in connector.sink_variables()
                         )
                         if connected:
                             # Port is connected => remove unknown
                             unknowns.pop(name)
                             if connector.source.owner is self:
                                 # Transfer unknown to parent level
                                 src = connector.source_variable(unknown.variable)
                                 transfer(unknown, f"{connector.source.name}.{src}")
-
-                # Prune target equations defined as weak if target is connected
-                origin = connector.source.owner
-                deferred_residues = origin._math.deferred_residues.values()
-
-                for deferred in filter(lambda target: target.weak, deferred_residues):
-                    targetted = list(deferred.variables)[0]
-                    ref = origin.name2variable[targetted]
-                    port = ref.mapping
-                    name = ref.key
-                    connected = (
-                        port.owner in self.children.values()
-                        and port is connector.source 
-                        and name in connector.source_variables()
-                    )
-                    if connected:
-                        # Remove deferred equation
-                        key = MathematicalProblem.target_key(f"{origin.name}.{targetted}")
-                        problem.deferred_residues.pop(key)
+                            else:
+                                popped.append(unknown.contextual_name())
 
             problem.extend(child_problem, copy=False)
 
-        return problem.extend(self.__loop_problem)
+        if popped:
+            if len(popped) == 1:
+                message = f"variable {popped[0]!r} is connected to an output"
+            else:
+                message = f"variables {popped} are connected to outputs"
+            warnings.warn(
+                f"In {self.full_name()}, time-dependent {message} and will not be computed."
+            )
+
+        return problem
 
     def get_unsolved_problem(self) -> MathematicalProblem:
         """Returns the consolidated mathematical problem, assembled from
         entire system tree, and accounting for cyclic dependency loops.
 
         Deprecated; use `assembled_problem` instead.
```

### Comparing `cosapp-0.15.4/cosapp/systems/system.schema.json` & `cosapp-0.16.0/cosapp/systems/system.schema.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/systems/systemConnector.py` & `cosapp-0.16.0/cosapp/systems/systemConnector.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/systems/systemSurrogate.py` & `cosapp-0.16.0/cosapp/systems/systemSurrogate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,24 @@
+from __future__ import annotations
 import numpy
 import collections
 import pickle
 import pandas
 import logging
 import warnings
 from numbers import Number
 from collections import OrderedDict
 from typing import (
+    TYPE_CHECKING,
     NoReturn, Any, Dict, List,
     Iterable, NamedTuple, Union,
     Optional, Type,
 )
+if TYPE_CHECKING:
+    from cosapp.systems import System
 
 from cosapp.utils.surrogate_models.base import SurrogateModel
 from cosapp.ports.enum import PortType
 from cosapp.utils.logging import LogLevel
 from cosapp.utils.helpers import check_arg
 from cosapp.utils.find_variables import find_variables, make_wishlist, natural_varname
 
@@ -88,15 +92,15 @@
     Class representing a surrogate model trained from the outputs of an owner system.
     Once the surrogate is created, it supersedes (whenever activated) the behaviour of
     `System.compute()`. 
     """
     __slots__ = ('__owner', '__state', '__need_doe')
 
     def __init__(self,
-        owner: "cosapp.systems.System",
+        owner: System,
         data_in: Union[pandas.DataFrame, Dict[str, Any]],
         model: Type[SurrogateModel],
         data_out: Optional[Union[pandas.DataFrame, Dict[str, Any]]] = None,
         postsynch: Union[str, List[str]] = '*',
         *args, **kwargs
     ):
         # CHECK ARGS
@@ -134,24 +138,24 @@
             )
             self.__check_unknowns_and_transients()
             self.__prepare_and_train()
 
         logger.debug(f"System surrogate initialized")
 
     @property
-    def owner(self)-> "cosapp.systems.System":
+    def owner(self) -> System:
         return self.__owner
 
     @property
-    def state(self)-> SystemSurrogateState:
+    def state(self) -> SystemSurrogateState:
         """SystemSurrogateState: inner state of system surrogate"""
         return self.__state
 
     @property
-    def model_type(self)-> Type[SurrogateModel]:
+    def model_type(self) -> Type[SurrogateModel]:
         return self.__state.model.get_type()
 
     @property
     def trained(self) -> bool:
         return self.__state.model.trained
 
     @property
@@ -318,15 +322,15 @@
     def dump(self, filename: str) -> None:
         """Dump current state to file"""
         logger.debug(f"Dumping metamodel in {filename}")
         with open(filename, 'wb') as fp:
             pickle.dump(self.__state, fp)
 
     @classmethod
-    def load(cls, owner: "cosapp.systems.System", filename: str) -> "SystemSurrogate":
+    def load(cls, owner: System, filename: str) -> SystemSurrogate:
         """Load system surrogate from file"""
         logger.debug(f"Loading metamodel from {filename}")
         from cosapp.systems import System
         check_arg(owner, 'owner', System)
         with open(filename, 'rb') as fp:
             state = pickle.load(fp)
         if not isinstance(state, SystemSurrogateState):
@@ -343,32 +347,32 @@
         if not trained_unknowns:
             warnings.warn(
                 "The following unknowns/transients are not part of the training set; "
                 f"future attempts to compute them with a driver may fail: "
                 f"{list(unknowns.difference(state.doe_in))}"
             )
 
-    def __get_owner_connections(self) -> "OrderedDict[str, list]":
+    def __get_owner_connections(self) -> Dict[str, list]:
         return get_dependent_connections(self.__owner)
 
 
 def flatten(iterable: Iterable) -> Iterable:
     for elem in iterable:
         if isinstance(elem, collections.abc.Iterable) and not isinstance(elem, str): 
             yield from flatten(elem)
         else:
             yield elem
 
 
-def get_dependent_connections(system: "cosapp.systems.System") -> Dict[str, PortType]:
+def get_dependent_connections(system: System) -> Dict[str, PortType]:
     """This function returns a dictionnary mapping variable names to a port direction.
     Keys are absolute paths to connected inputs and all outputs.
     Values are owner port direction.
     """
-    from cosapp.base import System
+    from cosapp.systems import System
 
     def get_connections(system: System, head_system: System) -> Dict[str, PortType]:
         """Recursive inner version of `get_dependent_connections`"""
         result = dict()
         prefix = ""
         if system is not head_system:
             prefix = f"{head_system.get_path_to_child(system)}."
@@ -402,13 +406,12 @@
 
     logger.debug(
         f"Recursive search of connected inputs and all outputs on {system.name}"
     )
     return get_connections(system, system)
 
 
-def get_unknowns_transients(system: "cosapp.systems.System") -> set:
-    res = set()
-    problem = system.assembled_problem()
-    for collection in (problem.unknowns, problem.transients):
-        res.update(collection)
-    return res
+def get_unknowns_transients(system: System) -> set[str]:
+    return set.union(
+        set(system.assembled_problem().unknowns),
+        set(system.assembled_time_problem().transients),
+    )
```

### Comparing `cosapp-0.15.4/cosapp/systems/systemfamily.py` & `cosapp-0.16.0/cosapp/systems/systemfamily.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/all_tests.py` & `cosapp-0.16.0/cosapp/tests/all_tests.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/data/export_doe.json` & `cosapp-0.16.0/cosapp/tests/data/export_doe.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/data/system_config.json` & `cosapp-0.16.0/cosapp/tests/data/system_config.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/data/system_config_ducts.json` & `cosapp-0.16.0/cosapp/tests/data/system_config_ducts.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss11bis.json` & `cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss11bis.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss12.json` & `cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss12.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss121.json` & `cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss121.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss131.json` & `cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss131.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss22.json` & `cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss22.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss222.json` & `cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss222.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/data/system_config_pressureloss2tank.json` & `cosapp-0.16.0/cosapp/tests/data/system_config_pressureloss2tank.json`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/library/ports.py` & `cosapp-0.16.0/cosapp/tests/library/ports.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/library/systems/__init__.py` & `cosapp-0.16.0/cosapp/tests/library/systems/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/library/systems/basicalgebra.py` & `cosapp-0.16.0/cosapp/tests/library/systems/basicalgebra.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/library/systems/dynamics.py` & `cosapp-0.16.0/cosapp/tests/library/systems/dynamics.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/library/systems/elec.py` & `cosapp-0.16.0/cosapp/tests/library/systems/elec.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/library/systems/multiply.py` & `cosapp-0.16.0/cosapp/tests/library/systems/multiply.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/library/systems/others.py` & `cosapp-0.16.0/cosapp/tests/library/systems/others.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/library/systems/pressurelossvarious.py` & `cosapp-0.16.0/cosapp/tests/library/systems/pressurelossvarious.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/library/systems/vectors.py` & `cosapp-0.16.0/cosapp/tests/library/systems/vectors.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/test_ComplexDuct.py` & `cosapp-0.16.0/cosapp/tests/test_ComplexDuct.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/test_MathematicalProblem_integration.py` & `cosapp-0.16.0/cosapp/tests/test_MathematicalProblem_integration.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/test_Turbofan.py` & `cosapp-0.16.0/cosapp/tests/test_Turbofan.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/test_dynamics.py` & `cosapp-0.16.0/cosapp/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/test_electric_circuit.py` & `cosapp-0.16.0/cosapp/tests/test_electric_circuit.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/test_multimode.py` & `cosapp-0.16.0/cosapp/tests/test_multimode.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,23 +179,23 @@
         self.add_outward('Requiv', 0.0)
         self.add_outward('deltaV', 0.0)
         self.add_event('switch', trigger='elec_in.V == elec_out.V')
     
     def compute(self):
         self.deltaV = self.elec_in.V - self.elec_out.V
         I = self.elec_in.I
-        self.Requiv = self.deltaV / I if abs(I) > 0 else numpy.nan
+        self.Requiv = self.deltaV / I if I != 0 else numpy.nan
 
     def transition(self):
         if self.switch.present:
             self.upbranch = not self.upbranch
             self.reconfig()
 
     def reconfig(self):
-        problem = self._math
+        problem = self.problem
         if not self.upbranch and problem.is_empty():
             self.add_unknown("R0.R").add_equation("R0.R == 500")
         else:
             problem.clear()
             self.R0.R = 100
```

### Comparing `cosapp-0.15.4/cosapp/tests/test_system_pressureloss.py` & `cosapp-0.16.0/cosapp/tests/test_system_pressureloss.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,9 +283,9 @@
     """Same as `test_system222` with redundant off-design unknowns.
     """
     s = system222
     solver = s.add_driver(NonLinearSolver("solver"))
     solver.add_child(RunSingleCase("case"))
     solver.case.add_unknown(["p2.s21.x", "s1.x"])
 
-    with pytest.raises(ValueError, match="'p2\.s21\.x' already exists in 'offdesign'"):
+    with pytest.raises(ValueError, match="\['p2\.s21\.x', 's1\.x'\] already exist in 'offdesign'"):
         s.run_drivers()
```

### Comparing `cosapp-0.15.4/cosapp/tests/test_tutorials.py` & `cosapp-0.16.0/cosapp/tests/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/test_unknown_aliasing.py` & `cosapp-0.16.0/cosapp/tests/test_unknown_aliasing.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tests/test_visitor_integration.py` & `cosapp-0.16.0/cosapp/tests/test_visitor_integration.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/__init__.py` & `cosapp-0.16.0/cosapp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/fmu/exporter.py` & `cosapp-0.16.0/cosapp/tools/fmu/exporter.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/fmu/logging.py` & `cosapp-0.16.0/cosapp/tools/fmu/logging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/fmu/tests/conftest.py` & `cosapp-0.16.0/cosapp/tools/fmu/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/fmu/tests/test_exporter.py` & `cosapp-0.16.0/cosapp/tools/fmu/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/fmu/tests/test_logging.py` & `cosapp-0.16.0/cosapp/tools/fmu/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/help.py` & `cosapp-0.16.0/cosapp/tools/help.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/module_parser/package_metadata.schema.json` & `cosapp-0.16.0/cosapp/tools/module_parser/package_metadata.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9435320216049382%*

 * *Differences: {"'$defs'": "{'portVariable': {'description': 'Variable in a port'}, 'sysPort': {'properties': "*

 * *            "{'mod': OrderedDict([('type', 'string')])}}, 'portClass': {'properties': {'mod': "*

 * *            "OrderedDict([('type', 'string')])}, 'required': {insert: [(3, 'mod')]}}}",*

 * * "'id'": "'0-2-0/modulePackage.schema.json'"}*

```diff
@@ -42,14 +42,17 @@
             "properties": {
                 "desc": {
                     "type": "string"
                 },
                 "kwargs": {
                     "type": "object"
                 },
+                "mod": {
+                    "type": "string"
+                },
                 "name": {
                     "type": "string"
                 },
                 "pack": {
                     "type": "string"
                 },
                 "variables": {
@@ -58,20 +61,21 @@
                     },
                     "type": "array"
                 }
             },
             "required": [
                 "name",
                 "pack",
-                "variables"
+                "variables",
+                "mod"
             ]
         },
         "portVariable": {
             "additionalProperties": false,
-            "description": "Variable in ports",
+            "description": "Variable in a port",
             "properties": {
                 "desc": {
                     "type": "string"
                 },
                 "name": {
                     "type": "string"
                 },
@@ -91,14 +95,17 @@
                     "type": "string"
                 }
             },
             "properties": {
                 "desc": {
                     "type": "string"
                 },
+                "mod": {
+                    "type": "string"
+                },
                 "name": {
                     "type": "string"
                 },
                 "pack": {
                     "type": "string"
                 },
                 "variables": {
@@ -159,15 +166,15 @@
                 "mod"
             ]
         }
     },
     "$schema": "https://json-schema.org/draft/2020-12/schema",
     "additionalProperties": false,
     "description": "JSON of a package containing name, systems and ports",
-    "id": "0-1-0/modulePackage.schema.json",
+    "id": "0-2-0/modulePackage.schema.json",
     "properties": {
         "name": {
             "description": "Name of the package",
             "type": "string"
         },
         "ports": {
             "description": "List of port classes from the package",
```

### Comparing `cosapp-0.15.4/cosapp/tools/module_parser/parseModule.py` & `cosapp-0.16.0/cosapp/tools/module_parser/parseModule.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,15 @@
             portDict = {
                 'name': port.name,
                 'type': typename,
             }
         fixed_size_port = isinstance(port, Port)
         if fixed_size_port:
             portDict['pack'] = package_name or modname.split('.', maxsplit=1)[0]
+            portDict['mod'] = get_shortest_import_path(ptype.__module__, ptype)
         else:
             portDict['pack'] = sysPackage
         
         if not fixed_size_port or is_port_type:
             portDict['variables'] = get_port_var(port)
             desc = "\n".join(PortMarkdownFormatter(port).var_repr()[3:-1])
             if desc:
@@ -181,15 +182,15 @@
         if (unit := variable.unit):
             data['unit'] = unit
         return data
 
     def get_port_var(port: BasePort):
         return list(map(get_var_data, port.variables()))
 
-    def get_shortest_import_path(modulePath: str, dtype: Type[System]) -> str:
+    def get_shortest_import_path(modulePath: str, dtype: type) -> str:
         pathParts = modulePath.split('.')
         className = dtype.__name__
 
         upperModulePath = modulePath
         i = len(pathParts) -1
         while i > 0:
             currentPath = '.'.join(pathParts[:i])
```

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/problem_viewer.py` & `cosapp-0.16.0/cosapp/tools/problem_viewer/problem_viewer.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/tests/test_viewmodeldata.py` & `cosapp-0.16.0/cosapp/tools/problem_viewer/tests/test_viewmodeldata.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/index.html` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/index.html`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/libs/awesomplete.js` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/libs/awesomplete.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/libs/d3.v4.min.js` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/libs/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/libs/http.js` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/libs/http.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/libs/jquery-3.2.1.min.js` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/libs/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/libs/vkBeautify.js` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/libs/vkBeautify.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/constants.js` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/constants.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/draw.js` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/draw.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/legend.js` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/legend.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/modal.js` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/modal.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/ptN2.js` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/ptN2.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/search.js` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/search.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/src/svg.js` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/src/svg.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/style/awesomplete.css` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/style/awesomplete.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/style/fontello.woff` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/style/fontello.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/problem_viewer/visualization/style/partition_tree.css` & `cosapp-0.16.0/cosapp/tools/problem_viewer/visualization/style/partition_tree.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/templates/lib/d3.min.js` & `cosapp-0.16.0/cosapp/tools/templates/lib/d3.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/templates/lib/vis.min.css` & `cosapp-0.16.0/cosapp/tools/templates/lib/vis.min.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/templates/lib/vis.min.js` & `cosapp-0.16.0/cosapp/tools/templates/lib/vis.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/templates/pythonfmu.j2` & `cosapp-0.16.0/cosapp/tools/templates/pythonfmu.j2`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         # Set variables can be done before exit_initialization_mode call
         self.__master.call_setup_run()
 
         # Initialize the problem
         self.__driver._precompute()
         self.__driver.compute_before()
         self.__driver._initialize()
-        self.__driver._update_children()
+        self.__driver._update_system()
 
     def __restore(self):
         self.__driver._postcompute()
         self.__master.call_clean_run()
         self.__master.close_loops()
         System._System__master_set = False
         BasePort.set_type_checking(True)
```

### Comparing `cosapp-0.15.4/cosapp/tools/templates/src/d3_draw.js` & `cosapp-0.16.0/cosapp/tools/templates/src/d3_draw.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/templates/system_repr.html` & `cosapp-0.16.0/cosapp/tools/templates/system_repr.html`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/trigger.py` & `cosapp-0.16.0/cosapp/tools/trigger.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/views/baseRenderer.py` & `cosapp-0.16.0/cosapp/tools/views/baseRenderer.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/views/d3js.py` & `cosapp-0.16.0/cosapp/tools/views/d3js.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/views/markdown.py` & `cosapp-0.16.0/cosapp/tools/views/markdown.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/views/prettyprint.py` & `cosapp-0.16.0/cosapp/tools/views/prettyprint.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/views/tests/test_VisJsRenderer.py` & `cosapp-0.16.0/cosapp/tools/views/tests/test_VisJsRenderer.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/views/tests/test_d3.py` & `cosapp-0.16.0/cosapp/tools/views/tests/test_d3.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/views/tests/test_markdown.py` & `cosapp-0.16.0/cosapp/tools/views/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/views/tests/test_prettyprint.py` & `cosapp-0.16.0/cosapp/tools/views/tests/test_prettyprint.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tools/views/visjs.py` & `cosapp-0.16.0/cosapp/tools/views/visjs.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/00-Introduction.ipynb` & `cosapp-0.16.0/cosapp/tutorials/00-Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/01-Systems.ipynb` & `cosapp-0.16.0/cosapp/tutorials/01-Systems.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/02-Ports.ipynb` & `cosapp-0.16.0/cosapp/tutorials/02-Ports.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/03-Drivers.ipynb` & `cosapp-0.16.0/cosapp/tutorials/03-Drivers.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/04-Triggers.ipynb` & `cosapp-0.16.0/cosapp/tutorials/04-Triggers.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/05-Validation.ipynb` & `cosapp-0.16.0/cosapp/tutorials/05-Validation.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/06-Visibility.ipynb` & `cosapp-0.16.0/cosapp/tutorials/06-Visibility.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/07-Metamodels.ipynb` & `cosapp-0.16.0/cosapp/tutorials/07-Metamodels.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/08-Multipoints-Design.ipynb` & `cosapp-0.16.0/cosapp/tutorials/08-Multipoints-Design.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/09-MonteCarlo.ipynb` & `cosapp-0.16.0/cosapp/tutorials/09-MonteCarlo.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/10-Recorders.ipynb` & `cosapp-0.16.0/cosapp/tutorials/10-Recorders.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/11-DesignMethods.ipynb` & `cosapp-0.16.0/cosapp/tutorials/11-DesignMethods.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/CustomConnectors.ipynb` & `cosapp-0.16.0/cosapp/tutorials/CustomConnectors.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/FMI.ipynb` & `cosapp-0.16.0/cosapp/tutorials/FMI.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/Guidelines.ipynb` & `cosapp-0.16.0/cosapp/tutorials/Guidelines.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/HybridSimulations.ipynb` & `cosapp-0.16.0/cosapp/tutorials/HybridSimulations.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/Logging.ipynb` & `cosapp-0.16.0/cosapp/tutorials/Logging.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/Optimization.ipynb` & `cosapp-0.16.0/cosapp/tutorials/Optimization.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/SwapSystems.ipynb` & `cosapp-0.16.0/cosapp/tutorials/SwapSystems.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/SystemSurrogates.ipynb` & `cosapp-0.16.0/cosapp/tutorials/SystemSurrogates.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/SystemSurrogatesAdvanced.ipynb` & `cosapp-0.16.0/cosapp/tutorials/SystemSurrogatesAdvanced.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/Targets.ipynb` & `cosapp-0.16.0/cosapp/tutorials/Targets.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/TimeDriver.ipynb` & `cosapp-0.16.0/cosapp/tutorials/TimeDriver.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/TimeDriverAdvanced.ipynb` & `cosapp-0.16.0/cosapp/tutorials/TimeDriverAdvanced.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/TipsAndTricks.ipynb` & `cosapp-0.16.0/cosapp/tutorials/TipsAndTricks.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/Visitors.ipynb` & `cosapp-0.16.0/cosapp/tutorials/Visitors.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/aa-SimpleCircuit.ipynb` & `cosapp-0.16.0/cosapp/tutorials/aa-SimpleCircuit.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/exprampode_fmu.py` & `cosapp-0.16.0/cosapp/tutorials/exprampode_fmu.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/cosapp.svg` & `cosapp-0.16.0/cosapp/tutorials/images/cosapp.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/design_circuit.svg` & `cosapp-0.16.0/cosapp/tutorials/images/design_circuit.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/drivers_1.svg` & `cosapp-0.16.0/cosapp/tutorials/images/drivers_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/drivers_2.svg` & `cosapp-0.16.0/cosapp/tutorials/images/drivers_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/drivers_3.svg` & `cosapp-0.16.0/cosapp/tutorials/images/drivers_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/drivers_4.svg` & `cosapp-0.16.0/cosapp/tutorials/images/drivers_4.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/drivers_5.svg` & `cosapp-0.16.0/cosapp/tutorials/images/drivers_5.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/drivers_nonlinear.svg` & `cosapp-0.16.0/cosapp/tutorials/images/drivers_nonlinear.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/experimental.svg` & `cosapp-0.16.0/cosapp/tutorials/images/experimental.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/in_progress.svg` & `cosapp-0.16.0/cosapp/tutorials/images/in_progress.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/ports_1.svg` & `cosapp-0.16.0/cosapp/tutorials/images/ports_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/ports_2.svg` & `cosapp-0.16.0/cosapp/tutorials/images/ports_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/ports_3.svg` & `cosapp-0.16.0/cosapp/tutorials/images/ports_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/simple_circuit.svg` & `cosapp-0.16.0/cosapp/tutorials/images/simple_circuit.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/systems_1.svg` & `cosapp-0.16.0/cosapp/tutorials/images/systems_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/systems_2.svg` & `cosapp-0.16.0/cosapp/tutorials/images/systems_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/systems_3.svg` & `cosapp-0.16.0/cosapp/tutorials/images/systems_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/systems_4.svg` & `cosapp-0.16.0/cosapp/tutorials/images/systems_4.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/systems_5.svg` & `cosapp-0.16.0/cosapp/tutorials/images/systems_5.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/tanks.svg` & `cosapp-0.16.0/cosapp/tutorials/images/tanks.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/triggers_1.svg` & `cosapp-0.16.0/cosapp/tutorials/images/triggers_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/triggers_2.svg` & `cosapp-0.16.0/cosapp/tutorials/images/triggers_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/validity.svg` & `cosapp-0.16.0/cosapp/tutorials/images/validity.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/images/visibility.svg` & `cosapp-0.16.0/cosapp/tutorials/images/visibility.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/multimode/BouncingBall.ipynb` & `cosapp-0.16.0/cosapp/tutorials/multimode/BouncingBall.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/multimode/MultimodeOde.ipynb` & `cosapp-0.16.0/cosapp/tutorials/multimode/MultimodeOde.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/multimode/NewtonPendulum.ipynb` & `cosapp-0.16.0/cosapp/tutorials/multimode/NewtonPendulum.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/optimization/BetzLimit.ipynb` & `cosapp-0.16.0/cosapp/tutorials/optimization/BetzLimit.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/optimization/Sellar.ipynb` & `cosapp-0.16.0/cosapp/tutorials/optimization/Sellar.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/quickstart.ipynb` & `cosapp-0.16.0/cosapp/tutorials/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/tutorials/time_solutions.py` & `cosapp-0.16.0/cosapp/tutorials/time_solutions.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/distributions/distribution.py` & `cosapp-0.16.0/cosapp/utils/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/distributions/normal.py` & `cosapp-0.16.0/cosapp/utils/distributions/normal.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/distributions/tests/test_distribution.py` & `cosapp-0.16.0/cosapp/utils/distributions/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/distributions/tests/test_normal.py` & `cosapp-0.16.0/cosapp/utils/distributions/tests/test_normal.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/distributions/tests/test_triangular.py` & `cosapp-0.16.0/cosapp/utils/distributions/tests/test_triangular.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/distributions/tests/test_uniform.py` & `cosapp-0.16.0/cosapp/utils/distributions/tests/test_uniform.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/distributions/triangular.py` & `cosapp-0.16.0/cosapp/utils/distributions/triangular.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/distributions/uniform.py` & `cosapp-0.16.0/cosapp/utils/distributions/uniform.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/find_variables.py` & `cosapp-0.16.0/cosapp/utils/find_variables.py`

 * *Files 9% similar despite different names*

```diff
@@ -118,27 +118,14 @@
             and name == natural_varname(name)
         )
         if not valid:
             continue  # skip `name`
 
         ports.add(port)
         result.update(find_matches(name, ref.value))
-    
-    # Find matches among port properties
-    Port_cls_attr = get_attributes(Port)
-
-    for port in ports:
-        if not isinstance(port, Port):
-            continue  # exclude `inwards` and `outwards` extensible ports
-        port_properties = get_attributes(port) - Port_cls_attr - set(port._variables)
-        port_name = port.full_name(trim_root=True)
-        for name in port_properties:
-            result.update(
-                find_matches(f"{port_name}.{name}", getattr(port, name))
-            )
 
     # Find matches among system properties
     system_properties = find_system_properties(system, include_const)
     for name in system_properties:
         try:
             child, attr = name.rsplit('.', maxsplit=1)
         except ValueError:
```

### Comparing `cosapp-0.15.4/cosapp/utils/graph_analysis.py` & `cosapp-0.16.0/cosapp/utils/graph_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,28 +41,28 @@
             if not connector.is_active:
                 continue
             sink, source = connector.sink, connector.source
             if sink.is_output:
                 continue
             sink_name = get_portname(sink)
             if source.is_output:
-                bound_inputs |= set(
+                bound_inputs.update(
                     f"{sink_name}.{target}"
                     for target in connector.sink_variables()
                 )
             else:
                 source_name = get_portname(source)
                 inputs.update({
                     f"{sink_name}.{target}": f"{source_name}.{origin}"
                     for target, origin in connector.mapping.items()
                 })
 
         for child in system.children.values():
             child_inputs, child_bound_inputs = recursive_search(child, head)
-            bound_inputs |= child_bound_inputs
+            bound_inputs.update(child_bound_inputs)
             for key, alias in child_inputs.items():
                 try:
                     # Check if `ref` is already mapped in parent
                     inputs[key] = inputs[alias]
                 except KeyError:
                     inputs[key] = alias
```

### Comparing `cosapp-0.15.4/cosapp/utils/helpers.py` & `cosapp-0.16.0/cosapp/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/json.py` & `cosapp-0.16.0/cosapp/utils/json.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/logging.py` & `cosapp-0.16.0/cosapp/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/naming.py` & `cosapp-0.16.0/cosapp/utils/naming.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/options_dictionary.py` & `cosapp-0.16.0/cosapp/utils/options_dictionary.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/parsing.py` & `cosapp-0.16.0/cosapp/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/pull_variables.py` & `cosapp-0.16.0/cosapp/utils/pull_variables.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/state_io.py` & `cosapp-0.16.0/cosapp/utils/state_io.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/__init__.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/__init__.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/base.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/base.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/kriging.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/kriging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/multifi_cokriging.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/multifi_cokriging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/nearest_neighbor.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/nn_interpolators/linear_interpolator.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/nn_interpolators/linear_interpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/nn_interpolators/nn_base.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/nn_interpolators/nn_base.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/nn_interpolators/rbf_interpolator.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/nn_interpolators/rbf_interpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/nn_interpolators/weighted_interpolator.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/nn_interpolators/weighted_interpolator.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/response_surface.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/response_surface.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/tests/test_kriging.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/tests/test_kriging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/tests/test_multifi_cokriging.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/tests/test_multifi_cokriging.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/tests/test_nearest_neighbor.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/tests/test_nearest_neighbor.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/surrogate_models/tests/test_response_surface.py` & `cosapp-0.16.0/cosapp/utils/surrogate_models/tests/test_response_surface.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/swap_system.py` & `cosapp-0.16.0/cosapp/utils/swap_system.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/testing.py` & `cosapp-0.16.0/cosapp/utils/testing.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp/utils/validate.py` & `cosapp-0.16.0/cosapp/utils/validate.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/cosapp.egg-info/PKG-INFO` & `cosapp-0.16.0/cosapp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosapp
-Version: 0.15.4
+Version: 0.16.0
 Summary: CoSApp, the Collaborative System Approach.
 Home-page: https://cosapp.readthedocs.io
 Author: CoSApp Development Team
 License: Apache-2.0
 Keywords: cosapp,system simulation,system design
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: End Users/Desktop
@@ -68,23 +68,56 @@
 CoSApp solvers can be combined into versatile, customized workflows that fit specific simulation intents.
 
 Have a look at the [introduction](https://cosapp.readthedocs.io/en/stable/tutorials/00-Introduction.html#), containing many tutorials!
 
 This code is the property of Safran SA.
 It uses code coming from various open-source projects (see [LICENSE](https://gitlab.com/cosapp/cosapp/blob/master/LICENSE.rst) file).
 
+# Citing
+
+If you use CoSApp, please cite us!
+
+Lac *et al.* (2024), [CoSApp: a Python library to create, simulate and design complex systems](https://doi.org/10.21105/joss.06292), Journal of Open Source Software 9(94), 6292. 
+
+BibTeX entry:
+
+```bibtex
+@article{Lac.etal:joss2024, author={Étienne Lac and Guy {De Spiegeleer} and Adrien Delsalle and Frédéric Collonval and Duc-Trung Lê and Mathias Malandain}, title={CoSApp: a Python library to create, simulate and design complex systems}, journal={Journal of Open Source Software}, year={2024}, volume={9}, number={94}, pages={6292}, doi={10.21105/joss.06292}, publisher={The Open Journal}}
+```
+
 # Try it now!
 
 Run a Jupyter Lab instance with binder to try out CoSApp features through examples.
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gl/cosapp%2Fcosapp/master?urlpath=lab/tree/docs/tutorials)
 
 # History
 
 
+## 0.16.0 (2024-04-18)
+
+### Bug fixes and code quality
+
+- Primary events triggered within the same time step are now correctly captured (MR [#287](https://gitlab.com/cosapp/cosapp/-/merge_requests/287)).
+  A bug persists when several primary events occur at the exact same time, though, as only one will be retained.
+- Fix bug preventing events from occurring during the first time step of a simulation (MR [#288](https://gitlab.com/cosapp/cosapp/-/merge_requests/288)).
+- Fix a bug causing recorders to crash when inspecting ports with properties (MR [#282](https://gitlab.com/cosapp/cosapp/-/merge_requests/282)).
+- Algebraic and time-dependent problems are now dissociated (MR [#284](https://gitlab.com/cosapp/cosapp/-/merge_requests/284)). As a consequence, invoking `self.problem.clear()` during transitions, for instance, no longer affects time-dependent unknowns such as transients.
+- Fix ambiguous warning message raised by `RunSingleCase` (MR [#279](https://gitlab.com/cosapp/cosapp/-/merge_requests/279)).
+- Various refactoring passes (MRs [#283](https://gitlab.com/cosapp/cosapp/-/merge_requests/283) and [#286](https://gitlab.com/cosapp/cosapp/-/merge_requests/286)).
+
+### Maintenance
+
+- Updated description inside the conda recipe (MR [#276](https://gitlab.com/cosapp/cosapp/-/merge_requests/276)).
+- Pin `pytest` version due to a bug in version 8.1 (MR [#280](https://gitlab.com/cosapp/cosapp/-/merge_requests/280)).
+- Add a "Citing" section in the main README file (MR [#281](https://gitlab.com/cosapp/cosapp/-/merge_requests/281)).
+- The module parser was updated (MR [#285](https://gitlab.com/cosapp/cosapp/-/merge_requests/285)).
+- Force `sphinx` < 7.3 in the documentation building environment, owing to an incompatibility with `sphinx-mdinclude` (MR [#289](https://gitlab.com/cosapp/cosapp/-/merge_requests/289)). This is a temporary patch until root cause is fixed.
+
+
 ## 0.15.4 (2024-02-28)
 
 ### Bug fixes and code quality
 
 - Fix bug raised in `NonLinearSolver` for systems with rates (MR [#268](https://gitlab.com/cosapp/cosapp/-/merge_requests/268)).
 - Minor refactoring pass (MR [#274](https://gitlab.com/cosapp/cosapp/-/merge_requests/274)).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cosapp-0.15.4/cosapp.egg-info/SOURCES.txt` & `cosapp-0.16.0/cosapp.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 cosapp/core/numerics/basics.py
 cosapp/core/numerics/boundary.py
 cosapp/core/numerics/enum.py
 cosapp/core/numerics/mathematicalproblem.schema.json
 cosapp/core/numerics/residues.py
 cosapp/core/numerics/root.py
 cosapp/core/numerics/sobol_seq.py
+cosapp/core/numerics/utils.py
 cosapp/core/signal/__init__.py
 cosapp/core/signal/signal.py
 cosapp/core/signal/slot.py
 cosapp/core/tests/__init__.py
 cosapp/core/tests/conftest.py
 cosapp/core/tests/test_AssignString.py
 cosapp/core/tests/test_CoSAppConfiguration.py
```

### Comparing `cosapp-0.15.4/docs/Makefile` & `cosapp-0.16.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/conf.py` & `cosapp-0.16.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/layout.html` & `cosapp-0.16.0/docs/cosapp_theme/layout.html`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/searchbox.html` & `cosapp-0.16.0/docs/cosapp_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/cosapp.css_t` & `cosapp-0.16.0/docs/cosapp_theme/static/cosapp.css_t`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/css/custom.css` & `cosapp-0.16.0/docs/cosapp_theme/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/css/font-awesome.min.css` & `cosapp-0.16.0/docs/cosapp_theme/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/css/font.css` & `cosapp-0.16.0/docs/cosapp_theme/static/css/font.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/css/highlight.css` & `cosapp-0.16.0/docs/cosapp_theme/static/css/highlight.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/css/kube.css` & `cosapp-0.16.0/docs/cosapp_theme/static/css/kube.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/css/kube.demo.css` & `cosapp-0.16.0/docs/cosapp_theme/static/css/kube.demo.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/css/kube.legenda.css` & `cosapp-0.16.0/docs/cosapp_theme/static/css/kube.legenda.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/css/kube.min.css` & `cosapp-0.16.0/docs/cosapp_theme/static/css/kube.min.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/css/master.css` & `cosapp-0.16.0/docs/cosapp_theme/static/css/master.css`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/font/Lato-Black.woff` & `cosapp-0.16.0/docs/cosapp_theme/static/font/Lato-Black.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/font/Lato-Bold.woff` & `cosapp-0.16.0/docs/cosapp_theme/static/font/Lato-Bold.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/font/Lato-BoldItalic.woff` & `cosapp-0.16.0/docs/cosapp_theme/static/font/Lato-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/font/Lato-Italic.woff` & `cosapp-0.16.0/docs/cosapp_theme/static/font/Lato-Italic.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/font/Lato-Regular.woff` & `cosapp-0.16.0/docs/cosapp_theme/static/font/Lato-Regular.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/font/Lato-Semibold.woff` & `cosapp-0.16.0/docs/cosapp_theme/static/font/Lato-Semibold.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/fonts/fontawesome-webfont.woff` & `cosapp-0.16.0/docs/cosapp_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/img/cosapp.svg` & `cosapp-0.16.0/docs/cosapp_theme/static/img/cosapp.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/js/jquery-2.1.4.min.js` & `cosapp-0.16.0/docs/cosapp_theme/static/js/jquery-2.1.4.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/js/kube.js` & `cosapp-0.16.0/docs/cosapp_theme/static/js/kube.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/js/kube.min.js` & `cosapp-0.16.0/docs/cosapp_theme/static/js/kube.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/js/tocbot.min.js` & `cosapp-0.16.0/docs/cosapp_theme/static/js/tocbot.min.js`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/static/sidebar.js_t` & `cosapp-0.16.0/docs/cosapp_theme/static/sidebar.js_t`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/cosapp_theme/theme.conf` & `cosapp-0.16.0/docs/cosapp_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/developer/installation_cases.rst` & `cosapp-0.16.0/docs/developer/installation_cases.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/developer/logger.rst` & `cosapp-0.16.0/docs/developer/logger.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/developer/project_structure.rst` & `cosapp-0.16.0/docs/developer/project_structure.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/developer/scenarii.rst` & `cosapp-0.16.0/docs/developer/scenarii.rst`

 * *Files 0% similar despite different names*

```diff
@@ -303,25 +303,25 @@
       solver->>solver: _precompute()
          Note right of solver: Solve children drivers
       solver->>+solver: compute()
          solver->>+solver: _initialize()
             solver->>+solver: _set_time(start_time)
             solver->>clock: time = t
             solver->>solver: Update boundary conditions
-            solver->>solver: _update_children()
+            solver->>solver: _update_system()
                Note right of solver: Solve children drivers
             solver->>solver: _update_rates()
          deactivate solver
          solver->>solver: Update initial conditions
          deactivate solver
          loop on Time
             solver->>+solver: _set_time(time)
                solver->>clock: time = t
                solver->>solver: Update boundary conditions
-               solver->>solver: _update_children()
+               solver->>solver: _update_system()
                   Note right of solver: Solve children drivers
                solver->>solver: _update_rates()
             deactivate solver
             solver->>solver: Get new time step
             solver->>solver: _update_transients(dt)
                Note right of solver: Time integration
          end
```

### Comparing `cosapp-0.15.4/docs/img/gitlab-cosapp-f4950f.svg` & `cosapp-0.16.0/docs/img/gitlab-cosapp-f4950f.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/img/website-docs-blue.svg` & `cosapp-0.16.0/docs/img/website-docs-blue.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/index.rst` & `cosapp-0.16.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/installation.rst` & `cosapp-0.16.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/make.bat` & `cosapp-0.16.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/nb_thumbnails/_images/verified.svg` & `cosapp-0.16.0/docs/nb_thumbnails/_images/verified.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/source/modules.rst` & `cosapp-0.16.0/docs/source/modules.rst`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tools/mermaid.py` & `cosapp-0.16.0/docs/tools/mermaid.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tools/mermaid_inheritance.py` & `cosapp-0.16.0/docs/tools/mermaid_inheritance.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/00-Introduction.ipynb` & `cosapp-0.16.0/docs/tutorials/00-Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/01-Systems.ipynb` & `cosapp-0.16.0/docs/tutorials/01-Systems.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/02-Ports.ipynb` & `cosapp-0.16.0/docs/tutorials/02-Ports.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/03-Drivers.ipynb` & `cosapp-0.16.0/docs/tutorials/03-Drivers.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/04-Triggers.ipynb` & `cosapp-0.16.0/docs/tutorials/04-Triggers.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/05-Validation.ipynb` & `cosapp-0.16.0/docs/tutorials/05-Validation.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/06-Visibility.ipynb` & `cosapp-0.16.0/docs/tutorials/06-Visibility.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/07-Metamodels.ipynb` & `cosapp-0.16.0/docs/tutorials/07-Metamodels.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/08-Multipoints-Design.ipynb` & `cosapp-0.16.0/docs/tutorials/08-Multipoints-Design.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/09-MonteCarlo.ipynb` & `cosapp-0.16.0/docs/tutorials/09-MonteCarlo.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/10-Recorders.ipynb` & `cosapp-0.16.0/docs/tutorials/10-Recorders.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/11-DesignMethods.ipynb` & `cosapp-0.16.0/docs/tutorials/11-DesignMethods.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/CustomConnectors.ipynb` & `cosapp-0.16.0/docs/tutorials/CustomConnectors.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/FMI.ipynb` & `cosapp-0.16.0/docs/tutorials/FMI.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/Guidelines.ipynb` & `cosapp-0.16.0/docs/tutorials/Guidelines.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/HybridSimulations.ipynb` & `cosapp-0.16.0/docs/tutorials/HybridSimulations.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/Logging.ipynb` & `cosapp-0.16.0/docs/tutorials/Logging.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/Optimization.ipynb` & `cosapp-0.16.0/docs/tutorials/Optimization.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/SwapSystems.ipynb` & `cosapp-0.16.0/docs/tutorials/SwapSystems.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/SystemSurrogates.ipynb` & `cosapp-0.16.0/docs/tutorials/SystemSurrogates.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/SystemSurrogatesAdvanced.ipynb` & `cosapp-0.16.0/docs/tutorials/SystemSurrogatesAdvanced.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/Targets.ipynb` & `cosapp-0.16.0/docs/tutorials/Targets.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/TimeDriver.ipynb` & `cosapp-0.16.0/docs/tutorials/TimeDriver.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/TimeDriverAdvanced.ipynb` & `cosapp-0.16.0/docs/tutorials/TimeDriverAdvanced.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/TipsAndTricks.ipynb` & `cosapp-0.16.0/docs/tutorials/TipsAndTricks.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/Visitors.ipynb` & `cosapp-0.16.0/docs/tutorials/Visitors.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/aa-SimpleCircuit.ipynb` & `cosapp-0.16.0/docs/tutorials/aa-SimpleCircuit.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/exprampode_fmu.py` & `cosapp-0.16.0/docs/tutorials/exprampode_fmu.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/Moise_tables_loi.jpg` & `cosapp-0.16.0/docs/tutorials/images/Moise_tables_loi.jpg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/cosapp.svg` & `cosapp-0.16.0/docs/tutorials/images/cosapp.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/design_circuit.svg` & `cosapp-0.16.0/docs/tutorials/images/design_circuit.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/drivers_1.svg` & `cosapp-0.16.0/docs/tutorials/images/drivers_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/drivers_2.svg` & `cosapp-0.16.0/docs/tutorials/images/drivers_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/drivers_3.svg` & `cosapp-0.16.0/docs/tutorials/images/drivers_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/drivers_4.svg` & `cosapp-0.16.0/docs/tutorials/images/drivers_4.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/drivers_5.svg` & `cosapp-0.16.0/docs/tutorials/images/drivers_5.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/drivers_nonlinear.svg` & `cosapp-0.16.0/docs/tutorials/images/drivers_nonlinear.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/experimental.svg` & `cosapp-0.16.0/docs/tutorials/images/experimental.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/in_progress.svg` & `cosapp-0.16.0/docs/tutorials/images/in_progress.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/ports_1.svg` & `cosapp-0.16.0/docs/tutorials/images/ports_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/ports_2.svg` & `cosapp-0.16.0/docs/tutorials/images/ports_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/ports_3.svg` & `cosapp-0.16.0/docs/tutorials/images/ports_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/simple_circuit.svg` & `cosapp-0.16.0/docs/tutorials/images/simple_circuit.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/systems_1.svg` & `cosapp-0.16.0/docs/tutorials/images/systems_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/systems_2.svg` & `cosapp-0.16.0/docs/tutorials/images/systems_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/systems_3.svg` & `cosapp-0.16.0/docs/tutorials/images/systems_3.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/systems_4.svg` & `cosapp-0.16.0/docs/tutorials/images/systems_4.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/systems_5.svg` & `cosapp-0.16.0/docs/tutorials/images/systems_5.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/tanks.svg` & `cosapp-0.16.0/docs/tutorials/images/tanks.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/triggers_1.svg` & `cosapp-0.16.0/docs/tutorials/images/triggers_1.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/triggers_2.svg` & `cosapp-0.16.0/docs/tutorials/images/triggers_2.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/validity.svg` & `cosapp-0.16.0/docs/tutorials/images/validity.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/images/visibility.svg` & `cosapp-0.16.0/docs/tutorials/images/visibility.svg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/multimode/BouncingBall.ipynb` & `cosapp-0.16.0/docs/tutorials/multimode/BouncingBall.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/multimode/MultimodeOde.ipynb` & `cosapp-0.16.0/docs/tutorials/multimode/MultimodeOde.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/multimode/NewtonPendulum.ipynb` & `cosapp-0.16.0/docs/tutorials/multimode/NewtonPendulum.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/optimization/BetzLimit.ipynb` & `cosapp-0.16.0/docs/tutorials/optimization/BetzLimit.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/optimization/Sellar.ipynb` & `cosapp-0.16.0/docs/tutorials/optimization/Sellar.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/quickstart.ipynb` & `cosapp-0.16.0/docs/tutorials/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/docs/tutorials/time_solutions.py` & `cosapp-0.16.0/docs/tutorials/time_solutions.py`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/setup.cfg` & `cosapp-0.16.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `cosapp-0.15.4/setup.py` & `cosapp-0.16.0/setup.py`

 * *Files identical despite different names*

