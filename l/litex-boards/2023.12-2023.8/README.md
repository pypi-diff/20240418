# Comparing `tmp/litex-boards-2023.12.tar.gz` & `tmp/litex-boards-2023.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litex-boards-2023.12.tar", last modified: Thu Apr 18 20:14:54 2024, max compression
+gzip compressed data, was "litex-boards-2023.8.tar", last modified: Sun Sep 17 21:47:25 2023, max compression
```

## Comparing `litex-boards-2023.12.tar` & `litex-boards-2023.8.tar`

### file list

```diff
@@ -1,357 +1,346 @@
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:14:54.584445 litex-boards-2023.12/
--rw-r--r--   0 timkpaine   (501) staff       (20)     1395 2024-04-18 20:14:26.000000 litex-boards-2023.12/LICENSE
--rw-r--r--   0 timkpaine   (501) staff       (20)    11393 2024-04-18 20:14:54.584157 litex-boards-2023.12/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)    11027 2024-04-18 20:14:50.000000 litex-boards-2023.12/README.md
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:14:54.508387 litex-boards-2023.12/litex_boards/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/__init__.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:14:54.549807 litex-boards-2023.12/litex_boards/platforms/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/__init__.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    17917 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/adi_adrv2crr_fmc.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1123 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/adi_plutosdr.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5068 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/alchitry_au.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2579 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/alchitry_cu.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4422 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/alchitry_mojo.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3155 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/aliexpress_xc7k420t.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7899 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/aliexpress_xc7k70t.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3532 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/alinx_ax7010.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6428 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/alinx_axu2cga.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8583 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/analog_pocket.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5519 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/antmicro_artix_dc_scm.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6890 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/antmicro_datacenter_ddr4_test_board.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4505 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/antmicro_lpddr4_test_board.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7091 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/antmicro_sdi_mipi_video_converter.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8990 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/arduino_mkrvidor4000.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3965 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/avalanche.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7721 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/avnet_aesku40.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    12075 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/berkeleylab_marble.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     9072 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/berkeleylab_marblemini.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2729 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/camlink_4k.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    11778 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/colorlight_5a_75b.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     9198 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/colorlight_5a_75e.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7866 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/colorlight_i5.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5720 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/colorlight_i5a_907.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5974 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/colorlight_i9plus.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2089 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/decklink_intensity_pro_4k.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5577 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/decklink_mini_4k.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7379 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/decklink_quad_hdmi_recorder.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    12363 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/digilent_arty.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7582 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/digilent_arty_s7.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     9535 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/digilent_arty_z7.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8995 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/digilent_atlys.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5607 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/digilent_basys3.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3207 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/digilent_cmod_a7.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6700 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/digilent_genesys2.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     9019 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/digilent_nexys4.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7942 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/digilent_nexys4ddr.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    11373 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/digilent_nexys_video.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7255 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/digilent_pynq_z1.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7176 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/digilent_zedboard.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6266 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/digilent_zybo_z7.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2660 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/ebaz4205.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2747 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/efinix_t8f81_dev_kit.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7588 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/efinix_titanium_ti60_f225_dev_kit.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8142 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/efinix_trion_t120_bga576_dev_kit.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4971 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/efinix_trion_t20_bga256_dev_kit.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2586 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/efinix_trion_t20_mipi_dev_kit.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3166 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/efinix_xyloni_dev_kit.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6309 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/ego1.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    11324 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/enclustra_mercury_kx2.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4614 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/enclustra_mercury_xu5.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    14280 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/enclustra_mercury_xu8_pe3.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    10242 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/enclustra_st1.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6085 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/fairwaves_xtrx.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6247 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/fpc_iii.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2591 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/fpgawars_alhambra2.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5091 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/gadgetfactory_papilio_pro.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8772 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/gsd_butterstick.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8819 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/gsd_orangecrab.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8596 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/hackaday_hadbadge.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2857 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/ice_v_wireless.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5347 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/icebreaker.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4690 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/icebreaker_bitsy.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5194 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/isx_im1283.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2238 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/jungle_electronics_fireant.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3138 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/kosagi_fomu_evt.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2563 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/kosagi_fomu_hacker.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2744 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/kosagi_fomu_pvt.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8746 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/kosagi_netv2.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3765 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/krtkl_snickerdoodle.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6452 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/lambdaconcept_ecpix5.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4065 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/lambdaconcept_pcie_screamer.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3110 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/lambdaconcept_pcie_screamer_m2.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    15127 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/lattice_crosslink_nx_evn.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    13568 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/lattice_crosslink_nx_vip.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5749 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/lattice_ecp5_evn.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5976 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/lattice_ecp5_vip.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4607 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/lattice_ice40up5k_evn.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3911 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/lattice_machxo3.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8601 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/lattice_versa_ecp5.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4358 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/limesdr_mini_v2.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8757 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/linsn_rv901t.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4672 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/litex_acorn_baseboard.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7751 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/logicbone.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4415 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/machdyne_konfekt.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5027 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/machdyne_kopflos.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2089 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/machdyne_krote.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4184 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/machdyne_mozart_ml1.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5006 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/machdyne_noir.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4813 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/machdyne_schoko.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    12075 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/marble.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     9072 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/marblemini.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2107 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/micronova_mercury2.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4284 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/mist.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7709 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/mnt_rkx7.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3825 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/muselab_icesugar.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5000 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/muselab_icesugar_pro.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4239 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/myminieye_runber.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2091 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/newae_cw305.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4936 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/numato_aller.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8545 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/numato_mimas_a7.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    11980 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/numato_nereid.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6145 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/numato_tagus.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8641 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/ocp_tap_timecard.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6312 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/opalkelly_xem8320.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5552 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/pano_logic_g2.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5476 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/qmtech_10cl006.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5384 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/qmtech_5cefa2.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5652 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/qmtech_5cefa5.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6860 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/qmtech_artix7_fbg484.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7166 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/qmtech_artix7_fgg676.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5895 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/qmtech_daughterboard.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5087 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/qmtech_ep4ce15_starter_kit.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5264 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/qmtech_ep4cex5.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5300 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/qmtech_ep4cgx150.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5971 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/qmtech_rp2040_daughterboard.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8725 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/qmtech_wukong.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6485 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/qmtech_xc7a35t.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6640 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/qmtech_xc7k325t.py
--rw-r--r--   0 timkpaine   (501) staff       (20)      904 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/quicklogic_quickfeather.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2836 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/qwertyembedded_beaglewire.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     8340 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/radiona_ulx3s.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6628 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/radiona_ulx4m_ld_v2.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     9345 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/rcs_arctic_tern_bmc_card.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5505 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/redpitaya.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2108 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/rz_easyfpga.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6097 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/saanlima_pipistrello.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6323 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/scarabhardware_minispartan6.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3649 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/seeedstudio_spartan_edge_accelerator.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4839 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/siglent_sds1104xe.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    12110 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/sipeed_tang_mega_138k.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2009 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/sipeed_tang_nano.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3678 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/sipeed_tang_nano_20k.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3706 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/sipeed_tang_nano_4k.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3695 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/sipeed_tang_nano_9k.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1905 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/sipeed_tang_primer.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    11440 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/sipeed_tang_primer_20k.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5654 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/sipeed_tang_primer_25k.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1880 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/sitlinv_a_e115fb.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    18361 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/sitlinv_stlv7325_v1.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    19009 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/sitlinv_stlv7325_v2.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    15103 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/sitlinv_xc7k420t.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6679 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/sqrl_acorn.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3990 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/sqrl_fk33.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    14992 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/sqrl_xcu1525.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5015 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/terasic_de0nano.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5560 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/terasic_de10lite.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6363 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/terasic_de10nano.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5964 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/terasic_de1soc.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4837 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/terasic_de2_115.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    14493 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/terasic_deca.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7962 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/terasic_sockit.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2583 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/tinyfpga_bx.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    11196 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/trellisboard.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4787 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/trenz_c10lprefkit.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     2906 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/trenz_cyc1000.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4043 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/trenz_max1000.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3638 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/trenz_te0725.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     4765 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/trenz_tec0117.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     3248 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/tul_pynq_z2.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     9257 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_ac701.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    16681 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_alveo_u200.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    16629 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_alveo_u250.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    12333 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_alveo_u280.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    19654 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_kc705.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    18771 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_kcu105.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1495 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_kv260.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5827 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_sp605.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    23087 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_vc707.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     9582 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_vcu118.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     6568 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_vcu128.py
--rw-r--r--   0 timkpaine   (501) staff       (20)    12596 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_zcu102.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5395 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_zcu104.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     5906 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_zcu106.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     1819 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/xilinx_zcu216.py
--rw-r--r--   0 timkpaine   (501) staff       (20)     7666 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/platforms/ztex213.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:14:54.583312 litex-boards-2023.12/litex_boards/targets/
--rw-r--r--   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/__init__.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5861 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/adi_adrv2crr_fmc.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3227 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/adi_plutosdr.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4879 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/alchitry_au.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4767 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/alchitry_cu.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7968 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/alchitry_mojo.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3357 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/aliexpress_xc7k420t.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7325 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/aliexpress_xc7k70t.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     2944 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/alinx_ax7010.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7618 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/alinx_axu2cga.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7493 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/analog_pocket.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7310 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/antmicro_artix_dc_scm.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    11498 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/antmicro_datacenter_ddr4_test_board.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6964 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/antmicro_lpddr4_test_board.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5225 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/antmicro_sdi_mipi_video_converter.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3196 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/arduino_mkrvidor4000.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5410 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/avnet_aesku40.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7029 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/berkeleylab_marble.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4548 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/camlink_4k.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    12390 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/colorlight_5a_75x.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    10771 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/colorlight_i5.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8195 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/colorlight_i9plus.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3444 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/decklink_intensity_pro_4k.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8214 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/decklink_mini_4k.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5534 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/decklink_quad_hdmi_recorder.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9571 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/digilent_arty.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4685 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/digilent_arty_s7.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8056 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/digilent_arty_z7.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9506 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/digilent_atlys.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4195 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/digilent_basys3.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6320 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/digilent_cmod_a7.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4984 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/digilent_genesys2.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9859 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/digilent_nexys4.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6486 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/digilent_nexys4ddr.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9282 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/digilent_nexys_video.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5190 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/digilent_pynq_z1.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6851 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/digilent_zedboard.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3185 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/ebaz4205.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4521 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/efinix_t8f81_dev_kit.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6978 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/efinix_titanium_ti60_f225_dev_kit.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    24244 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/efinix_trion_t120_bga576_dev_kit.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3877 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/efinix_trion_t20_bga256_dev_kit.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3405 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/efinix_trion_t20_mipi_dev_kit.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4433 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/efinix_xyloni_dev_kit.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3534 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/ego1.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4016 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/enclustra_mercury_kx2.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4000 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/enclustra_mercury_xu5.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5129 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/fairwaves_xtrx.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6409 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/fpc_iii.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3334 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/fpgawars_alhambra2.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4804 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/gadgetfactory_papilio_pro.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9092 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/gsd_butterstick.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8994 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/gsd_orangecrab.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3390 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/hackaday_hadbadge.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7667 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/ice_v_wireless.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7171 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/icebreaker.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7801 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/icebreaker_bitsy.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4382 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/isx_im1283.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4919 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/jungle_electronics_fireant.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7323 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/kosagi_fomu.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5977 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/kosagi_netv2.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5470 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/krtkl_snickerdoodle.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    10545 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/lambdaconcept_ecpix5.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6111 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/lattice_crosslink_nx_evn.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5184 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/lattice_crosslink_nx_vip.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3346 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/lattice_ecp5_evn.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8410 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/lattice_ecp5_vip.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5785 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/lattice_ice40up5k_evn.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6307 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/lattice_versa_ecp5.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5999 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/limesdr_mini_v2.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4922 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/linsn_rv901t.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7543 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/litex_acorn_baseboard.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6713 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/logicbone.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9381 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/machdyne_konfekt.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9239 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/machdyne_kopflos.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4797 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/machdyne_krote.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9186 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/machdyne_mozart_ml1.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9479 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/machdyne_noir.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8981 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/machdyne_schoko.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5594 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/micronova_mercury2.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4178 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/mist.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    10738 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/mnt_rkx7.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5471 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/muselab_icesugar.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9135 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/muselab_icesugar_pro.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3016 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/myminieye_runber.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3415 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/newae_cw305.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4857 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/numato_aller.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4407 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/numato_mimas_a7.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4319 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/numato_nereid.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4763 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/numato_tagus.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9948 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/ocp_tap_timecard.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7172 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/opalkelly_xem8320.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4721 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/pano_logic_g2.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5853 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/qmtech_10cl006.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8425 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/qmtech_5cefa2.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8365 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/qmtech_5cefa5.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9169 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/qmtech_artix7_fbg484.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9161 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/qmtech_artix7_fgg676.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4657 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/qmtech_ep4ce15_starter_kit.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8299 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/qmtech_ep4cex5.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8117 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/qmtech_ep4cgx150.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8404 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/qmtech_wukong.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8880 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/qmtech_xc7a35t.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    11713 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/qmtech_xc7k325t.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4501 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/quicklogic_quickfeather.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5035 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/qwertyembedded_beaglewire.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8901 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/radiona_ulx3s.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    10672 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/radiona_ulx4m_ld_v2.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7882 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/rcs_arctic_tern_bmc_card.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4804 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/redpitaya.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4487 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/rz_easyfpga.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8425 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/saanlima_pipistrello.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5851 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/scarabhardware_minispartan6.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4951 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/seeedstudio_spartan_edge_accelerator.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6800 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/siglent_sds1104xe.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     2792 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/simple.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    11535 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/sipeed_tang_mega_138k.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4138 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/sipeed_tang_nano.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6128 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/sipeed_tang_nano_20k.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7759 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/sipeed_tang_nano_4k.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7643 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/sipeed_tang_nano_9k.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3099 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/sipeed_tang_primer.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    10389 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/sipeed_tang_primer_20k.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4041 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/sipeed_tang_primer_25k.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     2745 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/sitlinv_a_e115fb.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    11025 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/sitlinv_stlv7325_v1.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9587 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/sitlinv_stlv7325_v2.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7032 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/sitlinv_xc7k420t.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8651 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/sqrl_acorn.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6996 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/sqrl_fk33.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6862 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/sqrl_xcu1525.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4420 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/terasic_de0nano.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4251 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/terasic_de10lite.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5444 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/terasic_de10nano.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3499 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/terasic_de1soc.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6438 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/terasic_de2_115.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7279 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/terasic_deca.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6433 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/terasic_sockit.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3018 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/tinyfpga_bx.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8734 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/trellisboard.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4987 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/trenz_c10lprefkit.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3400 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/trenz_cyc1000.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3475 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/trenz_max1000.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3324 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/trenz_te0725.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7805 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/trenz_tec0117.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     3458 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/tul_pynq_z2.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7643 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_ac701.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5257 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_alveo_u200.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     5204 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_alveo_u250.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8708 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_alveo_u280.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7350 2024-04-18 20:14:50.000000 litex-boards-2023.12/litex_boards/targets/xilinx_kc705.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     7924 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_kcu105.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)    10175 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_kv260.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4496 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_vc707.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4101 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_vcu118.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     6101 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_vcu128.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4023 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_zcu102.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4106 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_zcu104.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4727 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_zcu106.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     9451 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_zcu216.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     8981 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/xilinx_zybo_z7.py
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     4914 2024-04-18 20:14:26.000000 litex-boards-2023.12/litex_boards/targets/ztex213.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:14:54.583802 litex-boards-2023.12/litex_boards.egg-info/
--rw-r--r--   0 timkpaine   (501) staff       (20)    11393 2024-04-18 20:14:54.000000 litex-boards-2023.12/litex_boards.egg-info/PKG-INFO
--rw-r--r--   0 timkpaine   (501) staff       (20)    14642 2024-04-18 20:14:54.000000 litex-boards-2023.12/litex_boards.egg-info/SOURCES.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        1 2024-04-18 20:14:54.000000 litex-boards-2023.12/litex_boards.egg-info/dependency_links.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)        6 2024-04-18 20:14:54.000000 litex-boards-2023.12/litex_boards.egg-info/requires.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       13 2024-04-18 20:14:54.000000 litex-boards-2023.12/litex_boards.egg-info/top_level.txt
--rw-r--r--   0 timkpaine   (501) staff       (20)       38 2024-04-18 20:14:54.584495 litex-boards-2023.12/setup.cfg
--rwxr-xr-x   0 timkpaine   (501) staff       (20)     1013 2024-04-18 20:14:50.000000 litex-boards-2023.12/setup.py
-drwxr-xr-x   0 timkpaine   (501) staff       (20)        0 2024-04-18 20:14:54.583585 litex-boards-2023.12/test/
--rw-r--r--   0 timkpaine   (501) staff       (20)     3921 2024-04-18 20:14:50.000000 litex-boards-2023.12/test/test_targets.py
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:47:25.957851 litex-boards-2023.8/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     1395 2023-09-17 21:44:27.000000 litex-boards-2023.8/LICENSE
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    11203 2023-09-17 21:47:25.957851 litex-boards-2023.8/PKG-INFO
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    10859 2023-09-17 21:45:26.000000 litex-boards-2023.8/README.md
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:47:25.921850 litex-boards-2023.8/litex_boards/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/__init__.py
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:47:25.937850 litex-boards-2023.8/litex_boards/platforms/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/__init__.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    17917 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/adi_adrv2crr_fmc.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     1123 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/adi_plutosdr.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5068 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/alchitry_au.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2579 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/alchitry_cu.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4422 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/alchitry_mojo.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3155 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/aliexpress_xc7k420t.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3532 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/alinx_ax7010.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6428 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/alinx_axu2cga.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5519 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/antmicro_artix_dc_scm.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6890 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/antmicro_datacenter_ddr4_test_board.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4505 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/antmicro_lpddr4_test_board.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7091 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/antmicro_sdi_mipi_video_converter.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8990 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/arduino_mkrvidor4000.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3965 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/avalanche.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7721 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/avnet_aesku40.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    12075 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/berkeleylab_marble.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9072 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/berkeleylab_marblemini.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2729 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/camlink_4k.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    11778 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/colorlight_5a_75b.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9198 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/colorlight_5a_75e.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7866 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/colorlight_i5.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5720 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/colorlight_i5a_907.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5974 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/colorlight_i9plus.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2089 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/decklink_intensity_pro_4k.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5577 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/decklink_mini_4k.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7379 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/decklink_quad_hdmi_recorder.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    12363 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/digilent_arty.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7582 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/digilent_arty_s7.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9535 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/digilent_arty_z7.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8995 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/digilent_atlys.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5607 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/digilent_basys3.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3207 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/digilent_cmod_a7.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6700 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/digilent_genesys2.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9019 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/digilent_nexys4.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7942 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/digilent_nexys4ddr.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    11373 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/digilent_nexys_video.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7255 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/digilent_pynq_z1.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7176 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/digilent_zedboard.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6266 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/digilent_zybo_z7.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2660 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/ebaz4205.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2747 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/efinix_t8f81_dev_kit.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7588 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/efinix_titanium_ti60_f225_dev_kit.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6782 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/efinix_trion_t120_bga576_dev_kit.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4373 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/efinix_trion_t20_bga256_dev_kit.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2586 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/efinix_trion_t20_mipi_dev_kit.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3166 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/efinix_xyloni_dev_kit.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6309 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/ego1.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    11324 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/enclustra_mercury_kx2.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4614 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/enclustra_mercury_xu5.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    14280 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/enclustra_mercury_xu8_pe3.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    10242 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/enclustra_st1.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6085 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/fairwaves_xtrx.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6247 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/fpc_iii.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2591 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/fpgawars_alhambra2.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5091 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/gadgetfactory_papilio_pro.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8772 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/gsd_butterstick.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8819 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/gsd_orangecrab.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8596 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/hackaday_hadbadge.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2857 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/ice_v_wireless.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5347 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/icebreaker.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4690 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/icebreaker_bitsy.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5194 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/isx_im1283.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2238 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/jungle_electronics_fireant.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3138 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/kosagi_fomu_evt.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2563 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/kosagi_fomu_hacker.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2744 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/kosagi_fomu_pvt.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8746 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/kosagi_netv2.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3765 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/krtkl_snickerdoodle.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6452 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/lambdaconcept_ecpix5.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4065 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/lambdaconcept_pcie_screamer.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3110 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/lambdaconcept_pcie_screamer_m2.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    15127 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/lattice_crosslink_nx_evn.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    13568 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/lattice_crosslink_nx_vip.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5749 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/lattice_ecp5_evn.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5976 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/lattice_ecp5_vip.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4607 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/lattice_ice40up5k_evn.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3911 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/lattice_machxo3.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8601 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/lattice_versa_ecp5.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4358 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/limesdr_mini_v2.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8757 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/linsn_rv901t.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4672 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/litex_acorn_baseboard.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7751 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/logicbone.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4415 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/machdyne_konfekt.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5027 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/machdyne_kopflos.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2089 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/machdyne_krote.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5006 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/machdyne_noir.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4813 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/machdyne_schoko.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    12075 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/marble.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9072 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/marblemini.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2107 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/micronova_mercury2.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4284 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/mist.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7709 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/mnt_rkx7.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3825 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/muselab_icesugar.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5000 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/muselab_icesugar_pro.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4239 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/myminieye_runber.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2091 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/newae_cw305.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4936 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/numato_aller.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8545 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/numato_mimas_a7.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    11980 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/numato_nereid.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6145 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/numato_tagus.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8355 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/ocp_tap_timecard.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6312 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/opalkelly_xem8320.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5552 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/pano_logic_g2.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5476 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/qmtech_10cl006.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5384 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/qmtech_5cefa2.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5652 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/qmtech_5cefa5.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6905 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/qmtech_artix7_fbg484.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6885 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/qmtech_artix7_fgg676.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5895 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/qmtech_daughterboard.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5087 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/qmtech_ep4ce15_starter_kit.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5264 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/qmtech_ep4cex5.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5300 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/qmtech_ep4cgx150.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8724 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/qmtech_wukong.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6529 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/qmtech_xc7a35t.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6319 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/qmtech_xc7k325t.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)      904 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/quicklogic_quickfeather.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2836 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/qwertyembedded_beaglewire.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     8340 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/radiona_ulx3s.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6628 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/radiona_ulx4m_ld_v2.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9345 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/rcs_arctic_tern_bmc_card.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5505 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/redpitaya.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2108 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/rz_easyfpga.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6097 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/saanlima_pipistrello.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6323 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/scarabhardware_minispartan6.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3649 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/seeedstudio_spartan_edge_accelerator.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4839 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/siglent_sds1104xe.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2009 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/sipeed_tang_nano.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3678 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/sipeed_tang_nano_20k.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3706 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/sipeed_tang_nano_4k.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3695 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/sipeed_tang_nano_9k.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     1905 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/sipeed_tang_primer.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    11440 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/sipeed_tang_primer_20k.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     1880 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/sitlinv_a_e115fb.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    18361 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/sitlinv_stlv7325_v1.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    19009 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/sitlinv_stlv7325_v2.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    15103 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/sitlinv_xc7k420t.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6679 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/sqrl_acorn.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3990 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/sqrl_fk33.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    14992 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/sqrl_xcu1525.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5015 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/terasic_de0nano.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5560 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/terasic_de10lite.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6363 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/terasic_de10nano.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5964 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/terasic_de1soc.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     1908 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/terasic_de2_115.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    14493 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/terasic_deca.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7962 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/terasic_sockit.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2583 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/tinyfpga_bx.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    11196 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/trellisboard.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4787 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/trenz_c10lprefkit.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     2906 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/trenz_cyc1000.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4043 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/trenz_max1000.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3638 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/trenz_te0725.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     4765 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/trenz_tec0117.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3248 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/tul_pynq_z2.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9257 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_ac701.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    16681 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_alveo_u200.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    16629 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_alveo_u250.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    12333 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_alveo_u280.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    19654 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_kc705.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    18771 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_kcu105.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     1495 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_kv260.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5827 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_sp605.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    23087 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_vc707.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     9582 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_vcu118.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     6568 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_vcu128.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3083 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_zcu102.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5395 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_zcu104.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     5906 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_zcu106.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     1819 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/xilinx_zcu216.py
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     7666 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/platforms/ztex213.py
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:47:25.957851 litex-boards-2023.8/litex_boards/targets/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/__init__.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5951 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/adi_adrv2crr_fmc.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3314 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/adi_plutosdr.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4879 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/alchitry_au.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4767 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/alchitry_cu.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7968 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/alchitry_mojo.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3357 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/aliexpress_xc7k420t.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     2944 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/alinx_ax7010.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7618 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/alinx_axu2cga.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7310 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/antmicro_artix_dc_scm.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    12087 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/antmicro_datacenter_ddr4_test_board.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7677 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/antmicro_lpddr4_test_board.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5225 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/antmicro_sdi_mipi_video_converter.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3185 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/arduino_mkrvidor4000.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5410 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/avnet_aesku40.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7029 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/berkeleylab_marble.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4548 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/camlink_4k.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    12636 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/colorlight_5a_75x.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    10771 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/colorlight_i5.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8543 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/colorlight_i9plus.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3444 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/decklink_intensity_pro_4k.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8214 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/decklink_mini_4k.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5623 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/decklink_quad_hdmi_recorder.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9913 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/digilent_arty.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4685 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/digilent_arty_s7.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8056 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/digilent_arty_z7.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9506 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/digilent_atlys.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4195 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/digilent_basys3.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     6320 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/digilent_cmod_a7.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4984 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/digilent_genesys2.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9859 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/digilent_nexys4.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     6486 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/digilent_nexys4ddr.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9264 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/digilent_nexys_video.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5190 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/digilent_pynq_z1.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     6851 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/digilent_zedboard.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3185 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/ebaz4205.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4521 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/efinix_t8f81_dev_kit.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     6978 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/efinix_titanium_ti60_f225_dev_kit.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    24244 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/efinix_trion_t120_bga576_dev_kit.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3877 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/efinix_trion_t20_bga256_dev_kit.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3405 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/efinix_trion_t20_mipi_dev_kit.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4433 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/efinix_xyloni_dev_kit.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3534 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/ego1.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4016 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/enclustra_mercury_kx2.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4000 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/enclustra_mercury_xu5.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5129 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/fairwaves_xtrx.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     6409 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/fpc_iii.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3334 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/fpgawars_alhambra2.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4804 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/gadgetfactory_papilio_pro.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9092 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/gsd_butterstick.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8994 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/gsd_orangecrab.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3390 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/hackaday_hadbadge.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7667 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/ice_v_wireless.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7171 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/icebreaker.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7801 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/icebreaker_bitsy.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4710 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/isx_im1283.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4919 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/jungle_electronics_fireant.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7323 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/kosagi_fomu.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5977 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/kosagi_netv2.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5470 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/krtkl_snickerdoodle.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    10545 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/lambdaconcept_ecpix5.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     6462 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/lattice_crosslink_nx_evn.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5184 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/lattice_crosslink_nx_vip.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3679 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/lattice_ecp5_evn.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8410 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/lattice_ecp5_vip.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5969 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/lattice_ice40up5k_evn.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     6307 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/lattice_versa_ecp5.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     6086 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/limesdr_mini_v2.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4922 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/linsn_rv901t.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7543 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/litex_acorn_baseboard.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     6713 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/logicbone.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9381 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/machdyne_konfekt.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9239 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/machdyne_kopflos.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4797 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/machdyne_krote.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9479 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/machdyne_noir.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8981 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/machdyne_schoko.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5594 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/micronova_mercury2.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4178 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/mist.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    10829 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/mnt_rkx7.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5471 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/muselab_icesugar.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9135 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/muselab_icesugar_pro.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3016 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/myminieye_runber.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3502 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/newae_cw305.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4857 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/numato_aller.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4407 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/numato_mimas_a7.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4319 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/numato_nereid.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4763 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/numato_tagus.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9948 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/ocp_tap_timecard.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7172 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/opalkelly_xem8320.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4721 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/pano_logic_g2.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5853 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/qmtech_10cl006.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8425 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/qmtech_5cefa2.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8365 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/qmtech_5cefa5.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9526 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/qmtech_artix7_fbg484.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9518 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/qmtech_artix7_fgg676.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5269 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/qmtech_ep4ce15_starter_kit.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8299 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/qmtech_ep4cex5.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8117 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/qmtech_ep4cgx150.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8404 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/qmtech_wukong.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9237 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/qmtech_xc7a35t.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    12062 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/qmtech_xc7k325t.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4501 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/quicklogic_quickfeather.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5035 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/qwertyembedded_beaglewire.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8901 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/radiona_ulx3s.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    10672 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/radiona_ulx4m_ld_v2.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7882 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/rcs_arctic_tern_bmc_card.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4804 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/redpitaya.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4487 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/rz_easyfpga.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8425 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/saanlima_pipistrello.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5851 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/scarabhardware_minispartan6.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5314 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/seeedstudio_spartan_edge_accelerator.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8778 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/siglent_sds1104xe.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     2792 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/simple.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4204 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/sipeed_tang_nano.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     6130 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/sipeed_tang_nano_20k.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7314 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/sipeed_tang_nano_4k.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7643 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/sipeed_tang_nano_9k.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3099 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/sipeed_tang_primer.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    10389 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/sipeed_tang_primer_20k.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     2745 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/sitlinv_a_e115fb.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    11386 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/sitlinv_stlv7325_v1.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9949 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/sitlinv_stlv7325_v2.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7032 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/sitlinv_xc7k420t.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8586 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/sqrl_acorn.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7055 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/sqrl_fk33.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     6862 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/sqrl_xcu1525.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4422 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/terasic_de0nano.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4251 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/terasic_de10lite.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5444 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/terasic_de10nano.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3499 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/terasic_de1soc.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3175 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/terasic_de2_115.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8039 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/terasic_deca.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     6433 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/terasic_sockit.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3018 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/tinyfpga_bx.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8734 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/trellisboard.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4987 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/trenz_c10lprefkit.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3400 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/trenz_cyc1000.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3475 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/trenz_max1000.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3324 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/trenz_te0725.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7805 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/trenz_tec0117.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     3458 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/tul_pynq_z2.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7643 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/xilinx_ac701.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5257 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/xilinx_alveo_u200.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     5204 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/xilinx_alveo_u250.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8812 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/xilinx_alveo_u280.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7350 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/xilinx_kc705.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     7924 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/xilinx_kcu105.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)    10175 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/xilinx_kv260.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4496 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/xilinx_vc707.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4101 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/xilinx_vcu118.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     6101 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/xilinx_vcu128.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     2124 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/xilinx_zcu102.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4106 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/xilinx_zcu104.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4727 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/xilinx_zcu106.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     9451 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/xilinx_zcu216.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     8981 2023-09-17 21:44:27.000000 litex-boards-2023.8/litex_boards/targets/xilinx_zybo_z7.py
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)     4914 2023-09-17 21:45:26.000000 litex-boards-2023.8/litex_boards/targets/ztex213.py
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:47:25.921850 litex-boards-2023.8/litex_boards.egg-info/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    11203 2023-09-17 21:47:25.000000 litex-boards-2023.8/litex_boards.egg-info/PKG-INFO
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)    14142 2023-09-17 21:47:25.000000 litex-boards-2023.8/litex_boards.egg-info/SOURCES.txt
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        1 2023-09-17 21:47:25.000000 litex-boards-2023.8/litex_boards.egg-info/dependency_links.txt
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)        6 2023-09-17 21:47:25.000000 litex-boards-2023.8/litex_boards.egg-info/requires.txt
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)       13 2023-09-17 21:47:25.000000 litex-boards-2023.8/litex_boards.egg-info/top_level.txt
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)       38 2023-09-17 21:47:25.957851 litex-boards-2023.8/setup.cfg
+-rwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)      706 2023-09-17 21:47:18.000000 litex-boards-2023.8/setup.py
+drwxrwxr-x   0 timkpaine  (1000) timkpaine  (1000)        0 2023-09-17 21:47:25.957851 litex-boards-2023.8/test/
+-rw-rw-r--   0 timkpaine  (1000) timkpaine  (1000)     3845 2023-09-17 21:44:27.000000 litex-boards-2023.8/test/test_targets.py
```

### Comparing `litex-boards-2023.12/LICENSE` & `litex-boards-2023.8/LICENSE`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/PKG-INFO` & `litex-boards-2023.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: litex-boards
-Version: 2023.12
+Version: 2023.8
 Summary: LiteX supported boards
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/litex-hub/litex-boards
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
-Requires-Python: ~=3.7
+Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: litex
 
 
                                   __   _ __      _  __    ___                   __
                                  / /  (_) /____ | |/_/___/ _ )___  ___ ________/ /__
                                 / /__/ / __/ -_)>  </___/ _  / _ \/ _ `/ __/ _  (_-<
                                /____/_/\__/\__/_/|_|   /____/\___/\_,_/_/  \_,_/___/
 
@@ -107,18 +106,16 @@
 ---------------
     ├── adi_adrv2crr_fmc
     ├── adi_plutosdr
     ├── alchitry_au
     ├── alchitry_cu
     ├── alchitry_mojo
     ├── aliexpress_xc7k420t
-    ├── aliexpress_xc7k70t
     ├── alinx_ax7010
     ├── alinx_axu2cga
-    ├── analog_pocket
     ├── antmicro_artix_dc_scm
     ├── antmicro_datacenter_ddr4_test_board
     ├── antmicro_lpddr4_test_board
     ├── antmicro_sdi_mipi_video_converter
     ├── arduino_mkrvidor4000
     ├── avalanche
     ├── avnet_aesku40
@@ -184,15 +181,14 @@
     ├── limesdr_mini_v2
     ├── linsn_rv901t
     ├── litex_acorn_baseboard
     ├── logicbone
     ├── machdyne_konfekt
     ├── machdyne_kopflos
     ├── machdyne_krote
-    ├── machdyne_mozart_ml1
     ├── machdyne_noir
     ├── machdyne_schoko
     ├── marblemini
     ├── marble
     ├── micronova_mercury2
     ├── mist
     ├── mnt_rkx7
@@ -227,17 +223,15 @@
     ├── scarabhardware_minispartan6
     ├── seeedstudio_spartan_edge_accelerator
     ├── siglent_sds1104xe
     ├── sipeed_tang_nano_20k
     ├── sipeed_tang_nano_4k
     ├── sipeed_tang_nano_9k
     ├── sipeed_tang_nano
-    ├── sipeed_tang_mega_138k
     ├── sipeed_tang_primer_20k
-    ├── sipeed_tang_primer_25k
     ├── sipeed_tang_primer
     ├── sitlinv_a_e115fb
     ├── sitlinv_stlv7325
     ├── sitlinv_xc7k420t
     ├── sqrl_acorn
     ├── sqrl_fk33
     ├── sqrl_xcu1525
```

### Comparing `litex-boards-2023.12/README.md` & `litex-boards-2023.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -93,18 +93,16 @@
 ---------------
     ├── adi_adrv2crr_fmc
     ├── adi_plutosdr
     ├── alchitry_au
     ├── alchitry_cu
     ├── alchitry_mojo
     ├── aliexpress_xc7k420t
-    ├── aliexpress_xc7k70t
     ├── alinx_ax7010
     ├── alinx_axu2cga
-    ├── analog_pocket
     ├── antmicro_artix_dc_scm
     ├── antmicro_datacenter_ddr4_test_board
     ├── antmicro_lpddr4_test_board
     ├── antmicro_sdi_mipi_video_converter
     ├── arduino_mkrvidor4000
     ├── avalanche
     ├── avnet_aesku40
@@ -170,15 +168,14 @@
     ├── limesdr_mini_v2
     ├── linsn_rv901t
     ├── litex_acorn_baseboard
     ├── logicbone
     ├── machdyne_konfekt
     ├── machdyne_kopflos
     ├── machdyne_krote
-    ├── machdyne_mozart_ml1
     ├── machdyne_noir
     ├── machdyne_schoko
     ├── marblemini
     ├── marble
     ├── micronova_mercury2
     ├── mist
     ├── mnt_rkx7
@@ -213,17 +210,15 @@
     ├── scarabhardware_minispartan6
     ├── seeedstudio_spartan_edge_accelerator
     ├── siglent_sds1104xe
     ├── sipeed_tang_nano_20k
     ├── sipeed_tang_nano_4k
     ├── sipeed_tang_nano_9k
     ├── sipeed_tang_nano
-    ├── sipeed_tang_mega_138k
     ├── sipeed_tang_primer_20k
-    ├── sipeed_tang_primer_25k
     ├── sipeed_tang_primer
     ├── sitlinv_a_e115fb
     ├── sitlinv_stlv7325
     ├── sitlinv_xc7k420t
     ├── sqrl_acorn
     ├── sqrl_fk33
     ├── sqrl_xcu1525
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/adi_adrv2crr_fmc.py` & `litex-boards-2023.8/litex_boards/platforms/adi_adrv2crr_fmc.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/adi_plutosdr.py` & `litex-boards-2023.8/litex_boards/platforms/adi_plutosdr.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/alchitry_au.py` & `litex-boards-2023.8/litex_boards/platforms/alchitry_au.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/alchitry_cu.py` & `litex-boards-2023.8/litex_boards/platforms/alchitry_cu.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/alchitry_mojo.py` & `litex-boards-2023.8/litex_boards/platforms/alchitry_mojo.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/aliexpress_xc7k420t.py` & `litex-boards-2023.8/litex_boards/platforms/aliexpress_xc7k420t.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/aliexpress_xc7k70t.py` & `litex-boards-2023.8/litex_boards/platforms/kosagi_netv2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,245 +1,208 @@
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2023 Hans Baier <hansfbaier@gmail.com>
+# Copyright (c) 2019 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from litex.build.generic_platform import *
 from litex.build.xilinx import Xilinx7SeriesPlatform
 from litex.build.openocd import OpenOCD
 
-# This board is available here:
-# https://www.aliexpress.com/item/1005005572549665.html
-
 # IOs ----------------------------------------------------------------------------------------------
 
 _io = [
     # Clk / Rst
-    ("clk50",            0, Pins("E11"), IOStandard("LVCMOS33")),
-    ("sma_global_clock", 0, Pins("C12"), IOStandard("LVCMOS33")),
-    ("sma_global_clock", 1, Pins("C11"), IOStandard("LVCMOS33")),
+    ("clk50", 0, Pins("J19"), IOStandard("LVCMOS33")),
 
     # Leds
-    ("user_led", 0, Pins("AD9"),  IOStandard("LVCMOS18")),
-    ("user_led", 1, Pins("AD8"),  IOStandard("LVCMOS18")),
-    ("user_led", 2, Pins("AC9"),  IOStandard("LVCMOS18")),
-    ("user_led", 3, Pins("AC8"),  IOStandard("LVCMOS18")),
-
-    # Buttons
-    ("user_btn_n", 0, Pins("AF7"),  IOStandard("LVCMOS18")),
-    ("user_btn_n", 1, Pins("AF8"),  IOStandard("LVCMOS18")),
-    ("user_btn_n", 2, Pins("AE8"),  IOStandard("LVCMOS18")),
-    ("user_btn_n", 3, Pins("AF9"),  IOStandard("LVCMOS18")),
-
+    ("user_led", 0, Pins("M21"),  IOStandard("LVCMOS33")),
+    ("user_led", 1, Pins("N20"),  IOStandard("LVCMOS33")),
+    ("user_led", 2, Pins("L21"),  IOStandard("LVCMOS33")),
+    ("user_led", 3, Pins("AA21"), IOStandard("LVCMOS33")),
+    ("user_led", 4, Pins("R19"),  IOStandard("LVCMOS33")),
+    ("user_led", 5, Pins("M16"),  IOStandard("LVCMOS33")),
+
+    # SPIFlash
+    ("spiflash", 0,
+        Subsignal("cs_n", Pins("T19")),
+        Subsignal("mosi", Pins("P22")),
+        Subsignal("miso", Pins("R22")),
+        Subsignal("vpp",  Pins("P21")),
+        Subsignal("hold", Pins("R21")),
+        IOStandard("LVCMOS33")
+    ),
+    ("spiflash4x", 0,
+        Subsignal("cs_n", Pins("T19")),
+        Subsignal("dq",   Pins("P22 R22 P21 R21")),
+        IOStandard("LVCMOS33")
+    ),
 
     # Serial
     ("serial", 0,
-        Subsignal("tx",  Pins("HR_IO:0")),
-        Subsignal("rx",  Pins("HR_IO:1")),
-        IOStandard("LVCMOS33")
+        Subsignal("tx", Pins("E14")),
+        Subsignal("rx", Pins("E13")),
+        IOStandard("LVCMOS33"),
     ),
 
-    # SDRAM
-    ("sdram_clock", 0, Pins("P23"), IOStandard("LVCMOS33"), Misc("SLEW=FAST")),
-    ("sdram", 0,
-        Subsignal("a",     Pins("L25 L24 K23 M26 G25 F24 H26 F23 E23 J26 M25 G24")),
-        Subsignal("dq",    Pins("T23 T25 T24 R25 R23 R26 P24 P25 F25 H24 E26 H23 E25 J24 D26 J23")),
-        Subsignal("ba",    Pins("K25 M24")),
-        Subsignal("dm",    Pins("N23 G26")),
-        Subsignal("ras_n", Pins("N24")),
-        Subsignal("cas_n", Pins("K26")),
-        Subsignal("we_n",  Pins("P26")),
-        Subsignal("cs_n",  Pins("N26")),
-        Subsignal("cke",   Pins("J25")),
-        IOStandard("LVCMOS33"),
-        Misc("SLEW = FAST")
+    # DDR3 SDRAM
+    ("ddram", 0,
+        Subsignal("a", Pins(
+            "U6 V4 W5 V5 AA1 Y2 AB1 AB3",
+            "AB2 Y3 W6 Y1 V2 AA3"),
+            IOStandard("SSTL15_R")),
+        Subsignal("ba",    Pins("U5 W4 V7"), IOStandard("SSTL15_R")),
+        Subsignal("ras_n", Pins("Y9"), IOStandard("SSTL15_R")),
+        Subsignal("cas_n", Pins("Y7"), IOStandard("SSTL15_R")),
+        Subsignal("we_n",  Pins("V8"), IOStandard("SSTL15_R")),
+        Subsignal("dm", Pins("G1 H4 M5 L3"), IOStandard("SSTL15_R")),
+        Subsignal("dq", Pins(
+            "C2 F1 B1 F3 A1 D2 B2 E2",
+            "J5 H3 K1 H2 J1 G2 H5 G3",
+            "N2 M6 P1 N5 P2 N4 R1 P6",
+            "K3 M2 K4 M3 J6 L5 J4 K6"),
+            IOStandard("SSTL15_R"),
+            Misc("IN_TERM=UNTUNED_SPLIT_40")),
+        Subsignal("dqs_p", Pins("E1 K2 P5 M1"), IOStandard("DIFF_SSTL15_R")),
+        Subsignal("dqs_n", Pins("D1 J2 P4 L1"), IOStandard("DIFF_SSTL15_R")),
+        Subsignal("clk_p", Pins("R3"), IOStandard("DIFF_SSTL15_R")),
+        Subsignal("clk_n", Pins("R2"), IOStandard("DIFF_SSTL15_R")),
+        Subsignal("cke",   Pins("Y8"), IOStandard("SSTL15_R")),
+        Subsignal("odt",   Pins("W9"), IOStandard("SSTL15_R")),
+        Subsignal("reset_n", Pins("AB5"), IOStandard("LVCMOS15")),
+        Subsignal("cs_n", Pins("V9"), IOStandard("SSTL15_R")),
+        Misc("SLEW=FAST"),
     ),
 
-    ("spiflash4x", 0,  # clock needs to be accessed through STARTUPE2
-        Subsignal("cs_n", Pins("C23")),
-        Subsignal("dq",   Pins("B24 A25 B22 A22")),
-        IOStandard("LVCMOS33")
+    # PCIe
+    ("pcie_x1", 0,
+        Subsignal("rst_n", Pins("E18"), IOStandard("LVCMOS33")),
+        Subsignal("clk_p", Pins("F10")),
+        Subsignal("clk_n", Pins("E10")),
+        Subsignal("rx_p",  Pins("D11")),
+        Subsignal("rx_n",  Pins("C11")),
+        Subsignal("tx_p",  Pins("D5")),
+        Subsignal("tx_n",  Pins("C5"))
     ),
-    ("spiflash8x", 0,
-        Subsignal("clk",  Pins("A14")),
-        Subsignal("cs_n", Pins("B11")),
-        Subsignal("dq",   Pins("A13 A10 B10 B14 A15 B12 A12 B15")),
-        IOStandard("LVCMOS33")
+    ("pcie_x2", 0,
+        Subsignal("rst_n", Pins("E18"), IOStandard("LVCMOS33")),
+        Subsignal("clk_p", Pins("F10")),
+        Subsignal("clk_n", Pins("E10")),
+        Subsignal("rx_p",  Pins("D11 B10")),
+        Subsignal("rx_n",  Pins("C11 A10")),
+        Subsignal("tx_p",  Pins("D5 B6")),
+        Subsignal("tx_n",  Pins("C5 A6"))
+    ),
+    ("pcie_x4", 0,
+        Subsignal("rst_n", Pins("E18"), IOStandard("LVCMOS33")),
+        Subsignal("clk_p", Pins("F10")),
+        Subsignal("clk_n", Pins("E10")),
+        Subsignal("rx_p",  Pins("D11 B10 D9 B8")),
+        Subsignal("rx_n",  Pins("C11 A10 C9 A8")),
+        Subsignal("tx_p",  Pins("D5 B6 D7 B4")),
+        Subsignal("tx_n",  Pins("C5 A6 C7 A4"))
     ),
 
-    # RGMII Ethernet
+    # RMII Ethernet
     ("eth_clocks", 0,
-        Subsignal("tx",  Pins("AF13"), IOStandard("LVCMOS18")),
-        Subsignal("rx",  Pins("AB11"), IOStandard("LVCMOS18"))
+        Subsignal("ref_clk", Pins("D17")),
+        IOStandard("LVCMOS33"),
     ),
     ("eth", 0,
-        # Subsignal("rst_n",   Pins("")),
-        Subsignal("mdio",    Pins("AD13")),
-        Subsignal("mdc",     Pins("AC13")),
-        Subsignal("rx_ctl",  Pins("AF10")),
-        Subsignal("rx_data", Pins("AE10 AE11 AF12 AE12")),
-        Subsignal("tx_ctl",  Pins("AE13")),
-        Subsignal("tx_data", Pins("AD10 AD11 AC11 AC12")),
-        IOStandard("LVCMOS18")
-    ),
+        Subsignal("rst_n",   Pins("F16")),
+        Subsignal("rx_data", Pins("A20 B18")),
+        Subsignal("crs_dv",  Pins("C20")),
+        Subsignal("tx_en",   Pins("A19")),
+        Subsignal("tx_data", Pins("C18 C19")),
+        Subsignal("mdc",     Pins("F14")),
+        Subsignal("mdio",    Pins("F13")),
+        Subsignal("rx_er",   Pins("B20")),
+        Subsignal("int_n",   Pins("D21")),
+        IOStandard("LVCMOS33")
+     ),
 
-    # camera connector I2C, has pull up resistors
-    ("i2c", 0,
-        Subsignal("scl", Pins("C13")),
-        Subsignal("sda", Pins("C16")),
-        IOStandard("LVCMOS33"),
+     # SDCard
+    ("spisdcard", 0,
+        Subsignal("clk",  Pins("K18")),
+        Subsignal("cs_n", Pins("M13")),
+        Subsignal("mosi", Pins("L13"), Misc("PULLUP")),
+        Subsignal("miso", Pins("L15"), Misc("PULLUP")),
+        Misc("SLEW=FAST"),
+        IOStandard("LVCMOS33")
     ),
-
-    ("camera", 0,
-        Subsignal("d",     Pins("C17 B16 A17 B17 A18 D16 C18 D13")),
-        Subsignal("vsync", Pins("C14")),
-        Subsignal("xclk",  Pins("C19")),
-        Subsignal("pclk",  Pins("E18")),
-        Subsignal("pwdn",  Pins("D11")),
-        Subsignal("reset", Pins("D15")),
-        Subsignal("href",  Pins("D14")),
-        IOStandard("LVCMOS33"),
+    ("sdcard", 0,
+        Subsignal("clk",  Pins("K18")),
+        Subsignal("cmd",  Pins("L13"), Misc("PULLUP True")),
+        Subsignal("data", Pins("L15 L16 K14 M13"), Misc("PULLUP True")),
+        IOStandard("LVCMOS33"), Misc("SLEW=FAST")
+    ),
+
+    # HDMI In
+    ("hdmi_in", 0,
+        Subsignal("clk_p",   Pins("L19"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("clk_n",   Pins("L20"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data0_p", Pins("K21"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data0_n", Pins("K22"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data1_p", Pins("J20"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data1_n", Pins("J21"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data2_p", Pins("J22"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data2_n", Pins("H22"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("scl",     Pins("T18"), IOStandard("LVCMOS33")),
+        Subsignal("sda",     Pins("V18"), IOStandard("LVCMOS33")),
+    ),
+    ("hdmi_in", 1,
+        Subsignal("clk_p",   Pins("Y18"),  IOStandard("TMDS_33"), Inverted()),
+        Subsignal("clk_n",   Pins("Y19"),  IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data0_p", Pins("AA18"), IOStandard("TMDS_33")),
+        Subsignal("data0_n", Pins("AB18"), IOStandard("TMDS_33")),
+        Subsignal("data1_p", Pins("AA19"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data1_n", Pins("AB20"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data2_p", Pins("AB21"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data2_n", Pins("AB22"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("scl",     Pins("W17"),  IOStandard("LVCMOS33"), Inverted()),
+        Subsignal("sda",     Pins("R17"),  IOStandard("LVCMOS33")),
     ),
 
-    # HDMI out
+    # HDMI Out
     ("hdmi_out", 0,
-        Subsignal("clk_p",   Pins("E10")),
-        Subsignal("clk_n",   Pins("D10")),
-        Subsignal("data0_p", Pins("D9")),
-        Subsignal("data0_n", Pins("D8")),
-        Subsignal("data1_p", Pins("C9")),
-        Subsignal("data1_n", Pins("B9")),
-        Subsignal("data2_p", Pins("A9")),
-        Subsignal("data2_n", Pins("A8")),
-        IOStandard("TMDS_33"),
-    ),
-
-    # PCIe
-    ("pcie_x1", 0,
-        Subsignal("rst_n", Pins("F8"), IOStandard("LVCMOS33")),
-        Subsignal("clk_p", Pins("F5")),
-        Subsignal("clk_n", Pins("F6")),
-        Subsignal("rx_p",  Pins("B6")),
-        Subsignal("rx_n",  Pins("B5")),
-        Subsignal("tx_p",  Pins("A4")),
-        Subsignal("tx_n",  Pins("A3"))
-    ),
-    ("pcie_x2", 0,
-        Subsignal("rst_n", Pins("F8"), IOStandard("LVCMOS33")),
-        Subsignal("clk_p", Pins("F5")),
-        Subsignal("clk_n", Pins("F6")),
-        Subsignal("rx_p",  Pins("B6 C4")),
-        Subsignal("rx_n",  Pins("B5 C3")),
-        Subsignal("tx_p",  Pins("A4 B2")),
-        Subsignal("tx_n",  Pins("A3 B1"))
-    ),
-    ("pcie_x4", 0,
-        Subsignal("rst_n", Pins("F8"), IOStandard("LVCMOS33")),
-        Subsignal("clk_p", Pins("F5")),
-        Subsignal("clk_n", Pins("F6")),
-        Subsignal("rx_p",  Pins("B6 C4 E4 G4")),
-        Subsignal("rx_n",  Pins("B5 C3 E3 G3")),
-        Subsignal("tx_p",  Pins("A4 B2 D2 F2")),
-        Subsignal("tx_n",  Pins("A3 B1 D1 F1"))
+        Subsignal("clk_p",   Pins("W19"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("clk_n",   Pins("W20"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data0_p", Pins("W21"), IOStandard("TMDS_33")),
+        Subsignal("data0_n", Pins("W22"), IOStandard("TMDS_33")),
+        Subsignal("data1_p", Pins("U20"), IOStandard("TMDS_33")),
+        Subsignal("data1_n", Pins("V20"), IOStandard("TMDS_33")),
+        Subsignal("data2_p", Pins("T21"), IOStandard("TMDS_33")),
+        Subsignal("data2_n", Pins("U21"), IOStandard("TMDS_33"))
+    ),
+    ("hdmi_out", 1,
+        Subsignal("clk_p",   Pins("G21"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("clk_n",   Pins("G22"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data0_p", Pins("E22"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data0_n", Pins("D22"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data1_p", Pins("C22"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data1_n", Pins("B22"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data2_p", Pins("B21"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("data2_n", Pins("A21"), IOStandard("TMDS_33"), Inverted()),
     ),
 ]
 
-# Connectors ---------------------------------------------------------------------------------------
-
-_connectors = [
-    # 1.8V
-    ("HP_IO", {
-        "0_P"  :  "AE6",
-        "0_N"  :  "AE5",
-        "1_P"  :  "AD6",
-        "1_N"  :  "AD5",
-        "2_P"  :  "AF5",
-        "2_N"  :  "AF4",
-        "3_P"  :  "AD4",
-        "3_N"  :  "AD3",
-        "4_P"  :  "AF3",
-        "4_N"  :  "AF2",
-        "5_P"  :  "AE3",
-        "5_N"  :  "AE2",
-        "6_P"  :  "AB2",
-        "6_N"  :  "AC2",
-        "7_P"  :  "V2",
-        "7_N"  :  "V1",
-        "8_P"  :  "AA3",
-        "8_N"  :  "AA2",
-        "9_P"  :  "AB1",
-        "9_N"  :  "AC1",
-        "10_P" :  "W1",
-        "10_N" :  "Y1",
-        "11_P" :  "AD1",
-        "11_N" :  "AE1",
-    }),
-
-    # 3.3V
-    ("HR_IO", {
-        0  : "D19",
-        1  : "D18",
-        2  : "C21",
-        3  : "D20",
-        4  : "C22",
-        5  : "D21",
-        6  : "C24",
-        7  : "D23",
-        8  : "D24",
-        9  : "A19",
-        10 : "B19",
-        11 : "A20",
-        12 : "B20",
-        13 : "B21",
-        14 : "A23",
-        15 : "A24",
-        16 : "B25",
-        17 : "B26",
-        18 : "C26",
-        19 : "D25",
-    }),
-
-    # 3.3V
-    ("CAM", {
-        3  : "C14",
-        4  : "C13", # has pull up resistor
-        5  : "D14",
-        6  : "C16", # has pull up resistor
-        7  : "D15",
-        8  : "C17",
-        9  : "B16",
-        10 : "A17",
-        11 : "B17",
-        12 : "A18",
-        13 : "D16",
-        14 : "C18",
-        15 : "D13",
-        16 : "E18",
-        17 : "C19",
-        18 : "D11",
-    })
-]
 # Platform -----------------------------------------------------------------------------------------
 
 class Platform(Xilinx7SeriesPlatform):
     default_clk_name   = "clk50"
     default_clk_period = 1e9/50e6
 
-    def __init__(self):
-        Xilinx7SeriesPlatform.__init__(self, "xc7k70t-fbg676-1", _io, _connectors, toolchain="vivado")
-        self.add_platform_command("""
-set_property CFGBVS VCCO [current_design]
-set_property CONFIG_VOLTAGE 3.3 [current_design]
-set_property BITSTREAM.GENERAL.COMPRESS TRUE [current_design]
-""")
-        self.toolchain.bitstream_commands  = ["set_property BITSTREAM.CONFIG.SPI_BUSWIDTH 4 [current_design]"]
-        self.toolchain.additional_commands = ["write_cfgmem -force -format bin -interface spix4 -size 16 -loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin"]
+    def __init__(self, variant="a7-35", toolchain="vivado"):
+        device = {
+            "a7-35":  "xc7a35t-fgg484-2",
+            "a7-100": "xc7a100t-fgg484-2"
+        }[variant]
+        Xilinx7SeriesPlatform.__init__(self, device, _io, toolchain=toolchain)
 
     def create_programmer(self):
-        return OpenOCD("openocd_xc7_ft4232.cfg", "bscan_spi_xc7k70t.bit")
+        bscan_spi = "bscan_spi_xc7a100t.bit" if "xc7a100t" in self.device else "bscan_spi_xc7a35t.bit"
+        return OpenOCD("openocd_netv2_rpi.cfg", bscan_spi)
 
     def do_finalize(self, fragment):
         Xilinx7SeriesPlatform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk50",         0, loose=True), 1e9/50e6)
-        self.add_period_constraint(self.lookup_request("eth_clocks:rx", 0, loose=True), 1e9/125e6)
-        self.add_period_constraint(self.lookup_request("eth_clocks:tx", 0, loose=True), 1e9/125e6)
+        self.add_period_constraint(self.lookup_request("clk50",              loose=True), 1e9/50e6)
+        self.add_period_constraint(self.lookup_request("eth_clocks:ref_clk", loose=True), 1e9/50e6)
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/alinx_ax7010.py` & `litex-boards-2023.8/litex_boards/platforms/alinx_ax7010.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/alinx_axu2cga.py` & `litex-boards-2023.8/litex_boards/platforms/alinx_axu2cga.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/analog_pocket.py` & `litex-boards-2023.8/litex_boards/platforms/decklink_quad_hdmi_recorder.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,241 +1,183 @@
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2023 Florent Kermarrec <florent@enjoy-digital.fr>
-# Copyright (c) 2020 Paul Sajna <sajattack@gmail.com>
-# Copyright (c) 2022 Thomas Watson <twatson52@icloud.com>
+# Copyright (c) 2021 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from litex.build.generic_platform import *
-from litex.build.altera import AlteraPlatform
-from litex.build.openfpgaloader import OpenFPGALoader
+from litex.build.xilinx import XilinxUSPlatform, VivadoProgrammer
 
-# IOs (LiteX) --------------------------------------------------------------------------------------
+# IOs ----------------------------------------------------------------------------------------------
 
-_io_physical_litex = [
-    # Clk.
-    ("clk74a", 0, Pins("V15"), IOStandard("3.3-V LVCMOS")),
-    ("clk74b", 0, Pins("H16"), IOStandard("1.8 V")),
-
-    # Serial.
-    ("serial", 0,
-        Subsignal("tx", Pins("K21")),
-        Subsignal("rx", Pins("K22")),
-        IOStandard("1.8V")
-    ),
-
-    # SDR SDRAM
-    ("sdram_clock", 0, Pins("G12"),
-        Misc("OUTPUT_TERMINATION \"SERIES 50 OHM WITHOUT CALIBRATION\""),
-        IOStandard("1.8V")
-    ),
-    ("sdram", 0,
-        Subsignal("a",     Pins(
-            "D17 D12 F12 E14 F13 E16 E15 F14",
-            "J18 G17 C13 F15 J17")),
-        Subsignal("ba",    Pins("C16 E12")),
-        #Subsignal("cs_n",  Pins("")),
-        Subsignal("cke",   Pins("G18")),
-        Subsignal("ras_n", Pins("B11")),
-        Subsignal("cas_n", Pins("B16")),
-        Subsignal("we_n",  Pins("C11")),
-        Subsignal("dq",    Pins(
-            "C15 B15 A15 B13 A14 B12 A13 A12",
-            "J13 G15 G16 G13 H13 J19 G11 K20",
-        )),
-        Subsignal("dm", Pins("D13 H18")),
-        Misc("CURRENT_STRENGTH_NEW \"4MA\""),
-        IOStandard("1.8V"),
-    ),
-]
-
-_io_fpga2fpga_litex = [
-    # Video Scaler.
-    ("video", 0,
-        Subsignal("clk",   Pins("R17")),
-        Subsignal("de",    Pins("N20")),
-        Subsignal("skip",  Pins("N21")),
-        Subsignal("hsync", Pins("P17")),
-        Subsignal("vsync", Pins("T15")),
-        Subsignal("data",  Pins(
-            "R21 P22 N16 P18 P19 T20",
-            "T19 T18 T22 R22 R15 R16"
-        )),
-        Misc("OUTPUT_TERMINATION \"SERIES 50 OHM WITHOUT CALIBRATION\""),
-        IOStandard("1.8 V"),
-    ),
-]
-
-# IOs (Analog) -------------------------------------------------------------------------------------
-
-_io_physical_analog = [
-    # Clk.
-    ("clk_74a", 0, Pins("V15"), IOStandard("3.3-V LVCMOS")),
-    ("clk_74b", 0, Pins("H16"), IOStandard("1.8 V")),
-
-    # Cartbrige.
-    ("cart",  0,
-        Subsignal("tran_bank0",        Pins("AB7 AA8 AB8 AA9")),
-        Subsignal("tran_bank0_dir",    Pins("AB6")),
-        Subsignal("tran_bank1",        Pins("AB13 AA12 AB12 Y11 AB11 Y10 AB10 AA10")),
-        Subsignal("tran_bank1_dir",    Pins("AA13")),
-        Subsignal("tran_bank2",        Pins("AB20 AA19 AA18 AB18 AA17 AB17 AA15 AB15")),
-        Subsignal("tran_bank2_dir",    Pins("AA14")),
-        Subsignal("tran_bank3",        Pins("W22 W21 Y22 Y21 AA22 AB22 AB21 AA20")),
-        Subsignal("tran_bank3_dir",    Pins("V21")),
-        Subsignal("tran_pin30",        Pins("L8"),  IOStandard("1.8 V")),
-        Subsignal("tran_pin30_dir",    Pins("AB5")),
-        Subsignal("pin30_pwroff_reset",Pins("L17"), IOStandard("1.8 V")),
-        Subsignal("tran_pin31",        Pins("K9"),  IOStandard("1.8 V")),
-        Subsignal("tran_pin31_dir",    Pins("U22")),
-        IOStandard("3.3-V LVCMOS"),
-    ),
-
-    # Infrared.
-    ("port_ir", 0,
-        Subsignal("rx",         Pins("H10")),
-        Subsignal("tx",         Pins("H11")),
-        Subsignal("rx_disable", Pins("L18")),
-        IOStandard("1.8 V"),
-    ),
-
-    # GBA Link Port.
-    ("port_tran", 0,
-        Subsignal("si",      Pins("V10")),
-        Subsignal("si_dir",  Pins("V9")),
-        Subsignal("so",      Pins("J11"), IOStandard("1.8 V")),
-        Subsignal("so_dir",  Pins("T13")),
-        Subsignal("sck",     Pins("AA7")),
-        Subsignal("sck_dir", Pins("Y9")),
-        Subsignal("sd",      Pins("R9")),
-        Subsignal("sd_dir",  Pins("T9")),
-        IOStandard("3.3-V LVCMOS"),
-    ),
-
-    # PSRAM0 (AS1C8M16).
-    ("cram0", 0,
-        Subsignal("a",     Pins("H6 C6 B6 B7 H9 H8")),
-        Subsignal("dq",    Pins("B10 C8 A9 D7 E9 F10 G6 J7 C9 A10 D9 A8 E7 F9 L7 J9")),
-        Subsignal("wait",  Pins("K7")),
-        Subsignal("clk",   Pins("G10")),
-        Subsignal("adv_n", Pins("J8")),
-        Subsignal("cre",   Pins("F7")),
-        Subsignal("ce0_n", Pins("B5")),
-        Subsignal("ce1_n", Pins("E10")),
-        Subsignal("oe_n",  Pins("D6")),
-        Subsignal("we_n",  Pins("G8")),
-        Subsignal("ub_n",  Pins("A7")),
-        Subsignal("lb_n",  Pins("A5")),
-        IOStandard("1.8 V"),
-    ),
-
-    # PSRAM1 (AS1C8M16).
-    ("cram1", 0,
-        Subsignal("a",     Pins("U2 U1 N1 L2 AA2 Y3")),
-        Subsignal("dq",    Pins("C1 G2 E2 P6 R5 M6 U7 V6 D3 C2 N6 P7 R6 R7 U6 W8")),
-        Subsignal("wait",  Pins("W9")),
-        Subsignal("clk",   Pins("W2")),
-        Subsignal("adv_n", Pins("U8")),
-        Subsignal("cre",   Pins("T7")),
-        Subsignal("ce0_n", Pins("N2")),
-        Subsignal("ce1_n", Pins("T8")),
-        Subsignal("oe_n",  Pins("M7")),
-        Subsignal("we_n",  Pins("AA1")),
-        Subsignal("ub_n",  Pins("G1")),
-        Subsignal("lb_n",  Pins("L1")),
-        IOStandard("1.8 V"),
-    ),
-
-    # SDRAM (AS4C32M16).
-    ("dram", 0,
-        Subsignal("a",     Pins("D17 D12 F12 E14 F13 E16 E15 F14 J18 G17 C13 F15 J17")),
-        Subsignal("ba",    Pins("C16 E12")),
-        Subsignal("dq",    Pins("C15 B15 A15 B13 A14 B12 A13 A12 J13 G15 G16 G13 H13 J19 G11 K20")),
-        Subsignal("dqm",   Pins("D13 H18")),
-        Subsignal("clk",   Pins("G12")),
-        Subsignal("cke",   Pins("G18")),
-        Subsignal("ras_n", Pins("B11")),
-        Subsignal("cas_n", Pins("B16")),
-        Subsignal("we_n",  Pins("C11")),
-        IOStandard("1.8 V"),
-    ),
-
-    # SRAM (AS6C2016).
-    ("sram", 0,
-        Subsignal("a",    Pins("T14 M9 M8 U21 N9 V19 P8 Y19 U13 Y14 U11 T10 V14 R10 U15 U12 V16")),
-        Subsignal("dq",   Pins("N8 P9 P14 Y20 W19 T12 V13 R12 U16 U20 V18 V20 Y17 Y16 W16 Y15")),
-        Subsignal("oe_n", Pins("R14")),
-        Subsignal("we_n", Pins("R11")),
-        Subsignal("ub_n", Pins("U17")),
-        Subsignal("lb_n", Pins("P12")),
-        IOStandard("3.3-V LVCMOS"),
+_io = [
+    # Clk / Rst.
+    # TODO: Document SI5338A.
+    ("clk24",  0, Pins("P26"),  IOStandard("LVCMOS15")),
+    ("clk200", 0,
+        Subsignal("p", Pins("AJ29"), IOStandard("LVDS")),
+        Subsignal("n", Pins("AK30"), IOStandard("LVDS"))
     ),
+    ("clk",   0, Pins("AJ29"), IOStandard("LVCMOS15")),
+    ("clk",   0, Pins("AK30"), IOStandard("LVCMOS15")),
 
     # Debug.
-    ("dbg_tx", 0, Pins("K21"), IOStandard("1.8 V")),
-    ("dbg_rx", 0, Pins("K22"), IOStandard("1.8 V")),
-    ("user1",  0, Pins("M22"), IOStandard("1.8 V")),
-    ("user2",  0, Pins("L22"), IOStandard("1.8 V")),
-
-    # Aux I2C.
-    ("aux_sda", 0, Pins("M18"), IOStandard("1.8 V")),
-    ("aux_scl", 0, Pins("M16"), IOStandard("1.8 V")),
-
-    # Others.
-    ("vblank",    0, Pins("N19"), IOStandard("1.8 V")),
-    ("bist",      0, Pins("U10"), IOStandard("3.3-V LVCMOS")),
-    ("vpll_feed", 0, Pins("P16"), IOStandard("1.8 V")),
-]
+    ("debug", 0, Pins("AL34"), IOStandard("LVCMOS15")),
+    ("debug", 1, Pins("AM34"), IOStandard("LVCMOS15")),
+    ("debug", 2, Pins("AN34"), IOStandard("LVCMOS15")),
+    ("debug", 3, Pins("AP34"), IOStandard("LVCMOS15")),
 
-_io_fpga2fpga_analog = [
-    # Scaler.
-    ("scal", 0,
-        Subsignal("vid",  Pins("R21 P22 N16 P18 P19 T20 T19 T18 T22 R22 R15 R16")),
-        Subsignal("clk",  Pins("R17")),
-        Subsignal("de",   Pins("N20")),
-        Subsignal("skip", Pins("N21")),
-        Subsignal("vs",   Pins("T15")),
-        Subsignal("hs",   Pins("P17")),
-
-        Subsignal("audmclk", Pins("K16")),
-        Subsignal("audadc",  Pins("H15")),
-        Subsignal("auddac",  Pins("K19")),
-        Subsignal("audlrck", Pins("K17")),
-        IOStandard("1.8 V"),
-    ),
-
-    # Bridge.
-    ("bridge", 0,
-        Subsignal("spimosi", Pins("M20")),
-        Subsignal("spimiso", Pins("M21")),
-        Subsignal("spiclk",  Pins("T17")),
-        Subsignal("spiss",   Pins("H14")),
-        Subsignal("lwire",   Pins("L19")),
-        IOStandard("1.8 V"),
+
+    # Serial
+    ("serial", 0,
+        Subsignal("tx", Pins("AP9")),
+        Subsignal("rx", Pins("AN9")),
+        IOStandard("LVCMOS15")
+    ),
+
+    # SPIFlash (MX25L25645GSXDI).
+
+    # TODO (Probably similar to KCU105).
+
+    # PCIe
+    ("pcie_x1", 0,
+        #Subsignal("rst_n", Pins(""), IOStandard("")),
+        Subsignal("clk_p", Pins("AB6")),
+        Subsignal("clk_n", Pins("AB5")),
+        Subsignal("rx_p",  Pins("AB2")),
+        Subsignal("rx_n",  Pins("AB1")),
+        Subsignal("tx_p",  Pins("AC4")),
+        Subsignal("tx_n",  Pins("AC3"))
+    ),
+    ("pcie_x2", 0,
+        #Subsignal("rst_n", Pins(""), IOStandard("")),
+        Subsignal("clk_p", Pins("AB6")),
+        Subsignal("clk_n", Pins("AB5")),
+        Subsignal("rx_p",  Pins("AB2 AD2")),
+        Subsignal("rx_n",  Pins("AB1 AD1")),
+        Subsignal("tx_p",  Pins("AC4 AE4")),
+        Subsignal("tx_n",  Pins("AC3 AE3"))
+    ),
+    ("pcie_x4", 0,
+        #Subsignal("rst_n", Pins(""), IOStandard("")),
+        Subsignal("clk_p", Pins("AB6")),
+        Subsignal("clk_n", Pins("AB5")),
+        Subsignal("rx_p",  Pins("AB2 AD2 AF2 AH2")),
+        Subsignal("rx_n",  Pins("AB1 AD1 AF1 AH1")),
+        Subsignal("tx_p",  Pins("AC4 AE4 AG4 AH6")),
+        Subsignal("tx_n",  Pins("AC3 AE3 AG3 AH5"))
+    ),
+    ("pcie_x8", 0,
+        #Subsignal("rst_n", Pins(""), IOStandard("")),
+        Subsignal("clk_p", Pins("AB6")),
+        Subsignal("clk_n", Pins("AB5")),
+        Subsignal("rx_p",  Pins("AB2 AD2 AF2 AH2 AJ4 AK2 AM2 AP2")),
+        Subsignal("rx_n",  Pins("AB1 AD1 AF1 AH1 AJ3 AK1 AM1 AP1")),
+        Subsignal("tx_p",  Pins("AC4 AE4 AG4 AH6 AK6 AL4 AM6 AN4")),
+        Subsignal("tx_n",  Pins("AC3 AE3 AG3 AH5 AK5 AL3 AM5 AN3"))
+    ),
+
+    # DDR3 SDRAM (H5TQ4G63CFR).
+    ("ddram", 0,
+        Subsignal("a", Pins(
+            "AP16 AM19 AL17 AM14 AL19 AL14 AJ18 AK16",
+            "AJ19 AK17 AP18 AM17 AL18 AH17 AH14"),
+            IOStandard("SSTL15_DCI")),
+        Subsignal("ba",    Pins("AN14 AN19 AP14"), IOStandard("SSTL15_DCI")),
+        Subsignal("ras_n", Pins("AN16"), IOStandard("SSTL15_DCI")),
+        Subsignal("cas_n", Pins("AM16"), IOStandard("SSTL15_DCI")),
+        Subsignal("we_n",  Pins("AP15"), IOStandard("SSTL15_DCI")),
+        Subsignal("cs_n",  Pins("AM15"), IOStandard("SSTL15_DCI")),
+        Subsignal("dm", Pins("AH26 AN26 AJ21 AM21 AH18 AE25 AD21 AD19"),
+            IOStandard("SSTL15_DCI"),
+            Misc("DATA_RATE=DDR")),
+        Subsignal("dq", Pins(
+            "AM27 AK28 AH27 AJ28 AK26 AH28 AM26 AK27",
+            "AP29 AP28 AM30 AN27 AM29 AN28 AL30 AL29",
+            "AM20 AK22 AL20 AL22 AL23 AL24 AK23 AL25",
+            "AP25 AM24 AN24 AM22 AN23 AN22 AP24 AP23",
+            "AJ16 AG17 AG15 AG19 AH16 AH19 AG14 AG16",
+            "AJ24 AG24 AJ23 AF23 AH22 AF24 AH23 AG25",
+            "AE20 AF20 AD20 AG20 AE22 AE23 AF22 AG22",
+            "AF18 AD15 AF17 AE17 AF14 AE18 AF15 AD16"),
+            IOStandard("SSTL15_DCI"),
+            Misc("ODT=RTT_40"),
+            Misc("DATA_RATE=DDR")),
+        Subsignal("dqs_p", Pins("AL27 AN29 AJ20 AP20 AJ15 AH24 AG21 AE16"),
+            IOStandard("DIFF_SSTL15_DCI"),
+            Misc("ODT=RTT_40"),
+            Misc("DATA_RATE=DDR")),
+        Subsignal("dqs_n", Pins("AL28 AP30 AK20 AP21 AJ14 AJ25 AH21 AE15"),
+            IOStandard("DIFF_SSTL15_DCI"),
+             Misc("ODT=RTT_40"),
+            Misc("DATA_RATE=DDR")),
+        Subsignal("clk_p", Pins("AN18"), IOStandard("DIFF_SSTL15_DCI"), Misc("DATA_RATE=DDR")),
+        Subsignal("clk_n", Pins("AN17"), IOStandard("DIFF_SSTL15_DCI"), Misc("DATA_RATE=DDR")),
+        Subsignal("cke",   Pins("AK18"), IOStandard("SSTL15_DCI")),
+        Subsignal("odt",   Pins("AL15"), IOStandard("SSTL15_DCI")),
+        Subsignal("reset_n", Pins("AK15"), IOStandard("SSTL15")),
+        Misc("SLEW=FAST"),
+        Misc("OUTPUT_IMPEDANCE=RDRV_40_40")
+    ),
+
+    # HDMI (through PI3HDX1204)
+    ("hdmi_in", 0, # PCIe Edge Side.
+        #Subsignal("clk_p",   Pins(""), IOStandard("")),
+        #Subsignal("clk_n",   Pins(""), IOStandard("")),
+        Subsignal("data0_p", Pins("Y2")),
+        Subsignal("data0_n", Pins("Y1")),
+        Subsignal("data1_p", Pins("V2")),
+        Subsignal("data1_n", Pins("V1")),
+        Subsignal("data2_p", Pins("T2")),
+        Subsignal("data2_n", Pins("T1")),
+    ),
+    ("hdmi_in", 1,
+        #Subsignal("clk_p",   Pins(""), IOStandard("")),
+        #Subsignal("clk_n",   Pins(""), IOStandard("")),
+        Subsignal("data0_p", Pins("P2")),
+        Subsignal("data0_n", Pins("P1")),
+        Subsignal("data1_p", Pins("M2")),
+        Subsignal("data1_n", Pins("M1")),
+        Subsignal("data2_p", Pins("K2")),
+        Subsignal("data2_n", Pins("K1")),
+    ),
+    ("hdmi_in", 2,
+        #Subsignal("clk_p",   Pins(""), IOStandard("")),
+        #Subsignal("clk_n",   Pins(""), IOStandard("")),
+        Subsignal("data0_p", Pins("H2")),
+        Subsignal("data0_n", Pins("H1")),
+        Subsignal("data1_p", Pins("F2")),
+        Subsignal("data1_n", Pins("F1")),
+        Subsignal("data2_p", Pins("E4")),
+        Subsignal("data2_n", Pins("E3")),
+    ),
+    ("hdmi_in", 3,
+        #Subsignal("clk_p",   Pins(""), IOStandard("")),
+        #Subsignal("clk_n",   Pins(""), IOStandard("")),
+        Subsignal("data0_p", Pins("D2")),
+        Subsignal("data0_n", Pins("D1")),
+        Subsignal("data1_p", Pins("B2")),
+        Subsignal("data1_n", Pins("B1")),
+        Subsignal("data2_p", Pins("B4")),
+        Subsignal("data2_n", Pins("B3")),
     ),
 ]
 
-# Connectors ---------------------------------------------------------------------------------------
-
-_connectors = []
-
 # Platform -----------------------------------------------------------------------------------------
 
-class Platform(AlteraPlatform):
-    default_clk_name   = "clk74a"
-    default_clk_period = 1e9/74.25e6
-
-    def __init__(self, ios="litex", toolchain="quartus"):
-        _io = {
-            "litex"  : _io_physical_litex  + _io_fpga2fpga_litex,
-            "analog" : _io_physical_analog + _io_fpga2fpga_analog,
-        }[ios]
-        AlteraPlatform.__init__(self, "5CEBA4F23C8", _io, _connectors, toolchain=toolchain)
+class Platform(XilinxUSPlatform):
+    default_clk_name   = "clk200"
+    default_clk_period = 1e9/200e6
+
+    def __init__(self, toolchain="vivado"):
+        XilinxUSPlatform.__init__(self, "xcku040-ffva1156-2-e", _io, toolchain=toolchain)
 
     def create_programmer(self):
-        return OpenFPGALoader(cable="usb-blaster")
+        return VivadoProgrammer()
 
     def do_finalize(self, fragment):
-        AlteraPlatform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk74a", loose=True), 1e9/74.25e6)
-        self.add_period_constraint(self.lookup_request("clk74b", loose=True), 1e9/74.25e6)
+        XilinxUSPlatform.do_finalize(self, fragment)
+        self.add_period_constraint(self.lookup_request("clk24",  loose=True), 1e9/24e6)
+        self.add_period_constraint(self.lookup_request("clk200", loose=True), 1e9/200e6)
+        self.add_platform_command("set_property INTERNAL_VREF 0.75 [get_iobanks 44]")
+        self.add_platform_command("set_property INTERNAL_VREF 0.75 [get_iobanks 45]")
+        self.add_platform_command("set_property INTERNAL_VREF 0.75 [get_iobanks 46]")
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/antmicro_artix_dc_scm.py` & `litex-boards-2023.8/litex_boards/platforms/antmicro_artix_dc_scm.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/antmicro_datacenter_ddr4_test_board.py` & `litex-boards-2023.8/litex_boards/platforms/antmicro_datacenter_ddr4_test_board.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/antmicro_lpddr4_test_board.py` & `litex-boards-2023.8/litex_boards/platforms/antmicro_lpddr4_test_board.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/antmicro_sdi_mipi_video_converter.py` & `litex-boards-2023.8/litex_boards/platforms/antmicro_sdi_mipi_video_converter.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/arduino_mkrvidor4000.py` & `litex-boards-2023.8/litex_boards/platforms/arduino_mkrvidor4000.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/avalanche.py` & `litex-boards-2023.8/litex_boards/platforms/avalanche.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/avnet_aesku40.py` & `litex-boards-2023.8/litex_boards/platforms/avnet_aesku40.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/berkeleylab_marble.py` & `litex-boards-2023.8/litex_boards/platforms/berkeleylab_marble.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/berkeleylab_marblemini.py` & `litex-boards-2023.8/litex_boards/platforms/berkeleylab_marblemini.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/camlink_4k.py` & `litex-boards-2023.8/litex_boards/platforms/camlink_4k.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/colorlight_5a_75b.py` & `litex-boards-2023.8/litex_boards/platforms/colorlight_5a_75b.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/colorlight_5a_75e.py` & `litex-boards-2023.8/litex_boards/platforms/colorlight_5a_75e.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/colorlight_i5.py` & `litex-boards-2023.8/litex_boards/platforms/colorlight_i5.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/colorlight_i5a_907.py` & `litex-boards-2023.8/litex_boards/platforms/colorlight_i5a_907.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/colorlight_i9plus.py` & `litex-boards-2023.8/litex_boards/platforms/colorlight_i9plus.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/decklink_intensity_pro_4k.py` & `litex-boards-2023.8/litex_boards/platforms/decklink_intensity_pro_4k.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/decklink_mini_4k.py` & `litex-boards-2023.8/litex_boards/platforms/decklink_mini_4k.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/decklink_quad_hdmi_recorder.py` & `litex-boards-2023.8/litex_boards/platforms/lambdaconcept_ecpix5.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,183 +1,185 @@
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2021 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2020-2022 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from litex.build.generic_platform import *
-from litex.build.xilinx import XilinxUSPlatform, VivadoProgrammer
+from litex.build.lattice import LatticeECP5Platform
+from litex.build.openfpgaloader import OpenFPGALoader
 
 # IOs ----------------------------------------------------------------------------------------------
 
 _io = [
-    # Clk / Rst.
-    # TODO: Document SI5338A.
-    ("clk24",  0, Pins("P26"),  IOStandard("LVCMOS15")),
-    ("clk200", 0,
-        Subsignal("p", Pins("AJ29"), IOStandard("LVDS")),
-        Subsignal("n", Pins("AK30"), IOStandard("LVDS"))
-    ),
-    ("clk",   0, Pins("AJ29"), IOStandard("LVCMOS15")),
-    ("clk",   0, Pins("AK30"), IOStandard("LVCMOS15")),
-
-    # Debug.
-    ("debug", 0, Pins("AL34"), IOStandard("LVCMOS15")),
-    ("debug", 1, Pins("AM34"), IOStandard("LVCMOS15")),
-    ("debug", 2, Pins("AN34"), IOStandard("LVCMOS15")),
-    ("debug", 3, Pins("AP34"), IOStandard("LVCMOS15")),
-
+    # Clk / Rst
+    ("clk100", 0, Pins("K23"), IOStandard("LVCMOS33")),
+    ("rst_n",  0, Pins("N5"),  IOStandard("LVCMOS33")),
+
+    # Leds
+    ("rgb_led", 0,
+        Subsignal("r", Pins("P21")),
+        Subsignal("g", Pins("R23")),
+        Subsignal("b", Pins("P22")),
+        IOStandard("LVCMOS33"),
+    ),
+    ("rgb_led", 1,
+        Subsignal("r", Pins("K21")),
+        Subsignal("g", Pins("K24")),
+        Subsignal("b", Pins("M21")),
+        IOStandard("LVCMOS33"),
+    ),
+    ("rgb_led", 2,
+        Subsignal("r", Pins("U21")),
+        Subsignal("g", Pins("W21")),
+        Subsignal("b", Pins("T24")),
+        IOStandard("LVCMOS33"),
+    ),
+    ("rgb_led", 3,
+        Subsignal("r", Pins("T23")),
+        Subsignal("g", Pins("R21")),
+        Subsignal("b", Pins("T22")),
+        IOStandard("LVCMOS33"),
+    ),
 
     # Serial
     ("serial", 0,
-        Subsignal("tx", Pins("AP9")),
-        Subsignal("rx", Pins("AN9")),
-        IOStandard("LVCMOS15")
-    ),
-
-    # SPIFlash (MX25L25645GSXDI).
-
-    # TODO (Probably similar to KCU105).
-
-    # PCIe
-    ("pcie_x1", 0,
-        #Subsignal("rst_n", Pins(""), IOStandard("")),
-        Subsignal("clk_p", Pins("AB6")),
-        Subsignal("clk_n", Pins("AB5")),
-        Subsignal("rx_p",  Pins("AB2")),
-        Subsignal("rx_n",  Pins("AB1")),
-        Subsignal("tx_p",  Pins("AC4")),
-        Subsignal("tx_n",  Pins("AC3"))
-    ),
-    ("pcie_x2", 0,
-        #Subsignal("rst_n", Pins(""), IOStandard("")),
-        Subsignal("clk_p", Pins("AB6")),
-        Subsignal("clk_n", Pins("AB5")),
-        Subsignal("rx_p",  Pins("AB2 AD2")),
-        Subsignal("rx_n",  Pins("AB1 AD1")),
-        Subsignal("tx_p",  Pins("AC4 AE4")),
-        Subsignal("tx_n",  Pins("AC3 AE3"))
-    ),
-    ("pcie_x4", 0,
-        #Subsignal("rst_n", Pins(""), IOStandard("")),
-        Subsignal("clk_p", Pins("AB6")),
-        Subsignal("clk_n", Pins("AB5")),
-        Subsignal("rx_p",  Pins("AB2 AD2 AF2 AH2")),
-        Subsignal("rx_n",  Pins("AB1 AD1 AF1 AH1")),
-        Subsignal("tx_p",  Pins("AC4 AE4 AG4 AH6")),
-        Subsignal("tx_n",  Pins("AC3 AE3 AG3 AH5"))
-    ),
-    ("pcie_x8", 0,
-        #Subsignal("rst_n", Pins(""), IOStandard("")),
-        Subsignal("clk_p", Pins("AB6")),
-        Subsignal("clk_n", Pins("AB5")),
-        Subsignal("rx_p",  Pins("AB2 AD2 AF2 AH2 AJ4 AK2 AM2 AP2")),
-        Subsignal("rx_n",  Pins("AB1 AD1 AF1 AH1 AJ3 AK1 AM1 AP1")),
-        Subsignal("tx_p",  Pins("AC4 AE4 AG4 AH6 AK6 AL4 AM6 AN4")),
-        Subsignal("tx_n",  Pins("AC3 AE3 AG3 AH5 AK5 AL3 AM5 AN3"))
+        Subsignal("rx", Pins("R26"), IOStandard("LVCMOS33")),
+        Subsignal("tx", Pins("R24"), IOStandard("LVCMOS33")),
     ),
 
-    # DDR3 SDRAM (H5TQ4G63CFR).
+    # DDR3 SDRAM
     ("ddram", 0,
         Subsignal("a", Pins(
-            "AP16 AM19 AL17 AM14 AL19 AL14 AJ18 AK16",
-            "AJ19 AK17 AP18 AM17 AL18 AH17 AH14"),
-            IOStandard("SSTL15_DCI")),
-        Subsignal("ba",    Pins("AN14 AN19 AP14"), IOStandard("SSTL15_DCI")),
-        Subsignal("ras_n", Pins("AN16"), IOStandard("SSTL15_DCI")),
-        Subsignal("cas_n", Pins("AM16"), IOStandard("SSTL15_DCI")),
-        Subsignal("we_n",  Pins("AP15"), IOStandard("SSTL15_DCI")),
-        Subsignal("cs_n",  Pins("AM15"), IOStandard("SSTL15_DCI")),
-        Subsignal("dm", Pins("AH26 AN26 AJ21 AM21 AH18 AE25 AD21 AD19"),
-            IOStandard("SSTL15_DCI"),
-            Misc("DATA_RATE=DDR")),
+            "T5 M3 L3 V6 K2 W6 K3 L1",
+            "H2 L2 N1 J1 M1 K1 H1"),
+            IOStandard("SSTL15_I")),
+        Subsignal("ba",    Pins("U6 N3 N4"), IOStandard("SSTL15_I")),
+        Subsignal("ras_n", Pins("T3"), IOStandard("SSTL15_I")),
+        Subsignal("cas_n", Pins("P2"), IOStandard("SSTL15_I")),
+        Subsignal("we_n",  Pins("R3"), IOStandard("SSTL15_I")),
+        Subsignal("dm", Pins("U4 U1"), IOStandard("SSTL15_I")),
         Subsignal("dq", Pins(
-            "AM27 AK28 AH27 AJ28 AK26 AH28 AM26 AK27",
-            "AP29 AP28 AM30 AN27 AM29 AN28 AL30 AL29",
-            "AM20 AK22 AL20 AL22 AL23 AL24 AK23 AL25",
-            "AP25 AM24 AN24 AM22 AN23 AN22 AP24 AP23",
-            "AJ16 AG17 AG15 AG19 AH16 AH19 AG14 AG16",
-            "AJ24 AG24 AJ23 AF23 AH22 AF24 AH23 AG25",
-            "AE20 AF20 AD20 AG20 AE22 AE23 AF22 AG22",
-            "AF18 AD15 AF17 AE17 AF14 AE18 AF15 AD16"),
-            IOStandard("SSTL15_DCI"),
-            Misc("ODT=RTT_40"),
-            Misc("DATA_RATE=DDR")),
-        Subsignal("dqs_p", Pins("AL27 AN29 AJ20 AP20 AJ15 AH24 AG21 AE16"),
-            IOStandard("DIFF_SSTL15_DCI"),
-            Misc("ODT=RTT_40"),
-            Misc("DATA_RATE=DDR")),
-        Subsignal("dqs_n", Pins("AL28 AP30 AK20 AP21 AJ14 AJ25 AH21 AE15"),
-            IOStandard("DIFF_SSTL15_DCI"),
-             Misc("ODT=RTT_40"),
-            Misc("DATA_RATE=DDR")),
-        Subsignal("clk_p", Pins("AN18"), IOStandard("DIFF_SSTL15_DCI"), Misc("DATA_RATE=DDR")),
-        Subsignal("clk_n", Pins("AN17"), IOStandard("DIFF_SSTL15_DCI"), Misc("DATA_RATE=DDR")),
-        Subsignal("cke",   Pins("AK18"), IOStandard("SSTL15_DCI")),
-        Subsignal("odt",   Pins("AL15"), IOStandard("SSTL15_DCI")),
-        Subsignal("reset_n", Pins("AK15"), IOStandard("SSTL15")),
-        Misc("SLEW=FAST"),
-        Misc("OUTPUT_IMPEDANCE=RDRV_40_40")
-    ),
-
-    # HDMI (through PI3HDX1204)
-    ("hdmi_in", 0, # PCIe Edge Side.
-        #Subsignal("clk_p",   Pins(""), IOStandard("")),
-        #Subsignal("clk_n",   Pins(""), IOStandard("")),
-        Subsignal("data0_p", Pins("Y2")),
-        Subsignal("data0_n", Pins("Y1")),
-        Subsignal("data1_p", Pins("V2")),
-        Subsignal("data1_n", Pins("V1")),
-        Subsignal("data2_p", Pins("T2")),
-        Subsignal("data2_n", Pins("T1")),
-    ),
-    ("hdmi_in", 1,
-        #Subsignal("clk_p",   Pins(""), IOStandard("")),
-        #Subsignal("clk_n",   Pins(""), IOStandard("")),
-        Subsignal("data0_p", Pins("P2")),
-        Subsignal("data0_n", Pins("P1")),
-        Subsignal("data1_p", Pins("M2")),
-        Subsignal("data1_n", Pins("M1")),
-        Subsignal("data2_p", Pins("K2")),
-        Subsignal("data2_n", Pins("K1")),
-    ),
-    ("hdmi_in", 2,
-        #Subsignal("clk_p",   Pins(""), IOStandard("")),
-        #Subsignal("clk_n",   Pins(""), IOStandard("")),
-        Subsignal("data0_p", Pins("H2")),
-        Subsignal("data0_n", Pins("H1")),
-        Subsignal("data1_p", Pins("F2")),
-        Subsignal("data1_n", Pins("F1")),
-        Subsignal("data2_p", Pins("E4")),
-        Subsignal("data2_n", Pins("E3")),
-    ),
-    ("hdmi_in", 3,
-        #Subsignal("clk_p",   Pins(""), IOStandard("")),
-        #Subsignal("clk_n",   Pins(""), IOStandard("")),
-        Subsignal("data0_p", Pins("D2")),
-        Subsignal("data0_n", Pins("D1")),
-        Subsignal("data1_p", Pins("B2")),
-        Subsignal("data1_n", Pins("B1")),
-        Subsignal("data2_p", Pins("B4")),
-        Subsignal("data2_n", Pins("B3")),
+            "T4 W4 R4 W5 R6 P6 P5 P4",
+            "R1 W3 T2 V3 U3 W1 T1 W2",),
+            IOStandard("SSTL15_I"),
+            Misc("TERMINATION=75")),
+        Subsignal("dqs_p", Pins("V4 V1"), IOStandard("SSTL15D_I"),
+            Misc("TERMINATION=OFF"),
+            Misc("DIFFRESISTOR=100")),
+        Subsignal("clk_p", Pins("H3"), IOStandard("SSTL15D_I")),
+        Subsignal("cke",   Pins("P1"), IOStandard("SSTL15_I")),
+        Subsignal("odt",   Pins("P3"), IOStandard("SSTL15_I")),
+        Misc("SLEWRATE=FAST"),
+    ),
+
+    # RGMII Ethernetx
+    ("eth_clocks", 0,
+        Subsignal("tx", Pins("A12")),
+        Subsignal("rx", Pins("E11")),
+        IOStandard("LVCMOS33")
+    ),
+    ("eth", 0,
+        Subsignal("rst_n",   Pins("C13")),
+        Subsignal("mdio",    Pins("A13")),
+        Subsignal("mdc",     Pins("C11")),
+        Subsignal("rx_ctl",  Pins("A11")),
+        Subsignal("rx_data", Pins("B11 A10 B10 A9"), Misc("PULLMODE=UP")), # RGMII mode - Advertise all capabilities.
+        Subsignal("tx_ctl",  Pins("C9")),
+        Subsignal("tx_data", Pins("D8 C8 B8 A8")),
+        IOStandard("LVCMOS33")
+    ),
+
+    # SDCard
+    ("sdcard", 0,
+        Subsignal("data",      Pins("N26 N25 N23 N21"), Misc("PULLMODE=UP")),
+        Subsignal("cmd",       Pins("M24"),             Misc("PULLMODE=UP")),
+        Subsignal("clk",       Pins("P24")),
+        Subsignal("cd",        Pins("L22")),
+        Subsignal("cmd_dir",   Pins("M23")),
+        Subsignal("dat0_dir",  Pins("N24")),
+        Subsignal("dat13_dir", Pins("P26")),
+        IOStandard("LVCMOS33"),
+    ),
+
+    # Sata
+    ("sata", 0,
+        Subsignal("clk_p", Pins("AF12")),
+        Subsignal("clk_n", Pins("AF13")),
+        Subsignal("rx_p", Pins("AF15")),
+        Subsignal("rx_n", Pins("AF16")),
+        Subsignal("tx_p", Pins("AD16")),
+        Subsignal("tx_n", Pins("AD17")),
+        IOStandard("LVCMOS33"),
+    ),
+
+    # SPIFlash
+    ("spiflash", 0,
+        Subsignal("cs_n", Pins("AA2")),
+        Subsignal("mosi", Pins("AE2")),
+        Subsignal("miso", Pins("AD2")),
+        Subsignal("wp", Pins("AF2")),
+        Subsignal("hold", Pins("AE1")),
+        IOStandard("LVCMOS33")
+    ),
+    ("spiflash4x", 0,
+        Subsignal("cs_n", Pins("AA2")),
+        Subsignal("dq", Pins("AE2", "AD2", "AF2", "AE1")),
+        IOStandard("LVCMOS33")
+    ),
+
+    # USB
+    ("ulpi", 0,
+        Subsignal("rst",  Pins("E23")),
+        Subsignal("clk",  Pins("H24")),
+        Subsignal("dir",  Pins("F22")),
+        Subsignal("nxt",  Pins("F23")),
+        Subsignal("stp",  Pins("H23")),
+        Subsignal("data", Pins("M26 L25 L26 K25 K26 J23 P25 H25")),
+        IOStandard("LVCMOS33")
+    ),
+
+    # HDMI / IT6613
+    ("hdmi", 0,
+        Subsignal("r", Pins("AD26 AE25 AF25 AE26 E10 D11 D10 C10  D9  E8 H5 J4")),
+        Subsignal("g", Pins("AA23 AA22 AA24 AA25  E1  F2  F1 D17 D16 E16 J6 H6")),
+        Subsignal("b", Pins("AD25 AC26 AB24 AB25  B3  C3  D3  B1  C2  D2 D1 E3")),
+        Subsignal("de",    Pins("A3")),
+        Subsignal("clk",   Pins("C1")),
+        Subsignal("vsync", Pins("A4")),
+        Subsignal("hsync", Pins("B4")),
+        Subsignal("sda", Pins("E17")),
+        Subsignal("scl", Pins("C17")),
+        IOStandard("LVCMOS33")
     ),
 ]
 
-# Platform -----------------------------------------------------------------------------------------
+# Connectors ---------------------------------------------------------------------------------------
 
-class Platform(XilinxUSPlatform):
-    default_clk_name   = "clk200"
-    default_clk_period = 1e9/200e6
+_connectors = [
+    ("pmod0", "T25 U25 U24 V24 T26 U26 V26 W26"),
+    ("pmod1", "U23 V23 U22 V21 W25 W24 W23 W22"),
+    ("pmod2", "J24 H22 E21 D18 K22 J21 H21 D22"),
+    ("pmod3", "E4 F4 E6 H4 F3 D4 D5 F5"),
+    ("pmod4", "E26 D25 F26 F25 C26 C25 A25 A24"),
+    ("pmod5", "D19 C21 B21 C22 D21 A21 A22 A23"),
+    ("pmod6", "C16 B17 C18 B19 A17 A18 A19 C19"),
+    ("pmod7", "D14 B14 E14 B16 C14 A14 A15 A16"),
+]
+
+# Platform -----------------------------------------------------------------------------------------
 
-    def __init__(self, toolchain="vivado"):
-        XilinxUSPlatform.__init__(self, "xcku040-ffva1156-2-e", _io, toolchain=toolchain)
+class Platform(LatticeECP5Platform):
+    default_clk_name   = "clk100"
+    default_clk_period = 1e9/100e6
+
+    def __init__(self, device="85F", toolchain="trellis", **kwargs):
+        assert device in ["45F", "85F"]
+        LatticeECP5Platform.__init__(self, f"LFE5UM5G-{device}-8BG554I", _io, _connectors, toolchain=toolchain, **kwargs)
 
     def create_programmer(self):
-        return VivadoProgrammer()
+        return OpenFPGALoader("ecpix5")
 
     def do_finalize(self, fragment):
-        XilinxUSPlatform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk24",  loose=True), 1e9/24e6)
-        self.add_period_constraint(self.lookup_request("clk200", loose=True), 1e9/200e6)
-        self.add_platform_command("set_property INTERNAL_VREF 0.75 [get_iobanks 44]")
-        self.add_platform_command("set_property INTERNAL_VREF 0.75 [get_iobanks 45]")
-        self.add_platform_command("set_property INTERNAL_VREF 0.75 [get_iobanks 46]")
+        LatticeECP5Platform.do_finalize(self, fragment)
+        self.add_period_constraint(self.lookup_request("clk100", loose=True), 1e9/100e6)
+        self.add_period_constraint(self.lookup_request("eth_clocks:rx", 0, loose=True), 1e9/125e6)
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/digilent_arty.py` & `litex-boards-2023.8/litex_boards/platforms/digilent_arty.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/digilent_arty_s7.py` & `litex-boards-2023.8/litex_boards/platforms/digilent_arty_s7.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/digilent_arty_z7.py` & `litex-boards-2023.8/litex_boards/platforms/digilent_arty_z7.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/digilent_atlys.py` & `litex-boards-2023.8/litex_boards/platforms/digilent_atlys.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/digilent_basys3.py` & `litex-boards-2023.8/litex_boards/platforms/digilent_basys3.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/digilent_cmod_a7.py` & `litex-boards-2023.8/litex_boards/platforms/digilent_cmod_a7.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/digilent_genesys2.py` & `litex-boards-2023.8/litex_boards/platforms/digilent_genesys2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/digilent_nexys4.py` & `litex-boards-2023.8/litex_boards/platforms/digilent_nexys4.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/digilent_nexys4ddr.py` & `litex-boards-2023.8/litex_boards/platforms/digilent_nexys4ddr.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/digilent_nexys_video.py` & `litex-boards-2023.8/litex_boards/platforms/digilent_nexys_video.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/digilent_pynq_z1.py` & `litex-boards-2023.8/litex_boards/platforms/digilent_pynq_z1.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/digilent_zedboard.py` & `litex-boards-2023.8/litex_boards/platforms/digilent_zedboard.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/digilent_zybo_z7.py` & `litex-boards-2023.8/litex_boards/platforms/digilent_zybo_z7.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/ebaz4205.py` & `litex-boards-2023.8/litex_boards/platforms/ebaz4205.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/efinix_t8f81_dev_kit.py` & `litex-boards-2023.8/litex_boards/platforms/efinix_t8f81_dev_kit.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/efinix_titanium_ti60_f225_dev_kit.py` & `litex-boards-2023.8/litex_boards/platforms/efinix_titanium_ti60_f225_dev_kit.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/efinix_trion_t120_bga576_dev_kit.py` & `litex-boards-2023.8/litex_boards/platforms/efinix_trion_t120_bga576_dev_kit.py`

 * *Files 20% similar despite different names*

```diff
@@ -128,33 +128,14 @@
 _connectors = [
     ("pmod_a", " T12  V11  Y12  Y10  U12  U11  W12  Y11"),
     ("pmod_b", "AD11 AD10 AC10  W10 AA11 AC11 AA10  V10"),
     ("pmod_c", " A11  D11  J11  G10  B11  E11  H11  F10"),
     ("pmod_d", " D10  A10   A9   D9  E10  B10   B9   C9"),
     ("pmod_e", " C24  B23  A20  A22  B24  A23  B20  B22"),
     ("pmod_f", " V21  V20 AD20 AD19  U21  V19 AC20 AC19"),
-
-    ["P2",
-        "---", # 0
-        #                    GND   GND                      GND  GND                     GND  GND
-        "AA24  Y22  Y24 AA22 ---- ---- AC24  W22 AB24  V22 ---- ----  W24  T22  V24  R22 ---- ---- AB23  E19",
-        #   1    2    3    4    5    6    7    8    9   10   11   12   13   14   15   16   17   18   19   20
-        #  21   22   23   24   25   26   27   28   29   30   31   32   33   34   35   36   37   38   39   40
-        "AC23  D19 ----  ---  W23  A21  Y23  B21 ---- ----  U24  B19  U23  A19 ---- ---- AC22  G17 AD22  F17",
-        #           GND  GND                      GND  GND                      GND  GND
-    ],
-    ["P3",
-        "---", # 0
-        #                     GND  GND                      GND  GND        NC        NC  GND  GND        NC
-        " J16  B15  K16  A15 ---- ----  H15  B14  G15  A14 ---- ----  J14 ----  H14 ---- ---- ----  E15 ----",
-        #   1    2    3    4    5    6    7    8    9   10   11   12   13   14   15   16   17   18   19   20
-        #  21   22   23   24   25   26   27   28   28   30   31   32   33   34   35   36   37   38   39   40
-        " F15 ---- ----  ---  G16 ----  H16 ---- ---- ----  D15 ----  C15 ---- ---- ----  D16 ----  E16 ----",
-        #       NC  GND  GND        NC        NC  GND  GND        NC        NC  GND  GND        NC        NC
-    ],
 ]
 
 # PMODS --------------------------------------------------------------------------------------------
 
 def raw_pmod_io(pmod):
     return [(pmod, 0, Pins(" ".join([f"{pmod}:{i:d}" for i in range(8)])), IOStandard("3.3_V_LVTTL_/_LVCMOS"))]
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/efinix_trion_t20_bga256_dev_kit.py` & `litex-boards-2023.8/litex_boards/platforms/efinix_trion_t20_bga256_dev_kit.py`

 * *Files 23% similar despite different names*

```diff
@@ -65,24 +65,14 @@
             ("TL",       "1.2 V"),
             ("TR",       "1.2 V"),
 ]
 
 # Connectors ---------------------------------------------------------------------------------------
 
 _connectors = [
-    # LVDS RX
-    ["CON3", #   1   3 -   7   9  11  13 -  17  19  21  23 -  27  29  31  33
-             " M13 M12 - N13 P14 R15 T15 - N12 P12 R14 T14 - P13 R13 R12 T12",
-             #   2   4 -   8  10  12  14 -  18  20  22  24 -  28  30  32  34
-             " P11 N11 - M11 M10 R11 T11 - N10 P10 T10  T9 -  M9  N9  R9  P9"],
-    # LVDS TX
-    ["CON4", #  1  3 -  -  - 11 13 - 17 19 21 23 - 27 29 31 33
-             " P8 R8 -  -  - N8 M8 - T7 T8 P7 N7 - T6 R6 T5 R5",
-             #  2  4 -  8 10 12 14 - 18 20 22 24 - 28 30 32 34
-             " P6 N6 - M7 M6 P5 N5 - T3 T2 R4 R3 - P4 N4 M5 M4"],
     ["H4", # -  - 26 25 24 23 22 21 20 19 18 16 15 14 13 12 11
            " -  - H4 H2 H3 L1 H1 H5 J2 K2 K1 J3 K3 J4 L2 K4 J5",
            # - 27 28 29 30 31 32 33 34 35 36 37 39 40 41 42 43
            " - G3 G5 G2 F1 G1 F2 C1 E2 F3 D1 E1 E3 F5 C2 G4 F4"],
     ["H2", # - 45 47 49 51 53 55 57 59 61  - 63 65 67 69 71 73
            " - B2 D4 D5 C4 B4 E4 A3 A4 B5  - B7 A6 C5 D7 B8 D8",
            # - 44 46 48 50 52 54 56 58 60 62 64 66 68 70 72 74
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/efinix_trion_t20_mipi_dev_kit.py` & `litex-boards-2023.8/litex_boards/platforms/efinix_trion_t20_mipi_dev_kit.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/efinix_xyloni_dev_kit.py` & `litex-boards-2023.8/litex_boards/platforms/efinix_xyloni_dev_kit.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/ego1.py` & `litex-boards-2023.8/litex_boards/platforms/ego1.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/enclustra_mercury_kx2.py` & `litex-boards-2023.8/litex_boards/platforms/enclustra_mercury_kx2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/enclustra_mercury_xu5.py` & `litex-boards-2023.8/litex_boards/platforms/enclustra_mercury_xu5.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/enclustra_mercury_xu8_pe3.py` & `litex-boards-2023.8/litex_boards/platforms/enclustra_mercury_xu8_pe3.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/enclustra_st1.py` & `litex-boards-2023.8/litex_boards/platforms/enclustra_st1.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/fairwaves_xtrx.py` & `litex-boards-2023.8/litex_boards/platforms/fairwaves_xtrx.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/fpc_iii.py` & `litex-boards-2023.8/litex_boards/platforms/fpc_iii.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/fpgawars_alhambra2.py` & `litex-boards-2023.8/litex_boards/platforms/fpgawars_alhambra2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/gadgetfactory_papilio_pro.py` & `litex-boards-2023.8/litex_boards/platforms/gadgetfactory_papilio_pro.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/gsd_butterstick.py` & `litex-boards-2023.8/litex_boards/platforms/gsd_butterstick.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/gsd_orangecrab.py` & `litex-boards-2023.8/litex_boards/platforms/gsd_orangecrab.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/hackaday_hadbadge.py` & `litex-boards-2023.8/litex_boards/platforms/hackaday_hadbadge.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/ice_v_wireless.py` & `litex-boards-2023.8/litex_boards/platforms/ice_v_wireless.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/icebreaker.py` & `litex-boards-2023.8/litex_boards/platforms/icebreaker.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/icebreaker_bitsy.py` & `litex-boards-2023.8/litex_boards/platforms/icebreaker_bitsy.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/isx_im1283.py` & `litex-boards-2023.8/litex_boards/platforms/isx_im1283.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/jungle_electronics_fireant.py` & `litex-boards-2023.8/litex_boards/platforms/jungle_electronics_fireant.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/kosagi_fomu_evt.py` & `litex-boards-2023.8/litex_boards/platforms/kosagi_fomu_evt.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/kosagi_fomu_hacker.py` & `litex-boards-2023.8/litex_boards/platforms/kosagi_fomu_hacker.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/kosagi_fomu_pvt.py` & `litex-boards-2023.8/litex_boards/platforms/kosagi_fomu_pvt.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/kosagi_netv2.py` & `litex-boards-2023.8/litex_boards/platforms/numato_mimas_a7.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,208 +1,205 @@
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2019 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2018-2019 Rohit Singh <rohit@rohitksingh.in>
+# Copyright (c) 2020 Feliks Montez <feliks.montez@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from litex.build.generic_platform import *
 from litex.build.xilinx import Xilinx7SeriesPlatform
 from litex.build.openocd import OpenOCD
 
 # IOs ----------------------------------------------------------------------------------------------
 
 _io = [
     # Clk / Rst
-    ("clk50", 0, Pins("J19"), IOStandard("LVCMOS33")),
+    ("clk100", 0, Pins("H4"), IOStandard("LVCMOS33")),
+    ("cpu_reset", 0, Pins("M2"), IOStandard("LVCMOS33")),
 
     # Leds
-    ("user_led", 0, Pins("M21"),  IOStandard("LVCMOS33")),
-    ("user_led", 1, Pins("N20"),  IOStandard("LVCMOS33")),
-    ("user_led", 2, Pins("L21"),  IOStandard("LVCMOS33")),
-    ("user_led", 3, Pins("AA21"), IOStandard("LVCMOS33")),
-    ("user_led", 4, Pins("R19"),  IOStandard("LVCMOS33")),
-    ("user_led", 5, Pins("M16"),  IOStandard("LVCMOS33")),
+    ("user_led", 0, Pins("K17"), IOStandard("LVCMOS33")),
+    ("user_led", 1, Pins("J17"), IOStandard("LVCMOS33")),
+    ("user_led", 2, Pins("L14"), IOStandard("LVCMOS33")),
+    ("user_led", 3, Pins("L15"), IOStandard("LVCMOS33")),
+    ("user_led", 4, Pins("L16"), IOStandard("LVCMOS33")),
+    ("user_led", 5, Pins("K16"), IOStandard("LVCMOS33")),
+    ("user_led", 6, Pins("M15"), IOStandard("LVCMOS33")),
+    ("user_led", 7, Pins("M16"), IOStandard("LVCMOS33")),
+
+    # Switches
+    ("user_sw", 0, Pins("B21"), IOStandard("LVCMOS33")),
+    ("user_sw", 1, Pins("A21"), IOStandard("LVCMOS33")),
+    ("user_sw", 2, Pins("E22"), IOStandard("LVCMOS33")),
+    ("user_sw", 3, Pins("D22"), IOStandard("LVCMOS33")),
+    ("user_sw", 4, Pins("E21"), IOStandard("LVCMOS33")),
+    ("user_sw", 5, Pins("D21"), IOStandard("LVCMOS33")),
+    ("user_sw", 6, Pins("G21"), IOStandard("LVCMOS33")),
+    ("user_sw", 7, Pins("G22"), IOStandard("LVCMOS33")),
+
+    # Buttons
+    ("user_btn", 0, Pins("P20"), IOStandard("LVCMOS33")),
+    ("user_btn", 1, Pins("P19"), IOStandard("LVCMOS33")),
+    ("user_btn", 2, Pins("P17"), IOStandard("LVCMOS33")),
+    ("user_btn", 3, Pins("N17"), IOStandard("LVCMOS33")),
+
+    # Serial
+    ("serial", 0, # Can be used when FT2232H's Channel A configured to ASYNC Serial (UART) mode
+        Subsignal("tx", Pins("Y21")),
+        Subsignal("rx", Pins("Y22")),
+        IOStandard("LVCMOS33")
+    ),
+
+    # USB FIFO
+    ("usb_fifo", 0, # Can be used when FT2232H's Channel A configured to ASYNC FIFO 245 mode
+        Subsignal("data",  Pins("Y22 Y21 AB22 AA21 AB21 AA20 AB20 AA18")),
+        Subsignal("rxf_n", Pins("W21")),
+        Subsignal("txe_n", Pins("V22")),
+        Subsignal("rd_n",  Pins("AA19")),
+        Subsignal("wr_n",  Pins("W22")),
+        Subsignal("siwua", Pins("U21")),
+        Subsignal("oe_n",  Pins("T21")),
+        Misc("SLEW=FAST"),
+        Drive(8),
+        IOStandard("LVCMOS33"),
+    ),
 
     # SPIFlash
     ("spiflash", 0,
         Subsignal("cs_n", Pins("T19")),
+        Subsignal("clk",  Pins("L12")),
         Subsignal("mosi", Pins("P22")),
         Subsignal("miso", Pins("R22")),
-        Subsignal("vpp",  Pins("P21")),
+        Subsignal("wp",   Pins("P21")),
         Subsignal("hold", Pins("R21")),
-        IOStandard("LVCMOS33")
+        IOStandard("LVCMOS33"),
     ),
     ("spiflash4x", 0,
         Subsignal("cs_n", Pins("T19")),
-        Subsignal("dq",   Pins("P22 R22 P21 R21")),
+        Subsignal("clk",  Pins("L12")),
+        Subsignal("dq",   Pins("P22", "R22", "P21", "R21")),
         IOStandard("LVCMOS33")
     ),
 
-    # Serial
-    ("serial", 0,
-        Subsignal("tx", Pins("E14")),
-        Subsignal("rx", Pins("E13")),
-        IOStandard("LVCMOS33"),
-    ),
-
     # DDR3 SDRAM
     ("ddram", 0,
         Subsignal("a", Pins(
-            "U6 V4 W5 V5 AA1 Y2 AB1 AB3",
-            "AB2 Y3 W6 Y1 V2 AA3"),
-            IOStandard("SSTL15_R")),
-        Subsignal("ba",    Pins("U5 W4 V7"), IOStandard("SSTL15_R")),
-        Subsignal("ras_n", Pins("Y9"), IOStandard("SSTL15_R")),
-        Subsignal("cas_n", Pins("Y7"), IOStandard("SSTL15_R")),
-        Subsignal("we_n",  Pins("V8"), IOStandard("SSTL15_R")),
-        Subsignal("dm", Pins("G1 H4 M5 L3"), IOStandard("SSTL15_R")),
+            "U6 T5 Y6 T6 V2 T4 Y2 R2",
+            "Y1 R4 W5 W1 AA6 U2"),
+            IOStandard("SSTL15")),
+        Subsignal("ba",    Pins("W6 U5 R6"), IOStandard("SSTL15")),
+        Subsignal("ras_n", Pins("V5"),  IOStandard("SSTL15")),
+        Subsignal("cas_n", Pins("T1"),  IOStandard("SSTL15")),
+        Subsignal("we_n",  Pins("R3"),  IOStandard("SSTL15")),
+        Subsignal("dm", Pins("Y7 AA1"), IOStandard("SSTL15")),
         Subsignal("dq", Pins(
-            "C2 F1 B1 F3 A1 D2 B2 E2",
-            "J5 H3 K1 H2 J1 G2 H5 G3",
-            "N2 M6 P1 N5 P2 N4 R1 P6",
-            "K3 M2 K4 M3 J6 L5 J4 K6"),
-            IOStandard("SSTL15_R"),
+            "Y8 AB6 W9  AA8 AB7 V7 AB8 W7",
+            "V4 AB2 AA5 AB3 AB5 W4 AB1 AA4"),
+            IOStandard("SSTL15"),
             Misc("IN_TERM=UNTUNED_SPLIT_40")),
-        Subsignal("dqs_p", Pins("E1 K2 P5 M1"), IOStandard("DIFF_SSTL15_R")),
-        Subsignal("dqs_n", Pins("D1 J2 P4 L1"), IOStandard("DIFF_SSTL15_R")),
-        Subsignal("clk_p", Pins("R3"), IOStandard("DIFF_SSTL15_R")),
-        Subsignal("clk_n", Pins("R2"), IOStandard("DIFF_SSTL15_R")),
-        Subsignal("cke",   Pins("Y8"), IOStandard("SSTL15_R")),
-        Subsignal("odt",   Pins("W9"), IOStandard("SSTL15_R")),
-        Subsignal("reset_n", Pins("AB5"), IOStandard("LVCMOS15")),
-        Subsignal("cs_n", Pins("V9"), IOStandard("SSTL15_R")),
+        Subsignal("dqs_p", Pins("V9 Y3"),  IOStandard("DIFF_SSTL15")),
+        Subsignal("dqs_n", Pins("V8 AA3"), IOStandard("DIFF_SSTL15")),
+        Subsignal("clk_p", Pins("U3"), IOStandard("DIFF_SSTL15")),
+        Subsignal("clk_n", Pins("V3"), IOStandard("DIFF_SSTL15")),
+        Subsignal("cke",   Pins("U1"), IOStandard("SSTL15")),
+        Subsignal("odt",   Pins("W2"), IOStandard("SSTL15")),
+        Subsignal("cs_n",  Pins("T3"), IOStandard("SSTL15")),
+        Subsignal("reset_n", Pins("U7"), IOStandard("SSTL15")),
         Misc("SLEW=FAST"),
     ),
 
-    # PCIe
-    ("pcie_x1", 0,
-        Subsignal("rst_n", Pins("E18"), IOStandard("LVCMOS33")),
-        Subsignal("clk_p", Pins("F10")),
-        Subsignal("clk_n", Pins("E10")),
-        Subsignal("rx_p",  Pins("D11")),
-        Subsignal("rx_n",  Pins("C11")),
-        Subsignal("tx_p",  Pins("D5")),
-        Subsignal("tx_n",  Pins("C5"))
-    ),
-    ("pcie_x2", 0,
-        Subsignal("rst_n", Pins("E18"), IOStandard("LVCMOS33")),
-        Subsignal("clk_p", Pins("F10")),
-        Subsignal("clk_n", Pins("E10")),
-        Subsignal("rx_p",  Pins("D11 B10")),
-        Subsignal("rx_n",  Pins("C11 A10")),
-        Subsignal("tx_p",  Pins("D5 B6")),
-        Subsignal("tx_n",  Pins("C5 A6"))
-    ),
-    ("pcie_x4", 0,
-        Subsignal("rst_n", Pins("E18"), IOStandard("LVCMOS33")),
-        Subsignal("clk_p", Pins("F10")),
-        Subsignal("clk_n", Pins("E10")),
-        Subsignal("rx_p",  Pins("D11 B10 D9 B8")),
-        Subsignal("rx_n",  Pins("C11 A10 C9 A8")),
-        Subsignal("tx_p",  Pins("D5 B6 D7 B4")),
-        Subsignal("tx_n",  Pins("C5 A6 C7 A4"))
+    # I2C EEPROM
+    ("eeprom", 0,
+        Subsignal("scl", Pins("N5")),
+        Subsignal("sda", Pins("P6")),
+        IOStandard("LVCMOS33")
     ),
 
-    # RMII Ethernet
+    # RGMII Ethernet
     ("eth_clocks", 0,
-        Subsignal("ref_clk", Pins("D17")),
-        IOStandard("LVCMOS33"),
+        Subsignal("tx", Pins("U20")),
+        Subsignal("rx", Pins("W19")),
+        IOStandard("LVCMOS33")
     ),
     ("eth", 0,
-        Subsignal("rst_n",   Pins("F16")),
-        Subsignal("rx_data", Pins("A20 B18")),
-        Subsignal("crs_dv",  Pins("C20")),
-        Subsignal("tx_en",   Pins("A19")),
-        Subsignal("tx_data", Pins("C18 C19")),
-        Subsignal("mdc",     Pins("F14")),
-        Subsignal("mdio",    Pins("F13")),
-        Subsignal("rx_er",   Pins("B20")),
-        Subsignal("int_n",   Pins("D21")),
-        IOStandard("LVCMOS33")
-     ),
-
-     # SDCard
-    ("spisdcard", 0,
-        Subsignal("clk",  Pins("K18")),
-        Subsignal("cs_n", Pins("M13")),
-        Subsignal("mosi", Pins("L13"), Misc("PULLUP")),
-        Subsignal("miso", Pins("L15"), Misc("PULLUP")),
-        Misc("SLEW=FAST"),
+        Subsignal("rst_n",   Pins("R14"), IOStandard("LVCMOS33")),
+        Subsignal("int_n",   Pins("V19")),
+        Subsignal("mdio",    Pins("P16")),
+        Subsignal("mdc",     Pins("R19")),
+        Subsignal("rx_ctl",  Pins("Y19")),
+        Subsignal("rx_data", Pins("AB18 W20 W17 V20")),
+        Subsignal("tx_ctl",  Pins("T20")),
+        Subsignal("tx_data", Pins("V18 U18 V17 U17")),
         IOStandard("LVCMOS33")
     ),
-    ("sdcard", 0,
-        Subsignal("clk",  Pins("K18")),
-        Subsignal("cmd",  Pins("L13"), Misc("PULLUP True")),
-        Subsignal("data", Pins("L15 L16 K14 M13"), Misc("PULLUP True")),
-        IOStandard("LVCMOS33"), Misc("SLEW=FAST")
-    ),
 
     # HDMI In
     ("hdmi_in", 0,
-        Subsignal("clk_p",   Pins("L19"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("clk_n",   Pins("L20"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data0_p", Pins("K21"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data0_n", Pins("K22"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data1_p", Pins("J20"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data1_n", Pins("J21"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data2_p", Pins("J22"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data2_n", Pins("H22"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("scl",     Pins("T18"), IOStandard("LVCMOS33")),
-        Subsignal("sda",     Pins("V18"), IOStandard("LVCMOS33")),
-    ),
-    ("hdmi_in", 1,
-        Subsignal("clk_p",   Pins("Y18"),  IOStandard("TMDS_33"), Inverted()),
-        Subsignal("clk_n",   Pins("Y19"),  IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data0_p", Pins("AA18"), IOStandard("TMDS_33")),
-        Subsignal("data0_n", Pins("AB18"), IOStandard("TMDS_33")),
-        Subsignal("data1_p", Pins("AA19"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data1_n", Pins("AB20"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data2_p", Pins("AB21"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data2_n", Pins("AB22"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("scl",     Pins("W17"),  IOStandard("LVCMOS33"), Inverted()),
-        Subsignal("sda",     Pins("R17"),  IOStandard("LVCMOS33")),
+        Subsignal("clk_p",   Pins("K4"), IOStandard("TMDS_33")),
+        Subsignal("clk_n",   Pins("J4"), IOStandard("TMDS_33")),
+        Subsignal("data0_p", Pins("K1"), IOStandard("TMDS_33")),
+        Subsignal("data0_n", Pins("J1"), IOStandard("TMDS_33")),
+        Subsignal("data1_p", Pins("M1"), IOStandard("TMDS_33")),
+        Subsignal("data1_n", Pins("L1"), IOStandard("TMDS_33")),
+        Subsignal("data2_p", Pins("P2"), IOStandard("TMDS_33")),
+        Subsignal("data2_n", Pins("N2"), IOStandard("TMDS_33")),
+        Subsignal("scl",     Pins("J2"), IOStandard("LVCMOS33")),
+        Subsignal("sda",     Pins("H2"), IOStandard("LVCMOS33")),
+        Subsignal("hpd_en",  Pins("G2"), IOStandard("LVCMOS33")),
+        Subsignal("cec",     Pins("K2"), IOStandard("LVCMOS33")), # FIXME
+        # Subsignal("txen", Pins("R3"), IOStandard("LVCMOS33")),  # FIXME
     ),
 
     # HDMI Out
     ("hdmi_out", 0,
-        Subsignal("clk_p",   Pins("W19"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("clk_n",   Pins("W20"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data0_p", Pins("W21"), IOStandard("TMDS_33")),
-        Subsignal("data0_n", Pins("W22"), IOStandard("TMDS_33")),
-        Subsignal("data1_p", Pins("U20"), IOStandard("TMDS_33")),
-        Subsignal("data1_n", Pins("V20"), IOStandard("TMDS_33")),
-        Subsignal("data2_p", Pins("T21"), IOStandard("TMDS_33")),
-        Subsignal("data2_n", Pins("U21"), IOStandard("TMDS_33"))
-    ),
-    ("hdmi_out", 1,
-        Subsignal("clk_p",   Pins("G21"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("clk_n",   Pins("G22"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data0_p", Pins("E22"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data0_n", Pins("D22"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data1_p", Pins("C22"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data1_n", Pins("B22"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data2_p", Pins("B21"), IOStandard("TMDS_33"), Inverted()),
-        Subsignal("data2_n", Pins("A21"), IOStandard("TMDS_33"), Inverted()),
+        Subsignal("clk_p",   Pins("L3"), IOStandard("TMDS_33")),
+        Subsignal("clk_n",   Pins("K3"), IOStandard("TMDS_33")),
+        Subsignal("data0_p", Pins("B1"), IOStandard("TMDS_33")),
+        Subsignal("data0_n", Pins("A1"), IOStandard("TMDS_33")),
+        Subsignal("data1_p", Pins("E1"), IOStandard("TMDS_33")),
+        Subsignal("data1_n", Pins("D1"), IOStandard("TMDS_33")),
+        Subsignal("data2_p", Pins("G1"), IOStandard("TMDS_33")),
+        Subsignal("data2_n", Pins("F1"), IOStandard("TMDS_33")),
+        Subsignal("scl",     Pins("D2"), IOStandard("LVCMOS33")),
+        Subsignal("sda",     Pins("C2"), IOStandard("LVCMOS33")),
+        Subsignal("cec",     Pins("E2"), IOStandard("LVCMOS33")), # FIXME
+        Subsignal("hdp",     Pins("B2"), IOStandard("LVCMOS33")), # FIXME
     ),
 ]
 
+# Connectors ---------------------------------------------------------------------------------------
+
+_connectors = [
+    ("P12", "J20 J21 K21 K22 H20 G20 J19 H19",
+            "J22 H22 K18 K19 L19 L20 M21 N22",
+            "N20 M20 M18 L18 N18 N19 H17 H18",
+            "G17 G18 G15 G16 J15 H15 K13 K14",
+            "M13 K14 M13 L13 J14 H14 H13 G13"),
+    ("P13", "F19 F20 E19 D19 D20 C20 C22 B22",
+            "F18 E18 C18 C19 D17 C17 B20 A20",
+            "B17 B18 A18 A19 E16 D16 B15 B16",
+            "A15 A16 C14 C15 A13 A14 C13 B13",
+            "D14 D15 E13 E14 F13 F14 F16 E17")
+]
+
 # Platform -----------------------------------------------------------------------------------------
 
 class Platform(Xilinx7SeriesPlatform):
-    default_clk_name   = "clk50"
-    default_clk_period = 1e9/50e6
+    default_clk_name   = "clk100"
+    default_clk_period = 1e9/100e6
 
-    def __init__(self, variant="a7-35", toolchain="vivado"):
-        device = {
-            "a7-35":  "xc7a35t-fgg484-2",
-            "a7-100": "xc7a100t-fgg484-2"
-        }[variant]
-        Xilinx7SeriesPlatform.__init__(self, device, _io, toolchain=toolchain)
+    def __init__(self, toolchain="vivado"):
+        Xilinx7SeriesPlatform.__init__(self, "xc7a50tfgg484-1", _io, _connectors, toolchain=toolchain)
+        self.toolchain.bitstream_commands = \
+            ["set_property BITSTREAM.CONFIG.SPI_BUSWIDTH 4 [current_design]"]
+        self.toolchain.additional_commands = \
+            ["write_cfgmem -force -format bin -interface spix4 -size 16 "
+             "-loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin"]
+        self.add_platform_command("set_property INTERNAL_VREF 0.675 [get_iobanks 34]")
 
     def create_programmer(self):
-        bscan_spi = "bscan_spi_xc7a100t.bit" if "xc7a100t" in self.device else "bscan_spi_xc7a35t.bit"
-        return OpenOCD("openocd_netv2_rpi.cfg", bscan_spi)
+        return OpenOCD("openocd_xc7_ft2232.cfg", "bscan_spi_xc7a50t.bit")
 
     def do_finalize(self, fragment):
         Xilinx7SeriesPlatform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk50",              loose=True), 1e9/50e6)
-        self.add_period_constraint(self.lookup_request("eth_clocks:ref_clk", loose=True), 1e9/50e6)
+        self.add_period_constraint(self.lookup_request("clk100",        loose=True), 1e9/100e6)
+        self.add_period_constraint(self.lookup_request("eth_clocks:rx", loose=True), 1e9/125e6)
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/krtkl_snickerdoodle.py` & `litex-boards-2023.8/litex_boards/platforms/krtkl_snickerdoodle.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/lambdaconcept_ecpix5.py` & `litex-boards-2023.8/litex_boards/platforms/scarabhardware_minispartan6.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,185 +1,167 @@
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2020-2022 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2015 Matt O'Gorman <mog@rldn.net>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from litex.build.generic_platform import *
-from litex.build.lattice import LatticeECP5Platform
-from litex.build.openfpgaloader import OpenFPGALoader
+from litex.build.xilinx import XilinxSpartan6Platform
+from litex.build.xilinx.programmer import XC3SProg
 
 # IOs ----------------------------------------------------------------------------------------------
 
 _io = [
     # Clk / Rst
-    ("clk100", 0, Pins("K23"), IOStandard("LVCMOS33")),
-    ("rst_n",  0, Pins("N5"),  IOStandard("LVCMOS33")),
+    ("clk32", 0, Pins("J4"), IOStandard("LVCMOS33")),
+    ("clk50", 0, Pins("K3"), IOStandard("LVCMOS33")),
 
     # Leds
-    ("rgb_led", 0,
-        Subsignal("r", Pins("P21")),
-        Subsignal("g", Pins("R23")),
-        Subsignal("b", Pins("P22")),
-        IOStandard("LVCMOS33"),
+    ("user_led", 0, Pins("P11"), IOStandard("LVCMOS33")),
+    ("user_led", 1, Pins("N9"),  IOStandard("LVCMOS33")),
+    ("user_led", 2, Pins("M9"),  IOStandard("LVCMOS33")),
+    ("user_led", 3, Pins("P9"),  IOStandard("LVCMOS33")),
+    ("user_led", 4, Pins("T8"),  IOStandard("LVCMOS33")),
+    ("user_led", 5, Pins("N8"),  IOStandard("LVCMOS33")),
+    ("user_led", 6, Pins("P8"),  IOStandard("LVCMOS33")),
+    ("user_led", 7, Pins("P7"),  IOStandard("LVCMOS33")),
+
+    # Switches
+    ("user_sw", 0, Pins("L1"), IOStandard("LVCMOS33"), Misc("PULLUP")),
+    ("user_sw", 1, Pins("L3"), IOStandard("LVCMOS33"), Misc("PULLUP")),
+    ("user_sw", 2, Pins("L4"), IOStandard("LVCMOS33"), Misc("PULLUP")),
+    ("user_sw", 3, Pins("L5"), IOStandard("LVCMOS33"), Misc("PULLUP")),
+
+
+    # SPIFlash
+    ("spiflash", 0,
+        Subsignal("cs_n", Pins("T3"), IOStandard("LVCMOS33")),
+        Subsignal("clk",  Pins("R11"), IOStandard("LVCMOS33")),
+        Subsignal("mosi", Pins("T10"), IOStandard("LVCMOS33")),
+        Subsignal("miso", Pins("P10"), IOStandard("LVCMOS33"))
     ),
-    ("rgb_led", 1,
-        Subsignal("r", Pins("K21")),
-        Subsignal("g", Pins("K24")),
-        Subsignal("b", Pins("M21")),
-        IOStandard("LVCMOS33"),
+
+    # Serial
+    ("serial", 0,
+        Subsignal("tx", Pins("N6"), IOStandard("LVCMOS33")),  # FTDI D1
+        Subsignal("rx", Pins("M7"), IOStandard("LVCMOS33"))   # FTDI D0
     ),
-    ("rgb_led", 2,
-        Subsignal("r", Pins("U21")),
-        Subsignal("g", Pins("W21")),
-        Subsignal("b", Pins("T24")),
+
+    # USB FIFO
+    ("usb_fifo", 0,
+        Subsignal("data",  Pins("M7 N6 M6 P5 N5 P4 P2 P1")),
+        Subsignal("rxf_n", Pins("N3")),
+        Subsignal("txe_n", Pins("N1")),
+        Subsignal("rd_n",  Pins("M1")),
+        Subsignal("wr_n",  Pins("M2")),
+        Subsignal("siwua", Pins("M3")),
+        Misc("SLEW=FAST"),
+        Drive(8),
         IOStandard("LVCMOS33"),
     ),
-    ("rgb_led", 3,
-        Subsignal("r", Pins("T23")),
-        Subsignal("g", Pins("R21")),
-        Subsignal("b", Pins("T22")),
-        IOStandard("LVCMOS33"),
+
+    # ADC
+    ("adc", 0,
+        Subsignal("cs_n", Pins("F6"), IOStandard("LVCMOS33")),
+        Subsignal("clk",  Pins("G6"), IOStandard("LVCMOS33")),
+        Subsignal("mosi", Pins("H4"), IOStandard("LVCMOS33")),
+        Subsignal("miso", Pins("H5"), IOStandard("LVCMOS33"))
     ),
 
-    # Serial
-    ("serial", 0,
-        Subsignal("rx", Pins("R26"), IOStandard("LVCMOS33")),
-        Subsignal("tx", Pins("R24"), IOStandard("LVCMOS33")),
+    # Audio
+    ("audio", 0,
+        Subsignal("a0", Pins("B8"), IOStandard("LVCMOS33")),
+        Subsignal("a1", Pins("A8"), IOStandard("LVCMOS33"))
     ),
 
-    # DDR3 SDRAM
-    ("ddram", 0,
+    # SDR SDRAM
+    ("sdram_clock", 0, Pins("G16"), IOStandard("LVCMOS33"), Misc("SLEW=FAST")),
+    ("sdram", 0,
         Subsignal("a", Pins(
-            "T5 M3 L3 V6 K2 W6 K3 L1",
-            "H2 L2 N1 J1 M1 K1 H1"),
-            IOStandard("SSTL15_I")),
-        Subsignal("ba",    Pins("U6 N3 N4"), IOStandard("SSTL15_I")),
-        Subsignal("ras_n", Pins("T3"), IOStandard("SSTL15_I")),
-        Subsignal("cas_n", Pins("P2"), IOStandard("SSTL15_I")),
-        Subsignal("we_n",  Pins("R3"), IOStandard("SSTL15_I")),
-        Subsignal("dm", Pins("U4 U1"), IOStandard("SSTL15_I")),
+            "T15 R16 P15 P16 N16 M15 M16 L16",
+            "K15 K16 R15 J16 H15")),
         Subsignal("dq", Pins(
-            "T4 W4 R4 W5 R6 P6 P5 P4",
-            "R1 W3 T2 V3 U3 W1 T1 W2",),
-            IOStandard("SSTL15_I"),
-            Misc("TERMINATION=75")),
-        Subsignal("dqs_p", Pins("V4 V1"), IOStandard("SSTL15D_I"),
-            Misc("TERMINATION=OFF"),
-            Misc("DIFFRESISTOR=100")),
-        Subsignal("clk_p", Pins("H3"), IOStandard("SSTL15D_I")),
-        Subsignal("cke",   Pins("P1"), IOStandard("SSTL15_I")),
-        Subsignal("odt",   Pins("P3"), IOStandard("SSTL15_I")),
-        Misc("SLEWRATE=FAST"),
-    ),
-
-    # RGMII Ethernetx
-    ("eth_clocks", 0,
-        Subsignal("tx", Pins("A12")),
-        Subsignal("rx", Pins("E11")),
-        IOStandard("LVCMOS33")
-    ),
-    ("eth", 0,
-        Subsignal("rst_n",   Pins("C13")),
-        Subsignal("mdio",    Pins("A13")),
-        Subsignal("mdc",     Pins("C11")),
-        Subsignal("rx_ctl",  Pins("A11")),
-        Subsignal("rx_data", Pins("B11 A10 B10 A9"), Misc("PULLMODE=UP")), # RGMII mode - Advertise all capabilities.
-        Subsignal("tx_ctl",  Pins("C9")),
-        Subsignal("tx_data", Pins("D8 C8 B8 A8")),
-        IOStandard("LVCMOS33")
+            "T13 T12 R12  T9  R9  T7  R7  T6",
+            "F16 E15 E16 D16 B16 B15 C16 C15")),
+        Subsignal("we_n",  Pins("R5")),
+        Subsignal("ras_n", Pins("R2")),
+        Subsignal("cas_n", Pins("T4")),
+        Subsignal("cs_n",  Pins("R1")),
+        Subsignal("cke",   Pins("H16")),
+        Subsignal("ba",    Pins("R14 T14")),
+        Subsignal("dm",    Pins("T5 F15")),
+        Misc("SLEW=FAST"),
+        IOStandard("LVCMOS33"),
     ),
 
     # SDCard
-    ("sdcard", 0,
-        Subsignal("data",      Pins("N26 N25 N23 N21"), Misc("PULLMODE=UP")),
-        Subsignal("cmd",       Pins("M24"),             Misc("PULLMODE=UP")),
-        Subsignal("clk",       Pins("P24")),
-        Subsignal("cd",        Pins("L22")),
-        Subsignal("cmd_dir",   Pins("M23")),
-        Subsignal("dat0_dir",  Pins("N24")),
-        Subsignal("dat13_dir", Pins("P26")),
+    ("spisdcard", 0,
+        Subsignal("clk",  Pins("L12")),
+        Subsignal("mosi", Pins("K11"), Misc("PULLUP")),
+        Subsignal("cs_n", Pins("K12"), Misc("PULLUP")),
+        Subsignal("miso", Pins("M10"), Misc("PULLUP")),
+        Misc("SLEW=FAST"),
         IOStandard("LVCMOS33"),
     ),
-
-    # Sata
-    ("sata", 0,
-        Subsignal("clk_p", Pins("AF12")),
-        Subsignal("clk_n", Pins("AF13")),
-        Subsignal("rx_p", Pins("AF15")),
-        Subsignal("rx_n", Pins("AF16")),
-        Subsignal("tx_p", Pins("AD16")),
-        Subsignal("tx_n", Pins("AD17")),
+    ("sdcard", 0,
+        Subsignal("data", Pins("M10 L10 J11 K12"), Misc("PULLUP")),
+        Subsignal("cmd",  Pins("K11"), Misc("PULLUP")),
+        Subsignal("clk",  Pins("L12")),
+        Misc("SLEW=FAST"),
         IOStandard("LVCMOS33"),
     ),
 
-    # SPIFlash
-    ("spiflash", 0,
-        Subsignal("cs_n", Pins("AA2")),
-        Subsignal("mosi", Pins("AE2")),
-        Subsignal("miso", Pins("AD2")),
-        Subsignal("wp", Pins("AF2")),
-        Subsignal("hold", Pins("AE1")),
-        IOStandard("LVCMOS33")
-    ),
-    ("spiflash4x", 0,
-        Subsignal("cs_n", Pins("AA2")),
-        Subsignal("dq", Pins("AE2", "AD2", "AF2", "AE1")),
-        IOStandard("LVCMOS33")
-    ),
-
-    # USB
-    ("ulpi", 0,
-        Subsignal("rst",  Pins("E23")),
-        Subsignal("clk",  Pins("H24")),
-        Subsignal("dir",  Pins("F22")),
-        Subsignal("nxt",  Pins("F23")),
-        Subsignal("stp",  Pins("H23")),
-        Subsignal("data", Pins("M26 L25 L26 K25 K26 J23 P25 H25")),
-        IOStandard("LVCMOS33")
-    ),
-
-    # HDMI / IT6613
-    ("hdmi", 0,
-        Subsignal("r", Pins("AD26 AE25 AF25 AE26 E10 D11 D10 C10  D9  E8 H5 J4")),
-        Subsignal("g", Pins("AA23 AA22 AA24 AA25  E1  F2  F1 D17 D16 E16 J6 H6")),
-        Subsignal("b", Pins("AD25 AC26 AB24 AB25  B3  C3  D3  B1  C2  D2 D1 E3")),
-        Subsignal("de",    Pins("A3")),
-        Subsignal("clk",   Pins("C1")),
-        Subsignal("vsync", Pins("A4")),
-        Subsignal("hsync", Pins("B4")),
-        Subsignal("sda", Pins("E17")),
-        Subsignal("scl", Pins("C17")),
-        IOStandard("LVCMOS33")
-    ),
+    # HDMI In
+    ("hdmi_in", 0,
+        Subsignal("clk_p",   Pins("C9"), IOStandard("TMDS_33")),
+        Subsignal("clk_n",   Pins("A9"), IOStandard("TMDS_33")),
+        Subsignal("data0_p", Pins("C7"), IOStandard("TMDS_33")),
+        Subsignal("data0_n", Pins("A7"), IOStandard("TMDS_33")),
+        Subsignal("data1_p", Pins("B6"), IOStandard("TMDS_33")),
+        Subsignal("data1_n", Pins("A6"), IOStandard("TMDS_33")),
+        Subsignal("data2_p", Pins("B5"), IOStandard("TMDS_33")),
+        Subsignal("data2_n", Pins("A5"), IOStandard("TMDS_33")),
+        Subsignal("scl",     Pins("C1"), IOStandard("LVCMOS33")),
+        Subsignal("sda",     Pins("B1"), IOStandard("LVCMOS33"))
+    ),
+
+    # HDMI Out
+    ("hdmi_out", 0,
+        Subsignal("clk_p",  Pins("B14"), IOStandard("TMDS_33")),
+        Subsignal("clk_n",  Pins("A14"), IOStandard("TMDS_33")),
+        Subsignal("data0_p", Pins("C13"), IOStandard("TMDS_33")),
+        Subsignal("data0_n", Pins("A13"), IOStandard("TMDS_33")),
+        Subsignal("data1_p", Pins("B12"), IOStandard("TMDS_33")),
+        Subsignal("data1_n", Pins("A12"), IOStandard("TMDS_33")),
+        Subsignal("data2_p", Pins("C11"), IOStandard("TMDS_33")),
+        Subsignal("data2_n", Pins("A11"), IOStandard("TMDS_33")),
+    )
 ]
 
 # Connectors ---------------------------------------------------------------------------------------
 
 _connectors = [
-    ("pmod0", "T25 U25 U24 V24 T26 U26 V26 W26"),
-    ("pmod1", "U23 V23 U22 V21 W25 W24 W23 W22"),
-    ("pmod2", "J24 H22 E21 D18 K22 J21 H21 D22"),
-    ("pmod3", "E4 F4 E6 H4 F3 D4 D5 F5"),
-    ("pmod4", "E26 D25 F26 F25 C26 C25 A25 A24"),
-    ("pmod5", "D19 C21 B21 C22 D21 A21 A22 A23"),
-    ("pmod6", "C16 B17 C18 B19 A17 A18 A19 C19"),
-    ("pmod7", "D14 B14 E14 B16 C14 A14 A15 A16"),
+    ("A", "E7   C8  D8  E8  D9 A10 B10 C10 E10  F9 F10 D11"),
+    ("B", "E11 D14 D12 E12 E13 F13 F12 F14 G12 H14 J14"),
+    ("C", "J13 J12 K14 L14 L13 M14 M13 N14 M12 N12 P12 M11"),
+    ("D", "D6 C6 E6 C5"),
+    ("E", "D5 A4 G5 A3 B3 A2 B2 C3 C2 D3 D1 E3"),
+    ("F", "E2 E1 E4 F4 F5 G3 F3 G1 H3 H1 H2 J1")
 ]
 
 # Platform -----------------------------------------------------------------------------------------
 
-class Platform(LatticeECP5Platform):
-    default_clk_name   = "clk100"
-    default_clk_period = 1e9/100e6
-
-    def __init__(self, device="85F", toolchain="trellis", **kwargs):
-        assert device in ["45F", "85F"]
-        LatticeECP5Platform.__init__(self, f"LFE5UM5G-{device}-8BG554I", _io, _connectors, toolchain=toolchain, **kwargs)
+class Platform(XilinxSpartan6Platform):
+    default_clk_name   = "clk32"
+    default_clk_period = 1e9/32e6
+
+    def __init__(self, device="xc6slx25", toolchain="ise"):
+        assert device in ["xc6slx9", "xc6slx25"]
+        XilinxSpartan6Platform.__init__(self, device+"-3-ftg256", _io, _connectors, toolchain=toolchain)
 
     def create_programmer(self):
-        return OpenFPGALoader("ecpix5")
+        return XC3SProg(cable="ftdi")
 
     def do_finalize(self, fragment):
-        LatticeECP5Platform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk100", loose=True), 1e9/100e6)
-        self.add_period_constraint(self.lookup_request("eth_clocks:rx", 0, loose=True), 1e9/125e6)
+        XilinxSpartan6Platform.do_finalize(self, fragment)
+        self.add_period_constraint(self.lookup_request("clk32", loose=True), 1e9/32e6)
+        self.add_period_constraint(self.lookup_request("clk50", loose=True), 1e9/50e6)
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/lambdaconcept_pcie_screamer.py` & `litex-boards-2023.8/litex_boards/platforms/lambdaconcept_pcie_screamer.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/lambdaconcept_pcie_screamer_m2.py` & `litex-boards-2023.8/litex_boards/platforms/lambdaconcept_pcie_screamer_m2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/lattice_crosslink_nx_evn.py` & `litex-boards-2023.8/litex_boards/platforms/lattice_crosslink_nx_evn.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/lattice_crosslink_nx_vip.py` & `litex-boards-2023.8/litex_boards/platforms/lattice_crosslink_nx_vip.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/lattice_ecp5_evn.py` & `litex-boards-2023.8/litex_boards/platforms/lattice_ecp5_evn.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/lattice_ecp5_vip.py` & `litex-boards-2023.8/litex_boards/platforms/lattice_ecp5_vip.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/lattice_ice40up5k_evn.py` & `litex-boards-2023.8/litex_boards/platforms/lattice_ice40up5k_evn.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/lattice_machxo3.py` & `litex-boards-2023.8/litex_boards/platforms/lattice_machxo3.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/lattice_versa_ecp5.py` & `litex-boards-2023.8/litex_boards/platforms/lattice_versa_ecp5.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/limesdr_mini_v2.py` & `litex-boards-2023.8/litex_boards/platforms/limesdr_mini_v2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/linsn_rv901t.py` & `litex-boards-2023.8/litex_boards/platforms/linsn_rv901t.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/litex_acorn_baseboard.py` & `litex-boards-2023.8/litex_boards/platforms/litex_acorn_baseboard.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/logicbone.py` & `litex-boards-2023.8/litex_boards/platforms/logicbone.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/machdyne_konfekt.py` & `litex-boards-2023.8/litex_boards/platforms/machdyne_konfekt.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/machdyne_kopflos.py` & `litex-boards-2023.8/litex_boards/platforms/machdyne_kopflos.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/machdyne_krote.py` & `litex-boards-2023.8/litex_boards/platforms/machdyne_krote.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/machdyne_mozart_ml1.py` & `litex-boards-2023.8/litex_boards/platforms/sipeed_tang_nano_20k.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,140 +1,106 @@
 #
 # This file is part of LiteX-Boards.
 #
-# Copright (c) 2023 Lone Dynamics Corporation <info@lonedynamics.com>
-#
+# Copyright (c) 2023 Icenowy Zheng <uwu@icenowy.me>
 # SPDX-License-Identifier: BSD-2-Clause
 
+from migen import *
+
 from litex.build.generic_platform import *
-from litex.build.lattice import LatticePlatform
+from litex.build.gowin.platform import GowinPlatform
+from litex.build.gowin.programmer import GowinProgrammer
 from litex.build.openfpgaloader import OpenFPGALoader
 
-# IOs ----------------------------------------------------------------------------------------------
-
-_io_vx = [
-
-    # Clock
-    ("clk48", 0,  Pins("A7"),  IOStandard("LVCMOS33")),
-
-    # SDRAM
-    ("sdram_clock", 0, Pins("F16"), IOStandard("LVTTL33")),
-    ("sdram", 0,
-        Subsignal("a", Pins(
-            "M13 M14 L14 L13 G12 G13 G14 G15",
-            "F12 F13 T15 F14 E14")),
-        Subsignal("ba",    Pins("P14 N13")),
-        Subsignal("cs_n",  Pins("J16")),
-        Subsignal("cke",   Pins("F15")),
-        Subsignal("ras_n", Pins("K15")),
-        Subsignal("cas_n", Pins("K16")),
-        Subsignal("we_n",  Pins("L15")),
-        Subsignal("dq", Pins(
-            "R15 R16 P16 P15 N16 N14 M16 M15",
-            "E15 D16 D14 C16 C15 C14 B15 B16")),
-        Subsignal("dm", Pins("L16 E16")),
-        IOStandard("LVTTL33")
-    ),
-
-    # Differential Data Multiple Interface
-    ("ddmi", 0,
-        Subsignal("clk_p",    Pins("B13"),
-            IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        Subsignal("data0_p",  Pins("A11"),
-            IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        Subsignal("data1_p",  Pins("B12"),
-            IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        Subsignal("data2_p",  Pins("B10"),
-            IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-    ),
 
-    # USB-C
-    ("usb", 0,
-        Subsignal("d_p", Pins("A13")),
-        Subsignal("d_n", Pins("A14")),
-        Subsignal("pullup", Pins("D13")),
-        IOStandard("LVCMOS33")
-    ),
+# IOs ----------------------------------------------------------------------------------------------
 
-    # DUAL USB HOST
-    ("usb_host", 0,
-        Subsignal("dp", Pins("A9 C8")),
-        Subsignal("dm", Pins("A10 B8")),
-        IOStandard("LVCMOS33")
-    ),
+_io = [
+    # Clk / Rst.
+    ("clk27",  0, Pins("4"), IOStandard("LVCMOS33")),
 
-    # ETHERNET
-    ("eth_clocks", 0,
-        Subsignal("ref_clk", Pins("C7")),
-        IOStandard("LVCMOS33")
-    ),
-    ("eth", 0,
-        Subsignal("rx_data", Pins("E4 D4"), Misc("PULLMODE=UP")),
-        Subsignal("tx_data", Pins("E6 D6")),
-        Subsignal("tx_en", Pins("C5")),
-        Subsignal("crs_dv", Pins("A5"), Misc("PULLMODE=UP")),
-        Subsignal("rst_n", Pins("B5")),
-        IOStandard("LVCMOS33")
-    ),
-
-    # DEBUG UART
+    # Serial.
     ("serial", 0,
-        Subsignal("tx", Pins("B3")),
-        Subsignal("rx", Pins("A2")),
+        Subsignal("rx", Pins("70")),
+        Subsignal("tx", Pins("69")),
         IOStandard("LVCMOS33")
     ),
-]
 
-_io_v0 = [
-
-    # SD card w/ SD-mode interface
-    ("sdcard", 0,
-        Subsignal("cd", Pins("A6"), Misc("PULLMODE=UP")),
-        Subsignal("clk", Pins("L3")),
-        Subsignal("cmd", Pins("M1"), Misc("DRIVE=8 PULLMODE=UP")),
-        Subsignal("data", Pins("L1 M2 M3 L2"), Misc("DRIVE=8 PULLMODE=UP")),
-        Misc("SLEWRATE=FAST"),
-        IOStandard("LVCMOS33")
+    # SPIFlash.
+    ("spiflash", 0,
+        Subsignal("cs_n", Pins("60"), IOStandard("LVCMOS33")),
+        Subsignal("clk",  Pins("59"), IOStandard("LVCMOS33")),
+        Subsignal("miso", Pins("62"), IOStandard("LVCMOS33")),
+        Subsignal("mosi", Pins("61"), IOStandard("LVCMOS33")),
     ),
 
-    # SD card w/ SPI interface
+    # SDCard.
     ("spisdcard", 0,
-        Subsignal("clk",  Pins("L3")),
-        Subsignal("mosi", Pins("M1")),
-        Subsignal("cs_n", Pins("L2")),
-        Subsignal("miso", Pins("L1")),
-        Misc("SLEWRATE=FAST"),
+        Subsignal("clk",  Pins("83")),
+        Subsignal("mosi", Pins("82")),
+        Subsignal("cs_n", Pins("81")),
+        Subsignal("miso", Pins("84")),
+        IOStandard("LVCMOS33"),
+    ),
+    ("sdcard", 0,
+        Subsignal("data", Pins("84 85 80 81")),
+        Subsignal("cmd",  Pins("82")),
+        Subsignal("clk",  Pins("83")),
         IOStandard("LVCMOS33"),
     ),
 
+    # Leds
+    ("led_n", 0,  Pins("15"), IOStandard("LVCMOS33")),
+    ("led_n", 1,  Pins("16"), IOStandard("LVCMOS33")),
+    ("led_n", 2,  Pins("17"), IOStandard("LVCMOS33")),
+    ("led_n", 3,  Pins("18"), IOStandard("LVCMOS33")),
+    ("led_n", 4,  Pins("19"), IOStandard("LVCMOS33")),
+    ("led_n", 5,  Pins("20"), IOStandard("LVCMOS33")),
+
+    # RGB Led.
+    ("rgb_led", 0, Pins("79"), IOStandard("LVCMOS33")),
+
+    # Buttons.
+    ("btn", 0,  Pins("88"), IOStandard("LVCMOS33")),
+    ("btn", 1,  Pins("87"), IOStandard("LVCMOS33")),
+
+    # SDRAM (embedded in SIP, requires specific IO naming)
+    ("O_sdram_clk",   0, Pins(1),  IOStandard("LVCMOS33")),
+    ("O_sdram_cke",   0, Pins(1),  IOStandard("LVCMOS33")),
+    ("O_sdram_cs_n",  0, Pins(1),  IOStandard("LVCMOS33")),
+    ("O_sdram_cas_n", 0, Pins(1),  IOStandard("LVCMOS33")),
+    ("O_sdram_ras_n", 0, Pins(1),  IOStandard("LVCMOS33")),
+    ("O_sdram_wen_n", 0, Pins(1),  IOStandard("LVCMOS33")),
+    ("O_sdram_dqm",   0, Pins(4),  IOStandard("LVCMOS33")),
+    ("O_sdram_addr",  0, Pins(11), IOStandard("LVCMOS33")),
+    ("O_sdram_ba",    0, Pins(2),  IOStandard("LVCMOS33")),
+    ("IO_sdram_dq",   0, Pins(32), IOStandard("LVCMOS33")),
 ]
 
 # Connectors ---------------------------------------------------------------------------------------
 
-_connectors_vx = [
-
+_connectors = [
+        # TODO
 ]
 
 # Platform -----------------------------------------------------------------------------------------
 
-class Platform(LatticePlatform):
-    default_clk_name   = "clk48"
-    default_clk_period = 1e9/48e6
-
-    def __init__(self, revision="v0", device="45F", toolchain="trellis", **kwargs):
-        assert revision in ["v0"]
-        assert device in ["12F", "25F", "45F", "85F"]
-        self.revision = revision
-
-        io = _io_vx
-        connectors = _connectors_vx
-
-        if revision == "v0": io += _io_v0
-
-        LatticePlatform.__init__(self, f"LFE5U-{device}-6BG256", io, connectors, toolchain=toolchain, **kwargs)
+class Platform(GowinPlatform):
+    default_clk_name   = "clk27"
+    default_clk_period = 1e9/27e6
+
+    def __init__(self, dock="standard", toolchain="gowin"):
+
+        GowinPlatform.__init__(self, "GW2AR-LV18QN88C8/I7", _io, _connectors, toolchain=toolchain, devicename="GW2AR-18C")
+
+        self.toolchain.options["use_mspi_as_gpio"]  = 1
+        self.toolchain.options["use_sspi_as_gpio"]  = 1
+        self.toolchain.options["use_ready_as_gpio"] = 1
+        self.toolchain.options["use_done_as_gpio"]  = 1
+        self.toolchain.options["rw_check_on_ram"]   = 1
 
-    def create_programmer(self, cable):
-        return OpenFPGALoader(cable=cable)
+    def create_programmer(self, kit="openfpgaloader"):
+        return OpenFPGALoader(cable="ft2232")
 
     def do_finalize(self, fragment):
-        LatticePlatform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk48", loose=True), 1e9/48e6)
+        GowinPlatform.do_finalize(self, fragment)
+        self.add_period_constraint(self.lookup_request("clk27", loose=True), 1e9/27e6)
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/machdyne_noir.py` & `litex-boards-2023.8/litex_boards/platforms/machdyne_noir.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/machdyne_schoko.py` & `litex-boards-2023.8/litex_boards/platforms/machdyne_schoko.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/marble.py` & `litex-boards-2023.8/litex_boards/platforms/marble.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/marblemini.py` & `litex-boards-2023.8/litex_boards/platforms/marblemini.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/micronova_mercury2.py` & `litex-boards-2023.8/litex_boards/platforms/micronova_mercury2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/mist.py` & `litex-boards-2023.8/litex_boards/platforms/mist.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/mnt_rkx7.py` & `litex-boards-2023.8/litex_boards/platforms/mnt_rkx7.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/muselab_icesugar.py` & `litex-boards-2023.8/litex_boards/platforms/muselab_icesugar.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/muselab_icesugar_pro.py` & `litex-boards-2023.8/litex_boards/platforms/muselab_icesugar_pro.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/myminieye_runber.py` & `litex-boards-2023.8/litex_boards/platforms/myminieye_runber.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/newae_cw305.py` & `litex-boards-2023.8/litex_boards/platforms/newae_cw305.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/numato_aller.py` & `litex-boards-2023.8/litex_boards/platforms/numato_aller.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/numato_mimas_a7.py` & `litex-boards-2023.8/litex_boards/platforms/radiona_ulx3s.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,205 +1,217 @@
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2018-2019 Rohit Singh <rohit@rohitksingh.in>
-# Copyright (c) 2020 Feliks Montez <feliks.montez@gmail.com>
+# Copyright (c) 2018-2019 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from litex.build.generic_platform import *
-from litex.build.xilinx import Xilinx7SeriesPlatform
-from litex.build.openocd import OpenOCD
+from litex.build.lattice import LatticeECP5Platform
+from litex.build.lattice.programmer import UJProg
 
 # IOs ----------------------------------------------------------------------------------------------
 
-_io = [
+_io_common = [
     # Clk / Rst
-    ("clk100", 0, Pins("H4"), IOStandard("LVCMOS33")),
-    ("cpu_reset", 0, Pins("M2"), IOStandard("LVCMOS33")),
-
-    # Leds
-    ("user_led", 0, Pins("K17"), IOStandard("LVCMOS33")),
-    ("user_led", 1, Pins("J17"), IOStandard("LVCMOS33")),
-    ("user_led", 2, Pins("L14"), IOStandard("LVCMOS33")),
-    ("user_led", 3, Pins("L15"), IOStandard("LVCMOS33")),
-    ("user_led", 4, Pins("L16"), IOStandard("LVCMOS33")),
-    ("user_led", 5, Pins("K16"), IOStandard("LVCMOS33")),
-    ("user_led", 6, Pins("M15"), IOStandard("LVCMOS33")),
-    ("user_led", 7, Pins("M16"), IOStandard("LVCMOS33")),
-
-    # Switches
-    ("user_sw", 0, Pins("B21"), IOStandard("LVCMOS33")),
-    ("user_sw", 1, Pins("A21"), IOStandard("LVCMOS33")),
-    ("user_sw", 2, Pins("E22"), IOStandard("LVCMOS33")),
-    ("user_sw", 3, Pins("D22"), IOStandard("LVCMOS33")),
-    ("user_sw", 4, Pins("E21"), IOStandard("LVCMOS33")),
-    ("user_sw", 5, Pins("D21"), IOStandard("LVCMOS33")),
-    ("user_sw", 6, Pins("G21"), IOStandard("LVCMOS33")),
-    ("user_sw", 7, Pins("G22"), IOStandard("LVCMOS33")),
+    ("clk25", 0, Pins("G2"), IOStandard("LVCMOS33")),
+    ("rst",   0, Pins("R1"), IOStandard("LVCMOS33")),
 
     # Buttons
-    ("user_btn", 0, Pins("P20"), IOStandard("LVCMOS33")),
-    ("user_btn", 1, Pins("P19"), IOStandard("LVCMOS33")),
-    ("user_btn", 2, Pins("P17"), IOStandard("LVCMOS33")),
-    ("user_btn", 3, Pins("N17"), IOStandard("LVCMOS33")),
+    ("user_btn", 0, Pins( "D6"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # PWR
+    ("user_btn", 1, Pins( "R1"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # F1
+    ("user_btn", 2, Pins( "T1"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # F2
+    ("user_btn", 3, Pins("R18"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # UP
+    ("user_btn", 4, Pins( "V1"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # DOWN
+    ("user_btn", 5, Pins( "U1"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # LEFT
+    ("user_btn", 6, Pins("H16"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # RIGHT
+
+    # Leds
+    ("user_led", 0, Pins("B2"), IOStandard("LVCMOS33")),
+    ("user_led", 1, Pins("C2"), IOStandard("LVCMOS33")),
+    ("user_led", 2, Pins("C1"), IOStandard("LVCMOS33")),
+    ("user_led", 3, Pins("D2"), IOStandard("LVCMOS33")),
+    ("user_led", 4, Pins("D1"), IOStandard("LVCMOS33")),
+    ("user_led", 5, Pins("E2"), IOStandard("LVCMOS33")),
+    ("user_led", 6, Pins("E1"), IOStandard("LVCMOS33")),
+    ("user_led", 7, Pins("H3"), IOStandard("LVCMOS33")),
 
     # Serial
-    ("serial", 0, # Can be used when FT2232H's Channel A configured to ASYNC Serial (UART) mode
-        Subsignal("tx", Pins("Y21")),
-        Subsignal("rx", Pins("Y22")),
+    ("serial", 0,
+        Subsignal("tx", Pins("L4"), IOStandard("LVCMOS33")),
+        Subsignal("rx", Pins("M1"), IOStandard("LVCMOS33"))
+    ),
+
+    # SDR SDRAM
+    ("sdram_clock", 0, Pins("F19"), IOStandard("LVCMOS33")),
+    ("sdram", 0,
+        Subsignal("a",     Pins(
+            "M20 M19 L20 L19 K20 K19 K18 J20",
+            "J19 H20 N19 G20 G19")),
+        Subsignal("dq",    Pins(
+            "J16 L18 M18 N18 P18 T18 T17 U20",
+            "E19 D20 D19 C20 E18 F18 J18 J17")),
+        Subsignal("we_n",  Pins("T20")),
+        Subsignal("ras_n", Pins("R20")),
+        Subsignal("cas_n", Pins("T19")),
+        Subsignal("cs_n",  Pins("P20")),
+        Subsignal("cke",   Pins("F20")),
+        Subsignal("ba",    Pins("P19 N20")),
+        Subsignal("dm",    Pins("U19 E20")),
+        IOStandard("LVCMOS33"),
+        Misc("SLEWRATE=FAST"),
+    ),
+
+    # GPIOs
+    ("gpio", 0,
+        Subsignal("p", Pins("B11")),
+        Subsignal("n", Pins("C11")),
+        IOStandard("LVCMOS33")
+    ),
+    ("gpio", 1,
+        Subsignal("p", Pins("A10")),
+        Subsignal("n", Pins("A11")),
+        IOStandard("LVCMOS33")
+    ),
+    ("gpio", 2,
+        Subsignal("p", Pins("A9")),
+        Subsignal("n", Pins("B10")),
+        IOStandard("LVCMOS33")
+    ),
+    ("gpio", 3,
+        Subsignal("p", Pins("B9")),
+        Subsignal("n", Pins("C10")),
         IOStandard("LVCMOS33")
     ),
 
-    # USB FIFO
-    ("usb_fifo", 0, # Can be used when FT2232H's Channel A configured to ASYNC FIFO 245 mode
-        Subsignal("data",  Pins("Y22 Y21 AB22 AA21 AB21 AA20 AB20 AA18")),
-        Subsignal("rxf_n", Pins("W21")),
-        Subsignal("txe_n", Pins("V22")),
-        Subsignal("rd_n",  Pins("AA19")),
-        Subsignal("wr_n",  Pins("W22")),
-        Subsignal("siwua", Pins("U21")),
-        Subsignal("oe_n",  Pins("T21")),
-        Misc("SLEW=FAST"),
-        Drive(8),
-        IOStandard("LVCMOS33"),
+    # USB
+    ("usb", 0,
+        Subsignal("d_p", Pins("D15")),
+        Subsignal("d_n", Pins("E15")),
+        Subsignal("pullup", Pins("B12 C12")),
+        IOStandard("LVCMOS33")
     ),
 
     # SPIFlash
     ("spiflash", 0,
-        Subsignal("cs_n", Pins("T19")),
-        Subsignal("clk",  Pins("L12")),
-        Subsignal("mosi", Pins("P22")),
-        Subsignal("miso", Pins("R22")),
-        Subsignal("wp",   Pins("P21")),
-        Subsignal("hold", Pins("R21")),
-        IOStandard("LVCMOS33"),
+        Subsignal("cs_n", Pins("R2")),
+        Subsignal("miso", Pins("V2")),
+        Subsignal("mosi", Pins("W2")),
+        Subsignal("wp", Pins("Y2")),
+        Subsignal("hold", Pins("W1")),
+        IOStandard("LVCMOS33")
     ),
     ("spiflash4x", 0,
-        Subsignal("cs_n", Pins("T19")),
-        Subsignal("clk",  Pins("L12")),
-        Subsignal("dq",   Pins("P22", "R22", "P21", "R21")),
-        IOStandard("LVCMOS33")
-    ),
-
-    # DDR3 SDRAM
-    ("ddram", 0,
-        Subsignal("a", Pins(
-            "U6 T5 Y6 T6 V2 T4 Y2 R2",
-            "Y1 R4 W5 W1 AA6 U2"),
-            IOStandard("SSTL15")),
-        Subsignal("ba",    Pins("W6 U5 R6"), IOStandard("SSTL15")),
-        Subsignal("ras_n", Pins("V5"),  IOStandard("SSTL15")),
-        Subsignal("cas_n", Pins("T1"),  IOStandard("SSTL15")),
-        Subsignal("we_n",  Pins("R3"),  IOStandard("SSTL15")),
-        Subsignal("dm", Pins("Y7 AA1"), IOStandard("SSTL15")),
-        Subsignal("dq", Pins(
-            "Y8 AB6 W9  AA8 AB7 V7 AB8 W7",
-            "V4 AB2 AA5 AB3 AB5 W4 AB1 AA4"),
-            IOStandard("SSTL15"),
-            Misc("IN_TERM=UNTUNED_SPLIT_40")),
-        Subsignal("dqs_p", Pins("V9 Y3"),  IOStandard("DIFF_SSTL15")),
-        Subsignal("dqs_n", Pins("V8 AA3"), IOStandard("DIFF_SSTL15")),
-        Subsignal("clk_p", Pins("U3"), IOStandard("DIFF_SSTL15")),
-        Subsignal("clk_n", Pins("V3"), IOStandard("DIFF_SSTL15")),
-        Subsignal("cke",   Pins("U1"), IOStandard("SSTL15")),
-        Subsignal("odt",   Pins("W2"), IOStandard("SSTL15")),
-        Subsignal("cs_n",  Pins("T3"), IOStandard("SSTL15")),
-        Subsignal("reset_n", Pins("U7"), IOStandard("SSTL15")),
-        Misc("SLEW=FAST"),
-    ),
-
-    # I2C EEPROM
-    ("eeprom", 0,
-        Subsignal("scl", Pins("N5")),
-        Subsignal("sda", Pins("P6")),
-        IOStandard("LVCMOS33")
-    ),
-
-    # RGMII Ethernet
-    ("eth_clocks", 0,
-        Subsignal("tx", Pins("U20")),
-        Subsignal("rx", Pins("W19")),
-        IOStandard("LVCMOS33")
-    ),
-    ("eth", 0,
-        Subsignal("rst_n",   Pins("R14"), IOStandard("LVCMOS33")),
-        Subsignal("int_n",   Pins("V19")),
-        Subsignal("mdio",    Pins("P16")),
-        Subsignal("mdc",     Pins("R19")),
-        Subsignal("rx_ctl",  Pins("Y19")),
-        Subsignal("rx_data", Pins("AB18 W20 W17 V20")),
-        Subsignal("tx_ctl",  Pins("T20")),
-        Subsignal("tx_data", Pins("V18 U18 V17 U17")),
-        IOStandard("LVCMOS33")
-    ),
-
-    # HDMI In
-    ("hdmi_in", 0,
-        Subsignal("clk_p",   Pins("K4"), IOStandard("TMDS_33")),
-        Subsignal("clk_n",   Pins("J4"), IOStandard("TMDS_33")),
-        Subsignal("data0_p", Pins("K1"), IOStandard("TMDS_33")),
-        Subsignal("data0_n", Pins("J1"), IOStandard("TMDS_33")),
-        Subsignal("data1_p", Pins("M1"), IOStandard("TMDS_33")),
-        Subsignal("data1_n", Pins("L1"), IOStandard("TMDS_33")),
-        Subsignal("data2_p", Pins("P2"), IOStandard("TMDS_33")),
-        Subsignal("data2_n", Pins("N2"), IOStandard("TMDS_33")),
-        Subsignal("scl",     Pins("J2"), IOStandard("LVCMOS33")),
-        Subsignal("sda",     Pins("H2"), IOStandard("LVCMOS33")),
-        Subsignal("hpd_en",  Pins("G2"), IOStandard("LVCMOS33")),
-        Subsignal("cec",     Pins("K2"), IOStandard("LVCMOS33")), # FIXME
-        # Subsignal("txen", Pins("R3"), IOStandard("LVCMOS33")),  # FIXME
-    ),
-
-    # HDMI Out
-    ("hdmi_out", 0,
-        Subsignal("clk_p",   Pins("L3"), IOStandard("TMDS_33")),
-        Subsignal("clk_n",   Pins("K3"), IOStandard("TMDS_33")),
-        Subsignal("data0_p", Pins("B1"), IOStandard("TMDS_33")),
-        Subsignal("data0_n", Pins("A1"), IOStandard("TMDS_33")),
-        Subsignal("data1_p", Pins("E1"), IOStandard("TMDS_33")),
-        Subsignal("data1_n", Pins("D1"), IOStandard("TMDS_33")),
-        Subsignal("data2_p", Pins("G1"), IOStandard("TMDS_33")),
-        Subsignal("data2_n", Pins("F1"), IOStandard("TMDS_33")),
-        Subsignal("scl",     Pins("D2"), IOStandard("LVCMOS33")),
-        Subsignal("sda",     Pins("C2"), IOStandard("LVCMOS33")),
-        Subsignal("cec",     Pins("E2"), IOStandard("LVCMOS33")), # FIXME
-        Subsignal("hdp",     Pins("B2"), IOStandard("LVCMOS33")), # FIXME
+        Subsignal("cs_n", Pins("R2")),
+        Subsignal("dq", Pins("W2", "V2", "Y2", "W1")),
+        IOStandard("LVCMOS33")
     ),
+
+    # OLED
+    ("oled_spi", 0,
+        Subsignal("clk",  Pins("P4")),
+        Subsignal("mosi", Pins("P3")),
+        IOStandard("LVCMOS33"),
+    ),
+    ("oled_ctl", 0,
+        Subsignal("dc",   Pins("P1")),
+        Subsignal("resn", Pins("P2")),
+        Subsignal("csn",  Pins("N2")),
+        IOStandard("LVCMOS33"),
+    ),
+
+    # Others
+    ("ext0p", 0, Pins("B11"), IOStandard("LVCMOS33")),
+    ("ext1p", 0, Pins("A10"), IOStandard("LVCMOS33")),
+]
+
+_io_1_7 = [
+    # SDCard
+    ("spisdcard", 0,
+        Subsignal("clk",  Pins("J1")),
+        Subsignal("mosi", Pins("J3"), Misc("PULLMODE=UP")),
+        Subsignal("cs_n", Pins("H1"), Misc("PULLMODE=UP")),
+        Subsignal("miso", Pins("K2"), Misc("PULLMODE=UP")),
+        Misc("SLEWRATE=FAST"),
+        IOStandard("LVCMOS33"),
+    ),
+    ("sdcard", 0,
+        Subsignal("clk",  Pins("J1")),
+        Subsignal("cmd",  Pins("J3"), Misc("PULLMODE=UP")),
+        Subsignal("data", Pins("K2 K1 H2 H1"), Misc("PULLMODE=UP")),
+        Misc("SLEWRATE=FAST"),
+        IOStandard("LVCMOS33"),
+    ),
+
+    # GPDI
+    ("gpdi", 0,
+        Subsignal("clk_p",    Pins("A17"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        #Subsignal("clk_n",   Pins("B18"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        Subsignal("data0_p",  Pins("A12"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        #Subsignal("data0_n", Pins("A13"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        Subsignal("data1_p",  Pins("A14"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        #Subsignal("data1_n", Pins("C14"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        Subsignal("data2_p",  Pins("A16"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        #Subsignal("data2_n", Pins("B16"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        #Subsignal("cec",     Pins("A18"), IOStandard("LVCMOS33"), Misc("PULLMODE=UP")),
+        #Subsignal("scl",     Pins("E19"), IOStandard("LVCMOS33"), Misc("PULLMODE=UP")),
+        #Subsignal("sda",     Pins("B19"), IOStandard("LVCMOS33"), Misc("PULLMODE=UP"))
+    ),
+    # Wifi power
+    ("wifi_gpio0", 0, Pins("L2"), IOStandard("LVCMOS33")),
 ]
 
-# Connectors ---------------------------------------------------------------------------------------
+_io_2_0 = [
+    # SDCard
+    ("spisdcard", 0,
+        Subsignal("clk",  Pins("H2")),
+        Subsignal("mosi", Pins("J1"), Misc("PULLMODE=UP")),
+        Subsignal("cs_n", Pins("K2"), Misc("PULLMODE=UP")),
+        Subsignal("miso", Pins("J3"), Misc("PULLMODE=UP")),
+        Misc("SLEWRATE=FAST"),
+        IOStandard("LVCMOS33"),
+    ),
+    ("sdcard", 0,
+        Subsignal("clk",  Pins("H2")),
+        Subsignal("cmd",  Pins("J1"), Misc("PULLMODE=UP")),
+        Subsignal("data", Pins("J3 H1 K1 K2"), Misc("PULLMODE=UP")),
+        #Subsignal("cd", Pins("N5")), # Not connected
+        #Subsignal("wp", Pins("P5")), # Not connected
+        Misc("SLEWRATE=FAST"),
+        IOStandard("LVCMOS33"),
+    ),
 
-_connectors = [
-    ("P12", "J20 J21 K21 K22 H20 G20 J19 H19",
-            "J22 H22 K18 K19 L19 L20 M21 N22",
-            "N20 M20 M18 L18 N18 N19 H17 H18",
-            "G17 G18 G15 G16 J15 H15 K13 K14",
-            "M13 K14 M13 L13 J14 H14 H13 G13"),
-    ("P13", "F19 F20 E19 D19 D20 C20 C22 B22",
-            "F18 E18 C18 C19 D17 C17 B20 A20",
-            "B17 B18 A18 A19 E16 D16 B15 B16",
-            "A15 A16 C14 C15 A13 A14 C13 B13",
-            "D14 D15 E13 E14 F13 F14 F16 E17")
+    # GPDI
+    ("gpdi", 0,
+        Subsignal("clk_p",    Pins("A17"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        #Subsignal("clk_n",   Pins("B18"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        Subsignal("data0_p",  Pins("A16"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        #Subsignal("data0_n", Pins("B16"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        Subsignal("data1_p",  Pins("A14"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        #Subsignal("data1_n", Pins("C14"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        Subsignal("data2_p",  Pins("A12"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        #Subsignal("data2_n", Pins("A13"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
+        #Subsignal("cec",     Pins("A18"), IOStandard("LVCMOS33"), Misc("PULLMODE=UP")),
+        #Subsignal("scl",     Pins("E19"), IOStandard("LVCMOS33"), Misc("PULLMODE=UP")),
+        #Subsignal("sda",     Pins("B19"), IOStandard("LVCMOS33"), Misc("PULLMODE=UP"))
+    ),
+    # Wifi power
+    ("wifi_gpio0", 0, Pins("F1"), IOStandard("LVCMOS33")),    
 ]
 
 # Platform -----------------------------------------------------------------------------------------
 
-class Platform(Xilinx7SeriesPlatform):
-    default_clk_name   = "clk100"
-    default_clk_period = 1e9/100e6
-
-    def __init__(self, toolchain="vivado"):
-        Xilinx7SeriesPlatform.__init__(self, "xc7a50tfgg484-1", _io, _connectors, toolchain=toolchain)
-        self.toolchain.bitstream_commands = \
-            ["set_property BITSTREAM.CONFIG.SPI_BUSWIDTH 4 [current_design]"]
-        self.toolchain.additional_commands = \
-            ["write_cfgmem -force -format bin -interface spix4 -size 16 "
-             "-loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin"]
-        self.add_platform_command("set_property INTERNAL_VREF 0.675 [get_iobanks 34]")
+class Platform(LatticeECP5Platform):
+    default_clk_name   = "clk25"
+    default_clk_period = 1e9/25e6
+
+    def __init__(self, device="LFE5U-45F", revision="2.0", toolchain="trellis", **kwargs):
+        assert device in ["LFE5U-12F", "LFE5U-25F", "LFE5U-45F", "LFE5U-85F"]
+        assert revision in ["1.7", "2.0"]
+        _io = _io_common + {"1.7": _io_1_7, "2.0": _io_2_0}[revision]
+        LatticeECP5Platform.__init__(self, device + "-6BG381C", _io, toolchain=toolchain, **kwargs)
 
     def create_programmer(self):
-        return OpenOCD("openocd_xc7_ft2232.cfg", "bscan_spi_xc7a50t.bit")
+        return UJProg()
 
     def do_finalize(self, fragment):
-        Xilinx7SeriesPlatform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk100",        loose=True), 1e9/100e6)
-        self.add_period_constraint(self.lookup_request("eth_clocks:rx", loose=True), 1e9/125e6)
+        LatticeECP5Platform.do_finalize(self, fragment)
+        self.add_period_constraint(self.lookup_request("clk25", loose=True), 1e9/25e6)
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/numato_nereid.py` & `litex-boards-2023.8/litex_boards/platforms/numato_nereid.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/numato_tagus.py` & `litex-boards-2023.8/litex_boards/platforms/numato_tagus.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/ocp_tap_timecard.py` & `litex-boards-2023.8/litex_boards/platforms/ocp_tap_timecard.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,15 @@
         Subsignal("p", Pins("F6"), IOStandard("DIFF_SSTL15")),
         Subsignal("n", Pins("E6"), IOStandard("DIFF_SSTL15"))
     ),
     ("clk200", 0,
         Subsignal("p", Pins("R4"), IOStandard("DIFF_SSTL15")),
         Subsignal("n", Pins("T4"), IOStandard("DIFF_SSTL15"))
     ),
-    ("clk10", 0, Pins("W21"), IOStandard("LVCMOS33"), Misc("PULLDOWN=True")),
-    ("rst_n", 0, Pins("T6"),  IOStandard("LVCMOS15")),
+    ("rst_n", 0, Pins("T6"), IOStandard("LVCMOS15")),
 
     # Leds.
     ("user_led", 0, Pins("B13"), IOStandard("LVCMOS33")),
     ("user_led", 1, Pins("C13"), IOStandard("LVCMOS33")),
     ("user_led", 2, Pins("D14"), IOStandard("LVCMOS33")),
     ("user_led", 3, Pins("D15"), IOStandard("LVCMOS33")),
 
@@ -95,16 +94,14 @@
 
     # Leds.
     ("led", 0, Pins("E21"), IOStandard("LVCMOS33")),
     ("led", 1, Pins("D21"), IOStandard("LVCMOS33")),
     ("led", 2, Pins("E22"), IOStandard("LVCMOS33")),
     ("led", 3, Pins("D22"), IOStandard("LVCMOS33")),
 
-    ("som_led", 0, Pins("W5"), IOStandard("LVCMOS33")),
-
     # I2C.
     ("i2c", 0,
         Subsignal("scl", Pins("N17"), Misc("PULLUP=True")),
         Subsignal("sda", Pins("T16"), Misc("PULLUP=True")),
         IOStandard("LVCMOS33")
     ),
 
@@ -156,15 +153,15 @@
 
 # Platform -----------------------------------------------------------------------------------------
 
 class Platform(Xilinx7SeriesPlatform):
     default_clk_name   = "clk200"
     default_clk_period = 1e9/200e6
 
-    def __init__(self, toolchain="vivado", with_multiboot=True):
+    def __init__(self,toolchain="vivado"):
         Xilinx7SeriesPlatform.__init__(self, "xc7a100t-fgg484-2", _io, toolchain=toolchain)
         self.add_platform_command("set_property INTERNAL_VREF 0.750 [get_iobanks 34]")
         self.add_platform_command("set_property INTERNAL_VREF 0.750 [get_iobanks 35]")
 
         self.toolchain.bitstream_commands = [
             "set_property BITSTREAM.CONFIG.SPI_BUSWIDTH 4 [current_design]",
             "set_property BITSTREAM.CONFIG.CONFIGRATE 16 [current_design]",
@@ -172,28 +169,26 @@
             "set_property CFGBVS VCCO [current_design]",
             "set_property CONFIG_VOLTAGE 3.3 [current_design]",
         ]
 
         self.toolchain.additional_commands = [
             # Non-Multiboot SPI-Flash bitstream generation.
             "write_cfgmem -force -format bin -interface spix4 -size 16 -loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin",
+
+            # Multiboot SPI-Flash Operational bitstream generation.
+            "set_property BITSTREAM.CONFIG.TIMER_CFG 0x0001fbd0 [current_design]",
+            "set_property BITSTREAM.CONFIG.CONFIGFALLBACK Enable [current_design]",
+            "write_bitstream -force {build_name}_operational.bit ",
+            "write_cfgmem -force -format bin -interface spix4 -size 16 -loadbit \"up 0x0 {build_name}_operational.bit\" -file {build_name}_operational.bin",
+
+            # Multiboot SPI-Flash Fallback bitstream generation.
+            "set_property BITSTREAM.CONFIG.NEXT_CONFIG_ADDR 0x00400000 [current_design]",
+            "write_bitstream -force {build_name}_fallback.bit ",
+            "write_cfgmem -force -format bin -interface spix4 -size 16 -loadbit \"up 0x0 {build_name}_fallback.bit\" -file {build_name}_fallback.bin"
         ]
-        if with_multiboot:
-            self.toolchain.additional_commands += [
-                # Multiboot SPI-Flash Operational bitstream generation.
-                "set_property BITSTREAM.CONFIG.TIMER_CFG 0x0001fbd0 [current_design]",
-                "set_property BITSTREAM.CONFIG.CONFIGFALLBACK Enable [current_design]",
-                "write_bitstream -force {build_name}_operational.bit ",
-                "write_cfgmem -force -format bin -interface spix4 -size 16 -loadbit \"up 0x0 {build_name}_operational.bit\" -file {build_name}_operational.bin",
-
-                # Multiboot SPI-Flash Fallback bitstream generation.
-                "set_property BITSTREAM.CONFIG.NEXT_CONFIG_ADDR 0x00400000 [current_design]",
-                "write_bitstream -force {build_name}_fallback.bit ",
-                "write_cfgmem -force -format bin -interface spix4 -size 16 -loadbit \"up 0x0 {build_name}_fallback.bit\" -file {build_name}_fallback.bin"
-            ]
 
     def create_programmer(self, name='openocd'):
         if name == 'openocd':
             return OpenOCD("openocd_xc7_ft232.cfg", "bscan_spi_xc7a200t.bit")
         elif name == 'vivado':
             # TODO: some board versions may have s25fl128s
             return VivadoProgrammer(flash_part='s25fl256sxxxxxx0-spi-x1_x2_x4')
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/opalkelly_xem8320.py` & `litex-boards-2023.8/litex_boards/platforms/opalkelly_xem8320.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/pano_logic_g2.py` & `litex-boards-2023.8/litex_boards/platforms/pano_logic_g2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/qmtech_10cl006.py` & `litex-boards-2023.8/litex_boards/platforms/qmtech_10cl006.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/qmtech_5cefa2.py` & `litex-boards-2023.8/litex_boards/platforms/qmtech_5cefa2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/qmtech_5cefa5.py` & `litex-boards-2023.8/litex_boards/platforms/qmtech_5cefa5.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/qmtech_artix7_fbg484.py` & `litex-boards-2023.8/litex_boards/platforms/qmtech_artix7_fbg484.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,25 +157,24 @@
         if with_daughterboard:
             from litex_boards.platforms.qmtech_daughterboard import QMTechDaughterboard
             daughterboard = QMTechDaughterboard(IOStandard("LVCMOS33"))
             io += daughterboard.io
             connectors += daughterboard.connectors
 
         Xilinx7SeriesPlatform.__init__(self, device, io, connectors, toolchain=toolchain)
-
         self.toolchain.bitstream_commands = \
             ["set_property BITSTREAM.CONFIG.SPI_BUSWIDTH 4 [current_design]",
-            "set_property BITSTREAM.GENERAL.COMPRESS TRUE [current_design]"]
+             "set_property BITSTREAM.GENERAL.COMPRESS TRUE [current_design]"]
         self.toolchain.additional_commands = \
             ["write_cfgmem -force -format bin -interface spix4 -size 16 "
-            "-loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin"]
-
+             "-loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin"]
         self.add_platform_command("set_property INTERNAL_VREF 0.750 [get_iobanks 16]")
         self.add_platform_command("set_property CFGBVS VCCO [current_design]")
         self.add_platform_command("set_property CONFIG_VOLTAGE 3.3 [current_design]")
+        self.toolchain.f4pga_device = device
 
     def create_programmer(self):
         bscan_spi = f"bscan_spi_xc7a{self.kgates}t.bit"
         return OpenOCD("openocd_xc7_ft2232.cfg", bscan_spi)
 
 
     def do_finalize(self, fragment):
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/qmtech_artix7_fgg676.py` & `litex-boards-2023.8/litex_boards/platforms/qmtech_artix7_fgg676.py`

 * *Files 12% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 # Platform -----------------------------------------------------------------------------------------
 
 class Platform(Xilinx7SeriesPlatform):
     default_clk_name   = "clk50"
     default_clk_period = 1e9/50e6
     kgates             = None
 
-    def __init__(self, kgates=100, toolchain="vivado", with_daughterboard=False, with_rp2040_daughterboard=False):
+    def __init__(self, kgates=100, toolchain="vivado", with_daughterboard=False):
         assert(kgates in [75, 100], "kgates can only be 75 or 100 representing a XC7A75T, XC7TA100T")
         self.kgates = kgates
         device = f"xc7a{kgates}tfgg676-1"
         io = _io
         connectors = _connectors
 
         core_leds_name = "onboard_led" if with_daughterboard else "user_led"
@@ -156,34 +156,27 @@
 
         if with_daughterboard:
             from litex_boards.platforms.qmtech_daughterboard import QMTechDaughterboard
             daughterboard = QMTechDaughterboard(IOStandard("LVCMOS33"))
             io += daughterboard.io
             connectors += daughterboard.connectors
 
-        if with_rp2040_daughterboard:
-            from litex_boards.platforms.qmtech_rp2040_daughterboard import QMTechDaughterboard
-            daughterboard = QMTechDaughterboard(IOStandard("LVCMOS33"))
-            io += daughterboard.io
-            connectors += daughterboard.connectors
-
         Xilinx7SeriesPlatform.__init__(self, device, io, connectors, toolchain=toolchain)
-
         self.toolchain.bitstream_commands = \
             ["set_property BITSTREAM.CONFIG.SPI_BUSWIDTH 4 [current_design]",
-            "set_property BITSTREAM.GENERAL.COMPRESS TRUE [current_design]"]
+             "set_property BITSTREAM.GENERAL.COMPRESS TRUE [current_design]"]
         self.toolchain.additional_commands = \
             ["write_cfgmem -force -format bin -interface spix4 -size 16 "
-            "-loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin"]
-
+             "-loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin"]
         self.add_platform_command("set_property INTERNAL_VREF 0.750 [get_iobanks 16]")
         self.add_platform_command("set_property CFGBVS VCCO [current_design]")
         self.add_platform_command("set_property CONFIG_VOLTAGE 3.3 [current_design]")
+        self.toolchain.f4pga_device = device
 
     def create_programmer(self):
         bscan_spi = f"bscan_spi_xc7a{self.kgates}t.bit"
         return OpenOCD("openocd_xc7_ft2232.cfg", bscan_spi)
 
 
     def do_finalize(self, fragment):
         Xilinx7SeriesPlatform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk50", loose=True), 1e9/50e6)
+        self.add_period_constraint(self.lookup_request("clk50", loose=True), 1e9/50e6)
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/qmtech_daughterboard.py` & `litex-boards-2023.8/litex_boards/platforms/qmtech_daughterboard.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/qmtech_ep4ce15_starter_kit.py` & `litex-boards-2023.8/litex_boards/platforms/qmtech_ep4ce15_starter_kit.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/qmtech_ep4cex5.py` & `litex-boards-2023.8/litex_boards/platforms/qmtech_ep4cex5.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/qmtech_ep4cgx150.py` & `litex-boards-2023.8/litex_boards/platforms/qmtech_ep4cgx150.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/qmtech_wukong.py` & `litex-boards-2023.8/litex_boards/platforms/qmtech_wukong.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,21 +203,19 @@
     def __init__(self, board_version=1, speed_grade=-2, toolchain="vivado"):
         io = _io_common
         if board_version < 2:
             io.extend(_io_v1)
         else:
             io.extend(_io_v2)
         Xilinx7SeriesPlatform.__init__(self, "xc7a100t{}fgg676".format(speed_grade), io, _connectors,  toolchain=toolchain)
-
         self.toolchain.bitstream_commands = \
             ["set_property BITSTREAM.CONFIG.SPI_BUSWIDTH 4 [current_design]"]
         self.toolchain.additional_commands = \
             ["write_cfgmem -force -format bin -interface spix4 -size 16 "
-            "-loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin"]
-
+             "-loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin"]
         self.add_platform_command("set_property INTERNAL_VREF 0.675 [get_iobanks 16]")
         if board_version < 2:
             self.add_platform_command("set_property CLOCK_DEDICATED_ROUTE FALSE [get_nets clk50_IBUF]")
         self.add_platform_command("set_property CFGBVS VCCO [current_design]")
         self.add_platform_command("set_property CONFIG_VOLTAGE 3.3 [current_design]")
 
     def create_programmer(self):
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/qmtech_xc7a35t.py` & `litex-boards-2023.8/litex_boards/platforms/qmtech_xc7a35t.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,24 +155,23 @@
             daughterboard = QMTechDaughterboard(IOStandard("LVCMOS33"))
             io += daughterboard.io
             connectors += daughterboard.connectors
         else:
             io += self.core_resources
 
         Xilinx7SeriesPlatform.__init__(self, device, io, connectors, toolchain=toolchain)
-
         self.toolchain.bitstream_commands = \
             ["set_property BITSTREAM.CONFIG.SPI_BUSWIDTH 4 [current_design]"]
         self.toolchain.additional_commands = \
             ["write_cfgmem -force -format bin -interface spix4 -size 16 "
-            "-loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin"]
-
+             "-loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin"]
         self.add_platform_command("set_property INTERNAL_VREF 0.675 [get_iobanks 15]")
         self.add_platform_command("set_property CFGBVS VCCO [current_design]")
         self.add_platform_command("set_property CONFIG_VOLTAGE 3.3 [current_design]")
+        self.toolchain.f4pga_device = device
 
     def create_programmer(self):
         bscan_spi = "bscan_spi_xc7a35t.bit"
         return OpenOCD("openocd_xc7_ft2232.cfg", bscan_spi)
 
 
     def do_finalize(self, fragment):
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/qmtech_xc7k325t.py` & `litex-boards-2023.8/litex_boards/platforms/qmtech_xc7k325t.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,20 +161,14 @@
             io += daughterboard.io
             connectors += daughterboard.connectors
         else:
             io += self.core_resources_standalone
 
         XilinxPlatform.__init__(self, device, io, connectors, toolchain=toolchain)
 
-        self.toolchain.bitstream_commands = \
-            ["set_property BITSTREAM.CONFIG.SPI_BUSWIDTH 4 [current_design]"]
-        self.toolchain.additional_commands = \
-            ["write_cfgmem -force -format bin -interface spix4 -size 16 "
-            "-loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin"]
-
         self.add_platform_command("set_property INTERNAL_VREF 0.750 [get_iobanks 34]")
         self.add_platform_command("set_property INTERNAL_VREF 0.90  [get_iobanks 33]")
 
     def create_programmer(self):
         bscan_spi = "bscan_spi_xc7k325t.bit"
         return OpenOCD("openocd_xc7_ft2232.cfg", bscan_spi)
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/quicklogic_quickfeather.py` & `litex-boards-2023.8/litex_boards/platforms/quicklogic_quickfeather.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/qwertyembedded_beaglewire.py` & `litex-boards-2023.8/litex_boards/platforms/qwertyembedded_beaglewire.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/radiona_ulx3s.py` & `litex-boards-2023.8/litex_boards/platforms/trellisboard.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,217 +1,274 @@
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2018-2019 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2019 David Shah <dave@ds0.me>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from litex.build.generic_platform import *
 from litex.build.lattice import LatticeECP5Platform
-from litex.build.lattice.programmer import UJProg
+from litex.build.lattice.programmer import OpenOCDJTAGProgrammer
 
 # IOs ----------------------------------------------------------------------------------------------
 
-_io_common = [
+_io = [
     # Clk / Rst
-    ("clk25", 0, Pins("G2"), IOStandard("LVCMOS33")),
-    ("rst",   0, Pins("R1"), IOStandard("LVCMOS33")),
-
-    # Buttons
-    ("user_btn", 0, Pins( "D6"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # PWR
-    ("user_btn", 1, Pins( "R1"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # F1
-    ("user_btn", 2, Pins( "T1"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # F2
-    ("user_btn", 3, Pins("R18"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # UP
-    ("user_btn", 4, Pins( "V1"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # DOWN
-    ("user_btn", 5, Pins( "U1"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # LEFT
-    ("user_btn", 6, Pins("H16"), IOStandard("LVCMOS33"), Misc("PULLMODE=DOWN")), # RIGHT
+    ("clk100", 0, Pins("B29"), IOStandard("LVDS")), # [broken on rev1.0 (non diff pair)]
+    ("clk12",  0, Pins("B3"),  IOStandard("LVCMOS33")),
+    ("clkref", 0, Pins("E17"), IOStandard("LVCMOS33")),
 
     # Leds
-    ("user_led", 0, Pins("B2"), IOStandard("LVCMOS33")),
-    ("user_led", 1, Pins("C2"), IOStandard("LVCMOS33")),
-    ("user_led", 2, Pins("C1"), IOStandard("LVCMOS33")),
-    ("user_led", 3, Pins("D2"), IOStandard("LVCMOS33")),
-    ("user_led", 4, Pins("D1"), IOStandard("LVCMOS33")),
-    ("user_led", 5, Pins("E2"), IOStandard("LVCMOS33")),
-    ("user_led", 6, Pins("E1"), IOStandard("LVCMOS33")),
-    ("user_led", 7, Pins("H3"), IOStandard("LVCMOS33")),
+    ("user_led",  0, Pins("C26"),  IOStandard("LVCMOS33"), Misc("PULLMODE=NONE")),
+    ("user_led",  1, Pins("D26"),  IOStandard("LVCMOS33"), Misc("PULLMODE=NONE")),
+    ("user_led",  2, Pins("A28"),  IOStandard("LVCMOS33"), Misc("PULLMODE=NONE")),
+    ("user_led",  3, Pins("A29"),  IOStandard("LVCMOS33"), Misc("PULLMODE=NONE")),
+    ("user_led",  4, Pins("A30"),  IOStandard("LVCMOS33"), Misc("PULLMODE=NONE")),
+    ("user_led",  5, Pins("AK29"), IOStandard("LVCMOS33"), Misc("PULLMODE=NONE")),
+    ("user_led",  6, Pins("AH32"), IOStandard("LVCMOS33"), Misc("PULLMODE=NONE")),
+    ("user_led",  7, Pins("AH30"), IOStandard("LVCMOS33"), Misc("PULLMODE=NONE")),
+    ("user_led",  8, Pins("AH28"), IOStandard("LVCMOS33"), Misc("PULLMODE=NONE")),
+    ("user_led",  9, Pins("AG30"), IOStandard("LVCMOS33"), Misc("PULLMODE=NONE")),
+    ("user_led", 10, Pins("AG29"), IOStandard("LVCMOS33"), Misc("PULLMODE=NONE")),
+    ("user_led", 11, Pins("AK30"), IOStandard("LVCMOS33"), Misc("PULLMODE=NONE")),
+
+    # Buttons
+    ("user_btn", 0, Pins("Y32"),  IOStandard("SSTL135_I")),
+    ("user_btn", 1, Pins("W31"),  IOStandard("SSTL135_I")),
+    ("user_btn", 2, Pins("AD30"), IOStandard("SSTL135_I")),
+    ("user_btn", 3, Pins("AD29"), IOStandard("SSTL135_I")),
+
+    # Switches
+    ("user_dip", 0, Pins("AE31"), IOStandard("SSTL135_I")),
+    ("user_dip", 1, Pins("AE32"), IOStandard("SSTL135_I")),
+    ("user_dip", 2, Pins("AD32"), IOStandard("SSTL135_I")),
+    ("user_dip", 3, Pins("AC32"), IOStandard("SSTL135_I")),
+    ("user_dip", 4, Pins("AB32"), IOStandard("SSTL135_I")),
+    ("user_dip", 5, Pins("AB31"), IOStandard("SSTL135_I")),
+    ("user_dip", 6, Pins("AC31"), IOStandard("SSTL135_I")),
+    ("user_dip", 7, Pins("AC30"), IOStandard("SSTL135_I")),
 
     # Serial
     ("serial", 0,
-        Subsignal("tx", Pins("L4"), IOStandard("LVCMOS33")),
-        Subsignal("rx", Pins("M1"), IOStandard("LVCMOS33"))
+        Subsignal("rx", Pins("AM28"), IOStandard("LVCMOS33")),
+        Subsignal("tx", Pins("AL28"), IOStandard("LVCMOS33")),
     ),
 
-    # SDR SDRAM
-    ("sdram_clock", 0, Pins("F19"), IOStandard("LVCMOS33")),
-    ("sdram", 0,
-        Subsignal("a",     Pins(
-            "M20 M19 L20 L19 K20 K19 K18 J20",
-            "J19 H20 N19 G20 G19")),
-        Subsignal("dq",    Pins(
-            "J16 L18 M18 N18 P18 T18 T17 U20",
-            "E19 D20 D19 C20 E18 F18 J18 J17")),
-        Subsignal("we_n",  Pins("T20")),
-        Subsignal("ras_n", Pins("R20")),
-        Subsignal("cas_n", Pins("T19")),
-        Subsignal("cs_n",  Pins("P20")),
-        Subsignal("cke",   Pins("F20")),
-        Subsignal("ba",    Pins("P19 N20")),
-        Subsignal("dm",    Pins("U19 E20")),
-        IOStandard("LVCMOS33"),
+    # USB FIFO
+    ("usb_fifo", 0,
+        Subsignal("dq",    Pins("AM28 AL28 AM29 AK28 AK32 AM30 AJ32 AL30"), IOStandard("LVCMOS33")),
+        Subsignal("txe_n", Pins("AM31"),  IOStandard("LVCMOS33")),
+        Subsignal("rxf_n", Pins("AJ31"),  IOStandard("LVCMOS33")),
+        Subsignal("rd_n",  Pins("AL32"),  IOStandard("LVCMOS33")),
+        Subsignal("wr_n",  Pins("AG28"),  IOStandard("LVCMOS33")),
+        Subsignal("siwu_n", Pins("AJ28"), IOStandard("LVCMOS33")),
+    ),
+
+    # DDR3 SDRAM
+    ("dram_vtt_en", 0, Pins("E25"), IOStandard("LVCMOS33")),
+    ("ddram", 0,
+        Subsignal("a", Pins(
+            "E30 F28 C32 E29 F32 D30 E32 D29",
+            "D32 C31 H32 F31 F29 B32 D31"),
+            IOStandard("SSTL135_I")),
+        Subsignal("ba",    Pins("H31 H30 J30"), IOStandard("SSTL135_I")),
+        Subsignal("ras_n", Pins("K31"), IOStandard("SSTL135_I")),
+        Subsignal("cas_n", Pins("K30"), IOStandard("SSTL135_I")),
+        Subsignal("we_n",  Pins("J32"), IOStandard("SSTL135_I")),
+        Subsignal("cs_n",  Pins("K29"), IOStandard("SSTL135_I")),
+        Subsignal("dm", Pins("R26 L27 Y27 U31"), IOStandard("SSTL135_I")),
+        Subsignal("dq", Pins(
+            " V26  R27  V27  T26  U28  T27  T29  U26",
+            " P27  K28  P26  L26  K27  N26  L29  K26",
+            "AC27  W28 AC26  Y26 AB26  W29 AD26  Y28",
+            " T32  U32  P31  V32  P32  W32  N32  U30"),
+            IOStandard("SSTL135_I"),
+            Misc("TERMINATION=75")),
+        Subsignal("dqs_p", Pins("R29 N30 AB28 R32"), IOStandard("SSTL135D_I"),
+            Misc("TERMINATION=OFF"),
+            Misc("DIFFRESISTOR=100")),
+        Subsignal("clk_p", Pins("L31"), IOStandard("SSTL135D_I")),
+        Subsignal("cke",   Pins("K32"), IOStandard("SSTL135_I")),
+        Subsignal("odt",   Pins("J29"), IOStandard("SSTL135_I")),
+        Subsignal("reset_n", Pins("L32"), IOStandard("SSTL135_I")),
         Misc("SLEWRATE=FAST"),
     ),
 
-    # GPIOs
-    ("gpio", 0,
-        Subsignal("p", Pins("B11")),
-        Subsignal("n", Pins("C11")),
+    # RGMII Ethernet
+    ("eth_clocks", 0,
+        Subsignal("tx",  Pins("A15")),
+        Subsignal("rx",  Pins("C17")),
+        Subsignal("ref", Pins("A17")),
         IOStandard("LVCMOS33")
     ),
-    ("gpio", 1,
-        Subsignal("p", Pins("A10")),
-        Subsignal("n", Pins("A11")),
+    ("eth", 0,
+        Subsignal("rst_n",   Pins("D16")),
+        Subsignal("int_n",   Pins("E16")),
+        Subsignal("mdio",    Pins("F17")),
+        Subsignal("mdc",     Pins("B17")),
+        Subsignal("rx_ctl",  Pins("A16")),
+        Subsignal("rx_data", Pins("C16 B16 B14 F16")),
+        Subsignal("tx_ctl",  Pins("D15")),
+        Subsignal("tx_data", Pins("A14 F15 C15 C14")),
         IOStandard("LVCMOS33")
     ),
-    ("gpio", 2,
-        Subsignal("p", Pins("A9")),
-        Subsignal("n", Pins("B10")),
+
+    # I2C Clock Generator
+    ("clkgen", 0,
+        Subsignal("sda",   Pins("C22")),
+        Subsignal("scl",   Pins("A22")),
+        Subsignal("sd_oe", Pins("A2")),
         IOStandard("LVCMOS33")
     ),
-    ("gpio", 3,
-        Subsignal("p", Pins("B9")),
-        Subsignal("n", Pins("C10")),
-        IOStandard("LVCMOS33")
+
+    # PCIe
+    ("pcie_x2", 0,
+        Subsignal("clk_p",  Pins("AM14")),
+        Subsignal("clk_n",  Pins("AM15")),
+        Subsignal("rx_p",   Pins("AM8  AK12")),
+        Subsignal("rx_n",   Pins("AM9  AK13")),
+        Subsignal("tx_p",   Pins("AK9  AM11")),
+        Subsignal("tx_n",   Pins("AK10 AM12")),
+        Subsignal("perst",  Pins("D22"), IOStandard("LVCMOS33")),
+        Subsignal("wake_n", Pins("A23"), IOStandard("LVCMOS33")),
+    ),
+
+    # M2
+    ("m2", 0,
+        Subsignal("clk_p", Pins("AM23")),
+        Subsignal("clk_n", Pins("AM24")),
+        Subsignal("rx_p",  Pins("AM17 AK21")),
+        Subsignal("rx_n",  Pins("AM18 AK22")),
+        Subsignal("tx_p",  Pins("AK18 AM20")),
+        Subsignal("tx_n",  Pins("AK19 AM21")),
+
+        Subsignal("clksel", Pins("N3"), IOStandard("LVCMOS33")),
+
+        Subsignal("sdio_clk", Pins("L4"), IOStandard("LVCMOS33")),
+        Subsignal("sdio_cmd", Pins("K4"), IOStandard("LVCMOS33")),
+        Subsignal("sdio_dq",  Pins("L7 N4 L6 N6"), IOStandard("LVCMOS33")),
+
+        Subsignal("uart_tx",    Pins("P6"), IOStandard("LVCMOS33")),
+        Subsignal("uart_rx",    Pins("K5"), IOStandard("LVCMOS33")),
+        Subsignal("uart_rts_n", Pins("N7"), IOStandard("LVCMOS33")),
+        Subsignal("uart_cts_n", Pins("P7"), IOStandard("LVCMOS33"))
     ),
 
-    # USB
-    ("usb", 0,
-        Subsignal("d_p", Pins("D15")),
-        Subsignal("d_n", Pins("E15")),
-        Subsignal("pullup", Pins("B12 C12")),
-        IOStandard("LVCMOS33")
+    # SDCard
+    ("spisdcard", 0,
+        Subsignal("clk",  Pins("AK3")),
+        Subsignal("mosi", Pins("AH3"), Misc("PULLMODE=UP")),
+        Subsignal("cs_n", Pins("AK1"), Misc("PULLMODE=UP")),
+        Subsignal("miso", Pins("AG1"), Misc("PULLMODE=UP")),
+        Misc("SLEWRATE=FAST"),
+        IOStandard("LVCMOS33"),
+    ),
+    ("sdcard", 0,
+        Subsignal("clk",  Pins("AK3")),
+        Subsignal("cmd",  Pins("AH3"), Misc("PULLMODE=UP")),
+        Subsignal("data", Pins("AG1 AJ1 AH1 AK1"), Misc("PULLMODE=UP")),
+        Misc("SLEWRATE=FAST"),
+        IOStandard("LVCMOS33"),
     ),
 
+
     # SPIFlash
     ("spiflash", 0,
-        Subsignal("cs_n", Pins("R2")),
-        Subsignal("miso", Pins("V2")),
-        Subsignal("mosi", Pins("W2")),
-        Subsignal("wp", Pins("Y2")),
-        Subsignal("hold", Pins("W1")),
+        Subsignal("clk",  Pins("AM3")),
+        Subsignal("cs_n", Pins("AJ3")),
+        Subsignal("mosi", Pins("AK2")),
+        Subsignal("miso", Pins("AJ2")),
+        Subsignal("wp",   Pins("AM2")),
+        Subsignal("hold", Pins("AL1")),
         IOStandard("LVCMOS33")
     ),
     ("spiflash4x", 0,
-        Subsignal("cs_n", Pins("R2")),
-        Subsignal("dq", Pins("W2", "V2", "Y2", "W1")),
+        Subsignal("clk",  Pins("AM3")),
+        Subsignal("cs_n", Pins("AJ3")),
+        Subsignal("dq",   Pins("AK2 AJ2 AM2 AL1")),
         IOStandard("LVCMOS33")
     ),
 
-    # OLED
-    ("oled_spi", 0,
-        Subsignal("clk",  Pins("P4")),
-        Subsignal("mosi", Pins("P3")),
-        IOStandard("LVCMOS33"),
-    ),
-    ("oled_ctl", 0,
-        Subsignal("dc",   Pins("P1")),
-        Subsignal("resn", Pins("P2")),
-        Subsignal("csn",  Pins("N2")),
-        IOStandard("LVCMOS33"),
+    # USB ULPI
+    ("ulpi", 0,
+        Subsignal("clk",   Pins("A18")),
+        Subsignal("stp",   Pins("D18")),
+        Subsignal("dir",   Pins("C18")),
+        Subsignal("nxt",   Pins("F18")),
+        Subsignal("reset", Pins("D17")),
+        Subsignal("data",  Pins("C20 C19 E19 D20 A20 B19 D19 A19")),
+        IOStandard("LVCMOS33")
     ),
 
-    # Others
-    ("ext0p", 0, Pins("B11"), IOStandard("LVCMOS33")),
-    ("ext1p", 0, Pins("A10"), IOStandard("LVCMOS33")),
+    # HDMI
+    ("hdmi", 0,
+        Subsignal("r", Pins("F10  F9  D9  D8  C7  F8  E8 D11")),
+        Subsignal("g", Pins("B8   A7  C8  C9 F11 E11 E10 D10")),
+        Subsignal("b", Pins("C11 A11 B11 A10 B10 C10  A8  B7")),
+        Subsignal("de",      Pins("F14")),
+        Subsignal("clk",     Pins("A9")),
+        Subsignal("vsync_n", Pins("E14")),
+        Subsignal("hsync_n", Pins("F13")),
+        Subsignal("sda", Pins("D13")),
+        Subsignal("scl", Pins("C13")),
+        IOStandard("LVCMOS33")
+    ),
 ]
 
-_io_1_7 = [
-    # SDCard
-    ("spisdcard", 0,
-        Subsignal("clk",  Pins("J1")),
-        Subsignal("mosi", Pins("J3"), Misc("PULLMODE=UP")),
-        Subsignal("cs_n", Pins("H1"), Misc("PULLMODE=UP")),
-        Subsignal("miso", Pins("K2"), Misc("PULLMODE=UP")),
-        Misc("SLEWRATE=FAST"),
-        IOStandard("LVCMOS33"),
-    ),
-    ("sdcard", 0,
-        Subsignal("clk",  Pins("J1")),
-        Subsignal("cmd",  Pins("J3"), Misc("PULLMODE=UP")),
-        Subsignal("data", Pins("K2 K1 H2 H1"), Misc("PULLMODE=UP")),
-        Misc("SLEWRATE=FAST"),
-        IOStandard("LVCMOS33"),
-    ),
+# Connectors ---------------------------------------------------------------------------------------
 
-    # GPDI
-    ("gpdi", 0,
-        Subsignal("clk_p",    Pins("A17"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        #Subsignal("clk_n",   Pins("B18"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        Subsignal("data0_p",  Pins("A12"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        #Subsignal("data0_n", Pins("A13"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        Subsignal("data1_p",  Pins("A14"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        #Subsignal("data1_n", Pins("C14"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        Subsignal("data2_p",  Pins("A16"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        #Subsignal("data2_n", Pins("B16"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        #Subsignal("cec",     Pins("A18"), IOStandard("LVCMOS33"), Misc("PULLMODE=UP")),
-        #Subsignal("scl",     Pins("E19"), IOStandard("LVCMOS33"), Misc("PULLMODE=UP")),
-        #Subsignal("sda",     Pins("B19"), IOStandard("LVCMOS33"), Misc("PULLMODE=UP"))
-    ),
-    # Wifi power
-    ("wifi_gpio0", 0, Pins("L2"), IOStandard("LVCMOS33")),
+_connectors = [
+    ("pmoda", "F19 F20 B22 C23 D14 A13 E22 D23"),
+    ("pmodb", "C25 A26 F23 F25 B25 D25 F22 F24"),
+    ("pmodx", "A24 C24 D24 B23 D23 A25"),
+
+    ("ext0", "T1 U1 AE5 AE4 AB5 AB6 Y5 W5 W2 Y1 AB7 AC6 AB3 AB4 AD3 AE3 AB1 AC1 AD1 AE1 AD6 AE6 AC7 AD7"),
+    ("ext1", "P5 P4 R7 T7 R6 T6 U6 U7 R4 T5 T4 U5 U4 V4 V6 V7 P2 P3 R3 T3 N1 P1 U2 U3"),
+    ("ext2", "K6 K7 J7 J6 H6 H5 F4 F5 F3 E3 C4 C3 C5 D5 D3 D2 H2 H3 J3 K3 B1 C2 F1 H1")
 ]
 
-_io_2_0 = [
-    # SDCard
-    ("spisdcard", 0,
-        Subsignal("clk",  Pins("H2")),
-        Subsignal("mosi", Pins("J1"), Misc("PULLMODE=UP")),
-        Subsignal("cs_n", Pins("K2"), Misc("PULLMODE=UP")),
-        Subsignal("miso", Pins("J3"), Misc("PULLMODE=UP")),
-        Misc("SLEWRATE=FAST"),
-        IOStandard("LVCMOS33"),
-    ),
-    ("sdcard", 0,
-        Subsignal("clk",  Pins("H2")),
-        Subsignal("cmd",  Pins("J1"), Misc("PULLMODE=UP")),
-        Subsignal("data", Pins("J3 H1 K1 K2"), Misc("PULLMODE=UP")),
-        #Subsignal("cd", Pins("N5")), # Not connected
-        #Subsignal("wp", Pins("P5")), # Not connected
-        Misc("SLEWRATE=FAST"),
-        IOStandard("LVCMOS33"),
-    ),
 
-    # GPDI
-    ("gpdi", 0,
-        Subsignal("clk_p",    Pins("A17"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        #Subsignal("clk_n",   Pins("B18"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        Subsignal("data0_p",  Pins("A16"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        #Subsignal("data0_n", Pins("B16"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        Subsignal("data1_p",  Pins("A14"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        #Subsignal("data1_n", Pins("C14"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        Subsignal("data2_p",  Pins("A12"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        #Subsignal("data2_n", Pins("A13"), IOStandard("LVCMOS33D"), Misc("DRIVE=4")),
-        #Subsignal("cec",     Pins("A18"), IOStandard("LVCMOS33"), Misc("PULLMODE=UP")),
-        #Subsignal("scl",     Pins("E19"), IOStandard("LVCMOS33"), Misc("PULLMODE=UP")),
-        #Subsignal("sda",     Pins("B19"), IOStandard("LVCMOS33"), Misc("PULLMODE=UP"))
-    ),
-    # Wifi power
-    ("wifi_gpio0", 0, Pins("F1"), IOStandard("LVCMOS33")),    
+# PMODS --------------------------------------------------------------------------------------------
+
+def raw_pmod_io(pmod):
+    return [(pmod, 0, Pins(" ".join([f"{pmod}:{i:d}" for i in range(8)])), IOStandard("LVCMOS33"))]
+
+def sdcard_pmod_io(pmod):
+    return [
+        # SDCard PMOD:
+        # - https://store.digilentinc.com/pmod-microsd-microsd-card-slot/
+        # - https://github.com/antmicro/arty-expansion-board
+        ("spisdcard", 0,
+            Subsignal("clk",  Pins(f"{pmod}:3")),
+            Subsignal("mosi", Pins(f"{pmod}:1"), Misc("PULLMODE=UP")),
+            Subsignal("cs_n", Pins(f"{pmod}:0"), Misc("PULLMODE=UP")),
+            Subsignal("miso", Pins(f"{pmod}:2"), Misc("PULLMODE=UP")),
+            Misc("SLEWRATE=FAST"),
+            IOStandard("LVCMOS33"),
+        ),
+        ("sdcard", 0,
+            Subsignal("data", Pins(f"{pmod}:2 {pmod}:4 {pmod}:5 {pmod}:0"), Misc("PULLMODE=UP")),
+            Subsignal("cmd",  Pins(f"{pmod}:1"), Misc("PULLMODE=UP")),
+            Subsignal("clk",  Pins(f"{pmod}:3")),
+            Subsignal("cd",   Pins(f"{pmod}:6")),
+            Misc("SLEWRATE=FAST"),
+            IOStandard("LVCMOS33"),
+        ),
 ]
+_sdcard_pmod_io = sdcard_pmod_io("pmoda") # SDCARD PMOD on PMODA.
 
 # Platform -----------------------------------------------------------------------------------------
 
 class Platform(LatticeECP5Platform):
-    default_clk_name   = "clk25"
-    default_clk_period = 1e9/25e6
+    default_clk_name   = "clk12"
+    default_clk_period = 1e9/12e6
 
-    def __init__(self, device="LFE5U-45F", revision="2.0", toolchain="trellis", **kwargs):
-        assert device in ["LFE5U-12F", "LFE5U-25F", "LFE5U-45F", "LFE5U-85F"]
-        assert revision in ["1.7", "2.0"]
-        _io = _io_common + {"1.7": _io_1_7, "2.0": _io_2_0}[revision]
-        LatticeECP5Platform.__init__(self, device + "-6BG381C", _io, toolchain=toolchain, **kwargs)
+    def __init__(self, toolchain="trellis", **kwargs):
+        LatticeECP5Platform.__init__(self, "LFE5UM5G-85F-8BG756C", _io, _connectors, toolchain=toolchain, **kwargs)
 
     def create_programmer(self):
-        return UJProg()
+        return OpenOCDJTAGProgrammer("openocd_trellisboard.cfg")
 
     def do_finalize(self, fragment):
         LatticeECP5Platform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk25", loose=True), 1e9/25e6)
+        self.add_period_constraint(self.lookup_request("clk100",        loose=True), 1e9/100e6)
+        self.add_period_constraint(self.lookup_request("clk12",         loose=True), 1e9/12e6)
+        self.add_period_constraint(self.lookup_request("eth_clocks:rx", loose=True), 1e9/125e6)
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/radiona_ulx4m_ld_v2.py` & `litex-boards-2023.8/litex_boards/platforms/radiona_ulx4m_ld_v2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/rcs_arctic_tern_bmc_card.py` & `litex-boards-2023.8/litex_boards/platforms/rcs_arctic_tern_bmc_card.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/redpitaya.py` & `litex-boards-2023.8/litex_boards/platforms/redpitaya.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/rz_easyfpga.py` & `litex-boards-2023.8/litex_boards/platforms/rz_easyfpga.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/saanlima_pipistrello.py` & `litex-boards-2023.8/litex_boards/platforms/saanlima_pipistrello.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/scarabhardware_minispartan6.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_zcu106.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,167 +1,138 @@
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2015 Matt O'Gorman <mog@rldn.net>
+# Copyright (c) 2022 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from litex.build.generic_platform import *
-from litex.build.xilinx import XilinxSpartan6Platform
-from litex.build.xilinx.programmer import XC3SProg
+from litex.build.xilinx import XilinxUSPPlatform, VivadoProgrammer
 
 # IOs ----------------------------------------------------------------------------------------------
 
 _io = [
     # Clk / Rst
-    ("clk32", 0, Pins("J4"), IOStandard("LVCMOS33")),
-    ("clk50", 0, Pins("K3"), IOStandard("LVCMOS33")),
+    ("rst",    0, Pins("G13"), IOStandard("LVCMOS18")),
+    ("clk125", 0,
+        Subsignal("p", Pins("H9"), IOStandard("DIFF_SSTL15")),
+        Subsignal("n", Pins("G9"), IOStandard("DIFF_SSTL15")),
+    ),
 
     # Leds
-    ("user_led", 0, Pins("P11"), IOStandard("LVCMOS33")),
-    ("user_led", 1, Pins("N9"),  IOStandard("LVCMOS33")),
-    ("user_led", 2, Pins("M9"),  IOStandard("LVCMOS33")),
-    ("user_led", 3, Pins("P9"),  IOStandard("LVCMOS33")),
-    ("user_led", 4, Pins("T8"),  IOStandard("LVCMOS33")),
-    ("user_led", 5, Pins("N8"),  IOStandard("LVCMOS33")),
-    ("user_led", 6, Pins("P8"),  IOStandard("LVCMOS33")),
-    ("user_led", 7, Pins("P7"),  IOStandard("LVCMOS33")),
-
-    # Switches
-    ("user_sw", 0, Pins("L1"), IOStandard("LVCMOS33"), Misc("PULLUP")),
-    ("user_sw", 1, Pins("L3"), IOStandard("LVCMOS33"), Misc("PULLUP")),
-    ("user_sw", 2, Pins("L4"), IOStandard("LVCMOS33"), Misc("PULLUP")),
-    ("user_sw", 3, Pins("L5"), IOStandard("LVCMOS33"), Misc("PULLUP")),
-
-
-    # SPIFlash
-    ("spiflash", 0,
-        Subsignal("cs_n", Pins("T3"), IOStandard("LVCMOS33")),
-        Subsignal("clk",  Pins("R11"), IOStandard("LVCMOS33")),
-        Subsignal("mosi", Pins("T10"), IOStandard("LVCMOS33")),
-        Subsignal("miso", Pins("P10"), IOStandard("LVCMOS33"))
-    ),
+    ("user_led", 0, Pins("AL11"), IOStandard("LVCMOS12")),
+    ("user_led", 1, Pins("AL13"), IOStandard("LVCMOS12")),
+    ("user_led", 2, Pins("AK13"), IOStandard("LVCMOS12")),
+    ("user_led", 3, Pins("AE15"), IOStandard("LVCMOS12")),
+    ("user_led", 4, Pins("AM8"),  IOStandard("LVCMOS12")),
+    ("user_led", 5, Pins("AM9"),  IOStandard("LVCMOS12")),
+    ("user_led", 6, Pins("AM10"), IOStandard("LVCMOS12")),
+    ("user_led", 7, Pins("AM11"), IOStandard("LVCMOS12")),
+
+    # Buttons
+    ("user_btn_c", 0, Pins("AL11"), IOStandard("LVCMOS12")),
+    ("user_btn_n", 0, Pins("AG13"), IOStandard("LVCMOS12")),
+    ("user_btn_s", 0, Pins("AP20"), IOStandard("LVCMOS12")),
+    ("user_btn_w", 0, Pins("AK12"), IOStandard("LVCMOS12")),
+    ("user_btn_e", 0, Pins("AC14"), IOStandard("LVCMOS12")),
 
     # Serial
     ("serial", 0,
-        Subsignal("tx", Pins("N6"), IOStandard("LVCMOS33")),  # FTDI D1
-        Subsignal("rx", Pins("M7"), IOStandard("LVCMOS33"))   # FTDI D0
-    ),
-
-    # USB FIFO
-    ("usb_fifo", 0,
-        Subsignal("data",  Pins("M7 N6 M6 P5 N5 P4 P2 P1")),
-        Subsignal("rxf_n", Pins("N3")),
-        Subsignal("txe_n", Pins("N1")),
-        Subsignal("rd_n",  Pins("M1")),
-        Subsignal("wr_n",  Pins("M2")),
-        Subsignal("siwua", Pins("M3")),
-        Misc("SLEW=FAST"),
-        Drive(8),
-        IOStandard("LVCMOS33"),
-    ),
-
-    # ADC
-    ("adc", 0,
-        Subsignal("cs_n", Pins("F6"), IOStandard("LVCMOS33")),
-        Subsignal("clk",  Pins("G6"), IOStandard("LVCMOS33")),
-        Subsignal("mosi", Pins("H4"), IOStandard("LVCMOS33")),
-        Subsignal("miso", Pins("H5"), IOStandard("LVCMOS33"))
-    ),
-
-    # Audio
-    ("audio", 0,
-        Subsignal("a0", Pins("B8"), IOStandard("LVCMOS33")),
-        Subsignal("a1", Pins("A8"), IOStandard("LVCMOS33"))
-    ),
-
-    # SDR SDRAM
-    ("sdram_clock", 0, Pins("G16"), IOStandard("LVCMOS33"), Misc("SLEW=FAST")),
-    ("sdram", 0,
-        Subsignal("a", Pins(
-            "T15 R16 P15 P16 N16 M15 M16 L16",
-            "K15 K16 R15 J16 H15")),
-        Subsignal("dq", Pins(
-            "T13 T12 R12  T9  R9  T7  R7  T6",
-            "F16 E15 E16 D16 B16 B15 C16 C15")),
-        Subsignal("we_n",  Pins("R5")),
-        Subsignal("ras_n", Pins("R2")),
-        Subsignal("cas_n", Pins("T4")),
-        Subsignal("cs_n",  Pins("R1")),
-        Subsignal("cke",   Pins("H16")),
-        Subsignal("ba",    Pins("R14 T14")),
-        Subsignal("dm",    Pins("T5 F15")),
-        Misc("SLEW=FAST"),
-        IOStandard("LVCMOS33"),
-    ),
-
-    # SDCard
-    ("spisdcard", 0,
-        Subsignal("clk",  Pins("L12")),
-        Subsignal("mosi", Pins("K11"), Misc("PULLUP")),
-        Subsignal("cs_n", Pins("K12"), Misc("PULLUP")),
-        Subsignal("miso", Pins("M10"), Misc("PULLUP")),
-        Misc("SLEW=FAST"),
-        IOStandard("LVCMOS33"),
-    ),
-    ("sdcard", 0,
-        Subsignal("data", Pins("M10 L10 J11 K12"), Misc("PULLUP")),
-        Subsignal("cmd",  Pins("K11"), Misc("PULLUP")),
-        Subsignal("clk",  Pins("L12")),
+        Subsignal("cts", Pins("AP17")),
+        Subsignal("rts", Pins("AM15")),
+        Subsignal("tx",  Pins("AL17")),
+        Subsignal("rx",  Pins("AH17")),
+        IOStandard("LVCMOS12")
+    ),
+
+    # PCIe
+    ("pcie_x1", 0,
+        Subsignal("rst_n", Pins("L8"), IOStandard("LVCMOS33")),
+        Subsignal("clk_p", Pins("AB8")),
+        Subsignal("clk_n", Pins("AB7")),
+        Subsignal("rx_p",  Pins("AE2")),
+        Subsignal("rx_n",  Pins("AE1")),
+        Subsignal("tx_p",  Pins("AD4")),
+        Subsignal("tx_n",  Pins("AD3")),
+    ),
+    ("pcie_x2", 0,
+        Subsignal("rst_n", Pins("L8"), IOStandard("LVCMOS33")),
+        Subsignal("clk_p", Pins("AB8")),
+        Subsignal("clk_n", Pins("AB7")),
+        Subsignal("rx_p",  Pins("AE2 AF4")),
+        Subsignal("rx_n",  Pins("AE1 AF3")),
+        Subsignal("tx_p",  Pins("AD4 AE6")),
+        Subsignal("tx_n",  Pins("AD3 AE5")),
+    ),
+    ("pcie_x4", 0,
+        Subsignal("rst_n", Pins("L8"), IOStandard("LVCMOS33")),
+        Subsignal("clk_p", Pins("AB8")),
+        Subsignal("clk_n", Pins("AB7")),
+        Subsignal("rx_p",  Pins("AE2 AF4 AG2 AJ2")),
+        Subsignal("rx_n",  Pins("AE1 AF3 AG1 AJ1")),
+        Subsignal("tx_p",  Pins("AD4 AE6 AG6 AH4")),
+        Subsignal("tx_n",  Pins("AD3 AE5 AG5 AH3")),
+    ),
+
+    # DDR4 SDRAM
+    ("ddram", 0,
+        Subsignal("a",       Pins(
+            "AK9 AG11 AJ10 AL8 AK10 AH8 AJ9 AG8",
+            "AH9 AG10 AH13 AG9 AM13 AF8"),
+            IOStandard("SSTL12_DCI")),
+        Subsignal("ba",      Pins("AK8 AL12"), IOStandard("SSTL12_DCI")),
+        Subsignal("bg",      Pins("AE14"), IOStandard("SSTL12_DCI")),
+        Subsignal("ras_n",   Pins("AF11"), IOStandard("SSTL12_DCI")), # A16
+        Subsignal("cas_n",   Pins("AE12"), IOStandard("SSTL12_DCI")), # A15
+        Subsignal("we_n",    Pins("AC12"), IOStandard("SSTL12_DCI")), # A14
+        Subsignal("cs_n",    Pins("AD12"), IOStandard("SSTL12_DCI")),
+        Subsignal("act_n",   Pins("AD14"), IOStandard("SSTL12_DCI")),
+        # Subsignal("par",     Pins("AC13"), IOStandard("SSTL12_DCI")),
+        Subsignal("dm",      Pins("AH18 AD15 AM16 AP18 AE18 AH22 AL20 AP19"),
+            IOStandard("POD12_DCI")),
+        Subsignal("dq",      Pins(
+                "AF16 AF18 AG15 AF17 AF15 AG18 AG14 AE17",
+                "AA14 AC16 AB15 AD16 AB16 AC17 AB14 AD17",
+                "AJ16 AJ17 AL15 AK17 AJ15 AK18 AL16 AL18",
+                "AP13 AP16 AP15 AN16 AN13 AM18 AN17 AN18",
+                "AB19 AD19 AC18 AC19 AA20 AE20 AA19 AD20",
+                "AF22 AH21 AG19 AG21 AE24 AG20 AE23 AF21",
+                "AL22 AJ22 AL23 AJ21 AK20 AJ19 AK19 AJ20",
+                "AP22 AN22 AP21 AP23 AM19 AM23 AN19 AN23"),
+            IOStandard("POD12_DCI"),
+            Misc("PRE_EMPHASIS=RDRV_240"),
+            Misc("EQUALIZATION=EQ_LEVEL2")),
+        Subsignal("dqs_p",   Pins("AH14 AA16 AK15 AM14 AA18 AF23 AK22 AM21"),
+            IOStandard("DIFF_POD12_DCI"),
+            Misc("PRE_EMPHASIS=RDRV_240"),
+            Misc("EQUALIZATION=EQ_LEVEL2")),
+        Subsignal("dqs_n",   Pins("AJ14 AA15 AK14 AN14 AB18 AG23 AK23 AN21"),
+            IOStandard("DIFF_POD12_DCI"),
+            Misc("PRE_EMPHASIS=RDRV_240"),
+            Misc("EQUALIZATION=EQ_LEVEL2")),
+        Subsignal("clk_p",   Pins("AH11"), IOStandard("DIFF_SSTL12_DCI")),
+        Subsignal("clk_n",   Pins("AJ11"), IOStandard("DIFF_SSTL12_DCI")),
+        Subsignal("cke",     Pins("AB13"), IOStandard("SSTL12_DCI")),
+        Subsignal("odt",     Pins("AF10"), IOStandard("SSTL12_DCI")),
+        Subsignal("reset_n", Pins("AF12"), IOStandard("LVCMOS12")),
         Misc("SLEW=FAST"),
-        IOStandard("LVCMOS33"),
     ),
-
-    # HDMI In
-    ("hdmi_in", 0,
-        Subsignal("clk_p",   Pins("C9"), IOStandard("TMDS_33")),
-        Subsignal("clk_n",   Pins("A9"), IOStandard("TMDS_33")),
-        Subsignal("data0_p", Pins("C7"), IOStandard("TMDS_33")),
-        Subsignal("data0_n", Pins("A7"), IOStandard("TMDS_33")),
-        Subsignal("data1_p", Pins("B6"), IOStandard("TMDS_33")),
-        Subsignal("data1_n", Pins("A6"), IOStandard("TMDS_33")),
-        Subsignal("data2_p", Pins("B5"), IOStandard("TMDS_33")),
-        Subsignal("data2_n", Pins("A5"), IOStandard("TMDS_33")),
-        Subsignal("scl",     Pins("C1"), IOStandard("LVCMOS33")),
-        Subsignal("sda",     Pins("B1"), IOStandard("LVCMOS33"))
-    ),
-
-    # HDMI Out
-    ("hdmi_out", 0,
-        Subsignal("clk_p",  Pins("B14"), IOStandard("TMDS_33")),
-        Subsignal("clk_n",  Pins("A14"), IOStandard("TMDS_33")),
-        Subsignal("data0_p", Pins("C13"), IOStandard("TMDS_33")),
-        Subsignal("data0_n", Pins("A13"), IOStandard("TMDS_33")),
-        Subsignal("data1_p", Pins("B12"), IOStandard("TMDS_33")),
-        Subsignal("data1_n", Pins("A12"), IOStandard("TMDS_33")),
-        Subsignal("data2_p", Pins("C11"), IOStandard("TMDS_33")),
-        Subsignal("data2_n", Pins("A11"), IOStandard("TMDS_33")),
-    )
 ]
 
-# Connectors ---------------------------------------------------------------------------------------
-
-_connectors = [
-    ("A", "E7   C8  D8  E8  D9 A10 B10 C10 E10  F9 F10 D11"),
-    ("B", "E11 D14 D12 E12 E13 F13 F12 F14 G12 H14 J14"),
-    ("C", "J13 J12 K14 L14 L13 M14 M13 N14 M12 N12 P12 M11"),
-    ("D", "D6 C6 E6 C5"),
-    ("E", "D5 A4 G5 A3 B3 A2 B2 C3 C2 D3 D1 E3"),
-    ("F", "E2 E1 E4 F4 F5 G3 F3 G1 H3 H1 H2 J1")
-]
 
 # Platform -----------------------------------------------------------------------------------------
 
-class Platform(XilinxSpartan6Platform):
-    default_clk_name   = "clk32"
-    default_clk_period = 1e9/32e6
-
-    def __init__(self, device="xc6slx25", toolchain="ise"):
-        assert device in ["xc6slx9", "xc6slx25"]
-        XilinxSpartan6Platform.__init__(self, device+"-3-ftg256", _io, _connectors, toolchain=toolchain)
+class Platform(XilinxUSPPlatform):
+    default_clk_name   = "clk125"
+    default_clk_period = 1e9/125e6
+
+    def __init__(self, toolchain="vivado"):
+        XilinxUSPPlatform.__init__(self, "xczu7ev-ffvc1156-2-e", _io, toolchain=toolchain)
 
     def create_programmer(self):
-        return XC3SProg(cable="ftdi")
+        return VivadoProgrammer()
 
     def do_finalize(self, fragment):
-        XilinxSpartan6Platform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk32", loose=True), 1e9/32e6)
-        self.add_period_constraint(self.lookup_request("clk50", loose=True), 1e9/50e6)
+        XilinxUSPPlatform.do_finalize(self, fragment)
+        self.add_period_constraint(self.lookup_request("clk125", loose=True), 1e9/125e6)
+        self.add_platform_command("set_property INTERNAL_VREF 0.84 [get_iobanks 64]")
+        self.add_platform_command("set_property INTERNAL_VREF 0.84 [get_iobanks 65]")
+        self.add_platform_command("set_property INTERNAL_VREF 0.84 [get_iobanks 66]")
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/seeedstudio_spartan_edge_accelerator.py` & `litex-boards-2023.8/litex_boards/platforms/seeedstudio_spartan_edge_accelerator.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/siglent_sds1104xe.py` & `litex-boards-2023.8/litex_boards/platforms/siglent_sds1104xe.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/sipeed_tang_mega_138k.py` & `litex-boards-2023.8/litex_boards/platforms/sipeed_tang_primer_20k.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,261 +1,295 @@
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2022-2023 Icenowy Zheng <uwu@icenowy.me>
+# Copyright (c) 2022 Icenowy Zheng <icenowy@aosc.io>
 # Copyright (c) 2022 Florent Kermarrec <florent@enjoy-digital.fr>
-# Copyright (c) 2023 Gwenhael Goavec-Merou <gwenhael@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 
 from litex.build.generic_platform import *
 from litex.build.gowin.platform import GowinPlatform
 from litex.build.gowin.programmer import GowinProgrammer
 from litex.build.openfpgaloader import OpenFPGALoader
 
+
 # IOs ----------------------------------------------------------------------------------------------
 
 _io = [
     # Clk / Rst.
-    ("clk50",  0, Pins("P16"), IOStandard("LVCMOS33")),
-    ("rst",    0, Pins("U4"),  IOStandard("LVCMOS15")),
+    ("clk27",  0, Pins("H11"), IOStandard("LVCMOS33")),
 
     # Serial.
     ("serial", 0,
-        Subsignal("rx", Pins("N16")),
-        Subsignal("tx", Pins("P15")),
+        Subsignal("rx", Pins("T13")), # CARD1:1
+        Subsignal("tx", Pins("M11")), # CARD1:11
         IOStandard("LVCMOS33")
     ),
 
-    # Leds
-    ("led_n", 0,  Pins("J14"), IOStandard("LVCMOS33")),
-    ("led_n", 1,  Pins("R26"), IOStandard("LVCMOS33")),
-    ("led_n", 2,  Pins("L20"), IOStandard("LVCMOS33")),
-    ("led_n", 3,  Pins("M25"), IOStandard("LVCMOS33")),
-    ("led_n", 4,  Pins("N21"), IOStandard("LVCMOS33")),
-    ("led_n", 5,  Pins("N23"), IOStandard("LVCMOS33")),
+    # SPIFlash.
+    ("spiflash", 0,
+        Subsignal("cs_n", Pins("M9"),  IOStandard("LVCMOS33")),
+        Subsignal("clk",  Pins("L10"), IOStandard("LVCMOS33")),
+        Subsignal("miso", Pins("P10"), IOStandard("LVCMOS33")),
+        Subsignal("mosi", Pins("R10"), IOStandard("LVCMOS33")),
+    ),
+
+    # SDCard.
+    ("spisdcard", 0,
+        Subsignal("clk",  Pins("N10")),
+        Subsignal("mosi", Pins("R14")),
+        Subsignal("cs_n", Pins("N11")),
+        Subsignal("miso", Pins("M8")),
+        IOStandard("LVCMOS33"),
+    ),
+    ("sdcard", 0,
+        Subsignal("data", Pins("M8 M7 M10 N11")),
+        Subsignal("cmd",  Pins("R14")),
+        Subsignal("clk",  Pins("N10")),
+        Subsignal("cd",   Pins("D15")),
+        IOStandard("LVCMOS33"),
+    ),
 
-    # DDR3 SDRAM H5TQ4G63EFR-RDC
+    # DDR3 SDRAM IMD128M16R39CG8GNF-125.
     ("ddram", 0,
-        Subsignal("a", Pins(
-            "N1 R1 R2 N2 P1 T2 N4 U1",
-            "T4 T3 M1 P4 N3 U2 U5   "), # (M6 unused in 256x16)
-            IOStandard("SSTL15"),
-            Misc("DRIVE=12"),
-        ),
-        Subsignal("ba",      Pins("M4 L5 K3"),    IOStandard("SSTL15"), Misc("DRIVE=12")),
-        Subsignal("ras_n",   Pins("H2"),          IOStandard("SSTL15"), Misc("DRIVE=12")),
-        Subsignal("cas_n",   Pins("H1"),          IOStandard("SSTL15"), Misc("DRIVE=12")),
-        Subsignal("we_n",    Pins("J3"),          IOStandard("SSTL15"), Misc("DRIVE=12")),
-        Subsignal("cs_n",    Pins("L4"),          IOStandard("SSTL15"), Misc("DRIVE=12")),
-        Subsignal("dm",      Pins("F4 H9 E3 A3"), IOStandard("SSTL15"), Misc("DRIVE=12")),
-        Subsignal("dq",      Pins(
-            "G4 J6 L8 G5 K7 J5 K8 K6",
-            "E6 H8 H6 G8 D6 F8 G6 F7",
-            "C4 F3 B4 E5 D3 D5 A4 D4",
-            "E1 A2 G2 C2 F2 E2 G1 D1"),
+        Subsignal("a", Pins("F7 A4 D6 F8 C4 E6 B1 D8 A5 F9 K3 B7 A3 C8"),
+            IOStandard("SSTL15")),
+        Subsignal("ba", Pins("H4 D3 H5"), IOStandard("SSTL15")),
+        Subsignal("ras_n", Pins("R4"), IOStandard("SSTL15")),
+        Subsignal("cas_n", Pins("R6"), IOStandard("SSTL15")),
+        Subsignal("we_n",  Pins("L2"), IOStandard("SSTL15")),
+        Subsignal("cs_n",  Pins("P5"), IOStandard("SSTL15")),
+        Subsignal("dm", Pins("G1 K5"), IOStandard("SSTL15")),
+        Subsignal("dq", Pins(
+            "G5 F5 F4 F3 E2 C1 E1 B3",
+            "M3 K4 N2 L1 P4 H3 R1 M2"),
             IOStandard("SSTL15"),
-            Misc("DRIVE=12"),
-            ),
-        Subsignal("dqs_p",   Pins("J4 H7 B5 C1"), IOStandard("SSTL15D"), Misc("DRIVE=8")),
-        Subsignal("dqs_n",   Pins("H4 G7 A5 B1"), IOStandard("SSTL15D"), Misc("DRIVE=8")),
-        Subsignal("clk_p",   Pins("M2"),          IOStandard("SSTL15D"), Misc("DRIVE=8")),
-        Subsignal("clk_n",   Pins("L2"),          IOStandard("SSTL15D"), Misc("DRIVE=8")),
-        Subsignal("cke",     Pins("L3"),          IOStandard("SSTL15"),  Misc("DRIVE=4")),
-        Subsignal("odt",     Pins("J1"),          IOStandard("SSTL15"),  Misc("DRIVE=12")),
-        Subsignal("reset_n", Pins("N8"),          IOStandard("SSTL15"),  Misc("DRIVE=12")),
-        Misc("PULL_MODE=NONE BANK_VCCIO=1.5"),
+            Misc("VREF=INTERNAL")),
+        Subsignal("dqs_p", Pins("G2 J5"), IOStandard("SSTL15D")),
+        Subsignal("dqs_n", Pins("G3 K6"), IOStandard("SSTL15D")),
+        Subsignal("clk_p", Pins("J1"), IOStandard("SSTL15D")),
+        Subsignal("clk_n", Pins("J3"), IOStandard("SSTL15D")),
+        Subsignal("cke",   Pins("J2"), IOStandard("SSTL15")),
+        Subsignal("odt",   Pins("R3"), IOStandard("SSTL15")),
+        Subsignal("reset_n", Pins("B9"), IOStandard("SSTL15")),
     ),
 ]
 
-# Connectors ---------------------------------------------------------------------------------------
+# Dock 204 Pins SODIMM Connector -------------------------------------------------------------------
 
 _connectors = [
-    ["J1",
-        # -------------------------------------------------------------
-        "---", # 0
-        #  GND  GND                                           (   1-10).
-        " ---- ---- AC26 AC24 AB26 AB24 AB25 AA23 AA24 AA22",
-        #                                          GND  GND   (  11-20).
-        " AA25  Y23  Y25  Y22  Y26  W24  W25  V24 ---- ----",
-        #                                                     (  21-30).
-        "  W26  W23  V26  V23  U26  U24  U25  L24  R26  Y20",
-        #                                                     (  31-40).
-        "  P26  W20  P19  W19  N19  V19  M20  V22  L20  U22",
-        #   5V   5V   5V   5V   5V   5V   5V   5V   5V   5V   (  41-50).
-        " ---- ---- ---- ---- ---- ---- ---- ---- ---- ----",
-        #   5V   5V   5V   5V   5V   5V  3V3   5V  3V3   5V   (  51-60).
-        " ---- ---- ---- ---- ---- ---- ---- ---- ---- ----",
-        #  GND  GND                      GND                  (  61-70).
-        " ---- ----  R15  N16  L20  E17 ----  E18  M21  N17",
-        #            GND                           GND  GND   (  71-80).
-        "  M22  M24 ----  M25  N23  N22  N24  N21 ---- ----",
-        #                                                     (  81-90).
-        "  N26  L22  M26  L23  C19  K22  D19  K23  K25  K21",
-        #                                                     ( 91-100).
-        "  K26  J21  J25  N18  J26  M19  H26  L19  G26  K18",
-        #  GND  GND                                           (101-110).
-        " ---- ----  M15  J24  L15  H24  K20  J23  J20  H23",
-        #                                          GND  GND   (111-120).
-        "  E26  D23  D26  D24  C26  C22  B26  C23 ---- ----",
-    ],
-    ["J2",
-        # -------------------------------------------------------------
+    ["CARD1",
+        # A.
+        # -------------------------------------------------
         "---", # 0
-        #  GND  GND VCCO VCCO VCCO VCCO  GND  GND             (   1-10).
-        " ---- ---- ---- ---- ---- ---- ---- ----  V21  P25",
-        #            GND                                      (  11-20).
-        "  U21  R25 ----  T25  U20  T24  T20  T23  U19  R23",
-        #                                     GND             (  21-30).
-        "  T19  P24  W18  P23  V18  P21  R18 ----  T18  Y21",
-        #                 GND                                 (  31-40).
-        "  T17  W21  U17 ----  U14  V17  V14  V16  T15  U16",
-        #                                GND  GND             (  41-50).
-        "  T14  U15   Y9 AB15  AB7   W9 ---- ----  R17  J15",
-        #            GND  GND                      GND  GND   (  51-60).
-        "  R16  J14 ---- ----  R11 AE16  R12   U4 ---- ----",
-        #                      GND  GND                       (  61-70).
-        " AD14 AA11 AC14 AB11 ---- ---- AB13 AC10 AA13 AD10",
-        #  GND  GND                      GND  GND             (  71-80).
-        " ---- ---- AF13  Ac8 AE13  AD8 ---- ---- AF11  AE9",
-        #            GND  GND                      GND  GND   (  81-90).
-        " AE11  AF9 ---- ---- AD12  AE7 AC12  AF7 ---- ----",
-        #                      GND  GND                       ( 91-100).
-        "   W4  AB1   V4  AC1 ---- ----  AA3  AE5   Y3  AF5",
-        #  GND  GND                      GND  GND             (101-110).
-        " ---- ----   W3  AE3   V3  AF3 ---- ----  AA2  AE2",
-        #            GND  GND                      GND  GND   (111-120).
-        "   Y2  AF2 ---- ----   W1  AD1   V1  AE1 ---- ----",
-    ],
-    ["J3",
-        # -------------------------------------------------------------
-        "---", # 0
-        #  GND  GND                           GND             (   1-10).
-        " ---- ----  B25  A24  A25  A23  C24 ---- B24   H22",
-        #                                     GND  GND        (  11-20).
-        "  E25  H21  D25  F20  G24  G19  F24 ---- ----  F19",
-        #                                                     (  21-30).
-        "  E22  F18  H17  M17  F23  M16  E23  J16  B22  K15",
-        #       GND                                           (  31-40).
-        "  A22 ----  E21  F22  D21  G22  E20  G21  D20  G20",
-        #  GND  GND                                           (  41-50).
-        " ---- ----  D18  H19  C18  J19  C17  F25  B17  G25",
-        #       GND                                           (  51-60).
-        "  E16 ----  D16  H18  G17  J18  F17  K17  L17  K16",
-        #            GND                                      (  61-70).
-        "  L18  F15 ----  G15  H14  G16  H15  H16  C21  L14",
-        #                 GND            GND            GND   (  71-80).
-        "  B21  M14  B20 ----  A20  P11 ----  N12  B19 ----",
-        #       TCK  GND  TDI       TDO       TMS  GND  GND   (  81-90).
-        "  A19  H12 ----  H10  A17  J10  A18  H11 ---- ----",
-        #                      GND  GND                       ( 91-100).
-        "  F11  F13  E11  E13 ---- ----  D10  C12  C10  D12",
-        #  GND  GND                      GND  GND             (101-110).
-        " ---- ----   D8  C14   C8  D14 ---- ----   B9  A13",
-        #            GND  GND                      GND  GND   (111-120).
-        "   A9  B13 ---- ----   B7  P11   A7  N12 ---- ----",
+        #     GND GND  5V  5V  5V  5V GND GND  NC   ( 1-10).
+        " T13 --- --- --- --- --- --- --- --- ---",
+        #      NC GND GND      NC  NC  NC GND GND   (11-20).
+        " M11 --- --- --- T10 --- --- --- --- ---",
+        #  NC 3V3  NC 3V3 GND GND                   (21-30).
+        " --- --- --- --- --- ---  T6 R16  P6 P15",
+        # GND GND                 GND GND           (31-40).
+        " --- ---  T7 P16  R8 N15 --- ---  T8  N16",
+        #         GND                 GND GND       (41-50).
+        "  M6 N14 --- L16  T9 L14  P9 --- --- K15",
+        #             GND GND                 GND   (51-60).
+        " P11 K14 T11 --- --- K16 R11 J15 T12 ---",
+        # GND                 GND                   (61-70).
+        " --- H16 R12 H14 P13 --- R13 G16 T14 H15",
+        # GND GND                                   (71-72).
+        " --- ---",
+        # B.
+        # -------------------------------------------------
+        #                                      NC   (73-82).
+        " M15 L13 M14 K11 F13 K12 G12 K13 T15 ---",
+        #                  NC  NC                   (83-92).
+        " J16 H13 J14 J12 --- --- G14 H12 G15 G11",
+        #  NC  NC                  NC  NC      NC  (93-102).
+        " --- --- F14 B10 F16 A13 --- --- E15 ---",
+        #      NC  NC  NC      NC      NC  NC  NC  (103-112).
+        " D15 --- --- --- A15 --- B14 --- --- ---",
+        #      NC      NC  NC  NC      NC      NC  (113-122).
+        " A14 --- B13 --- --- --- C12 --- B12 ---",
+        #      NC      NC GND GND                  (123-132).
+        " A12 --- C11 --- --- --- B11 E16 A11 F15",
+        # GND GND          NC GND GND      NC      (133-142).
+        " --- --- C10 C13 --- --- --- D16 --- E14",
+        #     GND GND                 GND GND      (143-152).
+        "  B8 --- ---  C9  C6  A9  A7 --- --- L12",
+        #         GND GBD                 GND GND  (153-162).
+        "  A6 J11 --- ---  C7  E9  D7  E8 --- ---",
+        #     VCC     VCC GND GND     VCC     GND  (163-172).
+        "  T2 ---  T3 --- --- ---  T4 ---  T5 ---",
+        # GND VCC             GND GND              (173-182).
+        " --- ---  N6 F10  N7 --- --- D11  N9 D10",
+        #     GND GND      NC  NC GND GND          (183-192).
+        "  R9 --- --- E10 --- --- --- ---  N8 R7",
+        #         GND GND  NC      NC      NC  NC  (193-202).
+        "  L9  P7 --- --- ---  M6 ---  L8 --- ---",
+        #  NC  NC                                  (203-204).
+        " --- ---",
     ],
 ]
 
 # Dock IOs -----------------------------------------------------------------------------------------
 
-# Note: SOM.J1 -> dock.J6 odd/even revert
-#       SOM.J2 -> dock.J7 odd/even revert
-#       SOM.J3 -> dock.J8 odd/even revert
-
 _dock_io = [
-    # HDMI In
-    ("hdmi_in", 0,
-        Subsignal("clk_p",   Pins("J1:107")),
-        Subsignal("clk_n",   Pins("J1:109")),
-        Subsignal("data0_p", Pins("J1:87")),
-        Subsignal("data0_n", Pins("J1:85")),
-        Subsignal("data1_p", Pins("J1:103")),
-        Subsignal("data1_n", Pins("J1:105")),
-        Subsignal("data2_p", Pins("J1:93")),
-        Subsignal("data2_n", Pins("J1:95")),
-        Subsignal("hdp",     Pins("J1:99")),
-        #Subsignal("scl",     Pins("J1:89")),
-        #Subsignal("sda",     Pins("J1:91")),
-        #Subsignal("cec",     Pins("J1:97")),
-        IOStandard("LVCMOS33D"),
-        Misc("PULL_MODE=NONE DRIVE=8")
-    ),
-
-    # HDMI Out
-    ("hdmi_out", 0,
-        Subsignal("clk_p",   Pins("J1:14")),
-        Subsignal("clk_n",   Pins("J1:12")),
-        Subsignal("data0_p", Pins("J1:6")),
-        Subsignal("data0_n", Pins("J1:4")),
-        Subsignal("data1_p", Pins("J1:18")),
-        Subsignal("data1_n", Pins("J1:16")),
-        Subsignal("data2_p", Pins("J1:10")),
-        Subsignal("data2_n", Pins("J1:8")),
-        Subsignal("hdp",     Pins("J2:39")),
-        #Subsignal("scl",     Pins("J1:89")),
-        #Subsignal("sda",     Pins("J1:91")),
-        #Subsignal("cec",     Pins("J2:41")),
-        IOStandard("LVCMOS33D"),
-        Misc("PULL_MODE=NONE DRIVE=8")
+    # Leds
+    ("led", 0,  Pins( "CARD1:44"), IOStandard("LVCMOS18")), # CHECKME: Should be LVCMOS33.
+    ("led", 1,  Pins( "CARD1:46"), IOStandard("LVCMOS18")), # CHECKME: Should be LVCMOS33.
+    ("led", 3,  Pins( "CARD1:40"), IOStandard("LVCMOS18")), # CHECKME: Should be LVCMOS33.
+    ("led", 2,  Pins( "CARD1:42"), IOStandard("LVCMOS18")), # CHECKME: Should be LVCMOS33.
+    ("led", 4,  Pins( "CARD1:98"), IOStandard("LVCMOS33")),
+    ("led", 5,  Pins("CARD1:136"), IOStandard("LVCMOS33")),
+
+    # RGB Led.
+    ("rgb_led", 0, Pins("CARD1:45"), IOStandard("LVCMOS18")),
+
+    # Buttons.
+    ("btn_n", 0,  Pins( "CARD1:15"), IOStandard("LVCMOS33")),
+    ("btn_n", 1,  Pins("CARD1:165"), IOStandard("LVCMOS15")),
+    ("btn_n", 2,  Pins("CARD1:163"), IOStandard("LVCMOS15")),
+    ("btn_n", 3,  Pins("CARD1:159"), IOStandard("LVCMOS15")),
+    ("btn_n", 4,  Pins("CARD1:157"), IOStandard("LVCMOS15")),
+
+    # HDMI.
+    ("hdmi", 0,
+        Subsignal("clk_p",   Pins("CARD1:68")),
+        Subsignal("clk_n",   Pins("CARD1:70")),
+        Subsignal("data0_p", Pins("CARD1:64")),
+        Subsignal("data0_n", Pins("CARD1:62")),
+        Subsignal("data1_p", Pins("CARD1:58")),
+        Subsignal("data1_n", Pins("CARD1:56")),
+        Subsignal("data2_p", Pins("CARD1:52")),
+        Subsignal("data2_n", Pins("CARD1:50")),
+        Subsignal("hdp", Pins("CARD1:154"), IOStandard("LVCMOS18")),
+        Subsignal("cec", Pins("CARD1:152"), IOStandard("LVCMOS18")),
+        Subsignal("sda", Pins("CARD1:95"),  IOStandard("LVCMOS18")),
+        Subsignal("scl", Pins("CARD1:97"),  IOStandard("LVCMOS18")),
+        Misc("PULL_MODE=NONE"),
     ),
 
-    ("sdram_clock", 0, Pins("V23"), IOStandard("LVCMOS33")),
-    ("sdram", 0,
-        Subsignal("a",   Pins(
-            "V19   W19 U22 V22 Y25 AA25 AA24 AB25",
-            "AB26 AC26 Y20 U25 U24")),
-        Subsignal("dq",  Pins(
-            "U16 V16 U15 V17 W21 Y21 P21 U17",
-            "P25 W23 T25 R25 R23 T23 P24 P23")),
-        Subsignal("ba",    Pins("V26 W20")),
-        Subsignal("cas_n", Pins("W26")),
-        Subsignal("cs_n",  Pins("U26")),
-        Subsignal("ras_n", Pins("W25")),
-        Subsignal("we_n",  Pins("Y26")),
-        IOStandard("LVCMOS33"),
-        Misc("PULL_MODE=UP")
+    # LCD.
+    ("lcd", 0,
+        # Control.
+        Subsignal("rst",   Pins("CARD1:123")),
+        Subsignal("bl",    Pins("CARD1:186")),
+        Subsignal("sda",   Pins("CARD1: 95")),
+        Subsignal("scl",   Pins("CARD1: 97")),
+        Subsignal("int",   Pins("CARD1:125")),
+
+        # Video.
+        Subsignal("clk",   Pins("CARD1:183")),
+        Subsignal("de",    Pins("CARD1:101")),
+        Subsignal("hsync", Pins("CARD1:107")),
+        Subsignal("vsync", Pins("CARD1:103")),
+        Subsignal("r",     Pins("CARD1:193 CARD1:191 CARD1:181 CARD1:177 CARD1:175")),
+        Subsignal("g",     Pins("CARD1:180 CARD1:131 CARD1:129 CARD1:194 CARD1:192 CARD1:182")),
+        Subsignal("b",     Pins("CARD1:121 CARD1:119 CARD1:115 CARD1:113 CARD1:109")),
+        IOStandard("LVCMOS18")
     ),
 
-    # RGMII Ethernet
+    # RMII Ethernet
     ("eth_clocks", 0,
-        Subsignal("tx", Pins("H24")),
-        Subsignal("rx", Pins("C23")),
-        IOStandard("LVCMOS33")
-    ),
-    ("eth", 0,
-        Subsignal("rst_n",   Pins("E17")),
-        Subsignal("mdio",    Pins("K22")),
-        Subsignal("mdc",     Pins("K23")),
-        Subsignal("rx_ctl",  Pins("C22")),
-        Subsignal("rx_data", Pins("B26 C26 D26 E26")),
-        Subsignal("tx_ctl",  Pins("J24")),
-        Subsignal("tx_data", Pins("K21 J21 L19 K18")),
+        Subsignal("ref_clk", Pins("CARD1:148")),
         IOStandard("LVCMOS33"),
     ),
-    ("ephy_clk", 0, Pins("E18"), IOStandard("LVCMOS33")),
+    ("eth", 0,
+        Subsignal("rst_n",   Pins("CARD1:176")),
+        Subsignal("rx_data", Pins("CARD1:132 CARD1:146")),
+        Subsignal("crs_dv",  Pins("CARD1:198")),
+        Subsignal("tx_en",   Pins("CARD1:130")),
+        Subsignal("tx_data", Pins("CARD1:140 CARD1:142")),
+        Subsignal("mdc",     Pins("CARD1:95")),
+        Subsignal("mdio",    Pins("CARD1:97")),
+        Subsignal("rx_er",   Pins("CARD1:200")),
+        #Subsignal("int_n",   Pins("CARD1:")),
+        IOStandard("LVCMOS33")
+     ),
+]
+
+# Dock Lite IOs ------------------------------------------------------------------------------------
+
+_dock_lite_io = [
+    # Buttons.
+    ("btn_n",   0, Pins("CARD1:15"),  IOStandard("LVCMOS33")),
+    ("btn_n",   1, Pins("CARD1:163"), IOStandard("LVCMOS15")),
+
+    # Switches
+    ("user_sw", 0, Pins("CARD1:159"), IOStandard("LVCMOS15")),
+    ("user_sw", 1, Pins("CARD1:157"), IOStandard("LVCMOS15")),
+]
+
+_dock_lite_connectors = [
+    # Pmod
+    ("j2", "F15 D16 C9  L12 E15 E14 A9  J11"),
+    ("j6", "L8  P7  E10 D11 M6  R7  D10 F10"),
+    ("j7", "T6  T7  T8  T9  P6  R8  M6  P9"),
+    ("j8", "R16 P16 N16 L16 P15 N15 N14 L14"),
+
+    ("j1", {
+         7: "T5",
+         9: "T3",  10: "T5",
+        13: "E9",  14: "E8",
+        15: "T15", 16: "C13",
+        17: "T13", 18: "M11",
+        19: "B10", 20: "A13",
+        21: "H12", 22: "G11",
+        23: "H13", 24: "J12",
+        25: "K12", 26: "K13",
+        27: "L13", 28: "K11",
+        29: "R11", 30: "T12",
+        31: "P11", 32: "T11",
+        33: "G16", 34: "H15",
+        35: "H16", 36: "H14",
+        37: "K16", 38: "J15",
+        39: "K15", 40: "K14",
+    }),
+    ("j3", {
+         3: "N6",   4: "N7",
+         5: "B11",  6: "A12",
+         7: "L9",   8: "N8",
+         9: "R9",  10: "N9",
+        11: "A6",  12: "A7",
+        13: "C6",  14: "B8",
+        15: "C10",
+        17: "A11", 18: "C11",
+        19: "B12", 20: "C12",
+        21: "B13", 22: "A14",
+        23: "B14", 24: "A15",
+        25: "D15", 26: "E15",
+        27: "F16", 28: "F14",
+        29: "G15", 30: "G14",
+        31: "J14", 32: "J16",
+        33: "G12", 34: "F13",
+        35: "M14", 36: "M15",
+        37: "T14", 38: "R13",
+        39: "P13", 40: "R12",
+    })
 ]
 
 # Platform -----------------------------------------------------------------------------------------
 
 class Platform(GowinPlatform):
-    default_clk_name   = "clk50"
-    default_clk_period = 1e9/50e6
+    default_clk_name   = "clk27"
+    default_clk_period = 1e9/27e6
 
     def __init__(self, dock="standard", toolchain="gowin"):
-        GowinPlatform.__init__(self, "GW5AST-LV138FPG676AES", _io, _connectors, toolchain=toolchain, devicename="GW5AST-138B")
-        self.add_extension(_dock_io)
 
-        self.toolchain.options["use_sspi_as_gpio"] = 1
-        self.toolchain.options["use_cpu_as_gpio"]  = 1
-        self.toolchain.options["rw_check_on_ram"]  = 1
-        self.toolchain.options["bit_security"]     = 0
-        self.toolchain.options["bit_encrypt"]      = 0
-        self.toolchain.options["bit_compress"]     = 0
+        GowinPlatform.__init__(self, "GW2A-LV18PG256C8/I7", _io, _connectors, toolchain=toolchain, devicename="GW2A-18C")
+        self.add_extension(_dock_io if dock == "standard" else _dock_lite_io)
+        if dock == "lite":
+            self.add_connector(_dock_lite_connectors)
+
+        self.toolchain.options["use_mspi_as_gpio"]  = 1
+        self.toolchain.options["use_sspi_as_gpio"]  = 1
+        self.toolchain.options["use_ready_as_gpio"] = 1
+        self.toolchain.options["use_done_as_gpio"]  = 1
+        self.toolchain.options["rw_check_on_ram"]   = 1
 
     def create_programmer(self, kit="openfpgaloader"):
         return OpenFPGALoader(cable="ft2232")
 
     def do_finalize(self, fragment):
         GowinPlatform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk50", loose=True), 1e9/50e6)
+        self.add_period_constraint(self.lookup_request("clk27", loose=True), 1e9/27e6)
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/sipeed_tang_nano.py` & `litex-boards-2023.8/litex_boards/platforms/sipeed_tang_nano.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/sipeed_tang_nano_20k.py` & `litex-boards-2023.8/litex_boards/platforms/trenz_tec0117.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,120 @@
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2023 Icenowy Zheng <uwu@icenowy.me>
+# Copyright (c) 2020 Pepijn de Vos <pepijndevos@gmail.com>
+# Copyright (c) 2021 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 
 from litex.build.generic_platform import *
 from litex.build.gowin.platform import GowinPlatform
-from litex.build.gowin.programmer import GowinProgrammer
 from litex.build.openfpgaloader import OpenFPGALoader
 
-
 # IOs ----------------------------------------------------------------------------------------------
 
 _io = [
-    # Clk / Rst.
-    ("clk27",  0, Pins("4"), IOStandard("LVCMOS33")),
+    # Clk / Rst
+    ("clk12",  0, Pins("35"), IOStandard("LVCMOS33")),
+    ("clk100", 0, Pins("63"), IOStandard("LVCMOS33")),
+    ("rst_n",  0, Pins("77"), IOStandard("LVCMOS33")),
+
+    # Leds
+    ("user_led", 0, Pins("86"), IOStandard("LVCMOS33")),
+    ("user_led", 1, Pins("85"), IOStandard("LVCMOS33")),
+    ("user_led", 2, Pins("84"), IOStandard("LVCMOS33")),
+    ("user_led", 3, Pins("83"), IOStandard("LVCMOS33")),
+    ("user_led", 4, Pins("82"), IOStandard("LVCMOS33")),
+    ("user_led", 5, Pins("81"), IOStandard("LVCMOS33")),
+    ("user_led", 6, Pins("80"), IOStandard("LVCMOS33")),
+    ("user_led", 7, Pins("79"), IOStandard("LVCMOS33")),
 
-    # Serial.
+    # Serial
     ("serial", 0,
-        Subsignal("rx", Pins("70")),
-        Subsignal("tx", Pins("69")),
-        IOStandard("LVCMOS33")
+        Subsignal("tx", Pins("15"), IOStandard("LVCMOS33")),
+        Subsignal("rx", Pins("16"), IOStandard("LVCMOS33")),
     ),
 
-    # SPIFlash.
+    # SPIFlash
     ("spiflash", 0,
-        Subsignal("cs_n", Pins("60"), IOStandard("LVCMOS33")),
-        Subsignal("clk",  Pins("59"), IOStandard("LVCMOS33")),
-        Subsignal("miso", Pins("62"), IOStandard("LVCMOS33")),
-        Subsignal("mosi", Pins("61"), IOStandard("LVCMOS33")),
+        Subsignal("cs_n", Pins("51"), IOStandard("LVCMOS33")),
+        Subsignal("clk",  Pins("49"), IOStandard("LVCMOS33")),
+        Subsignal("miso", Pins("53"), IOStandard("LVCMOS33")),
+        Subsignal("mosi", Pins("48"), IOStandard("LVCMOS33")),
+        Subsignal("wp",   Pins("54"), IOStandard("LVCMOS33")),
+        Subsignal("hold", Pins("50"), IOStandard("LVCMOS33")),
     ),
-
-    # SDCard.
-    ("spisdcard", 0,
-        Subsignal("clk",  Pins("83")),
-        Subsignal("mosi", Pins("82")),
-        Subsignal("cs_n", Pins("81")),
-        Subsignal("miso", Pins("84")),
-        IOStandard("LVCMOS33"),
-    ),
-    ("sdcard", 0,
-        Subsignal("data", Pins("84 85 80 81")),
-        Subsignal("cmd",  Pins("82")),
-        Subsignal("clk",  Pins("83")),
-        IOStandard("LVCMOS33"),
+    ("spiflash4x", 0,
+        Subsignal("cs_n", Pins("51")),
+        Subsignal("clk",  Pins("49")),
+        Subsignal("dq",   Pins("48 53 54 50")),
+        IOStandard("LVCMOS33")
     ),
 
-    # Leds
-    ("led_n", 0,  Pins("15"), IOStandard("LVCMOS33")),
-    ("led_n", 1,  Pins("16"), IOStandard("LVCMOS33")),
-    ("led_n", 2,  Pins("17"), IOStandard("LVCMOS33")),
-    ("led_n", 3,  Pins("18"), IOStandard("LVCMOS33")),
-    ("led_n", 4,  Pins("19"), IOStandard("LVCMOS33")),
-    ("led_n", 5,  Pins("20"), IOStandard("LVCMOS33")),
-
-    # RGB Led.
-    ("rgb_led", 0, Pins("79"), IOStandard("LVCMOS33")),
-
-    # Buttons.
-    ("btn", 0,  Pins("88"), IOStandard("LVCMOS33")),
-    ("btn", 1,  Pins("87"), IOStandard("LVCMOS33")),
+    # SPIFlash (FTDI Chip)
+    ("spiflash", 1,
+        Subsignal("cs_n", Pins("13"), IOStandard("LVCMOS33")),
+        Subsignal("clk",  Pins("16"), IOStandard("LVCMOS33")),
+        Subsignal("miso", Pins("14"), IOStandard("LVCMOS33")),
+        Subsignal("mosi", Pins("15"), IOStandard("LVCMOS33")),
+    ),
 
     # SDRAM (embedded in SIP, requires specific IO naming)
     ("O_sdram_clk",   0, Pins(1),  IOStandard("LVCMOS33")),
     ("O_sdram_cke",   0, Pins(1),  IOStandard("LVCMOS33")),
     ("O_sdram_cs_n",  0, Pins(1),  IOStandard("LVCMOS33")),
     ("O_sdram_cas_n", 0, Pins(1),  IOStandard("LVCMOS33")),
     ("O_sdram_ras_n", 0, Pins(1),  IOStandard("LVCMOS33")),
     ("O_sdram_wen_n", 0, Pins(1),  IOStandard("LVCMOS33")),
-    ("O_sdram_dqm",   0, Pins(4),  IOStandard("LVCMOS33")),
-    ("O_sdram_addr",  0, Pins(11), IOStandard("LVCMOS33")),
+    ("O_sdram_dqm",   0, Pins(2),  IOStandard("LVCMOS33")),
+    ("O_sdram_addr",  0, Pins(12), IOStandard("LVCMOS33")),
     ("O_sdram_ba",    0, Pins(2),  IOStandard("LVCMOS33")),
-    ("IO_sdram_dq",   0, Pins(32), IOStandard("LVCMOS33")),
+    ("IO_sdram_dq",   0, Pins(16), IOStandard("LVCMOS33")),
 ]
 
 # Connectors ---------------------------------------------------------------------------------------
 
 _connectors = [
-        # TODO
+    ("pmod", "47 41 38 40 36 42 39 37"),
 ]
 
-# Platform -----------------------------------------------------------------------------------------
+# PMODs --------------------------------------------------------------------------------------------
 
-class Platform(GowinPlatform):
-    default_clk_name   = "clk27"
-    default_clk_period = 1e9/27e6
+def sdcard_pmod_io(pmod):
+    return [
+        # SDCard PMOD:
+        # - https://store.digilentinc.com/pmod-microsd-microsd-card-slot/
+        # - https://github.com/antmicro/arty-expansion-board
+        ("spisdcard", 0,
+            Subsignal("clk",  Pins(f"{pmod}:3")),
+            Subsignal("mosi", Pins(f"{pmod}:1"), Misc("PULL_MODE=UP")),
+            Subsignal("cs_n", Pins(f"{pmod}:0"), Misc("PULL_MODE=UP")),
+            Subsignal("miso", Pins(f"{pmod}:2"), Misc("PULL_MODE=UP")),
+            IOStandard("LVCMOS33"),
+        ),
+        ("sdcard", 0,
+            Subsignal("data", Pins(f"{pmod}:2 {pmod}:4 {pmod}:5 {pmod}:0"), Misc("PULL_MODE=UP")),
+            Subsignal("cmd",  Pins(f"{pmod}:1"), Misc("PULL_MODE=UP")),
+            Subsignal("clk",  Pins(f"{pmod}:3")),
+            Subsignal("cd",   Pins(f"{pmod}:6")),
+            IOStandard("LVCMOS33"),
+        ),
+]
+_sdcard_pmod_io = sdcard_pmod_io("pmod")
 
-    def __init__(self, dock="standard", toolchain="gowin"):
+# Platform -----------------------------------------------------------------------------------------
 
-        GowinPlatform.__init__(self, "GW2AR-LV18QN88C8/I7", _io, _connectors, toolchain=toolchain, devicename="GW2AR-18C")
+class Platform(GowinPlatform):
+    default_clk_name   = "clk12"
+    default_clk_period = 1e9/12e6
 
-        self.toolchain.options["use_mspi_as_gpio"]  = 1
-        self.toolchain.options["use_sspi_as_gpio"]  = 1
-        self.toolchain.options["use_ready_as_gpio"] = 1
-        self.toolchain.options["use_done_as_gpio"]  = 1
-        self.toolchain.options["rw_check_on_ram"]   = 1
+    def __init__(self, toolchain="gowin"):
+        GowinPlatform.__init__(self, "GW1NR-LV9QN88C6/I5", _io, _connectors, toolchain=toolchain, devicename="GW1NR-9")
 
-    def create_programmer(self, kit="openfpgaloader"):
-        return OpenFPGALoader(cable="ft2232")
+    def create_programmer(self):
+        return OpenFPGALoader("littleBee")
 
     def do_finalize(self, fragment):
         GowinPlatform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk27", loose=True), 1e9/27e6)
+        self.add_period_constraint(self.lookup_request("clk12",  loose=True), 1e9/12e6)
+        self.add_period_constraint(self.lookup_request("clk100", loose=True), 1e9/100e6)
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/sipeed_tang_nano_4k.py` & `litex-boards-2023.8/litex_boards/platforms/sipeed_tang_nano_4k.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/sipeed_tang_nano_9k.py` & `litex-boards-2023.8/litex_boards/platforms/sipeed_tang_nano_9k.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/sipeed_tang_primer.py` & `litex-boards-2023.8/litex_boards/platforms/sipeed_tang_primer.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/sipeed_tang_primer_25k.py` & `litex-boards-2023.8/litex_boards/platforms/sqrl_acorn.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,152 +1,157 @@
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2023 Gwenhael Goavec-Merou <gwenhael.goavec-merou@trabucayre.com>
+# Copyright (c) 2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
-from migen import *
+# The Acorn (CLE-101, CLE-215(+)) are cryptocurrency mining accelerator cards from SQRL that can be
+# repurposed as generic FPGA PCIe development boards:
+# - http://www.squirrelsresearch.com/acorn-cle-101
+# - http://www.squirrelsresearch.com/acorn-cle-215-plus
+# The 101 variant is eguivalent to the LiteFury and 215 variant equivalent to the NiteFury from
+# RHSResearchLLC that are documented at: https://github.com/RHSResearchLLC/NiteFury-and-LiteFury.
 
 from litex.build.generic_platform import *
-from litex.build.gowin.platform import GowinPlatform
-from litex.build.openfpgaloader import OpenFPGALoader
-
+from litex.build.xilinx import Xilinx7SeriesPlatform, VivadoProgrammer
+from litex.build.openocd import OpenOCD
 
 # IOs ----------------------------------------------------------------------------------------------
 
 _io = [
     # Clk / Rst.
-    ("clk50",  0, Pins("E2"), IOStandard("LVCMOS33")),
+    ("clk200", 0,
+        Subsignal("p", Pins("J19"), IOStandard("DIFF_SSTL15")),
+        Subsignal("n", Pins("H19"), IOStandard("DIFF_SSTL15"))
+    ),
+
+    # Leds.
+    ("user_led", 0, Pins("G3"), IOStandard("LVCMOS33")),
+    ("user_led", 1, Pins("H3"), IOStandard("LVCMOS33")),
+    ("user_led", 2, Pins("G4"), IOStandard("LVCMOS33")),
+    ("user_led", 3, Pins("H4"), IOStandard("LVCMOS33")),
 
     # SPIFlash.
-    ("spiflash", 0,
-        Subsignal("cs_n", Pins("E6"), IOStandard("LVCMOS33")),
-        Subsignal("clk",  Pins("E7"), IOStandard("LVCMOS33")),
-        Subsignal("mosi", Pins("D6"), IOStandard("LVCMOS33")),
-        Subsignal("miso", Pins("E5"), IOStandard("LVCMOS33")),
-        Subsignal("wp",   Pins("D5"), IOStandard("LVCMOS33")),
-        Subsignal("hold", Pins("E4"), IOStandard("LVCMOS33")),
-    ),
-    ("spiflashx4", 0,
-        Subsignal("cs_n", Pins("E6"),          IOStandard("LVCMOS33")),
-        Subsignal("clk",  Pins("E7"),          IOStandard("LVCMOS33")),
-        Subsignal("dq",   Pins("D6 E5 D5 E4"), IOStandard("LVCMOS33")),
+    ("flash_cs_n", 0, Pins("T19"), IOStandard("LVCMOS33")),
+    ("flash", 0,
+        Subsignal("mosi", Pins("P22")),
+        Subsignal("miso", Pins("R22")),
+        Subsignal("wp",   Pins("P21")),
+        Subsignal("hold", Pins("R21")),
+        IOStandard("LVCMOS33")
     ),
-]
 
-# Dock 204 Pins SODIMM Connector -------------------------------------------------------------------
+    # PCIe.
+    ("pcie_clkreq_n", 0, Pins("G1"), IOStandard("LVCMOS33")),
+    ("pcie_x4", 0,
+        Subsignal("rst_n", Pins("J1"), IOStandard("LVCMOS33"), Misc("PULLUP=TRUE")),
+        Subsignal("clk_p", Pins("F6")),
+        Subsignal("clk_n", Pins("E6")),
+        Subsignal("rx_p",  Pins("B10 B8 D11 D9")),
+        Subsignal("rx_n",  Pins("A10 A8 C11 C9")),
+        Subsignal("tx_p",  Pins("B6 B4 D5 D7")),
+        Subsignal("tx_n",  Pins("A6 A4 C5 C7")),
+    ),
 
-_connectors = [
-    ["J1",
-        # -------------------------------------------------
-        "---", # 0
-        # GND GND                                   ( 1-10).
-        " --- --- L9  H5  K9  J5  J8  L5  K8  K5",
-        #                 GND                       (11-20).
-        "  F7  H8  F6  H7 ---  G7  E8  G8  B3  F5",
-        #             3V3     3V3 GND GND 3V3       (21-30).
-        "  C3  G5  E3 ---  D7 --- --- --- ---  L6",
-        # 3V3                                       (31-40).
-        " ---  K6 J11  K7 J10  J7 H11  L7 H10  L8",
-        #                 GND                 GND   (41-50).
-        " G11 L10 G10 K10 --- K11 D11 L11 D10 ---",
-        #                                 GND GND   (51-60).
-        " C11 E11 C10 E10 B11 A11 B10 A10 --- ---",
-    ],
-    ["J2",
-        # ----------------------------------------------------------------------
-        "---", # 0
-        # GND     3V3         3V3                                       ( 1-10).
-        " ---     ---      B2 ---      C2  L2      F2  L1      F1  K1",
-        #                                                     GND       (11-20).
-        "  A1      K2      D8  J4      E1  K4      D1  G2     ---  G1",
-        # TCK             TMS         TDO         TDI         GND       (21-30).
-        "  C1      L4      B1  L3      A2  J1      A3  J2     ---  G4",
-        #                             GND             1V8         1V8   (31-40).
-        " M0_D3_P  H4 M0_D3_N  H1     ---  H2 M0_D2_P --- M0_D2_N ---",
-        # GND     2V5         2V5         3V3     GND 3V3         3V3   (41-50).
-        " ---     --- M0_CK_P --- M0_CK_N ---     --- --- M0_D1_P ---",
-        #          5V     GND GND          5V          5V     GND  5V   (51-60).
-        " M0_D1_N ---     --- --- M0_D0_P --- M0_D0_N ---     --- ---",
-    ],
+    # DDR3 SDRAM.
+    ("ddram", 0,
+        Subsignal("a", Pins(
+            "M15 L21 M16 L18 K21 M18 M21 N20",
+            "M20 N19 J21 M22 K22 N18 N22 J22"),
+            IOStandard("SSTL15")),
+        Subsignal("ba",    Pins("L19 J20 L20"), IOStandard("SSTL15")),
+        Subsignal("ras_n", Pins("H20"),  IOStandard("SSTL15")),
+        Subsignal("cas_n", Pins("K18"),  IOStandard("SSTL15")),
+        Subsignal("we_n",  Pins("L16"),  IOStandard("SSTL15")),
+        Subsignal("dm", Pins("A19 G22"), IOStandard("SSTL15")),
+        Subsignal("dq", Pins(
+            "D19 B20 E19 A20 F19 C19 F20 C18",
+            "E22 G21 D20 E21 C22 D21 B22 D22"),
+            IOStandard("SSTL15"),
+            Misc("IN_TERM=UNTUNED_SPLIT_50")),
+        Subsignal("dqs_p", Pins("F18 B21"),  IOStandard("DIFF_SSTL15")),
+        Subsignal("dqs_n", Pins("E18 A21"), IOStandard("DIFF_SSTL15")),
+        Subsignal("clk_p", Pins("K17"), IOStandard("DIFF_SSTL15")),
+        Subsignal("clk_n", Pins("J17"), IOStandard("DIFF_SSTL15")),
+        Subsignal("cke",   Pins("H22"), IOStandard("SSTL15")),
+        Subsignal("odt",   Pins("K19"), IOStandard("SSTL15")),
+        Subsignal("reset_n", Pins("K16"), IOStandard("LVCMOS15")),
+        #Subsignal("cs_n", Pins(""), IOStandard("SSTL15")),
+        Misc("SLEW=FAST"),
+    ),
 ]
 
-# Dock IOs -----------------------------------------------------------------------------------------
-
-_dock_io = [
-    # Serial.
+_serial_io = [
+    # Serial adapter on P2.
     ("serial", 0,
-        Subsignal("rx", Pins("J1:19")),
-        Subsignal("tx", Pins("J1:21")),
-        IOStandard("LVCMOS33")
-    ),
-
-    # Leds.
-    ("led", 0, Pins("J1:17"), IOStandard("LVCMOS33")), # Pin READY.
-    ("led", 1, Pins("J1:25"), IOStandard("LVCMOS33")), # Pin DONE.
-
-    # Buttons.
-    ("btn_n", 0, Pins("J1:37"), IOStandard("LVCMOS33")),
-    ("btn_n", 1, Pins("J1:39"), IOStandard("LVCMOS33")),
-
-    # USB.
-    ("usb", 0,
-        Subsignal("d_p", Pins("J1:30")),
-        Subsignal("d_n", Pins("J1:32")),
+        Subsignal("tx", Pins("K2")),
+        Subsignal("rx", Pins("J2")),
+        Misc("SLEW=FAST"),
         IOStandard("LVCMOS33"),
     ),
 ]
 
-_dock_connectors = [
-    # Pmod
-    ("j4", "G11 D11 B11 C11 G10 D10 B10 C10"),
-    ("j5", "A11 E11 K11  L5 A10 E10 L11  K5"),
-    ("j6", " F5  G7  H8  H5  G5  G8  H7  J5"),
-
-    ("j3", {
-         1:  "K2",  2:  "K1",
-         3:  "L1",  4:  "L2",
-         5:  "K4",  6:  "J4",
-         7:  "G1",  8:  "G2",
-         9:  "L3", 10:  "L4",
-        11: "---", 12: "---",
-        13:  "C2", 14:  "B2",
-        15:  "F1", 16:  "F2",
-        17:  "A1", 18:  "E1",
-        19:  "D1", 20:  "E3",
-        21:  "J2", 22:  "J1",
-        23:  "H4", 24:  "G4",
-        25:  "H2", 26:  "H1",
-        27:  "J7", 28:  "K7",
-        29:  "L8", 30:  "L7",
-        31: "K10", 32: "L10",
-        33:  "K9", 34:  "L9",
-        35:  "K8", 36:  "J8",
-        37:  "F6", 38:  "F7",
-        39: "J10", 40: "J11",
-    }),
+_sdcard_io = [
+    # SPI SDCard adapter on P2.
+    # https://spoolqueue.com/new-design/fpga/migen/litex/2020/08/11/acorn-cle-215.html
+    ("spisdcard", 0,
+        Subsignal("clk",  Pins("J2")),
+        Subsignal("mosi", Pins("J5"), Misc("PULLUP True")),
+        Subsignal("cs_n", Pins("H5"), Misc("PULLUP True")),
+        Subsignal("miso", Pins("K2"), Misc("PULLUP True")),
+        Misc("SLEW=FAST"),
+        IOStandard("LVCMOS33"),
+    ),
 ]
 
 # Platform -----------------------------------------------------------------------------------------
 
-class Platform(GowinPlatform):
-    default_clk_name   = "clk50"
-    default_clk_period = 1e9/50e6
-
-    def __init__(self, toolchain="gowin"):
-
-        GowinPlatform.__init__(self, "GW5A-LV25MG121NC1/I0", _io, _connectors, toolchain=toolchain, devicename="GW5A-25A")
-        self.add_extension(_dock_io)
-        self.add_connector(_dock_connectors)
-
-        self.toolchain.options["use_mspi_as_gpio"]  = 1 # spi flash
-        self.toolchain.options["use_ready_as_gpio"] = 1 # led
-        self.toolchain.options["use_done_as_gpio"]  = 1 # led
-        self.toolchain.options["use_cpu_as_gpio"]   = 1 # clk
-        self.toolchain.options["rw_check_on_ram"]   = 1
-
-    def create_programmer(self, kit="openfpgaloader"):
-        return OpenFPGALoader(cable="ft2232")
+class Platform(Xilinx7SeriesPlatform):
+    default_clk_name   = "clk200"
+    default_clk_period = 1e9/200e6
+
+    def __init__(self, variant="cle-215+", toolchain="vivado"):
+        device = {
+            "cle-101":  "xc7a100t-fgg484-2",
+            "cle-215":  "xc7a200t-fbg484-2",
+            "cle-215+": "xc7a200t-fbg484-3"
+        }[variant]
+
+        Xilinx7SeriesPlatform.__init__(self, device, _io, toolchain=toolchain)
+        self.add_extension(_serial_io)
+        self.add_extension(_sdcard_io)
+        self.add_platform_command("set_property INTERNAL_VREF 0.750 [get_iobanks 34]")
+
+        self.toolchain.bitstream_commands = [
+            "set_property BITSTREAM.CONFIG.SPI_BUSWIDTH 4 [current_design]",
+            "set_property BITSTREAM.CONFIG.CONFIGRATE 16 [current_design]",
+            "set_property BITSTREAM.GENERAL.COMPRESS TRUE [current_design]",
+            "set_property CFGBVS VCCO [current_design]",
+            "set_property CONFIG_VOLTAGE 3.3 [current_design]",
+        ]
+
+        self.toolchain.additional_commands = [
+            # Non-Multiboot SPI-Flash bitstream generation.
+            "write_cfgmem -force -format bin -interface spix4 -size 16 -loadbit \"up 0x0 {build_name}.bit\" -file {build_name}.bin",
+
+            # Multiboot SPI-Flash Operational bitstream generation.
+            "set_property BITSTREAM.CONFIG.TIMER_CFG 0x0001fbd0 [current_design]",
+            "set_property BITSTREAM.CONFIG.CONFIGFALLBACK Enable [current_design]",
+            "write_bitstream -force {build_name}_operational.bit ",
+            "write_cfgmem -force -format bin -interface spix4 -size 16 -loadbit \"up 0x0 {build_name}_operational.bit\" -file {build_name}_operational.bin",
+
+            # Multiboot SPI-Flash Fallback bitstream generation.
+            "set_property BITSTREAM.CONFIG.NEXT_CONFIG_ADDR 0x00400000 [current_design]",
+            "write_bitstream -force {build_name}_fallback.bit ",
+            "write_cfgmem -force -format bin -interface spix4 -size 16 -loadbit \"up 0x0 {build_name}_fallback.bit\" -file {build_name}_fallback.bin"
+        ]
+
+    def create_programmer(self, name='openocd'):
+        if name == 'openocd':
+            return OpenOCD("openocd_xc7_ft232.cfg", "bscan_spi_xc7a200t.bit")
+        elif name == 'vivado':
+            # TODO: some board versions may have s25fl128s
+            return VivadoProgrammer(flash_part='s25fl256sxxxxxx0-spi-x1_x2_x4')
 
     def do_finalize(self, fragment):
-        GowinPlatform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk50", loose=True), 1e9/50e6)
+        Xilinx7SeriesPlatform.do_finalize(self, fragment)
+        self.add_period_constraint(self.lookup_request("clk200", loose=True), 1e9/200e6)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/sitlinv_a_e115fb.py` & `litex-boards-2023.8/litex_boards/platforms/sitlinv_a_e115fb.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/sitlinv_stlv7325_v1.py` & `litex-boards-2023.8/litex_boards/platforms/sitlinv_stlv7325_v1.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/sitlinv_stlv7325_v2.py` & `litex-boards-2023.8/litex_boards/platforms/sitlinv_stlv7325_v2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/sitlinv_xc7k420t.py` & `litex-boards-2023.8/litex_boards/platforms/sitlinv_xc7k420t.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/sqrl_fk33.py` & `litex-boards-2023.8/litex_boards/platforms/sqrl_fk33.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/sqrl_xcu1525.py` & `litex-boards-2023.8/litex_boards/platforms/sqrl_xcu1525.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/terasic_de0nano.py` & `litex-boards-2023.8/litex_boards/platforms/terasic_de0nano.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/terasic_de10lite.py` & `litex-boards-2023.8/litex_boards/platforms/terasic_de10lite.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/terasic_de10nano.py` & `litex-boards-2023.8/litex_boards/platforms/terasic_de10nano.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/terasic_de1soc.py` & `litex-boards-2023.8/litex_boards/platforms/terasic_de1soc.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/terasic_de2_115.py` & `litex-boards-2023.8/litex_boards/platforms/trenz_c10lprefkit.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,132 +1,138 @@
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2019 Antony Pavlov <antonynpavlov@gmail.com>
+# Copyright (c) 2019 Antti Lukats <antti.lukats@gmail.com>
+# Copyright (c) 2019 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from litex.build.generic_platform import *
 from litex.build.altera import AlteraPlatform
 from litex.build.altera.programmer import USBBlaster
 
 # IOs ----------------------------------------------------------------------------------------------
 
 _io = [
-    # Clk
-    ("clk50", 0, Pins("Y2"), IOStandard("3.3-V LVTTL")),
-    ("clk25", 0, Pins("A14"), IOStandard("3.3-V LVTTL")),
-
-    # Red LEDs
-    ("user_led", 0,  Pins("G19"), IOStandard("2.5 V")),
-    ("user_led", 1,  Pins("F19"), IOStandard("2.5 V")),
-    ("user_led", 2,  Pins("E19"), IOStandard("2.5 V")),
-    ("user_led", 3,  Pins("F21"), IOStandard("2.5 V")),
-    ("user_led", 4,  Pins("F18"), IOStandard("2.5 V")),
-    ("user_led", 5,  Pins("E18"), IOStandard("2.5 V")),
-    ("user_led", 6,  Pins("J19"), IOStandard("2.5 V")),
-    ("user_led", 7,  Pins("H19"), IOStandard("2.5 V")),
-    ("user_led", 8,  Pins("J17"), IOStandard("2.5 V")),
-    ("user_led", 9,  Pins("G17"), IOStandard("2.5 V")),
-    ("user_led", 10, Pins("J15"), IOStandard("2.5 V")),
-    ("user_led", 11, Pins("H16"), IOStandard("2.5 V")),
-    ("user_led", 12, Pins("J16"), IOStandard("2.5 V")),
-    ("user_led", 13, Pins("H17"), IOStandard("2.5 V")),
-    ("user_led", 14, Pins("F15"), IOStandard("2.5 V")),
-    ("user_led", 15, Pins("G15"), IOStandard("2.5 V")),
-    ("user_led", 16, Pins("G16"), IOStandard("2.5 V")),
-    ("user_led", 17, Pins("H15"), IOStandard("2.5 V")),
+    # Clk / Rst
+    ("clk12", 0, Pins("G21"),  IOStandard("3.3-V LVTTL")),
+    ("clk25", 0, Pins("AA12"), IOStandard("3.3-V LVTTL")),
+    ("cpu_reset", 0, Pins("V15"), IOStandard("3.3-V LVTTL")),
+
+    # Leds
+    ("user_led", 0, Pins("C18"), IOStandard("3.3-V LVTTL")),
+    ("user_led", 1, Pins("D19"), IOStandard("3.3-V LVTTL")),
+    ("user_led", 2, Pins("C19"), IOStandard("3.3-V LVTTL")),
+    ("user_led", 3, Pins("C17"), IOStandard("3.3-V LVTTL")),
+    ("user_led", 4, Pins("D18"), IOStandard("3.3-V LVTTL")),
+
+    # Switches
+    ("sw", 0, Pins("U10"), IOStandard("3.3-V LVTTL")),
+    ("sw", 1, Pins("U11"), IOStandard("3.3-V LVTTL")),
+    ("sw", 2, Pins("V11"), IOStandard("3.3-V LVTTL")),
+    ("sw", 3, Pins("T10"), IOStandard("3.3-V LVTTL")),
+    ("sw", 4, Pins("T11"), IOStandard("3.3-V LVTTL")),
 
     # Serial
     ("serial", 0,
-        Subsignal("tx", Pins("G9"), IOStandard("3.3-V LVTTL")), # Use built-in Tx RS32 port
-        Subsignal("rx", Pins("G12"), IOStandard("3.3-V LVTTL"))  #  Use built-in Rx RS32 port
+        Subsignal("tx", Pins("B21"), IOStandard("3.3-V LVTTL")),
+        Subsignal("rx", Pins("C20"), IOStandard("3.3-V LVTTL")),
     ),
 
     # SDR SDRAM
-    ("sdram_clock", 0, Pins("AE5"), IOStandard("3.3-V LVTTL")),
+    ("sdram_clock", 0, Pins("AA3"), IOStandard("3.3-V LVTTL")),
     ("sdram", 0,
-        Subsignal("a",     Pins(
-            "R6 V8 U8 P1 V5 W8 W7 AA7",
-            "Y5 Y6 R5 AA5 Y7")),
-        Subsignal("ba",    Pins("U7 R4")),
-        Subsignal("cs_n",  Pins("T4")),
-        Subsignal("cke",   Pins("AA6")),
-        Subsignal("ras_n", Pins("U6")),
-        Subsignal("cas_n", Pins("V7")),
-        Subsignal("we_n",  Pins("V6")),
+        Subsignal("a", Pins(
+            "V5   Y3 W6  Y4 AB5 AB6 AA6 AA7",
+            "AB7 AA5 V6 AA8 AB8")),
+        Subsignal("ba",    Pins("Y6 V7")),
+        Subsignal("cs_n",  Pins("W7")),
+        Subsignal("cke",   Pins("AA4")),
+        Subsignal("ras_n", Pins("V8")),
+        Subsignal("cas_n", Pins("Y7")),
+        Subsignal("we_n",  Pins("W8")),
         Subsignal("dq", Pins(
-            "W3 W2  V4  W1  V3  V2  V1  U3",
-            "Y3 Y4 AB1 AA3 AB2 AC1 AB3 AC2")),
-        Subsignal("dm", Pins("U2 W4")),
+            "AB16 Y17 AA16 AA19 AB18 AA20 AB19 AB20",
+            "Y13  Y15 AA13 AB15 AB13 AA15 AA14 AB14")),
+        Subsignal("dm", Pins("Y14 W13")),
         IOStandard("3.3-V LVTTL")
     ),
 
-    # SD Card
-    ("sdcard", 0,
-        Subsignal("data", Pins("AE14 AF13 AB14 AC14")),
-        Subsignal("cmd",  Pins("AD14")),
-        Subsignal("clk",  Pins("AE13")),
-        Misc("FAST_OUTPUT_REGISTER ON"),
-        IOStandard("3.3-V LVTTL"),
+    # ECPS
+    ("epcs", 0,
+        Subsignal("data0", Pins("K1")),
+        Subsignal("dclk",  Pins("K2")),
+        Subsignal("ncs0",  Pins("E2")),
+        Subsignal("asd0",  Pins("D1")),
+        IOStandard("3.3-V LVTTL")
     ),
 
-    # MII Ethernet (88E1111)
+    # HyperRAM
+    ("hyperram", 0,
+        Subsignal("clk",   Pins("T16")),
+        Subsignal("rst_n", Pins("U12")),
+        Subsignal("dq",    Pins("T15 W17 U14 R15 R14 V16 U16 U17")),
+        Subsignal("cs_n",  Pins("V13")),
+        Subsignal("rwds",  Pins("U13")),
+        IOStandard("3.3-V LVTTL")
+    ),
+
+    # GPIO Leds
+    ("gpio_leds", 0,
+        Pins("AB10 AA10 AA9 Y10 W10 U9 U8 U7"),
+        IOStandard("3.3-V LVTTL")
+    ),
+
+    # MII Ethernet
     ("eth_clocks", 0,
-        Subsignal("tx", Pins("B17")),
-        Subsignal("rx", Pins("A15")),
-        IOStandard("2.5 V")
+        Subsignal("tx", Pins("U21")),
+        Subsignal("rx", Pins("V22")),
+        IOStandard("3.3-V LVTTL"),
     ),
     ("eth", 0,
-        Subsignal("rst_n",   Pins("C19")),
-        Subsignal("int_n",   Pins("A21")),
-        Subsignal("mdio",    Pins("B21")),
-        Subsignal("mdc",     Pins("C20")),
-        Subsignal("rx_dv",   Pins("C17")),
-        Subsignal("rx_er",   Pins("D18")),
-        Subsignal("rx_data", Pins("C16 D16 D17 C15")),
-        Subsignal("tx_en",   Pins("A18")),
-        Subsignal("tx_er",   Pins("B18")),
-        Subsignal("tx_data", Pins("C18 D19 A19 B19")),
-        Subsignal("col",     Pins("E15")),
-        Subsignal("crs",     Pins("D15")),
-        IOStandard("2.5 V")
+        Subsignal("rst_n",   Pins("R19")),
+        Subsignal("mdio",    Pins("AA21")),
+        Subsignal("mdc",     Pins("AA22")),
+        Subsignal("rx_dv",   Pins("W21")),
+        Subsignal("rx_er",   Pins("V21")),
+        Subsignal("rx_data", Pins("W22 W20 Y21 Y22")),
+        Subsignal("tx_en",   Pins("T18")),
+        Subsignal("tx_data", Pins("T17 U20 U19 T20")),
+        Subsignal("col",     Pins("T19")),
+        Subsignal("crs",     Pins("R20")),
+        IOStandard("3.3-V LVTTL"),
     ),
-
-    # MII Ethernet (88E1111)
     ("eth_clocks", 1,
-        Subsignal("tx", Pins("C22")),
-        Subsignal("rx", Pins("B15")),
-        IOStandard("2.5 V")
+        Subsignal("tx", Pins("N16")),
+        Subsignal("rx", Pins("V22")),
+        IOStandard("3.3-V LVTTL"),
     ),
     ("eth", 1,
-        Subsignal("rst_n",   Pins("D22")),
-        Subsignal("int_n",   Pins("D24")),
-        Subsignal("mdio",    Pins("D25")),
-        Subsignal("mdc",     Pins("D23")),
-        Subsignal("rx_dv",   Pins("A22")),
-        Subsignal("rx_er",   Pins("C24")),
-        Subsignal("rx_data", Pins("B23 C21 A23 D21")),
-        Subsignal("tx_en",   Pins("B25")),
-        Subsignal("tx_er",   Pins("A25")),
-        Subsignal("tx_data", Pins("C25 A26 B26 C26")),
-        Subsignal("col",     Pins("B22")),
-        Subsignal("crs",     Pins("D20")),
-        IOStandard("2.5 V")
+        Subsignal("rst_n",   Pins("M21")),
+        Subsignal("mdio",    Pins("N20")),
+        Subsignal("mdc",     Pins("N18")),
+        Subsignal("rx_dv",   Pins("R18")),
+        Subsignal("rx_er",   Pins("P17")),
+        Subsignal("rx_data", Pins("M20 M19 M16 N19")),
+        Subsignal("tx_en",   Pins("R22")),
+        Subsignal("tx_data", Pins("R21 N21 M22 N22")),
+        Subsignal("col",     Pins("P21")),
+        Subsignal("crs",     Pins("P22")),
+        IOStandard("3.3-V LVTTL"),
     ),
 ]
 
 # Platform -----------------------------------------------------------------------------------------
 
 class Platform(AlteraPlatform):
-    default_clk_name   = "clk50"
-    default_clk_period = 1e9/50e6
+    default_clk_name   = "clk12"
+    default_clk_period = 1e9/12e6
 
     def __init__(self, toolchain="quartus"):
-        AlteraPlatform.__init__(self, "EP4CE115F29C7", _io, toolchain=toolchain)
+        AlteraPlatform.__init__(self, "10CL055YU484A7G", _io, toolchain=toolchain)
 
     def create_programmer(self):
-        return USBBlaster()
+        return USBBlaster(cable_name="Arrow-USB-Blaster")
 
     def do_finalize(self, fragment):
         AlteraPlatform.do_finalize(self, fragment)
-        self.add_period_constraint(self.lookup_request("clk50", loose=True), 1e9/50e6)
+        self.add_period_constraint(self.lookup_request("clk12", loose=True), 1e9/12e6)
         self.add_period_constraint(self.lookup_request("clk25", loose=True), 1e9/25e6)
```

### Comparing `litex-boards-2023.12/litex_boards/platforms/terasic_deca.py` & `litex-boards-2023.8/litex_boards/platforms/terasic_deca.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/terasic_sockit.py` & `litex-boards-2023.8/litex_boards/platforms/terasic_sockit.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/tinyfpga_bx.py` & `litex-boards-2023.8/litex_boards/platforms/tinyfpga_bx.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/trenz_cyc1000.py` & `litex-boards-2023.8/litex_boards/platforms/trenz_cyc1000.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/trenz_max1000.py` & `litex-boards-2023.8/litex_boards/platforms/trenz_max1000.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/trenz_te0725.py` & `litex-boards-2023.8/litex_boards/platforms/trenz_te0725.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/tul_pynq_z2.py` & `litex-boards-2023.8/litex_boards/platforms/tul_pynq_z2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/xilinx_ac701.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_ac701.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/xilinx_alveo_u200.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_alveo_u200.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/xilinx_alveo_u250.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_alveo_u250.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/xilinx_alveo_u280.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_alveo_u280.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/xilinx_kc705.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_kc705.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/xilinx_kcu105.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_kcu105.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/xilinx_kv260.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_kv260.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/xilinx_sp605.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_sp605.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/xilinx_vc707.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_vc707.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/xilinx_vcu118.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_vcu118.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/xilinx_vcu128.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_vcu128.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/xilinx_zcu104.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_zcu104.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/xilinx_zcu216.py` & `litex-boards-2023.8/litex_boards/platforms/xilinx_zcu216.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/platforms/ztex213.py` & `litex-boards-2023.8/litex_boards/platforms/ztex213.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/adi_adrv2crr_fmc.py` & `litex-boards-2023.8/litex_boards/targets/adi_adrv2crr_fmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,14 @@
         **kwargs):
         platform = adi_adrv2crr_fmc.Platform()
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = CRG(platform, sys_clk_freq, ddram_channel)
 
         # SoCCore ----------------------------------------------------------------------------------
-        kwargs["with_jtagbone"] = True
-
         SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on ADI ADRV2CRR-FMC", **kwargs)
 
         # DDR4 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
             self.ddrphy = usddrphy.USPDDRPHY(
                 pads             = platform.request("ddram", ddram_channel),
                 memtype          = "DDR4",
@@ -115,14 +113,17 @@
         )
 
         self.comb += platform.request("fan").pwm_n.eq(~self.fan.pwm)
 
         # SYSMON -----------------------------------------------------------------------------------
         self.sysmon = ZynqUSPSystemMonitor()
 
+        # JTAG -------------------------------------------------------------------------------------
+        self.add_jtagbone()
+
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
     parser = LiteXArgumentParser(platform=adi_adrv2crr_fmc.Platform, description="LiteX SoC on ADI ADRV2CRR-FMC.")
     parser.add_target_argument("--sys-clk-freq", default=150e6, type=float, help="System clock frequency.")
     parser.add_target_argument("--with-pcie",    action="store_true",       help="Enable PCIe support.")
```

### Comparing `litex-boards-2023.12/litex_boards/targets/adi_plutosdr.py` & `litex-boards-2023.8/litex_boards/targets/adi_plutosdr.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,18 +60,20 @@
     def __init__(self, sys_clk_freq=100e6, **kwargs):
         platform = adi_plutosdr.Platform()
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        kwargs["uart_name"]     = "crossover"
-        kwargs["with_jtagbone"] = True
+        kwargs["uart_name"] = "crossover"
         SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Pluto SDR", **kwargs)
 
+        # JTAGBone ---------------------------------------------------------------------------------
+        self.add_jtagbone()
+
         # GPIOS ------------------------------------------------------------------------------------
         self.comb += platform.request("gpio", 0).eq(ClockSignal("sys"))
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
```

### Comparing `litex-boards-2023.12/litex_boards/targets/alchitry_au.py` & `litex-boards-2023.8/litex_boards/targets/alchitry_au.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/alchitry_cu.py` & `litex-boards-2023.8/litex_boards/targets/alchitry_cu.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/alchitry_mojo.py` & `litex-boards-2023.8/litex_boards/targets/alchitry_mojo.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/aliexpress_xc7k420t.py` & `litex-boards-2023.8/litex_boards/targets/aliexpress_xc7k420t.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/aliexpress_xc7k70t.py` & `litex-boards-2023.8/litex_boards/targets/digilent_nexys4ddr.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,159 +1,145 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2021 Nathaniel Lewis <github@nrlewis.dev>
-# Copyright (c) 2023 Hans Baier <hansfbaier@gmail.com>
+# Copyright (c) 2018-2019 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
+
 from migen import *
 
 from litex.gen import *
 
-from litex.build.io import DDROutput
-from litex_boards.platforms import aliexpress_xc7k70t
+from litex_boards.platforms import digilent_nexys4ddr
 
-from litex.soc.interconnect.csr import *
+from litex.soc.cores.clock import *
+from litex.soc.integration.soc import SoCRegion
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
-
-from litex.soc.cores.clock import *
-from litex.soc.cores.video import VideoS7HDMIPHY
+from litex.soc.cores.video import VideoVGAPHY
 from litex.soc.cores.led import LedChaser
 
-from litedram.modules import W9812G6JB, SDRModule
-from litedram.phy import GENSDRPHY, HalfRateGENSDRPHY
+from litedram.modules import MT47H64M16
+from litedram.phy import s7ddrphy
+
+from liteeth.phy.rmii import LiteEthPHYRMII
 
 # CRG ----------------------------------------------------------------------------------------------
 
-class CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq, sdram_rate="1:1"):
-        self.rst       = Signal()
-        self.cd_sys    = ClockDomain()
-        self.cd_hdmi   = ClockDomain()
-        self.cd_hdmi5x = ClockDomain()
-        if sdram_rate == "1:2":
-            self.cd_sys2x    = ClockDomain()
-            self.cd_sys2x_ps = ClockDomain()
-        else:
-            self.cd_sys_ps = ClockDomain()
-
-        # Clk/Rst
-        clk50 = platform.request("clk50")
-
-        # PLL
-        self.pll = pll = S7PLL()
-        self.comb += pll.reset.eq(self.rst)
-        pll.register_clkin(clk50, 50e6)
-        pll.create_clkout(self.cd_sys,    sys_clk_freq)
-        pll.create_clkout(self.cd_hdmi,   25e6,  margin=0)
-        pll.create_clkout(self.cd_hdmi5x, 125e6, margin=0)
-        if sdram_rate == "1:2":
-            pll.create_clkout(self.cd_sys2x,    2*sys_clk_freq)
-            pll.create_clkout(self.cd_sys2x_ps, 2*sys_clk_freq, phase=90)
-        else:
-            pll.create_clkout(self.cd_sys_ps, sys_clk_freq, phase=90)
+class _CRG(LiteXModule):
+    def __init__(self, platform, sys_clk_freq):
+        self.rst          = Signal()
+        self.cd_sys       = ClockDomain()
+        self.cd_sys2x     = ClockDomain()
+        self.cd_sys2x_dqs = ClockDomain()
+        self.cd_idelay    = ClockDomain()
+        self.cd_eth       = ClockDomain()
+        self.cd_vga       = ClockDomain()
+        # # #
+
+        self.pll = pll = S7MMCM(speedgrade=-1)
+        self.comb += pll.reset.eq(~platform.request("cpu_reset") | self.rst)
+        pll.register_clkin(platform.request("clk100"), 100e6)
+        pll.create_clkout(self.cd_sys,       sys_clk_freq)
+        pll.create_clkout(self.cd_sys2x,     2*sys_clk_freq)
+        pll.create_clkout(self.cd_sys2x_dqs, 2*sys_clk_freq, phase=90)
+        pll.create_clkout(self.cd_idelay,    200e6)
+        pll.create_clkout(self.cd_eth,       50e6)
+        pll.create_clkout(self.cd_vga,       40e6)
+        platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
+
+        self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
 
-# BaseSoC -----------------------------------------------------------------------------------------
+# BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=100e6, sdram_rate="1:1",
-        with_hdmi              = False,
+    def __init__(self, sys_clk_freq=75e6,
         with_ethernet          = False,
-        with_pcie              = False,
-        with_sdram             = True,
+        with_etherbone         = False,
         with_led_chaser        = True,
         with_video_terminal    = False,
         with_video_framebuffer = False,
-        with_video_colorbars   = False,
         **kwargs):
-        platform = aliexpress_xc7k70t.Platform()
+        platform = digilent_nexys4ddr.Platform()
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = CRG(platform, sys_clk_freq, sdram_rate)
+        self.crg = _CRG(platform, sys_clk_freq)
 
-        # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Alchitry Mojo", **kwargs)
+        # SoCCore ----------------------------------_-----------------------------------------------
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Nexys4DDR", **kwargs)
 
-        # Add SDRAM if a shield with RAM has been added
+        # DDR2 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
-            sdram_clk = ClockSignal("sys2x_ps" if sdram_rate == "1:2" else "sys_ps")
-            self.crg.specials += DDROutput(1, 0, platform.request("sdram_clock"), sdram_clk)
-
-            sdrphy_cls = HalfRateGENSDRPHY if sdram_rate == "1:2" else GENSDRPHY
-            self.sdrphy = sdrphy_cls(platform.request("sdram"), sys_clk_freq)
+            self.ddrphy = s7ddrphy.A7DDRPHY(platform.request("ddram"),
+                memtype      = "DDR2",
+                nphases      = 2,
+                sys_clk_freq = sys_clk_freq)
             self.add_sdram("sdram",
-                phy           = self.sdrphy,
-                module        = W9812G6JB(sys_clk_freq, sdram_rate),
-                l2_cache_size = kwargs.get("l2_size", 1024)
+                phy           = self.ddrphy,
+                module        = MT47H64M16(sys_clk_freq, "1:2"),
+                l2_cache_size = kwargs.get("l2_size", 8192)
             )
-        
-        # HDMI Options -----------------------------------------------------------------------------
-        if with_hdmi and (with_video_colorbars or with_video_framebuffer or with_video_terminal):
-            self.videophy = VideoS7HDMIPHY(platform.request("hdmi_out"), clock_domain="hdmi")
-            if with_video_colorbars:
-                self.add_video_colorbars(phy=self.videophy, timings="640x480@60Hz", clock_domain="hdmi")
-            if with_video_terminal:
-                self.add_video_terminal(phy=self.videophy, timings="640x480@60Hz", clock_domain="hdmi")
-            if with_video_framebuffer:
-                self.add_video_framebuffer(phy=self.videophy, timings="640x480@60Hz", clock_domain="hdmi")
 
         # Ethernet / Etherbone ---------------------------------------------------------------------
-        if with_ethernet:
-            self.ethphy = LiteEthPHYRGMII(
-                clock_pads = self.platform.request("eth_clocks", 0),
-                pads       = self.platform.request("eth", 0),
-                tx_delay = 1.417e-9,
-                rx_delay = 1.417e-9,
-            )
-            self.add_ethernet(phy=self.ethphy)
-
-        # PCIe -------------------------------------------------------------------------------------
-        if with_pcie:
-            self.pcie_phy = S7PCIEPHY(platform, platform.request("pcie_x4"),
-                data_width = 128,
-                bar0_size  = 0x20000)
-            self.add_pcie(phy=self.pcie_phy, ndmas=1)
+        if with_ethernet or with_etherbone:
+            self.ethphy = LiteEthPHYRMII(
+                clock_pads = self.platform.request("eth_clocks"),
+                pads       = self.platform.request("eth"))
+            if with_ethernet:
+                self.add_ethernet(phy=self.ethphy)
+            if with_etherbone:
+                self.add_etherbone(phy=self.ethphy)
+
+        # Video ------------------------------------------------------------------------------------
+        if with_video_terminal or with_video_framebuffer:
+            self.videophy = VideoVGAPHY(platform.request("vga"), clock_domain="vga")
+            if with_video_terminal:
+                self.add_video_terminal(phy=self.videophy, timings="800x600@60Hz", clock_domain="vga")
+            if with_video_framebuffer:
+                self.add_video_framebuffer(phy=self.videophy, timings="800x600@60Hz", clock_domain="vga")
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=aliexpress_xc7k70t.Platform, description="LiteX SoC on AliExpress XC7K70T PCIe board.")
-    parser.add_target_argument("--sys-clk-freq",    default=90e6, type=float,  help="System clock frequency.")
-    parser.add_target_argument("--sdram-rate",      default="1:1",             help="SDRAM Rate: (1:1 Full Rate or 1:2 Half Rate).")
-    parser.add_argument("--with-ethernet",          action="store_true",       help="Enable ethernet")
-    parser.add_argument("--with-pcie",              action="store_true",       help="Enable PCIe")
-    parser.add_argument("--with-hdmi",              action="store_true",       help="Enable HDMI")
+    parser = LiteXArgumentParser(platform=digilent_nexys4ddr.Platform, description="LiteX SoC on Nexys4DDR.")
+    parser.add_target_argument("--sys-clk-freq", default=75e6, type=float, help="System clock frequency.")
+    ethopts = parser.target_group.add_mutually_exclusive_group()
+    ethopts.add_argument("--with-ethernet",         action="store_true", help="Enable Ethernet support.")
+    ethopts.add_argument("--with-etherbone",        action="store_true", help="Enable Etherbone support.")
+    sdopts = parser.target_group.add_mutually_exclusive_group()
+    sdopts.add_argument("--with-spi-sdcard",        action="store_true", help="Enable SPI-mode SDCard support.")
+    sdopts.add_argument("--with-sdcard",            action="store_true", help="Enable SDCard support.")
     viopts = parser.target_group.add_mutually_exclusive_group()
-    viopts.add_argument("--with-video-terminal",    action="store_true",       help="Enable Video Terminal (HDMI).")
-    viopts.add_argument("--with-video-framebuffer", action="store_true",       help="Enable Video Framebuffer (HDMI).")
-    viopts.add_argument("--with-video-colorbars",   action="store_true",       help="Enable Video Colorbars (HDMI).")
+    viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (VGA).")
+    viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (VGA).")
     args = parser.parse_args()
 
-    # Note: baudrate is fixed because regardless of USB->TTL baud, the AVR <-> FPGA baudrate is
-    #       set to a fixed rate of 500 kilobaud.
     soc = BaseSoC(
         sys_clk_freq           = args.sys_clk_freq,
-        sdram_rate             = args.sdram_rate,
         with_ethernet          = args.with_ethernet,
-        with_pcie              = args.with_pcie,
-        with_hdmi              = args.with_hdmi,
+        with_etherbone         = args.with_etherbone,
         with_video_terminal    = args.with_video_terminal,
         with_video_framebuffer = args.with_video_framebuffer,
-        with_video_colorbars   = args.with_video_colorbars,
         **parser.soc_argdict
     )
-
+    if args.with_spi_sdcard:
+        soc.add_spi_sdcard()
+    if args.with_sdcard:
+        soc.add_sdcard()
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
+    if args.load:
+        prog = soc.platform.create_programmer()
+        prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
+
 if __name__ == "__main__":
     main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/alinx_ax7010.py` & `litex-boards-2023.8/litex_boards/targets/alinx_ax7010.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/alinx_axu2cga.py` & `litex-boards-2023.8/litex_boards/targets/alinx_axu2cga.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/analog_pocket.py` & `litex-boards-2023.8/litex_boards/targets/colorlight_i9plus.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,170 +1,197 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2023 Florent Kermarrec <florent@enjoy-digital.fr>
-# Copyright (c) 2020 Paul Sajna <sajattack@gmail.com>
-# Copyright (c) 2022 Thomas Watson <twatson52@icloud.com>
+# Copyright (c) 2015-2019 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2020 Antmicro <www.antmicro.com>
+# Copyright (c) 2022 Victor Suarez Rovere <suarezvictor@gmail.com>
+# Copyright (c) 2023 Charles-Henri Mousset <ch.mousset@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
-# ./analog_pocket.py --sdram-rate=1:2 --uart-name=jtag_uart --build --load
-# litex_term jtag --jtag-config=openocd_usb_blaster.cfg
+# Connecting to the JTAG port can be done using the 4 headers on the i9+:
+# J2: TDO
+# J3: TDI
+# J4: TMS
+# J5: TCK
+
+# wuxx's extension board's JTAG isn't compatible with the i9+ headers.
+# The extension board's pogopins must be isolated to avoid shorts.
+# However, is provides PMOD-compatible headers and the ethernet IOs are compatible.
+# See https://github.com/wuxx/Colorlight-FPGA-Projects#ext-board for more infos.
+
 
 from migen import *
 
 from litex.gen import *
 
-from litex_boards.platforms import analog_pocket
+from litex.build.io import DDROutput
+
+from litex_boards.platforms import colorlight_i9plus
 
+from litex.soc.cores.clock import *
+from litex.soc.integration.soc import SoCRegion
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
+from litex.soc.cores.led import LedChaser
+from litex.soc.cores.dna  import DNA
 
-from litex.build.io import DDROutput
+from litedram.modules import M12L64322A
+from litedram.phy import GENSDRPHY
 
-from litex.soc.cores.clock import CycloneVPLL
-
-from litedram.modules import AS4C32M16
-from litedram.phy import GENSDRPHY, HalfRateGENSDRPHY
+from liteeth.phy.s7rgmii import LiteEthPHYRGMII
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq, sdram_rate="1:1"):
-        self.rst         = Signal()
-        self.cd_sys      = ClockDomain()
-        self.cd_video    = ClockDomain()
-        self.cd_video_90 = ClockDomain()
-        if sdram_rate == "1:2":
-            self.cd_sys2x    = ClockDomain()
-            self.cd_sys2x_ps = ClockDomain()
-        else:
+    def __init__(self, platform, sys_clk_freq, with_dram=True, with_ethernet=True):
+        self.rst       = Signal()
+        self.cd_sys    = ClockDomain()
+        self.cd_idelay = ClockDomain()
+        if with_dram:
             self.cd_sys_ps = ClockDomain()
 
         # # #
 
-        # Clk / Rst
-        clk74 = platform.request("clk74a")
+        # Clk/Rst.
+        clk25 = platform.request("clk25")
 
-        # PLL
-        self.pll = pll = CycloneVPLL()
+        # PLL.
+        self.pll = pll = S7PLL(speedgrade=-1)
         self.comb += pll.reset.eq(self.rst)
-        pll.register_clkin(clk74, 74.25e6)
-        pll.create_clkout(self.cd_sys,    sys_clk_freq)
-        if sdram_rate == "1:2":
-            pll.create_clkout(self.cd_sys2x,    2*sys_clk_freq)
-            pll.create_clkout(self.cd_sys2x_ps, 2*sys_clk_freq, phase=180)  # Idealy 90° but needs to be increased.
-        else:
-            pll.create_clkout(self.cd_sys_ps, sys_clk_freq, phase=90)
-        pll.create_clkout(self.cd_video,    25e6)
-        pll.create_clkout(self.cd_video_90, 25e6, phase=90)
-
-        # SDRAM clock
-        sdram_clk = ClockSignal("sys2x_ps" if sdram_rate == "1:2" else "sys_ps")
-        self.specials += DDROutput(1, 0, platform.request("sdram_clock"), sdram_clk)
+        pll.register_clkin(clk25, 25e6)
+        pll.create_clkout(self.cd_sys, sys_clk_freq)
+        pll.create_clkout(self.cd_idelay,    200e6)
+        platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
+        if with_dram:
+            pll.create_clkout(self.cd_sys_ps, sys_clk_freq, phase=90) # untested
+            # SDRAM clock
+            sdram_clk = ClockSignal("sys_ps")
+            self.specials += DDROutput(1, 0, platform.request("sdram_clock"), sdram_clk)
+
+        self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
+
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=50e6, sdram_rate="1:1",
-        with_video_terminal    = False,
-        with_video_framebuffer = False,
-        with_video_colorbars   = False,
+    def __init__(self, toolchain="vivado", sys_clk_freq=100e6,
+        with_dna        = False,
+        with_pmod_uart  = False,
+        with_ethernet   = False,
+        with_etherbone  = False,
+        eth_port        = 0,
+        eth_ip          = "192.168.1.50",
+        eth_dynamic_ip  = False,
+        with_led_chaser = True,
+        with_jtagbone   = True,
+        with_spi_flash  = False,
         **kwargs):
-        platform = analog_pocket.Platform()
+        platform = colorlight_i9plus.Platform(toolchain=toolchain)
+
+        # PMOD: uart on P2 (top) -------------------------------------------------------------------
+        if with_pmod_uart or kwargs.get("uart_name", "") == "serial":
+            platform.add_extension(colorlight_i9plus.pmod_uart())
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = _CRG(platform, sys_clk_freq, sdram_rate)
+        with_dram = (kwargs.get("integrated_main_ram_size", 0) == 0)
+        self.crg  = _CRG(platform, sys_clk_freq, with_dram)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Analog Pocket", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Arty A7", **kwargs)
+
+        # DNA --------------------------------------------------------------------------------------
+        if with_dna:
+            self.dna = DNA()
+            self.dna.add_timing_constraints(platform, sys_clk_freq, self.crg.cd_sys.clk)
 
-        # SDR SDRAM --------------------------------------------------------------------------------
+        # SDRAM ------------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
-            sdrphy_cls = HalfRateGENSDRPHY if sdram_rate == "1:2" else GENSDRPHY
-            self.sdrphy = sdrphy_cls(platform.request("sdram"), sys_clk_freq)
+            sdrphy_cls = GENSDRPHY
+            self.sdrphy = sdrphy_cls(platform.request("sdram"))
             self.add_sdram("sdram",
                 phy           = self.sdrphy,
-                module        = AS4C32M16(sys_clk_freq, sdram_rate),
+                module        = M12L64322A(sys_clk_freq, "1:1"),
                 l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
-        # Video ------------------------------------------------------------------------------------
 
-        if with_video_colorbars or with_video_framebuffer or with_video_terminal:
+        # Ethernet / Etherbone ---------------------------------------------------------------------
+        if with_ethernet or with_etherbone:
+            self.ethphy = LiteEthPHYRGMII(
+                clock_pads = self.platform.request("eth_clocks", eth_port),
+                pads       = self.platform.request("eth", eth_port),
+                tx_delay = 0)
+            if with_ethernet:
+                self.add_ethernet(phy=self.ethphy, dynamic_ip=eth_dynamic_ip)
+            if with_etherbone:
+                self.add_etherbone(phy=self.ethphy, ip_address=eth_ip)
+
+        # Jtagbone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
+
+        # SPI Flash --------------------------------------------------------------------------------
+        if with_spi_flash:
+            from litespi.modules import MX25L12833F
+            from litespi.opcodes import SpiNorFlashOpCodes as Codes
+            self.add_spi_flash(mode="4x", module=MX25L12833F(Codes.READ_1_1_4), rate="1:2", with_master=True)
+
+        # Leds -------------------------------------------------------------------------------------
+        if with_led_chaser:
+            self.leds = LedChaser(
+                pads         = platform.request_all("user_led"),
+                sys_clk_freq = sys_clk_freq,
+            )
 
-            from litex.soc.interconnect import stream
-            from litex.soc.cores.video import video_data_layout
-            from litex.build.io import SDROutput, DDROutput
-
-            class VideoDDRPHY(Module):
-                def __init__(self, pads, clock_domain="sys"):
-                    self.sink = sink = stream.Endpoint(video_data_layout)
-
-                    # # #
-
-                    # Always ack Sink, no backpressure.
-                    self.comb += sink.ready.eq(1)
-
-                    # Drive Clk.
-                    self.specials += DDROutput(i1=1, i2=0, o=pads.clk, clk=ClockSignal(clock_domain+"_90"))
-
-                    # Drive Controls.
-                    self.specials += SDROutput(i=sink.de,     o=pads.de,    clk=ClockSignal(clock_domain))
-                    self.specials += SDROutput(i=sink.hsync,  o=pads.hsync, clk=ClockSignal(clock_domain))
-                    self.specials += SDROutput(i=sink.vsync,  o=pads.vsync, clk=ClockSignal(clock_domain))
-                    self.specials += SDROutput(i=Constant(0), o=pads.skip,  clk=ClockSignal(clock_domain))
-
-                    # Drive Datas.
-                    data = Signal(24)
-                    for i in range(8):
-                        self.comb += data[ 0+i].eq(sink.b[i] & sink.de)
-                        self.comb += data[ 8+i].eq(sink.g[i] & sink.de)
-                        self.comb += data[16+i].eq(sink.r[i] & sink.de)
-                    for i in range(12):
-                        self.specials += DDROutput(
-                            i1  = data[12 + i],
-                            i2  = data[ 0 + i],
-                            o   = pads.data[i],
-                            clk = ClockSignal(clock_domain)
-                        )
-
-            self.videophy = VideoDDRPHY(platform.request("video"), clock_domain="video")
-            if with_video_colorbars:
-                self.add_video_colorbars(phy=self.videophy, timings="640x480@60Hz", clock_domain="video")
-            if with_video_terminal:
-                self.add_video_terminal(phy=self.videophy, timings="640x480@60Hz", clock_domain="video")
-            if with_video_framebuffer:
-                self.add_video_framebuffer(phy=self.videophy, timings="640x480@60Hz", clock_domain="video")
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=analog_pocket.Platform, description="LiteX SoC on Analog Pocket.")
-    parser.add_target_argument("--sys-clk-freq", default=50e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--sdram-rate",   default="1:1",            help="SDRAM Rate (1:1 Full Rate or 1:2 Half Rate).")
-    viopts = parser.target_group.add_mutually_exclusive_group()
-    viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal.")
-    viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer.")
-    viopts.add_argument("--with-video-colorbars",   action="store_true", help="Enable Video Colorbars.")
+    parser = LiteXArgumentParser(platform=colorlight_i9plus.Platform, description="LiteX SoC on Arty A7.")
+    parser.add_target_argument("--flash",          action="store_true",       help="Flash bitstream.")
+    parser.add_target_argument("--sys-clk-freq",   default=100e6, type=float, help="System clock frequency.")
+    parser.add_target_argument("--with-dna",       action="store_true",       help="Enable 7-Series DNA.")
+    parser.add_target_argument("--with-pmod-uart", action="store_true",       help="Enable uart on P2 (top) PMOD")
+    ethopts = parser.target_group.add_mutually_exclusive_group()
+    ethopts.add_argument("--with-ethernet",        action="store_true",       help="Enable Ethernet support.")
+    ethopts.add_argument("--with-etherbone",       action="store_true",       help="Enable Etherbone support.")
+    parser.add_target_argument("--eth-port",       default=0, type=int,       help="Ethernet port to use (0/1)")
+    parser.add_target_argument("--eth-ip",         default="192.168.1.50",    help="Ethernet/Etherbone IP address.")
+    parser.add_target_argument("--eth-dynamic-ip", action="store_true",       help="Enable dynamic Ethernet IP addresses setting.")
+    parser.add_target_argument("--with-jtagbone",  action="store_true",       help="Enable JTAGbone support.")
+    parser.add_target_argument("--with-spi-flash", action="store_true",       help="Enable SPI Flash (MMAPed).")
     args = parser.parse_args()
 
+    assert not (args.with_etherbone and args.eth_dynamic_ip)
+
     soc = BaseSoC(
-        sys_clk_freq           = args.sys_clk_freq,
-        sdram_rate             = args.sdram_rate,
-        with_video_terminal    = args.with_video_terminal,
-        with_video_framebuffer = args.with_video_framebuffer,
-        with_video_colorbars   = args.with_video_colorbars,
+        toolchain      = args.toolchain,
+        sys_clk_freq   = args.sys_clk_freq,
+        with_dna       = args.with_dna,
+        with_pmod_uart = args.with_pmod_uart,
+        with_ethernet  = args.with_ethernet,
+        with_etherbone = args.with_etherbone,
+        eth_port       = args.eth_port,
+        eth_ip         = args.eth_ip,
+        eth_dynamic_ip = args.eth_dynamic_ip,
+        with_jtagbone  = args.with_jtagbone,
+        with_spi_flash = args.with_spi_flash,
         **parser.soc_argdict
     )
+
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
     if args.load:
-        prog = soc.platform.create_programmer()
-        prog.load_bitstream(builder.get_bitstream_filename(mode="sram").replace(".sof", ".rbf"))
+        prog = soc.platform.create_programmer(cfg="prog/openocd_xc7_ft2232.cfg")
+        prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
+
+    if args.flash:
+        prog = soc.platform.create_programmer(cfg="prog/openocd_xc7_ft2232.cfg")
+        prog.flash(0, builder.get_bitstream_filename(mode="flash"))
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `litex-boards-2023.12/litex_boards/targets/antmicro_artix_dc_scm.py` & `litex-boards-2023.8/litex_boards/targets/antmicro_artix_dc_scm.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/antmicro_datacenter_ddr4_test_board.py` & `litex-boards-2023.8/litex_boards/targets/antmicro_datacenter_ddr4_test_board.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,16 @@
             with_ethernet          = False,
             with_etherbone         = False,
             eth_ip                 = "192.168.1.50",
             eth_reset_time         = "10e-3",
             eth_dynamic_ip         = False,
             with_hyperram          = False,
             with_sdcard            = False,
+            with_jtagbone          = True,
+            with_uartbone          = False,
             with_spi_flash         = False,
             with_led_chaser        = True,
             with_video_terminal    = False,
             with_video_framebuffer = False,
             **kwargs):
         platform = antmicro_datacenter_ddr4_test_board.Platform()
 
@@ -136,14 +138,18 @@
                 hw_reset_cycles = math.ceil(float(eth_reset_time) * self.sys_clk_freq)
             )
             if with_ethernet:
                 self.add_ethernet(phy=self.ethphy, dynamic_ip=eth_dynamic_ip)
             if with_etherbone:
                 self.add_etherbone(phy=self.ethphy, ip_address=eth_ip)
 
+        # UartBone ---------------------------------------------------------------------------------
+        if with_uartbone:
+            self.add_uartbone(baudrate=1e6)
+
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
         # Video ------------------------------------------------------------------------------------
@@ -195,14 +201,16 @@
     ethopts.add_argument("--with-ethernet",                action="store_true",    help="Add Ethernet.")
     ethopts.add_argument("--with-etherbone",               action="store_true",    help="Add EtherBone.")
     parser.add_target_argument("--eth-ip",                 default="192.168.1.50", help="Ethernet/Etherbone IP address.")
     parser.add_target_argument("--eth-dynamic-ip",         action="store_true",    help="Enable dynamic Ethernet IP addresses setting.")
     parser.add_target_argument("--eth-reset-time",         default="10e-3",        help="Duration of Ethernet PHY reset.")
     parser.add_target_argument("--with-hyperram",          action="store_true",    help="Add HyperRAM.")
     parser.add_target_argument("--with-sdcard",            action="store_true",    help="Add SDCard.")
+    parser.add_target_argument("--with-jtagbone",          action="store_true",    help="Add JTAGBone.")
+    parser.add_target_argument("--with-uartbone",          action="store_true",    help="Add UartBone on 2nd serial.")
     parser.add_target_argument("--with-video-terminal",    action="store_true",    help="Enable Video Terminal (HDMI).")
     parser.add_target_argument("--with-video-framebuffer", action="store_true",    help="Enable Video Framebuffer (HDMI).")
     parser.add_target_argument("--with-spi-flash",         action="store_true",    help="Enable SPI Flash (MMAPed).")
     args = parser.parse_args()
 
     assert not (args.with_etherbone and args.eth_dynamic_ip)
 
@@ -211,14 +219,16 @@
         iodelay_clk_freq       = args.iodelay_clk_freq,
         with_ethernet          = args.with_ethernet,
         with_etherbone         = args.with_etherbone,
         eth_ip                 = args.eth_ip,
         eth_dynamic_ip         = args.eth_dynamic_ip,
         with_hyperram          = args.with_hyperram,
         with_sdcard            = args.with_sdcard,
+        with_jtagbone          = args.with_jtagbone,
+        with_uartbone          = args.with_uartbone,
         with_spi_flash         = args.with_spi_flash,
         with_video_terminal    = args.with_video_terminal,
         with_video_framebuffer = args.with_video_framebuffer,
         **parser.soc_argdict)
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
```

### Comparing `litex-boards-2023.12/litex_boards/targets/antmicro_lpddr4_test_board.py` & `litex-boards-2023.8/litex_boards/targets/antmicro_lpddr4_test_board.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,14 +51,16 @@
     def __init__(self, *, sys_clk_freq=50e6, iodelay_clk_freq=200e6,
             with_ethernet   = False,
             with_etherbone  = False,
             eth_ip          = "192.168.1.50",
             eth_dynamic_ip  = False,
             with_hyperram   = False,
             with_sdcard     = False,
+            with_jtagbone   = True,
+            with_uartbone   = False,
             with_led_chaser = True,
             **kwargs):
         platform = antmicro_lpddr4_test_board.Platform()
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq, iodelay_clk_freq=iodelay_clk_freq)
 
@@ -98,14 +100,22 @@
                 rx_delay   = 0.8e-9,
             )
             if with_ethernet:
                 self.add_ethernet(phy=self.ethphy, dynamic_ip=eth_dynamic_ip)
             if with_etherbone:
                 self.add_etherbone(phy=self.ethphy, ip_address=eth_ip)
 
+        # Jtagbone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
+
+        # UartBone ---------------------------------------------------------------------------------
+        if with_uartbone:
+            self.add_uartbone(baudrate=1e6)
+
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
@@ -119,27 +129,31 @@
     ethopts = parser.target_group.add_mutually_exclusive_group()
     ethopts.add_argument("--with-ethernet",          action="store_true",    help="Add Ethernet.")
     ethopts.add_argument("--with-etherbone",         action="store_true",    help="Add EtherBone.")
     parser.add_target_argument("--eth-ip",           default="192.168.1.50", help="Ethernet/Etherbone IP address.")
     parser.add_target_argument("--eth-dynamic-ip",   action="store_true",    help="Enable dynamic Ethernet IP addresses setting.")
     parser.add_target_argument("--with-hyperram",    action="store_true",    help="Add HyperRAM.")
     parser.add_target_argument("--with-sdcard",      action="store_true",    help="Add SDCard.")
+    parser.add_target_argument("--with-jtagbone",    action="store_true",    help="Add JTAGBone.")
+    parser.add_target_argument("--with-uartbone",    action="store_true",    help="Add UartBone on 2nd serial.")
     args = parser.parse_args()
 
     assert not (args.with_etherbone and args.eth_dynamic_ip)
 
     soc = BaseSoC(
         sys_clk_freq      = args.sys_clk_freq,
         iodelay_clk_freq  = args.iodelay_clk_freq,
         with_ethernet     = args.with_ethernet,
         with_etherbone    = args.with_etherbone,
         eth_ip            = args.eth_ip,
         eth_dynamic_ip    = args.eth_dynamic_ip,
         with_hyperram     = args.with_hyperram,
         with_sdcard       = args.with_sdcard,
+        with_jtagbone     = args.with_jtagbone,
+        with_uartbone     = args.with_uartbone,
         **parser.soc_argdict)
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
     if args.load:
         prog = soc.platform.create_programmer()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/antmicro_sdi_mipi_video_converter.py` & `litex-boards-2023.8/litex_boards/targets/antmicro_sdi_mipi_video_converter.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/arduino_mkrvidor4000.py` & `litex-boards-2023.8/litex_boards/targets/arduino_mkrvidor4000.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,18 @@
     def __init__(self, sys_clk_freq=48e6, **kwargs):
         platform = arduino_mkrvidor4000.Platform()
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        kwargs["with_jtagbone"] = True # TODO: untested
-
         SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on MKR Vidor 4000", **kwargs)
 
+        self.add_jtagbone() # TODO: untested
+
         # SDR SDRAM --------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
             self.sdrphy = GENSDRPHY(platform.request("sdram"), sys_clk_freq)
             self.add_sdram("sdram",
                 phy           = self.sdrphy,
                 module        = AS4C4M16(sys_clk_freq, "1:1"), # Alliance Memory AS4C4M16
                 l2_cache_size = kwargs.get("l2_size", 8192)
```

### Comparing `litex-boards-2023.12/litex_boards/targets/avnet_aesku40.py` & `litex-boards-2023.8/litex_boards/targets/avnet_aesku40.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/berkeleylab_marble.py` & `litex-boards-2023.8/litex_boards/targets/berkeleylab_marble.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/camlink_4k.py` & `litex-boards-2023.8/litex_boards/targets/camlink_4k.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/colorlight_5a_75x.py` & `litex-boards-2023.8/litex_boards/targets/colorlight_5a_75x.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
     def __init__(self, board, revision, sys_clk_freq=60e6, toolchain="trellis",
         with_ethernet    = False,
         with_etherbone   = False,
+        with_uartbone    = False,
         eth_ip           = "192.168.1.50",
         eth_phy          = 0,
         with_led_chaser  = True,
         use_internal_osc = False,
         sdram_rate       = "1:1",
         with_spi_flash   = False,
         **kwargs):
@@ -150,19 +151,14 @@
             use_internal_osc = use_internal_osc,
             with_usb_pll     = with_usb_pll,
             with_rst         = with_rst,
             sdram_rate       = sdram_rate
         )
 
         # SoCCore ----------------------------------------------------------------------------------
-        # Uartbone ---------------------------------------------------------------------------------
-        if kwargs["with_uartbone"]:
-            if board != "i5a-907":
-                raise ValueError("uartbone only supported on i5a-907")
-
         SoCCore.__init__(self, platform, int(sys_clk_freq), ident="LiteX SoC on Colorlight " + board.upper(), **kwargs)
 
         # SDR SDRAM --------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
             sdrphy_cls = HalfRateGENSDRPHY if sdram_rate == "1:2" else GENSDRPHY
             self.sdrphy = sdrphy_cls(platform.request("sdram"), sys_clk_freq)
             if board == "5a-75e" and revision == "6.0":
@@ -192,14 +188,20 @@
         # Disable leds when serial is used.
         if (platform.lookup_request("serial", loose=True) is None and with_led_chaser
             or board == "i5a-907"):
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led_n"),
                 sys_clk_freq = sys_clk_freq)
 
+        # Uartbone ---------------------------------------------------------------------------------
+        if with_uartbone:
+            if board != "i5a-907":
+                raise ValueError("uartbone only supported on i5a-907")
+            self.add_uartbone(uart_name="uartbone")
+
         # SPI Flash --------------------------------------------------------------------------------
         if with_spi_flash:
             if board == "i5a-907":
                 raise ValueError("SPI Flash chip is unknown on i5a-907, feel free to fix")
                 # from litespi.modules import XXXXXX as SpiFlashModule
             elif board == "5a-75b" and revision == "6.0":
                 raise ValueError("SPI Flash chip is unknown on 5A-75B v6.0, feel free to fix")
@@ -223,26 +225,28 @@
     parser = LiteXArgumentParser(platform=colorlight_5a_75b.Platform, description="LiteX SoC on Colorlight 5A-75X.")
     parser.add_target_argument("--board",             default="5a-75b",         help="Board type (5a-75b, 5a-75e or i5a-907).")
     parser.add_target_argument("--revision",          default="7.0",            help="Board revision (6.0, 6.1, 7.0 or 8.0).")
     parser.add_target_argument("--sys-clk-freq",      default=60e6, type=float, help="System clock frequency.")
     ethopts = parser.target_group.add_mutually_exclusive_group()
     ethopts.add_argument("--with-ethernet",           action="store_true",    help="Enable Ethernet support.")
     ethopts.add_argument("--with-etherbone",          action="store_true",    help="Enable Etherbone support.")
+    parser.add_target_argument("--with-uartbone",     action="store_true",    help="Add uartbone on 'FAN OUT' connector.")
     parser.add_target_argument("--eth-ip",            default="192.168.1.50", help="Ethernet/Etherbone IP address.")
     parser.add_target_argument("--eth-phy",           default=0, type=int,    help="Ethernet PHY (0 or 1).")
     parser.add_target_argument("--use-internal-osc",  action="store_true",    help="Use internal oscillator.")
     parser.add_target_argument("--sdram-rate",        default="1:1",          help="SDRAM Rate (1:1 Full Rate or 1:2 Half Rate).")
     parser.add_target_argument("--with-spi-flash",    action="store_true",    help="Add SPI flash support to the SoC")
     args = parser.parse_args()
 
     soc = BaseSoC(board=args.board, revision=args.revision,
         sys_clk_freq     = args.sys_clk_freq,
         toolchain        = args.toolchain,
         with_ethernet    = args.with_ethernet,
         with_etherbone   = args.with_etherbone,
+        with_uartbone    = args.with_uartbone,
         eth_ip           = args.eth_ip,
         eth_phy          = args.eth_phy,
         use_internal_osc = args.use_internal_osc,
         sdram_rate       = args.sdram_rate,
         with_spi_flash   = args.with_spi_flash,
         **parser.soc_argdict
     )
```

### Comparing `litex-boards-2023.12/litex_boards/targets/colorlight_i5.py` & `litex-boards-2023.8/litex_boards/targets/colorlight_i5.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/colorlight_i9plus.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_ac701.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,190 +1,176 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2015-2019 Florent Kermarrec <florent@enjoy-digital.fr>
-# Copyright (c) 2020 Antmicro <www.antmicro.com>
-# Copyright (c) 2022 Victor Suarez Rovere <suarezvictor@gmail.com>
-# Copyright (c) 2023 Charles-Henri Mousset <ch.mousset@gmail.com>
+# Copyright (c) 2019 Vamsi K Vytla <vamsi.vytla@gmail.com>
+# Copyright (c) 2019-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
-# Connecting to the JTAG port can be done using the 4 headers on the i9+:
-# J2: TDO
-# J3: TDI
-# J4: TMS
-# J5: TCK
-
-# wuxx's extension board's JTAG isn't compatible with the i9+ headers.
-# The extension board's pogopins must be isolated to avoid shorts.
-# However, is provides PMOD-compatible headers and the ethernet IOs are compatible.
-# See https://github.com/wuxx/Colorlight-FPGA-Projects#ext-board for more infos.
-
+import os
 
 from migen import *
 
 from litex.gen import *
 
-from litex.build.io import DDROutput
-
-from litex_boards.platforms import colorlight_i9plus
+from litex_boards.platforms import xilinx_ac701
 
 from litex.soc.cores.clock import *
-from litex.soc.integration.soc import SoCRegion
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
 from litex.soc.cores.led import LedChaser
-from litex.soc.cores.dna  import DNA
 
-from litedram.modules import M12L64322A
-from litedram.phy import GENSDRPHY
+from litedram.common import PHYPadsReducer
+from litedram.modules import MT8JTF12864
+from litedram.phy import s7ddrphy
 
+from liteeth.phy.a7_gtp import QPLLSettings, QPLL
+from liteeth.phy.a7_1000basex import A7_1000BASEX
 from liteeth.phy.s7rgmii import LiteEthPHYRGMII
 
+from litepcie.phy.s7pciephy import S7PCIEPHY
+from litepcie.software import generate_litepcie_software
+
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq, with_dram=True, with_ethernet=True):
-        self.rst       = Signal()
-        self.cd_sys    = ClockDomain()
-        self.cd_idelay = ClockDomain()
-        if with_dram:
-            self.cd_sys_ps = ClockDomain()
+    def __init__(self, platform, sys_clk_freq):
+        self.rst          = Signal()
+        self.cd_sys       = ClockDomain()
+        self.cd_sys4x     = ClockDomain()
+        self.cd_sys4x_dqs = ClockDomain()
+        self.cd_idelay    = ClockDomain()
 
         # # #
 
-        # Clk/Rst.
-        clk25 = platform.request("clk25")
-
-        # PLL.
         self.pll = pll = S7PLL(speedgrade=-1)
-        self.comb += pll.reset.eq(self.rst)
-        pll.register_clkin(clk25, 25e6)
-        pll.create_clkout(self.cd_sys, sys_clk_freq)
+        self.comb += pll.reset.eq(platform.request("cpu_reset") | self.rst)
+        pll.register_clkin(platform.request("clk200"), 200e6)
+        pll.create_clkout(self.cd_sys,       sys_clk_freq)
+        pll.create_clkout(self.cd_sys4x,     4*sys_clk_freq)
+        pll.create_clkout(self.cd_sys4x_dqs, 4*sys_clk_freq, phase=90)
         pll.create_clkout(self.cd_idelay,    200e6)
         platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
-        if with_dram:
-            pll.create_clkout(self.cd_sys_ps, sys_clk_freq, phase=90) # untested
-            # SDRAM clock
-            sdram_clk = ClockSignal("sys_ps")
-            self.specials += DDROutput(1, 0, platform.request("sdram_clock"), sdram_clk)
 
         self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
 
-
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, toolchain="vivado", sys_clk_freq=100e6,
-        with_dna        = False,
-        with_pmod_uart  = False,
+    def __init__(self, sys_clk_freq=100e6,
         with_ethernet   = False,
-        with_etherbone  = False,
-        eth_port        = 0,
-        eth_ip          = "192.168.1.50",
-        eth_dynamic_ip  = False,
-        with_led_chaser = True,
+        eth_phy         = "rgmii",
         with_spi_flash  = False,
+        with_led_chaser = True,
+        with_pcie       = False,
         **kwargs):
-        platform = colorlight_i9plus.Platform(toolchain=toolchain)
-
-        # PMOD: uart on P2 (top) -------------------------------------------------------------------
-        if with_pmod_uart or kwargs.get("uart_name", "") == "serial":
-            platform.add_extension(colorlight_i9plus.pmod_uart())
+        platform = xilinx_ac701.Platform()
 
         # CRG --------------------------------------------------------------------------------------
-        with_dram = (kwargs.get("integrated_main_ram_size", 0) == 0)
-        self.crg  = _CRG(platform, sys_clk_freq, with_dram)
+        self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Arty A7", **kwargs)
-
-        # DNA --------------------------------------------------------------------------------------
-        if with_dna:
-            self.dna = DNA()
-            self.dna.add_timing_constraints(platform, sys_clk_freq, self.crg.cd_sys.clk)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on AC701", **kwargs)
 
-        # SDRAM ------------------------------------------------------------------------------------
+        # DDR3 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
-            sdrphy_cls = GENSDRPHY
-            self.sdrphy = sdrphy_cls(platform.request("sdram"))
+            self.ddrphy = s7ddrphy.A7DDRPHY(
+                pads         = PHYPadsReducer(platform.request("ddram"), [0, 1, 2, 3]),
+                memtype      = "DDR3",
+                nphases      = 4,
+                sys_clk_freq = sys_clk_freq)
             self.add_sdram("sdram",
-                phy           = self.sdrphy,
-                module        = M12L64322A(sys_clk_freq, "1:1"),
+                phy           = self.ddrphy,
+                module        = MT8JTF12864(sys_clk_freq, "1:4"),
                 l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
+        # Ethernet ---------------------------------------------------------------------------------
+        if with_ethernet:
+            # RGMII Ethernet PHY -------------------------------------------------------------------
+            if eth_phy == "rgmii":
+                # phy
+                self.ethphy = LiteEthPHYRGMII(
+                    clock_pads = self.platform.request("eth_clocks"),
+                    pads       = self.platform.request("eth"))
+
+            # 1000BaseX Ethernet PHY ---------------------------------------------------------------
+            if eth_phy == "1000basex":
+                # phy
+                self.comb += self.platform.request("sfp_mgt_clk_sel0", 0).eq(0)
+                self.comb += self.platform.request("sfp_mgt_clk_sel1", 0).eq(0)
+                self.comb += self.platform.request("sfp_tx_disable_n", 0).eq(0)
+                qpll_settings = QPLLSettings(
+                    refclksel  = 0b001,
+                    fbdiv      = 4,
+                    fbdiv_45   = 5,
+                    refclk_div = 1)
+                refclk125 = self.platform.request("gtp_refclk")
+                refclk125_se = Signal()
+                self.specials += \
+                    Instance("IBUFDS_GTE2",
+                        i_CEB = 0,
+                        i_I   = refclk125.p,
+                        i_IB  = refclk125.n,
+                        o_O   = refclk125_se)
+                qpll = QPLL(refclk125_se, qpll_settings)
+                self.submodules += qpll
+                self.ethphy = A7_1000BASEX(
+                    qpll_channel = qpll.channels[0],
+                    data_pads    = self.platform.request("sfp", 0),
+                    sys_clk_freq = self.clk_freq)
 
-        # Ethernet / Etherbone ---------------------------------------------------------------------
-        if with_ethernet or with_etherbone:
-            self.ethphy = LiteEthPHYRGMII(
-                clock_pads = self.platform.request("eth_clocks", eth_port),
-                pads       = self.platform.request("eth", eth_port),
-                tx_delay = 0)
-            if with_ethernet:
-                self.add_ethernet(phy=self.ethphy, dynamic_ip=eth_dynamic_ip)
-            if with_etherbone:
-                self.add_etherbone(phy=self.ethphy, ip_address=eth_ip)
+            self.add_ethernet(phy=self.ethphy)
 
         # SPI Flash --------------------------------------------------------------------------------
         if with_spi_flash:
-            from litespi.modules import MX25L12833F
+            from litespi.modules import N25Q256A
             from litespi.opcodes import SpiNorFlashOpCodes as Codes
-            self.add_spi_flash(mode="4x", module=MX25L12833F(Codes.READ_1_1_4), rate="1:2", with_master=True)
+            self.add_spi_flash(mode="4x", module=N25Q256A(Codes.READ_1_1_4), rate="1:1", with_master=True)
+
+        # PCIe -------------------------------------------------------------------------------------
+        if with_pcie:
+            self.pcie_phy = S7PCIEPHY(platform, platform.request("pcie_x4"),
+                data_width = 128,
+                bar0_size  = 0x20000)
+            self.add_pcie(phy=self.pcie_phy, ndmas=1)
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
-                sys_clk_freq = sys_clk_freq,
-            )
-
+                sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
-
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=colorlight_i9plus.Platform, description="LiteX SoC on Arty A7.")
-    parser.add_target_argument("--flash",          action="store_true",       help="Flash bitstream.")
-    parser.add_target_argument("--sys-clk-freq",   default=100e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--with-dna",       action="store_true",       help="Enable 7-Series DNA.")
-    parser.add_target_argument("--with-pmod-uart", action="store_true",       help="Enable uart on P2 (top) PMOD")
-    ethopts = parser.target_group.add_mutually_exclusive_group()
-    ethopts.add_argument("--with-ethernet",        action="store_true",       help="Enable Ethernet support.")
-    ethopts.add_argument("--with-etherbone",       action="store_true",       help="Enable Etherbone support.")
-    parser.add_target_argument("--eth-port",       default=0, type=int,       help="Ethernet port to use (0/1)")
-    parser.add_target_argument("--eth-ip",         default="192.168.1.50",    help="Ethernet/Etherbone IP address.")
-    parser.add_target_argument("--eth-dynamic-ip", action="store_true",       help="Enable dynamic Ethernet IP addresses setting.")
-    parser.add_target_argument("--with-spi-flash", action="store_true",       help="Enable SPI Flash (MMAPed).")
+    parser = LiteXArgumentParser(platform=xilinx_ac701.Platform, description="LiteX SoC on AC701.")
+    parser.add_target_argument("--sys-clk-freq",   default=100e6, type=float,  help="System clock frequency.")
+    parser.add_target_argument("--with-ethernet",  action="store_true",        help="Enable Ethernet support.")
+    parser.add_target_argument("--eth-phy",        default="rgmii",            help="Select Ethernet PHY (rgmii or 1000basex).")
+    parser.add_target_argument("--with-spi-flash", action="store_true",        help="Enable SPI Flash (MMAPed).")
+    parser.add_target_argument("--with-pcie",      action="store_true",        help="Enable PCIe support.")
+    parser.add_target_argument("--driver",         action="store_true",        help="Generate PCIe driver.")
     args = parser.parse_args()
 
-    assert not (args.with_etherbone and args.eth_dynamic_ip)
-
     soc = BaseSoC(
-        toolchain      = args.toolchain,
         sys_clk_freq   = args.sys_clk_freq,
-        with_dna       = args.with_dna,
-        with_pmod_uart = args.with_pmod_uart,
         with_ethernet  = args.with_ethernet,
-        with_etherbone = args.with_etherbone,
-        eth_port       = args.eth_port,
-        eth_ip         = args.eth_ip,
-        eth_dynamic_ip = args.eth_dynamic_ip,
+        eth_phy        = args.eth_phy,
         with_spi_flash = args.with_spi_flash,
+        with_pcie      = args.with_pcie,
         **parser.soc_argdict
     )
-
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
+    if args.driver:
+        generate_litepcie_software(soc, os.path.join(builder.output_dir, "driver"))
+
     if args.load:
-        prog = soc.platform.create_programmer(cfg="prog/openocd_xc7_ft2232.cfg")
+        prog = soc.platform.create_programmer()
         prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
 
-    if args.flash:
-        prog = soc.platform.create_programmer(cfg="prog/openocd_xc7_ft2232.cfg")
-        prog.flash(0, builder.get_bitstream_filename(mode="flash"))
-
 if __name__ == "__main__":
     main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/decklink_intensity_pro_4k.py` & `litex-boards-2023.8/litex_boards/targets/decklink_intensity_pro_4k.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/decklink_mini_4k.py` & `litex-boards-2023.8/litex_boards/targets/decklink_mini_4k.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/decklink_quad_hdmi_recorder.py` & `litex-boards-2023.8/litex_boards/targets/decklink_quad_hdmi_recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,18 +65,20 @@
     def __init__(self, sys_clk_freq=200e6, with_pcie=False, pcie_lanes=4, **kwargs):
         platform = decklink_quad_hdmi_recorder.Platform()
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        kwargs["uart_name"]    = "crossover"
-        kwargs["with_jtabone"] = True
+        kwargs["uart_name"] = "crossover"
         SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Blackmagic Decklink Quad HDMI Recorder", **kwargs)
 
+        # JTAGBone  --------------------------------------------------------------------------------
+        self.add_jtagbone()
+
         # DDR3 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
             self.ddrphy = usddrphy.USDDRPHY(
                 pads             = PHYPadsReducer(platform.request("ddram"), [0, 1, 2, 3]),
                 memtype          = "DDR3",
                 sys_clk_freq     = sys_clk_freq,
                 iodelay_clk_freq = 200e6)
```

### Comparing `litex-boards-2023.12/litex_boards/targets/digilent_arty.py` & `litex-boards-2023.8/litex_boards/targets/digilent_arty.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
         with_xadc       = False,
         with_dna        = False,
         with_ethernet   = False,
         with_etherbone  = False,
         eth_ip          = "192.168.1.50",
         eth_dynamic_ip  = False,
         with_led_chaser = True,
+        with_jtagbone   = True,
         with_spi_flash  = False,
         with_buttons    = False,
         with_pmod_gpio  = False,
         **kwargs):
         platform = digilent_arty.Platform(variant=variant, toolchain=toolchain)
 
         # CRG --------------------------------------------------------------------------------------
@@ -118,14 +119,18 @@
                 clock_pads = self.platform.request("eth_clocks"),
                 pads       = self.platform.request("eth"))
             if with_ethernet:
                 self.add_ethernet(phy=self.ethphy, dynamic_ip=eth_dynamic_ip)
             if with_etherbone:
                 self.add_etherbone(phy=self.ethphy, ip_address=eth_ip)
 
+        # Jtagbone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
+
         # SPI Flash --------------------------------------------------------------------------------
         if with_spi_flash:
             from litespi.modules import S25FL128L
             from litespi.opcodes import SpiNorFlashOpCodes as Codes
             self.add_spi_flash(mode="4x", module=S25FL128L(Codes.READ_1_1_4), rate="1:2", with_master=True)
 
         # Leds -------------------------------------------------------------------------------------
@@ -165,14 +170,15 @@
     ethopts.add_argument("--with-etherbone",       action="store_true",    help="Enable Etherbone support.")
     parser.add_target_argument("--eth-ip",         default="192.168.1.50", help="Ethernet/Etherbone IP address.")
     parser.add_target_argument("--eth-dynamic-ip", action="store_true",    help="Enable dynamic Ethernet IP addresses setting.")
     sdopts = parser.target_group.add_mutually_exclusive_group()
     sdopts.add_argument("--with-spi-sdcard",       action="store_true", help="Enable SPI-mode SDCard support.")
     sdopts.add_argument("--with-sdcard",           action="store_true", help="Enable SDCard support.")
     parser.add_target_argument("--sdcard-adapter",                      help="SDCard PMOD adapter (digilent or numato).")
+    parser.add_target_argument("--with-jtagbone",  action="store_true", help="Enable JTAGbone support.")
     parser.add_target_argument("--with-spi-flash", action="store_true", help="Enable SPI Flash (MMAPed).")
     parser.add_target_argument("--with-pmod-gpio", action="store_true", help="Enable GPIOs through PMOD.") # FIXME: Temporary test.
     args = parser.parse_args()
 
     assert not (args.with_etherbone and args.eth_dynamic_ip)
 
     soc = BaseSoC(
@@ -181,14 +187,15 @@
         sys_clk_freq   = args.sys_clk_freq,
         with_xadc      = args.with_xadc,
         with_dna       = args.with_dna,
         with_ethernet  = args.with_ethernet,
         with_etherbone = args.with_etherbone,
         eth_ip         = args.eth_ip,
         eth_dynamic_ip = args.eth_dynamic_ip,
+        with_jtagbone  = args.with_jtagbone,
         with_spi_flash = args.with_spi_flash,
         with_pmod_gpio = args.with_pmod_gpio,
         **parser.soc_argdict
     )
     if args.sdcard_adapter == "numato":
         soc.platform.add_extension(digilent_arty._numato_sdcard_pmod_io)
     else:
```

### Comparing `litex-boards-2023.12/litex_boards/targets/digilent_arty_s7.py` & `litex-boards-2023.8/litex_boards/targets/digilent_arty_s7.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/digilent_arty_z7.py` & `litex-boards-2023.8/litex_boards/targets/digilent_arty_z7.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/digilent_atlys.py` & `litex-boards-2023.8/litex_boards/targets/digilent_atlys.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/digilent_basys3.py` & `litex-boards-2023.8/litex_boards/targets/digilent_basys3.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/digilent_cmod_a7.py` & `litex-boards-2023.8/litex_boards/targets/digilent_cmod_a7.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/digilent_genesys2.py` & `litex-boards-2023.8/litex_boards/targets/digilent_genesys2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/digilent_nexys4.py` & `litex-boards-2023.8/litex_boards/targets/digilent_nexys4.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/digilent_nexys4ddr.py` & `litex-boards-2023.8/litex_boards/targets/opalkelly_xem8320.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,145 +1,162 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2018-2019 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2022 Andrew Elbert Wilson <Andrew.E.Wilson@ieee.org>
 # SPDX-License-Identifier: BSD-2-Clause
 
+import os
+
 from migen import *
+from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex_boards.platforms import digilent_nexys4ddr
+from litex_boards.platforms import opalkelly_xem8320
 
 from litex.soc.cores.clock import *
-from litex.soc.integration.soc import SoCRegion
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
-from litex.soc.cores.video import VideoVGAPHY
 from litex.soc.cores.led import LedChaser
+from litex.soc.cores.video import VideoDVIPHY
 
-from litedram.modules import MT47H64M16
-from litedram.phy import s7ddrphy
-
-from liteeth.phy.rmii import LiteEthPHYRMII
+from litedram.modules import MT40A512M16
+from litedram.phy import usddrphy
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq):
-        self.rst          = Signal()
-        self.cd_sys       = ClockDomain()
-        self.cd_sys2x     = ClockDomain()
-        self.cd_sys2x_dqs = ClockDomain()
-        self.cd_idelay    = ClockDomain()
-        self.cd_eth       = ClockDomain()
-        self.cd_vga       = ClockDomain()
+    def __init__(self, platform, sys_clk_freq, with_video_pll=False):
+        self.rst = Signal()
+        self.cd_sys    = ClockDomain()
+        self.cd_sys4x  = ClockDomain()
+        self.cd_idelay = ClockDomain()
+        if with_video_pll:
+            self.cd_hdmi   = ClockDomain()
+            self.cd_hdmi5x = ClockDomain()
+
         # # #
 
-        self.pll = pll = S7MMCM(speedgrade=-1)
-        self.comb += pll.reset.eq(~platform.request("cpu_reset") | self.rst)
-        pll.register_clkin(platform.request("clk100"), 100e6)
-        pll.create_clkout(self.cd_sys,       sys_clk_freq)
-        pll.create_clkout(self.cd_sys2x,     2*sys_clk_freq)
-        pll.create_clkout(self.cd_sys2x_dqs, 2*sys_clk_freq, phase=90)
-        pll.create_clkout(self.cd_idelay,    200e6)
-        pll.create_clkout(self.cd_eth,       50e6)
-        pll.create_clkout(self.cd_vga,       40e6)
+        # Clk.
+        clk100 = platform.request("ddr_clk100")
+
+        # PLL.
+        self.pll = pll = USMMCM(speedgrade=-2)
+        self.comb += pll.reset.eq(self.rst)
+        pll.register_clkin(clk100, 100e6)
+        pll.create_clkout(self.cd_sys,    sys_clk_freq, with_reset=False)
+        pll.create_clkout(self.cd_sys4x,  4*sys_clk_freq)
         platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
+        self.idelayctrl = USIDELAYCTRL(cd_ref=self.cd_sys4x, cd_sys=self.cd_sys)
 
-        self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
+        # Video PLL.
+        if with_video_pll:
+            self.video_pll = video_pll = USMMCM(speedgrade=-2)
+            video_pll.reset.eq(self.rst)
+            video_pll.register_clkin(self.cd_sys.clk, sys_clk_freq)
+            video_pll.create_clkout(self.cd_hdmi,   25e6)
+            video_pll.create_clkout(self.cd_hdmi5x, 5*25e6)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=75e6,
+    def __init__(self, sys_clk_freq=int(125e6),
         with_ethernet          = False,
         with_etherbone         = False,
+        eth_ip                 = "192.168.1.50",
         with_led_chaser        = True,
-        with_video_terminal    = False,
         with_video_framebuffer = False,
         **kwargs):
-        platform = digilent_nexys4ddr.Platform()
+        platform = opalkelly_xem8320.Platform()
+
+        # TODO: add okHost FrontPanel API for UART, Data streaing, and Debug
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = _CRG(platform, sys_clk_freq)
+        self.crg = _CRG(platform, sys_clk_freq, with_video_pll=with_video_framebuffer)
 
-        # SoCCore ----------------------------------_-----------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Nexys4DDR", **kwargs)
+        # SoCCore ----------------------------------------------------------------------------------
+        kwargs["uart_name"] = "jtag_uart"
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on XEM8320", **kwargs)
 
-        # DDR2 SDRAM -------------------------------------------------------------------------------
+        # DDR4 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
-            self.ddrphy = s7ddrphy.A7DDRPHY(platform.request("ddram"),
-                memtype      = "DDR2",
-                nphases      = 2,
-                sys_clk_freq = sys_clk_freq)
+            self.ddrphy = usddrphy.USPDDRPHY(platform.request("ddram"),
+                memtype          = "DDR4",
+                sys_clk_freq     = sys_clk_freq,
+                iodelay_clk_freq = 500e6)
             self.add_sdram("sdram",
                 phy           = self.ddrphy,
-                module        = MT47H64M16(sys_clk_freq, "1:2"),
+                module        = MT40A512M16(sys_clk_freq, "1:4"),
+                size          = 0x40000000,
                 l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
+        # TODO: add SFP+ cages for ethernet
         # Ethernet / Etherbone ---------------------------------------------------------------------
-        if with_ethernet or with_etherbone:
-            self.ethphy = LiteEthPHYRMII(
-                clock_pads = self.platform.request("eth_clocks"),
-                pads       = self.platform.request("eth"))
-            if with_ethernet:
-                self.add_ethernet(phy=self.ethphy)
-            if with_etherbone:
-                self.add_etherbone(phy=self.ethphy)
+        # if with_ethernet or with_etherbone:
+        #     self.ethphy = KU_1000BASEX(self.crg.cd_eth.clk,
+        #         data_pads    = self.platform.request("sfp", 0),
+        #         sys_clk_freq = self.clk_freq)
+        #     self.comb += self.platform.request("sfp_tx_disable_n", 0).eq(1)
+        #     self.platform.add_platform_command("set_property SEVERITY {{Warning}} [get_drc_checks REQP-1753]")
+        #     if with_ethernet:
+        #         self.add_ethernet(phy=self.ethphy)
+        #     if with_etherbone:
+        #         self.add_etherbone(phy=self.ethphy, ip_address=eth_ip)
 
         # Video ------------------------------------------------------------------------------------
-        if with_video_terminal or with_video_framebuffer:
-            self.videophy = VideoVGAPHY(platform.request("vga"), clock_domain="vga")
-            if with_video_terminal:
-                self.add_video_terminal(phy=self.videophy, timings="800x600@60Hz", clock_domain="vga")
-            if with_video_framebuffer:
-                self.add_video_framebuffer(phy=self.videophy, timings="800x600@60Hz", clock_domain="vga")
+        if with_video_framebuffer:
+            platform.add_extension(opalkelly_xem8320._dvi_pmod_io)
+            self.videophy = VideoDVIPHY(platform.request("dvi"), clock_domain="hdmi")
+            self.add_video_framebuffer(phy=self.videophy, timings="640x480@75Hz", clock_domain="hdmi")
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=digilent_nexys4ddr.Platform, description="LiteX SoC on Nexys4DDR.")
-    parser.add_target_argument("--sys-clk-freq", default=75e6, type=float, help="System clock frequency.")
-    ethopts = parser.target_group.add_mutually_exclusive_group()
-    ethopts.add_argument("--with-ethernet",         action="store_true", help="Enable Ethernet support.")
-    ethopts.add_argument("--with-etherbone",        action="store_true", help="Enable Etherbone support.")
-    sdopts = parser.target_group.add_mutually_exclusive_group()
-    sdopts.add_argument("--with-spi-sdcard",        action="store_true", help="Enable SPI-mode SDCard support.")
-    sdopts.add_argument("--with-sdcard",            action="store_true", help="Enable SDCard support.")
+    parser = LiteXArgumentParser(platform=opalkelly_xem8320.Platform, description="LiteX SoC on XEM8320.")
+    parser.add_target_argument("--sys-clk-freq",    default=125e6, type=float, help="System clock frequency.")
+    #ethopts = parser.target_group.add_mutually_exclusive_group()
+    #ethopts.add_argument("--with-ethernet",        action="store_true",    help="Enable Ethernet support.")
+    #ethopts.add_argument("--with-etherbone",       action="store_true",    help="Enable Etherbone support.")
+    #parser.add_target_argument("--eth-ip",         default="192.168.1.50", help="Ethernet/Etherbone IP address.")
+    #parser.add_target_argument("--eth-dynamic-ip", action="store_true",    help="Enable dynamic Ethernet IP addresses setting.")
     viopts = parser.target_group.add_mutually_exclusive_group()
-    viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (VGA).")
-    viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (VGA).")
+    viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (HDMI).")
+    viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (HDMI).")
     args = parser.parse_args()
 
+    #assert not (args.with_etherbone and args.eth_dynamic_ip)
+
     soc = BaseSoC(
         sys_clk_freq           = args.sys_clk_freq,
-        with_ethernet          = args.with_ethernet,
-        with_etherbone         = args.with_etherbone,
+        #with_ethernet         = args.with_ethernet,
+        #with_etherbone        = args.with_etherbone,
+        #eth_ip                = args.eth_ip,
+        #eth_dynamic_ip        = args.eth_dynamic_ip,
         with_video_terminal    = args.with_video_terminal,
         with_video_framebuffer = args.with_video_framebuffer,
         **parser.soc_argdict
-    )
-    if args.with_spi_sdcard:
-        soc.add_spi_sdcard()
-    if args.with_sdcard:
-        soc.add_sdcard()
+	)
+
+    soc.platform.add_extension(opalkelly_xem8320._sdcard_pmod_io)
+    soc.add_spi_sdcard()
+
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
     if args.load:
         prog = soc.platform.create_programmer()
         prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
+        # TODO: add option for FrontPanel Programming
 
 if __name__ == "__main__":
     main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/digilent_nexys_video.py` & `litex-boards-2023.8/litex_boards/targets/digilent_nexys_video.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         # PLL.
         if toolchain == "vivado":
             self.pll = pll = S7MMCM(speedgrade=-1)
         else:
             self.pll = pll = S7PLL(speedgrade=-1)
         self.comb += pll.reset.eq(~rst_n | self.rst)
         pll.register_clkin(clk100, 100e6)
-        pll.create_clkout(self.cd_sys,       sys_clk_freq, reset_buf="bufg")
+        pll.create_clkout(self.cd_sys,       sys_clk_freq)
         pll.create_clkout(self.cd_sys4x,     4*sys_clk_freq)
         pll.create_clkout(self.cd_sys4x_dqs, 4*sys_clk_freq, phase=90)
         pll.create_clkout(self.cd_idelay,    200e6)
         pll.create_clkout(self.cd_clk100,    100e6)
         platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
 
         self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
```

### Comparing `litex-boards-2023.12/litex_boards/targets/digilent_pynq_z1.py` & `litex-boards-2023.8/litex_boards/targets/digilent_pynq_z1.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/digilent_zedboard.py` & `litex-boards-2023.8/litex_boards/targets/digilent_zedboard.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/ebaz4205.py` & `litex-boards-2023.8/litex_boards/targets/ebaz4205.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/efinix_t8f81_dev_kit.py` & `litex-boards-2023.8/litex_boards/targets/efinix_t8f81_dev_kit.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/efinix_titanium_ti60_f225_dev_kit.py` & `litex-boards-2023.8/litex_boards/targets/efinix_titanium_ti60_f225_dev_kit.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/efinix_trion_t120_bga576_dev_kit.py` & `litex-boards-2023.8/litex_boards/targets/efinix_trion_t120_bga576_dev_kit.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/efinix_trion_t20_bga256_dev_kit.py` & `litex-boards-2023.8/litex_boards/targets/efinix_trion_t20_bga256_dev_kit.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/efinix_trion_t20_mipi_dev_kit.py` & `litex-boards-2023.8/litex_boards/targets/efinix_trion_t20_mipi_dev_kit.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/efinix_xyloni_dev_kit.py` & `litex-boards-2023.8/litex_boards/targets/efinix_xyloni_dev_kit.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/ego1.py` & `litex-boards-2023.8/litex_boards/targets/ego1.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/enclustra_mercury_kx2.py` & `litex-boards-2023.8/litex_boards/targets/enclustra_mercury_kx2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/enclustra_mercury_xu5.py` & `litex-boards-2023.8/litex_boards/targets/enclustra_mercury_xu5.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/fairwaves_xtrx.py` & `litex-boards-2023.8/litex_boards/targets/fairwaves_xtrx.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/fpc_iii.py` & `litex-boards-2023.8/litex_boards/targets/fpc_iii.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/fpgawars_alhambra2.py` & `litex-boards-2023.8/litex_boards/targets/fpgawars_alhambra2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/gadgetfactory_papilio_pro.py` & `litex-boards-2023.8/litex_boards/targets/gadgetfactory_papilio_pro.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/gsd_butterstick.py` & `litex-boards-2023.8/litex_boards/targets/gsd_butterstick.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/gsd_orangecrab.py` & `litex-boards-2023.8/litex_boards/targets/gsd_orangecrab.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/hackaday_hadbadge.py` & `litex-boards-2023.8/litex_boards/targets/hackaday_hadbadge.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/ice_v_wireless.py` & `litex-boards-2023.8/litex_boards/targets/ice_v_wireless.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/icebreaker.py` & `litex-boards-2023.8/litex_boards/targets/icebreaker.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/icebreaker_bitsy.py` & `litex-boards-2023.8/litex_boards/targets/icebreaker_bitsy.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/isx_im1283.py` & `litex-boards-2023.8/litex_boards/targets/isx_im1283.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,25 +47,29 @@
         platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
 
         self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=80e6, with_led_chaser=True, **kwargs):
+    def __init__(self, sys_clk_freq=80e6, with_led_chaser=True, with_jtagbone=True, **kwargs):
         platform = isx_im1283.Platform()
 
         # SoCCore ----------------------------------------------------------------------------------
         SoCCore.__init__(self, platform, sys_clk_freq,
             ident          = "LiteX SoC on ISX iM1283",
             **kwargs)
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
+        # Jtagbone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
+
         # DDR3 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
             self.ddrphy = s7ddrphy.A7DDRPHY(platform.request("ddram"),
                 memtype        = "DDR3",
                 nphases        = 4,
                 sys_clk_freq   = sys_clk_freq)
             self.add_sdram("sdram",
@@ -82,21 +86,23 @@
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
     parser = LiteXArgumentParser(platform=isx_im1283.Platform, description="LiteX SoC on iM1283.")
     parser.add_argument("--sys-clk-freq", default=80e6, type=float, help="System clock frequency.")
+    parser.add_target_argument("--with-jtagbone", action="store_true", help="Enable Jtagbone support.")
     sdopts = parser.add_mutually_exclusive_group()
     sdopts.add_argument("--with-spi-sdcard", action="store_true", help="Enable SPI-mode SDCard support.")
     sdopts.add_argument("--with-sdcard",     action="store_true", help="Enable SDCard support.")
     args = parser.parse_args()
 
     soc = BaseSoC(
         sys_clk_freq = args.sys_clk_freq,
+        with_jtagbone = args.with_jtagbone,
         **parser.soc_argdict
     )
     if args.with_spi_sdcard:
         soc.add_spi_sdcard()
     if args.with_sdcard:
         soc.add_sdcard()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/jungle_electronics_fireant.py` & `litex-boards-2023.8/litex_boards/targets/jungle_electronics_fireant.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/kosagi_fomu.py` & `litex-boards-2023.8/litex_boards/targets/kosagi_fomu.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/kosagi_netv2.py` & `litex-boards-2023.8/litex_boards/targets/kosagi_netv2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/krtkl_snickerdoodle.py` & `litex-boards-2023.8/litex_boards/targets/krtkl_snickerdoodle.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/lambdaconcept_ecpix5.py` & `litex-boards-2023.8/litex_boards/targets/lambdaconcept_ecpix5.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/lattice_crosslink_nx_evn.py` & `litex-boards-2023.8/litex_boards/targets/lattice_crosslink_nx_evn.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         "main_ram" : 0x60000000,
         "csr"      : 0xf0000000,
     }
 
     def __init__(self, sys_clk_freq=75e6, device="LIFCL-40-9BG400C", toolchain="radiant",
         with_led_chaser = True,
         with_spi_flash  = False,
+        with_uartbone   = False,
         **kwargs):
         platform = lattice_crosslink_nx_evn.Platform(device=device, toolchain=toolchain)
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore -----------------------------------------_----------------------------------------
@@ -94,14 +95,18 @@
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = Cat(*[platform.request("user_led", i) for i in range(14)]),
                 sys_clk_freq = sys_clk_freq)
 
+        # UARTBone ---------------------------------------------------------------------------------
+        if with_uartbone:
+            self.add_uartbone()
+
         # SPI Flash --------------------------------------------------------------------------------
         if with_spi_flash:
             from litespi.modules import MX25L12833F
             from litespi.opcodes import SpiNorFlashOpCodes as Codes
             self.add_spi_flash(mode="4x", clk_freq=100_000, module=MX25L12833F(Codes.READ_4_4_4), with_master=True)
 
 
@@ -113,21 +118,23 @@
     parser.add_target_argument("--device",        default="LIFCL-40-9BG400C", help="FPGA device (LIFCL-40-9BG400C, LIFCL-40-8BG400CES, or LIFCL-40-8BG400CES2).")
     parser.add_target_argument("--sys-clk-freq",  default=75e6, type=float,   help="System clock frequency.")
     parser.add_target_argument("--serial",        default="serial",           help="UART Pins (serial (requires R15 and R17 to be soldered) or serial_pmod[0-2]).")
     parser.add_target_argument("--programmer",    default="radiant",          help="Programmer (radiant or ecpprog or openocd).")
     parser.add_target_argument("--address",       default=0x0,                help="Flash address to program bitstream at.")
     parser.add_target_argument("--prog-target",   default="direct",           help="Programming Target (direct or flash).")
     parser.add_target_argument("--with-spi-flash", action="store_true",       help="Enable SPI Flash (MMAPed).")
+    parser.add_target_argument("--with-uartbone", action="store_true",        help="Add UartBone on 1st serial.")
     args = parser.parse_args()
 
     soc = BaseSoC(
         sys_clk_freq = args.sys_clk_freq,
         device       = args.device,
         toolchain    = args.toolchain,
         with_spi_flash = args.with_spi_flash,
+        with_uartbone = args.with_uartbone,
         **parser.soc_argdict
     )
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
     if args.load:
```

### Comparing `litex-boards-2023.12/litex_boards/targets/lattice_crosslink_nx_vip.py` & `litex-boards-2023.8/litex_boards/targets/lattice_crosslink_nx_vip.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/lattice_ecp5_evn.py` & `litex-boards-2023.8/litex_boards/targets/lattice_ecp5_evn.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,42 +42,49 @@
         pll.create_clkout(self.cd_sys, sys_clk_freq)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
     def __init__(self, sys_clk_freq=50e6, toolchain="trellis", x5_clk_freq=None,
         with_led_chaser = True,
+        with_jtagbone   = True,
         **kwargs):
         platform = lattice_ecp5_evn.Platform(toolchain=toolchain)
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq, x5_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
         SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on ECP5 Evaluation Board", **kwargs)
 
+        # JtagBone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
+
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
     parser = LiteXArgumentParser(platform=lattice_ecp5_evn.Platform, description="LiteX SoC on ECP5 Evaluation Board.")
     parser.add_target_argument("--sys-clk-freq", default=60e6, type=float, help="System clock frequency.")
     parser.add_target_argument("--x5-clk-freq",  type=int,                 help="Use X5 oscillator as system clock at the specified frequency.")
+    parser.add_target_argument("--with-jtagbone", action="store_true",     help="Add JTAGBone.")
     args = parser.parse_args()
 
     soc = BaseSoC(
         toolchain    = args.toolchain,
         sys_clk_freq = args.sys_clk_freq,
         x5_clk_freq  = args.x5_clk_freq,
+        with_jtagbone = args.with_jtagbone,
         **parser.soc_argdict)
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
     if args.load:
         prog = soc.platform.create_programmer()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/lattice_ecp5_vip.py` & `litex-boards-2023.8/litex_boards/targets/lattice_ecp5_vip.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/lattice_ice40up5k_evn.py` & `litex-boards-2023.8/litex_boards/targets/lattice_ice40up5k_evn.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,19 @@
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led_n"),
                 sys_clk_freq = sys_clk_freq)
 
+        # Add a UARTBone bridge --------------------------------------------------------------------
+        debug_uart = False
+        if debug_uart:
+            self.add_uartbone()
+
 # Flash --------------------------------------------------------------------------------------------
 
 def flash(bios_flash_offset, target="lattice_ice40up5k_evn"):
     from litex.build.dfu import DFUProg
     prog = IceStormProgrammer()
     bitstream  = open("build/"+target+"/gateware/"+target+".bin",  "rb")
     bios       = open("build/"+target+"/software/bios/bios.bin", "rb")
```

### Comparing `litex-boards-2023.12/litex_boards/targets/lattice_versa_ecp5.py` & `litex-boards-2023.8/litex_boards/targets/lattice_versa_ecp5.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/limesdr_mini_v2.py` & `litex-boards-2023.8/litex_boards/targets/limesdr_mini_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,18 +71,20 @@
     def __init__(self, sys_clk_freq=80e6, toolchain="trellis",
         with_usb_fifo   = True, with_usb_fifo_loopback=False,
         with_led_chaser = True,
         **kwargs):
         platform = limesdr_mini_v2.Platform(toolchain=toolchain)
 
         # SoCCore ----------------------------------------------------------------------------------
-        kwargs["uart_name"]     = "crossover"
-        kwargs["with_jtagbone"] = True
+        kwargs["uart_name"] = "crossover"
         SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on LimeSDR-Mini-V2", **kwargs)
 
+        # JTAGBone ---------------------------------------------------------------------------------
+        self.add_jtagbone()
+
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
         # Info -------------------------------------------------------------------------------------
         self.info = BoardInfo(platform.request("revision"))
 
         # I2C Bus ----------------------------------------------------------------------------------
```

### Comparing `litex-boards-2023.12/litex_boards/targets/linsn_rv901t.py` & `litex-boards-2023.8/litex_boards/targets/linsn_rv901t.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/litex_acorn_baseboard.py` & `litex-boards-2023.8/litex_boards/targets/litex_acorn_baseboard.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/logicbone.py` & `litex-boards-2023.8/litex_boards/targets/logicbone.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/machdyne_konfekt.py` & `litex-boards-2023.8/litex_boards/targets/machdyne_konfekt.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/machdyne_kopflos.py` & `litex-boards-2023.8/litex_boards/targets/machdyne_kopflos.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/machdyne_krote.py` & `litex-boards-2023.8/litex_boards/targets/machdyne_krote.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/machdyne_mozart_ml1.py` & `litex-boards-2023.8/litex_boards/targets/machdyne_schoko.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,49 +12,43 @@
 import sys
 import json
 
 from migen import *
 
 from litex.gen import *
 
-from litex_boards.platforms import machdyne_mozart_ml1
+from litex_boards.platforms import machdyne_schoko
 
 from litex.build.io import DDROutput
 
-from litex.build.lattice.trellis import trellis_args, trellis_argdict
-
-from migen.genlib.resetsync import AsyncResetSynchronizer
-
 from litex.soc.cores.clock import *
+from litex.soc.cores.led import LedChaser
 from litex.soc.cores.usb_ohci import USBOHCI
+from litex.soc.cores.video import VideoVGAPHY
 from litex.soc.cores.video import VideoHDMIPHY
 
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
-from litex.soc.interconnect.csr_eventmanager import *
 
 from litedram.modules import W9825G6KH6
 from litedram.phy import GENSDRPHY, HalfRateGENSDRPHY
+#from litedram.phy import QuarterRateGENSDRPHY
 
 from litex.soc.integration.soc import SoCRegion
 
 # CRG ---------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
     def __init__(self, platform, sys_clk_freq, sdram_rate):
         self.rst        = Signal()
         self.cd_por     = ClockDomain()
         self.cd_sys     = ClockDomain()
-        self.cd_init    = ClockDomain()
         self.cd_video   = ClockDomain()
         self.cd_video5x = ClockDomain()
 
-        self.stop  = Signal()
-        self.reset = Signal()
-
         # Clk / Rst
         clk48 = platform.request("clk48")
 
         # Power on reset
         por_count = Signal(16, reset=2**16-1)
         por_done  = Signal()
         self.comb += self.cd_por.clk.eq(clk48)
@@ -87,47 +81,46 @@
             sdram_clk = ClockSignal("sys2x_ps")
         elif sdram_rate == "1:4":
             sdram_clk = ClockSignal("sys4x_ps")
         else:
             sdram_clk = ClockSignal("sys_ps")
 
         self.specials += DDROutput(1, 0, platform.request("sdram_clock"), sdram_clk)
-
         pll2 = ECP5PLL()
         self.pll2 = pll2
         pll2.register_clkin(clk48, 48e6)
         pll2.create_clkout(self.cd_video, 25e6)
         pll2.create_clkout(self.cd_video5x, 125e6)
 
-        pll3 = ECP5PLL()
-        self.pll3 = pll3
-        pll3.register_clkin(clk48, 48e6)
         self.cd_usb_12 = ClockDomain()
         self.cd_usb = ClockDomain()
         self.cd_usb_48 = ClockDomain()
         self.cd_usb_48 = self.cd_usb
-        pll3.create_clkout(self.cd_usb, 48e6)
-        pll3.create_clkout(self.cd_usb_12, 12e6)
-        self.comb += pll3.reset.eq(~por_done)
+        pll2.create_clkout(self.cd_usb, 48e6)
+        pll2.create_clkout(self.cd_usb_12, 12e6)
+        self.comb += pll2.reset.eq(~por_done)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
     mem_map = {**SoCCore.mem_map, **{
         "usb_ohci":     0xc0000000,
     }}
-    def __init__(self, revision="v0", device="45F", sdram_rate="1:2", sys_clk_freq=int(48e6), toolchain="trellis", with_usb_host=False, with_ethernet=False, **kwargs):
-
-        platform = machdyne_mozart_ml1.Platform(revision=revision, device=device ,toolchain=toolchain)
+    def __init__(self, revision="v1", device="45F",  sys_clk_freq=40e6, toolchain="trellis",
+        sdram_rate      = "1:2",
+        with_led_chaser = True,
+        with_usb_host   = False,
+        **kwargs):
+        platform = machdyne_schoko.Platform(revision=revision, device=device ,toolchain=toolchain)
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq, sdram_rate=sdram_rate)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Mozart ML1", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Schoko", **kwargs)
 
         # DRAM -------------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
             if sdram_rate == "1:2":
                 sdrphy_cls = HalfRateGENSDRPHY
             elif sdram_rate == "1:4":
                 sdrphy_cls = QuarterRateGENSDRPHY
@@ -137,82 +130,83 @@
             self.sdrphy = sdrphy_cls(platform.request("sdram"), sys_clk_freq)
             self.add_sdram("sdram",
                 phy           = self.sdrphy,
                 module        = W9825G6KH6(sys_clk_freq, sdram_rate),
                 l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
-        # DDMI Framebuffer -------------------------------------------------------------------------------------
-        self.videophy = VideoHDMIPHY(platform.request("ddmi"),
-            clock_domain="video")
-        self.add_video_framebuffer(phy=self.videophy, timings="640x480@60Hz",
-            clock_domain="video", format="rgb565")
-
         # USB Host ---------------------------------------------------------------------------------
         if with_usb_host:
             self.usb_ohci = USBOHCI(platform, platform.request("usb_host"), usb_clk_freq=int(48e6))
             self.bus.add_slave("usb_ohci_ctrl", self.usb_ohci.wb_ctrl, region=SoCRegion(origin=self.mem_map["usb_ohci"], size=0x100000, cached=False))
             self.dma_bus.add_master("usb_ohci_dma", master=self.usb_ohci.wb_dma)
             self.comb += self.cpu.interrupt[16].eq(self.usb_ohci.interrupt)
 
-        # Ethernet ---------------------------------------------------------------------------------
-        if with_ethernet:
-            from liteeth.phy.rmii import LiteEthPHYRMII
-            self.ethphy = LiteEthPHYRMII(
-                clock_pads = platform.request("eth_clocks"),
-                pads = platform.request("eth"),
-                with_hw_init_reset=True,
-                refclk_cd=None)
-            self.add_ethernet(phy=self.ethphy)
+        # VGA Framebuffer --------------------------------------------------------------------------
+        #self.videophy = VideoVGAPHY(platform.request("vga"),
+        #    clock_domain="video")
+        #self.add_video_framebuffer(phy=self.videophy, timings="640x480@60Hz",
+        #    clock_domain="video", format="rgb565")
+
+        # VGA Terminal -------------------------------------------------------------------------------------
+        #self.videophy = VideoVGAPHY(platform.request("vga"),
+        #    clock_domain="video")
+        #self.add_video_terminal(phy=self.videophy, timings="640x480@60Hz",
+        #    clock_domain="video")
+
+        # DDMI Framebuffer -------------------------------------------------------------------------------------
+        self.videophy = VideoHDMIPHY(platform.request("ddmi"),
+            clock_domain="video")
+        self.add_video_framebuffer(phy=self.videophy, timings="640x480@60Hz",
+            clock_domain="video", format="rgb565")
+
+        # DDMI Terminal -------------------------------------------------------------------------------------
+        #self.videophy = VideoHDMIPHY(platform.request("ddmi"),
+        #    clock_domain="video")
+        #self.add_video_terminal(phy=self.videophy, timings="640x480@60Hz",
+        #    clock_domain="video")
+
+        # Leds -------------------------------------------------------------------------------------
+        if with_led_chaser:
+            self.leds = LedChaser(
+                pads         = platform.request_all("user_led"),
+                sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
-    from litex.soc.integration.soc import LiteXSoCArgumentParser
-    parser = LiteXSoCArgumentParser(description="LiteX SoC on Mozart ML1")
-    target_group = parser.add_argument_group(title="Target options")
-    target_group.add_argument("--build",           action="store_true",  help="Build design.")
-    target_group.add_argument("--load",            action="store_true",  help="Load bitstream to SRAM.")
-    target_group.add_argument("--flash",           action="store_true",  help="Flash bitstream to MMOD.")
-    target_group.add_argument("--toolchain",       default="trellis",    help="FPGA toolchain (trellis or diamond).")
-    target_group.add_argument("--sys-clk-freq",    default=48e6,         help="System clock frequency.")
-    target_group.add_argument("--revision",        default="v0",         help="Board Revision (v0).")
-    target_group.add_argument("--device",          default="45F",        help="ECP5 device (12F, 25F, 45F or 85F).")
-    target_group.add_argument("--cable",           default="usb-blaster", help="Specify an openFPGALoader cable.")
-    target_group.add_argument("--with-sdcard",     action="store_true",  help="Enable SDCard support.")
-    target_group.add_argument("--with-spi-sdcard", action="store_true",  help="Enable SPI-mode SDCard support.")
-    target_group.add_argument("--with-usb-host",   action="store_true",  help="Enable USB host support.")
-    target_group.add_argument("--with-ethernet",   action="store_true",  help="Enable ethernet support.")
-    target_group.add_argument("--boot-from-flash", action="store_true",  help="Boot from flash MMOD.")
-
-    builder_args(parser)
-    soc_core_args(parser)
-    trellis_args(parser)
+    from litex.build.parser import LiteXArgumentParser
+    parser = LiteXArgumentParser(platform=machdyne_schoko.Platform, description="LiteX SoC on Schoko.")
+    parser.add_target_argument("--flash",           action="store_true",       help="Flash bitstream to MMOD.")
+    parser.add_target_argument("--sys-clk-freq",    default=40e6,  type=float, help="System clock frequency.")
+    parser.add_target_argument("--revision",        default="v1",              help="Board Revision (v1, v2).")
+    parser.add_target_argument("--device",          default="45F",             help="ECP5 device (25F, 45F or 85F).")
+    parser.add_target_argument("--cable",           default="usb-blaster",     help="Specify an openFPGALoader cable.")
+    parser.add_target_argument("--with-sdcard",     action="store_true",       help="Enable SDCard support.")
+    parser.add_target_argument("--with-spi-sdcard", action="store_true",       help="Enable SPI-mode SDCard support.")
+    parser.add_target_argument("--with-usb-host",   action="store_true",       help="Enable USB host support.")
     args = parser.parse_args()
 
     soc = BaseSoC(
         toolchain    = args.toolchain,
         revision     = args.revision,
         device       = args.device,
-        sys_clk_freq = int(float(args.sys_clk_freq)),
-        with_usb_host = args.with_usb_host,
-        with_ethernet = args.with_ethernet,
-        **soc_core_argdict(args))
+        sys_clk_freq = args.sys_clk_freq,
+        **parser.soc_argdict)
 
     if args.with_sdcard:
         soc.add_sdcard()
 
     if args.with_spi_sdcard:
         soc.add_spi_sdcard()
 
-    builder = Builder(soc, **builder_argdict(args))
-    builder_kargs = trellis_argdict(args) if args.toolchain == "trellis" else {}
+    builder = Builder(soc, **parser.builder_argdict)
 
     if args.build:
-        builder.build(**builder_kargs)
+        builder.build(**parser.toolchain_argdict)
 
     if args.load:
         prog = soc.platform.create_programmer(args.cable)
         prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
 
     if args.flash:
         prog = soc.platform.create_programmer(args.cable)
```

### Comparing `litex-boards-2023.12/litex_boards/targets/machdyne_noir.py` & `litex-boards-2023.8/litex_boards/targets/machdyne_noir.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/machdyne_schoko.py` & `litex-boards-2023.8/litex_boards/targets/trellisboard.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,216 +1,214 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) Lone Dynamics Corporation <info@lonedynamics.com>
-#
+# Copyright (c) 2019 David Shah <dave@ds0.me>
 # SPDX-License-Identifier: BSD-2-Clause
-#
-
-import os
-import sys
-import json
 
 from migen import *
+from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex_boards.platforms import machdyne_schoko
-
-from litex.build.io import DDROutput
+from litex_boards.platforms import trellisboard
 
 from litex.soc.cores.clock import *
-from litex.soc.cores.led import LedChaser
-from litex.soc.cores.usb_ohci import USBOHCI
-from litex.soc.cores.video import VideoVGAPHY
-from litex.soc.cores.video import VideoHDMIPHY
-
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
+from litex.soc.cores.led import LedChaser
+from litex.soc.cores.gpio import GPIOTristate
+from litex.soc.cores.video import VideoDVIPHY
+from litex.soc.cores.bitbang import I2CMaster
 
-from litedram.modules import W9825G6KH6
-from litedram.phy import GENSDRPHY, HalfRateGENSDRPHY
-#from litedram.phy import QuarterRateGENSDRPHY
+from litedram.modules import MT41J256M16
+from litedram.phy import ECP5DDRPHY
 
-from litex.soc.integration.soc import SoCRegion
+from liteeth.phy.ecp5rgmii import LiteEthPHYRGMII
 
-# CRG ---------------------------------------------------------------------------------------------
+# CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq, sdram_rate):
+    def __init__(self, platform, sys_clk_freq):
+        self.rst    = Signal()
+        self.cd_por = ClockDomain()
+        self.cd_sys = ClockDomain()
+
+        # # #
+
+        # Clk / Rst
+        clk12 = platform.request("clk12")
+        rst   = platform.request("user_btn", 0)
+
+        # Power on reset
+        por_count = Signal(16, reset=2**16-1)
+        por_done  = Signal()
+        self.comb += self.cd_por.clk.eq(clk12)
+        self.comb += por_done.eq(por_count == 0)
+        self.sync.por += If(~por_done, por_count.eq(por_count - 1))
+
+        # PLL
+        self.pll = pll = ECP5PLL()
+        self.comb += pll.reset.eq(~por_done | rst | self.rst)
+        pll.register_clkin(clk12, 12e6)
+        pll.create_clkout(self.cd_sys, sys_clk_freq)
+
+
+class _CRGSDRAM(LiteXModule):
+    def __init__(self, platform, sys_clk_freq):
         self.rst        = Signal()
+        self.cd_init    = ClockDomain()
         self.cd_por     = ClockDomain()
         self.cd_sys     = ClockDomain()
-        self.cd_video   = ClockDomain()
-        self.cd_video5x = ClockDomain()
+        self.cd_sys2x   = ClockDomain()
+        self.cd_sys2x_i = ClockDomain()
+
+        # # #
+
+        self.stop  = Signal()
+        self.reset = Signal()
 
         # Clk / Rst
-        clk48 = platform.request("clk48")
+        clk12 = platform.request("clk12")
+        rst   = platform.request("user_btn", 0)
 
         # Power on reset
         por_count = Signal(16, reset=2**16-1)
         por_done  = Signal()
-        self.comb += self.cd_por.clk.eq(clk48)
+        self.comb += self.cd_por.clk.eq(clk12)
         self.comb += por_done.eq(por_count == 0)
         self.sync.por += If(~por_done, por_count.eq(por_count - 1))
 
         # PLL
+        sys2x_clk_ecsout = Signal()
         self.pll = pll = ECP5PLL()
-        self.comb += pll.reset.eq(~por_done | self.rst)
-        pll.register_clkin(clk48, 48e6)
-        pll.create_clkout(self.cd_sys, sys_clk_freq)
+        self.comb += pll.reset.eq(~por_done | rst | self.rst)
+        pll.register_clkin(clk12, 12e6)
+        pll.create_clkout(self.cd_sys2x_i, 2*sys_clk_freq)
+        pll.create_clkout(self.cd_init,   25e6)
+        self.specials += [
+            Instance("ECLKBRIDGECS",
+                i_CLK0   = self.cd_sys2x_i.clk,
+                i_SEL    = 0,
+                o_ECSOUT = sys2x_clk_ecsout,
+            ),
+            Instance("ECLKSYNCB",
+                i_ECLKI = sys2x_clk_ecsout,
+                i_STOP  = self.stop,
+                o_ECLKO = self.cd_sys2x.clk),
+            Instance("CLKDIVF",
+                p_DIV     = "2.0",
+                i_ALIGNWD = 0,
+                i_CLKI    = self.cd_sys2x.clk,
+                i_RST     = self.reset,
+                o_CDIVX   = self.cd_sys.clk),
+            AsyncResetSynchronizer(self.cd_sys, ~pll.locked | self.reset),
+        ]
 
-        if sdram_rate == "1:2":
-            self.cd_sys2x = ClockDomain()
-            self.cd_sys2x_ps = ClockDomain()
-            pll.create_clkout(self.cd_sys2x,    2*sys_clk_freq)
-            pll.create_clkout(self.cd_sys2x_ps, 2*sys_clk_freq, phase=180)
-        elif sdram_rate == "1:4":
-            self.cd_sys2x = ClockDomain()
-            self.cd_sys4x = ClockDomain()
-            self.cd_sys4x_ps = ClockDomain()
-            pll.create_clkout(self.cd_sys2x,    2*sys_clk_freq)
-            pll.create_clkout(self.cd_sys4x,    4*sys_clk_freq)
-            pll.create_clkout(self.cd_sys4x_ps, 4*sys_clk_freq, phase=180)
-        else:
-            self.cd_sys_ps = ClockDomain()
-            pll.create_clkout(self.cd_sys_ps, sys_clk_freq, phase=90)
-
-        if sdram_rate == "1:2":
-            sdram_clk = ClockSignal("sys2x_ps")
-        elif sdram_rate == "1:4":
-            sdram_clk = ClockSignal("sys4x_ps")
-        else:
-            sdram_clk = ClockSignal("sys_ps")
-
-        self.specials += DDROutput(1, 0, platform.request("sdram_clock"), sdram_clk)
-        pll2 = ECP5PLL()
-        self.pll2 = pll2
-        pll2.register_clkin(clk48, 48e6)
-        pll2.create_clkout(self.cd_video, 25e6)
-        pll2.create_clkout(self.cd_video5x, 125e6)
-
-        self.cd_usb_12 = ClockDomain()
-        self.cd_usb = ClockDomain()
-        self.cd_usb_48 = ClockDomain()
-        self.cd_usb_48 = self.cd_usb
-        pll2.create_clkout(self.cd_usb, 48e6)
-        pll2.create_clkout(self.cd_usb_12, 12e6)
-        self.comb += pll2.reset.eq(~por_done)
+        self.comb += platform.request("dram_vtt_en").eq(1)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    mem_map = {**SoCCore.mem_map, **{
-        "usb_ohci":     0xc0000000,
-    }}
-    def __init__(self, revision="v1", device="45F",  sys_clk_freq=40e6, toolchain="trellis",
-        sdram_rate      = "1:2",
-        with_led_chaser = True,
-        with_usb_host   = False,
+    def __init__(self, sys_clk_freq=75e6, toolchain="trellis",
+        with_ethernet          = False,
+        with_video_terminal    = False,
+        with_video_framebuffer = False,
+        with_led_chaser        = True,
+        with_pmod_gpio         = False,
         **kwargs):
-        platform = machdyne_schoko.Platform(revision=revision, device=device ,toolchain=toolchain)
+        platform = trellisboard.Platform(toolchain=toolchain)
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = _CRG(platform, sys_clk_freq, sdram_rate=sdram_rate)
+        crg_cls = _CRGSDRAM if kwargs.get("integrated_main_ram_size", 0) == 0 else _CRG
+        self.crg = crg_cls(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Schoko", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Trellis Board", **kwargs)
 
-        # DRAM -------------------------------------------------------------------------------------
+        # DDR3 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
-            if sdram_rate == "1:2":
-                sdrphy_cls = HalfRateGENSDRPHY
-            elif sdram_rate == "1:4":
-                sdrphy_cls = QuarterRateGENSDRPHY
-            else:
-                sdrphy_cls = GENSDRPHY
-
-            self.sdrphy = sdrphy_cls(platform.request("sdram"), sys_clk_freq)
+            self.ddrphy = ECP5DDRPHY(
+                platform.request("ddram"),
+                sys_clk_freq=sys_clk_freq)
+            self.comb += self.crg.stop.eq(self.ddrphy.init.stop)
+            self.comb += self.crg.reset.eq(self.ddrphy.init.reset)
             self.add_sdram("sdram",
-                phy           = self.sdrphy,
-                module        = W9825G6KH6(sys_clk_freq, sdram_rate),
-                l2_cache_size = kwargs.get("l2_size", 8192)
+                phy           = self.ddrphy,
+                module        = MT41J256M16(sys_clk_freq, "1:2"),
+                l2_cache_size = kwargs.get("l2_size", 8192),
             )
 
-        # USB Host ---------------------------------------------------------------------------------
-        if with_usb_host:
-            self.usb_ohci = USBOHCI(platform, platform.request("usb_host"), usb_clk_freq=int(48e6))
-            self.bus.add_slave("usb_ohci_ctrl", self.usb_ohci.wb_ctrl, region=SoCRegion(origin=self.mem_map["usb_ohci"], size=0x100000, cached=False))
-            self.dma_bus.add_master("usb_ohci_dma", master=self.usb_ohci.wb_dma)
-            self.comb += self.cpu.interrupt[16].eq(self.usb_ohci.interrupt)
-
-        # VGA Framebuffer --------------------------------------------------------------------------
-        #self.videophy = VideoVGAPHY(platform.request("vga"),
-        #    clock_domain="video")
-        #self.add_video_framebuffer(phy=self.videophy, timings="640x480@60Hz",
-        #    clock_domain="video", format="rgb565")
-
-        # VGA Terminal -------------------------------------------------------------------------------------
-        #self.videophy = VideoVGAPHY(platform.request("vga"),
-        #    clock_domain="video")
-        #self.add_video_terminal(phy=self.videophy, timings="640x480@60Hz",
-        #    clock_domain="video")
-
-        # DDMI Framebuffer -------------------------------------------------------------------------------------
-        self.videophy = VideoHDMIPHY(platform.request("ddmi"),
-            clock_domain="video")
-        self.add_video_framebuffer(phy=self.videophy, timings="640x480@60Hz",
-            clock_domain="video", format="rgb565")
-
-        # DDMI Terminal -------------------------------------------------------------------------------------
-        #self.videophy = VideoHDMIPHY(platform.request("ddmi"),
-        #    clock_domain="video")
-        #self.add_video_terminal(phy=self.videophy, timings="640x480@60Hz",
-        #    clock_domain="video")
+        # Ethernet ---------------------------------------------------------------------------------
+        if with_ethernet:
+            self.ethphy = LiteEthPHYRGMII(
+                clock_pads = self.platform.request("eth_clocks"),
+                pads       = self.platform.request("eth"))
+            self.add_ethernet(phy=self.ethphy)
+
+        # HDMI -------------------------------------------------------------------------------------
+        if with_video_terminal or with_video_framebuffer:
+            # PHY + TP410 I2C initialization.
+            hdmi_pads = platform.request("hdmi")
+            self.videophy = VideoDVIPHY(hdmi_pads, clock_domain="init")
+            self.videoi2c = I2CMaster(hdmi_pads)
+            self.videoi2c.add_init(addr=0x38, init=[
+                (0x08, 0x35) # CTL_1_MODE: Normal operation, 24-bit, HSYNC/VSYNC.
+            ])
+
+            # Video Terminal/Framebuffer.
+            if with_video_terminal:
+                self.add_video_terminal(phy=self.videophy, timings="640x480@75Hz", clock_domain="init")
+            if with_video_framebuffer:
+                self.add_video_framebuffer(phy=self.videophy, timings="640x480@75Hz", clock_domain="init")
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
+        # GPIOs ------------------------------------------------------------------------------------
+        if with_pmod_gpio:
+            platform.add_extension(trellisboard.raw_pmod_io("pmoda"))
+            self.gpio = GPIOTristate(platform.request("pmoda"))
+
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=machdyne_schoko.Platform, description="LiteX SoC on Schoko.")
-    parser.add_target_argument("--flash",           action="store_true",       help="Flash bitstream to MMOD.")
-    parser.add_target_argument("--sys-clk-freq",    default=40e6,  type=float, help="System clock frequency.")
-    parser.add_target_argument("--revision",        default="v1",              help="Board Revision (v1, v2).")
-    parser.add_target_argument("--device",          default="45F",             help="ECP5 device (25F, 45F or 85F).")
-    parser.add_target_argument("--cable",           default="usb-blaster",     help="Specify an openFPGALoader cable.")
-    parser.add_target_argument("--with-sdcard",     action="store_true",       help="Enable SDCard support.")
-    parser.add_target_argument("--with-spi-sdcard", action="store_true",       help="Enable SPI-mode SDCard support.")
-    parser.add_target_argument("--with-usb-host",   action="store_true",       help="Enable USB host support.")
+    parser = LiteXArgumentParser(platform=trellisboard.Platform, description="LiteX SoC on Trellis Board.")
+    parser.add_target_argument("--sys-clk-freq",    default=75e6, type=float, help="System clock frequency.")
+    parser.add_target_argument("--with-ethernet",   action="store_true",      help="Enable Ethernet support.")
+    viopts = parser.target_group.add_mutually_exclusive_group()
+    viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (HDMI).")
+    viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (HDMI).")
+    sdopts = parser.target_group.add_mutually_exclusive_group()
+    sdopts.add_argument("--with-spi-sdcard",       action="store_true", help="Enable SPI-mode SDCard support.")
+    sdopts.add_argument("--with-sdcard",           action="store_true", help="Enable SDCard support.")
+    parser.add_target_argument("--with-pmod-gpio", action="store_true", help="Enable GPIOs through PMOD.") # FIXME: Temporary test.
     args = parser.parse_args()
 
     soc = BaseSoC(
-        toolchain    = args.toolchain,
-        revision     = args.revision,
-        device       = args.device,
-        sys_clk_freq = args.sys_clk_freq,
-        **parser.soc_argdict)
-
-    if args.with_sdcard:
-        soc.add_sdcard()
-
+        sys_clk_freq           = args.sys_clk_freq,
+        toolchain              = args.toolchain,
+        with_ethernet          = args.with_ethernet,
+        with_video_terminal    = args.with_video_terminal,
+        with_video_framebuffer = args.with_video_framebuffer,
+        with_pmod_gpio         = args.with_pmod_gpio,
+        **parser.soc_argdict
+    )
     if args.with_spi_sdcard:
         soc.add_spi_sdcard()
-
+    if args.with_sdcard:
+        soc.add_sdcard()
     builder = Builder(soc, **parser.builder_argdict)
-
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
     if args.load:
-        prog = soc.platform.create_programmer(args.cable)
-        prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
-
-    if args.flash:
-        prog = soc.platform.create_programmer(args.cable)
-        prog.flash(0x100000, builder.get_bitstream_filename(mode="sram"))
+        prog = soc.platform.create_programmer()
+        prog.load_bitstream(builder.get_bitstream_filename(mode="sram", ext=".svf")) # FIXME
 
 if __name__ == "__main__":
     main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/micronova_mercury2.py` & `litex-boards-2023.8/litex_boards/targets/micronova_mercury2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/mist.py` & `litex-boards-2023.8/litex_boards/targets/mist.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/mnt_rkx7.py` & `litex-boards-2023.8/litex_boards/targets/mnt_rkx7.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,14 @@
         **kwargs):
         platform = mnt_rkx7.Platform()
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        #kwargs["with_jtagbone"] = True
         SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on MNT-RKX7", **kwargs)
 
         # DDR3 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
             self.ddrphy = s7ddrphy.K7DDRPHY(platform.request("ddram"),
                 memtype      = "DDR3",
                 nphases      = 4,
@@ -139,14 +138,17 @@
         self.leds = GPIOOut(gpio_signals)
 
         # Additional I2C Ports ---------------------------------------------------------------------
         self.i2c0 = I2CMaster(platform.request("i2c", 0))
         self.i2c1 = I2CMaster(platform.request("i2c", 1))
         self.i2c2 = I2CMaster(platform.request("i2c", 2))
 
+        # JTAG -------------------------------------------------------------------------------------
+        #self.add_jtagbone()
+
         # Backlight --------------------------------------------------------------------------------
         # Motherboard display connector backlight, currently unused (the new backlight signals
         # are on the 50pin RGB->eDP connector)
         backlight = platform.request("backlight")
         self.comb += backlight.en.eq(Signal(reset=1))
         self.comb += backlight.pwm.eq(Signal(reset=1))
```

### Comparing `litex-boards-2023.12/litex_boards/targets/muselab_icesugar.py` & `litex-boards-2023.8/litex_boards/targets/muselab_icesugar.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/muselab_icesugar_pro.py` & `litex-boards-2023.8/litex_boards/targets/muselab_icesugar_pro.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/myminieye_runber.py` & `litex-boards-2023.8/litex_boards/targets/myminieye_runber.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/newae_cw305.py` & `litex-boards-2023.8/litex_boards/targets/newae_cw305.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,18 +61,20 @@
     def __init__(self, sys_clk_freq=100e6, with_led_chaser=True, **kwargs):
         platform = newae_cw305.Platform()
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        kwargs["uart_name"]     = "crossover"
-        kwargs["with_jtagbone"] = True
+        kwargs["uart_name"] = "crossover"
         SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on NewAE-CW305", **kwargs)
 
+        # JTAGBone ---------------------------------------------------------------------------------
+        self.add_jtagbone()
+
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq,
             )
```

### Comparing `litex-boards-2023.12/litex_boards/targets/numato_aller.py` & `litex-boards-2023.8/litex_boards/targets/numato_aller.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/numato_mimas_a7.py` & `litex-boards-2023.8/litex_boards/targets/numato_mimas_a7.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/numato_nereid.py` & `litex-boards-2023.8/litex_boards/targets/numato_nereid.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/numato_tagus.py` & `litex-boards-2023.8/litex_boards/targets/numato_tagus.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/ocp_tap_timecard.py` & `litex-boards-2023.8/litex_boards/targets/ocp_tap_timecard.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/opalkelly_xem8320.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_kc705.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,162 +1,177 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2022 Andrew Elbert Wilson <Andrew.E.Wilson@ieee.org>
+# Copyright (c) 2014-2015 Sebastien Bourdeauducq <sb@m-labs.hk>
+# Copyright (c) 2014-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2014-2015 Yann Sionneau <ys@m-labs.hk>
 # SPDX-License-Identifier: BSD-2-Clause
 
 import os
 
 from migen import *
-from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex_boards.platforms import opalkelly_xem8320
+from litex_boards.platforms import xilinx_kc705
 
 from litex.soc.cores.clock import *
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
 from litex.soc.cores.led import LedChaser
-from litex.soc.cores.video import VideoDVIPHY
 
-from litedram.modules import MT40A512M16
-from litedram.phy import usddrphy
+from litedram.modules import MT8JTF12864
+from litedram.phy import s7ddrphy
+
+from liteeth.phy import LiteEthPHY
+
+from litepcie.phy.s7pciephy import S7PCIEPHY
+from litepcie.software import generate_litepcie_software
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq, with_video_pll=False):
-        self.rst = Signal()
+    def __init__(self, platform, sys_clk_freq):
+        self.rst       = Signal()
         self.cd_sys    = ClockDomain()
         self.cd_sys4x  = ClockDomain()
         self.cd_idelay = ClockDomain()
-        if with_video_pll:
-            self.cd_hdmi   = ClockDomain()
-            self.cd_hdmi5x = ClockDomain()
 
         # # #
 
-        # Clk.
-        clk100 = platform.request("ddr_clk100")
-
-        # PLL.
-        self.pll = pll = USMMCM(speedgrade=-2)
-        self.comb += pll.reset.eq(self.rst)
-        pll.register_clkin(clk100, 100e6)
-        pll.create_clkout(self.cd_sys,    sys_clk_freq, with_reset=False)
+        self.pll = pll = S7MMCM(speedgrade=-2)
+        self.comb += pll.reset.eq(platform.request("cpu_reset") | self.rst)
+        pll.register_clkin(platform.request("clk200"), 200e6)
+        pll.create_clkout(self.cd_sys,    sys_clk_freq)
         pll.create_clkout(self.cd_sys4x,  4*sys_clk_freq)
+        pll.create_clkout(self.cd_idelay, 200e6)
         platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
-        self.idelayctrl = USIDELAYCTRL(cd_ref=self.cd_sys4x, cd_sys=self.cd_sys)
 
-        # Video PLL.
-        if with_video_pll:
-            self.video_pll = video_pll = USMMCM(speedgrade=-2)
-            video_pll.reset.eq(self.rst)
-            video_pll.register_clkin(self.cd_sys.clk, sys_clk_freq)
-            video_pll.create_clkout(self.cd_hdmi,   25e6)
-            video_pll.create_clkout(self.cd_hdmi5x, 5*25e6)
+        self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=int(125e6),
-        with_ethernet          = False,
-        with_etherbone         = False,
-        eth_ip                 = "192.168.1.50",
-        with_led_chaser        = True,
-        with_video_framebuffer = False,
+    def __init__(self, sys_clk_freq=125e6,
+        with_ethernet   = False,
+        with_led_chaser = True,
+        with_spi_flash  = False,
+        with_pcie       = False,
+        with_sata       = False,
         **kwargs):
-        platform = opalkelly_xem8320.Platform()
-
-        # TODO: add okHost FrontPanel API for UART, Data streaing, and Debug
+        platform = xilinx_kc705.Platform()
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = _CRG(platform, sys_clk_freq, with_video_pll=with_video_framebuffer)
+        self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        kwargs["uart_name"] = "jtag_uart"
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on XEM8320", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on KC705", **kwargs)
 
-        # DDR4 SDRAM -------------------------------------------------------------------------------
+        # DDR3 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
-            self.ddrphy = usddrphy.USPDDRPHY(platform.request("ddram"),
-                memtype          = "DDR4",
-                sys_clk_freq     = sys_clk_freq,
-                iodelay_clk_freq = 500e6)
+            self.ddrphy = s7ddrphy.K7DDRPHY(platform.request("ddram"),
+                memtype      = "DDR3",
+                nphases      = 4,
+                sys_clk_freq = sys_clk_freq)
             self.add_sdram("sdram",
                 phy           = self.ddrphy,
-                module        = MT40A512M16(sys_clk_freq, "1:4"),
-                size          = 0x40000000,
+                module        = MT8JTF12864(sys_clk_freq, "1:4"),
                 l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
-        # TODO: add SFP+ cages for ethernet
-        # Ethernet / Etherbone ---------------------------------------------------------------------
-        # if with_ethernet or with_etherbone:
-        #     self.ethphy = KU_1000BASEX(self.crg.cd_eth.clk,
-        #         data_pads    = self.platform.request("sfp", 0),
-        #         sys_clk_freq = self.clk_freq)
-        #     self.comb += self.platform.request("sfp_tx_disable_n", 0).eq(1)
-        #     self.platform.add_platform_command("set_property SEVERITY {{Warning}} [get_drc_checks REQP-1753]")
-        #     if with_ethernet:
-        #         self.add_ethernet(phy=self.ethphy)
-        #     if with_etherbone:
-        #         self.add_etherbone(phy=self.ethphy, ip_address=eth_ip)
-
-        # Video ------------------------------------------------------------------------------------
-        if with_video_framebuffer:
-            platform.add_extension(opalkelly_xem8320._dvi_pmod_io)
-            self.videophy = VideoDVIPHY(platform.request("dvi"), clock_domain="hdmi")
-            self.add_video_framebuffer(phy=self.videophy, timings="640x480@75Hz", clock_domain="hdmi")
+        # Ethernet ---------------------------------------------------------------------------------
+        if with_ethernet:
+            self.ethphy = LiteEthPHY(
+                clock_pads = self.platform.request("eth_clocks"),
+                pads       = self.platform.request("eth"),
+                clk_freq   = self.clk_freq)
+            self.add_ethernet(phy=self.ethphy)
+
+        # SPI Flash --------------------------------------------------------------------------------
+        if with_spi_flash:
+            from litespi.modules import N25Q128A13
+            from litespi.opcodes import SpiNorFlashOpCodes as Codes
+            self.add_spi_flash(mode="4x", module=N25Q128A13(Codes.READ_1_1_4), rate="1:1", with_master=True)
+
+        # PCIe -------------------------------------------------------------------------------------
+        if with_pcie:
+            self.pcie_phy = S7PCIEPHY(platform, platform.request("pcie_x4"),
+                data_width = 128,
+                bar0_size  = 0x20000)
+            self.add_pcie(phy=self.pcie_phy, ndmas=1)
+
+        # SATA -------------------------------------------------------------------------------------
+        if with_sata:
+            from litex.build.generic_platform import Subsignal, Pins
+            from litesata.phy import LiteSATAPHY
+
+            # IOs
+            _sata_io = [
+                # SFP 2 SATA Adapter / https://shop.trenz-electronic.de/en/TE0424-01-SFP-2-SATA-Adapter
+                ("sfp2sata", 0,
+                    Subsignal("tx_p", Pins("H2")),
+                    Subsignal("tx_n", Pins("H1")),
+                    Subsignal("rx_p", Pins("G4")),
+                    Subsignal("rx_n", Pins("G3")),
+                ),
+            ]
+            platform.add_extension(_sata_io)
+
+            # RefClk, Generate 150MHz from PLL.
+            self.cd_sata_refclk = ClockDomain()
+            self.crg.pll.create_clkout(self.cd_sata_refclk, 150e6)
+            sata_refclk = ClockSignal("sata_refclk")
+            platform.add_platform_command("set_property SEVERITY {{Warning}} [get_drc_checks REQP-52]")
+
+            # PHY
+            self.sata_phy = LiteSATAPHY(platform.device,
+                refclk     = sata_refclk,
+                pads       = platform.request("sfp2sata"),
+                gen        = "gen2",
+                clk_freq   = sys_clk_freq,
+                data_width = 16)
+
+            # Core
+            self.add_sata(phy=self.sata_phy, mode="read+write")
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=opalkelly_xem8320.Platform, description="LiteX SoC on XEM8320.")
-    parser.add_target_argument("--sys-clk-freq",    default=125e6, type=float, help="System clock frequency.")
-    #ethopts = parser.target_group.add_mutually_exclusive_group()
-    #ethopts.add_argument("--with-ethernet",        action="store_true",    help="Enable Ethernet support.")
-    #ethopts.add_argument("--with-etherbone",       action="store_true",    help="Enable Etherbone support.")
-    #parser.add_target_argument("--eth-ip",         default="192.168.1.50", help="Ethernet/Etherbone IP address.")
-    #parser.add_target_argument("--eth-dynamic-ip", action="store_true",    help="Enable dynamic Ethernet IP addresses setting.")
-    viopts = parser.target_group.add_mutually_exclusive_group()
-    viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (HDMI).")
-    viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (HDMI).")
+    parser = LiteXArgumentParser(platform=xilinx_kc705.Platform, description="LiteX SoC on KC705.")
+    parser.add_target_argument("--sys-clk-freq",   default=125e6, type=float, help="System clock frequency.")
+    parser.add_target_argument("--with-ethernet",  action="store_true",       help="Enable Ethernet support.")
+    parser.add_target_argument("--with-spi-flash", action="store_true",       help="Enable SPI Flash (MMAPed).")
+    parser.add_target_argument("--with-pcie",      action="store_true",       help="Enable PCIe support.")
+    parser.add_target_argument("--driver",         action="store_true",       help="Generate PCIe driver.")
+    parser.add_target_argument("--with-sata",      action="store_true",       help="Enable SATA support (over SFP2SATA).")
     args = parser.parse_args()
 
-    #assert not (args.with_etherbone and args.eth_dynamic_ip)
-
     soc = BaseSoC(
-        sys_clk_freq           = args.sys_clk_freq,
-        #with_ethernet         = args.with_ethernet,
-        #with_etherbone        = args.with_etherbone,
-        #eth_ip                = args.eth_ip,
-        #eth_dynamic_ip        = args.eth_dynamic_ip,
-        with_video_terminal    = args.with_video_terminal,
-        with_video_framebuffer = args.with_video_framebuffer,
+        sys_clk_freq   = args.sys_clk_freq,
+        with_ethernet  = args.with_ethernet,
+        with_spi_flash = args.with_spi_flash,
+        with_pcie      = args.with_pcie,
+        with_sata      = args.with_sata,
         **parser.soc_argdict
-	)
-
-    soc.platform.add_extension(opalkelly_xem8320._sdcard_pmod_io)
-    soc.add_spi_sdcard()
-
+    )
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
+    if args.driver:
+        generate_litepcie_software(soc, os.path.join(builder.output_dir, "driver"))
+
     if args.load:
         prog = soc.platform.create_programmer()
         prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
-        # TODO: add option for FrontPanel Programming
 
 if __name__ == "__main__":
     main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/pano_logic_g2.py` & `litex-boards-2023.8/litex_boards/targets/pano_logic_g2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/qmtech_10cl006.py` & `litex-boards-2023.8/litex_boards/targets/qmtech_10cl006.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/qmtech_5cefa2.py` & `litex-boards-2023.8/litex_boards/targets/qmtech_5cefa2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/qmtech_5cefa5.py` & `litex-boards-2023.8/litex_boards/targets/qmtech_5cefa5.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/qmtech_artix7_fbg484.py` & `litex-boards-2023.8/litex_boards/targets/qmtech_artix7_fgg676.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 #
 # This file is part of LiteX-Boards.
 #
 # Copyright (c) 2021 Hans Baier <hansfbaier@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
-# https://www.aliexpress.com/item/1005002960622091.html
+# https://www.aliexpress.com/item/4000170003461.html
 
 from migen import *
 
 from litex.gen import *
 
-from litex_boards.platforms import qmtech_artix7_fbg484
+from litex_boards.platforms import qmtech_artix7_fgg676
 
 from litex.soc.cores.clock import *
 from litex.soc.integration.soc import SoCRegion
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
 from litex.soc.cores.video import VideoVGAPHY
 from litex.soc.cores.led import LedChaser
@@ -63,25 +63,26 @@
         platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
 
         self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, toolchain="vivado", kgates=200, sys_clk_freq=100e6, with_daughterboard=False,
+    def __init__(self, toolchain="vivado", kgates=100, sys_clk_freq=100e6, with_daughterboard=False,
         with_ethernet          = False,
         with_etherbone         = False,
         eth_ip                 = "192.168.1.50",
         eth_dynamic_ip         = False,
         with_led_chaser        = True,
         with_video_terminal    = False,
         with_video_framebuffer = False,
+        with_jtagbone          = True,
         with_spi_flash         = False,
         **kwargs):
-        platform = qmtech_artix7_fbg484.Platform(kgates=kgates, toolchain=toolchain, with_daughterboard=with_daughterboard)
+        platform = qmtech_artix7_fgg676.Platform(kgates=kgates, toolchain=toolchain, with_daughterboard=with_daughterboard)
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq,
             with_ethernet = (with_ethernet or with_etherbone),
             with_vga      = (with_video_terminal or with_video_framebuffer)
         )
 
@@ -112,14 +113,18 @@
             if with_ethernet:
                 self.add_ethernet(phy=self.ethphy, dynamic_ip=eth_dynamic_ip)
             if with_etherbone:
                 self.add_etherbone(phy=self.ethphy, ip_address=eth_ip)
             # The daughterboard has the tx clock wired to a non-clock pin, so we can't help it
             self.platform.add_platform_command("set_property CLOCK_DEDICATED_ROUTE FALSE [get_nets eth_clocks_tx_IBUF]")
 
+        # Jtagbone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
+
         # SPI Flash --------------------------------------------------------------------------------
         if with_spi_flash:
             from litespi.modules import MT25QL128
             from litespi.opcodes import SpiNorFlashOpCodes as Codes
             self.add_spi_flash(mode="4x", module=MT25QL128(Codes.READ_1_1_1), with_master=True)
 
         # Video ------------------------------------------------------------------------------------
@@ -139,26 +144,27 @@
         if not with_daughterboard and kwargs["uart_name"] == "serial":
             kwargs["uart_name"] = "jtag_serial"
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=qmtech_artix7_fbg484.Platform, description="LiteX SoC on QMTech Artix7 FBG484.")
-    parser.add_target_argument("--kgates",              default=200,   type=int,  help="Number of kgates. Allowed values: 75, 100, 200, representing XC7A75T, XC7A100T and XC7A200T")
+    parser = LiteXArgumentParser(platform=qmtech_artix7_fgg676.Platform, description="LiteX SoC on QMTech XC7AXXXT.")
+    parser.add_target_argument("--kgates",              default=100,   type=int,  help="Number of kgates. Allowed values: 75, 100, 200, representing XC7A75T, XC7A100T and XC7A200T")
     parser.add_target_argument("--sys-clk-freq",        default=100e6, type=float,  help="System clock frequency.")
     parser.add_target_argument("--with-daughterboard",  action="store_true",        help="Board plugged into the QMTech daughterboard.")
     ethopts = parser.target_group.add_mutually_exclusive_group()
     ethopts.add_argument("--with-ethernet",        action="store_true",    help="Enable Ethernet support.")
     ethopts.add_argument("--with-etherbone",       action="store_true",    help="Enable Etherbone support.")
     parser.add_target_argument("--eth-ip",         default="192.168.1.50", help="Ethernet/Etherbone IP address.")
     parser.add_target_argument("--eth-dynamic-ip", action="store_true",    help="Enable dynamic Ethernet IP addresses setting.")
     sdopts = parser.target_group.add_mutually_exclusive_group()
     sdopts.add_argument("--with-spi-sdcard",       action="store_true", help="Enable SPI-mode SDCard support.")
     sdopts.add_argument("--with-sdcard",           action="store_true", help="Enable SDCard support.")
+    parser.add_target_argument("--with-jtagbone",  action="store_true", help="Enable Jtagbone support.")
     parser.add_target_argument("--with-spi-flash", action="store_true", help="Enable SPI Flash (MMAPed).")
     viopts = parser.target_group.add_mutually_exclusive_group()
     viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (VGA).")
     viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (VGA).")
     args = parser.parse_args()
 
     soc = BaseSoC(
@@ -166,14 +172,15 @@
         kgates                 = args.kgates,
         sys_clk_freq           = args.sys_clk_freq,
         with_daughterboard     = args.with_daughterboard,
         with_ethernet          = args.with_ethernet,
         with_etherbone         = args.with_etherbone,
         eth_ip                 = args.eth_ip,
         eth_dynamic_ip         = args.eth_dynamic_ip,
+        with_jtagbone          = args.with_jtagbone,
         with_spi_flash         = args.with_spi_flash,
         with_video_terminal    = args.with_video_terminal,
         with_video_framebuffer = args.with_video_framebuffer,
         **parser.soc_argdict
     )
 
     if args.with_spi_sdcard:
```

### Comparing `litex-boards-2023.12/litex_boards/targets/qmtech_artix7_fgg676.py` & `litex-boards-2023.8/litex_boards/targets/qmtech_artix7_fbg484.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 #
 # This file is part of LiteX-Boards.
 #
 # Copyright (c) 2021 Hans Baier <hansfbaier@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
-# https://www.aliexpress.com/item/4000170003461.html
+# https://www.aliexpress.com/item/1005002960622091.html
 
 from migen import *
 
 from litex.gen import *
 
-from litex_boards.platforms import qmtech_artix7_fgg676
+from litex_boards.platforms import qmtech_artix7_fbg484
 
 from litex.soc.cores.clock import *
 from litex.soc.integration.soc import SoCRegion
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
 from litex.soc.cores.video import VideoVGAPHY
 from litex.soc.cores.led import LedChaser
@@ -63,25 +63,26 @@
         platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
 
         self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, toolchain="vivado", kgates=100, sys_clk_freq=100e6, with_daughterboard=False,
+    def __init__(self, toolchain="vivado", kgates=200, sys_clk_freq=100e6, with_daughterboard=False,
         with_ethernet          = False,
         with_etherbone         = False,
         eth_ip                 = "192.168.1.50",
         eth_dynamic_ip         = False,
         with_led_chaser        = True,
         with_video_terminal    = False,
         with_video_framebuffer = False,
+        with_jtagbone          = True,
         with_spi_flash         = False,
         **kwargs):
-        platform = qmtech_artix7_fgg676.Platform(kgates=kgates, toolchain=toolchain, with_daughterboard=with_daughterboard)
+        platform = qmtech_artix7_fbg484.Platform(kgates=kgates, toolchain=toolchain, with_daughterboard=with_daughterboard)
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq,
             with_ethernet = (with_ethernet or with_etherbone),
             with_vga      = (with_video_terminal or with_video_framebuffer)
         )
 
@@ -112,14 +113,18 @@
             if with_ethernet:
                 self.add_ethernet(phy=self.ethphy, dynamic_ip=eth_dynamic_ip)
             if with_etherbone:
                 self.add_etherbone(phy=self.ethphy, ip_address=eth_ip)
             # The daughterboard has the tx clock wired to a non-clock pin, so we can't help it
             self.platform.add_platform_command("set_property CLOCK_DEDICATED_ROUTE FALSE [get_nets eth_clocks_tx_IBUF]")
 
+        # Jtagbone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
+
         # SPI Flash --------------------------------------------------------------------------------
         if with_spi_flash:
             from litespi.modules import MT25QL128
             from litespi.opcodes import SpiNorFlashOpCodes as Codes
             self.add_spi_flash(mode="4x", module=MT25QL128(Codes.READ_1_1_1), with_master=True)
 
         # Video ------------------------------------------------------------------------------------
@@ -139,26 +144,27 @@
         if not with_daughterboard and kwargs["uart_name"] == "serial":
             kwargs["uart_name"] = "jtag_serial"
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=qmtech_artix7_fgg676.Platform, description="LiteX SoC on QMTech XC7AXXXT.")
-    parser.add_target_argument("--kgates",              default=100,   type=int,  help="Number of kgates. Allowed values: 75, 100, 200, representing XC7A75T, XC7A100T and XC7A200T")
+    parser = LiteXArgumentParser(platform=qmtech_artix7_fbg484.Platform, description="LiteX SoC on QMTech Artix7 FBG484.")
+    parser.add_target_argument("--kgates",              default=200,   type=int,  help="Number of kgates. Allowed values: 75, 100, 200, representing XC7A75T, XC7A100T and XC7A200T")
     parser.add_target_argument("--sys-clk-freq",        default=100e6, type=float,  help="System clock frequency.")
     parser.add_target_argument("--with-daughterboard",  action="store_true",        help="Board plugged into the QMTech daughterboard.")
     ethopts = parser.target_group.add_mutually_exclusive_group()
     ethopts.add_argument("--with-ethernet",        action="store_true",    help="Enable Ethernet support.")
     ethopts.add_argument("--with-etherbone",       action="store_true",    help="Enable Etherbone support.")
     parser.add_target_argument("--eth-ip",         default="192.168.1.50", help="Ethernet/Etherbone IP address.")
     parser.add_target_argument("--eth-dynamic-ip", action="store_true",    help="Enable dynamic Ethernet IP addresses setting.")
     sdopts = parser.target_group.add_mutually_exclusive_group()
     sdopts.add_argument("--with-spi-sdcard",       action="store_true", help="Enable SPI-mode SDCard support.")
     sdopts.add_argument("--with-sdcard",           action="store_true", help="Enable SDCard support.")
+    parser.add_target_argument("--with-jtagbone",  action="store_true", help="Enable Jtagbone support.")
     parser.add_target_argument("--with-spi-flash", action="store_true", help="Enable SPI Flash (MMAPed).")
     viopts = parser.target_group.add_mutually_exclusive_group()
     viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (VGA).")
     viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (VGA).")
     args = parser.parse_args()
 
     soc = BaseSoC(
@@ -166,14 +172,15 @@
         kgates                 = args.kgates,
         sys_clk_freq           = args.sys_clk_freq,
         with_daughterboard     = args.with_daughterboard,
         with_ethernet          = args.with_ethernet,
         with_etherbone         = args.with_etherbone,
         eth_ip                 = args.eth_ip,
         eth_dynamic_ip         = args.eth_dynamic_ip,
+        with_jtagbone          = args.with_jtagbone,
         with_spi_flash         = args.with_spi_flash,
         with_video_terminal    = args.with_video_terminal,
         with_video_framebuffer = args.with_video_framebuffer,
         **parser.soc_argdict
     )
 
     if args.with_spi_sdcard:
```

### Comparing `litex-boards-2023.12/litex_boards/targets/qmtech_ep4ce15_starter_kit.py` & `litex-boards-2023.8/litex_boards/targets/qmtech_ep4ce15_starter_kit.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,31 +57,39 @@
         sdram_clk = ClockSignal("sys2x_ps" if sdram_rate == "1:2" else "sys_ps")
         self.specials += DDROutput(1, 0, platform.request("sdram_clock"), sdram_clk)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
     def __init__(self, sys_clk_freq=50e6,
+        with_jtaguart   = False,
+        with_jtagbone   = False,
         with_led_chaser = True,
         sdram_rate      = "1:1",
         **kwargs):
         platform = qmtech_ep4ce15_starter_kit.Platform()
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq, sdram_rate = sdram_rate)
 
         # SoCCore ----------------------------------------------------------------------------------
-        if kwargs["with_jtagbone"]:
+        if with_jtagbone:
             kwargs["uart_name"] = "crossover"
+        if with_jtaguart:
+            kwargs["uart_name"] = "jtag_uart"
 
         SoCCore.__init__(self, platform, sys_clk_freq,
             ident = "LiteX SoC on QMTECH Cyclone IV Starter Kit",
             **kwargs
         )
 
+        # JTAGbone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
+
         # SDR SDRAM --------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
             sdrphy_cls = HalfRateGENSDRPHY if sdram_rate == "1:2" else GENSDRPHY
             self.sdrphy = sdrphy_cls(platform.request("sdram"), sys_clk_freq)
             self.add_sdram("sdram",
                 phy           = self.sdrphy,
                 module        = W9825G6KH6(sys_clk_freq, sdram_rate),
@@ -99,19 +107,23 @@
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
     parser = LiteXArgumentParser(platform=qmtech_ep4ce15_starter_kit.Platform, description="LiteX SoC on QMTECH EP4CE15")
     parser.add_target_argument("--sys-clk-freq",  default=50e6, type=float, help="System clock frequency.")
     parser.add_target_argument("--sdram-rate",    default="1:1",            help="SDRAM Rate (1:1 Full Rate or 1:2 Half Rate).")
+    parser.add_target_argument("--with-jtaguart", action="store_true",      help="Enable JTAGUart support.")
+    parser.add_target_argument("--with-jtagbone", action="store_true",      help="Enable JTAGbone support.")
     args = parser.parse_args()
 
     soc = BaseSoC(
         sys_clk_freq           = args.sys_clk_freq,
         sdram_rate             = args.sdram_rate,
+        with_jtagbone          = args.with_jtagbone,
+        with_jtaguart          = args.with_jtaguart,
         **parser.soc_argdict
     )
 
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
```

### Comparing `litex-boards-2023.12/litex_boards/targets/qmtech_ep4cex5.py` & `litex-boards-2023.8/litex_boards/targets/qmtech_ep4cex5.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/qmtech_ep4cgx150.py` & `litex-boards-2023.8/litex_boards/targets/qmtech_ep4cgx150.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/qmtech_wukong.py` & `litex-boards-2023.8/litex_boards/targets/qmtech_wukong.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/qmtech_xc7a35t.py` & `litex-boards-2023.8/litex_boards/targets/qmtech_xc7a35t.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         with_ethernet          = False,
         with_etherbone         = False,
         eth_ip                 = "192.168.1.50",
         eth_dynamic_ip         = False,
         with_led_chaser        = True,
         with_video_terminal    = False,
         with_video_framebuffer = False,
+        with_jtagbone          = True,
         with_spi_flash         = False,
         **kwargs):
         platform = qmtech_xc7a35t.Platform(toolchain=toolchain, with_daughterboard=with_daughterboard)
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq,
             with_ethernet = (with_ethernet or with_etherbone),
@@ -112,14 +113,18 @@
             if with_ethernet:
                 self.add_ethernet(phy=self.ethphy, dynamic_ip=eth_dynamic_ip)
             if with_etherbone:
                 self.add_etherbone(phy=self.ethphy, ip_address=eth_ip)
             # The daughterboard has the tx clock wired to a non-clock pin, so we can't help it
             self.platform.add_platform_command("set_property CLOCK_DEDICATED_ROUTE FALSE [get_nets eth_clocks_tx_IBUF]")
 
+        # Jtagbone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
+
         # SPI Flash --------------------------------------------------------------------------------
         if with_spi_flash:
             from litespi.modules import MT25QL128
             from litespi.opcodes import SpiNorFlashOpCodes as Codes
             self.add_spi_flash(mode="4x", module=MT25QL128(Codes.READ_1_1_1), with_master=True)
 
         # Video ------------------------------------------------------------------------------------
@@ -150,28 +155,30 @@
     ethopts.add_argument("--with-ethernet",        action="store_true",    help="Enable Ethernet support.")
     ethopts.add_argument("--with-etherbone",       action="store_true",    help="Enable Etherbone support.")
     parser.add_target_argument("--eth-ip",         default="192.168.1.50", help="Ethernet/Etherbone IP address.")
     parser.add_target_argument("--eth-dynamic-ip", action="store_true",    help="Enable dynamic Ethernet IP addresses setting.")
     sdopts = parser.target_group.add_mutually_exclusive_group()
     sdopts.add_argument("--with-spi-sdcard",       action="store_true", help="Enable SPI-mode SDCard support.")
     sdopts.add_argument("--with-sdcard",           action="store_true", help="Enable SDCard support.")
+    parser.add_target_argument("--with-jtagbone",  action="store_true", help="Enable Jtagbone support.")
     parser.add_target_argument("--with-spi-flash", action="store_true", help="Enable SPI Flash (MMAPed).")
     viopts = parser.target_group.add_mutually_exclusive_group()
     viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (VGA).")
     viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (VGA).")
     args = parser.parse_args()
 
     soc = BaseSoC(
         toolchain              = args.toolchain,
         sys_clk_freq           = args.sys_clk_freq,
         with_daughterboard     = args.with_daughterboard,
         with_ethernet          = args.with_ethernet,
         with_etherbone         = args.with_etherbone,
         eth_ip                 = args.eth_ip,
         eth_dynamic_ip         = args.eth_dynamic_ip,
+        with_jtagbone          = args.with_jtagbone,
         with_spi_flash         = args.with_spi_flash,
         with_video_terminal    = args.with_video_terminal,
         with_video_framebuffer = args.with_video_framebuffer,
         **parser.soc_argdict
     )
 
     if args.with_spi_sdcard:
```

### Comparing `litex-boards-2023.12/litex_boards/targets/qmtech_xc7k325t.py` & `litex-boards-2023.8/litex_boards/targets/qmtech_xc7k325t.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
     def __init__(self, toolchain="vivado", sys_clk_freq=int(100e6), with_daughterboard=False,
                  with_ethernet=False, with_etherbone=False, eth_ip="192.168.1.50", eth_dynamic_ip=False,
                  local_ip="", remote_ip="",
                  with_led_chaser=True, with_video_terminal=False, with_video_framebuffer=False, with_video_colorbars=False,
-                 with_spi_flash=False, **kwargs):
+                 with_jtagbone=True, with_spi_flash=False, **kwargs):
         platform = qmtech_xc7k325t.Platform(toolchain=toolchain, with_daughterboard=with_daughterboard)
 
         # SoCCore ----------------------------------------------------------------------------------
         print(f"{str(kwargs)}")
         if (kwargs["uart_name"] == "serial") and (not with_daughterboard):
             kwargs["uart_name"] = "gpio_serial"
 
@@ -121,14 +121,18 @@
         if remote_ip:
             remote_ip = remote_ip.split(".")
             self.add_constant("REMOTEIP1", int(remote_ip[0]))
             self.add_constant("REMOTEIP2", int(remote_ip[1]))
             self.add_constant("REMOTEIP3", int(remote_ip[2]))
             self.add_constant("REMOTEIP4", int(remote_ip[3]))
 
+        # Jtagbone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
+
         # SPI Flash --------------------------------------------------------------------------------
         if with_spi_flash:
             from litespi.modules import MT25QL128
             from litespi.opcodes import SpiNorFlashOpCodes as Codes
             self.add_spi_flash(mode="4x", module=MT25QL128(Codes.READ_1_1_1), with_master=True)
 
         # Video ------------------------------------------------------------------------------------
@@ -174,14 +178,15 @@
     parser.add_argument("--remote-ip",           default="192.168.1.100",
    help="Remote IP address of TFTP server.")
     parser.add_argument("--local-ip",            default="192.168.1.50",
    help="Local IP address.")
     sdopts = parser.add_mutually_exclusive_group()
     sdopts.add_argument("--with-spi-sdcard",     action="store_true",              help="Enable SPI-mode SDCard support.")
     sdopts.add_argument("--with-sdcard",         action="store_true",              help="Enable SDCard support.")
+    parser.add_argument("--with-jtagbone",       action="store_true",              help="Enable Jtagbone support.")
     parser.add_argument("--with-spi-flash",      action="store_true",              help="Enable SPI Flash (MMAPed).")
     viopts = parser.add_mutually_exclusive_group()
     viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (VGA).")
     viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (VGA).")
     viopts.add_argument("--with-video-colorbars", action="store_true", help="Enable Video Colorbars (VGA).")
     builder_args(parser)
     soc_core_args(parser)
@@ -194,14 +199,15 @@
         with_daughterboard     = args.with_daughterboard,
         with_ethernet          = args.with_ethernet,
         with_etherbone         = args.with_etherbone,
         eth_ip                 = args.eth_ip,
         eth_dynamic_ip         = args.eth_dynamic_ip,
         local_ip               = args.local_ip,
         remote_ip              = args.remote_ip,
+        with_jtagbone          = args.with_jtagbone,
         with_spi_flash         = args.with_spi_flash,
         with_video_terminal    = args.with_video_terminal,
         with_video_framebuffer = args.with_video_framebuffer,
         with_video_colorbars = args.with_video_colorbars,
         **soc_core_argdict(args)
     )
```

### Comparing `litex-boards-2023.12/litex_boards/targets/quicklogic_quickfeather.py` & `litex-boards-2023.8/litex_boards/targets/quicklogic_quickfeather.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/qwertyembedded_beaglewire.py` & `litex-boards-2023.8/litex_boards/targets/qwertyembedded_beaglewire.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/radiona_ulx3s.py` & `litex-boards-2023.8/litex_boards/targets/radiona_ulx3s.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/radiona_ulx4m_ld_v2.py` & `litex-boards-2023.8/litex_boards/targets/radiona_ulx4m_ld_v2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/rcs_arctic_tern_bmc_card.py` & `litex-boards-2023.8/litex_boards/targets/rcs_arctic_tern_bmc_card.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/redpitaya.py` & `litex-boards-2023.8/litex_boards/targets/redpitaya.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/rz_easyfpga.py` & `litex-boards-2023.8/litex_boards/targets/rz_easyfpga.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/saanlima_pipistrello.py` & `litex-boards-2023.8/litex_boards/targets/saanlima_pipistrello.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/scarabhardware_minispartan6.py` & `litex-boards-2023.8/litex_boards/targets/scarabhardware_minispartan6.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/seeedstudio_spartan_edge_accelerator.py` & `litex-boards-2023.8/litex_boards/targets/seeedstudio_spartan_edge_accelerator.py`

 * *Files 12% similar despite different names*

```diff
@@ -60,26 +60,31 @@
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
     
     def __init__(self, sys_clk_freq=100e6,
         with_led_chaser     = True,
+        with_jtagbone       = False,
         with_video_terminal = True,
         with_neopixel       = False,
         **kwargs):
         platform = seeedstudio_spartan_edge_accelerator.Platform()
         platform.add_extension(_serial_io)
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq, with_video_pll=with_video_terminal)
 
         # SoCCore ----------------------------------------------------------------------------------
         SoCCore.__init__(self, platform, sys_clk_freq, ident = "LiteX SoC on Seeedstudio Spartan Edge Accelerator", **kwargs)
 
+        # Jtagbone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
+
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq
             )
 
@@ -99,20 +104,22 @@
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
     parser = LiteXArgumentParser(platform=seeedstudio_spartan_edge_accelerator.Platform, description="LiteX SoC on Spartan Edge Accelerator.")
     parser.add_target_argument("--sys-clk-freq",        default=100e6, type=float, help="System clock frequency.")
+    parser.add_target_argument("--with-jtagbone",       action="store_true",       help="Enable Jtagbone support.")
     parser.add_target_argument("--with-video-terminal", action="store_true",       help="Enable Video Colorbars (HDMI).")
     parser.add_target_argument("--with-neopixel",       action="store_true",       help="Enable onboard 2 Neopixels Leds.")
 
     args = parser.parse_args()
     soc = BaseSoC(
         sys_clk_freq        = args.sys_clk_freq,
+        with_jtagbone       = args.with_jtagbone,
         with_video_terminal = args.with_video_terminal,
         with_neopixel       = args.with_neopixel,
         **parser.soc_argdict
     )
 
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
```

### Comparing `litex-boards-2023.12/litex_boards/targets/siglent_sds1104xe.py` & `litex-boards-2023.8/litex_boards/targets/sipeed_tang_nano_9k.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,165 +1,173 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2022 Icenowy Zheng <icenowy@aosc.io>
 # SPDX-License-Identifier: BSD-2-Clause
 
-# Build/Use ----------------------------------------------------------------------------------------
-# Build/Load bitstream:
-# ./siglent_sds1104xe.py --with-etherbone --uart-name=crossover --csr-csv=csr.csv --build --load
-#
-# Test Ethernet:
-# ping 192.168.1.50
-#
-# Test Console:
-# litex_server --udp
-# litex_term crossover
-# --------------------------------------------------------------------------------------------------
-
+import os
 from migen import *
 
 from litex.gen import *
 
-from litex_boards.platforms import siglent_sds1104xe
+from litex_boards.platforms import sipeed_tang_nano_9k
 
-from litex.soc.cores.clock import *
+from litex.soc.cores.clock.gowin_gw1n import GW1NPLL
 from litex.soc.integration.soc_core import *
+from litex.soc.integration.soc import SoCRegion
 from litex.soc.integration.builder import *
-from litex.soc.cores.video import VideoVGAPHY
+from litex.soc.cores.led import LedChaser
+from litex.soc.cores.video import *
 
-from litedram.common import PHYPadsReducer
-from litedram.modules import MT41K64M16
-from litedram.phy import s7ddrphy
+from litex.soc.cores.hyperbus import HyperRAM
 
-from liteeth.phy.mii import LiteEthPHYMII
+kB = 1024
+mB = 1024*kB
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq, with_ethernet=False):
-        self.rst          = Signal()
-        self.cd_sys       = ClockDomain()
-        self.cd_sys4x     = ClockDomain()
-        self.cd_sys4x_dqs = ClockDomain()
-        self.cd_idelay    = ClockDomain()
-        self.cd_dvi       = ClockDomain()
+    def __init__(self, platform, sys_clk_freq, with_video_pll=False):
+        self.rst    = Signal()
+        self.cd_sys = ClockDomain()
 
         # # #
 
         # Clk / Rst
-        clk25 = ClockSignal("eth_tx") if with_ethernet else platform.request("eth_clocks").rx
+        clk27 = platform.request("clk27")
+        rst_n = platform.request("user_btn", 0)
 
         # PLL
-        self.pll = pll = S7PLL(speedgrade=-1)
-        pll.register_clkin(clk25, 25e6)
-        pll.create_clkout(self.cd_sys,       sys_clk_freq)
-        pll.create_clkout(self.cd_sys4x,     4*sys_clk_freq)
-        pll.create_clkout(self.cd_sys4x_dqs, 4*sys_clk_freq, phase=90)
-        pll.create_clkout(self.cd_idelay,    200e6)
-        pll.create_clkout(self.cd_dvi,       33.3e6)
-        platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
-
-        self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
+        self.pll = pll = GW1NPLL(devicename=platform.devicename, device=platform.device)
+        self.comb += pll.reset.eq(~rst_n)
+        pll.register_clkin(clk27, 27e6)
+        pll.create_clkout(self.cd_sys, sys_clk_freq)
+
+        # Video PLL
+        if with_video_pll:
+            self.video_pll = video_pll = GW1NPLL(devicename=platform.devicename, device=platform.device)
+            self.comb += video_pll.reset.eq(~rst_n)
+            video_pll.register_clkin(clk27, 27e6)
+            self.cd_hdmi   = ClockDomain()
+            self.cd_hdmi5x = ClockDomain()
+            video_pll.create_clkout(self.cd_hdmi5x, 125e6)
+            self.specials += Instance("CLKDIV",
+                p_DIV_MODE= "5",
+                i_RESETN = rst_n,
+                i_HCLKIN = self.cd_hdmi5x.clk,
+                o_CLKOUT = self.cd_hdmi.clk
+            )
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=100e6,
-        with_etherbone         = True,
-        eth_ip                 = "192.168.1.50",
-        with_video_terminal    = False,
-        with_video_framebuffer = False,
+    def __init__(self, sys_clk_freq=27e6, bios_flash_offset=0x0,
+        with_led_chaser     = True,
+        with_video_terminal = False,
         **kwargs):
-        platform = siglent_sds1104xe.Platform()
+        platform = sipeed_tang_nano_9k.Platform()
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = _CRG(platform, sys_clk_freq, with_ethernet=with_etherbone)
+        self.crg = _CRG(platform, sys_clk_freq, with_video_pll=with_video_terminal)
 
         # SoCCore ----------------------------------------------------------------------------------
-        if kwargs.get("uart_name", "serial") == "serial":
-            kwargs["uart_name"] = "crossover" # Defaults to Crossover UART.
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Siglent SDS1104X-E", **kwargs)
+        # Disable Integrated ROM
+        kwargs["integrated_rom_size"] = 0
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Tang Nano 9K", **kwargs)
+
+        # SPI Flash --------------------------------------------------------------------------------
+        from litespi.modules import W25Q32
+        from litespi.opcodes import SpiNorFlashOpCodes as Codes
+        self.add_spi_flash(mode="1x", module=W25Q32(Codes.READ_1_1_1), with_master=False)
+
+        # Add ROM linker region --------------------------------------------------------------------
+        self.bus.add_region("rom", SoCRegion(
+            origin = self.bus.regions["spiflash"].origin + bios_flash_offset,
+            size   = 64*kB,
+            linker = True)
+        )
+        self.cpu.set_reset_address(self.bus.regions["rom"].origin)
 
-        # DDR3 SDRAM -------------------------------------------------------------------------------
+        # HyperRAM ---------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
-            self.ddrphy = s7ddrphy.A7DDRPHY(
-                pads           = PHYPadsReducer(platform.request("ddram"), [0, 1, 2, 3]),
-                memtype        = "DDR3",
-                nphases        = 4,
-                sys_clk_freq   = sys_clk_freq)
-            self.add_sdram("sdram",
-                phy           = self.ddrphy,
-                module        = MT41K64M16(sys_clk_freq, "1:4"),
-                l2_cache_size = kwargs.get("l2_size", 8192)
-            )
+            # TODO: Use second 32Mbit PSRAM chip.
+            dq      = platform.request("IO_psram_dq")
+            rwds    = platform.request("IO_psram_rwds")
+            reset_n = platform.request("O_psram_reset_n")
+            cs_n    = platform.request("O_psram_cs_n")
+            ck      = platform.request("O_psram_ck")
+            ck_n    = platform.request("O_psram_ck_n")
+            class HyperRAMPads:
+                def __init__(self, n):
+                    self.clk   = Signal()
+                    self.rst_n = reset_n[n]
+                    self.dq    = dq[8*n:8*(n+1)]
+                    self.cs_n  = cs_n[n]
+                    self.rwds  = rwds[n]
+
+            hyperram_pads = HyperRAMPads(0)
+            self.comb += ck[0].eq(hyperram_pads.clk)
+            self.comb += ck_n[0].eq(~hyperram_pads.clk)
+            # FIXME: Issue with upstream HyperRAM core, so use old one. Need to investigate.
+            if not os.path.exists("hyperbus.py"):
+                os.system("wget https://github.com/litex-hub/litex-boards/files/8831568/hyperbus.py.txt")
+                os.system("mv hyperbus.py.txt hyperbus.py")
+            from hyperbus import HyperRAM
+            self.hyperram = HyperRAM(hyperram_pads)
+            self.bus.add_slave("main_ram", slave=self.hyperram.bus, region=SoCRegion(origin=self.mem_map["main_ram"], size=4*mB))
 
-        # Etherbone + Ethernet ---------------------------------------------------------------------
-        if with_etherbone:
-            # Ethernet PHY
-            self.ethphy = LiteEthPHYMII(
-                clock_pads = self.platform.request("eth_clocks"),
-                pads       = self.platform.request("eth"),
-            )
+        # Video ------------------------------------------------------------------------------------
+        if with_video_terminal:
+            self.videophy = VideoGowinHDMIPHY(platform.request("hdmi"), clock_domain="hdmi")
+            self.add_video_colorbars(phy=self.videophy, timings="640x480@60Hz", clock_domain="hdmi")
+            #self.add_video_terminal(phy=self.videophy, timings="640x480@75Hz", clock_domain="hdmi") # FIXME: Free up BRAMs.
 
-            # Etherbone.
-            self.add_etherbone(
-                phy         = self.ethphy,
-                ip_address  = "192.168.1.51",
-                mac_address = 0x10e2d5000001,
-                data_width  = 8,
-                with_ethmac = True,
-            )
 
-        # Video ------------------------------------------------------------------------------------
-        video_timings = ("800x480@60Hz", {
-            "pix_clk"       : 33.3e6,
-            "h_active"      : 800,
-            "h_blanking"    : 256,
-            "h_sync_offset" : 210,
-            "h_sync_width"  : 1,
-            "v_active"      : 480,
-            "v_blanking"    : 45,
-            "v_sync_offset" : 22,
-            "v_sync_width"  : 1,
-        })
-        if with_video_terminal or with_video_framebuffer:
-            self.videophy = VideoVGAPHY(platform.request("lcd"), clock_domain="dvi")
-            if with_video_terminal:
-                self.add_video_terminal(phy=self.videophy, timings=video_timings, clock_domain="dvi")
-            if with_video_framebuffer:
-                self.add_video_framebuffer(phy=self.videophy, timings=video_timings, clock_domain="dvi")
+        # Leds -------------------------------------------------------------------------------------
+        if with_led_chaser:
+            self.leds = LedChaser(
+                pads         = platform.request_all("user_led"),
+                sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=siglent_sds1104xe.Platform, description="LiteX SoC on SDS1104X-E.")
-    parser.add_target_argument("--sys-clk-freq",   default=100e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--with-etherbone", action="store_true",       help="Enable Etherbone support.")
-    parser.add_target_argument("--eth-ip",         default="192.168.1.50",     help="Ethernet/Etherbone IP address.")
-    viopts = parser.target_group.add_mutually_exclusive_group()
-    viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (HDMI).")
-    viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (HDMI).")
+    parser = LiteXArgumentParser(platform=sipeed_tang_nano_9k.Platform, description="LiteX SoC on Tang Nano 9K.")
+    parser.add_target_argument("--flash",                action="store_true",      help="Flash Bitstream.")
+    parser.add_target_argument("--sys-clk-freq",         default=27e6, type=float, help="System clock frequency.")
+    parser.add_target_argument("--bios-flash-offset",    default="0x0",            help="BIOS offset in SPI Flash.")
+    parser.add_target_argument("--with-spi-sdcard",      action="store_true",      help="Enable SPI-mode SDCard support.")
+    parser.add_target_argument("--with-video-terminal",  action="store_true",      help="Enable Video Terminal (HDMI).")
+    parser.add_target_argument("--prog-kit",             default="openfpgaloader", help="Programmer select from Gowin/openFPGALoader.")
     args = parser.parse_args()
 
     soc = BaseSoC(
-        sys_clk_freq   = args.sys_clk_freq,
-        with_etherbone = args.with_etherbone,
-        eth_ip         = args.eth_ip,
-        with_video_terminal    = args.with_video_terminal,
-        with_video_framebuffer = args.with_video_framebuffer,
+        sys_clk_freq        = args.sys_clk_freq,
+        bios_flash_offset   = int(args.bios_flash_offset, 0),
+        with_video_terminal = args.with_video_terminal,
         **parser.soc_argdict
     )
 
+    if args.with_spi_sdcard:
+        soc.add_spi_sdcard()
+
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
     if args.load:
-        prog = soc.platform.create_programmer()
-        prog.load_bitstream(builder.get_bitstream_filename(mode="sram"), device=1)
+        prog = soc.platform.create_programmer(kit=args.prog_kit)
+        prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
+
+    if args.flash:
+        prog = soc.platform.create_programmer(kit=args.prog_kit)
+        prog.flash(0, builder.get_bitstream_filename(mode="flash", ext=".fs")) # FIXME
+        # Axternal SPI programming not supported by gowin 'programmer_cli' now!
+        # if needed, use openFPGALoader or Gowin programmer GUI
+        if args.prog_kit == "openfpgaloader":
+            prog.flash(int(args.bios_flash_offset, 0), builder.get_bios_filename(), external=True)
 
 if __name__ == "__main__":
     main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/simple.py` & `litex-boards-2023.8/litex_boards/targets/simple.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/sipeed_tang_mega_138k.py` & `litex-boards-2023.8/litex_boards/targets/sipeed_tang_primer_20k.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,252 +1,231 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2022-2023 Icenowy Zheng <uwu@icenowy.me>
+# Copyright (c) 2022 Icenowy Zheng <icenowy@aosc.io>
 # Copyright (c) 2022 Florent Kermarrec <florent@enjoy-digital.fr>
-# Copyright (c) 2023 Gwenhael Goavec-Merou <gwenhael@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex.soc.cores.clock.gowin_gw5a import GW5APLL
+from litex.soc.cores.clock.gowin_gw2a import GW2APLL
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.soc import SoCRegion
 from litex.soc.integration.builder import *
 from litex.soc.cores.led import LedChaser, WS2812
+from litex.soc.cores.gpio import GPIOIn
 from litex.soc.cores.video import *
 
-from liteeth.phy.gw5rgmii import LiteEthPHYRGMII
+from liteeth.phy.rmii import LiteEthPHYRMII
 
-from litedram.modules import AS4C32M16, MT41J256M16
-from litedram.phy import GENSDRPHY, HalfRateGENSDRPHY
-from litedram.phy import GW5DDRPHY
-from litex.build.io import DDROutput
+from litex_boards.platforms import sipeed_tang_primer_20k
 
-from litex_boards.platforms import sipeed_tang_mega_138k
+from litedram.common import PHYPadsReducer
+from litedram.modules import MT41K64M16
+from litedram.phy import GW2DDRPHY
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq, with_sdram=False, sdram_rate="1:2", with_ddr3=False, with_video_pll=False):
-        self.rst      = Signal()
-        self.cd_sys   = ClockDomain()
-        self.cd_por   = ClockDomain()
-        if with_sdram:
-            if sdram_rate == "1:2":
-                self.cd_sys2x    = ClockDomain()
-                self.cd_sys2x_ps = ClockDomain()
-            else:
-                self.cd_sys_ps = ClockDomain()
-
-        if with_ddr3:
-            self.cd_init    = ClockDomain()
-            self.cd_sys2x   = ClockDomain()
-            self.cd_sys2x_i = ClockDomain()
-            self.stop       = Signal()
-            self.reset      = Signal()
+    def __init__(self, platform, sys_clk_freq, with_video_pll=False):
+        self.rst        = Signal()
+        self.cd_sys     = ClockDomain()
+        self.cd_por     = ClockDomain()
+        self.cd_init    = ClockDomain()
+        self.cd_sys2x   = ClockDomain()
+        self.cd_sys2x_i = ClockDomain()
+
+        # # #
+
+        self.stop  = Signal()
+        self.reset = Signal()
 
         # Clk
-        self.clk50 = platform.request("clk50")
-        rst = platform.request("rst")
+        clk27 = platform.request("clk27")
 
-        # Power on reset
+        # Power on reset (the onboard POR is not aware of reprogramming)
         por_count = Signal(16, reset=2**16-1)
         por_done  = Signal()
-        self.comb += self.cd_por.clk.eq(self.clk50)
+        self.comb += self.cd_por.clk.eq(clk27)
         self.comb += por_done.eq(por_count == 0)
         self.sync.por += If(~por_done, por_count.eq(por_count - 1))
 
         # PLL
-        self.pll = pll = GW5APLL(devicename=platform.devicename, device=platform.device)
-        self.comb += pll.reset.eq(~por_done | self.rst | rst)
-        pll.register_clkin(self.clk50, 50e6)
-        pll.create_clkout(self.cd_sys, sys_clk_freq, with_reset=not with_ddr3)
-
-        # SDRAM clock
-        if with_sdram:
-            if sdram_rate == "1:2":
-                pll.create_clkout(self.cd_sys2x,    2*sys_clk_freq)
-                pll.create_clkout(self.cd_sys2x_ps, 2*sys_clk_freq, phase=180)
-                sdram_clk = ClockSignal("sys2x_ps")
-            else:
-                pll.create_clkout(self.cd_sys_ps, sys_clk_freq, phase=90)
-                sdram_clk = ClockSignal("sys_ps")
-            self.specials += DDROutput(1, 0, platform.request("sdram_clock"), sdram_clk)
-
-        # DDR3 clock
-        if with_ddr3:
-            pll.create_clkout(self.cd_sys2x_i, 2*sys_clk_freq)
-            self.specials += [
-                Instance("DHCE",
-                    i_CLKIN  = self.cd_sys2x_i.clk,
-                    i_CEN    = self.stop,
-                    o_CLKOUT = self.cd_sys2x.clk
-                ),
-                AsyncResetSynchronizer(self.cd_sys, ~pll.locked | self.rst | self.reset),
-            ]
-            # Init clock domain
-            self.comb += self.cd_init.clk.eq(self.clk50)
-            self.comb += self.cd_init.rst.eq(pll.reset)
+        self.pll = pll = GW2APLL(devicename=platform.devicename, device=platform.device)
+        self.comb += pll.reset.eq(~por_done)
+        pll.register_clkin(clk27, 27e6)
+        pll.create_clkout(self.cd_sys2x_i, 2*sys_clk_freq)
+        self.specials += [
+            Instance("DHCEN",
+                i_CLKIN  = self.cd_sys2x_i.clk,
+                i_CE     = self.stop,
+                o_CLKOUT = self.cd_sys2x.clk),
+            Instance("CLKDIV",
+                p_DIV_MODE = "2",
+                i_CALIB    = 0,
+                i_HCLKIN   = self.cd_sys2x.clk,
+                i_RESETN   = ~self.reset,
+                o_CLKOUT   = self.cd_sys.clk),
+            AsyncResetSynchronizer(self.cd_sys, ~pll.locked | self.rst | self.reset),
+        ]
+
+        # Init clock domain
+        self.comb += self.cd_init.clk.eq(clk27)
+        self.comb += self.cd_init.rst.eq(pll.reset)
 
+        # Video PLL
         if with_video_pll:
+            self.video_pll = video_pll = GW2APLL(devicename=platform.devicename, device=platform.device)
+            video_pll.register_clkin(clk27, 27e6)
             self.cd_hdmi   = ClockDomain()
             self.cd_hdmi5x = ClockDomain()
-            pll.create_clkout(self.cd_hdmi5x, 125e6, margin=1e-3)
+            video_pll.create_clkout(self.cd_hdmi5x, 125e6, margin=1e-3)
             self.specials += Instance("CLKDIV",
                 p_DIV_MODE = "5",
-                i_HCLKIN   = self.cd_hdmi5x.clk,
                 i_RESETN   = 1, # Disable reset signal.
                 i_CALIB    = 0, # No calibration.
+                i_HCLKIN   = self.cd_hdmi5x.clk,
                 o_CLKOUT   = self.cd_hdmi.clk
             )
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=50e6,
-        with_ethernet       = True,
-        with_etherbone      = False,
-        local_ip            = "192.168.1.50",
-        remote_ip           = "",
-        eth_dynamic_ip      = False,
-        with_video_terminal = False,
-        with_ddr3           = False,
-        with_sdram          = False,
-        sdram_rate          = "1:2",
+    def __init__(self, sys_clk_freq=48e6,
+        with_spi_flash      = False,
         with_led_chaser     = True,
         with_rgb_led        = False,
         with_buttons        = True,
+        with_video_terminal = False,
+        with_ethernet       = False,
+        with_etherbone      = False,
+        eth_ip              = "192.168.1.50",
+        eth_dynamic_ip      = False,
+        dock                = "standard",
         **kwargs):
 
-        platform = sipeed_tang_mega_138k.Platform(toolchain="gowin")
+        assert dock in ["standard", "lite"]
+
+        platform = sipeed_tang_primer_20k.Platform(dock, toolchain="gowin")
+
+        if dock == "lite":
+            with_led_chaser = False # No leds on core board nor on dock lite.
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = _CRG(platform, sys_clk_freq,
-            with_sdram     = with_sdram,
-            with_ddr3      = with_ddr3,
-            with_video_pll = with_video_terminal)
+        self.crg = _CRG(platform, sys_clk_freq, with_video_pll=with_video_terminal)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Tang Mega 138K", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Tang Primer 20K", **kwargs)
 
         # DDR3 SDRAM -------------------------------------------------------------------------------
-        if with_ddr3 and not self.integrated_main_ram_size:
-            self.ddrphy = GW5DDRPHY(
+        if not self.integrated_main_ram_size:
+            self.ddrphy = GW2DDRPHY(
                 pads         = platform.request("ddram"),
                 sys_clk_freq = sys_clk_freq
             )
             self.ddrphy.settings.rtt_nom = "disabled"
             self.comb += self.crg.stop.eq(self.ddrphy.init.stop)
             self.comb += self.crg.reset.eq(self.ddrphy.init.reset)
             self.add_sdram("sdram",
                 phy           = self.ddrphy,
-                module        = MT41J256M16(sys_clk_freq, "1:2"),
-                l2_cache_size = 0#kwargs.get("l2_size", 8192)
+                module        = MT41K64M16(sys_clk_freq, "1:2"),
+                l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
+        # SPI Flash --------------------------------------------------------------------------------
+        if with_spi_flash:
+            from litespi.modules import W25Q32JV as SpiFlashModule
+            from litespi.opcodes import SpiNorFlashOpCodes as Codes
+            self.add_spi_flash(mode="1x", module=SpiFlashModule(Codes.READ_1_1_1))
+
+        # Ethernet / Etherbone ---------------------------------------------------------------------
+        if with_ethernet or with_etherbone:
+            from liteeth.phy.rmii import LiteEthPHYRMII
+            self.ethphy = LiteEthPHYRMII(
+                clock_pads = self.platform.request("eth_clocks"),
+                pads       = self.platform.request("eth"),
+                refclk_cd  = None
+            )
+            if with_ethernet:
+                self.add_ethernet(phy=self.ethphy, dynamic_ip=eth_dynamic_ip, with_timing_constraints=False)
+            if with_etherbone:
+                self.add_etherbone(phy=self.ethphy, ip_address=eth_ip, with_timing_constraints=False)
+
         # Video ------------------------------------------------------------------------------------
         if with_video_terminal:
-            hdmi_pads = platform.request("hdmi_in") # yes DVI_RX because DVI_TX seems not working
+            hdmi_pads = platform.request("hdmi")
             self.comb += hdmi_pads.hdp.eq(1)
-            self.videophy = VideoGowinHDMIPHY(hdmi_pads, clock_domain="hdmi")
+            self.videophy = VideoHDMIPHY(hdmi_pads, clock_domain="hdmi")
             #self.add_video_colorbars(phy=self.videophy, timings="640x480@60Hz", clock_domain="hdmi")
             self.add_video_terminal(phy=self.videophy, timings="640x480@75Hz", clock_domain="hdmi")
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
-                pads         = platform.request_all("led_n"),
+                pads         = platform.request_all("led"),
                 sys_clk_freq = sys_clk_freq
             )
 
-        # Ethernet / Etherbone ---------------------------------------------------------------------
-        if with_ethernet or with_etherbone:
-            self.ethphy = LiteEthPHYRGMII(
-                clock_pads = self.platform.request("eth_clocks"),
-                pads       = self.platform.request("eth"),
-                tx_delay   = 2e-9,
-                rx_delay   = 2e-9)
-            self.clk50_half = Signal()
-            self.specials += Instance("CLKDIV",
-                p_DIV_MODE = "2",
-                i_HCLKIN   = self.crg.clk50,
-                i_RESETN   = 1,
-                i_CALIB    = 0,
-                o_CLKOUT   = self.clk50_half)
-            self.specials += DDROutput(1, 0, platform.request("ephy_clk"), self.clk50_half)
-            if with_ethernet:
-                self.add_ethernet(phy=self.ethphy, dynamic_ip=eth_dynamic_ip, data_width=32, software_debug=True)
-            if with_etherbone:
-                self.add_etherbone(phy=self.ethphy, data_width=32)
-
-        if local_ip:
-            local_ip = local_ip.split(".")
-            self.add_constant("LOCALIP1", int(local_ip[0]))
-            self.add_constant("LOCALIP2", int(local_ip[1]))
-            self.add_constant("LOCALIP3", int(local_ip[2]))
-            self.add_constant("LOCALIP4", int(local_ip[3]))
-
-        if remote_ip:
-            remote_ip = remote_ip.split(".")
-            self.add_constant("REMOTEIP1", int(remote_ip[0]))
-            self.add_constant("REMOTEIP2", int(remote_ip[1]))
-            self.add_constant("REMOTEIP3", int(remote_ip[2]))
-            self.add_constant("REMOTEIP4", int(remote_ip[3]))
-
-        # SDR SDRAM --------------------------------------------------------------------------------
-        if with_sdram and not self.integrated_main_ram_size:
-            if sdram_rate == "1:2":
-                sdrphy_cls = HalfRateGENSDRPHY
-            else:
-                sdrphy_cls = GENSDRPHY
-            self.sdrphy = sdrphy_cls(platform.request("sdram"), sys_clk_freq)
-            self.add_sdram("sdram",
-                phy           = self.sdrphy,
-                module        = AS4C32M16(sys_clk_freq, sdram_rate),
-                l2_cache_size = kwargs.get("l2_size", 8192)
+        # RGB Led ----------------------------------------------------------------------------------
+        if with_rgb_led:
+            self.rgb_led = WS2812(
+                pad          = platform.request("rgb_led"),
+                nleds        = 1,
+                sys_clk_freq = sys_clk_freq
             )
+            self.bus.add_slave(name="rgb_led", slave=self.rgb_led.bus, region=SoCRegion(
+                origin = 0x2000_0000,
+                size   = 4,
+            ))
+
+        # Buttons ----------------------------------------------------------------------------------
+        if with_buttons:
+            self.buttons = GPIOIn(pads=~platform.request_all("btn_n"))
+
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=sipeed_tang_mega_138k.Platform, description="LiteX SoC on Tang Mega 138K.")
-    parser.add_target_argument("--flash",           action="store_true",      help="Flash Bitstream.")
-    parser.add_target_argument("--sys-clk-freq",    default=50e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--with-sdram",      action="store_true",      help="Enable optional SDRAM module.")
-    parser.add_target_argument("--with-ddr3",       action="store_true",      help="Enable optional DDR3 module.")
-    parser.add_target_argument("--with-video-terminal", action="store_true",  help="Enable Video Terminal (HDMI).")
+    parser = LiteXArgumentParser(platform=sipeed_tang_primer_20k.Platform, description="LiteX SoC on Tang Primer 20K.")
+    parser.add_target_argument("--dock",         default="standard",       help="Dock version (standard (default) or lite.")
+    parser.add_target_argument("--flash",        action="store_true",      help="Flash Bitstream.")
+    parser.add_target_argument("--sys-clk-freq", default=48e6, type=float, help="System clock frequency.")
+    sdopts = parser.target_group.add_mutually_exclusive_group()
+    sdopts.add_argument("--with-spi-sdcard",            action="store_true", help="Enable SPI-mode SDCard support.")
+    sdopts.add_argument("--with-sdcard",                action="store_true", help="Enable SDCard support.")
+    parser.add_target_argument("--with-spi-flash",      action="store_true", help="Enable SPI Flash (MMAPed).")
+    parser.add_target_argument("--with-video-terminal", action="store_true", help="Enable Video Terminal (HDMI).")
     ethopts = parser.target_group.add_mutually_exclusive_group()
-    ethopts.add_argument("--with-ethernet",         action="store_true",      help="Enable Ethernet support.")
-    ethopts.add_argument("--with-etherbone",        action="store_true",      help="Enable Etherbone support.")
-    parser.add_target_argument("--eth-dynamic-ip",  action="store_true",      help="Enable dynamic Ethernet IP addresses setting.")
-    parser.add_target_argument("--remote-ip",       default="192.168.1.100",  help="Remote IP address of TFTP server.")
-    parser.add_target_argument("--local-ip",        default="192.168.1.50",   help="Local IP address.")
+    ethopts.add_argument("--with-ethernet",         action="store_true",    help="Add Ethernet.")
+    ethopts.add_argument("--with-etherbone",        action="store_true",    help="Add EtherBone.")
+    parser.add_target_argument("--eth-ip",          default="192.168.1.50", help="Etherbone IP address.")
+    parser.add_target_argument("--eth-dynamic-ip",  action="store_true",    help="Enable dynamic Ethernet IP addresses setting.")
     args = parser.parse_args()
 
-    assert not (args.with_etherbone and args.eth_dynamic_ip)
-
     soc = BaseSoC(
         sys_clk_freq        = args.sys_clk_freq,
+        with_spi_flash      = args.with_spi_flash,
         with_video_terminal = args.with_video_terminal,
-        with_ddr3           = args.with_ddr3,
-        with_sdram          = args.with_sdram,
         with_ethernet       = args.with_ethernet,
         with_etherbone      = args.with_etherbone,
-        local_ip            = args.local_ip,
-        remote_ip           = args.remote_ip,
+        eth_ip              = args.eth_ip,
         eth_dynamic_ip      = args.eth_dynamic_ip,
+        dock                = args.dock,
         **parser.soc_argdict
     )
+    if args.with_spi_sdcard:
+        soc.add_spi_sdcard()
+    if args.with_sdcard:
+        soc.add_sdcard()
 
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
     if args.load:
         prog = soc.platform.create_programmer()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `litex-boards-2023.12/litex_boards/targets/sipeed_tang_nano.py` & `litex-boards-2023.8/litex_boards/targets/sipeed_tang_nano.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,19 +65,20 @@
     def __init__(self, sys_clk_freq=48e6, with_led_chaser=True, **kwargs):
         platform = sipeed_tang_nano.Platform()
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCMini ----------------------------------------------------------------------------------
-        kwargs["uart_name"]     = "crossover"
-        kwargs["uart_baudrate"] = 1e6 # CH552 firmware does not support traditional baudrates.
-        kwargs["with_uartbone"] = True
+        kwargs["uart_name"] = "crossover"
         SoCMini.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Tang Nano", **kwargs)
 
+        # UARTBone ---------------------------------------------------------------------------------
+        self.add_uartbone(baudrate=int(1e6)) # CH552 firmware does not support traditional baudrates.
+
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
```

### Comparing `litex-boards-2023.12/litex_boards/targets/sipeed_tang_nano_20k.py` & `litex-boards-2023.8/litex_boards/targets/sipeed_tang_nano_20k.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             self.buttons = GPIOIn(pads=~platform.request_all("btn"))
 
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=sipeed_tang_nano_20k.Platform, description="LiteX SoC on Tang Nano 20K.")
+    parser = LiteXArgumentParser(platform=sipeed_tang_nano_20k.Platform, description="LiteX SoC on Tang Primer 20K.")
     parser.add_target_argument("--flash",        action="store_true",      help="Flash Bitstream.")
     parser.add_target_argument("--sys-clk-freq", default=48e6, type=float, help="System clock frequency.")
     sdopts = parser.target_group.add_mutually_exclusive_group()
     sdopts.add_argument("--with-spi-sdcard",            action="store_true", help="Enable SPI-mode SDCard support.")
     sdopts.add_argument("--with-sdcard",                action="store_true", help="Enable SDCard support.")
     args = parser.parse_args()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/sipeed_tang_nano_4k.py` & `litex-boards-2023.8/litex_boards/targets/sipeed_tang_nano_4k.py`

 * *Files 6% similar despite different names*

```diff
@@ -161,24 +161,12 @@
     if args.load:
         prog = soc.platform.create_programmer()
         prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
 
     if args.flash:
         prog = soc.platform.create_programmer()
         prog.flash(0, builder.get_bitstream_filename(mode="flash", ext=".fs")) # FIXME
-        if args.cpu_type != "gowin_emcu":
-            prog.flash(0, builder.get_bios_filename(), external=True)
-
-    if args.cpu_type == "gowin_emcu":
-        import time
-        bios_filename = builder.get_bios_filename()
-        msg = "\n"
-        msg += "Gowin EMCU firmware must be written in flash with:\n"
-        msg += f"openFPGALoader -b tangnano4k --mcufw {bios_filename}\n"
-        msg += "Warning: this will erase ALL the internal flash"
-        msg += "\n"
-        print(msg)
-        time.sleep(2)
+        prog.flash(0, builder.get_bios_filename(), external=True)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/sipeed_tang_nano_9k.py` & `litex-boards-2023.8/litex_boards/targets/sitlinv_xc7k420t.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,173 +1,169 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2022 Icenowy Zheng <icenowy@aosc.io>
+# Copyright (c) 2022 Andrew Gillham <gillham@roadsign.com>
+# Copyright (c) 2014-2015 Sebastien Bourdeauducq <sb@m-labs.hk>
+# Copyright (c) 2014-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2014-2015 Yann Sionneau <ys@m-labs.hk>
+# Copyright (c) 2020 Hans Baier <hansfbaier@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
+# Board support for this chinese Kintex 420T board by "SITLINV FPGA Board Store"
+# https://www.aliexpress.com/item/1005001631827738.html
+
 import os
+
 from migen import *
 
 from litex.gen import *
 
-from litex_boards.platforms import sipeed_tang_nano_9k
+from litex_boards.platforms import sitlinv_xc7k420t
 
-from litex.soc.cores.clock.gowin_gw1n import GW1NPLL
+from litex.soc.cores.clock import *
 from litex.soc.integration.soc_core import *
-from litex.soc.integration.soc import SoCRegion
 from litex.soc.integration.builder import *
 from litex.soc.cores.led import LedChaser
-from litex.soc.cores.video import *
+from litex.soc.cores.bitbang import I2CMaster
 
-from litex.soc.cores.hyperbus import HyperRAM
+from litedram.phy import s7ddrphy
+from litedram.common import PHYPadsReducer
+from litedram.modules import K4B1G0446F
 
-kB = 1024
-mB = 1024*kB
+from litepcie.phy.s7pciephy import S7PCIEPHY
+from litepcie.software import generate_litepcie_software
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq, with_video_pll=False):
-        self.rst    = Signal()
-        self.cd_sys = ClockDomain()
+    def __init__(self, platform, sys_clk_freq):
+        self.rst          = Signal()
+        self.cd_sys       = ClockDomain()
+        self.cd_sys4x     = ClockDomain()
+        self.cd_sys4x_dqs = ClockDomain()
+        self.cd_idelay    = ClockDomain()
 
         # # #
 
-        # Clk / Rst
-        clk27 = platform.request("clk27")
-        rst_n = platform.request("user_btn", 0)
-
-        # PLL
-        self.pll = pll = GW1NPLL(devicename=platform.devicename, device=platform.device)
-        self.comb += pll.reset.eq(~rst_n)
-        pll.register_clkin(clk27, 27e6)
-        pll.create_clkout(self.cd_sys, sys_clk_freq)
-
-        # Video PLL
-        if with_video_pll:
-            self.video_pll = video_pll = GW1NPLL(devicename=platform.devicename, device=platform.device)
-            self.comb += video_pll.reset.eq(~rst_n)
-            video_pll.register_clkin(clk27, 27e6)
-            self.cd_hdmi   = ClockDomain()
-            self.cd_hdmi5x = ClockDomain()
-            video_pll.create_clkout(self.cd_hdmi5x, 125e6)
-            self.specials += Instance("CLKDIV",
-                p_DIV_MODE= "5",
-                i_RESETN = rst_n,
-                i_HCLKIN = self.cd_hdmi5x.clk,
-                o_CLKOUT = self.cd_hdmi.clk
-            )
+        # Clk/Rst.
+        clk100 = platform.request("clk100")
+        rst_n  = platform.request("cpu_reset_n")
+
+        # PLL.
+        self.pll = pll = S7PLL(speedgrade=-2)
+        self.comb += pll.reset.eq(~rst_n | self.rst)
+        pll.register_clkin(clk100, 100e6)
+        pll.create_clkout(self.cd_sys,       sys_clk_freq)
+        pll.create_clkout(self.cd_sys4x,     4*sys_clk_freq)
+        pll.create_clkout(self.cd_sys4x_dqs, 4*sys_clk_freq, phase=120)
+        pll.create_clkout(self.cd_idelay,    200e6)
+        platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
+
+        self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=27e6, bios_flash_offset=0x0,
-        with_led_chaser     = True,
-        with_video_terminal = False,
+    def __init__(self, sys_clk_freq=100e6,
+        io_voltage      = "3.3V",
+        with_led_chaser = True,
+        with_pcie       = False,
+        with_sata       = False,
         **kwargs):
-        platform = sipeed_tang_nano_9k.Platform()
+        platform = sitlinv_xc7k420t.Platform(io_voltage)
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = _CRG(platform, sys_clk_freq, with_video_pll=with_video_terminal)
+        self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        # Disable Integrated ROM
-        kwargs["integrated_rom_size"] = 0
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Tang Nano 9K", **kwargs)
-
-        # SPI Flash --------------------------------------------------------------------------------
-        from litespi.modules import W25Q32
-        from litespi.opcodes import SpiNorFlashOpCodes as Codes
-        self.add_spi_flash(mode="1x", module=W25Q32(Codes.READ_1_1_1), with_master=False)
-
-        # Add ROM linker region --------------------------------------------------------------------
-        self.bus.add_region("rom", SoCRegion(
-            origin = self.bus.regions["spiflash"].origin + bios_flash_offset,
-            size   = 64*kB,
-            linker = True)
-        )
-        self.cpu.set_reset_address(self.bus.regions["rom"].origin)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on SITLINV XC7K420T", **kwargs)
 
-        # HyperRAM ---------------------------------------------------------------------------------
+        # DDR3 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
-            # TODO: Use second 32Mbit PSRAM chip.
-            dq      = platform.request("IO_psram_dq")
-            rwds    = platform.request("IO_psram_rwds")
-            reset_n = platform.request("O_psram_reset_n")
-            cs_n    = platform.request("O_psram_cs_n")
-            ck      = platform.request("O_psram_ck")
-            ck_n    = platform.request("O_psram_ck_n")
-            class HyperRAMPads:
-                def __init__(self, n):
-                    self.clk   = Signal()
-                    self.rst_n = reset_n[n]
-                    self.dq    = dq[8*n:8*(n+1)]
-                    self.cs_n  = cs_n[n]
-                    self.rwds  = rwds[n]
-
-            hyperram_pads = HyperRAMPads(0)
-            self.comb += ck[0].eq(hyperram_pads.clk)
-            self.comb += ck_n[0].eq(~hyperram_pads.clk)
-            # FIXME: Issue with upstream HyperRAM core, so use old one. Need to investigate.
-            if not os.path.exists("hyperbus.py"):
-                os.system("wget https://github.com/litex-hub/litex-boards/files/8831568/hyperbus.py.txt")
-                os.system("mv hyperbus.py.txt hyperbus.py")
-            from hyperbus import HyperRAM
-            self.hyperram = HyperRAM(hyperram_pads)
-            self.bus.add_slave("main_ram", slave=self.hyperram.bus, region=SoCRegion(origin=self.mem_map["main_ram"], size=4*mB))
-
-        # Video ------------------------------------------------------------------------------------
-        if with_video_terminal:
-            self.videophy = VideoGowinHDMIPHY(platform.request("hdmi"), clock_domain="hdmi")
-            self.add_video_colorbars(phy=self.videophy, timings="640x480@60Hz", clock_domain="hdmi")
-            #self.add_video_terminal(phy=self.videophy, timings="640x480@75Hz", clock_domain="hdmi") # FIXME: Free up BRAMs.
+            # we need to use A7DDRPHY instead of K7DDRPHY, because the 420T has no ODELAYE2
+            self.ddrphy = s7ddrphy.A7DDRPHY(
+                pads         = PHYPadsReducer(platform.request("ddram", 0), [0, 1, 2, 3]),
+                #pads         = platform.request("ddram", 0),
+                memtype      = "DDR3",
+                nphases      = 4,
+                sys_clk_freq = sys_clk_freq,
+                iodelay_clk_freq = 200e6
+            )
+            self.add_sdram("sdram",
+                phy           = self.ddrphy,
+                module        = K4B1G0446F(sys_clk_freq, "1:4", "800"),
+                l2_cache_size = kwargs.get("l2_size", 8192),
+            )
 
+        # PCIe -------------------------------------------------------------------------------------
+        if with_pcie:
+            self.pcie_phy = S7PCIEPHY(platform, platform.request("pcie_x4"),
+                data_width = 128,
+                bar0_size  = 0x20000)
+            self.add_pcie(phy=self.pcie_phy, ndmas=1)
+
+        # TODO verify / test
+        # SATA -------------------------------------------------------------------------------------
+        if with_sata:
+            from litex.build.generic_platform import Subsignal, Pins
+            from litesata.phy import LiteSATAPHY
+
+            # RefClk, Generate 150MHz from PLL.
+            self.cd_sata_refclk = ClockDomain()
+            self.crg.pll.create_clkout(self.cd_sata_refclk, 150e6)
+            sata_refclk = ClockSignal("sata_refclk")
+            platform.add_platform_command("set_property SEVERITY {{Warning}} [get_drc_checks REQP-52]")
+
+            # PHY
+            self.sata_phy = LiteSATAPHY(platform.device,
+                refclk     = sata_refclk,
+                pads       = platform.request("sata", 0),
+                gen        = "gen2",
+                clk_freq   = sys_clk_freq,
+                data_width = 16)
+
+            # Core
+            self.add_sata(phy=self.sata_phy, mode="read+write")
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
-                pads         = platform.request_all("user_led"),
+                pads         = platform.request_all("user_led_n"),
                 sys_clk_freq = sys_clk_freq)
 
+        # I2C --------------------------------------------------------------------------------------
+        self.i2c = I2CMaster(platform.request("i2c"))
+
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=sipeed_tang_nano_9k.Platform, description="LiteX SoC on Tang Nano 9K.")
-    parser.add_target_argument("--flash",                action="store_true",      help="Flash Bitstream.")
-    parser.add_target_argument("--sys-clk-freq",         default=27e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--bios-flash-offset",    default="0x0",            help="BIOS offset in SPI Flash.")
-    parser.add_target_argument("--with-spi-sdcard",      action="store_true",      help="Enable SPI-mode SDCard support.")
-    parser.add_target_argument("--with-video-terminal",  action="store_true",      help="Enable Video Terminal (HDMI).")
-    parser.add_target_argument("--prog-kit",             default="openfpgaloader", help="Programmer select from Gowin/openFPGALoader.")
+    parser = LiteXArgumentParser(platform=sitlinv_xc7k420t.Platform, description="LiteX SoC on AliExpress SITLINV FPGA Store XC7K420T")
+    parser.add_target_argument("--sys-clk-freq",    default=100e6, type=float, help="System clock frequency.")
+    parser.add_target_argument("--io-voltage",      default="3.3V",            help="IO voltage chosen by Jumper J3. Can be: '3.3V' or '2.5V'.")
+    parser.add_target_argument("--with-pcie",       action="store_true",       help="Enable PCIe support.")
+    parser.add_target_argument("--driver",          action="store_true",       help="Generate PCIe driver.")
+    parser.add_target_argument("--with-sata",       action="store_true",       help="Enable SATA support.")
     args = parser.parse_args()
 
     soc = BaseSoC(
-        sys_clk_freq        = args.sys_clk_freq,
-        bios_flash_offset   = int(args.bios_flash_offset, 0),
-        with_video_terminal = args.with_video_terminal,
+        sys_clk_freq   = args.sys_clk_freq,
+        io_voltage     = args.io_voltage,
+        with_pcie      = args.with_pcie,
+        with_sata      = args.with_sata,
         **parser.soc_argdict
     )
-
-    if args.with_spi_sdcard:
-        soc.add_spi_sdcard()
-
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
+    if args.driver:
+        generate_litepcie_software(soc, os.path.join(builder.output_dir, "driver"))
+
     if args.load:
-        prog = soc.platform.create_programmer(kit=args.prog_kit)
+        prog = soc.platform.create_programmer()
         prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
 
-    if args.flash:
-        prog = soc.platform.create_programmer(kit=args.prog_kit)
-        prog.flash(0, builder.get_bitstream_filename(mode="flash", ext=".fs")) # FIXME
-        # Axternal SPI programming not supported by gowin 'programmer_cli' now!
-        # if needed, use openFPGALoader or Gowin programmer GUI
-        if args.prog_kit == "openfpgaloader":
-            prog.flash(int(args.bios_flash_offset, 0), builder.get_bios_filename(), external=True)
-
 if __name__ == "__main__":
     main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/sipeed_tang_primer.py` & `litex-boards-2023.8/litex_boards/targets/sipeed_tang_primer.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/sipeed_tang_primer_20k.py` & `litex-boards-2023.8/litex_boards/targets/sitlinv_stlv7325_v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,239 +1,247 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2022 Icenowy Zheng <icenowy@aosc.io>
-# Copyright (c) 2022 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2022 Andrew Gillham <gillham@roadsign.com>
+# Copyright (c) 2014-2015 Sebastien Bourdeauducq <sb@m-labs.hk>
+# Copyright (c) 2014-2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2014-2015 Yann Sionneau <ys@m-labs.hk>
 # SPDX-License-Identifier: BSD-2-Clause
 
+import os
+
 from migen import *
-from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex.soc.cores.clock.gowin_gw2a import GW2APLL
+from litex_boards.platforms import sitlinv_stlv7325_v1
+
+from litex.soc.cores.clock import *
 from litex.soc.integration.soc_core import *
-from litex.soc.integration.soc import SoCRegion
 from litex.soc.integration.builder import *
-from litex.soc.cores.led import LedChaser, WS2812
-from litex.soc.cores.gpio import GPIOIn
-from litex.soc.cores.video import *
+from litex.soc.cores.led import LedChaser
+from litex.soc.cores.bitbang import I2CMaster
+from litex.soc.cores.video   import VideoS7HDMIPHY
 
-from liteeth.phy.rmii import LiteEthPHYRMII
+from litedram.modules import MT8JTF12864
+from litedram.phy import s7ddrphy
 
-from litex_boards.platforms import sipeed_tang_primer_20k
+from liteeth.phy import LiteEthPHY
 
-from litedram.common import PHYPadsReducer
-from litedram.modules import MT41K64M16
-from litedram.phy import GW2DDRPHY
+from litepcie.phy.s7pciephy import S7PCIEPHY
+from litepcie.software import generate_litepcie_software
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq, with_video_pll=False):
-        self.rst        = Signal()
-        self.cd_sys     = ClockDomain()
-        self.cd_por     = ClockDomain()
-        self.cd_init    = ClockDomain()
-        self.cd_sys2x   = ClockDomain()
-        self.cd_sys2x_i = ClockDomain()
+    def __init__(self, platform, sys_clk_freq):
+        self.rst       = Signal()
+        self.cd_sys    = ClockDomain()
+        self.cd_sys4x  = ClockDomain()
+        self.cd_idelay = ClockDomain()
+        self.cd_hdmi   = ClockDomain()
+        self.cd_hdmi5x = ClockDomain()
 
         # # #
 
-        self.stop  = Signal()
-        self.reset = Signal()
+        # Clk/Rst.
+        clk200 = platform.request("clk200")
+        clk100 = platform.request("clk100")
+        rst_n  = platform.request("cpu_reset_n")
+
+        # PLL.
+        self.pll = pll = S7PLL(speedgrade=-2)
+        self.comb += pll.reset.eq(~rst_n | self.rst)
+        pll.register_clkin(clk200, 200e6)
+        pll.create_clkout(self.cd_sys,    sys_clk_freq)
+        pll.create_clkout(self.cd_sys4x,  4*sys_clk_freq)
+        pll.create_clkout(self.cd_idelay, 200e6)
+        platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
+
+        self.submodules.pll2 = pll2 = S7PLL(speedgrade=-2)
+        self.comb += pll2.reset.eq(~rst_n | self.rst)
+        pll2.register_clkin(clk100, 100e6)
+        pll2.create_clkout(self.cd_hdmi,   25e6,  margin=0)
+        pll2.create_clkout(self.cd_hdmi5x, 125e6, margin=0)
 
-        # Clk
-        clk27 = platform.request("clk27")
-
-        # Power on reset (the onboard POR is not aware of reprogramming)
-        por_count = Signal(16, reset=2**16-1)
-        por_done  = Signal()
-        self.comb += self.cd_por.clk.eq(clk27)
-        self.comb += por_done.eq(por_count == 0)
-        self.sync.por += If(~por_done, por_count.eq(por_count - 1))
-
-        # PLL
-        self.pll = pll = GW2APLL(devicename=platform.devicename, device=platform.device)
-        self.comb += pll.reset.eq(~por_done)
-        pll.register_clkin(clk27, 27e6)
-        pll.create_clkout(self.cd_sys2x_i, 2*sys_clk_freq)
-        self.specials += [
-            Instance("DHCEN",
-                i_CLKIN  = self.cd_sys2x_i.clk,
-                i_CE     = self.stop,
-                o_CLKOUT = self.cd_sys2x.clk),
-            Instance("CLKDIV",
-                p_DIV_MODE = "2",
-                i_CALIB    = 0,
-                i_HCLKIN   = self.cd_sys2x.clk,
-                i_RESETN   = ~self.reset,
-                o_CLKOUT   = self.cd_sys.clk),
-            AsyncResetSynchronizer(self.cd_sys, ~pll.locked | self.rst | self.reset),
-        ]
-
-        # Init clock domain
-        self.comb += self.cd_init.clk.eq(clk27)
-        self.comb += self.cd_init.rst.eq(pll.reset)
-
-        # Video PLL
-        if with_video_pll:
-            self.video_pll = video_pll = GW2APLL(devicename=platform.devicename, device=platform.device)
-            video_pll.register_clkin(clk27, 27e6)
-            self.cd_hdmi   = ClockDomain()
-            self.cd_hdmi5x = ClockDomain()
-            video_pll.create_clkout(self.cd_hdmi5x, 125e6, margin=1e-3)
-            self.specials += Instance("CLKDIV",
-                p_DIV_MODE = "5",
-                i_RESETN   = 1, # Disable reset signal.
-                i_CALIB    = 0, # No calibration.
-                i_HCLKIN   = self.cd_hdmi5x.clk,
-                o_CLKOUT   = self.cd_hdmi.clk
-            )
+        self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=48e6,
-        with_spi_flash      = False,
-        with_led_chaser     = True,
-        with_rgb_led        = False,
-        with_buttons        = True,
-        with_video_terminal = False,
-        with_ethernet       = False,
-        with_etherbone      = False,
-        eth_ip              = "192.168.1.50",
-        eth_dynamic_ip      = False,
-        dock                = "standard",
+    def __init__(self, sys_clk_freq=100e6,
+        vccio                  = "2.5V",
+        with_ethernet          = False,
+        with_etherbone         = False,
+        local_ip               = "192.168.1.50",
+        remote_ip              = "",
+        eth_dynamic_ip         = False,
+        with_led_chaser        = True,
+        with_pcie              = False,
+        with_sata              = False,
+        with_jtagbone          = True,
+        with_video_colorbars   = False,
+        with_video_framebuffer = False,
+        with_video_terminal    = False,
         **kwargs):
-
-        assert dock in ["standard", "lite"]
-
-        platform = sipeed_tang_primer_20k.Platform(dock, toolchain="gowin")
-
-        if dock == "lite":
-            with_led_chaser = False # No leds on core board nor on dock lite.
+        platform = sitlinv_stlv7325_v1.Platform(vccio)
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = _CRG(platform, sys_clk_freq, with_video_pll=with_video_terminal)
+        self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Tang Primer 20K", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Sitlinv STLV7325-V1", **kwargs)
 
         # DDR3 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
-            self.ddrphy = GW2DDRPHY(
-                pads         = platform.request("ddram"),
-                sys_clk_freq = sys_clk_freq
+            self.ddrphy = s7ddrphy.K7DDRPHY(platform.request("ddram"),
+                memtype      = "DDR3",
+                nphases      = 4,
+                sys_clk_freq = sys_clk_freq,
             )
-            self.ddrphy.settings.rtt_nom = "disabled"
-            self.comb += self.crg.stop.eq(self.ddrphy.init.stop)
-            self.comb += self.crg.reset.eq(self.ddrphy.init.reset)
             self.add_sdram("sdram",
                 phy           = self.ddrphy,
-                module        = MT41K64M16(sys_clk_freq, "1:2"),
-                l2_cache_size = kwargs.get("l2_size", 8192)
+                module        = MT8JTF12864(sys_clk_freq, "1:4"),
+                l2_cache_size = kwargs.get("l2_size", 8192),
             )
 
-        # SPI Flash --------------------------------------------------------------------------------
-        if with_spi_flash:
-            from litespi.modules import W25Q32JV as SpiFlashModule
-            from litespi.opcodes import SpiNorFlashOpCodes as Codes
-            self.add_spi_flash(mode="1x", module=SpiFlashModule(Codes.READ_1_1_1))
+        # Jtagbone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
 
         # Ethernet / Etherbone ---------------------------------------------------------------------
         if with_ethernet or with_etherbone:
-            from liteeth.phy.rmii import LiteEthPHYRMII
-            self.ethphy = LiteEthPHYRMII(
-                clock_pads = self.platform.request("eth_clocks"),
-                pads       = self.platform.request("eth"),
-                refclk_cd  = None
-            )
+            self.ethphy = LiteEthPHY(
+                clock_pads = self.platform.request("eth_clocks", 0),
+                pads       = self.platform.request("eth", 0),
+                clk_freq   = self.clk_freq)
             if with_ethernet:
-                self.add_ethernet(phy=self.ethphy, dynamic_ip=eth_dynamic_ip, with_timing_constraints=False)
+                self.add_ethernet(phy=self.ethphy, dynamic_ip=eth_dynamic_ip)
             if with_etherbone:
-                self.add_etherbone(phy=self.ethphy, ip_address=eth_ip, with_timing_constraints=False)
+                self.add_etherbone(phy=self.ethphy)
 
-        # Video ------------------------------------------------------------------------------------
-        if with_video_terminal:
-            hdmi_pads = platform.request("hdmi")
-            self.comb += hdmi_pads.hdp.eq(1)
-            self.videophy = VideoHDMIPHY(hdmi_pads, clock_domain="hdmi")
-            #self.add_video_colorbars(phy=self.videophy, timings="640x480@60Hz", clock_domain="hdmi")
-            self.add_video_terminal(phy=self.videophy, timings="640x480@75Hz", clock_domain="hdmi")
+        if local_ip:
+            local_ip = local_ip.split(".")
+            self.add_constant("LOCALIP1", int(local_ip[0]))
+            self.add_constant("LOCALIP2", int(local_ip[1]))
+            self.add_constant("LOCALIP3", int(local_ip[2]))
+            self.add_constant("LOCALIP4", int(local_ip[3]))
+
+        if remote_ip:
+            remote_ip = remote_ip.split(".")
+            self.add_constant("REMOTEIP1", int(remote_ip[0]))
+            self.add_constant("REMOTEIP2", int(remote_ip[1]))
+            self.add_constant("REMOTEIP3", int(remote_ip[2]))
+            self.add_constant("REMOTEIP4", int(remote_ip[3]))
+
+        # PCIe -------------------------------------------------------------------------------------
+        if with_pcie:
+            self.pcie_phy = S7PCIEPHY(platform, platform.request("pcie_x4"),
+                data_width = 128,
+                bar0_size  = 0x20000)
+            self.add_pcie(phy=self.pcie_phy, ndmas=1)
+
+        # TODO verify / test
+        # SATA -------------------------------------------------------------------------------------
+        if with_sata:
+            from litex.build.generic_platform import Subsignal, Pins
+            from litesata.phy import LiteSATAPHY
+
+            # RefClk, Generate 150MHz from PLL.
+            self.cd_sata_refclk = ClockDomain()
+            self.crg.pll.create_clkout(self.cd_sata_refclk, 150e6)
+            sata_refclk = ClockSignal("sata_refclk")
+            platform.add_platform_command("set_property SEVERITY {{Warning}} [get_drc_checks REQP-52]")
+
+            # PHY
+            self.sata_phy = LiteSATAPHY(platform.device,
+                refclk     = sata_refclk,
+                pads       = platform.request("sata", 0),
+                gen        = "gen2",
+                clk_freq   = sys_clk_freq,
+                data_width = 16)
+
+            # Core
+            self.add_sata(phy=self.sata_phy, mode="read+write")
+
+        # HDMI Options -----------------------------------------------------------------------------
+        if (with_video_colorbars or with_video_framebuffer or with_video_terminal):
+            self.submodules.videophy = VideoS7HDMIPHY(platform.request("hdmi_out"), clock_domain="hdmi")
+            if with_video_colorbars:
+                self.add_video_colorbars(phy=self.videophy, timings="640x480@60Hz", clock_domain="hdmi")
+            if with_video_terminal:
+                self.add_video_terminal(phy=self.videophy, timings="640x480@60Hz", clock_domain="hdmi")
+            if with_video_framebuffer:
+                self.add_video_framebuffer(phy=self.videophy, timings="640x480@60Hz", clock_domain="hdmi")
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
-                pads         = platform.request_all("led"),
-                sys_clk_freq = sys_clk_freq
-            )
-
-        # RGB Led ----------------------------------------------------------------------------------
-        if with_rgb_led:
-            self.rgb_led = WS2812(
-                pad          = platform.request("rgb_led"),
-                nleds        = 1,
-                sys_clk_freq = sys_clk_freq
-            )
-            self.bus.add_slave(name="rgb_led", slave=self.rgb_led.bus, region=SoCRegion(
-                origin = 0x2000_0000,
-                size   = 4,
-            ))
-
-        # Buttons ----------------------------------------------------------------------------------
-        if with_buttons:
-            self.buttons = GPIOIn(pads=~platform.request_all("btn_n"))
+                pads         = platform.request_all("user_led_n"),
+                sys_clk_freq = sys_clk_freq)
 
+        # I2C --------------------------------------------------------------------------------------
+        self.i2c = I2CMaster(platform.request("i2c"))
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=sipeed_tang_primer_20k.Platform, description="LiteX SoC on Tang Primer 20K.")
-    parser.add_target_argument("--dock",         default="standard",       help="Dock version (standard (default) or lite.")
-    parser.add_target_argument("--flash",        action="store_true",      help="Flash Bitstream.")
-    parser.add_target_argument("--sys-clk-freq", default=48e6, type=float, help="System clock frequency.")
-    sdopts = parser.target_group.add_mutually_exclusive_group()
-    sdopts.add_argument("--with-spi-sdcard",            action="store_true", help="Enable SPI-mode SDCard support.")
-    sdopts.add_argument("--with-sdcard",                action="store_true", help="Enable SDCard support.")
-    parser.add_target_argument("--with-spi-flash",      action="store_true", help="Enable SPI Flash (MMAPed).")
-    parser.add_target_argument("--with-video-terminal", action="store_true", help="Enable Video Terminal (HDMI).")
+    parser = LiteXArgumentParser(platform=sitlinv_stlv7325_v1.Platform, description="LiteX SoC on Sitlinv STLV7325-V1.")
+    parser.add_target_argument("--sys-clk-freq",  default=100e6, type=float, help="System clock frequency.")
+    parser.add_target_argument("--vccio",         default="2.5V", type=str, help="IO Voltage (set by J4), can be 2.5V or 3.3V")
     ethopts = parser.target_group.add_mutually_exclusive_group()
-    ethopts.add_argument("--with-ethernet",         action="store_true",    help="Add Ethernet.")
-    ethopts.add_argument("--with-etherbone",        action="store_true",    help="Add EtherBone.")
-    parser.add_target_argument("--eth-ip",          default="192.168.1.50", help="Etherbone IP address.")
+    ethopts.add_argument("--with-ethernet",         action="store_true",    help="Enable Ethernet support.")
+    ethopts.add_argument("--with-etherbone",        action="store_true",    help="Enable Etherbone support.")
+    parser.add_target_argument("--remote-ip",       default="192.168.1.100",help="Remote IP address of TFTP server.")
+    parser.add_target_argument("--local-ip",        default="192.168.1.50", help="Local IP address.")
     parser.add_target_argument("--eth-dynamic-ip",  action="store_true",    help="Enable dynamic Ethernet IP addresses setting.")
+    parser.add_target_argument("--with-pcie",       action="store_true",    help="Enable PCIe support.")
+    parser.add_target_argument("--driver",          action="store_true",    help="Generate PCIe driver.")
+    parser.add_target_argument("--with-sata",       action="store_true",    help="Enable SATA support.")
+    parser.add_target_argument("--with-jtagbone",   action="store_true",    help="Enable Jtagbone support.")
+    sdopts = parser.target_group.add_mutually_exclusive_group()
+    sdopts.add_argument("--with-spi-sdcard", action="store_true", help="Enable SPI-mode SDCard support.")
+    sdopts.add_argument("--with-sdcard",     action="store_true", help="Enable SDCard support.")
+    viopts = parser.target_group.add_mutually_exclusive_group()
+    viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (HDMI).")
+    viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (HDMI).")
+    viopts.add_argument("--with-video-colorbars",   action="store_true", help="Enable Video Colorbars (HDMI).")
     args = parser.parse_args()
 
+    assert not (args.with_etherbone and args.eth_dynamic_ip)
+
     soc = BaseSoC(
-        sys_clk_freq        = args.sys_clk_freq,
-        with_spi_flash      = args.with_spi_flash,
-        with_video_terminal = args.with_video_terminal,
-        with_ethernet       = args.with_ethernet,
-        with_etherbone      = args.with_etherbone,
-        eth_ip              = args.eth_ip,
-        eth_dynamic_ip      = args.eth_dynamic_ip,
-        dock                = args.dock,
+        sys_clk_freq           = args.sys_clk_freq,
+        vccio                  = args.vccio,
+        with_ethernet          = args.with_ethernet,
+        with_etherbone         = args.with_etherbone,
+        local_ip               = args.local_ip,
+        remote_ip              = args.remote_ip,
+        eth_dynamic_ip         = args.eth_dynamic_ip,
+        with_pcie              = args.with_pcie,
+        with_sata              = args.with_sata,
+        with_jtagbone          = args.with_jtagbone,
+        with_video_colorbars   = args.with_video_colorbars,
+        with_video_framebuffer = args.with_video_framebuffer,
+        with_video_terminal    = args.with_video_terminal,
         **parser.soc_argdict
     )
     if args.with_spi_sdcard:
         soc.add_spi_sdcard()
     if args.with_sdcard:
         soc.add_sdcard()
-
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
+    if args.driver:
+        generate_litepcie_software(soc, os.path.join(builder.output_dir, "driver"))
+
     if args.load:
         prog = soc.platform.create_programmer()
         prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
 
-    if args.flash:
-        prog = soc.platform.create_programmer()
-        prog.flash(0, builder.get_bitstream_filename(mode="flash", ext=".fs"), external=True)
-
 if __name__ == "__main__":
     main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/sipeed_tang_primer_25k.py` & `litex-boards-2023.8/litex_boards/targets/ztex213.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,105 +1,116 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2023 Gwenhael Goavec-Merou <gwenhael.goavec-merou@trabucayre.com>
+# Copyright (c) 2015-2019 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2020-2021 Romain Dolbeau <romain@dolbeau.org>
 # SPDX-License-Identifier: BSD-2-Clause
 
+# Support for the ZTEX USB-FGPA Module 2.13:https://www.ztex.de/usb-fpga-2/usb-fpga-2.13.e.html.
+# With (no-so-optional) expansion, either the ZTEX Debug board:
+# https://www.ztex.de/usb-fpga-2/debug.e.html
+# Or the SBusFPGA adapter board:
+# https://github.com/rdolbeau/SBusFPGA
+
 from migen import *
 
 from litex.gen import *
 
-from litex.soc.cores.clock.gowin_gw5a import GW5APLL
+from litex_boards.platforms import ztex213
+
+from litex.soc.cores.clock import *
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
 from litex.soc.cores.led import LedChaser
-from litex.soc.cores.gpio import GPIOIn
 
-from litex_boards.platforms import sipeed_tang_primer_25k
+from litedram.modules import MT41J128M16
+from litedram.phy import s7ddrphy
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
     def __init__(self, platform, sys_clk_freq):
-        self.rst    = Signal()
-        self.cd_sys = ClockDomain()
-        self.cd_por = ClockDomain()
+        self.rst          = Signal()
+        self.cd_sys       = ClockDomain()
+        self.cd_sys4x     = ClockDomain()
+        self.cd_sys4x_dqs = ClockDomain()
+        self.cd_idelay    = ClockDomain()
+        self.cd_por       = ClockDomain()
 
         # # #
+        clk48 = platform.request("clk48")
 
-        # Clk
-        clk50 = platform.request("clk50")
+        self.pll = pll = S7MMCM(speedgrade=-1)
+        pll.register_clkin(clk48, 48e6)
+        pll.create_clkout(self.cd_sys,       sys_clk_freq)
+        pll.create_clkout(self.cd_sys4x,     4*sys_clk_freq)
+        pll.create_clkout(self.cd_sys4x_dqs, 4*sys_clk_freq, phase=90)
+        pll.create_clkout(self.cd_idelay,    200e6)
 
         # Power on reset
         por_count = Signal(16, reset=2**16-1)
         por_done  = Signal()
-        self.comb += [
-            self.cd_por.clk.eq(clk50),
-            por_done.eq(por_count == 0),
-        ]
+        self.comb += self.cd_por.clk.eq(clk48)
+        self.comb += por_done.eq(por_count == 0)
         self.sync.por += If(~por_done, por_count.eq(por_count - 1))
-
-        # PLL
-        self.pll = pll = GW5APLL(devicename=platform.devicename, device=platform.device)
         self.comb += pll.reset.eq(~por_done | self.rst)
-        pll.register_clkin(clk50, 50e6)
-        pll.create_clkout(self.cd_sys, sys_clk_freq)
+
+        self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=50e6,
-        with_spi_flash      = False,
-        with_led_chaser     = True,
-        with_buttons        = True,
+    def __init__(self, variant="ztex2.13a", sys_clk_freq=100e6, expansion="debug",
+        with_led_chaser = True,
         **kwargs):
-
-        platform = sipeed_tang_primer_25k.Platform(toolchain="gowin")
+        platform = ztex213.Platform(variant=variant, expansion=expansion)
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Tang Primer 25K", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Ztex 2.13", **kwargs)
 
-        # SPI Flash --------------------------------------------------------------------------------
-        if with_spi_flash:
-            from litespi.modules import W25Q64FV as SpiFlashModule
-            from litespi.opcodes import SpiNorFlashOpCodes as Codes
-            self.add_spi_flash(mode="1x", module=SpiFlashModule(Codes.READ_1_1_1))
+        # DDR3 SDRAM -------------------------------------------------------------------------------
+        if not self.integrated_main_ram_size:
+            self.ddrphy = s7ddrphy.A7DDRPHY(platform.request("ddram"),
+                memtype        = "DDR3",
+                nphases        = 4,
+                sys_clk_freq   = sys_clk_freq)
+            self.add_sdram("sdram",
+                phy           = self.ddrphy,
+                module        = MT41J128M16(sys_clk_freq, "1:4"),
+                l2_cache_size = kwargs.get("l2_size", 8192)
+            )
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
-                pads         = platform.request_all("led"),
-                sys_clk_freq = sys_clk_freq
-            )
-
-        # Buttons ----------------------------------------------------------------------------------
-        if with_buttons:
-            self.buttons = GPIOIn(pads=~platform.request_all("btn_n"))
-
+                pads         = platform.request_all("user_led"),
+                sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=sipeed_tang_primer_25k.Platform, description="LiteX SoC on Tang Primer 25K.")
-    parser.add_target_argument("--flash",        action="store_true",      help="Flash Bitstream.")
-    parser.add_target_argument("--sys-clk-freq", default=50e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--with-spi-flash",      action="store_true", help="Enable SPI Flash (MMAPed).")
+    parser = LiteXArgumentParser(platform=ztex213.Platform, description="LiteX SoC on Ztex 2.13.")
+    parser.add_target_argument("--expansion",       default="debug",           help="Expansion board (debug or sbus).")
+    parser.add_target_argument("--sys-clk-freq",    default=100e6, type=float, help="System clock frequency.")
+    parser.add_target_argument("--with-spi-sdcard", action="store_true",       help="Enable SPI-mode SDCard support.")
+    parser.add_target_argument("--with-sdcard",     action="store_true",       help="Enable SDCard support.")
     args = parser.parse_args()
 
-    soc = BaseSoC(
-        sys_clk_freq   = args.sys_clk_freq,
-        with_spi_flash = args.with_spi_flash,
-        **parser.soc_argdict
-    )
+    soc = BaseSoC(sys_clk_freq=args.sys_clk_freq, expansion=args.expansion, **parser.soc_argdict)
+    assert not (args.with_spi_sdcard and args.with_sdcard)
+    if args.with_spi_sdcard:
+        soc.add_spi_sdcard() # SBus only
+    if args.with_sdcard:
+        soc.add_sdcard() # SBus only
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
     if args.load:
         prog = soc.platform.create_programmer()
         prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
```

### Comparing `litex-boards-2023.12/litex_boards/targets/sitlinv_a_e115fb.py` & `litex-boards-2023.8/litex_boards/targets/sitlinv_a_e115fb.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/sitlinv_stlv7325_v1.py` & `litex-boards-2023.8/litex_boards/targets/sitlinv_stlv7325_v2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
+# Copyright (c) 2023 Gabriel Somlo <gsomlo@gmail.com>
 # Copyright (c) 2022 Andrew Gillham <gillham@roadsign.com>
 # Copyright (c) 2014-2015 Sebastien Bourdeauducq <sb@m-labs.hk>
 # Copyright (c) 2014-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # Copyright (c) 2014-2015 Yann Sionneau <ys@m-labs.hk>
 # SPDX-License-Identifier: BSD-2-Clause
 
 import os
 
 from migen import *
 
 from litex.gen import *
 
-from litex_boards.platforms import sitlinv_stlv7325_v1
+from litex_boards.platforms import sitlinv_stlv7325_v2
 
 from litex.soc.cores.clock import *
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
 from litex.soc.cores.led import LedChaser
 from litex.soc.cores.bitbang import I2CMaster
 from litex.soc.cores.video   import VideoS7HDMIPHY
 
 from litedram.modules import MT8JTF12864
 from litedram.phy import s7ddrphy
 
-from liteeth.phy import LiteEthPHY
+from liteeth.phy.s7rgmii import LiteEthPHYRGMII
 
 from litepcie.phy.s7pciephy import S7PCIEPHY
 from litepcie.software import generate_litepcie_software
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
@@ -43,96 +44,82 @@
         self.cd_hdmi   = ClockDomain()
         self.cd_hdmi5x = ClockDomain()
 
         # # #
 
         # Clk/Rst.
         clk200 = platform.request("clk200")
-        clk100 = platform.request("clk100")
+        clk50  = platform.request("clk50")
         rst_n  = platform.request("cpu_reset_n")
 
         # PLL.
         self.pll = pll = S7PLL(speedgrade=-2)
         self.comb += pll.reset.eq(~rst_n | self.rst)
         pll.register_clkin(clk200, 200e6)
         pll.create_clkout(self.cd_sys,    sys_clk_freq)
         pll.create_clkout(self.cd_sys4x,  4*sys_clk_freq)
         pll.create_clkout(self.cd_idelay, 200e6)
         platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
 
         self.submodules.pll2 = pll2 = S7PLL(speedgrade=-2)
         self.comb += pll2.reset.eq(~rst_n | self.rst)
-        pll2.register_clkin(clk100, 100e6)
+        pll2.register_clkin(clk50, 50e6)
         pll2.create_clkout(self.cd_hdmi,   25e6,  margin=0)
         pll2.create_clkout(self.cd_hdmi5x, 125e6, margin=0)
 
         self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
     def __init__(self, sys_clk_freq=100e6,
-        vccio                  = "2.5V",
+        vccio                  = "3.3V",
         with_ethernet          = False,
-        with_etherbone         = False,
-        local_ip               = "192.168.1.50",
-        remote_ip              = "",
-        eth_dynamic_ip         = False,
         with_led_chaser        = True,
         with_pcie              = False,
-        with_sata              = False,
+        with_sata              = False, sata_gen="gen2",
+        with_jtagbone          = False,
         with_video_colorbars   = False,
         with_video_framebuffer = False,
         with_video_terminal    = False,
         **kwargs):
-        platform = sitlinv_stlv7325_v1.Platform(vccio)
+        platform = sitlinv_stlv7325_v2.Platform(vccio)
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Sitlinv STLV7325-V1", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Sitlinv STLV7325-v2", **kwargs)
 
         # DDR3 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
             self.ddrphy = s7ddrphy.K7DDRPHY(platform.request("ddram"),
                 memtype      = "DDR3",
                 nphases      = 4,
                 sys_clk_freq = sys_clk_freq,
             )
             self.add_sdram("sdram",
                 phy           = self.ddrphy,
                 module        = MT8JTF12864(sys_clk_freq, "1:4"),
                 l2_cache_size = kwargs.get("l2_size", 8192),
             )
 
+        # Jtagbone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
+
         # Ethernet / Etherbone ---------------------------------------------------------------------
-        if with_ethernet or with_etherbone:
-            self.ethphy = LiteEthPHY(
+        if with_ethernet:
+            self.ethphy = LiteEthPHYRGMII(
                 clock_pads = self.platform.request("eth_clocks", 0),
                 pads       = self.platform.request("eth", 0),
-                clk_freq   = self.clk_freq)
-            if with_ethernet:
-                self.add_ethernet(phy=self.ethphy, dynamic_ip=eth_dynamic_ip)
-            if with_etherbone:
-                self.add_etherbone(phy=self.ethphy)
-
-        if local_ip:
-            local_ip = local_ip.split(".")
-            self.add_constant("LOCALIP1", int(local_ip[0]))
-            self.add_constant("LOCALIP2", int(local_ip[1]))
-            self.add_constant("LOCALIP3", int(local_ip[2]))
-            self.add_constant("LOCALIP4", int(local_ip[3]))
-
-        if remote_ip:
-            remote_ip = remote_ip.split(".")
-            self.add_constant("REMOTEIP1", int(remote_ip[0]))
-            self.add_constant("REMOTEIP2", int(remote_ip[1]))
-            self.add_constant("REMOTEIP3", int(remote_ip[2]))
-            self.add_constant("REMOTEIP4", int(remote_ip[3]))
+                tx_delay = 1.417e-9,
+                rx_delay = 1.417e-9,
+            )
+            self.add_ethernet(phy=self.ethphy)
 
         # PCIe -------------------------------------------------------------------------------------
         if with_pcie:
             self.pcie_phy = S7PCIEPHY(platform, platform.request("pcie_x4"),
                 data_width = 128,
                 bar0_size  = 0x20000)
             self.add_pcie(phy=self.pcie_phy, ndmas=1)
@@ -149,15 +136,15 @@
             sata_refclk = ClockSignal("sata_refclk")
             platform.add_platform_command("set_property SEVERITY {{Warning}} [get_drc_checks REQP-52]")
 
             # PHY
             self.sata_phy = LiteSATAPHY(platform.device,
                 refclk     = sata_refclk,
                 pads       = platform.request("sata", 0),
-                gen        = "gen2",
+                gen        = sata_gen,
                 clk_freq   = sys_clk_freq,
                 data_width = 16)
 
             # Core
             self.add_sata(phy=self.sata_phy, mode="read+write")
 
         # HDMI Options -----------------------------------------------------------------------------
@@ -179,47 +166,40 @@
         # I2C --------------------------------------------------------------------------------------
         self.i2c = I2CMaster(platform.request("i2c"))
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=sitlinv_stlv7325_v1.Platform, description="LiteX SoC on Sitlinv STLV7325-V1.")
+    parser = LiteXArgumentParser(platform=sitlinv_stlv7325_v2.Platform, description="LiteX SoC on AliExpress STLV7325-v2.")
     parser.add_target_argument("--sys-clk-freq",  default=100e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--vccio",         default="2.5V", type=str, help="IO Voltage (set by J4), can be 2.5V or 3.3V")
-    ethopts = parser.target_group.add_mutually_exclusive_group()
-    ethopts.add_argument("--with-ethernet",         action="store_true",    help="Enable Ethernet support.")
-    ethopts.add_argument("--with-etherbone",        action="store_true",    help="Enable Etherbone support.")
-    parser.add_target_argument("--remote-ip",       default="192.168.1.100",help="Remote IP address of TFTP server.")
-    parser.add_target_argument("--local-ip",        default="192.168.1.50", help="Local IP address.")
-    parser.add_target_argument("--eth-dynamic-ip",  action="store_true",    help="Enable dynamic Ethernet IP addresses setting.")
+    parser.add_target_argument("--vccio",         default="3.3V", type=str, help="IO Voltage (set by J4), can be 2.5V or 3.3V")
     parser.add_target_argument("--with-pcie",       action="store_true",    help="Enable PCIe support.")
     parser.add_target_argument("--driver",          action="store_true",    help="Generate PCIe driver.")
+    parser.add_target_argument("--with-ethernet",   action="store_true",    help="Enable Ethernet support.")
     parser.add_target_argument("--with-sata",       action="store_true",    help="Enable SATA support.")
+    parser.add_target_argument("--sata-gen",        default="2",    help="SATA Gen..", choices=["1", "2", "3"])
+    parser.add_target_argument("--with-jtagbone",   action="store_true",    help="Enable Jtagbone support.")
     sdopts = parser.target_group.add_mutually_exclusive_group()
     sdopts.add_argument("--with-spi-sdcard", action="store_true", help="Enable SPI-mode SDCard support.")
     sdopts.add_argument("--with-sdcard",     action="store_true", help="Enable SDCard support.")
     viopts = parser.target_group.add_mutually_exclusive_group()
     viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (HDMI).")
     viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (HDMI).")
     viopts.add_argument("--with-video-colorbars",   action="store_true", help="Enable Video Colorbars (HDMI).")
     args = parser.parse_args()
 
-    assert not (args.with_etherbone and args.eth_dynamic_ip)
-
     soc = BaseSoC(
         sys_clk_freq           = args.sys_clk_freq,
         vccio                  = args.vccio,
         with_ethernet          = args.with_ethernet,
-        with_etherbone         = args.with_etherbone,
-        local_ip               = args.local_ip,
-        remote_ip              = args.remote_ip,
-        eth_dynamic_ip         = args.eth_dynamic_ip,
         with_pcie              = args.with_pcie,
         with_sata              = args.with_sata,
+        sata_gen               = "gen" + args.sata_gen,
+        with_jtagbone          = args.with_jtagbone,
         with_video_colorbars   = args.with_video_colorbars,
         with_video_framebuffer = args.with_video_framebuffer,
         with_video_terminal    = args.with_video_terminal,
         **parser.soc_argdict
     )
     if args.with_spi_sdcard:
         soc.add_spi_sdcard()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/sitlinv_stlv7325_v2.py` & `litex-boards-2023.8/litex_boards/targets/siglent_sds1104xe.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,213 +1,197 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2023 Gabriel Somlo <gsomlo@gmail.com>
-# Copyright (c) 2022 Andrew Gillham <gillham@roadsign.com>
-# Copyright (c) 2014-2015 Sebastien Bourdeauducq <sb@m-labs.hk>
-# Copyright (c) 2014-2020 Florent Kermarrec <florent@enjoy-digital.fr>
-# Copyright (c) 2014-2015 Yann Sionneau <ys@m-labs.hk>
+# Copyright (c) 2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
-import os
+# Build/Use ----------------------------------------------------------------------------------------
+# Build/Load bitstream:
+# ./siglent_ds1104xe.py --with-etherbone --uart-name=crossover --csr-csv=csr.csv --build --load
+#
+# Test Ethernet:
+# ping 192.168.1.50
+#
+# Test Console:
+# litex_server --udp
+# litex_term crossover
+# --------------------------------------------------------------------------------------------------
 
 from migen import *
 
 from litex.gen import *
 
-from litex_boards.platforms import sitlinv_stlv7325_v2
+from litex_boards.platforms import siglent_sds1104xe
 
 from litex.soc.cores.clock import *
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
-from litex.soc.cores.led import LedChaser
-from litex.soc.cores.bitbang import I2CMaster
-from litex.soc.cores.video   import VideoS7HDMIPHY
+from litex.soc.cores.video import VideoVGAPHY
 
-from litedram.modules import MT8JTF12864
+from litedram.common import PHYPadsReducer
+from litedram.modules import MT41K64M16
 from litedram.phy import s7ddrphy
 
-from liteeth.phy.s7rgmii import LiteEthPHYRGMII
-
-from litepcie.phy.s7pciephy import S7PCIEPHY
-from litepcie.software import generate_litepcie_software
+from liteeth.phy.mii import LiteEthPHYMII
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq):
-        self.rst       = Signal()
-        self.cd_sys    = ClockDomain()
-        self.cd_sys4x  = ClockDomain()
-        self.cd_idelay = ClockDomain()
-        self.cd_hdmi   = ClockDomain()
-        self.cd_hdmi5x = ClockDomain()
+    def __init__(self, platform, sys_clk_freq, with_ethernet=False):
+        self.rst          = Signal()
+        self.cd_sys       = ClockDomain()
+        self.cd_sys4x     = ClockDomain()
+        self.cd_sys4x_dqs = ClockDomain()
+        self.cd_idelay    = ClockDomain()
+        self.cd_dvi       = ClockDomain()
 
         # # #
 
-        # Clk/Rst.
-        clk200 = platform.request("clk200")
-        clk50  = platform.request("clk50")
-        rst_n  = platform.request("cpu_reset_n")
-
-        # PLL.
-        self.pll = pll = S7PLL(speedgrade=-2)
-        self.comb += pll.reset.eq(~rst_n | self.rst)
-        pll.register_clkin(clk200, 200e6)
-        pll.create_clkout(self.cd_sys,    sys_clk_freq)
-        pll.create_clkout(self.cd_sys4x,  4*sys_clk_freq)
-        pll.create_clkout(self.cd_idelay, 200e6)
-        platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
+        # Clk / Rst
+        clk25 = ClockSignal("eth_tx") if with_ethernet else platform.request("eth_clocks").rx
 
-        self.submodules.pll2 = pll2 = S7PLL(speedgrade=-2)
-        self.comb += pll2.reset.eq(~rst_n | self.rst)
-        pll2.register_clkin(clk50, 50e6)
-        pll2.create_clkout(self.cd_hdmi,   25e6,  margin=0)
-        pll2.create_clkout(self.cd_hdmi5x, 125e6, margin=0)
+        # PLL
+        self.pll = pll = S7PLL(speedgrade=-1)
+        pll.register_clkin(clk25, 25e6)
+        pll.create_clkout(self.cd_sys,       sys_clk_freq)
+        pll.create_clkout(self.cd_sys4x,     4*sys_clk_freq)
+        pll.create_clkout(self.cd_sys4x_dqs, 4*sys_clk_freq, phase=90)
+        pll.create_clkout(self.cd_idelay,    200e6)
+        pll.create_clkout(self.cd_dvi,       33.3e6)
+        platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
 
         self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
     def __init__(self, sys_clk_freq=100e6,
-        vccio                  = "3.3V",
-        with_ethernet          = False,
-        with_led_chaser        = True,
-        with_pcie              = False,
-        with_sata              = False, sata_gen="gen2",
-        with_video_colorbars   = False,
-        with_video_framebuffer = False,
+        with_etherbone         = True,
+        eth_ip                 = "192.168.1.50",
         with_video_terminal    = False,
+        with_video_framebuffer = False,
         **kwargs):
-        platform = sitlinv_stlv7325_v2.Platform(vccio)
+        platform = siglent_sds1104xe.Platform()
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = _CRG(platform, sys_clk_freq)
+        self.crg = _CRG(platform, sys_clk_freq, with_ethernet=with_etherbone)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Sitlinv STLV7325-v2", **kwargs)
+        if kwargs.get("uart_name", "serial") == "serial":
+            kwargs["uart_name"] = "crossover" # Defaults to Crossover UART.
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Siglent SDS1104X-E", **kwargs)
 
         # DDR3 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
-            self.ddrphy = s7ddrphy.K7DDRPHY(platform.request("ddram"),
-                memtype      = "DDR3",
-                nphases      = 4,
-                sys_clk_freq = sys_clk_freq,
-            )
+            self.ddrphy = s7ddrphy.A7DDRPHY(
+                pads           = PHYPadsReducer(platform.request("ddram"), [0, 1, 2, 3]),
+                memtype        = "DDR3",
+                nphases        = 4,
+                sys_clk_freq   = sys_clk_freq)
             self.add_sdram("sdram",
                 phy           = self.ddrphy,
-                module        = MT8JTF12864(sys_clk_freq, "1:4"),
-                l2_cache_size = kwargs.get("l2_size", 8192),
+                module        = MT41K64M16(sys_clk_freq, "1:4"),
+                l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
-        # Ethernet / Etherbone ---------------------------------------------------------------------
-        if with_ethernet:
-            self.ethphy = LiteEthPHYRGMII(
-                clock_pads = self.platform.request("eth_clocks", 0),
-                pads       = self.platform.request("eth", 0),
-                tx_delay = 1.417e-9,
-                rx_delay = 1.417e-9,
-            )
-            self.add_ethernet(phy=self.ethphy)
-
-        # PCIe -------------------------------------------------------------------------------------
-        if with_pcie:
-            self.pcie_phy = S7PCIEPHY(platform, platform.request("pcie_x4"),
-                data_width = 128,
-                bar0_size  = 0x20000)
-            self.add_pcie(phy=self.pcie_phy, ndmas=1)
-
-        # TODO verify / test
-        # SATA -------------------------------------------------------------------------------------
-        if with_sata:
-            from litex.build.generic_platform import Subsignal, Pins
-            from litesata.phy import LiteSATAPHY
-
-            # RefClk, Generate 150MHz from PLL.
-            self.cd_sata_refclk = ClockDomain()
-            self.crg.pll.create_clkout(self.cd_sata_refclk, 150e6)
-            sata_refclk = ClockSignal("sata_refclk")
-            platform.add_platform_command("set_property SEVERITY {{Warning}} [get_drc_checks REQP-52]")
-
-            # PHY
-            self.sata_phy = LiteSATAPHY(platform.device,
-                refclk     = sata_refclk,
-                pads       = platform.request("sata", 0),
-                gen        = sata_gen,
-                clk_freq   = sys_clk_freq,
-                data_width = 16)
-
-            # Core
-            self.add_sata(phy=self.sata_phy, mode="read+write")
-
-        # HDMI Options -----------------------------------------------------------------------------
-        if (with_video_colorbars or with_video_framebuffer or with_video_terminal):
-            self.submodules.videophy = VideoS7HDMIPHY(platform.request("hdmi_out"), clock_domain="hdmi")
-            if with_video_colorbars:
-                self.add_video_colorbars(phy=self.videophy, timings="640x480@60Hz", clock_domain="hdmi")
+        # Etherbone --------------------------------------------------------------------------------
+        if with_etherbone:
+            # FIXME: Simplify LiteEth Hybrid MAC integration.
+            from liteeth.common import convert_ip
+            from liteeth.mac import LiteEthMAC
+            from liteeth.core.arp import LiteEthARP
+            from liteeth.core.ip import LiteEthIP
+            from liteeth.core.udp import LiteEthUDP
+            from liteeth.core.icmp import LiteEthICMP
+            from liteeth.core import LiteEthUDPIPCore
+            from liteeth.frontend.etherbone import LiteEthEtherbone
+
+            # Ethernet PHY
+            self.ethphy = LiteEthPHYMII(
+                clock_pads = self.platform.request("eth_clocks"),
+                pads       = self.platform.request("eth"))
+            etherbone_ip_address  = convert_ip("192.168.1.51")
+            etherbone_mac_address = 0x10e2d5000001
+
+            # Ethernet MAC
+            self.ethmac = LiteEthMAC(phy=self.ethphy, dw=8,
+                interface  = "hybrid",
+                endianness = self.cpu.endianness,
+                hw_mac     = etherbone_mac_address)
+
+            # Software Interface.
+            self.add_memory_region("ethmac", getattr(self.mem_map, "ethmac", None), 0x2000, type="io")
+            self.add_wb_slave(self.mem_regions["ethmac"].origin, self.ethmac.bus, 0x2000)
+            if self.irq.enabled:
+                self.irq.add("ethmac", use_loc_if_exists=True)
+
+            # Hardware Interface.
+            self.arp  = LiteEthARP(self.ethmac, etherbone_mac_address, etherbone_ip_address, sys_clk_freq, dw=8)
+            self.ip   = LiteEthIP(self.ethmac, etherbone_mac_address, etherbone_ip_address, self.arp.table, dw=8)
+            self.icmp = LiteEthICMP(self.ip, etherbone_ip_address, dw=8)
+            self.udp  = LiteEthUDP(self.ip, etherbone_ip_address, dw=8)
+            self.add_constant("ETH_PHY_NO_RESET") # Disable reset from BIOS to avoid disabling Hardware Interface.
+
+            # Etherbone
+            self.etherbone = LiteEthEtherbone(self.udp, 1234, mode="master")
+            self.bus.add_master(master=self.etherbone.wishbone.bus)
+
+            # Timing constraints
+            eth_rx_clk = self.ethphy.crg.cd_eth_rx.clk
+            eth_tx_clk = self.ethphy.crg.cd_eth_tx.clk
+            self.platform.add_period_constraint(eth_rx_clk, 1e9/self.ethphy.rx_clk_freq)
+            self.platform.add_period_constraint(eth_tx_clk, 1e9/self.ethphy.tx_clk_freq)
+            self.platform.add_false_path_constraints(self.crg.cd_sys.clk, eth_rx_clk, eth_tx_clk)
+
+        # Video ------------------------------------------------------------------------------------
+        video_timings = ("800x480@60Hz", {
+            "pix_clk"       : 33.3e6,
+            "h_active"      : 800,
+            "h_blanking"    : 256,
+            "h_sync_offset" : 210,
+            "h_sync_width"  : 1,
+            "v_active"      : 480,
+            "v_blanking"    : 45,
+            "v_sync_offset" : 22,
+            "v_sync_width"  : 1,
+        })
+        if with_video_terminal or with_video_framebuffer:
+            self.videophy = VideoVGAPHY(platform.request("lcd"), clock_domain="dvi")
             if with_video_terminal:
-                self.add_video_terminal(phy=self.videophy, timings="640x480@60Hz", clock_domain="hdmi")
+                self.add_video_terminal(phy=self.videophy, timings=video_timings, clock_domain="dvi")
             if with_video_framebuffer:
-                self.add_video_framebuffer(phy=self.videophy, timings="640x480@60Hz", clock_domain="hdmi")
-
-        # Leds -------------------------------------------------------------------------------------
-        if with_led_chaser:
-            self.leds = LedChaser(
-                pads         = platform.request_all("user_led_n"),
-                sys_clk_freq = sys_clk_freq)
-
-        # I2C --------------------------------------------------------------------------------------
-        self.i2c = I2CMaster(platform.request("i2c"))
+                self.add_video_framebuffer(phy=self.videophy, timings=video_timings, clock_domain="dvi")
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=sitlinv_stlv7325_v2.Platform, description="LiteX SoC on AliExpress STLV7325-v2.")
-    parser.add_target_argument("--sys-clk-freq",  default=100e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--vccio",         default="3.3V", type=str, help="IO Voltage (set by J4), can be 2.5V or 3.3V")
-    parser.add_target_argument("--with-pcie",       action="store_true",    help="Enable PCIe support.")
-    parser.add_target_argument("--driver",          action="store_true",    help="Generate PCIe driver.")
-    parser.add_target_argument("--with-ethernet",   action="store_true",    help="Enable Ethernet support.")
-    parser.add_target_argument("--with-sata",       action="store_true",    help="Enable SATA support.")
-    parser.add_target_argument("--sata-gen",        default="2",    help="SATA Gen..", choices=["1", "2", "3"])
-    sdopts = parser.target_group.add_mutually_exclusive_group()
-    sdopts.add_argument("--with-spi-sdcard", action="store_true", help="Enable SPI-mode SDCard support.")
-    sdopts.add_argument("--with-sdcard",     action="store_true", help="Enable SDCard support.")
+    parser = LiteXArgumentParser(platform=siglent_sds1104xe.Platform, description="LiteX SoC on SDS1104X-E.")
+    parser.add_target_argument("--sys-clk-freq",   default=100e6, type=float, help="System clock frequency.")
+    parser.add_target_argument("--with-etherbone", action="store_true",       help="Enable Etherbone support.")
+    parser.add_target_argument("--eth-ip",         default="192.168.1.50",     help="Ethernet/Etherbone IP address.")
     viopts = parser.target_group.add_mutually_exclusive_group()
     viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (HDMI).")
     viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (HDMI).")
-    viopts.add_argument("--with-video-colorbars",   action="store_true", help="Enable Video Colorbars (HDMI).")
     args = parser.parse_args()
 
     soc = BaseSoC(
-        sys_clk_freq           = args.sys_clk_freq,
-        vccio                  = args.vccio,
-        with_ethernet          = args.with_ethernet,
-        with_pcie              = args.with_pcie,
-        with_sata              = args.with_sata,
-        sata_gen               = "gen" + args.sata_gen,
-        with_video_colorbars   = args.with_video_colorbars,
-        with_video_framebuffer = args.with_video_framebuffer,
+        sys_clk_freq   = args.sys_clk_freq,
+        with_etherbone = args.with_etherbone,
+        eth_ip         = args.eth_ip,
         with_video_terminal    = args.with_video_terminal,
+        with_video_framebuffer = args.with_video_framebuffer,
         **parser.soc_argdict
     )
-    if args.with_spi_sdcard:
-        soc.add_spi_sdcard()
-    if args.with_sdcard:
-        soc.add_sdcard()
+
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
-    if args.driver:
-        generate_litepcie_software(soc, os.path.join(builder.output_dir, "driver"))
-
     if args.load:
         prog = soc.platform.create_programmer()
-        prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
+        prog.load_bitstream(builder.get_bitstream_filename(mode="sram"), device=1)
 
 if __name__ == "__main__":
     main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/sitlinv_xc7k420t.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_kcu105.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,163 +1,183 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2022 Andrew Gillham <gillham@roadsign.com>
-# Copyright (c) 2014-2015 Sebastien Bourdeauducq <sb@m-labs.hk>
-# Copyright (c) 2014-2020 Florent Kermarrec <florent@enjoy-digital.fr>
-# Copyright (c) 2014-2015 Yann Sionneau <ys@m-labs.hk>
-# Copyright (c) 2020 Hans Baier <hansfbaier@gmail.com>
+# Copyright (c) 2018-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
-# Board support for this chinese Kintex 420T board by "SITLINV FPGA Board Store"
-# https://www.aliexpress.com/item/1005001631827738.html
-
 import os
 
 from migen import *
+from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex_boards.platforms import sitlinv_xc7k420t
+from litex_boards.platforms import xilinx_kcu105
 
 from litex.soc.cores.clock import *
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
 from litex.soc.cores.led import LedChaser
-from litex.soc.cores.bitbang import I2CMaster
 
-from litedram.phy import s7ddrphy
-from litedram.common import PHYPadsReducer
-from litedram.modules import K4B1G0446F
+from litedram.modules import EDY4016A
+from litedram.phy import usddrphy
+
+from liteeth.phy.ku_1000basex import KU_1000BASEX
 
-from litepcie.phy.s7pciephy import S7PCIEPHY
+from litepcie.phy.uspciephy import USPCIEPHY
 from litepcie.software import generate_litepcie_software
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
     def __init__(self, platform, sys_clk_freq):
-        self.rst          = Signal()
-        self.cd_sys       = ClockDomain()
-        self.cd_sys4x     = ClockDomain()
-        self.cd_sys4x_dqs = ClockDomain()
-        self.cd_idelay    = ClockDomain()
+        self.rst       = Signal()
+        self.cd_sys    = ClockDomain()
+        self.cd_sys4x  = ClockDomain()
+        self.cd_pll4x  = ClockDomain()
+        self.cd_idelay = ClockDomain()
+        self.cd_eth    = ClockDomain()
 
         # # #
 
-        # Clk/Rst.
-        clk100 = platform.request("clk100")
-        rst_n  = platform.request("cpu_reset_n")
-
-        # PLL.
-        self.pll = pll = S7PLL(speedgrade=-2)
-        self.comb += pll.reset.eq(~rst_n | self.rst)
-        pll.register_clkin(clk100, 100e6)
-        pll.create_clkout(self.cd_sys,       sys_clk_freq)
-        pll.create_clkout(self.cd_sys4x,     4*sys_clk_freq)
-        pll.create_clkout(self.cd_sys4x_dqs, 4*sys_clk_freq, phase=120)
-        pll.create_clkout(self.cd_idelay,    200e6)
+        self.pll = pll = USMMCM(speedgrade=-2)
+        self.comb += pll.reset.eq(platform.request("cpu_reset") | self.rst)
+        pll.register_clkin(platform.request("clk125"), 125e6)
+        pll.create_clkout(self.cd_pll4x, sys_clk_freq*4, buf=None, with_reset=False)
+        pll.create_clkout(self.cd_idelay, 200e6)
+        pll.create_clkout(self.cd_eth,    200e6)
         platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
 
-        self.idelayctrl = S7IDELAYCTRL(self.cd_idelay)
+        self.specials += [
+            Instance("BUFGCE_DIV",
+                p_BUFGCE_DIVIDE=4,
+                i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys.clk),
+            Instance("BUFGCE",
+                i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys4x.clk),
+        ]
+
+        self.idelayctrl = USIDELAYCTRL(cd_ref=self.cd_idelay, cd_sys=self.cd_sys)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=100e6,
-        io_voltage      = "3.3V",
+    def __init__(self, sys_clk_freq=125e6,
+        with_ethernet   = False,
+        with_etherbone  = False,
+        eth_ip          = "192.168.1.50",
         with_led_chaser = True,
         with_pcie       = False,
         with_sata       = False,
         **kwargs):
-        platform = sitlinv_xc7k420t.Platform(io_voltage)
+        platform = xilinx_kcu105.Platform()
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on SITLINV XC7K420T", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on KCU105", **kwargs)
 
-        # DDR3 SDRAM -------------------------------------------------------------------------------
+        # DDR4 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
-            # we need to use A7DDRPHY instead of K7DDRPHY, because the 420T has no ODELAYE2
-            self.ddrphy = s7ddrphy.A7DDRPHY(
-                pads         = PHYPadsReducer(platform.request("ddram", 0), [0, 1, 2, 3]),
-                #pads         = platform.request("ddram", 0),
-                memtype      = "DDR3",
-                nphases      = 4,
-                sys_clk_freq = sys_clk_freq,
-                iodelay_clk_freq = 200e6
-            )
+            self.ddrphy = usddrphy.USDDRPHY(platform.request("ddram"),
+                memtype          = "DDR4",
+                sys_clk_freq     = sys_clk_freq,
+                iodelay_clk_freq = 200e6)
             self.add_sdram("sdram",
                 phy           = self.ddrphy,
-                module        = K4B1G0446F(sys_clk_freq, "1:4", "800"),
-                l2_cache_size = kwargs.get("l2_size", 8192),
+                module        = EDY4016A(sys_clk_freq, "1:4"),
+                size          = 0x40000000,
+                l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
+        # Ethernet / Etherbone ---------------------------------------------------------------------
+        if with_ethernet or with_etherbone:
+            self.ethphy = KU_1000BASEX(self.crg.cd_eth.clk,
+                data_pads    = self.platform.request("sfp", 0),
+                sys_clk_freq = self.clk_freq)
+            self.comb += self.platform.request("sfp_tx_disable_n", 0).eq(1)
+            self.platform.add_platform_command("set_property SEVERITY {{Warning}} [get_drc_checks REQP-1753]")
+            if with_ethernet:
+                self.add_ethernet(phy=self.ethphy)
+            if with_etherbone:
+                self.add_etherbone(phy=self.ethphy, ip_address=eth_ip)
+
         # PCIe -------------------------------------------------------------------------------------
         if with_pcie:
-            self.pcie_phy = S7PCIEPHY(platform, platform.request("pcie_x4"),
+            self.pcie_phy = USPCIEPHY(platform, platform.request("pcie_x4"),
                 data_width = 128,
                 bar0_size  = 0x20000)
             self.add_pcie(phy=self.pcie_phy, ndmas=1)
 
-        # TODO verify / test
         # SATA -------------------------------------------------------------------------------------
         if with_sata:
             from litex.build.generic_platform import Subsignal, Pins
             from litesata.phy import LiteSATAPHY
 
+            # IOs
+            _sata_io = [
+                # SFP 2 SATA Adapter / https://shop.trenz-electronic.de/en/TE0424-01-SFP-2-SATA-Adapter
+                ("sfp2sata", 0,
+                    Subsignal("tx_p", Pins("U4")),
+                    Subsignal("tx_n", Pins("U3")),
+                    Subsignal("rx_p", Pins("T2")),
+                    Subsignal("rx_n", Pins("T1")),
+                ),
+            ]
+            platform.add_extension(_sata_io)
+
             # RefClk, Generate 150MHz from PLL.
             self.cd_sata_refclk = ClockDomain()
             self.crg.pll.create_clkout(self.cd_sata_refclk, 150e6)
             sata_refclk = ClockSignal("sata_refclk")
-            platform.add_platform_command("set_property SEVERITY {{Warning}} [get_drc_checks REQP-52]")
+            platform.add_platform_command("set_property SEVERITY {{Warning}} [get_drc_checks REQP-1753]")
 
             # PHY
             self.sata_phy = LiteSATAPHY(platform.device,
                 refclk     = sata_refclk,
-                pads       = platform.request("sata", 0),
+                pads       = platform.request("sfp2sata"),
                 gen        = "gen2",
                 clk_freq   = sys_clk_freq,
                 data_width = 16)
 
             # Core
             self.add_sata(phy=self.sata_phy, mode="read+write")
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
-                pads         = platform.request_all("user_led_n"),
+                pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
-        # I2C --------------------------------------------------------------------------------------
-        self.i2c = I2CMaster(platform.request("i2c"))
-
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=sitlinv_xc7k420t.Platform, description="LiteX SoC on AliExpress SITLINV FPGA Store XC7K420T")
-    parser.add_target_argument("--sys-clk-freq",    default=100e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--io-voltage",      default="3.3V",            help="IO voltage chosen by Jumper J3. Can be: '3.3V' or '2.5V'.")
-    parser.add_target_argument("--with-pcie",       action="store_true",       help="Enable PCIe support.")
-    parser.add_target_argument("--driver",          action="store_true",       help="Generate PCIe driver.")
-    parser.add_target_argument("--with-sata",       action="store_true",       help="Enable SATA support.")
+    parser = LiteXArgumentParser(platform=xilinx_kcu105.Platform, description="LiteX SoC on KCU105.")
+    parser.add_target_argument("--sys-clk-freq", default=125e6, type=float, help="System clock frequency.")
+    ethopts = parser.target_group.add_mutually_exclusive_group()
+    ethopts.add_argument("--with-ethernet",   action="store_true",    help="Enable Ethernet support.")
+    ethopts.add_argument("--with-etherbone",  action="store_true",    help="Enable Etherbone support.")
+    parser.add_target_argument("--eth-ip",    default="192.168.1.50", help="Ethernet/Etherbone IP address.")
+    parser.add_target_argument("--with-pcie", action="store_true",    help="Enable PCIe support.")
+    parser.add_target_argument("--driver",    action="store_true",    help="Generate PCIe driver.")
+    parser.add_target_argument("--with-sata", action="store_true",    help="Enable SATA support (over SFP2SATA).")
     args = parser.parse_args()
 
     soc = BaseSoC(
         sys_clk_freq   = args.sys_clk_freq,
-        io_voltage     = args.io_voltage,
+        with_ethernet  = args.with_ethernet,
+        with_etherbone = args.with_etherbone,
+        eth_ip         = args.eth_ip,
         with_pcie      = args.with_pcie,
         with_sata      = args.with_sata,
         **parser.soc_argdict
-    )
+	)
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
     if args.driver:
         generate_litepcie_software(soc, os.path.join(builder.output_dir, "driver"))
```

### Comparing `litex-boards-2023.12/litex_boards/targets/sqrl_acorn.py` & `litex-boards-2023.8/litex_boards/targets/sqrl_acorn.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,14 @@
                 phy           = self.ddrphy,
                 module        = MT41K512M16(sys_clk_freq, "1:4"),
                 l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
         # PCIe -------------------------------------------------------------------------------------
         if with_pcie:
-            self.comb += platform.request("pcie_clkreq_n").eq(0)
             self.pcie_phy = S7PCIEPHY(platform, platform.request("pcie_x4"),
                 data_width = 128,
                 bar0_size  = 0x20000)
             self.add_pcie(phy=self.pcie_phy, ndmas=1, address_width=64)
             platform.add_period_constraint(self.crg.cd_sys.clk, 1e9/sys_clk_freq)
 
             # ICAP (For FPGA reload over PCIe).
```

### Comparing `litex-boards-2023.12/litex_boards/targets/sqrl_fk33.py` & `litex-boards-2023.8/litex_boards/targets/sqrl_fk33.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,19 @@
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq, with_hbm)
 
         # SoCCore ----------------------------------------------------------------------------------
         if kwargs.get("uart_name", "serial") == "serial":
             kwargs["uart_name"] = "crossover" # Defaults to Crossover-UART.
-        kwargs["with_jtagbone"]  = True
-        kwargs["jtagbone_chain"] = 2 # Chain 1 already used by HBM2 debug probes.
         SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on FK33", **kwargs)
 
+        # JTAGBone --------------------------------------------------------------------------------
+        self.add_jtagbone(chain=2) # Chain 1 already used by HBM2 debug probes.
+
         # HBM --------------------------------------------------------------------------------------
         if with_hbm:
             # Add HBM Core.
             self.hbm = hbm = ClockDomainsRenamer({"axi": "sys"})(USPHBM2(platform))
 
             # Get HBM .xci.
             os.system("wget https://github.com/litex-hub/litex-boards/files/8178874/hbm_0.xci.txt")
```

### Comparing `litex-boards-2023.12/litex_boards/targets/sqrl_xcu1525.py` & `litex-boards-2023.8/litex_boards/targets/sqrl_xcu1525.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/terasic_de0nano.py` & `litex-boards-2023.8/litex_boards/targets/terasic_de0nano.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file is part of LiteX-Boards.
 #
 # Copyright (c) 2015-2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 # Build/Use:
 # ./terasic_de0nano.py --uart-name=jtag_uart --build --load
-# litex_term --jtag-config ../prog/openocd_usb_blaster.cfg jtag
+# litex_term --jtag-config ../prog/openocd_max10_blaster.cfg jtag
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
 from litex.build.io import DDROutput
```

### Comparing `litex-boards-2023.12/litex_boards/targets/terasic_de10lite.py` & `litex-boards-2023.8/litex_boards/targets/terasic_de10lite.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/terasic_de10nano.py` & `litex-boards-2023.8/litex_boards/targets/terasic_de10nano.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/terasic_de1soc.py` & `litex-boards-2023.8/litex_boards/targets/terasic_de1soc.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/terasic_de2_115.py` & `litex-boards-2023.8/litex_boards/targets/terasic_sockit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,159 +1,138 @@
 #!/usr/bin/env python3
-
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2015-2019 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2020 Hans Baier <hansfbaier@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
-from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex.build.io import DDROutput
-
-from litex_boards.platforms import terasic_de2_115
+from litex_boards.platforms import terasic_sockit
 
-from litex.soc.cores.clock import CycloneIVPLL
-from litex.soc.cores.led import LedChaser
-from litex.soc.integration.soc_core import *
+from litex.soc.cores.clock import CycloneVPLL
+from litex.soc.integration.soc_core  import *
 from litex.soc.integration.builder import *
+from litex.soc.cores.led import LedChaser
+from litex.soc.cores.video import VideoVGAPHY
 
-from litedram.modules import IS42S16320
-from litedram.phy import GENSDRPHY
+from litex.build.io import DDROutput
 
-from liteeth.phy.mii import LiteEthPHYMII
+from litedram.modules import W9825G6KH6, AS4C32M16
+from litedram.phy import HalfRateGENSDRPHY, GENSDRPHY
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq):
-        self.rst       = Signal()
-        self.cd_sys    = ClockDomain()
-        self.cd_sys_ps = ClockDomain()
-
-        # # #
+    def __init__(self, platform, sys_clk_freq, with_sdram=False, sdram_rate="1:2", with_video_terminal=False):
+        self.sdram_rate = sdram_rate
+        self.rst    = Signal()
+        self.cd_sys = ClockDomain()
+        if with_video_terminal:
+            self.cd_vga = ClockDomain()
+        if with_sdram:
+            if sdram_rate == "1:2":
+                self.cd_sys2x    = ClockDomain()
+                self.cd_sys2x_ps = ClockDomain()
+            else:
+                self.cd_sys_ps = ClockDomain()
 
         # Clk / Rst
         clk50 = platform.request("clk50")
 
         # PLL
-        self.pll = pll = CycloneIVPLL(speedgrade="-7")
+        self.pll = pll = CycloneVPLL(speedgrade="-C6")
         self.comb += pll.reset.eq(self.rst)
         pll.register_clkin(clk50, 50e6)
-        pll.create_clkout(self.cd_sys,    sys_clk_freq)
-        pll.create_clkout(self.cd_sys_ps, sys_clk_freq, phase=90)
+        pll.create_clkout(self.cd_sys, sys_clk_freq)
+
+        if with_video_terminal:
+            pll.create_clkout(self.cd_vga, 65e6)
+
+        if with_sdram:
+            if sdram_rate == "1:2":
+                pll.create_clkout(self.cd_sys2x,    2*sys_clk_freq)
+                pll.create_clkout(self.cd_sys2x_ps, 2*sys_clk_freq, phase=180)  # Idealy 90° but needs to be increased.
+            else:
+                pll.create_clkout(self.cd_sys_ps, sys_clk_freq, phase=90)
 
         # SDRAM clock
-        self.specials += DDROutput(1, 0, platform.request("sdram_clock"), ClockSignal("sys_ps"))
+        if with_sdram:
+            sdram_clk = ClockSignal("sys2x_ps" if sdram_rate == "1:2" else "sys_ps")
+            self.specials += DDROutput(1, 0, platform.request("sdram_clock"), sdram_clk)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=50e6,
-        with_ethernet   = False,
-        with_etherbone  = False,
-        with_sdcard     = False,
-        with_led_chaser = True,
-        ethernet_phy    = 0,
-        etherbone_ip    = "192.168.1.50",
-        etherbone_phy   = 1,
-        **kwargs,
-    ):
-        platform = terasic_de2_115.Platform()
+    def __init__(self, sys_clk_freq=50e6, revision="revd", sdram_rate="1:2", mister_sdram=None,
+        with_led_chaser     = True,
+        with_video_terminal = False,
+        **kwargs):
+        platform = terasic_sockit.Platform(revision)
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = _CRG(platform, sys_clk_freq)
+        self.crg = _CRG(platform, sys_clk_freq,
+            with_sdram          = mister_sdram != None,
+            sdram_rate          = sdram_rate,
+            with_video_terminal = with_video_terminal
+        )
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on DE2-115", **kwargs)
+        if kwargs.get("uart_name", "serial") == "serial":
+            kwargs["uart_name"] = "jtag_uart" # Defaults to JTAG-UART.
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on the Terasic SoCKit", **kwargs)
 
         # SDR SDRAM --------------------------------------------------------------------------------
-        if not self.integrated_main_ram_size:
-            self.sdrphy = GENSDRPHY(platform.request("sdram"), sys_clk_freq)
+        if mister_sdram is not None:
+            sdrphy_cls = HalfRateGENSDRPHY if sdram_rate == "1:2" else GENSDRPHY
+            sdrphy_mod = {"xs_v22": W9825G6KH6, "xs_v24": AS4C32M16}[mister_sdram]
+            self.sdrphy = sdrphy_cls(platform.request("sdram"), sys_clk_freq)
             self.add_sdram("sdram",
                 phy           = self.sdrphy,
-                module        = IS42S16320(self.clk_freq, "1:1"),
+                module        = sdrphy_mod(sys_clk_freq, sdram_rate),
                 l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
-        # Add debug interface if the CPU has one ---------------------------------------------------
-        if hasattr(self.cpu, "debug_bus"):
-            self.register_mem(
-                name      = "vexriscv_debug",
-                address   = 0xF00F0000,
-                interface = self.cpu.debug_bus,
-                size      = 0x100,
-            )
+        # Video Terminal ---------------------------------------------------------------------------
+        if with_video_terminal:
+            vga_pads = platform.request("vga")
+            self.comb += [ vga_pads.sync_n.eq(0), vga_pads.blank_n.eq(1) ]
+            self.specials += DDROutput(i1=1, i2=0, o=vga_pads.clk, clk=ClockSignal("vga"))
+            self.videophy = VideoVGAPHY(vga_pads, clock_domain="vga")
+            self.add_video_terminal(phy=self.videophy, timings="1024x768@60Hz", clock_domain="vga")
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
-                pads = platform.request_all("user_led"), sys_clk_freq=sys_clk_freq
-            )
-            self.leds.add_pwm()
-
-        # SD Card ----------------------------------------------------------------------------------
-        if with_sdcard:
-            self.add_sdcard()
-
-        # Ethernet ---------------------------------------------------------------------------------
-        if with_ethernet:
-            # Ethernet PHY
-            self.submodules.ethphy = LiteEthPHYMII(
-                clock_pads = platform.request("eth_clocks", ethernet_phy),
-                pads       = platform.request("eth", ethernet_phy),
-            )
-            self.add_ethernet(
-                phy        = self.ethphy,
-                phy_cd     = "ethphy_eth" if with_etherbone else "eth",
-                dynamic_ip = True,
-            )
-        if with_etherbone:
-            # Ethernet PHY
-            self.submodules.ethbphy = LiteEthPHYMII(
-                clock_pads = platform.request("eth_clocks", etherbone_phy),
-                pads       = platform.request("eth", etherbone_phy),
-            )
-            self.add_etherbone(
-                phy        = self.ethbphy,
-                phy_cd     = "ethbphy_eth" if with_ethernet else "eth",
-                ip_address = etherbone_ip,
-            )
+                pads         = platform.request_all("user_led"),
+                sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=terasic_de2_115.Platform, description="LiteX SoC on DE2-115.")
-
-    parser.add_target_argument("--sys-clk-freq",    default=50e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--with-led-chaser", action="store_true",      help="Enable LED chaser.")
-    parser.add_target_argument("--with-sdcard",     action="store_true",      help="Enable SD card support.")
-    parser.add_target_argument("--with-ethernet",   action="store_true",      help="Enable Ethernet support.")
-    parser.add_target_argument("--with-etherbone",  action="store_true",      help="Enable Etherbone support.")
-    parser.add_target_argument("--etherbone-ip",    default="192.168.48.100", help="Etherbone IP address.")
-    parser.add_target_argument("--etherbone-phy",   default=1, type=int,      help="Etherbone PHY (0 or 1).")
-    parser.add_target_argument("--ethernet-phy",    default=0, type=int,      help="Ethernet  PHY (0 or 1).")
+    parser = LiteXArgumentParser(platform=terasic_sockit.Platform, description="LiteX SoC on the Terasic SoCKit.")
+    parser.add_target_argument("--single-rate-sdram",   action="store_true",      help="Clock SDRAM with 1x the sytem clock (instead of 2x).")
+    parser.add_target_argument("--mister-sdram-xs-v22", action="store_true",      help="Use optional MiSTer SDRAM module XS v2.2 on J2 on GPIO daughter card.")
+    parser.add_target_argument("--mister-sdram-xs-v24", action="store_true",      help="Use optional MiSTer SDRAM module XS v2.4 on J2 on GPIO daughter card.")
+    parser.add_target_argument("--revision",            default="revd",           help="Board revision (revb, revc or revd).")
+    parser.add_target_argument("--sys-clk-freq",        default=50e6, type=float, help="System clock frequency.")
+    parser.add_target_argument("--with-video-terminal", action="store_true",      help="Enable Video Terminal (VGA).")
     args = parser.parse_args()
 
     soc = BaseSoC(
-        sys_clk_freq    = args.sys_clk_freq,
-        with_sdcard     = args.with_sdcard,
-        with_ethernet   = args.with_ethernet,
-        with_etherbone  = args.with_etherbone,
-        with_led_chaser = args.with_led_chaser,
-        etherbone_ip    = args.etherbone_ip,
-        etherbone_phy   = args.etherbone_phy,
-        ethernet_phy    = args.ethernet_phy,
-        **parser.soc_argdict,
+        sys_clk_freq        = args.sys_clk_freq,
+        revision            = args.revision,
+        sdram_rate          = "1:1" if args.single_rate_sdram else "1:2",
+        mister_sdram        = "xs_v22" if args.mister_sdram_xs_v22 else "xs_v24" if args.mister_sdram_xs_v24 else None,
+        with_video_terminal = args.with_video_terminal,
+        **parser.soc_argdict
     )
-
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
     if args.load:
         prog = soc.platform.create_programmer()
         prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `litex-boards-2023.12/litex_boards/targets/terasic_deca.py` & `litex-boards-2023.8/litex_boards/targets/terasic_deca.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This file is part of LiteX-Boards.
 #
 # Copyright (c) 2019 msloniewski <marcin.sloniewski@gmail.com>
 # SPDX-License-Identifier: BSD-2-Clause
 
 # Build/Use:
 # ./terasic_deca.py --uart-name jtag_uart --build --load
-# litex_term --jtag-config ../prog/openocd_usb_blaster2.cfg jtag
+# litex_term --jtag-config ../prog/openocd_max10_blaster2.cfg jtag
 
 from migen import *
 from litex_boards.platforms import terasic_deca
 
 from litex.gen import *
 
 from litex.soc.cores.clock import Max10PLL
@@ -54,14 +54,16 @@
             pll.create_clkout(self.cd_usb, 60e6, phase=-120) # -120° from DECA's example (also validated with LUNA).
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
     def __init__(self, sys_clk_freq=50e6,
         with_led_chaser     = True,
+        with_uartbone       = False,
+        with_jtagbone       = False,
         with_video_terminal = False,
         with_spi_sdcard     = False,
         with_ethernet       = False,
         with_etherbone      = False,
         eth_ip              = "192.168.1.50",
         eth_dynamic_ip      = False,
         **kwargs):
@@ -70,22 +72,30 @@
         # CRG --------------------------------------------------------------------------------------
         self.crg = self.crg = _CRG(platform, sys_clk_freq, with_usb_pll=False)
 
         # SoCCore ----------------------------------------------------------------------------------
         # Defaults to JTAG-UART since no hardware UART.
         real_uart_name = kwargs["uart_name"]
         if real_uart_name == "serial":
-            if kwargs["with_jtagbone"]:
+            if with_jtagbone:
                 kwargs["uart_name"] = "crossover"
             else:
                 kwargs["uart_name"] = "jtag_uart"
-        if kwargs["with_uartbone"]:
+        if with_uartbone:
             kwargs["uart_name"] = "crossover"
         SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Terasic DECA", **kwargs)
 
+        # UARTbone ---------------------------------------------------------------------------------
+        if with_uartbone:
+            self.add_uartbone(uart_name=real_uart_name, baudrate=kwargs["uart_baudrate"])
+
+        # JTAGbone ---------------------------------------------------------------------------------
+        if with_jtagbone:
+            self.add_jtagbone()
+
         # Ethernet ---------------------------------------------------------------------------------
         if with_ethernet or with_etherbone:
             self.platform.toolchain.additional_sdc_commands += [
                 'create_clock -name eth_rx_clk -period 40.0 [get_ports {eth_clocks_rx}]',
                 'create_clock -name eth_tx_clk -period 40.0 [get_ports {eth_clocks_tx}]',
                 'set_false_path -from [get_clocks {sys_clk}] -to [get_clocks {eth_rx_clk}]',
                 'set_false_path -from [get_clocks {sys_clk}] -to [get_clocks {eth_tx_clk}]',
@@ -135,24 +145,28 @@
     parser = LiteXArgumentParser(platform=terasic_deca.Platform, description="LiteX SoC on DECA.")
     parser.add_target_argument("--sys-clk-freq", default=50e6, type=float, help="System clock frequency.")
     ethopts = parser.target_group.add_mutually_exclusive_group()
     ethopts.add_argument("--with-ethernet",             action="store_true",    help="Enable Ethernet support.")
     ethopts.add_argument("--with-etherbone",            action="store_true",    help="Enable Etherbone support.")
     parser.add_target_argument("--eth-ip",              default="192.168.1.50", help="Ethernet/Etherbone IP address.")
     parser.add_target_argument("--eth-dynamic-ip",      action="store_true",    help="Enable dynamic Ethernet IP addresses setting.")
+    parser.add_target_argument("--with-uartbone",       action="store_true",    help="Enable UARTbone support.")
+    parser.add_target_argument("--with-jtagbone",       action="store_true",    help="Enable JTAGbone support.")
     parser.add_target_argument("--with-video-terminal", action="store_true",    help="Enable Video Terminal (VGA).")
     parser.add_target_argument("--with-spi-sdcard",     action="store_true",    help="Enable SPI SD card controller.")
     args = parser.parse_args()
 
     soc = BaseSoC(
         sys_clk_freq        = args.sys_clk_freq,
         with_ethernet       = args.with_ethernet,
         with_etherbone      = args.with_etherbone,
         eth_ip              = args.eth_ip,
         eth_dynamic_ip      = args.eth_dynamic_ip,
+        with_uartbone       = args.with_uartbone,
+        with_jtagbone       = args.with_jtagbone,
         with_video_terminal = args.with_video_terminal,
         with_spi_sdcard     = args.with_spi_sdcard,
         **parser.soc_argdict
     )
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
```

### Comparing `litex-boards-2023.12/litex_boards/targets/terasic_sockit.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_alveo_u200.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,141 +1,131 @@
 #!/usr/bin/env python3
+
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2020 Hans Baier <hansfbaier@gmail.com>
+# Copyright (c) 2023 Do Viet Thanh <thanhdv@soc.one>
+# Copyright (c) 2020 Fei Gao <feig@princeton.edu>
+# Copyright (c) 2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2020 David Shah <dave@ds0.me>
 # SPDX-License-Identifier: BSD-2-Clause
 
+import os
+
 from migen import *
+from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex_boards.platforms import terasic_sockit
+from litex_boards.platforms import xilinx_alveo_u200
 
-from litex.soc.cores.clock import CycloneVPLL
-from litex.soc.integration.soc_core  import *
+from litex.soc.cores.clock import *
+from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
-from litex.soc.cores.led import LedChaser
-from litex.soc.cores.video import VideoVGAPHY
 
-from litex.build.io import DDROutput
+from litex.soc.cores.led import LedChaser
+from litedram.modules import MTA18ASF2G72PZ
+from litedram.phy import usddrphy
 
-from litedram.modules import W9825G6KH6, AS4C32M16
-from litedram.phy import HalfRateGENSDRPHY, GENSDRPHY
+from litepcie.phy.usppciephy import USPPCIEPHY
+from litepcie.software import generate_litepcie_software
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq, with_sdram=False, sdram_rate="1:2", with_video_terminal=False):
-        self.sdram_rate = sdram_rate
-        self.rst    = Signal()
-        self.cd_sys = ClockDomain()
-        if with_video_terminal:
-            self.cd_vga = ClockDomain()
-        if with_sdram:
-            if sdram_rate == "1:2":
-                self.cd_sys2x    = ClockDomain()
-                self.cd_sys2x_ps = ClockDomain()
-            else:
-                self.cd_sys_ps = ClockDomain()
+    def __init__(self, platform, sys_clk_freq):
+        self.rst       = Signal()
+        self.cd_sys    = ClockDomain()
+        self.cd_sys4x  = ClockDomain()
+        self.cd_pll4x  = ClockDomain()
+        self.cd_idelay = ClockDomain()
 
-        # Clk / Rst
-        clk50 = platform.request("clk50")
+        # # #
 
-        # PLL
-        self.pll = pll = CycloneVPLL(speedgrade="-C6")
+        self.pll = pll = USMMCM(speedgrade=-2)
         self.comb += pll.reset.eq(self.rst)
-        pll.register_clkin(clk50, 50e6)
-        pll.create_clkout(self.cd_sys, sys_clk_freq)
+        pll.register_clkin(platform.request("clk300", 0), 300e6)
+        pll.create_clkout(self.cd_pll4x, sys_clk_freq*4, buf=None, with_reset=False)
+        pll.create_clkout(self.cd_idelay, 500e6)
+        platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
+
+        self.specials += [
+            Instance("BUFGCE_DIV",
+                p_BUFGCE_DIVIDE=4,
+                i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys.clk),
+            Instance("BUFGCE",
+                i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys4x.clk),
+        ]
 
-        if with_video_terminal:
-            pll.create_clkout(self.cd_vga, 65e6)
-
-        if with_sdram:
-            if sdram_rate == "1:2":
-                pll.create_clkout(self.cd_sys2x,    2*sys_clk_freq)
-                pll.create_clkout(self.cd_sys2x_ps, 2*sys_clk_freq, phase=180)  # Idealy 90° but needs to be increased.
-            else:
-                pll.create_clkout(self.cd_sys_ps, sys_clk_freq, phase=90)
-
-        # SDRAM clock
-        if with_sdram:
-            sdram_clk = ClockSignal("sys2x_ps" if sdram_rate == "1:2" else "sys_ps")
-            self.specials += DDROutput(1, 0, platform.request("sdram_clock"), sdram_clk)
+        self.idelayctrl = USIDELAYCTRL(cd_ref=self.cd_idelay, cd_sys=self.cd_sys)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=50e6, revision="revd", sdram_rate="1:2", mister_sdram=None,
-        with_led_chaser     = True,
-        with_video_terminal = False,
-        **kwargs):
-        platform = terasic_sockit.Platform(revision)
+    def __init__(self, sys_clk_freq=125e6, with_led_chaser=True, with_pcie=False, **kwargs):
+        platform = xilinx_alveo_u200.Platform()
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = _CRG(platform, sys_clk_freq,
-            with_sdram          = mister_sdram != None,
-            sdram_rate          = sdram_rate,
-            with_video_terminal = with_video_terminal
-        )
+        self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        if kwargs.get("uart_name", "serial") == "serial":
-            kwargs["uart_name"] = "jtag_uart" # Defaults to JTAG-UART.
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on the Terasic SoCKit", **kwargs)
-
-        # SDR SDRAM --------------------------------------------------------------------------------
-        if mister_sdram is not None:
-            sdrphy_cls = HalfRateGENSDRPHY if sdram_rate == "1:2" else GENSDRPHY
-            sdrphy_mod = {"xs_v22": W9825G6KH6, "xs_v24": AS4C32M16}[mister_sdram]
-            self.sdrphy = sdrphy_cls(platform.request("sdram"), sys_clk_freq)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Alveo U200", **kwargs)
+
+        # DDR4 SDRAM -------------------------------------------------------------------------------
+        if not self.integrated_main_ram_size:
+            self.ddrphy = usddrphy.USPDDRPHY(platform.request("ddram"),
+                memtype          = "DDR4",
+                sys_clk_freq     = sys_clk_freq,
+                cmd_latency      = 1,
+                iodelay_clk_freq = 500e6,
+                is_rdimm         = True)
             self.add_sdram("sdram",
-                phy           = self.sdrphy,
-                module        = sdrphy_mod(sys_clk_freq, sdram_rate),
+                phy           = self.ddrphy,
+                module        = MTA18ASF2G72PZ(sys_clk_freq, "1:4"),
+                size          = 0x40000000,
                 l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
-        # Video Terminal ---------------------------------------------------------------------------
-        if with_video_terminal:
-            vga_pads = platform.request("vga")
-            self.comb += [ vga_pads.sync_n.eq(0), vga_pads.blank_n.eq(1) ]
-            self.specials += DDROutput(i1=1, i2=0, o=vga_pads.clk, clk=ClockSignal("vga"))
-            self.videophy = VideoVGAPHY(vga_pads, clock_domain="vga")
-            self.add_video_terminal(phy=self.videophy, timings="1024x768@60Hz", clock_domain="vga")
+        # Firmware RAM (To ease initial LiteDRAM calibration support) ------------------------------
+        self.add_ram("firmware_ram", 0x20000000, 0x8000)
+
+        # PCIe -------------------------------------------------------------------------------------
+        if with_pcie:
+            self.pcie_phy = USPPCIEPHY(platform, platform.request("pcie_x4"),
+                data_width = 128,
+                bar0_size  = 0x20000)
+            self.add_pcie(phy=self.pcie_phy, ndmas=1)
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=terasic_sockit.Platform, description="LiteX SoC on the Terasic SoCKit.")
-    parser.add_target_argument("--single-rate-sdram",   action="store_true",      help="Clock SDRAM with 1x the sytem clock (instead of 2x).")
-    parser.add_target_argument("--mister-sdram-xs-v22", action="store_true",      help="Use optional MiSTer SDRAM module XS v2.2 on J2 on GPIO daughter card.")
-    parser.add_target_argument("--mister-sdram-xs-v24", action="store_true",      help="Use optional MiSTer SDRAM module XS v2.4 on J2 on GPIO daughter card.")
-    parser.add_target_argument("--revision",            default="revd",           help="Board revision (revb, revc or revd).")
-    parser.add_target_argument("--sys-clk-freq",        default=50e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--with-video-terminal", action="store_true",      help="Enable Video Terminal (VGA).")
+    parser = LiteXArgumentParser(platform=xilinx_alveo_u200.Platform, description="LiteX SoC on Alveo U200.")
+    parser.add_target_argument("--sys-clk-freq", default=125e6, type=float, help="System clock frequency.")
+    parser.add_target_argument("--with-pcie",    action="store_true",       help="Enable PCIe support.")
+    parser.add_target_argument("--driver",       action="store_true",       help="Generate PCIe driver.")
     args = parser.parse_args()
 
     soc = BaseSoC(
-        sys_clk_freq        = args.sys_clk_freq,
-        revision            = args.revision,
-        sdram_rate          = "1:1" if args.single_rate_sdram else "1:2",
-        mister_sdram        = "xs_v22" if args.mister_sdram_xs_v22 else "xs_v24" if args.mister_sdram_xs_v24 else None,
-        with_video_terminal = args.with_video_terminal,
+        sys_clk_freq = args.sys_clk_freq,
+        with_pcie    = args.with_pcie,
         **parser.soc_argdict
     )
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
+    if args.driver:
+        generate_litepcie_software(soc, os.path.join(builder.output_dir, "driver"))
+
     if args.load:
         prog = soc.platform.create_programmer()
         prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `litex-boards-2023.12/litex_boards/targets/tinyfpga_bx.py` & `litex-boards-2023.8/litex_boards/targets/tinyfpga_bx.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/trellisboard.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_alveo_u280.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,214 +1,199 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2019 David Shah <dave@ds0.me>
+# Copyright (c) 2021 Sergiu Mosanu <sm7ed@virginia.edu>
+# Copyright (c) 2020-2021 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2020 Antmicro <www.antmicro.com>
+#
 # SPDX-License-Identifier: BSD-2-Clause
 
+# To interface via the serial port use:
+#     lxterm /dev/ttyUSBx --speed=115200
+
+import os
+
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex_boards.platforms import trellisboard
+from litex_boards.platforms import xilinx_alveo_u280
 
 from litex.soc.cores.clock import *
 from litex.soc.integration.soc_core import *
+from litex.soc.integration.soc import SoCRegion
 from litex.soc.integration.builder import *
+from litex.soc.interconnect.axi import *
+from litex.soc.interconnect.csr import *
+from litex.soc.cores.ram.xilinx_usp_hbm2 import USPHBM2
+
 from litex.soc.cores.led import LedChaser
-from litex.soc.cores.gpio import GPIOTristate
-from litex.soc.cores.video import VideoDVIPHY
-from litex.soc.cores.bitbang import I2CMaster
+from litedram.modules import MTA18ASF2G72PZ
+from litedram.phy import usddrphy
+
+from litepcie.phy.usppciephy import USPPCIEPHY
+from litepcie.software import generate_litepcie_software
 
-from litedram.modules import MT41J256M16
-from litedram.phy import ECP5DDRPHY
+from litedram.common import *
+from litedram.frontend.axi import *
 
-from liteeth.phy.ecp5rgmii import LiteEthPHYRGMII
+from litescope import LiteScopeAnalyzer
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq):
-        self.rst    = Signal()
-        self.cd_por = ClockDomain()
-        self.cd_sys = ClockDomain()
-
-        # # #
-
-        # Clk / Rst
-        clk12 = platform.request("clk12")
-        rst   = platform.request("user_btn", 0)
-
-        # Power on reset
-        por_count = Signal(16, reset=2**16-1)
-        por_done  = Signal()
-        self.comb += self.cd_por.clk.eq(clk12)
-        self.comb += por_done.eq(por_count == 0)
-        self.sync.por += If(~por_done, por_count.eq(por_count - 1))
-
-        # PLL
-        self.pll = pll = ECP5PLL()
-        self.comb += pll.reset.eq(~por_done | rst | self.rst)
-        pll.register_clkin(clk12, 12e6)
-        pll.create_clkout(self.cd_sys, sys_clk_freq)
-
-
-class _CRGSDRAM(LiteXModule):
-    def __init__(self, platform, sys_clk_freq):
-        self.rst        = Signal()
-        self.cd_init    = ClockDomain()
-        self.cd_por     = ClockDomain()
-        self.cd_sys     = ClockDomain()
-        self.cd_sys2x   = ClockDomain()
-        self.cd_sys2x_i = ClockDomain()
+    def __init__(self, platform, sys_clk_freq, ddram_channel, with_hbm):
+        if with_hbm:
+            self.rst        = Signal()
+            self.cd_sys     = ClockDomain()
+            self.cd_hbm_ref = ClockDomain()
+            self.cd_apb     = ClockDomain()
+        else: # ddr4
+            self.rst = Signal()
+            self.cd_sys    = ClockDomain()
+            self.cd_sys4x  = ClockDomain()
+            self.cd_pll4x  = ClockDomain()
+            self.cd_idelay = ClockDomain()
 
         # # #
 
-        self.stop  = Signal()
-        self.reset = Signal()
-
-        # Clk / Rst
-        clk12 = platform.request("clk12")
-        rst   = platform.request("user_btn", 0)
-
-        # Power on reset
-        por_count = Signal(16, reset=2**16-1)
-        por_done  = Signal()
-        self.comb += self.cd_por.clk.eq(clk12)
-        self.comb += por_done.eq(por_count == 0)
-        self.sync.por += If(~por_done, por_count.eq(por_count - 1))
-
-        # PLL
-        sys2x_clk_ecsout = Signal()
-        self.pll = pll = ECP5PLL()
-        self.comb += pll.reset.eq(~por_done | rst | self.rst)
-        pll.register_clkin(clk12, 12e6)
-        pll.create_clkout(self.cd_sys2x_i, 2*sys_clk_freq)
-        pll.create_clkout(self.cd_init,   25e6)
-        self.specials += [
-            Instance("ECLKBRIDGECS",
-                i_CLK0   = self.cd_sys2x_i.clk,
-                i_SEL    = 0,
-                o_ECSOUT = sys2x_clk_ecsout,
-            ),
-            Instance("ECLKSYNCB",
-                i_ECLKI = sys2x_clk_ecsout,
-                i_STOP  = self.stop,
-                o_ECLKO = self.cd_sys2x.clk),
-            Instance("CLKDIVF",
-                p_DIV     = "2.0",
-                i_ALIGNWD = 0,
-                i_CLKI    = self.cd_sys2x.clk,
-                i_RST     = self.reset,
-                o_CDIVX   = self.cd_sys.clk),
-            AsyncResetSynchronizer(self.cd_sys, ~pll.locked | self.reset),
-        ]
+        if with_hbm:
+            self.pll = pll = USMMCM(speedgrade=-2)
+            self.comb += pll.reset.eq(self.rst)
+            pll.register_clkin(platform.request("sysclk", ddram_channel), 100e6)
+            pll.create_clkout(self.cd_sys,     sys_clk_freq)
+            pll.create_clkout(self.cd_hbm_ref, 100e6)
+            pll.create_clkout(self.cd_apb,     100e6)
+            platform.add_false_path_constraints(self.cd_sys.clk, self.cd_apb.clk)
+        else: # ddr4
+            self.pll = pll = USMMCM(speedgrade=-2)
+            self.comb += pll.reset.eq(self.rst)
+            pll.register_clkin(platform.request("sysclk", ddram_channel), 100e6)
+            pll.create_clkout(self.cd_pll4x, sys_clk_freq*4, buf=None, with_reset=False)
+            pll.create_clkout(self.cd_idelay, 600e6) #, with_reset=False
+            platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
+
+            self.specials += [
+                Instance("BUFGCE_DIV",
+                    p_BUFGCE_DIVIDE=4,
+                    i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys.clk),
+                Instance("BUFGCE",
+                    i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys4x.clk),
+                # AsyncResetSynchronizer(self.cd_idelay, ~pll.locked),
+            ]
 
-        self.comb += platform.request("dram_vtt_en").eq(1)
+            self.idelayctrl = USIDELAYCTRL(cd_ref=self.cd_idelay, cd_sys=self.cd_sys)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=75e6, toolchain="trellis",
-        with_ethernet          = False,
-        with_video_terminal    = False,
-        with_video_framebuffer = False,
-        with_led_chaser        = True,
-        with_pmod_gpio         = False,
+    def __init__(self, sys_clk_freq=150e6, ddram_channel=0,
+        with_pcie       = False,
+        with_led_chaser = False,
+        with_hbm        = False,
         **kwargs):
-        platform = trellisboard.Platform(toolchain=toolchain)
+        platform = xilinx_alveo_u280.Platform()
+        if with_hbm:
+            assert 225e6 <= sys_clk_freq <= 450e6
 
         # CRG --------------------------------------------------------------------------------------
-        crg_cls = _CRGSDRAM if kwargs.get("integrated_main_ram_size", 0) == 0 else _CRG
-        self.crg = crg_cls(platform, sys_clk_freq)
+        self.crg = _CRG(platform, sys_clk_freq, ddram_channel, with_hbm)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Trellis Board", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Alveo U280 (ES1)", **kwargs)
 
-        # DDR3 SDRAM -------------------------------------------------------------------------------
-        if not self.integrated_main_ram_size:
-            self.ddrphy = ECP5DDRPHY(
-                platform.request("ddram"),
-                sys_clk_freq=sys_clk_freq)
-            self.comb += self.crg.stop.eq(self.ddrphy.init.stop)
-            self.comb += self.crg.reset.eq(self.ddrphy.init.reset)
-            self.add_sdram("sdram",
-                phy           = self.ddrphy,
-                module        = MT41J256M16(sys_clk_freq, "1:2"),
-                l2_cache_size = kwargs.get("l2_size", 8192),
-            )
-
-        # Ethernet ---------------------------------------------------------------------------------
-        if with_ethernet:
-            self.ethphy = LiteEthPHYRGMII(
-                clock_pads = self.platform.request("eth_clocks"),
-                pads       = self.platform.request("eth"))
-            self.add_ethernet(phy=self.ethphy)
-
-        # HDMI -------------------------------------------------------------------------------------
-        if with_video_terminal or with_video_framebuffer:
-            # PHY + TP410 I2C initialization.
-            hdmi_pads = platform.request("hdmi")
-            self.videophy = VideoDVIPHY(hdmi_pads, clock_domain="init")
-            self.videoi2c = I2CMaster(hdmi_pads)
-            self.videoi2c.add_init(addr=0x38, init=[
-                (0x08, 0x35) # CTL_1_MODE: Normal operation, 24-bit, HSYNC/VSYNC.
-            ])
-
-            # Video Terminal/Framebuffer.
-            if with_video_terminal:
-                self.add_video_terminal(phy=self.videophy, timings="640x480@75Hz", clock_domain="init")
-            if with_video_framebuffer:
-                self.add_video_framebuffer(phy=self.videophy, timings="640x480@75Hz", clock_domain="init")
+        # HBM / DRAM -------------------------------------------------------------------------------
+        if with_hbm:
+            # JTAGBone -----------------------------------------------------------------------------
+            #self.add_jtagbone(chain=2) # Chain 1 already used by HBM2 debug probes.
+
+            # Add HBM Core.
+            self.hbm = hbm = ClockDomainsRenamer({"axi": "sys"})(USPHBM2(platform))
+
+            # Get HBM .xci.
+            os.system("wget https://github.com/litex-hub/litex-boards/files/6893157/hbm_0.xci.txt")
+            os.makedirs("ip/hbm", exist_ok=True)
+            os.system("mv hbm_0.xci.txt ip/hbm/hbm_0.xci")
+
+            # Connect four of the HBM's AXI interfaces to the main bus of the SoC.
+            for i in range(4):
+                axi_hbm      = hbm.axi[i]
+                axi_lite_hbm = AXILiteInterface(data_width=256, address_width=33)
+                self.submodules += AXILite2AXI(axi_lite_hbm, axi_hbm)
+                self.bus.add_slave(f"hbm{i}", axi_lite_hbm, SoCRegion(origin=0x4000_0000 + 0x1000_0000*i, size=0x1000_0000)) # 256MB.
+            # Link HBM2 channel 0 as main RAM
+            self.bus.add_region("main_ram", SoCRegion(origin=0x4000_0000, size=0x1000_0000, linker=True)) # 256MB.
+
+        else:
+            # DDR4 SDRAM -------------------------------------------------------------------------------
+            if not self.integrated_main_ram_size:
+                self.ddrphy = usddrphy.USPDDRPHY(platform.request("ddram", ddram_channel),
+                    memtype          = "DDR4",
+                    cmd_latency      = 1, # seems to work better with cmd_latency=1
+                    sys_clk_freq     = sys_clk_freq,
+                    iodelay_clk_freq = 600e6,
+                    is_rdimm         = True)
+                self.add_sdram("sdram",
+                    phy           = self.ddrphy,
+                    module        = MTA18ASF2G72PZ(sys_clk_freq, "1:4"),
+                    size          = 0x40000000,
+                    l2_cache_size = kwargs.get("l2_size", 8192)
+                )
+
+            # Firmware RAM (To ease initial LiteDRAM calibration support) --------------------------
+            self.add_ram("firmware_ram", 0x20000000, 0x8000)
+
+        # PCIe -------------------------------------------------------------------------------------
+        if with_pcie:
+            self.pcie_phy = USPPCIEPHY(platform, platform.request("pcie_x4"),
+                data_width = 128,
+                bar0_size  = 0x20000)
+            self.add_pcie(phy=self.pcie_phy, ndmas=1)
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
-                pads         = platform.request_all("user_led"),
+                pads         = platform.request_all("gpio_led"),
                 sys_clk_freq = sys_clk_freq)
 
-        # GPIOs ------------------------------------------------------------------------------------
-        if with_pmod_gpio:
-            platform.add_extension(trellisboard.raw_pmod_io("pmoda"))
-            self.gpio = GPIOTristate(platform.request("pmoda"))
-
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=trellisboard.Platform, description="LiteX SoC on Trellis Board.")
-    parser.add_target_argument("--sys-clk-freq",    default=75e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--with-ethernet",   action="store_true",      help="Enable Ethernet support.")
-    viopts = parser.target_group.add_mutually_exclusive_group()
-    viopts.add_argument("--with-video-terminal",    action="store_true", help="Enable Video Terminal (HDMI).")
-    viopts.add_argument("--with-video-framebuffer", action="store_true", help="Enable Video Framebuffer (HDMI).")
-    sdopts = parser.target_group.add_mutually_exclusive_group()
-    sdopts.add_argument("--with-spi-sdcard",       action="store_true", help="Enable SPI-mode SDCard support.")
-    sdopts.add_argument("--with-sdcard",           action="store_true", help="Enable SDCard support.")
-    parser.add_target_argument("--with-pmod-gpio", action="store_true", help="Enable GPIOs through PMOD.") # FIXME: Temporary test.
+    parser = LiteXArgumentParser(platform=xilinx_alveo_u280.Platform, description="LiteX SoC on Alveo U280.")
+    parser.add_target_argument("--sys-clk-freq",    default=150e6, type=float, help="System clock frequency.") # HBM2 with 250MHz, DDR4 with 150MHz (1:4)
+    parser.add_target_argument("--ddram-channel",   default="0",               help="DDRAM channel (0, 1, 2 or 3).") # also selects clk 0 or 1
+    parser.add_target_argument("--with-pcie",       action="store_true",       help="Enable PCIe support.")
+    parser.add_target_argument("--driver",          action="store_true",       help="Generate PCIe driver.")
+    parser.add_target_argument("--with-hbm",        action="store_true",       help="Use HBM2.")
+    parser.add_target_argument("--with-analyzer",   action="store_true",       help="Enable Analyzer.")
+    parser.add_target_argument("--with-led-chaser", action="store_true",       help="Enable LED Chaser.")
     args = parser.parse_args()
 
+    if args.with_hbm:
+        args.sys_clk_freq = 250e6
+
     soc = BaseSoC(
-        sys_clk_freq           = args.sys_clk_freq,
-        toolchain              = args.toolchain,
-        with_ethernet          = args.with_ethernet,
-        with_video_terminal    = args.with_video_terminal,
-        with_video_framebuffer = args.with_video_framebuffer,
-        with_pmod_gpio         = args.with_pmod_gpio,
+        sys_clk_freq    = args.sys_clk_freq,
+        ddram_channel   = int(args.ddram_channel, 0),
+        with_pcie       = args.with_pcie,
+        with_led_chaser = args.with_led_chaser,
+        with_hbm        = args.with_hbm,
+        with_analyzer   = args.with_analyzer,
         **parser.soc_argdict
-    )
-    if args.with_spi_sdcard:
-        soc.add_spi_sdcard()
-    if args.with_sdcard:
-        soc.add_sdcard()
+	)
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
+    if args.driver:
+        generate_litepcie_software(soc, os.path.join(builder.output_dir, "driver"))
+
     if args.load:
         prog = soc.platform.create_programmer()
-        prog.load_bitstream(builder.get_bitstream_filename(mode="sram", ext=".svf")) # FIXME
+        prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
 
 if __name__ == "__main__":
     main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/trenz_c10lprefkit.py` & `litex-boards-2023.8/litex_boards/targets/trenz_c10lprefkit.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/trenz_cyc1000.py` & `litex-boards-2023.8/litex_boards/targets/trenz_cyc1000.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/trenz_max1000.py` & `litex-boards-2023.8/litex_boards/targets/trenz_max1000.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/trenz_te0725.py` & `litex-boards-2023.8/litex_boards/targets/trenz_te0725.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/trenz_tec0117.py` & `litex-boards-2023.8/litex_boards/targets/trenz_tec0117.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/tul_pynq_z2.py` & `litex-boards-2023.8/litex_boards/targets/tul_pynq_z2.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/xilinx_alveo_u200.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_alveo_u250.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2023 Do Viet Thanh <thanhdv@soc.one>
 # Copyright (c) 2020 Fei Gao <feig@princeton.edu>
 # Copyright (c) 2020 Florent Kermarrec <florent@enjoy-digital.fr>
 # Copyright (c) 2020 David Shah <dave@ds0.me>
 # SPDX-License-Identifier: BSD-2-Clause
 
 import os
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex_boards.platforms import xilinx_alveo_u200
+from litex_boards.platforms import xilinx_alveo_u250
 
 from litex.soc.cores.clock import *
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
 
 from litex.soc.cores.led import LedChaser
 from litedram.modules import MTA18ASF2G72PZ
@@ -58,21 +57,21 @@
 
         self.idelayctrl = USIDELAYCTRL(cd_ref=self.cd_idelay, cd_sys=self.cd_sys)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
     def __init__(self, sys_clk_freq=125e6, with_led_chaser=True, with_pcie=False, **kwargs):
-        platform = xilinx_alveo_u200.Platform()
+        platform = xilinx_alveo_u250.Platform()
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Alveo U200", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Alveo U250", **kwargs)
 
         # DDR4 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
             self.ddrphy = usddrphy.USPDDRPHY(platform.request("ddram"),
                 memtype          = "DDR4",
                 sys_clk_freq     = sys_clk_freq,
                 cmd_latency      = 1,
@@ -101,15 +100,15 @@
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=xilinx_alveo_u200.Platform, description="LiteX SoC on Alveo U200.")
+    parser = LiteXArgumentParser(platform=xilinx_alveo_u250.Platform, description="LiteX SoC on Alveo U250.")
     parser.add_target_argument("--sys-clk-freq", default=125e6, type=float, help="System clock frequency.")
     parser.add_target_argument("--with-pcie",    action="store_true",       help="Enable PCIe support.")
     parser.add_target_argument("--driver",       action="store_true",       help="Generate PCIe driver.")
     args = parser.parse_args()
 
     soc = BaseSoC(
         sys_clk_freq = args.sys_clk_freq,
```

### Comparing `litex-boards-2023.12/litex_boards/targets/xilinx_alveo_u250.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_zcu106.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2020 Fei Gao <feig@princeton.edu>
-# Copyright (c) 2020 Florent Kermarrec <florent@enjoy-digital.fr>
-# Copyright (c) 2020 David Shah <dave@ds0.me>
+# Copyright (c) 2022 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
-import os
-
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex_boards.platforms import xilinx_alveo_u250
+from litex_boards.platforms import xilinx_zcu106
 
 from litex.soc.cores.clock import *
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
-
 from litex.soc.cores.led import LedChaser
-from litedram.modules import MTA18ASF2G72PZ
+
+from litedram.modules import MT40A256M16
 from litedram.phy import usddrphy
 
 from litepcie.phy.usppciephy import USPPCIEPHY
 from litepcie.software import generate_litepcie_software
 
 # CRG ----------------------------------------------------------------------------------------------
 
@@ -36,17 +32,20 @@
         self.cd_sys    = ClockDomain()
         self.cd_sys4x  = ClockDomain()
         self.cd_pll4x  = ClockDomain()
         self.cd_idelay = ClockDomain()
 
         # # #
 
+        clk125 = platform.request("clk125")
+        rst    = platform.request("rst")
+
         self.pll = pll = USMMCM(speedgrade=-2)
-        self.comb += pll.reset.eq(self.rst)
-        pll.register_clkin(platform.request("clk300", 0), 300e6)
+        self.comb += pll.reset.eq(self.rst | rst)
+        pll.register_clkin(clk125, 125e6)
         pll.create_clkout(self.cd_pll4x, sys_clk_freq*4, buf=None, with_reset=False)
         pll.create_clkout(self.cd_idelay, 500e6)
         platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
 
         self.specials += [
             Instance("BUFGCE_DIV",
                 p_BUFGCE_DIVIDE=4,
@@ -57,74 +56,66 @@
 
         self.idelayctrl = USIDELAYCTRL(cd_ref=self.cd_idelay, cd_sys=self.cd_sys)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
     def __init__(self, sys_clk_freq=125e6, with_led_chaser=True, with_pcie=False, **kwargs):
-        platform = xilinx_alveo_u250.Platform()
+        platform = xilinx_zcu106.Platform()
+
+        # SoCCore ----------------------------------------------------------------------------------
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on ZCU106", **kwargs)
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
-        # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Alveo U250", **kwargs)
-
         # DDR4 SDRAM -------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
             self.ddrphy = usddrphy.USPDDRPHY(platform.request("ddram"),
                 memtype          = "DDR4",
                 sys_clk_freq     = sys_clk_freq,
-                cmd_latency      = 1,
-                iodelay_clk_freq = 500e6,
-                is_rdimm         = True)
+                iodelay_clk_freq = 500e6)
             self.add_sdram("sdram",
                 phy           = self.ddrphy,
-                module        = MTA18ASF2G72PZ(sys_clk_freq, "1:4"),
-                size          = 0x40000000,
+                module        = MT40A256M16(sys_clk_freq, "1:4"),
+                size          = 0x20000000,
                 l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
-        # Firmware RAM (To ease initial LiteDRAM calibration support) ------------------------------
-        self.add_ram("firmware_ram", 0x20000000, 0x8000)
-
         # PCIe -------------------------------------------------------------------------------------
         if with_pcie:
             self.pcie_phy = USPPCIEPHY(platform, platform.request("pcie_x4"),
+                speed      = "gen3",
                 data_width = 128,
                 bar0_size  = 0x20000)
             self.add_pcie(phy=self.pcie_phy, ndmas=1)
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=xilinx_alveo_u250.Platform, description="LiteX SoC on Alveo U250.")
+    parser = LiteXArgumentParser(platform=xilinx_zcu106.Platform, description="LiteX SoC on ZCU106.")
     parser.add_target_argument("--sys-clk-freq", default=125e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--with-pcie",    action="store_true",       help="Enable PCIe support.")
-    parser.add_target_argument("--driver",       action="store_true",       help="Generate PCIe driver.")
+    parser.add_target_argument("--with-pcie",    action="store_true",       help="Enable PCIe support")
     args = parser.parse_args()
 
     soc = BaseSoC(
         sys_clk_freq = args.sys_clk_freq,
         with_pcie    = args.with_pcie,
         **parser.soc_argdict
     )
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
-    if args.driver:
-        generate_litepcie_software(soc, os.path.join(builder.output_dir, "driver"))
-
     if args.load:
         prog = soc.platform.create_programmer()
         prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
 
 if __name__ == "__main__":
     main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/xilinx_alveo_u280.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_vcu128.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,87 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2021 Sergiu Mosanu <sm7ed@virginia.edu>
-# Copyright (c) 2020-2021 Florent Kermarrec <florent@enjoy-digital.fr>
-# Copyright (c) 2020 Antmicro <www.antmicro.com>
-#
+# Copyright (c) 2020 Fei Gao <feig@princeton.edu>
+# Copyright (c) 2020 Florent Kermarrec <florent@enjoy-digital.fr>
+# Copyright (c) 2022 Jiajie Chen <c@jia.je>
 # SPDX-License-Identifier: BSD-2-Clause
 
-# To interface via the serial port use:
-#     lxterm /dev/ttyUSBx --speed=115200
-
-import os
-
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex_boards.platforms import xilinx_alveo_u280
+from litex_boards.platforms import xilinx_vcu128
 
 from litex.soc.cores.clock import *
+from litex.soc.cores.ram.xilinx_usp_hbm2 import USPHBM2
+from litex.soc.interconnect.axi import *
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.soc import SoCRegion
 from litex.soc.integration.builder import *
-from litex.soc.interconnect.axi import *
-from litex.soc.interconnect.csr import *
-from litex.soc.cores.ram.xilinx_usp_hbm2 import USPHBM2
-
 from litex.soc.cores.led import LedChaser
-from litedram.modules import MTA18ASF2G72PZ
-from litedram.phy import usddrphy
-
-from litepcie.phy.usppciephy import USPPCIEPHY
-from litepcie.software import generate_litepcie_software
 
-from litedram.common import *
-from litedram.frontend.axi import *
-
-from litescope import LiteScopeAnalyzer
+from litedram.modules import MT40A512M16
+from litedram.phy import usddrphy
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq, ddram_channel, with_hbm):
+    def __init__(self, platform, sys_clk_freq, with_hbm):
+        self.rst       = Signal()
+        self.cd_sys    = ClockDomain()
         if with_hbm:
-            self.rst        = Signal()
-            self.cd_sys     = ClockDomain()
             self.cd_hbm_ref = ClockDomain()
             self.cd_apb     = ClockDomain()
-        else: # ddr4
-            self.rst = Signal()
-            self.cd_sys    = ClockDomain()
+        else: # DDR4
             self.cd_sys4x  = ClockDomain()
             self.cd_pll4x  = ClockDomain()
             self.cd_idelay = ClockDomain()
 
         # # #
 
+        self.pll = pll = USMMCM(speedgrade=-2)
+        self.comb += pll.reset.eq(platform.request("cpu_reset") | self.rst)
+        pll.register_clkin(platform.request("clk100_ddr4"), 100e6)
         if with_hbm:
-            self.pll = pll = USMMCM(speedgrade=-2)
-            self.comb += pll.reset.eq(self.rst)
-            pll.register_clkin(platform.request("sysclk", ddram_channel), 100e6)
             pll.create_clkout(self.cd_sys,     sys_clk_freq)
             pll.create_clkout(self.cd_hbm_ref, 100e6)
             pll.create_clkout(self.cd_apb,     100e6)
             platform.add_false_path_constraints(self.cd_sys.clk, self.cd_apb.clk)
-        else: # ddr4
-            self.pll = pll = USMMCM(speedgrade=-2)
-            self.comb += pll.reset.eq(self.rst)
-            pll.register_clkin(platform.request("sysclk", ddram_channel), 100e6)
+        else:
             pll.create_clkout(self.cd_pll4x, sys_clk_freq*4, buf=None, with_reset=False)
-            pll.create_clkout(self.cd_idelay, 600e6) #, with_reset=False
+            pll.create_clkout(self.cd_idelay, 500e6)
             platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
 
             self.specials += [
                 Instance("BUFGCE_DIV",
                     p_BUFGCE_DIVIDE=4,
                     i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys.clk),
                 Instance("BUFGCE",
                     i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys4x.clk),
-                # AsyncResetSynchronizer(self.cd_idelay, ~pll.locked),
             ]
 
             self.idelayctrl = USIDELAYCTRL(cd_ref=self.cd_idelay, cd_sys=self.cd_sys)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=150e6, ddram_channel=0,
-        with_pcie       = False,
-        with_led_chaser = False,
-        with_hbm        = False,
-        **kwargs):
-        platform = xilinx_alveo_u280.Platform()
-        if with_hbm:
-            assert 225e6 <= sys_clk_freq <= 450e6
+    def __init__(self, sys_clk_freq=125e6, with_led_chaser=True, with_hbm=False, **kwargs):
+        platform = xilinx_vcu128.Platform()
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = _CRG(platform, sys_clk_freq, ddram_channel, with_hbm)
+        self.crg = _CRG(platform, sys_clk_freq, with_hbm)
 
         # SoCCore ----------------------------------------------------------------------------------
-        kwargs["jtagbone_chain"] = 2 # Chain 1 already used by HBM2 debug probes.
-
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on Alveo U280 (ES1)", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on VCU128", **kwargs)
 
-        # HBM / DRAM -------------------------------------------------------------------------------
+        # HBM --------------------------------------------------------------------------------------
         if with_hbm:
             # Add HBM Core.
             self.hbm = hbm = ClockDomainsRenamer({"axi": "sys"})(USPHBM2(platform))
 
             # Get HBM .xci.
             os.system("wget https://github.com/litex-hub/litex-boards/files/6893157/hbm_0.xci.txt")
             os.makedirs("ip/hbm", exist_ok=True)
@@ -120,79 +91,52 @@
             for i in range(4):
                 axi_hbm      = hbm.axi[i]
                 axi_lite_hbm = AXILiteInterface(data_width=256, address_width=33)
                 self.submodules += AXILite2AXI(axi_lite_hbm, axi_hbm)
                 self.bus.add_slave(f"hbm{i}", axi_lite_hbm, SoCRegion(origin=0x4000_0000 + 0x1000_0000*i, size=0x1000_0000)) # 256MB.
             # Link HBM2 channel 0 as main RAM
             self.bus.add_region("main_ram", SoCRegion(origin=0x4000_0000, size=0x1000_0000, linker=True)) # 256MB.
-
-        else:
+        elif not self.integrated_main_ram_size:
             # DDR4 SDRAM -------------------------------------------------------------------------------
-            if not self.integrated_main_ram_size:
-                self.ddrphy = usddrphy.USPDDRPHY(platform.request("ddram", ddram_channel),
-                    memtype          = "DDR4",
-                    cmd_latency      = 1, # seems to work better with cmd_latency=1
-                    sys_clk_freq     = sys_clk_freq,
-                    iodelay_clk_freq = 600e6,
-                    is_rdimm         = True)
-                self.add_sdram("sdram",
-                    phy           = self.ddrphy,
-                    module        = MTA18ASF2G72PZ(sys_clk_freq, "1:4"),
-                    size          = 0x40000000,
-                    l2_cache_size = kwargs.get("l2_size", 8192)
-                )
-
-            # Firmware RAM (To ease initial LiteDRAM calibration support) --------------------------
-            self.add_ram("firmware_ram", 0x20000000, 0x8000)
-
-        # PCIe -------------------------------------------------------------------------------------
-        if with_pcie:
-            self.pcie_phy = USPPCIEPHY(platform, platform.request("pcie_x4"),
-                data_width = 128,
-                bar0_size  = 0x20000)
-            self.add_pcie(phy=self.pcie_phy, ndmas=1)
+            self.ddrphy = usddrphy.USPDDRPHY(
+                pads             = platform.request("ddram"),
+                memtype          = "DDR4",
+                sys_clk_freq     = sys_clk_freq,
+                is_clam_shell    = True,
+                iodelay_clk_freq = 500e6)
+            self.add_sdram("sdram",
+                phy           = self.ddrphy,
+                module        = MT40A512M16(sys_clk_freq, "1:4"),
+                size          = 0x40000000,
+                l2_cache_size = kwargs.get("l2_size", 8192)
+            )
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
-                pads         = platform.request_all("gpio_led"),
+                pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=xilinx_alveo_u280.Platform, description="LiteX SoC on Alveo U280.")
-    parser.add_target_argument("--sys-clk-freq",    default=150e6, type=float, help="System clock frequency.") # HBM2 with 250MHz, DDR4 with 150MHz (1:4)
-    parser.add_target_argument("--ddram-channel",   default="0",               help="DDRAM channel (0, 1, 2 or 3).") # also selects clk 0 or 1
-    parser.add_target_argument("--with-pcie",       action="store_true",       help="Enable PCIe support.")
-    parser.add_target_argument("--driver",          action="store_true",       help="Generate PCIe driver.")
-    parser.add_target_argument("--with-hbm",        action="store_true",       help="Use HBM2.")
-    parser.add_target_argument("--with-analyzer",   action="store_true",       help="Enable Analyzer.")
-    parser.add_target_argument("--with-led-chaser", action="store_true",       help="Enable LED Chaser.")
+    parser = LiteXArgumentParser(platform=xilinx_vcu128.Platform, description="LiteX SoC on VCU128.")
+    parser.add_target_argument("--sys-clk-freq",  default=125e6, type=float, help="System clock frequency.")
+    parser.add_target_argument("--with-hbm",      action="store_true",       help="Use HBM2.")
     args = parser.parse_args()
 
-    if args.with_hbm:
-        args.sys_clk_freq = 250e6
-
     soc = BaseSoC(
-        sys_clk_freq    = args.sys_clk_freq,
-        ddram_channel   = int(args.ddram_channel, 0),
-        with_pcie       = args.with_pcie,
-        with_led_chaser = args.with_led_chaser,
-        with_hbm        = args.with_hbm,
-        with_analyzer   = args.with_analyzer,
+        sys_clk_freq = args.sys_clk_freq,
+        with_hbm     = args.with_hbm,
         **parser.soc_argdict
-	)
+    )
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
-    if args.driver:
-        generate_litepcie_software(soc, os.path.join(builder.output_dir, "driver"))
-
     if args.load:
         prog = soc.platform.create_programmer()
         prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
 
 if __name__ == "__main__":
     main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/xilinx_kv260.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_kv260.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/xilinx_vc707.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_vc707.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/xilinx_vcu118.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_vcu118.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/xilinx_vcu128.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_zcu104.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,137 +1,102 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2020 Fei Gao <feig@princeton.edu>
-# Copyright (c) 2020 Florent Kermarrec <florent@enjoy-digital.fr>
-# Copyright (c) 2022 Jiajie Chen <c@jia.je>
+# Copyright (c) 2020 Antmicro <www.antmicro.com>
+# Copyright (c) 2019 David Shah <dave@ds0.me>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
 from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex_boards.platforms import xilinx_vcu128
+from litex_boards.platforms import xilinx_zcu104
 
 from litex.soc.cores.clock import *
-from litex.soc.cores.ram.xilinx_usp_hbm2 import USPHBM2
-from litex.soc.interconnect.axi import *
 from litex.soc.integration.soc_core import *
-from litex.soc.integration.soc import SoCRegion
 from litex.soc.integration.builder import *
 from litex.soc.cores.led import LedChaser
+from litex.soc.cores.bitbang import I2CMaster
 
-from litedram.modules import MT40A512M16
+from litedram.modules import MTA4ATF51264HZ
 from litedram.phy import usddrphy
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
-    def __init__(self, platform, sys_clk_freq, with_hbm):
+    def __init__(self, platform, sys_clk_freq):
         self.rst       = Signal()
         self.cd_sys    = ClockDomain()
-        if with_hbm:
-            self.cd_hbm_ref = ClockDomain()
-            self.cd_apb     = ClockDomain()
-        else: # DDR4
-            self.cd_sys4x  = ClockDomain()
-            self.cd_pll4x  = ClockDomain()
-            self.cd_idelay = ClockDomain()
+        self.cd_sys4x  = ClockDomain()
+        self.cd_pll4x  = ClockDomain()
+        self.cd_idelay = ClockDomain()
 
         # # #
 
         self.pll = pll = USMMCM(speedgrade=-2)
-        self.comb += pll.reset.eq(platform.request("cpu_reset") | self.rst)
-        pll.register_clkin(platform.request("clk100_ddr4"), 100e6)
-        if with_hbm:
-            pll.create_clkout(self.cd_sys,     sys_clk_freq)
-            pll.create_clkout(self.cd_hbm_ref, 100e6)
-            pll.create_clkout(self.cd_apb,     100e6)
-            platform.add_false_path_constraints(self.cd_sys.clk, self.cd_apb.clk)
-        else:
-            pll.create_clkout(self.cd_pll4x, sys_clk_freq*4, buf=None, with_reset=False)
-            pll.create_clkout(self.cd_idelay, 500e6)
-            platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
-
-            self.specials += [
-                Instance("BUFGCE_DIV",
-                    p_BUFGCE_DIVIDE=4,
-                    i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys.clk),
-                Instance("BUFGCE",
-                    i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys4x.clk),
-            ]
+        self.comb += pll.reset.eq(self.rst)
+        pll.register_clkin(platform.request("clk125"), 125e6)
+        pll.create_clkout(self.cd_pll4x, sys_clk_freq*4, buf=None, with_reset=False)
+        pll.create_clkout(self.cd_idelay, 500e6)
+        platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
+
+        self.specials += [
+            Instance("BUFGCE_DIV",
+                p_BUFGCE_DIVIDE=4,
+                i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys.clk),
+            Instance("BUFGCE",
+                i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys4x.clk),
+        ]
 
-            self.idelayctrl = USIDELAYCTRL(cd_ref=self.cd_idelay, cd_sys=self.cd_sys)
+        self.idelayctrl = USIDELAYCTRL(cd_ref=self.cd_idelay, cd_sys=self.cd_sys)
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=125e6, with_led_chaser=True, with_hbm=False, **kwargs):
-        platform = xilinx_vcu128.Platform()
+    def __init__(self, sys_clk_freq=125e6, with_led_chaser=True, **kwargs):
+        platform = xilinx_zcu104.Platform()
 
         # CRG --------------------------------------------------------------------------------------
-        self.crg = _CRG(platform, sys_clk_freq, with_hbm)
+        self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on VCU128", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on ZCU104", **kwargs)
 
-        # HBM --------------------------------------------------------------------------------------
-        if with_hbm:
-            # Add HBM Core.
-            self.hbm = hbm = ClockDomainsRenamer({"axi": "sys"})(USPHBM2(platform))
-
-            # Get HBM .xci.
-            os.system("wget https://github.com/litex-hub/litex-boards/files/6893157/hbm_0.xci.txt")
-            os.makedirs("ip/hbm", exist_ok=True)
-            os.system("mv hbm_0.xci.txt ip/hbm/hbm_0.xci")
-
-            # Connect four of the HBM's AXI interfaces to the main bus of the SoC.
-            for i in range(4):
-                axi_hbm      = hbm.axi[i]
-                axi_lite_hbm = AXILiteInterface(data_width=256, address_width=33)
-                self.submodules += AXILite2AXI(axi_lite_hbm, axi_hbm)
-                self.bus.add_slave(f"hbm{i}", axi_lite_hbm, SoCRegion(origin=0x4000_0000 + 0x1000_0000*i, size=0x1000_0000)) # 256MB.
-            # Link HBM2 channel 0 as main RAM
-            self.bus.add_region("main_ram", SoCRegion(origin=0x4000_0000, size=0x1000_0000, linker=True)) # 256MB.
-        elif not self.integrated_main_ram_size:
-            # DDR4 SDRAM -------------------------------------------------------------------------------
-            self.ddrphy = usddrphy.USPDDRPHY(
-                pads             = platform.request("ddram"),
+        # DDR4 SDRAM -------------------------------------------------------------------------------
+        if not self.integrated_main_ram_size:
+            self.ddrphy = usddrphy.USPDDRPHY(platform.request("ddram"),
                 memtype          = "DDR4",
                 sys_clk_freq     = sys_clk_freq,
-                is_clam_shell    = True,
                 iodelay_clk_freq = 500e6)
             self.add_sdram("sdram",
                 phy           = self.ddrphy,
-                module        = MT40A512M16(sys_clk_freq, "1:4"),
+                module        = MTA4ATF51264HZ(sys_clk_freq, "1:4"),
                 size          = 0x40000000,
                 l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
         # Leds -------------------------------------------------------------------------------------
         if with_led_chaser:
             self.leds = LedChaser(
                 pads         = platform.request_all("user_led"),
                 sys_clk_freq = sys_clk_freq)
 
 # Build --------------------------------------------------------------------------------------------
 
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=xilinx_vcu128.Platform, description="LiteX SoC on VCU128.")
-    parser.add_target_argument("--sys-clk-freq",  default=125e6, type=float, help="System clock frequency.")
-    parser.add_target_argument("--with-hbm",      action="store_true",       help="Use HBM2.")
+    parser = LiteXArgumentParser(platform=xilinx_zcu104.Platform, description="LiteX SoC on ZCU104.")
+    parser.add_target_argument("--sys-clk-freq", default=125e6, type=float, help="System clock frequency.")
     args = parser.parse_args()
 
     soc = BaseSoC(
         sys_clk_freq = args.sys_clk_freq,
-        with_hbm     = args.with_hbm,
         **parser.soc_argdict
     )
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
     if args.load:
```

### Comparing `litex-boards-2023.12/litex_boards/targets/xilinx_zcu102.py` & `litex-boards-2023.8/litex_boards/targets/terasic_de2_115.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,102 +1,90 @@
 #!/usr/bin/env python3
 
 #
 # This file is part of LiteX-Boards.
 #
-# Copyright (c) 2022 Joseph FAYE <joseph-wagane.faye@insa-rennes.fr>
-# Copyright (c) 2023 Ryohei Niwase <niwase@lila.cs.tsukuba.ac.jp>
+# Copyright (c) 2015-2019 Florent Kermarrec <florent@enjoy-digital.fr>
 # SPDX-License-Identifier: BSD-2-Clause
 
 from migen import *
+from migen.genlib.resetsync import AsyncResetSynchronizer
 
 from litex.gen import *
 
-from litex_boards.platforms import xilinx_zcu102
+from litex.build.io import DDROutput
 
-from litex.soc.cores.clock import *
+from litex_boards.platforms import terasic_de2_115
+
+from litex.soc.cores.clock import CycloneIVPLL
 from litex.soc.integration.soc_core import *
 from litex.soc.integration.builder import *
-from litex.soc.cores.led import LedChaser
 
-from litedram.modules import MT40A256M16
-from litedram.phy import usddrphy
+from litedram.modules import IS42S16320
+from litedram.phy import GENSDRPHY
 
 # CRG ----------------------------------------------------------------------------------------------
 
 class _CRG(LiteXModule):
     def __init__(self, platform, sys_clk_freq):
         self.rst       = Signal()
         self.cd_sys    = ClockDomain()
-        self.cd_sys4x  = ClockDomain()
-        self.cd_pll4x  = ClockDomain()
-        self.cd_idelay = ClockDomain()
+        self.cd_sys_ps = ClockDomain()
 
         # # #
 
-        self.pll = pll = USMMCM(speedgrade=-2)
+        # Clk / Rst
+        clk50 = platform.request("clk50")
+
+        # PLL
+        self.pll = pll = CycloneIVPLL(speedgrade="-7")
         self.comb += pll.reset.eq(self.rst)
-        pll.register_clkin(platform.request("clk125"), 125e6)
-        pll.create_clkout(self.cd_pll4x, sys_clk_freq*4, buf=None, with_reset=False)
-        pll.create_clkout(self.cd_idelay, 500e6)
-        platform.add_false_path_constraints(self.cd_sys.clk, pll.clkin) # Ignore sys_clk to pll.clkin path created by SoC's rst.
-
-        self.specials += [
-            Instance("BUFGCE_DIV",
-                p_BUFGCE_DIVIDE=4,
-                i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys.clk),
-            Instance("BUFGCE",
-                i_CE=1, i_I=self.cd_pll4x.clk, o_O=self.cd_sys4x.clk),
-        ]
+        pll.register_clkin(clk50, 50e6)
+        pll.create_clkout(self.cd_sys,    sys_clk_freq)
+        pll.create_clkout(self.cd_sys_ps, sys_clk_freq, phase=90)
 
-        self.idelayctrl = USIDELAYCTRL(cd_ref=self.cd_idelay, cd_sys=self.cd_sys)
+        # SDRAM clock
+        self.specials += DDROutput(1, 0, platform.request("sdram_clock"), ClockSignal("sys_ps"))
 
 # BaseSoC ------------------------------------------------------------------------------------------
 
 class BaseSoC(SoCCore):
-    def __init__(self, sys_clk_freq=125e6, with_led_chaser=True, **kwargs):
-        platform = xilinx_zcu102.Platform()
+    def __init__(self, sys_clk_freq=50e6, **kwargs):
+        platform = terasic_de2_115.Platform()
 
         # CRG --------------------------------------------------------------------------------------
         self.crg = _CRG(platform, sys_clk_freq)
 
         # SoCCore ----------------------------------------------------------------------------------
-        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on ZCU102", **kwargs)
+        SoCCore.__init__(self, platform, sys_clk_freq, ident="LiteX SoC on DE2-115", **kwargs)
 
-        # DDR4 SDRAM -------------------------------------------------------------------------------
+        # SDR SDRAM --------------------------------------------------------------------------------
         if not self.integrated_main_ram_size:
-            self.ddrphy = usddrphy.USPDDRPHY(platform.request("ddram"),
-                memtype          = "DDR4",
-                sys_clk_freq     = sys_clk_freq,
-                iodelay_clk_freq = 500e6)
+            self.sdrphy = GENSDRPHY(platform.request("sdram"), sys_clk_freq)
             self.add_sdram("sdram",
-                phy           = self.ddrphy,
-                module        = MT40A256M16(sys_clk_freq, "1:4"),
-                size          = 0x20000000,
+                phy           = self.sdrphy,
+                module        = IS42S16320(self.clk_freq, "1:1"),
                 l2_cache_size = kwargs.get("l2_size", 8192)
             )
 
-        # Leds -------------------------------------------------------------------------------------
-        if with_led_chaser:
-            self.leds = LedChaser(
-                pads         = platform.request_all("user_led"),
-                sys_clk_freq = sys_clk_freq
-            )
-
 # Build --------------------------------------------------------------------------------------------
+
 def main():
     from litex.build.parser import LiteXArgumentParser
-    parser = LiteXArgumentParser(platform=xilinx_zcu102.Platform, description="LiteX SoC on ZCU102.")
-    parser.add_target_argument("--sys-clk-freq", default=125e6, type=float, help="System clock generator.")
+    parser = LiteXArgumentParser(platform=terasic_de2_115.Platform, description="LiteX SoC on DE2-115.")
+    parser.add_target_argument("--sys-clk-freq", default=50e6, type=float, help="System clock frequency.")
     args = parser.parse_args()
 
-    soc = BaseSoC(sys_clk_freq=args.sys_clk_freq, **parser.soc_argdict)
+    soc = BaseSoC(
+        sys_clk_freq = args.sys_clk_freq,
+        **parser.soc_argdict
+    )
     builder = Builder(soc, **parser.builder_argdict)
     if args.build:
         builder.build(**parser.toolchain_argdict)
 
     if args.load:
         prog = soc.platform.create_programmer()
         prog.load_bitstream(builder.get_bitstream_filename(mode="sram"))
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `litex-boards-2023.12/litex_boards/targets/xilinx_zcu216.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_zcu216.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards/targets/xilinx_zybo_z7.py` & `litex-boards-2023.8/litex_boards/targets/xilinx_zybo_z7.py`

 * *Files identical despite different names*

### Comparing `litex-boards-2023.12/litex_boards.egg-info/PKG-INFO` & `litex-boards-2023.8/litex_boards.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: litex-boards
-Version: 2023.12
+Version: 2023.8
 Summary: LiteX supported boards
 Home-page: http://enjoy-digital.fr
 Download-URL: https://github.com/litex-hub/litex-boards
 Author: Florent Kermarrec
 Author-email: florent@enjoy-digital.fr
 License: BSD
-Requires-Python: ~=3.7
+Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: litex
 
 
                                   __   _ __      _  __    ___                   __
                                  / /  (_) /____ | |/_/___/ _ )___  ___ ________/ /__
                                 / /__/ / __/ -_)>  </___/ _  / _ \/ _ `/ __/ _  (_-<
                                /____/_/\__/\__/_/|_|   /____/\___/\_,_/_/  \_,_/___/
 
@@ -107,18 +106,16 @@
 ---------------
     ├── adi_adrv2crr_fmc
     ├── adi_plutosdr
     ├── alchitry_au
     ├── alchitry_cu
     ├── alchitry_mojo
     ├── aliexpress_xc7k420t
-    ├── aliexpress_xc7k70t
     ├── alinx_ax7010
     ├── alinx_axu2cga
-    ├── analog_pocket
     ├── antmicro_artix_dc_scm
     ├── antmicro_datacenter_ddr4_test_board
     ├── antmicro_lpddr4_test_board
     ├── antmicro_sdi_mipi_video_converter
     ├── arduino_mkrvidor4000
     ├── avalanche
     ├── avnet_aesku40
@@ -184,15 +181,14 @@
     ├── limesdr_mini_v2
     ├── linsn_rv901t
     ├── litex_acorn_baseboard
     ├── logicbone
     ├── machdyne_konfekt
     ├── machdyne_kopflos
     ├── machdyne_krote
-    ├── machdyne_mozart_ml1
     ├── machdyne_noir
     ├── machdyne_schoko
     ├── marblemini
     ├── marble
     ├── micronova_mercury2
     ├── mist
     ├── mnt_rkx7
@@ -227,17 +223,15 @@
     ├── scarabhardware_minispartan6
     ├── seeedstudio_spartan_edge_accelerator
     ├── siglent_sds1104xe
     ├── sipeed_tang_nano_20k
     ├── sipeed_tang_nano_4k
     ├── sipeed_tang_nano_9k
     ├── sipeed_tang_nano
-    ├── sipeed_tang_mega_138k
     ├── sipeed_tang_primer_20k
-    ├── sipeed_tang_primer_25k
     ├── sipeed_tang_primer
     ├── sitlinv_a_e115fb
     ├── sitlinv_stlv7325
     ├── sitlinv_xc7k420t
     ├── sqrl_acorn
     ├── sqrl_fk33
     ├── sqrl_xcu1525
```

### Comparing `litex-boards-2023.12/litex_boards.egg-info/SOURCES.txt` & `litex-boards-2023.8/litex_boards.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 litex_boards/platforms/__init__.py
 litex_boards/platforms/adi_adrv2crr_fmc.py
 litex_boards/platforms/adi_plutosdr.py
 litex_boards/platforms/alchitry_au.py
 litex_boards/platforms/alchitry_cu.py
 litex_boards/platforms/alchitry_mojo.py
 litex_boards/platforms/aliexpress_xc7k420t.py
-litex_boards/platforms/aliexpress_xc7k70t.py
 litex_boards/platforms/alinx_ax7010.py
 litex_boards/platforms/alinx_axu2cga.py
-litex_boards/platforms/analog_pocket.py
 litex_boards/platforms/antmicro_artix_dc_scm.py
 litex_boards/platforms/antmicro_datacenter_ddr4_test_board.py
 litex_boards/platforms/antmicro_lpddr4_test_board.py
 litex_boards/platforms/antmicro_sdi_mipi_video_converter.py
 litex_boards/platforms/arduino_mkrvidor4000.py
 litex_boards/platforms/avalanche.py
 litex_boards/platforms/avnet_aesku40.py
@@ -91,15 +89,14 @@
 litex_boards/platforms/limesdr_mini_v2.py
 litex_boards/platforms/linsn_rv901t.py
 litex_boards/platforms/litex_acorn_baseboard.py
 litex_boards/platforms/logicbone.py
 litex_boards/platforms/machdyne_konfekt.py
 litex_boards/platforms/machdyne_kopflos.py
 litex_boards/platforms/machdyne_krote.py
-litex_boards/platforms/machdyne_mozart_ml1.py
 litex_boards/platforms/machdyne_noir.py
 litex_boards/platforms/machdyne_schoko.py
 litex_boards/platforms/marble.py
 litex_boards/platforms/marblemini.py
 litex_boards/platforms/micronova_mercury2.py
 litex_boards/platforms/mist.py
 litex_boards/platforms/mnt_rkx7.py
@@ -119,37 +116,34 @@
 litex_boards/platforms/qmtech_5cefa5.py
 litex_boards/platforms/qmtech_artix7_fbg484.py
 litex_boards/platforms/qmtech_artix7_fgg676.py
 litex_boards/platforms/qmtech_daughterboard.py
 litex_boards/platforms/qmtech_ep4ce15_starter_kit.py
 litex_boards/platforms/qmtech_ep4cex5.py
 litex_boards/platforms/qmtech_ep4cgx150.py
-litex_boards/platforms/qmtech_rp2040_daughterboard.py
 litex_boards/platforms/qmtech_wukong.py
 litex_boards/platforms/qmtech_xc7a35t.py
 litex_boards/platforms/qmtech_xc7k325t.py
 litex_boards/platforms/quicklogic_quickfeather.py
 litex_boards/platforms/qwertyembedded_beaglewire.py
 litex_boards/platforms/radiona_ulx3s.py
 litex_boards/platforms/radiona_ulx4m_ld_v2.py
 litex_boards/platforms/rcs_arctic_tern_bmc_card.py
 litex_boards/platforms/redpitaya.py
 litex_boards/platforms/rz_easyfpga.py
 litex_boards/platforms/saanlima_pipistrello.py
 litex_boards/platforms/scarabhardware_minispartan6.py
 litex_boards/platforms/seeedstudio_spartan_edge_accelerator.py
 litex_boards/platforms/siglent_sds1104xe.py
-litex_boards/platforms/sipeed_tang_mega_138k.py
 litex_boards/platforms/sipeed_tang_nano.py
 litex_boards/platforms/sipeed_tang_nano_20k.py
 litex_boards/platforms/sipeed_tang_nano_4k.py
 litex_boards/platforms/sipeed_tang_nano_9k.py
 litex_boards/platforms/sipeed_tang_primer.py
 litex_boards/platforms/sipeed_tang_primer_20k.py
-litex_boards/platforms/sipeed_tang_primer_25k.py
 litex_boards/platforms/sitlinv_a_e115fb.py
 litex_boards/platforms/sitlinv_stlv7325_v1.py
 litex_boards/platforms/sitlinv_stlv7325_v2.py
 litex_boards/platforms/sitlinv_xc7k420t.py
 litex_boards/platforms/sqrl_acorn.py
 litex_boards/platforms/sqrl_fk33.py
 litex_boards/platforms/sqrl_xcu1525.py
@@ -187,18 +181,16 @@
 litex_boards/targets/__init__.py
 litex_boards/targets/adi_adrv2crr_fmc.py
 litex_boards/targets/adi_plutosdr.py
 litex_boards/targets/alchitry_au.py
 litex_boards/targets/alchitry_cu.py
 litex_boards/targets/alchitry_mojo.py
 litex_boards/targets/aliexpress_xc7k420t.py
-litex_boards/targets/aliexpress_xc7k70t.py
 litex_boards/targets/alinx_ax7010.py
 litex_boards/targets/alinx_axu2cga.py
-litex_boards/targets/analog_pocket.py
 litex_boards/targets/antmicro_artix_dc_scm.py
 litex_boards/targets/antmicro_datacenter_ddr4_test_board.py
 litex_boards/targets/antmicro_lpddr4_test_board.py
 litex_boards/targets/antmicro_sdi_mipi_video_converter.py
 litex_boards/targets/arduino_mkrvidor4000.py
 litex_boards/targets/avnet_aesku40.py
 litex_boards/targets/berkeleylab_marble.py
@@ -256,15 +248,14 @@
 litex_boards/targets/limesdr_mini_v2.py
 litex_boards/targets/linsn_rv901t.py
 litex_boards/targets/litex_acorn_baseboard.py
 litex_boards/targets/logicbone.py
 litex_boards/targets/machdyne_konfekt.py
 litex_boards/targets/machdyne_kopflos.py
 litex_boards/targets/machdyne_krote.py
-litex_boards/targets/machdyne_mozart_ml1.py
 litex_boards/targets/machdyne_noir.py
 litex_boards/targets/machdyne_schoko.py
 litex_boards/targets/micronova_mercury2.py
 litex_boards/targets/mist.py
 litex_boards/targets/mnt_rkx7.py
 litex_boards/targets/muselab_icesugar.py
 litex_boards/targets/muselab_icesugar_pro.py
@@ -296,22 +287,20 @@
 litex_boards/targets/redpitaya.py
 litex_boards/targets/rz_easyfpga.py
 litex_boards/targets/saanlima_pipistrello.py
 litex_boards/targets/scarabhardware_minispartan6.py
 litex_boards/targets/seeedstudio_spartan_edge_accelerator.py
 litex_boards/targets/siglent_sds1104xe.py
 litex_boards/targets/simple.py
-litex_boards/targets/sipeed_tang_mega_138k.py
 litex_boards/targets/sipeed_tang_nano.py
 litex_boards/targets/sipeed_tang_nano_20k.py
 litex_boards/targets/sipeed_tang_nano_4k.py
 litex_boards/targets/sipeed_tang_nano_9k.py
 litex_boards/targets/sipeed_tang_primer.py
 litex_boards/targets/sipeed_tang_primer_20k.py
-litex_boards/targets/sipeed_tang_primer_25k.py
 litex_boards/targets/sitlinv_a_e115fb.py
 litex_boards/targets/sitlinv_stlv7325_v1.py
 litex_boards/targets/sitlinv_stlv7325_v2.py
 litex_boards/targets/sitlinv_xc7k420t.py
 litex_boards/targets/sqrl_acorn.py
 litex_boards/targets/sqrl_fk33.py
 litex_boards/targets/sqrl_xcu1525.py
```

### Comparing `litex-boards-2023.12/test/test_targets.py` & `litex-boards-2023.8/test/test_targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from migen import *
 
 from litex.soc.integration.builder import *
 
 class TestTargets(unittest.TestCase):
     excluded_platforms = [
         "qmtech_daughterboard",              # Reason: Not a real platform.
-        "qmtech_rp2040_daughterboard",       # Reason: Not a real platform.
         "enclustra_st1",                     # Readon: Not a real platform.
         "quicklogic_quickfeather",           # Reason: No default clock.
         "efinix_titanium_ti60_f225_dev_kit", # Reason: Require Efinity toolchain.
         "efinix_trion_t120_bga576_dev_kit",  # Reason: Require Efinity toolchain.
         "efinix_trion_t20_bga256_dev_kit",   # Reason: Require Efinity toolchain.
         "efinix_trion_t20_mipi_dev_kit",     # Reason: Require Efinity toolchain.
         "efinix_xyloni_dev_kit",             # Reason: Require Efinity toolchain.
```

