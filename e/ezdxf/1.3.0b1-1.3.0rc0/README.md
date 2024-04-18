# Comparing `tmp/ezdxf-1.3.0b1.zip` & `tmp/ezdxf-1.3.0rc0.zip`

## zipinfo {}

```diff
@@ -1,855 +1,860 @@
-Zip file size: 2186890 bytes, number of entries: 853
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/integration_tests/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/tests/
--rw-rw-rw-  2.0 fat     1092 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/LICENSE
--rw-rw-rw-  2.0 fat      329 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/MANIFEST.in
--rw-rw-rw-  2.0 fat    10110 b- defN 24-Mar-25 08:04 ezdxf-1.3.0b1/PKG-INFO
--rw-rw-rw-  2.0 fat     2527 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/pyproject.toml
--rw-rw-rw-  2.0 fat     7479 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/README.md
--rw-rw-rw-  2.0 fat       74 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/requirements.txt
--rw-rw-rw-  2.0 fat       42 b- defN 24-Mar-25 08:04 ezdxf-1.3.0b1/setup.cfg
--rw-rw-rw-  2.0 fat     2140 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/integration_tests/data/
--rw-rw-rw-  2.0 fat      567 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/check_disable_c_ext_by_config_file.py
--rw-rw-rw-  2.0 fat      541 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/check_disable_c_ext_by_env_var.py
--rw-rw-rw-  2.0 fat      410 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/conftest.py
--rw-rw-rw-  2.0 fat     1054 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_acad_table.py
--rw-rw-rw-  2.0 fat     4686 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_all_dimline_styles.py
--rw-rw-rw-  2.0 fat     4153 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_all_ellipse_transformations.py
--rw-rw-rw-  2.0 fat     1064 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_anonymous_blocks.py
--rw-rw-rw-  2.0 fat      577 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_appsettings.py
--rw-rw-rw-  2.0 fat      871 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_audit_critical_dxf_files.py
--rw-rw-rw-  2.0 fat     1603 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_audit_layouts.py
--rw-rw-rw-  2.0 fat     1726 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_complex_line_type_2.py
--rw-rw-rw-  2.0 fat     1003 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_create_basic_graphics.py
--rw-rw-rw-  2.0 fat     1921 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_document_guid.py
--rw-rw-rw-  2.0 fat     1832 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_document_page_setup.py
--rw-rw-rw-  2.0 fat      998 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_dxf_info_scanning.py
--rw-rw-rw-  2.0 fat     1299 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_dynblkhelper.py
--rw-rw-rw-  2.0 fat     1558 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_entities_iterator.py
--rw-rw-rw-  2.0 fat      934 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_fix_dulicate_handles.py
--rw-rw-rw-  2.0 fat     1901 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_geo.py
--rw-rw-rw-  2.0 fat     1250 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_groups.py
--rw-rw-rw-  2.0 fat      905 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_hpgl2_addon.py
--rw-rw-rw-  2.0 fat      630 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_ignore_junk_beyond_EOF.py
--rw-rw-rw-  2.0 fat     1155 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_launcher.py
--rw-rw-rw-  2.0 fat      631 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_leica_disto_r12.py
--rw-rw-rw-  2.0 fat      737 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_load_dxf_unicode_notation.py
--rw-rw-rw-  2.0 fat     2931 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_mapbox_earcut.py
--rw-rw-rw-  2.0 fat     2230 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_mtext_columns.py
--rw-rw-rw-  2.0 fat     2392 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_mtext_explode_addon.py
--rw-rw-rw-  2.0 fat     1846 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_mtext_text_frame.py
--rw-rw-rw-  2.0 fat     1053 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_new_table_entries.py
--rw-rw-rw-  2.0 fat      887 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_none_ascii_read_write.py
--rw-rw-rw-  2.0 fat     3435 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_odafc.py
--rw-rw-rw-  2.0 fat     1737 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_open_binary_DXF_files.py
--rw-rw-rw-  2.0 fat      751 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_open_coord_order_issue.py
--rw-rw-rw-  2.0 fat     3842 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_open_exotic_dxf_files.py
--rw-rw-rw-  2.0 fat      879 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_open_R13_R14.py
--rw-rw-rw-  2.0 fat     3152 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_polyline_entity.py
--rw-rw-rw-  2.0 fat     1749 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_preserve_binary_data_in_xrecords.py
--rw-rw-rw-  2.0 fat     6944 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_r12export.py
--rw-rw-rw-  2.0 fat     6256 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_r12strict.py
--rw-rw-rw-  2.0 fat     3410 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_r12writer.py
--rw-rw-rw-  2.0 fat      567 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_read_file_without_handles.py
--rw-rw-rw-  2.0 fat     1121 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_read_write_modern_entites.py
--rw-rw-rw-  2.0 fat     7747 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_recover.py
--rw-rw-rw-  2.0 fat     1959 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_redraw_order.py
--rw-rw-rw-  2.0 fat     1819 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_rotated_block_attributes.py
--rw-rw-rw-  2.0 fat      774 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_surface_entities.py
--rw-rw-rw-  2.0 fat      928 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_write_fixed_meta_data.py
--rw-rw-rw-  2.0 fat     1806 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_write_without_handles.py
--rw-rw-rw-  2.0 fat     3638 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/test_xref_detach.py
--rw-rw-rw-  2.0 fat     3060 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/AC1003_LINE_Example.dxf
--rw-rw-rw-  2.0 fat   179505 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/acad_table_with_blk_ref.dxf
--rw-rw-rw-  2.0 fat     7956 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/ASCII_R12.dxf
--rw-rw-rw-  2.0 fat     3761 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/bin_dxf_r12.dxf
--rw-rw-rw-  2.0 fat    20914 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/bin_dxf_r13.dxf
--rw-rw-rw-  2.0 fat    21137 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/bin_dxf_r14.dxf
--rw-rw-rw-  2.0 fat    11564 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/bin_dxf_r2000.dxf
--rw-rw-rw-  2.0 fat     6424 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/cc_dxflib.dxf
--rw-rw-rw-  2.0 fat   173753 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/custom_blocks.dxf
--rw-rw-rw-  2.0 fat    32203 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/duplicate_handles.dxf
--rw-rw-rw-  2.0 fat    18554 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/dxf_unicode.dxf
--rw-rw-rw-  2.0 fat    56494 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/dynblks.zip
--rw-rw-rw-  2.0 fat     1592 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/empty_handles.dxf
--rw-rw-rw-  2.0 fat    97103 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/groups.dxf
--rw-rw-rw-  2.0 fat    19533 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/layout_broken_links.dxf
--rw-rw-rw-  2.0 fat    19506 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/layout_broken_links_2.dxf
--rw-rw-rw-  2.0 fat    19291 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/layout_missing_block_definition.dxf
--rw-rw-rw-  2.0 fat    19383 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/layout_missing_block_record.dxf
--rw-rw-rw-  2.0 fat     9146 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/Leica_Disto_S910.dxf
--rw-rw-rw-  2.0 fat    17986 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/MODEL.dxf
--rw-rw-rw-  2.0 fat    25799 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/mtext_columns_R2007.dxf
--rw-rw-rw-  2.0 fat    23927 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/mtext_columns_R2018.dxf
--rw-rw-rw-  2.0 fat    98230 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/mtext_framed_columns.dxf
--rw-rw-rw-  2.0 fat   106574 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/mtext_text_frame.dxf
--rw-rw-rw-  2.0 fat    12001 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/no_layouts.dxf
--rw-rw-rw-  2.0 fat    16295 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/PLOTFILE.plt
--rw-rw-rw-  2.0 fat    28788 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/POLI-ALL210_12.DXF
--rw-rw-rw-  2.0 fat      144 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/R12_with_trash_beyond_EOF.dxf
--rw-rw-rw-  2.0 fat   212407 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/recover01.dxf
--rw-rw-rw-  2.0 fat   115423 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/recover02.dxf
--rw-rw-rw-  2.0 fat    21178 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/small_r13.dxf
--rw-rw-rw-  2.0 fat    10326 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/small_r14.dxf
--rw-rw-rw-  2.0 fat    11286 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/XRECORD_0.bin
--rw-rw-rw-  2.0 fat    11662 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/XRECORD_1.bin
--rw-rw-rw-  2.0 fat    15337 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/integration_tests/data/XRECORD_2.bin
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/acc/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/acis/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/addons/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/entities/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/fonts/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/lldxf/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/math/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/path/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/render/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/resources/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/sections/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/tools/
--rw-rw-rw-  2.0 fat     4841 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/appsettings.py
--rw-rw-rw-  2.0 fat    19886 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/audit.py
--rw-rw-rw-  2.0 fat     5324 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/bbox.py
--rw-rw-rw-  2.0 fat     7872 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/blkrefs.py
--rw-rw-rw-  2.0 fat    17062 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/colors.py
--rw-rw-rw-  2.0 fat    33508 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/commands.py
--rw-rw-rw-  2.0 fat     1549 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/comments.py
--rw-rw-rw-  2.0 fat    22334 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/disassemble.py
--rw-rw-rw-  2.0 fat    54828 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/document.py
--rw-rw-rw-  2.0 fat      832 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/dwginfo.py
--rw-rw-rw-  2.0 fat     2475 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/dynblkhelper.py
--rw-rw-rw-  2.0 fat    16254 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entitydb.py
--rw-rw-rw-  2.0 fat     7495 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/enums.py
--rw-rw-rw-  2.0 fat    14519 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/explode.py
--rw-rw-rw-  2.0 fat     1653 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/eztypes.py
--rw-rw-rw-  2.0 fat    10366 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/filemanagement.py
--rw-rw-rw-  2.0 fat    12157 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/gfxattribs.py
--rw-rw-rw-  2.0 fat   107528 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/graphicsfactory.py
--rw-rw-rw-  2.0 fat     3416 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/groupby.py
--rw-rw-rw-  2.0 fat    20554 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/npshapes.py
--rw-rw-rw-  2.0 fat     2743 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/protocols.py
--rw-rw-rw-  2.0 fat    35308 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/proxygraphic.py
--rw-rw-rw-  2.0 fat       95 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/py.typed
--rw-rw-rw-  2.0 fat    22499 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/query.py
--rw-rw-rw-  2.0 fat     2780 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/queryparser.py
--rw-rw-rw-  2.0 fat     9564 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/r12strict.py
--rw-rw-rw-  2.0 fat    31442 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/recover.py
--rw-rw-rw-  2.0 fat     3515 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/reorder.py
--rw-rw-rw-  2.0 fat     3926 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/revcloud.py
--rw-rw-rw-  2.0 fat    11250 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/select.py
--rw-rw-rw-  2.0 fat    10450 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/transform.py
--rw-rw-rw-  2.0 fat     5750 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/units.py
--rw-rw-rw-  2.0 fat     8280 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/upright.py
--rw-rw-rw-  2.0 fat     9875 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/urecord.py
--rw-rw-rw-  2.0 fat     1024 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/version.py
--rw-rw-rw-  2.0 fat    18280 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/xclip.py
--rw-rw-rw-  2.0 fat    65734 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/xref.py
--rw-rw-rw-  2.0 fat     2853 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/zoom.py
--rw-rw-rw-  2.0 fat    10898 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/_options.py
--rw-rw-rw-  2.0 fat     3138 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/__init__.py
--rw-rw-rw-  2.0 fat     3259 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/__main__.py
--rw-rw-rw-  2.0 fat     6788 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acc/bezier3p.pyx
--rw-rw-rw-  2.0 fat    11502 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acc/bezier4p.pyx
--rw-rw-rw-  2.0 fat    14048 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acc/bspline.pyx
--rw-rw-rw-  2.0 fat      252 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acc/constants.h
--rw-rw-rw-  2.0 fat    11844 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acc/construct.pyx
--rw-rw-rw-  2.0 fat     3161 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acc/linetypes.pyx
--rw-rw-rw-  2.0 fat    23976 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acc/mapbox_earcut.pyx
--rw-rw-rw-  2.0 fat      385 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acc/matrix44.pxd
--rw-rw-rw-  2.0 fat    23703 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acc/matrix44.pyx
--rw-rw-rw-  2.0 fat     4705 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acc/np_support.pyx
--rw-rw-rw-  2.0 fat     1719 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acc/vector.pxd
--rw-rw-rw-  2.0 fat    23377 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acc/vector.pyx
--rw-rw-rw-  2.0 fat     1265 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acc/__init__.py
--rw-rw-rw-  2.0 fat     6398 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acis/abstract.py
--rw-rw-rw-  2.0 fat      888 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acis/api.py
--rw-rw-rw-  2.0 fat     5489 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acis/const.py
--rw-rw-rw-  2.0 fat     6731 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acis/dbg.py
--rw-rw-rw-  2.0 fat     2985 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acis/dxf.py
--rw-rw-rw-  2.0 fat    28996 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acis/entities.py
--rw-rw-rw-  2.0 fat     4093 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acis/hdr.py
--rw-rw-rw-  2.0 fat    12834 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acis/mesh.py
--rw-rw-rw-  2.0 fat    18695 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acis/sab.py
--rw-rw-rw-  2.0 fat    13189 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acis/sat.py
--rw-rw-rw-  2.0 fat      120 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/acis/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/addons/acisbrowser/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/addons/browser/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/addons/dwg/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/
--rw-rw-rw-  2.0 fat    26415 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/acadctb.py
--rw-rw-rw-  2.0 fat    22229 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/binpacking.py
--rw-rw-rw-  2.0 fat    27692 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/dimlines.py
--rw-rw-rw-  2.0 fat    31454 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/dxf2code.py
--rw-rw-rw-  2.0 fat    22005 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/genetic_algorithm.py
--rw-rw-rw-  2.0 fat    38393 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/geo.py
--rw-rw-rw-  2.0 fat     2674 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/gerber_D6673.py
--rw-rw-rw-  2.0 fat    25472 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/importer.py
--rw-rw-rw-  2.0 fat    17355 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/iterdxf.py
--rw-rw-rw-  2.0 fat     8946 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/menger_sponge.py
--rw-rw-rw-  2.0 fat    24787 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/meshex.py
--rw-rw-rw-  2.0 fat      492 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/mixins.py
--rw-rw-rw-  2.0 fat     6203 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/mtextsurrogate.py
--rw-rw-rw-  2.0 fat    13528 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/mtxpl.py
--rw-rw-rw-  2.0 fat    16307 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/odafc.py
--rw-rw-rw-  2.0 fat     9456 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/openscad.py
--rw-rw-rw-  2.0 fat    15878 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/pycsg.py
--rw-rw-rw-  2.0 fat    22301 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/r12export.py
--rw-rw-rw-  2.0 fat    27191 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/r12writer.py
--rw-rw-rw-  2.0 fat     7605 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/sierpinski_pyramid.py
--rw-rw-rw-  2.0 fat    33167 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/tablepainter.py
--rw-rw-rw-  2.0 fat    12768 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/text2path.py
--rw-rw-rw-  2.0 fat     3335 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/xplayer.py
--rw-rw-rw-  2.0 fat     2312 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/xqt.py
--rw-rw-rw-  2.0 fat      453 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/__init__.py
--rw-rw-rw-  2.0 fat     9975 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/acisbrowser/browser.py
--rw-rw-rw-  2.0 fat     1907 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/acisbrowser/data.py
--rw-rw-rw-  2.0 fat       64 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/acisbrowser/__init__.py
--rw-rw-rw-  2.0 fat      820 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/browser/bookmarks.py
--rw-rw-rw-  2.0 fat    29347 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/browser/browser.py
--rw-rw-rw-  2.0 fat    14891 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/browser/data.py
--rw-rw-rw-  2.0 fat    10993 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/browser/find_dialog.py
--rw-rw-rw-  2.0 fat     1249 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/browser/loader.py
--rw-rw-rw-  2.0 fat    21111 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/browser/model.py
--rw-rw-rw-  2.0 fat     6896 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/browser/reflinks.py
--rw-rw-rw-  2.0 fat     2214 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/browser/tags.py
--rw-rw-rw-  2.0 fat     1366 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/browser/views.py
--rw-rw-rw-  2.0 fat      133 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/browser/__init__.py
--rw-rw-rw-  2.0 fat     9265 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/backend.py
--rw-rw-rw-  2.0 fat    11113 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/config.py
--rw-rw-rw-  2.0 fat     1756 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/debug_backend.py
--rw-rw-rw-  2.0 fat      514 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/debug_utils.py
--rw-rw-rw-  2.0 fat     7391 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/dxf.py
--rw-rw-rw-  2.0 fat     7753 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/file_output.py
--rw-rw-rw-  2.0 fat    44576 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/frontend.py
--rw-rw-rw-  2.0 fat     1877 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/gfxproxy.py
--rw-rw-rw-  2.0 fat    20834 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/hpgl2.py
--rw-rw-rw-  2.0 fat    20101 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/json.py
--rw-rw-rw-  2.0 fat    18871 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/layout.py
--rw-rw-rw-  2.0 fat    13209 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/matplotlib.py
--rw-rw-rw-  2.0 fat     9862 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/mtext_complex.py
--rw-rw-rw-  2.0 fat    31952 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/pipeline.py
--rw-rw-rw-  2.0 fat    40194 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/properties.py
--rw-rw-rw-  2.0 fat    18036 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/pymupdf.py
--rw-rw-rw-  2.0 fat    11577 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/pyqt.py
--rw-rw-rw-  2.0 fat    22713 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/qtviewer.py
--rw-rw-rw-  2.0 fat    16434 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/recorder.py
--rw-rw-rw-  2.0 fat    16222 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/svg.py
--rw-rw-rw-  2.0 fat    13023 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/text.py
--rw-rw-rw-  2.0 fat     1194 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/text_renderer.py
--rw-rw-rw-  2.0 fat      314 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/type_hints.py
--rw-rw-rw-  2.0 fat     2559 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/unified_text_renderer.py
--rw-rw-rw-  2.0 fat      171 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/drawing/__init__.py
--rw-rw-rw-  2.0 fat     3112 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/dwg/classes_section.py
--rw-rw-rw-  2.0 fat      763 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/dwg/const.py
--rw-rw-rw-  2.0 fat     6091 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/dwg/crc.py
--rw-rw-rw-  2.0 fat     3160 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/dwg/fileheader.py
--rw-rw-rw-  2.0 fat    14851 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/dwg/header_section.py
--rw-rw-rw-  2.0 fat     2976 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/dwg/loader.py
--rw-rw-rw-  2.0 fat      141 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/dwg/__init__.py
--rw-rw-rw-  2.0 fat    13443 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/api.py
--rw-rw-rw-  2.0 fat     8554 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/backend.py
--rw-rw-rw-  2.0 fat      561 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/deps.py
--rw-rw-rw-  2.0 fat    16079 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/interpreter.py
--rw-rw-rw-  2.0 fat     4836 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/page.py
--rw-rw-rw-  2.0 fat    11766 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/plotter.py
--rw-rw-rw-  2.0 fat     1698 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/polygon_buffer.py
--rw-rw-rw-  2.0 fat     5615 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/properties.py
--rw-rw-rw-  2.0 fat     6222 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/tokenizer.py
--rw-rw-rw-  2.0 fat    19435 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/viewer.py
--rw-rw-rw-  2.0 fat      164 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/__init__.py
--rw-rw-rw-  2.0 fat     5729 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/acad_proxy_entity.py
--rw-rw-rw-  2.0 fat    21432 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/acad_table.py
--rw-rw-rw-  2.0 fat     2850 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/acad_xrec_roundtrip.py
--rw-rw-rw-  2.0 fat    25905 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/acis.py
--rw-rw-rw-  2.0 fat     4996 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/appdata.py
--rw-rw-rw-  2.0 fat     1954 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/appid.py
--rw-rw-rw-  2.0 fat     4942 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/arc.py
--rw-rw-rw-  2.0 fat    27102 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/attrib.py
--rw-rw-rw-  2.0 fat     8850 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/block.py
--rw-rw-rw-  2.0 fat    10555 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/blockrecord.py
--rw-rw-rw-  2.0 fat    50111 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/boundary_paths.py
--rw-rw-rw-  2.0 fat     7929 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/circle.py
--rw-rw-rw-  2.0 fat     3214 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/copy.py
--rw-rw-rw-  2.0 fat    24960 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/dictionary.py
--rw-rw-rw-  2.0 fat    48727 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/dimension.py
--rw-rw-rw-  2.0 fat    35012 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/dimstyle.py
--rw-rw-rw-  2.0 fat    23813 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/dimstyleoverride.py
--rw-rw-rw-  2.0 fat     4399 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/dxfclass.py
--rw-rw-rw-  2.0 fat    40455 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/dxfentity.py
--rw-rw-rw-  2.0 fat    27091 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/dxfgfx.py
--rw-rw-rw-  2.0 fat    15319 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/dxfgroups.py
--rw-rw-rw-  2.0 fat    23679 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/dxfns.py
--rw-rw-rw-  2.0 fat    13862 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/dxfobj.py
--rw-rw-rw-  2.0 fat    11186 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/ellipse.py
--rw-rw-rw-  2.0 fat     4138 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/factory.py
--rw-rw-rw-  2.0 fat    23747 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/geodata.py
--rw-rw-rw-  2.0 fat     4026 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/gradient.py
--rw-rw-rw-  2.0 fat    12263 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/hatch.py
--rw-rw-rw-  2.0 fat     3944 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/helix.py
--rw-rw-rw-  2.0 fat     4807 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/idbuffer.py
--rw-rw-rw-  2.0 fat    27140 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/image.py
--rw-rw-rw-  2.0 fat    28117 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/insert.py
--rw-rw-rw-  2.0 fat    28667 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/layer.py
--rw-rw-rw-  2.0 fat    14252 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/layout.py
--rw-rw-rw-  2.0 fat    13044 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/leader.py
--rw-rw-rw-  2.0 fat     4718 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/light.py
--rw-rw-rw-  2.0 fat     3718 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/line.py
--rw-rw-rw-  2.0 fat     9737 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/ltype.py
--rw-rw-rw-  2.0 fat    19060 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/lwpolyline.py
--rw-rw-rw-  2.0 fat    19321 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/material.py
--rw-rw-rw-  2.0 fat    17413 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/mesh.py
--rw-rw-rw-  2.0 fat    57411 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/mleader.py
--rw-rw-rw-  2.0 fat    37249 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/mline.py
--rw-rw-rw-  2.0 fat     8385 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/mpolygon.py
--rw-rw-rw-  2.0 fat    48213 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/mtext.py
--rw-rw-rw-  2.0 fat     4351 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/mtext_columns.py
--rw-rw-rw-  2.0 fat     6230 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/objectcollection.py
--rw-rw-rw-  2.0 fat     2151 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/oleframe.py
--rw-rw-rw-  2.0 fat     4332 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/pattern.py
--rw-rw-rw-  2.0 fat     5238 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/point.py
--rw-rw-rw-  2.0 fat    16499 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/polygon.py
--rw-rw-rw-  2.0 fat    40126 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/polyline.py
--rw-rw-rw-  2.0 fat     4822 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/shape.py
--rw-rw-rw-  2.0 fat    10485 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/solid.py
--rw-rw-rw-  2.0 fat     7970 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/spatial_filter.py
--rw-rw-rw-  2.0 fat    23809 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/spline.py
--rw-rw-rw-  2.0 fat     8356 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/subentity.py
--rw-rw-rw-  2.0 fat     5196 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/sun.py
--rw-rw-rw-  2.0 fat     2449 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/table.py
--rw-rw-rw-  2.0 fat    17602 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/text.py
--rw-rw-rw-  2.0 fat     9053 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/textstyle.py
--rw-rw-rw-  2.0 fat     3597 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/tolerance.py
--rw-rw-rw-  2.0 fat     2703 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/ucs.py
--rw-rw-rw-  2.0 fat    14426 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/underlay.py
--rw-rw-rw-  2.0 fat     6040 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/view.py
--rw-rw-rw-  2.0 fat    28334 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/viewport.py
--rw-rw-rw-  2.0 fat     7927 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/visualstyle.py
--rw-rw-rw-  2.0 fat     9970 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/vport.py
--rw-rw-rw-  2.0 fat    17024 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/xdata.py
--rw-rw-rw-  2.0 fat     8531 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/xdict.py
--rw-rw-rw-  2.0 fat     3062 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/xline.py
--rw-rw-rw-  2.0 fat     3191 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/entities/__init__.py
--rw-rw-rw-  2.0 fat    26337 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/fonts/fonts.py
--rw-rw-rw-  2.0 fat     2242 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/fonts/font_face.py
--rw-rw-rw-  2.0 fat    18620 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/fonts/font_manager.py
--rw-rw-rw-  2.0 fat     1702 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/fonts/font_measurements.py
--rw-rw-rw-  2.0 fat      288 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/fonts/font_synonyms.py
--rw-rw-rw-  2.0 fat     1175 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/fonts/glyphs.py
--rw-rw-rw-  2.0 fat    10763 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/fonts/lff.py
--rw-rw-rw-  2.0 fat    35414 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/fonts/shapefile.py
--rw-rw-rw-  2.0 fat     7244 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/fonts/ttfonts.py
--rw-rw-rw-  2.0 fat       64 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/fonts/__init__.py
--rw-rw-rw-  2.0 fat    16748 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/layouts/base.py
--rw-rw-rw-  2.0 fat     4343 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/layouts/blocklayout.py
--rw-rw-rw-  2.0 fat    32460 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/layouts/layout.py
--rw-rw-rw-  2.0 fat    15314 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/layouts/layouts.py
--rw-rw-rw-  2.0 fat      232 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/layouts/__init__.py
--rw-rw-rw-  2.0 fat     8327 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/attributes.py
--rw-rw-rw-  2.0 fat    16560 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/const.py
--rw-rw-rw-  2.0 fat     2715 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/encoding.py
--rw-rw-rw-  2.0 fat    16997 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/extendedtags.py
--rw-rw-rw-  2.0 fat     5363 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/fileindex.py
--rw-rw-rw-  2.0 fat      727 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/hdrvars.py
--rw-rw-rw-  2.0 fat     5469 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/loader.py
--rw-rw-rw-  2.0 fat     7152 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/packedtags.py
--rw-rw-rw-  2.0 fat     6355 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/repair.py
--rw-rw-rw-  2.0 fat    14509 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/tagger.py
--rw-rw-rw-  2.0 fat    14325 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/tags.py
--rw-rw-rw-  2.0 fat    11054 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/tagwriter.py
--rw-rw-rw-  2.0 fat    12000 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/types.py
--rw-rw-rw-  2.0 fat    17303 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/validator.py
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/lldxf/__init__.py
--rw-rw-rw-  2.0 fat    19209 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/arc.py
--rw-rw-rw-  2.0 fat    15532 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/bbox.py
--rw-rw-rw-  2.0 fat     9310 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/bezier.py
--rw-rw-rw-  2.0 fat     2458 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/bezier_interpolation.py
--rw-rw-rw-  2.0 fat     8730 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/box.py
--rw-rw-rw-  2.0 fat    53170 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/bspline.py
--rw-rw-rw-  2.0 fat     5608 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/bulge.py
--rw-rw-rw-  2.0 fat     9135 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/circle.py
--rw-rw-rw-  2.0 fat    33170 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/clipping.py
--rw-rw-rw-  2.0 fat     4319 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/clustering.py
--rw-rw-rw-  2.0 fat    11618 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/construct2d.py
--rw-rw-rw-  2.0 fat    26176 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/construct3d.py
--rw-rw-rw-  2.0 fat     1273 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/cspline.py
--rw-rw-rw-  2.0 fat     9114 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/curvetools.py
--rw-rw-rw-  2.0 fat    21723 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/ellipse.py
--rw-rw-rw-  2.0 fat     4406 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/eulerspiral.py
--rw-rw-rw-  2.0 fat    13190 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/legacy.py
--rw-rw-rw-  2.0 fat    27210 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/linalg.py
--rw-rw-rw-  2.0 fat    10213 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/line.py
--rw-rw-rw-  2.0 fat     3053 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/offset2d.py
--rw-rw-rw-  2.0 fat     8171 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/parametrize.py
--rw-rw-rw-  2.0 fat    15602 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/perlin.py
--rw-rw-rw-  2.0 fat    15934 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/polyline.py
--rw-rw-rw-  2.0 fat    11827 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/rtree.py
--rw-rw-rw-  2.0 fat     4815 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/shape.py
--rw-rw-rw-  2.0 fat    12135 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/transformtools.py
--rw-rw-rw-  2.0 fat     3539 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/triangulation.py
--rw-rw-rw-  2.0 fat    17116 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/ucs.py
--rw-rw-rw-  2.0 fat     6710 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/_bezier3p.py
--rw-rw-rw-  2.0 fat    11876 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/_bezier4p.py
--rw-rw-rw-  2.0 fat     9440 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/_bspline.py
--rw-rw-rw-  2.0 fat    12477 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/_construct.py
--rw-rw-rw-  2.0 fat     2548 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/_ctypes.py
--rw-rw-rw-  2.0 fat    24812 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    22757 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/_matrix44.py
--rw-rw-rw-  2.0 fat    25882 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/_vector.py
--rw-rw-rw-  2.0 fat     1978 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/math/__init__.py
--rw-rw-rw-  2.0 fat     1306 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/path/commands.py
--rw-rw-rw-  2.0 fat    31043 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/path/converter.py
--rw-rw-rw-  2.0 fat     5868 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/path/nesting.py
--rw-rw-rw-  2.0 fat    18224 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/path/path.py
--rw-rw-rw-  2.0 fat    10129 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/path/shapes.py
--rw-rw-rw-  2.0 fat    34213 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/path/tools.py
--rw-rw-rw-  2.0 fat      385 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/path/__init__.py
--rw-rw-rw-  2.0 fat    10125 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/abstract_mtext_renderer.py
--rw-rw-rw-  2.0 fat    20495 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/arrows.py
--rw-rw-rw-  2.0 fat    17745 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/curves.py
--rw-rw-rw-  2.0 fat     4041 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/dimension.py
--rw-rw-rw-  2.0 fat    51443 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/dim_base.py
--rw-rw-rw-  2.0 fat    35702 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/dim_curved.py
--rw-rw-rw-  2.0 fat     6894 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/dim_diameter.py
--rw-rw-rw-  2.0 fat    24751 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/dim_linear.py
--rw-rw-rw-  2.0 fat     8084 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/dim_ordinate.py
--rw-rw-rw-  2.0 fat    20295 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/dim_radius.py
--rw-rw-rw-  2.0 fat    47170 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/forms.py
--rw-rw-rw-  2.0 fat    25780 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/hatching.py
--rw-rw-rw-  2.0 fat     4728 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/leader.py
--rw-rw-rw-  2.0 fat      664 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/linetypes.py
--rw-rw-rw-  2.0 fat    65258 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/mesh.py
--rw-rw-rw-  2.0 fat    60907 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/mleader.py
--rw-rw-rw-  2.0 fat     8437 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/mline.py
--rw-rw-rw-  2.0 fat     2964 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/point.py
--rw-rw-rw-  2.0 fat     8736 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/polyline.py
--rw-rw-rw-  2.0 fat     7886 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/r12spline.py
--rw-rw-rw-  2.0 fat    22557 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/trace.py
--rw-rw-rw-  2.0 fat     2881 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/_linetypes.py
--rw-rw-rw-  2.0 fat      778 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/render/__init__.py
--rw-rw-rw-  2.0 fat     1050 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/16x16.png
--rw-rw-rw-  2.0 fat     1420 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/24x24.png
--rw-rw-rw-  2.0 fat    10638 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/256x256.png
--rw-rw-rw-  2.0 fat     1758 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/32x32.png
--rw-rw-rw-  2.0 fat     2335 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/48x48.png
--rw-rw-rw-  2.0 fat     3050 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/64x64.png
--rw-rw-rw-  2.0 fat     2090 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/icon-copy-64px.png
--rw-rw-rw-  2.0 fat     3109 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/icon-find-64px.png
--rw-rw-rw-  2.0 fat     2388 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/icon-goto-bookmark-64px.png
--rw-rw-rw-  2.0 fat     2519 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/icon-goto-handle-64px.png
--rw-rw-rw-  2.0 fat     2409 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/icon-goto-line-64px.png
--rw-rw-rw-  2.0 fat     2231 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/icon-left-arrow-64px.png
--rw-rw-rw-  2.0 fat     2322 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/icon-next-entity-64px.png
--rw-rw-rw-  2.0 fat     2320 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/icon-prev-entity-64px.png
--rw-rw-rw-  2.0 fat     2244 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/icon-right-arrow-64px.png
--rw-rw-rw-  2.0 fat     2553 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/icon-show-in-tree-64px.png
--rw-rw-rw-  2.0 fat     2373 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/resources/icon-store-bookmark-64px.png
--rw-rw-rw-  2.0 fat    10650 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/sections/acdsdata.py
--rw-rw-rw-  2.0 fat    16492 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/sections/blocks.py
--rw-rw-rw-  2.0 fat    11639 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/sections/classes.py
--rw-rw-rw-  2.0 fat     4137 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/sections/entities.py
--rw-rw-rw-  2.0 fat    11937 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/sections/header.py
--rw-rw-rw-  2.0 fat    61373 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/sections/headervars.py
--rw-rw-rw-  2.0 fat    27009 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/sections/objects.py
--rw-rw-rw-  2.0 fat    26565 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/sections/table.py
--rw-rw-rw-  2.0 fat     5270 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/sections/tables.py
--rw-rw-rw-  2.0 fat       67 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/sections/__init__.py
--rw-rw-rw-  2.0 fat    19711 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/analyze.py
--rw-rw-rw-  2.0 fat    20440 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/binarydata.py
--rw-rw-rw-  2.0 fat    15737 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/clipping_portal.py
--rw-rw-rw-  2.0 fat     2931 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/codepage.py
--rw-rw-rw-  2.0 fat     7613 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/complex_ltype.py
--rw-rw-rw-  2.0 fat     1782 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/crypt.py
--rw-rw-rw-  2.0 fat     1511 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/debug.py
--rw-rw-rw-  2.0 fat     2325 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/difftags.py
--rw-rw-rw-  2.0 fat     1235 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/handle.py
--rw-rw-rw-  2.0 fat      780 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/indexing.py
--rw-rw-rw-  2.0 fat     2145 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/juliandate.py
--rw-rw-rw-  2.0 fat     6166 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/pattern.py
--rw-rw-rw-  2.0 fat     1224 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/rawloader.py
--rw-rw-rw-  2.0 fat   129174 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/standards.py
--rw-rw-rw-  2.0 fat     6187 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/strip.py
--rw-rw-rw-  2.0 fat     1466 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/test.py
--rw-rw-rw-  2.0 fat    66061 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/text.py
--rw-rw-rw-  2.0 fat    54140 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/text_layout.py
--rw-rw-rw-  2.0 fat     6893 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/text_size.py
--rw-rw-rw-  2.0 fat     3116 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/zipmanager.py
--rw-rw-rw-  2.0 fat   142734 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/_iso_pattern.py
--rw-rw-rw-  2.0 fat     4413 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/src/ezdxf/tools/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       46 b- defN 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf.egg-info/entry_points.txt
--rw-rw-rw-  2.0 fat        2 b- defN 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat    10110 b- defN 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      316 b- defN 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf.egg-info/requires.txt
--rw-rw-rw-  2.0 fat    32756 b- defN 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        6 b- defN 24-Mar-25 08:04 ezdxf-1.3.0b1/src/ezdxf.egg-info/top_level.txt
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/tests/test_01_dxf_entities/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/tests/test_05_tools/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/tests/test_06_math/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/tests/test_07_render/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/tests/test_08_addons/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/tests/test_09_cython_acceleration/
-drwxrwxrwx  2.0 fat        0 b- stor 24-Mar-25 08:04 ezdxf-1.3.0b1/tests/test_10_issues/
--rw-rw-rw-  2.0 fat      410 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/conftest.py
--rw-rw-rw-  2.0 fat     2336 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
--rw-rw-rw-  2.0 fat      780 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
--rw-rw-rw-  2.0 fat     2599 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
--rw-rw-rw-  2.0 fat     1124 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
--rw-rw-rw-  2.0 fat     5667 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
--rw-rw-rw-  2.0 fat      582 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
--rw-rw-rw-  2.0 fat      473 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_011_codepage.py
--rw-rw-rw-  2.0 fat    11593 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py
--rw-rw-rw-  2.0 fat     1191 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
--rw-rw-rw-  2.0 fat     1033 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
--rw-rw-rw-  2.0 fat     4792 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
--rw-rw-rw-  2.0 fat      989 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py
--rw-rw-rw-  2.0 fat     1383 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_018_handle.py
--rw-rw-rw-  2.0 fat     5518 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
--rw-rw-rw-  2.0 fat     8688 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
--rw-rw-rw-  2.0 fat     3787 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
--rw-rw-rw-  2.0 fat      401 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
--rw-rw-rw-  2.0 fat      539 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
--rw-rw-rw-  2.0 fat     2092 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
--rw-rw-rw-  2.0 fat    10917 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_040_tags.py
--rw-rw-rw-  2.0 fat     3073 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
--rw-rw-rw-  2.0 fat     6419 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
--rw-rw-rw-  2.0 fat     1632 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
--rw-rw-rw-  2.0 fat    11265 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
--rw-rw-rw-  2.0 fat     3363 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
--rw-rw-rw-  2.0 fat     1974 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
--rw-rw-rw-  2.0 fat     2321 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
--rw-rw-rw-  2.0 fat      568 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
--rw-rw-rw-  2.0 fat     8797 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
--rw-rw-rw-  2.0 fat     2581 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py
--rw-rw-rw-  2.0 fat     1500 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
--rw-rw-rw-  2.0 fat     1947 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_058_json_tags.py
--rw-rw-rw-  2.0 fat    11689 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py
--rw-rw-rw-  2.0 fat     2893 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_102_appdata.py
--rw-rw-rw-  2.0 fat     2622 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_103_reactors.py
--rw-rw-rw-  2.0 fat     4679 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_104_extension_dict.py
--rw-rw-rw-  2.0 fat    20860 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_105_xdata.py
--rw-rw-rw-  2.0 fat    14169 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_110_dxfentity.py
--rw-rw-rw-  2.0 fat     2433 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
--rw-rw-rw-  2.0 fat     6781 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py
--rw-rw-rw-  2.0 fat      695 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_112b_dxfobj.py
--rw-rw-rw-  2.0 fat     2431 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_113_dxfclass.py
--rw-rw-rw-  2.0 fat     4044 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_114_factory.py
--rw-rw-rw-  2.0 fat     2256 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
--rw-rw-rw-  2.0 fat    15794 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_116_dictionary.py
--rw-rw-rw-  2.0 fat     4999 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py
--rw-rw-rw-  2.0 fat      385 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_118_appid_table_entry.py
--rw-rw-rw-  2.0 fat     1058 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
--rw-rw-rw-  2.0 fat     3003 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_120_style_table_entry.py
--rw-rw-rw-  2.0 fat     2943 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
--rw-rw-rw-  2.0 fat      379 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_122_vport_table_entry.py
--rw-rw-rw-  2.0 fat     1113 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_123_view_table_entry.py
--rw-rw-rw-  2.0 fat     8757 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
--rw-rw-rw-  2.0 fat     1698 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_125_image_def.py
--rw-rw-rw-  2.0 fat     1312 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py
--rw-rw-rw-  2.0 fat     1430 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_127_raster_variables.py
--rw-rw-rw-  2.0 fat     1540 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_128_pdf_definition.py
--rw-rw-rw-  2.0 fat     2778 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_129_xrecord.py
--rw-rw-rw-  2.0 fat     2423 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_130_id_buffer.py
--rw-rw-rw-  2.0 fat     2470 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_131_field_list.py
--rw-rw-rw-  2.0 fat     2435 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_132_layer_filter.py
--rw-rw-rw-  2.0 fat     2153 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_133_sun.py
--rw-rw-rw-  2.0 fat      852 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_134_material.py
--rw-rw-rw-  2.0 fat    11497 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_135_geo_data.py
--rw-rw-rw-  2.0 fat     1087 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_136_vba_project.py
--rw-rw-rw-  2.0 fat     3099 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_137_sortentstable.py
--rw-rw-rw-  2.0 fat      704 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
--rw-rw-rw-  2.0 fat     7570 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_139_user_record.py
--rw-rw-rw-  2.0 fat      714 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_140_block_record.py
--rw-rw-rw-  2.0 fat     9199 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py
--rw-rw-rw-  2.0 fat     1876 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_142_copy_strategy.py
--rw-rw-rw-  2.0 fat     2268 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_143_spatial_filter.py
--rw-rw-rw-  2.0 fat     2141 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py
--rw-rw-rw-  2.0 fat     2231 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/conftest.py
--rw-rw-rw-  2.0 fat     6532 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_200_line.py
--rw-rw-rw-  2.0 fat     4273 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_201_point.py
--rw-rw-rw-  2.0 fat     6827 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_202_circle.py
--rw-rw-rw-  2.0 fat     8949 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_203_arc.py
--rw-rw-rw-  2.0 fat     2852 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_204_shape.py
--rw-rw-rw-  2.0 fat     8274 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_205_solid.py
--rw-rw-rw-  2.0 fat     8476 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_206_text.py
--rw-rw-rw-  2.0 fat     6487 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_207_attdef.py
--rw-rw-rw-  2.0 fat     8628 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_208_attrib.py
--rw-rw-rw-  2.0 fat     2671 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_209_vertex.py
--rw-rw-rw-  2.0 fat     5916 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_210_polyline_1.py
--rw-rw-rw-  2.0 fat    13489 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_210_polyline_2.py
--rw-rw-rw-  2.0 fat     6650 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py
--rw-rw-rw-  2.0 fat     1780 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
--rw-rw-rw-  2.0 fat     7847 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_211_viewport.py
--rw-rw-rw-  2.0 fat    12629 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_212_insert.py
--rw-rw-rw-  2.0 fat     6024 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_213_minsert.py
--rw-rw-rw-  2.0 fat     3284 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_214_block.py
--rw-rw-rw-  2.0 fat     6914 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_215_dimension.py
--rw-rw-rw-  2.0 fat     4907 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
--rw-rw-rw-  2.0 fat    13186 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
--rw-rw-rw-  2.0 fat     6471 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
--rw-rw-rw-  2.0 fat     5535 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
--rw-rw-rw-  2.0 fat     3056 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
--rw-rw-rw-  2.0 fat     7345 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
--rw-rw-rw-  2.0 fat     2066 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
--rw-rw-rw-  2.0 fat     3615 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
--rw-rw-rw-  2.0 fat     6919 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_221_ellipse.py
--rw-rw-rw-  2.0 fat     2223 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_222_xline.py
--rw-rw-rw-  2.0 fat     1493 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_223_ray.py
--rw-rw-rw-  2.0 fat     2176 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_224_group.py
--rw-rw-rw-  2.0 fat    10917 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_225_mtext.py
--rw-rw-rw-  2.0 fat    12226 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_226_spline.py
--rw-rw-rw-  2.0 fat     5529 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
--rw-rw-rw-  2.0 fat    10893 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
--rw-rw-rw-  2.0 fat    15284 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_228_mesh.py
--rw-rw-rw-  2.0 fat     2695 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
--rw-rw-rw-  2.0 fat    21421 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
--rw-rw-rw-  2.0 fat     6587 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
--rw-rw-rw-  2.0 fat     3140 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
--rw-rw-rw-  2.0 fat    12486 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
--rw-rw-rw-  2.0 fat     2274 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_231_underlay.py
--rw-rw-rw-  2.0 fat     5243 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_231_underlay_2.py
--rw-rw-rw-  2.0 fat     2294 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_232_acis.py
--rw-rw-rw-  2.0 fat     6799 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_232_acis_2.py
--rw-rw-rw-  2.0 fat     1854 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_232_surface.py
--rw-rw-rw-  2.0 fat     2695 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_233_helix.py
--rw-rw-rw-  2.0 fat     2040 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_234_light.py
--rw-rw-rw-  2.0 fat     3806 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_235_leader.py
--rw-rw-rw-  2.0 fat    20392 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_236_multileader.py
--rw-rw-rw-  2.0 fat    10992 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_237_mline.py
--rw-rw-rw-  2.0 fat     2356 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_238_tolerance.py
--rw-rw-rw-  2.0 fat    27392 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
--rw-rw-rw-  2.0 fat     4347 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py
--rw-rw-rw-  2.0 fat     1069 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_241_hyperlink.py
--rw-rw-rw-  2.0 fat    11333 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_242_random_transform.py
--rw-rw-rw-  2.0 fat     3725 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_243_replace_entity.py
--rw-rw-rw-  2.0 fat     1445 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
--rw-rw-rw-  2.0 fat     4456 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_245_wipeout.py
--rw-rw-rw-  2.0 fat     6175 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_246_spline_audit.py
--rw-rw-rw-  2.0 fat     8165 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
--rw-rw-rw-  2.0 fat     6003 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_248_mpolygon.py
--rw-rw-rw-  2.0 fat    13682 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
--rw-rw-rw-  2.0 fat     5713 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py
--rw-rw-rw-  2.0 fat     8331 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
--rw-rw-rw-  2.0 fat     7331 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_251_upright.py
--rw-rw-rw-  2.0 fat     4850 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
--rw-rw-rw-  2.0 fat     2082 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_253_ole2frame.py
--rw-rw-rw-  2.0 fat     1039 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_254_get_font_name.py
--rw-rw-rw-  2.0 fat     5149 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_300_layout.py
--rw-rw-rw-  2.0 fat     4274 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
--rw-rw-rw-  2.0 fat     5582 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_302_block_references.py
--rw-rw-rw-  2.0 fat     2695 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py
--rw-rw-rw-  2.0 fat      913 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py
--rw-rw-rw-  2.0 fat     3279 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
--rw-rw-rw-  2.0 fat     2609 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
--rw-rw-rw-  2.0 fat     2343 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_307_groupby.py
--rw-rw-rw-  2.0 fat    17748 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_308_query.py
--rw-rw-rw-  2.0 fat     6382 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_309_query_parser.py
--rw-rw-rw-  2.0 fat     5031 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
--rw-rw-rw-  2.0 fat     5782 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py
--rw-rw-rw-  2.0 fat      647 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_313_redraw_order.py
--rw-rw-rw-  2.0 fat     6128 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py
--rw-rw-rw-  2.0 fat     2750 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py
--rw-rw-rw-  2.0 fat     5208 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
--rw-rw-rw-  2.0 fat     6795 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py
--rw-rw-rw-  2.0 fat     4981 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
--rw-rw-rw-  2.0 fat     2450 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_405_classes.py
--rw-rw-rw-  2.0 fat     9094 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
--rw-rw-rw-  2.0 fat      848 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
--rw-rw-rw-  2.0 fat     3375 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
--rw-rw-rw-  2.0 fat     1433 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
--rw-rw-rw-  2.0 fat     5736 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_410_table.py
--rw-rw-rw-  2.0 fat     6607 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
--rw-rw-rw-  2.0 fat     1058 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
--rw-rw-rw-  2.0 fat     2246 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
--rw-rw-rw-  2.0 fat    18072 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
--rw-rw-rw-  2.0 fat     4638 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
--rw-rw-rw-  2.0 fat    12327 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
--rw-rw-rw-  2.0 fat     6509 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
--rw-rw-rw-  2.0 fat     5656 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py
--rw-rw-rw-  2.0 fat     5434 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
--rw-rw-rw-  2.0 fat      733 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
--rw-rw-rw-  2.0 fat     1240 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
--rw-rw-rw-  2.0 fat     5007 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
--rw-rw-rw-  2.0 fat      769 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
--rw-rw-rw-  2.0 fat     7549 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_424_audit.py
--rw-rw-rw-  2.0 fat     3737 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
--rw-rw-rw-  2.0 fat     2981 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
--rw-rw-rw-  2.0 fat     2416 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
--rw-rw-rw-  2.0 fat     2533 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
--rw-rw-rw-  2.0 fat     7813 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_429_xclip.py
--rw-rw-rw-  2.0 fat   112800 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/conftest.py
--rw-rw-rw-  2.0 fat     5510 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_500_units.py
--rw-rw-rw-  2.0 fat     2665 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_501_truecolor.py
--rw-rw-rw-  2.0 fat     1021 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_502_raw_color.py
--rw-rw-rw-  2.0 fat     1695 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_503_indexing.py
--rw-rw-rw-  2.0 fat     1442 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_504_suppress_zeros.py
--rw-rw-rw-  2.0 fat      216 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_506_version.py
--rw-rw-rw-  2.0 fat      657 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_508_read_zip.py
--rw-rw-rw-  2.0 fat     1445 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_509_comments.py
--rw-rw-rw-  2.0 fat     1185 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_510_byte_stream.py
--rw-rw-rw-  2.0 fat     4239 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_511_bit_stream.py
--rw-rw-rw-  2.0 fat     5595 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_512_pattern.py
--rw-rw-rw-  2.0 fat     2372 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_513_reorder_entities.py
--rw-rw-rw-  2.0 fat    18181 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_514_text.py
--rw-rw-rw-  2.0 fat     9361 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_515a_fonts_truetype.py
--rw-rw-rw-  2.0 fat     4752 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_515b_fonts_shapefiles.py
--rw-rw-rw-  2.0 fat     2469 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_515c_fonts_lff.py
--rw-rw-rw-  2.0 fat     4002 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_516_zoom.py
--rw-rw-rw-  2.0 fat    34209 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_517_text_layout.py
--rw-rw-rw-  2.0 fat      474 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_518_header_guid.py
--rw-rw-rw-  2.0 fat     3716 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_519_mtext_editor.py
--rw-rw-rw-  2.0 fat     3205 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_520_mtext_context.py
--rw-rw-rw-  2.0 fat    24496 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_521_mtext_parser.py
--rw-rw-rw-  2.0 fat     3863 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_522_text_scanner.py
--rw-rw-rw-  2.0 fat     5564 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_523_text_size.py
--rw-rw-rw-  2.0 fat     5063 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_524_block_reference_manager.py
--rw-rw-rw-  2.0 fat      773 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_525_transparency.py
--rw-rw-rw-  2.0 fat     2133 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_526_explode.py
--rw-rw-rw-  2.0 fat    13521 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_527_gfxattribs.py
--rw-rw-rw-  2.0 fat     2748 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_528_difftags.py
--rw-rw-rw-  2.0 fat     6700 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_529_acis_sat.py
--rw-rw-rw-  2.0 fat     2062 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_530_acis_sab.py
--rw-rw-rw-  2.0 fat    12366 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_531_acis_entities.py
--rw-rw-rw-  2.0 fat     7533 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_532_acis_mesh.py
--rw-rw-rw-  2.0 fat    43259 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_533_shapefiles.py
--rw-rw-rw-  2.0 fat     1034 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_534_dwg_info.py
--rw-rw-rw-  2.0 fat    48174 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_535_xref_basic.py
--rw-rw-rw-  2.0 fat    27614 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_536_xref_conflict.py
--rw-rw-rw-  2.0 fat     6887 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_537_transform.py
--rw-rw-rw-  2.0 fat     2246 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
--rw-rw-rw-  2.0 fat    17771 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_539_npshapes.py
--rw-rw-rw-  2.0 fat     2605 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_540_lff_parser.py
--rw-rw-rw-  2.0 fat     1206 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_541_clipping_portal.py
--rw-rw-rw-  2.0 fat     1400 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_542_itertools.py
--rw-rw-rw-  2.0 fat    11705 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_543_select.py
--rw-rw-rw-  2.0 fat     1264 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_05_tools/test_544_revcloud.py
--rw-rw-rw-  2.0 fat     4026 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/conftest.py
--rw-rw-rw-  2.0 fat     7503 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_600_base.py
--rw-rw-rw-  2.0 fat     2098 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_601_bulge.py
--rw-rw-rw-  2.0 fat    14661 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_602_vec3.py
--rw-rw-rw-  2.0 fat     8956 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_603_vec2.py
--rw-rw-rw-  2.0 fat     2829 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_604_banded_matrix.py
--rw-rw-rw-  2.0 fat     9709 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_604_linalg.py
--rw-rw-rw-  2.0 fat    14118 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_605_matrix44.py
--rw-rw-rw-  2.0 fat     5888 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_606_convexhull.py
--rw-rw-rw-  2.0 fat     1010 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_607_perlin_noise.py
--rw-rw-rw-  2.0 fat     3833 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_608_intersection_line_line_2d.py
--rw-rw-rw-  2.0 fat     1676 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_609_point_on_line.py
--rw-rw-rw-  2.0 fat     3171 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_610_ocs.py
--rw-rw-rw-  2.0 fat     7529 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_611_ucs.py
--rw-rw-rw-  2.0 fat     1831 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_612_ucs_pass_trough.py
--rw-rw-rw-  2.0 fat     6332 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_613_is_point_in_polygon_2d.py
--rw-rw-rw-  2.0 fat    10913 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_614_construct_3d.py
--rw-rw-rw-  2.0 fat      602 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_615_rytz_axis.py
--rw-rw-rw-  2.0 fat     5215 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_616_plane.py
--rw-rw-rw-  2.0 fat      772 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_617_clockwise_orientation.py
--rw-rw-rw-  2.0 fat     7712 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_618_clipping.py
--rw-rw-rw-  2.0 fat    10108 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_619_greiner_hormann.py
--rw-rw-rw-  2.0 fat     2669 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_620_knot.py
--rw-rw-rw-  2.0 fat    18834 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_621_bspline.py
--rw-rw-rw-  2.0 fat     7652 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_622_bsplineu.py
--rw-rw-rw-  2.0 fat    11314 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_623_rbspline.py
--rw-rw-rw-  2.0 fat    10869 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_624_global_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1247 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_626_local_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1967 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_627_bspline_basis.py
--rw-rw-rw-  2.0 fat    10545 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_629_bezier.py
--rw-rw-rw-  2.0 fat    10900 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_630a_bezier4p_base.py
--rw-rw-rw-  2.0 fat    10354 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_630b_bezier4p_functions.py
--rw-rw-rw-  2.0 fat     1683 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_631_euler_spiral.py
--rw-rw-rw-  2.0 fat     4054 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_632_bezier3p.py
--rw-rw-rw-  2.0 fat    20154 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_640_bbox.py
--rw-rw-rw-  2.0 fat     5393 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_641_construction_ray.py
--rw-rw-rw-  2.0 fat     3673 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_642_construction_line.py
--rw-rw-rw-  2.0 fat     9459 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_643_construction_box.py
--rw-rw-rw-  2.0 fat    11561 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_644_construction_circle.py
--rw-rw-rw-  2.0 fat    10988 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_645_construction_arc.py
--rw-rw-rw-  2.0 fat     3422 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_646_offset_vertices_2d.py
--rw-rw-rw-  2.0 fat     7672 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_647_transform_tools.py
--rw-rw-rw-  2.0 fat     9001 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_648_construction_ellipse.py
--rw-rw-rw-  2.0 fat     4243 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_650_elliptic_arc_span.py
--rw-rw-rw-  2.0 fat     9024 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_651_construction_polyline.py
--rw-rw-rw-  2.0 fat     3212 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_652_approx_param_t.py
--rw-rw-rw-  2.0 fat     5806 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_653_polyline_intersection.py
--rw-rw-rw-  2.0 fat     5193 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_654_rtree.py
--rw-rw-rw-  2.0 fat      788 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_655_dbscan.py
--rw-rw-rw-  2.0 fat      834 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_656_k_means.py
--rw-rw-rw-  2.0 fat     4654 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_657_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    11654 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_658_bevel_tools.py
--rw-rw-rw-  2.0 fat     1875 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py
--rw-rw-rw-  2.0 fat     1428 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
--rw-rw-rw-  2.0 fat     1741 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
--rw-rw-rw-  2.0 fat     3307 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_662_is_convex_polygon_2d.py
--rw-rw-rw-  2.0 fat     1266 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_663_is_axes_aligned_rectange.py
--rw-rw-rw-  2.0 fat    17333 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_664_concave_clipping_polygon.py
--rw-rw-rw-  2.0 fat     7980 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_665_inverted_clipping_polygon.py
--rw-rw-rw-  2.0 fat     1553 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_06_math/test_666_wgs84_transform.py
--rw-rw-rw-  2.0 fat     1466 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_701_arrows.py
--rw-rw-rw-  2.0 fat    17245 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_702_render_forms.py
--rw-rw-rw-  2.0 fat    34554 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_703_mesh_builder.py
--rw-rw-rw-  2.0 fat     4459 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_704_render_linear_dimension.py
--rw-rw-rw-  2.0 fat     1345 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_705_shape.py
--rw-rw-rw-  2.0 fat      483 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_706_random_path.py
--rw-rw-rw-  2.0 fat     5603 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_707_trace.py
--rw-rw-rw-  2.0 fat    34121 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_708a_path.py
--rw-rw-rw-  2.0 fat    27365 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_708b_path_tools.py
--rw-rw-rw-  2.0 fat     3352 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_708c_matplotlib_path_tools.py
--rw-rw-rw-  2.0 fat     3278 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_708d_qpainter_path_tools.py
--rw-rw-rw-  2.0 fat     4589 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_708e_path_shapes.py
--rw-rw-rw-  2.0 fat     4121 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_708f_path_nesting.py
--rw-rw-rw-  2.0 fat     1308 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_709_linetype_renderer.py
--rw-rw-rw-  2.0 fat     2815 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_711_points.py
--rw-rw-rw-  2.0 fat     6594 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_712_render_curved_dimension.py
--rw-rw-rw-  2.0 fat     1472 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_713_mleader_builder.py
--rw-rw-rw-  2.0 fat     1091 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_714_mleader_render_engine.py
--rw-rw-rw-  2.0 fat    11887 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_715_hatching.py
--rw-rw-rw-  2.0 fat     2626 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
--rw-rw-rw-  2.0 fat     4771 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_800_mtext_surrogate.py
--rw-rw-rw-  2.0 fat     1352 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_801_r12spline.py
--rw-rw-rw-  2.0 fat     7881 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_802_table_painter.py
--rw-rw-rw-  2.0 fat    12491 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_803_entities_to_code.py
--rw-rw-rw-  2.0 fat     6844 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_804_importer.py
--rw-rw-rw-  2.0 fat     2362 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_805_pycsg.py
--rw-rw-rw-  2.0 fat    15467 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_806_acadctb.py
--rw-rw-rw-  2.0 fat     4860 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_807_dwg_loader_basics.py
--rw-rw-rw-  2.0 fat    11204 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_810_drawing_properties.py
--rw-rw-rw-  2.0 fat    12549 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_811a_drawing_frontend.py
--rw-rw-rw-  2.0 fat     9101 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_811b_drawing_recorder.py
--rw-rw-rw-  2.0 fat     2898 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_811c_viewport_processing.py
--rw-rw-rw-  2.0 fat     4229 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py
--rw-rw-rw-  2.0 fat    13751 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_813_geo_interface.py
--rw-rw-rw-  2.0 fat    14853 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_814_text2path.py
--rw-rw-rw-  2.0 fat    16239 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_815_dxf_browser.py
--rw-rw-rw-  2.0 fat    11275 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_816_bin_packing.py
--rw-rw-rw-  2.0 fat    12554 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_817_genetic_algorithm.py
--rw-rw-rw-  2.0 fat     9008 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_818_meshex.py
--rw-rw-rw-  2.0 fat     1003 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_819_menger_sponge.py
--rw-rw-rw-  2.0 fat     4433 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_820_openscad.py
--rw-rw-rw-  2.0 fat    15655 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_821_hpgl2.py
--rw-rw-rw-  2.0 fat     1376 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
--rw-rw-rw-  2.0 fat     5284 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_823_drawing_layout.py
--rw-rw-rw-  2.0 fat     3312 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_824_svg_drawing_backend.py
--rw-rw-rw-  2.0 fat     2014 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
--rw-rw-rw-  2.0 fat     3158 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_826_custom_json_backend.py
--rw-rw-rw-  2.0 fat     3388 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_08_addons/test_827_geojson_backend.py
--rw-rw-rw-  2.0 fat     2527 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py
--rw-rw-rw-  2.0 fat     2199 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py
--rw-rw-rw-  2.0 fat     2142 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
--rw-rw-rw-  2.0 fat     3175 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
--rw-rw-rw-  2.0 fat     1463 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
--rw-rw-rw-  2.0 fat     4773 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py
--rw-rw-rw-  2.0 fat     2656 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_10_issues/test_issue_414_bbox_calculation.py
--rw-rw-rw-  2.0 fat     1213 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
--rw-rw-rw-  2.0 fat     2268 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_10_issues/test_issue_574_flattening_error.py
--rw-rw-rw-  2.0 fat     1754 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
--rw-rw-rw-  2.0 fat      682 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_10_issues/test_issue_749_text_layout.py
--rw-rw-rw-  2.0 fat    11094 b- defN 24-Mar-25 08:03 ezdxf-1.3.0b1/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
-853 files, 8882949 bytes uncompressed, 2032820 bytes compressed:  77.1%
+Zip file size: 2194990 bytes, number of entries: 858
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/integration_tests/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/
+-rw-rw-rw-  2.0 fat     1092 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/LICENSE
+-rw-rw-rw-  2.0 fat      329 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/MANIFEST.in
+-rw-rw-rw-  2.0 fat    10111 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/PKG-INFO
+-rw-rw-rw-  2.0 fat     2527 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/pyproject.toml
+-rw-rw-rw-  2.0 fat     7479 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/README.md
+-rw-rw-rw-  2.0 fat       74 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/requirements.txt
+-rw-rw-rw-  2.0 fat       42 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/setup.cfg
+-rw-rw-rw-  2.0 fat     2140 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/integration_tests/data/
+-rw-rw-rw-  2.0 fat      567 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/check_disable_c_ext_by_config_file.py
+-rw-rw-rw-  2.0 fat      541 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/check_disable_c_ext_by_env_var.py
+-rw-rw-rw-  2.0 fat      410 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/conftest.py
+-rw-rw-rw-  2.0 fat     1054 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_acad_table.py
+-rw-rw-rw-  2.0 fat     1339 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_acis_entites.py
+-rw-rw-rw-  2.0 fat     4686 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_all_dimline_styles.py
+-rw-rw-rw-  2.0 fat     4153 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_all_ellipse_transformations.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_anonymous_blocks.py
+-rw-rw-rw-  2.0 fat      577 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_appsettings.py
+-rw-rw-rw-  2.0 fat      871 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_audit_critical_dxf_files.py
+-rw-rw-rw-  2.0 fat     1603 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_audit_layouts.py
+-rw-rw-rw-  2.0 fat     1726 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_complex_line_type_2.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_create_basic_graphics.py
+-rw-rw-rw-  2.0 fat     1921 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_document_guid.py
+-rw-rw-rw-  2.0 fat     1832 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_document_page_setup.py
+-rw-rw-rw-  2.0 fat      998 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_dxf_info_scanning.py
+-rw-rw-rw-  2.0 fat     1299 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_dynblkhelper.py
+-rw-rw-rw-  2.0 fat     1558 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_entities_iterator.py
+-rw-rw-rw-  2.0 fat      934 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_fix_dulicate_handles.py
+-rw-rw-rw-  2.0 fat     1901 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_geo.py
+-rw-rw-rw-  2.0 fat     1250 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_groups.py
+-rw-rw-rw-  2.0 fat      905 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_hpgl2_addon.py
+-rw-rw-rw-  2.0 fat      630 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_ignore_junk_beyond_EOF.py
+-rw-rw-rw-  2.0 fat     1155 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_launcher.py
+-rw-rw-rw-  2.0 fat      631 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_leica_disto_r12.py
+-rw-rw-rw-  2.0 fat      737 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_load_dxf_unicode_notation.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat     2230 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_mtext_columns.py
+-rw-rw-rw-  2.0 fat     2392 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_mtext_explode_addon.py
+-rw-rw-rw-  2.0 fat     1846 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_mtext_text_frame.py
+-rw-rw-rw-  2.0 fat     1053 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_new_table_entries.py
+-rw-rw-rw-  2.0 fat      887 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_none_ascii_read_write.py
+-rw-rw-rw-  2.0 fat     3435 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_odafc.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_open_binary_DXF_files.py
+-rw-rw-rw-  2.0 fat      751 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_open_coord_order_issue.py
+-rw-rw-rw-  2.0 fat     3842 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_open_exotic_dxf_files.py
+-rw-rw-rw-  2.0 fat      879 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_open_R13_R14.py
+-rw-rw-rw-  2.0 fat     3152 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_polyline_entity.py
+-rw-rw-rw-  2.0 fat     1749 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_preserve_binary_data_in_xrecords.py
+-rw-rw-rw-  2.0 fat     6944 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_r12export.py
+-rw-rw-rw-  2.0 fat     6256 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_r12strict.py
+-rw-rw-rw-  2.0 fat     3410 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_r12writer.py
+-rw-rw-rw-  2.0 fat      567 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_read_file_without_handles.py
+-rw-rw-rw-  2.0 fat     1121 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_read_write_modern_entites.py
+-rw-rw-rw-  2.0 fat     7747 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_recover.py
+-rw-rw-rw-  2.0 fat     1959 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_redraw_order.py
+-rw-rw-rw-  2.0 fat     1819 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_rotated_block_attributes.py
+-rw-rw-rw-  2.0 fat      774 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_surface_entities.py
+-rw-rw-rw-  2.0 fat      928 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_write_fixed_meta_data.py
+-rw-rw-rw-  2.0 fat     1806 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_write_without_handles.py
+-rw-rw-rw-  2.0 fat     3638 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_xref_detach.py
+-rw-rw-rw-  2.0 fat     2347 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/test_xref_load_acis.py
+-rw-rw-rw-  2.0 fat     3060 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/AC1003_LINE_Example.dxf
+-rw-rw-rw-  2.0 fat   179505 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/acad_table_with_blk_ref.dxf
+-rw-rw-rw-  2.0 fat     7956 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/ASCII_R12.dxf
+-rw-rw-rw-  2.0 fat     3761 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r12.dxf
+-rw-rw-rw-  2.0 fat    20914 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r13.dxf
+-rw-rw-rw-  2.0 fat    21137 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r14.dxf
+-rw-rw-rw-  2.0 fat    11564 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r2000.dxf
+-rw-rw-rw-  2.0 fat     6424 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/cc_dxflib.dxf
+-rw-rw-rw-  2.0 fat   173753 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/custom_blocks.dxf
+-rw-rw-rw-  2.0 fat    32203 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/duplicate_handles.dxf
+-rw-rw-rw-  2.0 fat    18554 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/dxf_unicode.dxf
+-rw-rw-rw-  2.0 fat    56494 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/dynblks.zip
+-rw-rw-rw-  2.0 fat     1592 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/empty_handles.dxf
+-rw-rw-rw-  2.0 fat    97103 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/groups.dxf
+-rw-rw-rw-  2.0 fat    19533 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/layout_broken_links.dxf
+-rw-rw-rw-  2.0 fat    19506 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/layout_broken_links_2.dxf
+-rw-rw-rw-  2.0 fat    19291 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/layout_missing_block_definition.dxf
+-rw-rw-rw-  2.0 fat    19383 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/layout_missing_block_record.dxf
+-rw-rw-rw-  2.0 fat     9146 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/Leica_Disto_S910.dxf
+-rw-rw-rw-  2.0 fat    17986 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/MODEL.dxf
+-rw-rw-rw-  2.0 fat    25799 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/mtext_columns_R2007.dxf
+-rw-rw-rw-  2.0 fat    23927 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/mtext_columns_R2018.dxf
+-rw-rw-rw-  2.0 fat    98230 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/mtext_framed_columns.dxf
+-rw-rw-rw-  2.0 fat   106574 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/mtext_text_frame.dxf
+-rw-rw-rw-  2.0 fat    12001 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/no_layouts.dxf
+-rw-rw-rw-  2.0 fat    16295 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/PLOTFILE.plt
+-rw-rw-rw-  2.0 fat    28788 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/POLI-ALL210_12.DXF
+-rw-rw-rw-  2.0 fat      144 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+-rw-rw-rw-  2.0 fat   212407 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/recover01.dxf
+-rw-rw-rw-  2.0 fat   115423 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/recover02.dxf
+-rw-rw-rw-  2.0 fat    21178 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/small_r13.dxf
+-rw-rw-rw-  2.0 fat    10326 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/small_r14.dxf
+-rw-rw-rw-  2.0 fat    11286 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/XRECORD_0.bin
+-rw-rw-rw-  2.0 fat    11662 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/XRECORD_1.bin
+-rw-rw-rw-  2.0 fat    15337 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/integration_tests/data/XRECORD_2.bin
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/acc/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/acis/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/addons/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/entities/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/fonts/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/lldxf/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/math/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/path/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/render/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/resources/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/sections/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/tools/
+-rw-rw-rw-  2.0 fat     4841 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/appsettings.py
+-rw-rw-rw-  2.0 fat    19886 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/audit.py
+-rw-rw-rw-  2.0 fat     5324 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/bbox.py
+-rw-rw-rw-  2.0 fat     7872 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/blkrefs.py
+-rw-rw-rw-  2.0 fat    17062 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/colors.py
+-rw-rw-rw-  2.0 fat    33508 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/commands.py
+-rw-rw-rw-  2.0 fat     1549 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/comments.py
+-rw-rw-rw-  2.0 fat    22334 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/disassemble.py
+-rw-rw-rw-  2.0 fat    55319 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/document.py
+-rw-rw-rw-  2.0 fat      832 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/dwginfo.py
+-rw-rw-rw-  2.0 fat     2475 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/dynblkhelper.py
+-rw-rw-rw-  2.0 fat    16254 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entitydb.py
+-rw-rw-rw-  2.0 fat     7495 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/enums.py
+-rw-rw-rw-  2.0 fat    14519 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/explode.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/eztypes.py
+-rw-rw-rw-  2.0 fat    10366 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/filemanagement.py
+-rw-rw-rw-  2.0 fat    12157 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/gfxattribs.py
+-rw-rw-rw-  2.0 fat   107528 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/graphicsfactory.py
+-rw-rw-rw-  2.0 fat     3416 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/groupby.py
+-rw-rw-rw-  2.0 fat    20554 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/npshapes.py
+-rw-rw-rw-  2.0 fat     2876 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/protocols.py
+-rw-rw-rw-  2.0 fat    35308 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/proxygraphic.py
+-rw-rw-rw-  2.0 fat       95 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/py.typed
+-rw-rw-rw-  2.0 fat    22499 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/query.py
+-rw-rw-rw-  2.0 fat     2780 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/queryparser.py
+-rw-rw-rw-  2.0 fat     9564 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/r12strict.py
+-rw-rw-rw-  2.0 fat    31442 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/recover.py
+-rw-rw-rw-  2.0 fat     3515 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/reorder.py
+-rw-rw-rw-  2.0 fat     3926 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/revcloud.py
+-rw-rw-rw-  2.0 fat    11250 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/select.py
+-rw-rw-rw-  2.0 fat    12848 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/transform.py
+-rw-rw-rw-  2.0 fat     5750 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/units.py
+-rw-rw-rw-  2.0 fat     8280 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/upright.py
+-rw-rw-rw-  2.0 fat     9875 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/urecord.py
+-rw-rw-rw-  2.0 fat     1026 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/version.py
+-rw-rw-rw-  2.0 fat    18280 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/xclip.py
+-rw-rw-rw-  2.0 fat    65739 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/xref.py
+-rw-rw-rw-  2.0 fat     2853 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/zoom.py
+-rw-rw-rw-  2.0 fat    10898 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/_options.py
+-rw-rw-rw-  2.0 fat     3138 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/__init__.py
+-rw-rw-rw-  2.0 fat     3259 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/__main__.py
+-rw-rw-rw-  2.0 fat     6788 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/bezier3p.pyx
+-rw-rw-rw-  2.0 fat    11502 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/bezier4p.pyx
+-rw-rw-rw-  2.0 fat    14048 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/bspline.pyx
+-rw-rw-rw-  2.0 fat      252 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/constants.h
+-rw-rw-rw-  2.0 fat    11844 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/construct.pyx
+-rw-rw-rw-  2.0 fat     3161 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/linetypes.pyx
+-rw-rw-rw-  2.0 fat    23976 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/mapbox_earcut.pyx
+-rw-rw-rw-  2.0 fat      385 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/matrix44.pxd
+-rw-rw-rw-  2.0 fat    23703 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/matrix44.pyx
+-rw-rw-rw-  2.0 fat     4705 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/np_support.pyx
+-rw-rw-rw-  2.0 fat     1719 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/vector.pxd
+-rw-rw-rw-  2.0 fat    23377 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/vector.pyx
+-rw-rw-rw-  2.0 fat     1265 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acc/__init__.py
+-rw-rw-rw-  2.0 fat     6398 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/abstract.py
+-rw-rw-rw-  2.0 fat      888 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/api.py
+-rw-rw-rw-  2.0 fat     5489 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/const.py
+-rw-rw-rw-  2.0 fat     6731 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/dbg.py
+-rw-rw-rw-  2.0 fat     2985 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/dxf.py
+-rw-rw-rw-  2.0 fat    28782 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/entities.py
+-rw-rw-rw-  2.0 fat     4093 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/hdr.py
+-rw-rw-rw-  2.0 fat    12834 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/mesh.py
+-rw-rw-rw-  2.0 fat    18695 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/sab.py
+-rw-rw-rw-  2.0 fat    13189 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/sat.py
+-rw-rw-rw-  2.0 fat      120 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/acis/__init__.py
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/
+-rw-rw-rw-  2.0 fat    26415 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/acadctb.py
+-rw-rw-rw-  2.0 fat    22229 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/binpacking.py
+-rw-rw-rw-  2.0 fat    27692 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dimlines.py
+-rw-rw-rw-  2.0 fat    31454 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dxf2code.py
+-rw-rw-rw-  2.0 fat    22005 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/genetic_algorithm.py
+-rw-rw-rw-  2.0 fat    38393 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/geo.py
+-rw-rw-rw-  2.0 fat     2674 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/gerber_D6673.py
+-rw-rw-rw-  2.0 fat    25472 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/importer.py
+-rw-rw-rw-  2.0 fat    17355 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/iterdxf.py
+-rw-rw-rw-  2.0 fat     8946 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/menger_sponge.py
+-rw-rw-rw-  2.0 fat    24787 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/meshex.py
+-rw-rw-rw-  2.0 fat      492 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/mixins.py
+-rw-rw-rw-  2.0 fat     6203 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/mtextsurrogate.py
+-rw-rw-rw-  2.0 fat    13528 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/mtxpl.py
+-rw-rw-rw-  2.0 fat    16307 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/odafc.py
+-rw-rw-rw-  2.0 fat     9456 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/openscad.py
+-rw-rw-rw-  2.0 fat    15878 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/pycsg.py
+-rw-rw-rw-  2.0 fat    22301 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/r12export.py
+-rw-rw-rw-  2.0 fat    27191 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/r12writer.py
+-rw-rw-rw-  2.0 fat     7605 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/sierpinski_pyramid.py
+-rw-rw-rw-  2.0 fat    33167 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/tablepainter.py
+-rw-rw-rw-  2.0 fat    12768 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/text2path.py
+-rw-rw-rw-  2.0 fat     3335 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/xplayer.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/xqt.py
+-rw-rw-rw-  2.0 fat      453 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/__init__.py
+-rw-rw-rw-  2.0 fat     9975 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/browser.py
+-rw-rw-rw-  2.0 fat     1907 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/data.py
+-rw-rw-rw-  2.0 fat       64 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/__init__.py
+-rw-rw-rw-  2.0 fat      820 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/bookmarks.py
+-rw-rw-rw-  2.0 fat    29347 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/browser.py
+-rw-rw-rw-  2.0 fat    14891 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/data.py
+-rw-rw-rw-  2.0 fat    10993 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/find_dialog.py
+-rw-rw-rw-  2.0 fat     1249 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/loader.py
+-rw-rw-rw-  2.0 fat    21111 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/model.py
+-rw-rw-rw-  2.0 fat     6896 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/reflinks.py
+-rw-rw-rw-  2.0 fat     2214 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/tags.py
+-rw-rw-rw-  2.0 fat     1366 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/views.py
+-rw-rw-rw-  2.0 fat      133 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/browser/__init__.py
+-rw-rw-rw-  2.0 fat     9265 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/backend.py
+-rw-rw-rw-  2.0 fat    11113 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/config.py
+-rw-rw-rw-  2.0 fat     1756 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/debug_backend.py
+-rw-rw-rw-  2.0 fat      514 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/debug_utils.py
+-rw-rw-rw-  2.0 fat     7391 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/dxf.py
+-rw-rw-rw-  2.0 fat     7753 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/file_output.py
+-rw-rw-rw-  2.0 fat    44576 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/frontend.py
+-rw-rw-rw-  2.0 fat     1877 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/gfxproxy.py
+-rw-rw-rw-  2.0 fat    20834 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/hpgl2.py
+-rw-rw-rw-  2.0 fat    20101 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/json.py
+-rw-rw-rw-  2.0 fat    18871 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/layout.py
+-rw-rw-rw-  2.0 fat    13209 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/matplotlib.py
+-rw-rw-rw-  2.0 fat     9862 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/mtext_complex.py
+-rw-rw-rw-  2.0 fat    32445 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pipeline.py
+-rw-rw-rw-  2.0 fat    40194 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/properties.py
+-rw-rw-rw-  2.0 fat    18036 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pymupdf.py
+-rw-rw-rw-  2.0 fat    11577 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pyqt.py
+-rw-rw-rw-  2.0 fat    22713 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/qtviewer.py
+-rw-rw-rw-  2.0 fat    16434 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/recorder.py
+-rw-rw-rw-  2.0 fat    16222 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/svg.py
+-rw-rw-rw-  2.0 fat    13023 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/text.py
+-rw-rw-rw-  2.0 fat     1194 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/text_renderer.py
+-rw-rw-rw-  2.0 fat      314 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/type_hints.py
+-rw-rw-rw-  2.0 fat     2559 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/unified_text_renderer.py
+-rw-rw-rw-  2.0 fat      171 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/__init__.py
+-rw-rw-rw-  2.0 fat     3112 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/classes_section.py
+-rw-rw-rw-  2.0 fat      763 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/const.py
+-rw-rw-rw-  2.0 fat     6091 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/crc.py
+-rw-rw-rw-  2.0 fat     3160 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/fileheader.py
+-rw-rw-rw-  2.0 fat    14851 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/header_section.py
+-rw-rw-rw-  2.0 fat     2976 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/loader.py
+-rw-rw-rw-  2.0 fat      141 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/__init__.py
+-rw-rw-rw-  2.0 fat    13443 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/api.py
+-rw-rw-rw-  2.0 fat     8554 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/backend.py
+-rw-rw-rw-  2.0 fat      561 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/deps.py
+-rw-rw-rw-  2.0 fat    16079 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/interpreter.py
+-rw-rw-rw-  2.0 fat     4836 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/page.py
+-rw-rw-rw-  2.0 fat    11766 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/plotter.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/polygon_buffer.py
+-rw-rw-rw-  2.0 fat     5615 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/properties.py
+-rw-rw-rw-  2.0 fat     6222 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/tokenizer.py
+-rw-rw-rw-  2.0 fat    19435 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/viewer.py
+-rw-rw-rw-  2.0 fat      164 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/__init__.py
+-rw-rw-rw-  2.0 fat     5729 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat    21463 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/acad_table.py
+-rw-rw-rw-  2.0 fat     2850 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/acad_xrec_roundtrip.py
+-rw-rw-rw-  2.0 fat    29778 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/acis.py
+-rw-rw-rw-  2.0 fat     4996 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/appdata.py
+-rw-rw-rw-  2.0 fat     1954 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/appid.py
+-rw-rw-rw-  2.0 fat     4942 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/arc.py
+-rw-rw-rw-  2.0 fat    27092 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/attrib.py
+-rw-rw-rw-  2.0 fat     8881 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/block.py
+-rw-rw-rw-  2.0 fat    10586 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/blockrecord.py
+-rw-rw-rw-  2.0 fat    50111 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/boundary_paths.py
+-rw-rw-rw-  2.0 fat     7929 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/circle.py
+-rw-rw-rw-  2.0 fat     3214 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/copy.py
+-rw-rw-rw-  2.0 fat    24981 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dictionary.py
+-rw-rw-rw-  2.0 fat    48717 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dimension.py
+-rw-rw-rw-  2.0 fat    35043 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dimstyle.py
+-rw-rw-rw-  2.0 fat    23813 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dimstyleoverride.py
+-rw-rw-rw-  2.0 fat     4399 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dxfclass.py
+-rw-rw-rw-  2.0 fat    40656 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dxfentity.py
+-rw-rw-rw-  2.0 fat    27114 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dxfgfx.py
+-rw-rw-rw-  2.0 fat    15319 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dxfgroups.py
+-rw-rw-rw-  2.0 fat    23679 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dxfns.py
+-rw-rw-rw-  2.0 fat    13910 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/dxfobj.py
+-rw-rw-rw-  2.0 fat    11186 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/ellipse.py
+-rw-rw-rw-  2.0 fat     4138 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/factory.py
+-rw-rw-rw-  2.0 fat    23747 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/geodata.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/gradient.py
+-rw-rw-rw-  2.0 fat    12263 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/hatch.py
+-rw-rw-rw-  2.0 fat     3944 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/helix.py
+-rw-rw-rw-  2.0 fat     4838 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/idbuffer.py
+-rw-rw-rw-  2.0 fat    27125 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/image.py
+-rw-rw-rw-  2.0 fat    28148 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/insert.py
+-rw-rw-rw-  2.0 fat    28698 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/layer.py
+-rw-rw-rw-  2.0 fat    14278 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/layout.py
+-rw-rw-rw-  2.0 fat    13070 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/leader.py
+-rw-rw-rw-  2.0 fat     4718 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/light.py
+-rw-rw-rw-  2.0 fat     3718 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/line.py
+-rw-rw-rw-  2.0 fat     9763 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/ltype.py
+-rw-rw-rw-  2.0 fat    19055 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/lwpolyline.py
+-rw-rw-rw-  2.0 fat    19352 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/material.py
+-rw-rw-rw-  2.0 fat    17444 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/mesh.py
+-rw-rw-rw-  2.0 fat    57437 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/mleader.py
+-rw-rw-rw-  2.0 fat    37229 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/mline.py
+-rw-rw-rw-  2.0 fat     8385 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/mpolygon.py
+-rw-rw-rw-  2.0 fat    48239 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/mtext.py
+-rw-rw-rw-  2.0 fat     4351 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/mtext_columns.py
+-rw-rw-rw-  2.0 fat     6230 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/objectcollection.py
+-rw-rw-rw-  2.0 fat     2151 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/oleframe.py
+-rw-rw-rw-  2.0 fat     4332 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/pattern.py
+-rw-rw-rw-  2.0 fat     5238 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/point.py
+-rw-rw-rw-  2.0 fat    16525 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/polygon.py
+-rw-rw-rw-  2.0 fat    40126 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/polyline.py
+-rw-rw-rw-  2.0 fat     4822 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/shape.py
+-rw-rw-rw-  2.0 fat    10485 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/solid.py
+-rw-rw-rw-  2.0 fat     7990 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/spatial_filter.py
+-rw-rw-rw-  2.0 fat    23810 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/spline.py
+-rw-rw-rw-  2.0 fat     8382 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/subentity.py
+-rw-rw-rw-  2.0 fat     5196 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/sun.py
+-rw-rw-rw-  2.0 fat     2449 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/table.py
+-rw-rw-rw-  2.0 fat     1341 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/temporary_transform.py
+-rw-rw-rw-  2.0 fat    17633 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/text.py
+-rw-rw-rw-  2.0 fat     9053 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/textstyle.py
+-rw-rw-rw-  2.0 fat     3617 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/tolerance.py
+-rw-rw-rw-  2.0 fat     2703 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/ucs.py
+-rw-rw-rw-  2.0 fat    14452 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/underlay.py
+-rw-rw-rw-  2.0 fat     6040 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/view.py
+-rw-rw-rw-  2.0 fat    28360 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/viewport.py
+-rw-rw-rw-  2.0 fat     7958 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/visualstyle.py
+-rw-rw-rw-  2.0 fat     9970 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/vport.py
+-rw-rw-rw-  2.0 fat    17024 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/xdata.py
+-rw-rw-rw-  2.0 fat     8531 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/xdict.py
+-rw-rw-rw-  2.0 fat     3062 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/xline.py
+-rw-rw-rw-  2.0 fat     3191 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/entities/__init__.py
+-rw-rw-rw-  2.0 fat    26337 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/fonts.py
+-rw-rw-rw-  2.0 fat     2242 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/font_face.py
+-rw-rw-rw-  2.0 fat    18620 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/font_manager.py
+-rw-rw-rw-  2.0 fat     1702 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/font_measurements.py
+-rw-rw-rw-  2.0 fat      288 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/font_synonyms.py
+-rw-rw-rw-  2.0 fat     1175 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/glyphs.py
+-rw-rw-rw-  2.0 fat    10763 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/lff.py
+-rw-rw-rw-  2.0 fat    35414 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/shapefile.py
+-rw-rw-rw-  2.0 fat     7244 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/ttfonts.py
+-rw-rw-rw-  2.0 fat       64 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/fonts/__init__.py
+-rw-rw-rw-  2.0 fat    16748 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/layouts/base.py
+-rw-rw-rw-  2.0 fat     4343 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/layouts/blocklayout.py
+-rw-rw-rw-  2.0 fat    32460 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/layouts/layout.py
+-rw-rw-rw-  2.0 fat    15314 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/layouts/layouts.py
+-rw-rw-rw-  2.0 fat      232 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/layouts/__init__.py
+-rw-rw-rw-  2.0 fat     8327 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/attributes.py
+-rw-rw-rw-  2.0 fat    16560 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/const.py
+-rw-rw-rw-  2.0 fat     2715 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/encoding.py
+-rw-rw-rw-  2.0 fat    16997 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/extendedtags.py
+-rw-rw-rw-  2.0 fat     5363 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/fileindex.py
+-rw-rw-rw-  2.0 fat      727 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/hdrvars.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/loader.py
+-rw-rw-rw-  2.0 fat     7152 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/packedtags.py
+-rw-rw-rw-  2.0 fat     6355 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/repair.py
+-rw-rw-rw-  2.0 fat    14509 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/tagger.py
+-rw-rw-rw-  2.0 fat    14325 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/tags.py
+-rw-rw-rw-  2.0 fat    11054 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/tagwriter.py
+-rw-rw-rw-  2.0 fat    12000 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/types.py
+-rw-rw-rw-  2.0 fat    17303 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/validator.py
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/lldxf/__init__.py
+-rw-rw-rw-  2.0 fat    19209 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/arc.py
+-rw-rw-rw-  2.0 fat    15532 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/bbox.py
+-rw-rw-rw-  2.0 fat     9310 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/bezier.py
+-rw-rw-rw-  2.0 fat     2458 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/bezier_interpolation.py
+-rw-rw-rw-  2.0 fat     8730 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/box.py
+-rw-rw-rw-  2.0 fat    53170 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/bspline.py
+-rw-rw-rw-  2.0 fat     5608 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/bulge.py
+-rw-rw-rw-  2.0 fat     9135 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/circle.py
+-rw-rw-rw-  2.0 fat    33170 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/clipping.py
+-rw-rw-rw-  2.0 fat     4319 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/clustering.py
+-rw-rw-rw-  2.0 fat    11618 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/construct2d.py
+-rw-rw-rw-  2.0 fat    26176 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/construct3d.py
+-rw-rw-rw-  2.0 fat     1273 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/cspline.py
+-rw-rw-rw-  2.0 fat     9114 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/curvetools.py
+-rw-rw-rw-  2.0 fat    21723 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/ellipse.py
+-rw-rw-rw-  2.0 fat     4406 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/eulerspiral.py
+-rw-rw-rw-  2.0 fat    13190 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/legacy.py
+-rw-rw-rw-  2.0 fat    27210 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/linalg.py
+-rw-rw-rw-  2.0 fat    10213 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/line.py
+-rw-rw-rw-  2.0 fat     3053 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/offset2d.py
+-rw-rw-rw-  2.0 fat     8171 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/parametrize.py
+-rw-rw-rw-  2.0 fat    15602 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/perlin.py
+-rw-rw-rw-  2.0 fat    15934 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/polyline.py
+-rw-rw-rw-  2.0 fat    11827 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/rtree.py
+-rw-rw-rw-  2.0 fat     4815 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/shape.py
+-rw-rw-rw-  2.0 fat    12135 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/transformtools.py
+-rw-rw-rw-  2.0 fat     3539 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/triangulation.py
+-rw-rw-rw-  2.0 fat    17116 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/ucs.py
+-rw-rw-rw-  2.0 fat     6710 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_bezier3p.py
+-rw-rw-rw-  2.0 fat    11876 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_bezier4p.py
+-rw-rw-rw-  2.0 fat     9440 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_bspline.py
+-rw-rw-rw-  2.0 fat    12477 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_construct.py
+-rw-rw-rw-  2.0 fat     2548 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_ctypes.py
+-rw-rw-rw-  2.0 fat    24812 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    22757 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_matrix44.py
+-rw-rw-rw-  2.0 fat    25882 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/_vector.py
+-rw-rw-rw-  2.0 fat     1978 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/math/__init__.py
+-rw-rw-rw-  2.0 fat     1306 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/commands.py
+-rw-rw-rw-  2.0 fat    31043 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/converter.py
+-rw-rw-rw-  2.0 fat     5868 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/nesting.py
+-rw-rw-rw-  2.0 fat    18224 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/path.py
+-rw-rw-rw-  2.0 fat    10129 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/shapes.py
+-rw-rw-rw-  2.0 fat    34213 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/tools.py
+-rw-rw-rw-  2.0 fat      385 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/path/__init__.py
+-rw-rw-rw-  2.0 fat    10125 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/abstract_mtext_renderer.py
+-rw-rw-rw-  2.0 fat    20495 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/arrows.py
+-rw-rw-rw-  2.0 fat    17745 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/curves.py
+-rw-rw-rw-  2.0 fat     4041 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dimension.py
+-rw-rw-rw-  2.0 fat    51443 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dim_base.py
+-rw-rw-rw-  2.0 fat    35702 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dim_curved.py
+-rw-rw-rw-  2.0 fat     6894 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dim_diameter.py
+-rw-rw-rw-  2.0 fat    24751 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dim_linear.py
+-rw-rw-rw-  2.0 fat     8084 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dim_ordinate.py
+-rw-rw-rw-  2.0 fat    20295 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/dim_radius.py
+-rw-rw-rw-  2.0 fat    47170 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/forms.py
+-rw-rw-rw-  2.0 fat    25780 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/hatching.py
+-rw-rw-rw-  2.0 fat     4728 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/leader.py
+-rw-rw-rw-  2.0 fat      664 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/linetypes.py
+-rw-rw-rw-  2.0 fat    65258 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/mesh.py
+-rw-rw-rw-  2.0 fat    60907 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/mleader.py
+-rw-rw-rw-  2.0 fat     8437 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/mline.py
+-rw-rw-rw-  2.0 fat     2964 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/point.py
+-rw-rw-rw-  2.0 fat     8736 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/polyline.py
+-rw-rw-rw-  2.0 fat     7886 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/r12spline.py
+-rw-rw-rw-  2.0 fat    22557 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/trace.py
+-rw-rw-rw-  2.0 fat     2881 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/_linetypes.py
+-rw-rw-rw-  2.0 fat      778 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/render/__init__.py
+-rw-rw-rw-  2.0 fat     1050 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/16x16.png
+-rw-rw-rw-  2.0 fat     1420 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/24x24.png
+-rw-rw-rw-  2.0 fat    10638 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/256x256.png
+-rw-rw-rw-  2.0 fat     1758 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/32x32.png
+-rw-rw-rw-  2.0 fat     2335 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/48x48.png
+-rw-rw-rw-  2.0 fat     3050 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/64x64.png
+-rw-rw-rw-  2.0 fat     2090 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-copy-64px.png
+-rw-rw-rw-  2.0 fat     3109 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-find-64px.png
+-rw-rw-rw-  2.0 fat     2388 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-bookmark-64px.png
+-rw-rw-rw-  2.0 fat     2519 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-handle-64px.png
+-rw-rw-rw-  2.0 fat     2409 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-line-64px.png
+-rw-rw-rw-  2.0 fat     2231 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-left-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2322 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-next-entity-64px.png
+-rw-rw-rw-  2.0 fat     2320 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-prev-entity-64px.png
+-rw-rw-rw-  2.0 fat     2244 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-right-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2553 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-show-in-tree-64px.png
+-rw-rw-rw-  2.0 fat     2373 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/resources/icon-store-bookmark-64px.png
+-rw-rw-rw-  2.0 fat    10650 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/acdsdata.py
+-rw-rw-rw-  2.0 fat    16492 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/blocks.py
+-rw-rw-rw-  2.0 fat    11639 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/classes.py
+-rw-rw-rw-  2.0 fat     4137 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/entities.py
+-rw-rw-rw-  2.0 fat    11937 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/header.py
+-rw-rw-rw-  2.0 fat    61373 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/headervars.py
+-rw-rw-rw-  2.0 fat    27009 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/objects.py
+-rw-rw-rw-  2.0 fat    26565 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/table.py
+-rw-rw-rw-  2.0 fat     5270 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/tables.py
+-rw-rw-rw-  2.0 fat       67 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/sections/__init__.py
+-rw-rw-rw-  2.0 fat    19711 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/analyze.py
+-rw-rw-rw-  2.0 fat    20440 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/binarydata.py
+-rw-rw-rw-  2.0 fat    15737 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/clipping_portal.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/codepage.py
+-rw-rw-rw-  2.0 fat     7613 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/complex_ltype.py
+-rw-rw-rw-  2.0 fat     1782 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/crypt.py
+-rw-rw-rw-  2.0 fat     1511 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/debug.py
+-rw-rw-rw-  2.0 fat     2325 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/difftags.py
+-rw-rw-rw-  2.0 fat     1235 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/handle.py
+-rw-rw-rw-  2.0 fat      780 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/indexing.py
+-rw-rw-rw-  2.0 fat     2145 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/juliandate.py
+-rw-rw-rw-  2.0 fat     6166 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/pattern.py
+-rw-rw-rw-  2.0 fat     1224 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/rawloader.py
+-rw-rw-rw-  2.0 fat   129174 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/standards.py
+-rw-rw-rw-  2.0 fat     6187 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/strip.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/test.py
+-rw-rw-rw-  2.0 fat    66061 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/text.py
+-rw-rw-rw-  2.0 fat    54140 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/text_layout.py
+-rw-rw-rw-  2.0 fat     6893 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/text_size.py
+-rw-rw-rw-  2.0 fat     3116 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/zipmanager.py
+-rw-rw-rw-  2.0 fat   142734 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/_iso_pattern.py
+-rw-rw-rw-  2.0 fat     4413 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/src/ezdxf/tools/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat       46 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat    10111 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      316 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat    33000 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-18 07:42 ezdxf-1.3.0rc0/src/ezdxf.egg-info/top_level.txt
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_05_tools/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_06_math/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_07_render/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_08_addons/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/
+drwxrwxrwx  2.0 fat        0 b- stor 24-Apr-18 07:42 ezdxf-1.3.0rc0/tests/test_10_issues/
+-rw-rw-rw-  2.0 fat      410 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/conftest.py
+-rw-rw-rw-  2.0 fat     2336 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+-rw-rw-rw-  2.0 fat      780 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+-rw-rw-rw-  2.0 fat     2599 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+-rw-rw-rw-  2.0 fat     1124 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+-rw-rw-rw-  2.0 fat     5667 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+-rw-rw-rw-  2.0 fat      582 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+-rw-rw-rw-  2.0 fat      473 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+-rw-rw-rw-  2.0 fat    11593 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+-rw-rw-rw-  2.0 fat     1191 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+-rw-rw-rw-  2.0 fat     1033 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+-rw-rw-rw-  2.0 fat     4792 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+-rw-rw-rw-  2.0 fat      989 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+-rw-rw-rw-  2.0 fat     1383 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_018_handle.py
+-rw-rw-rw-  2.0 fat     5518 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+-rw-rw-rw-  2.0 fat     8688 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+-rw-rw-rw-  2.0 fat     3787 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+-rw-rw-rw-  2.0 fat      401 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+-rw-rw-rw-  2.0 fat      539 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+-rw-rw-rw-  2.0 fat     2092 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_040_tags.py
+-rw-rw-rw-  2.0 fat     3073 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+-rw-rw-rw-  2.0 fat     6419 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+-rw-rw-rw-  2.0 fat     1632 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+-rw-rw-rw-  2.0 fat    11265 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+-rw-rw-rw-  2.0 fat     3363 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+-rw-rw-rw-  2.0 fat     1974 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+-rw-rw-rw-  2.0 fat     2321 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+-rw-rw-rw-  2.0 fat      568 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+-rw-rw-rw-  2.0 fat     8797 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+-rw-rw-rw-  2.0 fat     2581 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py
+-rw-rw-rw-  2.0 fat     1500 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+-rw-rw-rw-  2.0 fat     1947 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_058_json_tags.py
+-rw-rw-rw-  2.0 fat    11689 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+-rw-rw-rw-  2.0 fat     2893 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_102_appdata.py
+-rw-rw-rw-  2.0 fat     2622 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_103_reactors.py
+-rw-rw-rw-  2.0 fat     4679 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_104_extension_dict.py
+-rw-rw-rw-  2.0 fat    20860 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_105_xdata.py
+-rw-rw-rw-  2.0 fat    14169 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_110_dxfentity.py
+-rw-rw-rw-  2.0 fat     2433 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+-rw-rw-rw-  2.0 fat     6781 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+-rw-rw-rw-  2.0 fat      695 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_112b_dxfobj.py
+-rw-rw-rw-  2.0 fat     2431 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_113_dxfclass.py
+-rw-rw-rw-  2.0 fat     4044 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_114_factory.py
+-rw-rw-rw-  2.0 fat     2256 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+-rw-rw-rw-  2.0 fat    15794 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_116_dictionary.py
+-rw-rw-rw-  2.0 fat     4999 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+-rw-rw-rw-  2.0 fat      385 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+-rw-rw-rw-  2.0 fat     3003 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_120_style_table_entry.py
+-rw-rw-rw-  2.0 fat     2943 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+-rw-rw-rw-  2.0 fat      379 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+-rw-rw-rw-  2.0 fat     1113 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_123_view_table_entry.py
+-rw-rw-rw-  2.0 fat     8757 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_125_image_def.py
+-rw-rw-rw-  2.0 fat     1312 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+-rw-rw-rw-  2.0 fat     1430 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_127_raster_variables.py
+-rw-rw-rw-  2.0 fat     1540 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_128_pdf_definition.py
+-rw-rw-rw-  2.0 fat     2778 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_129_xrecord.py
+-rw-rw-rw-  2.0 fat     2423 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_130_id_buffer.py
+-rw-rw-rw-  2.0 fat     2470 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_131_field_list.py
+-rw-rw-rw-  2.0 fat     2435 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_132_layer_filter.py
+-rw-rw-rw-  2.0 fat     2153 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_133_sun.py
+-rw-rw-rw-  2.0 fat      852 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_134_material.py
+-rw-rw-rw-  2.0 fat    11497 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_135_geo_data.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_136_vba_project.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_137_sortentstable.py
+-rw-rw-rw-  2.0 fat      704 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+-rw-rw-rw-  2.0 fat     7570 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_139_user_record.py
+-rw-rw-rw-  2.0 fat      714 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_140_block_record.py
+-rw-rw-rw-  2.0 fat     9199 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+-rw-rw-rw-  2.0 fat     1876 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_142_copy_strategy.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_143_spatial_filter.py
+-rw-rw-rw-  2.0 fat     2141 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py
+-rw-rw-rw-  2.0 fat     2231 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/conftest.py
+-rw-rw-rw-  2.0 fat     6532 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_200_line.py
+-rw-rw-rw-  2.0 fat     4273 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_201_point.py
+-rw-rw-rw-  2.0 fat     6827 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_202_circle.py
+-rw-rw-rw-  2.0 fat     8949 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_203_arc.py
+-rw-rw-rw-  2.0 fat     2852 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_204_shape.py
+-rw-rw-rw-  2.0 fat     8274 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_205_solid.py
+-rw-rw-rw-  2.0 fat     8476 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_206_text.py
+-rw-rw-rw-  2.0 fat     6487 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_207_attdef.py
+-rw-rw-rw-  2.0 fat     8628 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_208_attrib.py
+-rw-rw-rw-  2.0 fat     2671 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_209_vertex.py
+-rw-rw-rw-  2.0 fat     5916 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_1.py
+-rw-rw-rw-  2.0 fat    13489 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_2.py
+-rw-rw-rw-  2.0 fat     6650 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+-rw-rw-rw-  2.0 fat     1780 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+-rw-rw-rw-  2.0 fat     7847 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_211_viewport.py
+-rw-rw-rw-  2.0 fat    12629 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_212_insert.py
+-rw-rw-rw-  2.0 fat     6024 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_213_minsert.py
+-rw-rw-rw-  2.0 fat     3284 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_214_block.py
+-rw-rw-rw-  2.0 fat     6914 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_215_dimension.py
+-rw-rw-rw-  2.0 fat     4907 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+-rw-rw-rw-  2.0 fat    13186 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+-rw-rw-rw-  2.0 fat     6471 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+-rw-rw-rw-  2.0 fat     5535 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+-rw-rw-rw-  2.0 fat     3056 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+-rw-rw-rw-  2.0 fat     7345 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+-rw-rw-rw-  2.0 fat     2066 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+-rw-rw-rw-  2.0 fat     3615 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+-rw-rw-rw-  2.0 fat     6919 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_221_ellipse.py
+-rw-rw-rw-  2.0 fat     2223 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_222_xline.py
+-rw-rw-rw-  2.0 fat     1493 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_223_ray.py
+-rw-rw-rw-  2.0 fat     2176 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_224_group.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_225_mtext.py
+-rw-rw-rw-  2.0 fat    12226 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_226_spline.py
+-rw-rw-rw-  2.0 fat     5529 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+-rw-rw-rw-  2.0 fat    10893 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+-rw-rw-rw-  2.0 fat    15284 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_228_mesh.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+-rw-rw-rw-  2.0 fat    21421 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+-rw-rw-rw-  2.0 fat     6587 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+-rw-rw-rw-  2.0 fat     3140 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+-rw-rw-rw-  2.0 fat    12486 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+-rw-rw-rw-  2.0 fat     2274 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_231_underlay.py
+-rw-rw-rw-  2.0 fat     5243 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_231_underlay_2.py
+-rw-rw-rw-  2.0 fat     2294 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232a_add_acis.py
+-rw-rw-rw-  2.0 fat     7614 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232b_acis_export.py
+-rw-rw-rw-  2.0 fat     1854 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232c_acis_surface.py
+-rw-rw-rw-  2.0 fat     4215 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232d_acis_copy.py
+-rw-rw-rw-  2.0 fat     1936 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232e_acis_transform.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_233_helix.py
+-rw-rw-rw-  2.0 fat     2040 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_234_light.py
+-rw-rw-rw-  2.0 fat     3806 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_235_leader.py
+-rw-rw-rw-  2.0 fat    20392 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_236_multileader.py
+-rw-rw-rw-  2.0 fat    10992 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_237_mline.py
+-rw-rw-rw-  2.0 fat     2356 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_238_tolerance.py
+-rw-rw-rw-  2.0 fat    27392 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+-rw-rw-rw-  2.0 fat     4347 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_241_hyperlink.py
+-rw-rw-rw-  2.0 fat    11333 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_242_random_transform.py
+-rw-rw-rw-  2.0 fat     3725 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_243_replace_entity.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+-rw-rw-rw-  2.0 fat     4456 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_245_wipeout.py
+-rw-rw-rw-  2.0 fat     6175 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_246_spline_audit.py
+-rw-rw-rw-  2.0 fat     8165 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+-rw-rw-rw-  2.0 fat     6003 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_248_mpolygon.py
+-rw-rw-rw-  2.0 fat    13682 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+-rw-rw-rw-  2.0 fat     5713 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+-rw-rw-rw-  2.0 fat     8331 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+-rw-rw-rw-  2.0 fat     7331 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_251_upright.py
+-rw-rw-rw-  2.0 fat     4850 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat     2082 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_253_ole2frame.py
+-rw-rw-rw-  2.0 fat     1039 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_254_get_font_name.py
+-rw-rw-rw-  2.0 fat     5149 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_300_layout.py
+-rw-rw-rw-  2.0 fat     4274 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+-rw-rw-rw-  2.0 fat     5582 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_302_block_references.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+-rw-rw-rw-  2.0 fat      913 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+-rw-rw-rw-  2.0 fat     3279 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+-rw-rw-rw-  2.0 fat     2609 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+-rw-rw-rw-  2.0 fat     2343 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_307_groupby.py
+-rw-rw-rw-  2.0 fat    17748 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_308_query.py
+-rw-rw-rw-  2.0 fat     6382 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_309_query_parser.py
+-rw-rw-rw-  2.0 fat     5031 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+-rw-rw-rw-  2.0 fat     5782 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+-rw-rw-rw-  2.0 fat      647 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_313_redraw_order.py
+-rw-rw-rw-  2.0 fat     6128 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+-rw-rw-rw-  2.0 fat     2750 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+-rw-rw-rw-  2.0 fat     5208 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+-rw-rw-rw-  2.0 fat     6795 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+-rw-rw-rw-  2.0 fat     4981 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+-rw-rw-rw-  2.0 fat     2450 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_405_classes.py
+-rw-rw-rw-  2.0 fat     9094 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+-rw-rw-rw-  2.0 fat      848 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+-rw-rw-rw-  2.0 fat     3375 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+-rw-rw-rw-  2.0 fat     1433 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+-rw-rw-rw-  2.0 fat     5736 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_410_table.py
+-rw-rw-rw-  2.0 fat     6607 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+-rw-rw-rw-  2.0 fat    18072 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+-rw-rw-rw-  2.0 fat     4638 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+-rw-rw-rw-  2.0 fat    12327 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+-rw-rw-rw-  2.0 fat     6509 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+-rw-rw-rw-  2.0 fat     5656 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+-rw-rw-rw-  2.0 fat     5434 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+-rw-rw-rw-  2.0 fat      733 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+-rw-rw-rw-  2.0 fat     1240 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+-rw-rw-rw-  2.0 fat     5007 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+-rw-rw-rw-  2.0 fat      769 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+-rw-rw-rw-  2.0 fat     7549 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_424_audit.py
+-rw-rw-rw-  2.0 fat     3737 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+-rw-rw-rw-  2.0 fat     2981 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+-rw-rw-rw-  2.0 fat     2416 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+-rw-rw-rw-  2.0 fat     2533 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+-rw-rw-rw-  2.0 fat     7813 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_429_xclip.py
+-rw-rw-rw-  2.0 fat   112800 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/conftest.py
+-rw-rw-rw-  2.0 fat     5510 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_500_units.py
+-rw-rw-rw-  2.0 fat     2665 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_501_truecolor.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_502_raw_color.py
+-rw-rw-rw-  2.0 fat     1695 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_503_indexing.py
+-rw-rw-rw-  2.0 fat     1442 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_504_suppress_zeros.py
+-rw-rw-rw-  2.0 fat      216 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_506_version.py
+-rw-rw-rw-  2.0 fat      657 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_508_read_zip.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_509_comments.py
+-rw-rw-rw-  2.0 fat     1185 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_510_byte_stream.py
+-rw-rw-rw-  2.0 fat     4239 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_511_bit_stream.py
+-rw-rw-rw-  2.0 fat     5595 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_512_pattern.py
+-rw-rw-rw-  2.0 fat     2372 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_513_reorder_entities.py
+-rw-rw-rw-  2.0 fat    18181 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_514_text.py
+-rw-rw-rw-  2.0 fat     9361 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_515a_fonts_truetype.py
+-rw-rw-rw-  2.0 fat     4752 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_515b_fonts_shapefiles.py
+-rw-rw-rw-  2.0 fat     2469 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_515c_fonts_lff.py
+-rw-rw-rw-  2.0 fat     4002 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_516_zoom.py
+-rw-rw-rw-  2.0 fat    34209 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_517_text_layout.py
+-rw-rw-rw-  2.0 fat      474 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_518_header_guid.py
+-rw-rw-rw-  2.0 fat     3716 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_519_mtext_editor.py
+-rw-rw-rw-  2.0 fat     3205 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_520_mtext_context.py
+-rw-rw-rw-  2.0 fat    24496 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_521_mtext_parser.py
+-rw-rw-rw-  2.0 fat     3863 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_522_text_scanner.py
+-rw-rw-rw-  2.0 fat     5564 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_523_text_size.py
+-rw-rw-rw-  2.0 fat     5063 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_524_block_reference_manager.py
+-rw-rw-rw-  2.0 fat      773 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_525_transparency.py
+-rw-rw-rw-  2.0 fat     2133 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_526_explode.py
+-rw-rw-rw-  2.0 fat    13521 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_527_gfxattribs.py
+-rw-rw-rw-  2.0 fat     2748 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_528_difftags.py
+-rw-rw-rw-  2.0 fat     6700 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_529_acis_sat.py
+-rw-rw-rw-  2.0 fat     2062 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_530_acis_sab.py
+-rw-rw-rw-  2.0 fat    12357 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_531_acis_entities.py
+-rw-rw-rw-  2.0 fat     7533 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_532_acis_mesh.py
+-rw-rw-rw-  2.0 fat    43259 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_533_shapefiles.py
+-rw-rw-rw-  2.0 fat     1034 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_534_dwg_info.py
+-rw-rw-rw-  2.0 fat    48174 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_535_xref_basic.py
+-rw-rw-rw-  2.0 fat    27614 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_536_xref_conflict.py
+-rw-rw-rw-  2.0 fat     7186 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_537_transform.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+-rw-rw-rw-  2.0 fat    17771 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_539_npshapes.py
+-rw-rw-rw-  2.0 fat     2605 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_540_lff_parser.py
+-rw-rw-rw-  2.0 fat     1206 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_541_clipping_portal.py
+-rw-rw-rw-  2.0 fat     1400 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_542_itertools.py
+-rw-rw-rw-  2.0 fat    11705 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_543_select.py
+-rw-rw-rw-  2.0 fat     1264 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_05_tools/test_544_revcloud.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/conftest.py
+-rw-rw-rw-  2.0 fat     7503 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_600_base.py
+-rw-rw-rw-  2.0 fat     2098 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_601_bulge.py
+-rw-rw-rw-  2.0 fat    14661 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_602_vec3.py
+-rw-rw-rw-  2.0 fat     8956 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_603_vec2.py
+-rw-rw-rw-  2.0 fat     2829 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_604_banded_matrix.py
+-rw-rw-rw-  2.0 fat     9709 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_604_linalg.py
+-rw-rw-rw-  2.0 fat    14118 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_605_matrix44.py
+-rw-rw-rw-  2.0 fat     5888 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_606_convexhull.py
+-rw-rw-rw-  2.0 fat     1010 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_607_perlin_noise.py
+-rw-rw-rw-  2.0 fat     3833 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_608_intersection_line_line_2d.py
+-rw-rw-rw-  2.0 fat     1676 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_609_point_on_line.py
+-rw-rw-rw-  2.0 fat     3171 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_610_ocs.py
+-rw-rw-rw-  2.0 fat     7529 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_611_ucs.py
+-rw-rw-rw-  2.0 fat     1831 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_612_ucs_pass_trough.py
+-rw-rw-rw-  2.0 fat     6332 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_613_is_point_in_polygon_2d.py
+-rw-rw-rw-  2.0 fat    10913 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_614_construct_3d.py
+-rw-rw-rw-  2.0 fat      602 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_615_rytz_axis.py
+-rw-rw-rw-  2.0 fat     5215 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_616_plane.py
+-rw-rw-rw-  2.0 fat      772 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_617_clockwise_orientation.py
+-rw-rw-rw-  2.0 fat     7712 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_618_clipping.py
+-rw-rw-rw-  2.0 fat    10108 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_619_greiner_hormann.py
+-rw-rw-rw-  2.0 fat     2669 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_620_knot.py
+-rw-rw-rw-  2.0 fat    18834 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_621_bspline.py
+-rw-rw-rw-  2.0 fat     7652 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_622_bsplineu.py
+-rw-rw-rw-  2.0 fat    11314 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_623_rbspline.py
+-rw-rw-rw-  2.0 fat    10869 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_624_global_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1247 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_626_local_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1967 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_627_bspline_basis.py
+-rw-rw-rw-  2.0 fat    10545 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_629_bezier.py
+-rw-rw-rw-  2.0 fat    10900 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_630a_bezier4p_base.py
+-rw-rw-rw-  2.0 fat    10354 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_630b_bezier4p_functions.py
+-rw-rw-rw-  2.0 fat     1683 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_631_euler_spiral.py
+-rw-rw-rw-  2.0 fat     4054 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_632_bezier3p.py
+-rw-rw-rw-  2.0 fat    20154 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_640_bbox.py
+-rw-rw-rw-  2.0 fat     5393 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_641_construction_ray.py
+-rw-rw-rw-  2.0 fat     3673 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_642_construction_line.py
+-rw-rw-rw-  2.0 fat     9459 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_643_construction_box.py
+-rw-rw-rw-  2.0 fat    11561 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_644_construction_circle.py
+-rw-rw-rw-  2.0 fat    10988 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_645_construction_arc.py
+-rw-rw-rw-  2.0 fat     3422 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_646_offset_vertices_2d.py
+-rw-rw-rw-  2.0 fat     7672 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_647_transform_tools.py
+-rw-rw-rw-  2.0 fat     9001 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_648_construction_ellipse.py
+-rw-rw-rw-  2.0 fat     4243 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_650_elliptic_arc_span.py
+-rw-rw-rw-  2.0 fat     9024 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_651_construction_polyline.py
+-rw-rw-rw-  2.0 fat     3212 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_652_approx_param_t.py
+-rw-rw-rw-  2.0 fat     5806 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_653_polyline_intersection.py
+-rw-rw-rw-  2.0 fat     5193 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_654_rtree.py
+-rw-rw-rw-  2.0 fat      788 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_655_dbscan.py
+-rw-rw-rw-  2.0 fat      834 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_656_k_means.py
+-rw-rw-rw-  2.0 fat     4654 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_657_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    11654 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_658_bevel_tools.py
+-rw-rw-rw-  2.0 fat     1875 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1428 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1741 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+-rw-rw-rw-  2.0 fat     3307 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_662_is_convex_polygon_2d.py
+-rw-rw-rw-  2.0 fat     1266 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_663_is_axes_aligned_rectange.py
+-rw-rw-rw-  2.0 fat    17333 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_664_concave_clipping_polygon.py
+-rw-rw-rw-  2.0 fat     7980 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_665_inverted_clipping_polygon.py
+-rw-rw-rw-  2.0 fat     1553 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_06_math/test_666_wgs84_transform.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_701_arrows.py
+-rw-rw-rw-  2.0 fat    17245 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_702_render_forms.py
+-rw-rw-rw-  2.0 fat    34554 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_703_mesh_builder.py
+-rw-rw-rw-  2.0 fat     4459 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_704_render_linear_dimension.py
+-rw-rw-rw-  2.0 fat     1345 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_705_shape.py
+-rw-rw-rw-  2.0 fat      483 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_706_random_path.py
+-rw-rw-rw-  2.0 fat     5603 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_707_trace.py
+-rw-rw-rw-  2.0 fat    34121 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_708a_path.py
+-rw-rw-rw-  2.0 fat    27365 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_708b_path_tools.py
+-rw-rw-rw-  2.0 fat     3352 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_708c_matplotlib_path_tools.py
+-rw-rw-rw-  2.0 fat     3278 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_708d_qpainter_path_tools.py
+-rw-rw-rw-  2.0 fat     4589 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_708e_path_shapes.py
+-rw-rw-rw-  2.0 fat     4121 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_708f_path_nesting.py
+-rw-rw-rw-  2.0 fat     1308 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_709_linetype_renderer.py
+-rw-rw-rw-  2.0 fat     2815 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_711_points.py
+-rw-rw-rw-  2.0 fat     6594 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_712_render_curved_dimension.py
+-rw-rw-rw-  2.0 fat     1472 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_713_mleader_builder.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_714_mleader_render_engine.py
+-rw-rw-rw-  2.0 fat    11887 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_715_hatching.py
+-rw-rw-rw-  2.0 fat     2626 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+-rw-rw-rw-  2.0 fat     4771 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_800_mtext_surrogate.py
+-rw-rw-rw-  2.0 fat     1352 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_801_r12spline.py
+-rw-rw-rw-  2.0 fat     7881 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_802_table_painter.py
+-rw-rw-rw-  2.0 fat    12491 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_803_entities_to_code.py
+-rw-rw-rw-  2.0 fat     6844 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_804_importer.py
+-rw-rw-rw-  2.0 fat     2362 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_805_pycsg.py
+-rw-rw-rw-  2.0 fat    15467 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_806_acadctb.py
+-rw-rw-rw-  2.0 fat     4860 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_807_dwg_loader_basics.py
+-rw-rw-rw-  2.0 fat    11204 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_810_drawing_properties.py
+-rw-rw-rw-  2.0 fat    12549 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_811a_drawing_frontend.py
+-rw-rw-rw-  2.0 fat     9101 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_811b_drawing_recorder.py
+-rw-rw-rw-  2.0 fat     2898 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_811c_viewport_processing.py
+-rw-rw-rw-  2.0 fat     4229 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+-rw-rw-rw-  2.0 fat    13751 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_813_geo_interface.py
+-rw-rw-rw-  2.0 fat    14853 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_814_text2path.py
+-rw-rw-rw-  2.0 fat    16239 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_815_dxf_browser.py
+-rw-rw-rw-  2.0 fat    11275 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_816_bin_packing.py
+-rw-rw-rw-  2.0 fat    12554 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_817_genetic_algorithm.py
+-rw-rw-rw-  2.0 fat     9008 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_818_meshex.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_819_menger_sponge.py
+-rw-rw-rw-  2.0 fat     4433 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_820_openscad.py
+-rw-rw-rw-  2.0 fat    15655 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_821_hpgl2.py
+-rw-rw-rw-  2.0 fat     1376 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+-rw-rw-rw-  2.0 fat     5284 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_823_drawing_layout.py
+-rw-rw-rw-  2.0 fat     3312 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_824_svg_drawing_backend.py
+-rw-rw-rw-  2.0 fat     2014 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
+-rw-rw-rw-  2.0 fat     3158 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_826_custom_json_backend.py
+-rw-rw-rw-  2.0 fat     3388 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_08_addons/test_827_geojson_backend.py
+-rw-rw-rw-  2.0 fat     2527 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+-rw-rw-rw-  2.0 fat     2199 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+-rw-rw-rw-  2.0 fat     2142 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+-rw-rw-rw-  2.0 fat     3175 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+-rw-rw-rw-  2.0 fat     1463 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+-rw-rw-rw-  2.0 fat     4773 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+-rw-rw-rw-  2.0 fat     2656 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_414_bbox_calculation.py
+-rw-rw-rw-  2.0 fat     1213 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_574_flattening_error.py
+-rw-rw-rw-  2.0 fat     1754 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+-rw-rw-rw-  2.0 fat      682 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_749_text_layout.py
+-rw-rw-rw-  2.0 fat    11094 b- defN 24-Apr-18 07:41 ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
+858 files, 8903508 bytes uncompressed, 2038206 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -1,2560 +1,2575 @@
-Filename: ezdxf-1.3.0b1/
+Filename: ezdxf-1.3.0rc0/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/
+Filename: ezdxf-1.3.0rc0/integration_tests/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/
+Filename: ezdxf-1.3.0rc0/src/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/
+Filename: ezdxf-1.3.0rc0/tests/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/LICENSE
+Filename: ezdxf-1.3.0rc0/LICENSE
 Comment: 
 
-Filename: ezdxf-1.3.0b1/MANIFEST.in
+Filename: ezdxf-1.3.0rc0/MANIFEST.in
 Comment: 
 
-Filename: ezdxf-1.3.0b1/PKG-INFO
+Filename: ezdxf-1.3.0rc0/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.3.0b1/pyproject.toml
+Filename: ezdxf-1.3.0rc0/pyproject.toml
 Comment: 
 
-Filename: ezdxf-1.3.0b1/README.md
+Filename: ezdxf-1.3.0rc0/README.md
 Comment: 
 
-Filename: ezdxf-1.3.0b1/requirements.txt
+Filename: ezdxf-1.3.0rc0/requirements.txt
 Comment: 
 
-Filename: ezdxf-1.3.0b1/setup.cfg
+Filename: ezdxf-1.3.0rc0/setup.cfg
 Comment: 
 
-Filename: ezdxf-1.3.0b1/setup.py
+Filename: ezdxf-1.3.0rc0/setup.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/
+Filename: ezdxf-1.3.0rc0/integration_tests/data/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/check_disable_c_ext_by_config_file.py
+Filename: ezdxf-1.3.0rc0/integration_tests/check_disable_c_ext_by_config_file.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/check_disable_c_ext_by_env_var.py
+Filename: ezdxf-1.3.0rc0/integration_tests/check_disable_c_ext_by_env_var.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/conftest.py
+Filename: ezdxf-1.3.0rc0/integration_tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_acad_table.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_acad_table.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_all_dimline_styles.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_acis_entites.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_all_ellipse_transformations.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_all_dimline_styles.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_anonymous_blocks.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_all_ellipse_transformations.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_appsettings.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_anonymous_blocks.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_audit_critical_dxf_files.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_appsettings.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_audit_layouts.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_audit_critical_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_complex_line_type_2.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_audit_layouts.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_create_basic_graphics.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_complex_line_type_2.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_document_guid.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_create_basic_graphics.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_document_page_setup.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_document_guid.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_dxf_info_scanning.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_document_page_setup.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_dynblkhelper.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_dxf_info_scanning.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_entities_iterator.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_dynblkhelper.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_fix_dulicate_handles.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_entities_iterator.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_geo.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_fix_dulicate_handles.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_groups.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_geo.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_hpgl2_addon.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_groups.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_ignore_junk_beyond_EOF.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_hpgl2_addon.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_launcher.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_ignore_junk_beyond_EOF.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_leica_disto_r12.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_launcher.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_load_dxf_unicode_notation.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_leica_disto_r12.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_mapbox_earcut.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_load_dxf_unicode_notation.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_mtext_columns.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_mtext_explode_addon.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_mtext_text_frame.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_mtext_explode_addon.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_new_table_entries.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_mtext_text_frame.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_none_ascii_read_write.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_new_table_entries.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_odafc.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_none_ascii_read_write.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_open_binary_DXF_files.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_odafc.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_open_coord_order_issue.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_open_binary_DXF_files.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_open_exotic_dxf_files.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_open_coord_order_issue.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_open_R13_R14.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_open_exotic_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_polyline_entity.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_open_R13_R14.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_preserve_binary_data_in_xrecords.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_polyline_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_r12export.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_preserve_binary_data_in_xrecords.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_r12strict.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_r12export.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_r12writer.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_r12strict.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_read_file_without_handles.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_r12writer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_read_write_modern_entites.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_read_file_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_recover.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_read_write_modern_entites.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_redraw_order.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_recover.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_rotated_block_attributes.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_surface_entities.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_rotated_block_attributes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_write_fixed_meta_data.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_surface_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_write_without_handles.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_write_fixed_meta_data.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/test_xref_detach.py
+Filename: ezdxf-1.3.0rc0/integration_tests/test_write_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/AC1003_LINE_Example.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/test_xref_detach.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/acad_table_with_blk_ref.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/test_xref_load_acis.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/ASCII_R12.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/AC1003_LINE_Example.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/bin_dxf_r12.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/acad_table_with_blk_ref.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/bin_dxf_r13.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/ASCII_R12.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/bin_dxf_r14.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r12.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/bin_dxf_r2000.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/cc_dxflib.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/custom_blocks.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r2000.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/duplicate_handles.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/cc_dxflib.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/dxf_unicode.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/custom_blocks.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/dynblks.zip
+Filename: ezdxf-1.3.0rc0/integration_tests/data/duplicate_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/empty_handles.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/dxf_unicode.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/groups.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/dynblks.zip
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/layout_broken_links.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/empty_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/layout_broken_links_2.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/groups.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/layout_missing_block_definition.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/layout_broken_links.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/layout_missing_block_record.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/layout_broken_links_2.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/Leica_Disto_S910.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/layout_missing_block_definition.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/MODEL.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/layout_missing_block_record.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/mtext_columns_R2007.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/Leica_Disto_S910.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/mtext_columns_R2018.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/MODEL.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/mtext_framed_columns.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/mtext_columns_R2007.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/mtext_text_frame.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/mtext_columns_R2018.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/no_layouts.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/mtext_framed_columns.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/PLOTFILE.plt
+Filename: ezdxf-1.3.0rc0/integration_tests/data/mtext_text_frame.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/POLI-ALL210_12.DXF
+Filename: ezdxf-1.3.0rc0/integration_tests/data/no_layouts.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/PLOTFILE.plt
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/recover01.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/POLI-ALL210_12.DXF
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/recover02.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/small_r13.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/recover01.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/small_r14.dxf
+Filename: ezdxf-1.3.0rc0/integration_tests/data/recover02.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/XRECORD_0.bin
+Filename: ezdxf-1.3.0rc0/integration_tests/data/small_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/XRECORD_1.bin
+Filename: ezdxf-1.3.0rc0/integration_tests/data/small_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.3.0b1/integration_tests/data/XRECORD_2.bin
+Filename: ezdxf-1.3.0rc0/integration_tests/data/XRECORD_0.bin
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/
+Filename: ezdxf-1.3.0rc0/integration_tests/data/XRECORD_1.bin
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf.egg-info/
+Filename: ezdxf-1.3.0rc0/integration_tests/data/XRECORD_2.bin
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acis/
+Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/fonts/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/layouts/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/layouts/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/path/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/path/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/sections/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/appsettings.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/audit.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/bbox.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/appsettings.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/blkrefs.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/audit.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/colors.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/bbox.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/commands.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/blkrefs.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/comments.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/colors.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/disassemble.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/commands.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/document.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/comments.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/dwginfo.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/disassemble.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/dynblkhelper.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/document.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entitydb.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/dwginfo.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/enums.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/dynblkhelper.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/explode.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entitydb.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/eztypes.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/enums.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/filemanagement.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/explode.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/gfxattribs.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/eztypes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/graphicsfactory.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/filemanagement.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/groupby.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/npshapes.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/graphicsfactory.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/protocols.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/groupby.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/proxygraphic.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/npshapes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/py.typed
+Filename: ezdxf-1.3.0rc0/src/ezdxf/protocols.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/query.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/proxygraphic.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/queryparser.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/py.typed
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/r12strict.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/query.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/recover.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/queryparser.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/reorder.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/r12strict.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/revcloud.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/recover.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/select.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/reorder.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/transform.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/revcloud.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/units.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/select.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/upright.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/transform.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/urecord.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/units.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/version.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/upright.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/xclip.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/urecord.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/xref.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/version.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/zoom.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/xclip.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/_options.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/xref.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/zoom.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/__main__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/_options.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/bezier3p.pyx
+Filename: ezdxf-1.3.0rc0/src/ezdxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/bezier4p.pyx
+Filename: ezdxf-1.3.0rc0/src/ezdxf/__main__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/bspline.pyx
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/bezier3p.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/constants.h
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/bezier4p.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/construct.pyx
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/bspline.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/linetypes.pyx
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/constants.h
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/mapbox_earcut.pyx
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/construct.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/matrix44.pxd
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/linetypes.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/matrix44.pyx
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/mapbox_earcut.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/np_support.pyx
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/matrix44.pxd
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/vector.pxd
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/matrix44.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/vector.pyx
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/np_support.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acc/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/vector.pxd
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acis/abstract.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/vector.pyx
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acis/api.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acc/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acis/const.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/abstract.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acis/dbg.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/api.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acis/dxf.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/const.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acis/entities.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/dbg.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acis/hdr.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/dxf.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acis/mesh.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acis/sab.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/hdr.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acis/sat.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/acis/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/sab.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/acisbrowser/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/sat.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/browser/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/acis/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/dwg/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/acadctb.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/binpacking.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/dimlines.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/acadctb.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/dxf2code.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/binpacking.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/genetic_algorithm.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dimlines.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/geo.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dxf2code.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/gerber_D6673.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/importer.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/geo.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/iterdxf.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/gerber_D6673.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/menger_sponge.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/importer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/meshex.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/iterdxf.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/mixins.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/mtextsurrogate.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/meshex.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/mtxpl.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/mixins.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/odafc.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/mtextsurrogate.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/openscad.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/mtxpl.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/pycsg.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/odafc.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/r12export.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/openscad.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/r12writer.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/pycsg.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/sierpinski_pyramid.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/r12export.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/tablepainter.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/r12writer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/text2path.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/sierpinski_pyramid.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/xplayer.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/tablepainter.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/xqt.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/text2path.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/xplayer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/acisbrowser/browser.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/xqt.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/acisbrowser/data.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/acisbrowser/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/browser.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/browser/bookmarks.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/data.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/browser/browser.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/browser/data.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/bookmarks.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/browser/find_dialog.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/browser.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/browser/loader.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/data.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/browser/model.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/find_dialog.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/browser/reflinks.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/loader.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/browser/tags.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/model.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/browser/views.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/reflinks.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/browser/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/backend.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/views.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/config.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/browser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/debug_backend.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/debug_utils.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/config.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/dxf.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/debug_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/file_output.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/debug_utils.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/frontend.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/dxf.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/gfxproxy.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/file_output.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/hpgl2.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/frontend.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/json.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/gfxproxy.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/layout.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/matplotlib.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/json.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/mtext_complex.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/pipeline.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/matplotlib.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/properties.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/mtext_complex.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/pymupdf.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pipeline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/pyqt.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/properties.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/qtviewer.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pymupdf.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/recorder.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pyqt.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/svg.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/qtviewer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/text.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/recorder.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/text_renderer.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/svg.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/type_hints.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/text.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/unified_text_renderer.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/drawing/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/type_hints.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/dwg/classes_section.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/unified_text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/dwg/const.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/dwg/crc.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/classes_section.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/dwg/fileheader.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/const.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/dwg/header_section.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/crc.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/dwg/loader.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/fileheader.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/dwg/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/header_section.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/api.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/loader.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/backend.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/deps.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/api.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/interpreter.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/page.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/deps.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/plotter.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/interpreter.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/polygon_buffer.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/page.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/properties.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/plotter.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/tokenizer.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/polygon_buffer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/viewer.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/properties.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/tokenizer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/acad_proxy_entity.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/viewer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/acad_table.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/acad_xrec_roundtrip.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/acis.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/acad_table.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/appdata.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/acad_xrec_roundtrip.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/appid.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/acis.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/arc.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/appdata.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/attrib.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/appid.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/block.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/arc.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/blockrecord.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/attrib.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/boundary_paths.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/block.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/circle.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/blockrecord.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/copy.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/dictionary.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/circle.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/dimension.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/copy.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/dimstyle.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dictionary.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/dimstyleoverride.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/dxfclass.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dimstyle.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/dxfentity.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dimstyleoverride.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/dxfgfx.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/dxfgroups.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/dxfns.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/dxfobj.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/ellipse.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dxfns.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/factory.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/geodata.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/gradient.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/factory.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/hatch.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/geodata.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/helix.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/gradient.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/idbuffer.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/hatch.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/image.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/helix.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/insert.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/idbuffer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/layer.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/image.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/layout.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/insert.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/leader.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/layer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/light.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/line.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/leader.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/ltype.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/light.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/lwpolyline.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/line.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/material.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/ltype.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/mesh.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/lwpolyline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/mleader.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/material.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/mline.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/mpolygon.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/mleader.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/mtext.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/mline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/mtext_columns.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/objectcollection.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/mtext.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/oleframe.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/pattern.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/objectcollection.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/point.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/oleframe.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/polygon.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/pattern.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/polyline.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/point.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/shape.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/polygon.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/solid.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/polyline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/spatial_filter.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/shape.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/spline.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/solid.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/subentity.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/spatial_filter.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/sun.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/spline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/table.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/subentity.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/text.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/sun.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/textstyle.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/table.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/tolerance.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/temporary_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/ucs.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/text.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/underlay.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/textstyle.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/view.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/tolerance.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/viewport.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/ucs.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/visualstyle.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/underlay.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/vport.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/view.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/xdata.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/viewport.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/xdict.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/visualstyle.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/xline.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/vport.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/entities/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/xdata.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/fonts/fonts.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/xdict.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/fonts/font_face.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/xline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/fonts/font_manager.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/entities/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/fonts/font_measurements.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/fonts.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/fonts/font_synonyms.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/font_face.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/fonts/glyphs.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/font_manager.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/fonts/lff.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/font_measurements.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/fonts/shapefile.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/font_synonyms.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/fonts/ttfonts.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/glyphs.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/fonts/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/lff.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/layouts/base.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/shapefile.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/layouts/blocklayout.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/ttfonts.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/layouts/layout.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/fonts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/layouts/layouts.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/layouts/base.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/layouts/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/layouts/blocklayout.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/attributes.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/layouts/layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/const.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/layouts/layouts.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/encoding.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/layouts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/extendedtags.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/attributes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/fileindex.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/const.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/hdrvars.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/encoding.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/loader.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/extendedtags.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/packedtags.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/fileindex.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/repair.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/hdrvars.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/tagger.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/loader.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/tags.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/packedtags.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/tagwriter.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/repair.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/types.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/tagger.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/validator.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/lldxf/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/tagwriter.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/arc.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/types.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/bbox.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/validator.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/bezier.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/lldxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/bezier_interpolation.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/arc.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/box.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/bbox.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/bspline.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/bezier.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/bulge.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/bezier_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/circle.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/box.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/clipping.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/bspline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/clustering.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/bulge.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/construct2d.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/circle.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/construct3d.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/clipping.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/cspline.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/clustering.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/curvetools.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/construct2d.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/ellipse.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/construct3d.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/eulerspiral.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/cspline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/legacy.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/curvetools.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/linalg.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/line.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/eulerspiral.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/offset2d.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/legacy.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/parametrize.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/linalg.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/perlin.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/line.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/polyline.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/offset2d.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/rtree.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/parametrize.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/shape.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/perlin.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/transformtools.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/polyline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/triangulation.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/rtree.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/ucs.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/shape.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/_bezier3p.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/transformtools.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/_bezier4p.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/triangulation.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/_bspline.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/ucs.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/_construct.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/_ctypes.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/_mapbox_earcut.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_bspline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/_matrix44.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_construct.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/_vector.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_ctypes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/math/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/path/commands.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/path/converter.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/_vector.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/path/nesting.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/math/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/path/path.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/path/commands.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/path/shapes.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/path/converter.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/path/tools.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/path/nesting.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/path/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/path/path.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/abstract_mtext_renderer.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/path/shapes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/arrows.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/path/tools.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/curves.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/path/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/dimension.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/abstract_mtext_renderer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/dim_base.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/arrows.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/dim_curved.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/curves.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/dim_diameter.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/dim_linear.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dim_base.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/dim_ordinate.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dim_curved.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/dim_radius.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dim_diameter.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/forms.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dim_linear.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/hatching.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dim_ordinate.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/leader.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/dim_radius.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/linetypes.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/forms.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/mesh.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/hatching.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/mleader.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/leader.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/mline.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/linetypes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/point.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/polyline.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/mleader.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/r12spline.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/mline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/trace.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/point.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/_linetypes.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/polyline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/render/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/r12spline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/16x16.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/trace.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/24x24.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/_linetypes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/256x256.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/render/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/32x32.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/16x16.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/48x48.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/24x24.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/64x64.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/256x256.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/icon-copy-64px.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/32x32.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/icon-find-64px.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/48x48.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/icon-goto-bookmark-64px.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/64x64.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/icon-goto-handle-64px.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-copy-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/icon-goto-line-64px.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-find-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/icon-left-arrow-64px.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/icon-next-entity-64px.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-handle-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/icon-prev-entity-64px.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-line-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/icon-right-arrow-64px.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-left-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/icon-show-in-tree-64px.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-next-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/resources/icon-store-bookmark-64px.png
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-prev-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/sections/acdsdata.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-right-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/sections/blocks.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-show-in-tree-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/sections/classes.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/resources/icon-store-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/sections/entities.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/acdsdata.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/sections/header.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/blocks.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/sections/headervars.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/classes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/sections/objects.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/sections/table.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/header.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/sections/tables.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/headervars.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/sections/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/objects.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/analyze.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/table.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/binarydata.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/tables.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/clipping_portal.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/sections/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/codepage.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/analyze.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/complex_ltype.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/binarydata.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/crypt.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/clipping_portal.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/debug.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/codepage.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/difftags.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/complex_ltype.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/handle.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/crypt.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/indexing.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/debug.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/juliandate.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/difftags.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/pattern.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/handle.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/rawloader.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/indexing.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/standards.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/juliandate.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/strip.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/pattern.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/test.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/rawloader.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/text.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/standards.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/text_layout.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/strip.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/text_size.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/test.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/zipmanager.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/text.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/_iso_pattern.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/text_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf/tools/__init__.py
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/text_size.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf.egg-info/dependency_links.txt
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/zipmanager.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf.egg-info/entry_points.txt
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/_iso_pattern.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf.egg-info/not-zip-safe
+Filename: ezdxf-1.3.0rc0/src/ezdxf/tools/__init__.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf.egg-info/PKG-INFO
+Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf.egg-info/requires.txt
+Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/entry_points.txt
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf.egg-info/SOURCES.txt
+Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/not-zip-safe
 Comment: 
 
-Filename: ezdxf-1.3.0b1/src/ezdxf.egg-info/top_level.txt
+Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/
+Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/requires.txt
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/
+Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/
+Filename: ezdxf-1.3.0rc0/src/ezdxf.egg-info/top_level.txt
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_09_cython_acceleration/
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_10_issues/
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/conftest.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+Filename: ezdxf-1.3.0rc0/tests/test_10_issues/
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+Filename: ezdxf-1.3.0rc0/tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_018_handle.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_018_handle.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_040_tags.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_040_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_058_json_tags.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_102_appdata.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_103_reactors.py
+Filename: ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_058_json_tags.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_104_extension_dict.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_105_xdata.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_102_appdata.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_110_dxfentity.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_103_reactors.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_104_extension_dict.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_105_xdata.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_112b_dxfobj.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_110_dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_113_dxfclass.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_114_factory.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_112b_dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_116_dictionary.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_113_dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_114_factory.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_116_dictionary.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_120_style_table_entry.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_123_view_table_entry.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_120_style_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_125_image_def.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_123_view_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_127_raster_variables.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_128_pdf_definition.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_125_image_def.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_129_xrecord.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_130_id_buffer.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_127_raster_variables.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_131_field_list.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_128_pdf_definition.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_132_layer_filter.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_129_xrecord.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_133_sun.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_130_id_buffer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_134_material.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_131_field_list.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_135_geo_data.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_132_layer_filter.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_136_vba_project.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_133_sun.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_137_sortentstable.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_134_material.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_135_geo_data.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_139_user_record.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_136_vba_project.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_140_block_record.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_137_sortentstable.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_142_copy_strategy.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_139_user_record.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_143_spatial_filter.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_140_block_record.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/conftest.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_142_copy_strategy.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_200_line.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_143_spatial_filter.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_201_point.py
+Filename: ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_202_circle.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_203_arc.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_200_line.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_204_shape.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_201_point.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_205_solid.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_202_circle.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_206_text.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_203_arc.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_207_attdef.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_204_shape.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_208_attrib.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_205_solid.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_209_vertex.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_206_text.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_210_polyline_1.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_207_attdef.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_210_polyline_2.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_208_attrib.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_209_vertex.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_1.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_211_viewport.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_2.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_212_insert.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_213_minsert.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_214_block.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_211_viewport.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_215_dimension.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_212_insert.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_213_minsert.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_214_block.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_215_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_221_ellipse.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_222_xline.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_223_ray.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_224_group.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_221_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_225_mtext.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_222_xline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_226_spline.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_223_ray.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_224_group.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_225_mtext.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_228_mesh.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_226_spline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_228_mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_231_underlay.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_231_underlay_2.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_232_acis.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_232_acis_2.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_231_underlay.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_232_surface.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_231_underlay_2.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_233_helix.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232a_add_acis.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_234_light.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232b_acis_export.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_235_leader.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232c_acis_surface.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_236_multileader.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232d_acis_copy.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_237_mline.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232e_acis_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_238_tolerance.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_233_helix.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_234_light.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_235_leader.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_241_hyperlink.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_236_multileader.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_242_random_transform.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_237_mline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_243_replace_entity.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_238_tolerance.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_245_wipeout.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_246_spline_audit.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_241_hyperlink.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_242_random_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_248_mpolygon.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_243_replace_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_245_wipeout.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_246_spline_audit.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_251_upright.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_248_mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_253_ole2frame.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_254_get_font_name.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_300_layout.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_251_upright.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_302_block_references.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_253_ole2frame.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+Filename: ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_254_get_font_name.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_300_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_307_groupby.py
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_302_block_references.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_308_query.py
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_309_query_parser.py
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_313_redraw_order.py
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_307_groupby.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_308_query.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_309_query_parser.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+Filename: ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_313_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_405_classes.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_410_table.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_405_classes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_410_table.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_424_audit.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_429_xclip.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_424_audit.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/conftest.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_500_units.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_501_truecolor.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_502_raw_color.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_503_indexing.py
+Filename: ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_429_xclip.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_504_suppress_zeros.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_506_version.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_500_units.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_508_read_zip.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_501_truecolor.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_509_comments.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_502_raw_color.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_510_byte_stream.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_503_indexing.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_511_bit_stream.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_504_suppress_zeros.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_512_pattern.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_506_version.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_513_reorder_entities.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_508_read_zip.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_514_text.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_509_comments.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_515a_fonts_truetype.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_510_byte_stream.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_515b_fonts_shapefiles.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_511_bit_stream.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_515c_fonts_lff.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_512_pattern.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_516_zoom.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_513_reorder_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_517_text_layout.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_514_text.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_518_header_guid.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_515a_fonts_truetype.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_519_mtext_editor.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_515b_fonts_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_520_mtext_context.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_515c_fonts_lff.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_521_mtext_parser.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_516_zoom.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_522_text_scanner.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_517_text_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_523_text_size.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_518_header_guid.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_524_block_reference_manager.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_519_mtext_editor.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_525_transparency.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_520_mtext_context.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_526_explode.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_521_mtext_parser.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_527_gfxattribs.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_522_text_scanner.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_528_difftags.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_523_text_size.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_529_acis_sat.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_524_block_reference_manager.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_530_acis_sab.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_525_transparency.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_531_acis_entities.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_526_explode.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_532_acis_mesh.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_527_gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_533_shapefiles.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_528_difftags.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_534_dwg_info.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_529_acis_sat.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_535_xref_basic.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_530_acis_sab.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_536_xref_conflict.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_531_acis_entities.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_537_transform.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_532_acis_mesh.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_533_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_539_npshapes.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_534_dwg_info.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_540_lff_parser.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_535_xref_basic.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_541_clipping_portal.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_536_xref_conflict.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_542_itertools.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_537_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_543_select.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_05_tools/test_544_revcloud.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_539_npshapes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/conftest.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_540_lff_parser.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_600_base.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_541_clipping_portal.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_601_bulge.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_542_itertools.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_602_vec3.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_543_select.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_603_vec2.py
+Filename: ezdxf-1.3.0rc0/tests/test_05_tools/test_544_revcloud.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_604_banded_matrix.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/conftest.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_604_linalg.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_600_base.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_605_matrix44.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_601_bulge.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_606_convexhull.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_602_vec3.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_607_perlin_noise.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_603_vec2.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_608_intersection_line_line_2d.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_604_banded_matrix.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_609_point_on_line.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_604_linalg.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_610_ocs.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_605_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_611_ucs.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_606_convexhull.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_612_ucs_pass_trough.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_607_perlin_noise.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_613_is_point_in_polygon_2d.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_608_intersection_line_line_2d.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_614_construct_3d.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_609_point_on_line.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_615_rytz_axis.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_610_ocs.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_616_plane.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_611_ucs.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_617_clockwise_orientation.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_612_ucs_pass_trough.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_618_clipping.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_613_is_point_in_polygon_2d.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_619_greiner_hormann.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_614_construct_3d.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_620_knot.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_615_rytz_axis.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_621_bspline.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_616_plane.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_622_bsplineu.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_617_clockwise_orientation.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_623_rbspline.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_618_clipping.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_624_global_bspline_interpolation.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_619_greiner_hormann.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_626_local_bspline_interpolation.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_620_knot.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_627_bspline_basis.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_621_bspline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_629_bezier.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_622_bsplineu.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_630a_bezier4p_base.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_623_rbspline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_630b_bezier4p_functions.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_624_global_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_631_euler_spiral.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_626_local_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_632_bezier3p.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_627_bspline_basis.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_640_bbox.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_629_bezier.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_641_construction_ray.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_630a_bezier4p_base.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_642_construction_line.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_630b_bezier4p_functions.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_643_construction_box.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_631_euler_spiral.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_644_construction_circle.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_632_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_645_construction_arc.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_640_bbox.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_646_offset_vertices_2d.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_641_construction_ray.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_647_transform_tools.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_642_construction_line.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_648_construction_ellipse.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_643_construction_box.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_650_elliptic_arc_span.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_644_construction_circle.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_651_construction_polyline.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_645_construction_arc.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_652_approx_param_t.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_646_offset_vertices_2d.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_653_polyline_intersection.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_647_transform_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_654_rtree.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_648_construction_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_655_dbscan.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_650_elliptic_arc_span.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_656_k_means.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_651_construction_polyline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_657_mapbox_earcut.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_652_approx_param_t.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_658_bevel_tools.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_653_polyline_intersection.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_654_rtree.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_655_dbscan.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_656_k_means.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_662_is_convex_polygon_2d.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_657_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_663_is_axes_aligned_rectange.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_658_bevel_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_664_concave_clipping_polygon.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_665_inverted_clipping_polygon.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_06_math/test_666_wgs84_transform.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_701_arrows.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_662_is_convex_polygon_2d.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_702_render_forms.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_663_is_axes_aligned_rectange.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_703_mesh_builder.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_664_concave_clipping_polygon.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_704_render_linear_dimension.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_665_inverted_clipping_polygon.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_705_shape.py
+Filename: ezdxf-1.3.0rc0/tests/test_06_math/test_666_wgs84_transform.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_706_random_path.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_701_arrows.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_707_trace.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_702_render_forms.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_708a_path.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_703_mesh_builder.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_708b_path_tools.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_704_render_linear_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_708c_matplotlib_path_tools.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_705_shape.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_708d_qpainter_path_tools.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_706_random_path.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_708e_path_shapes.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_707_trace.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_708f_path_nesting.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_708a_path.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_709_linetype_renderer.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_708b_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_711_points.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_708c_matplotlib_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_712_render_curved_dimension.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_708d_qpainter_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_713_mleader_builder.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_708e_path_shapes.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_714_mleader_render_engine.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_708f_path_nesting.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_715_hatching.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_709_linetype_renderer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_711_points.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_800_mtext_surrogate.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_712_render_curved_dimension.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_801_r12spline.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_713_mleader_builder.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_802_table_painter.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_714_mleader_render_engine.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_803_entities_to_code.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_715_hatching.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_804_importer.py
+Filename: ezdxf-1.3.0rc0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_805_pycsg.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_800_mtext_surrogate.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_806_acadctb.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_801_r12spline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_807_dwg_loader_basics.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_802_table_painter.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_810_drawing_properties.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_803_entities_to_code.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_811a_drawing_frontend.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_804_importer.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_811b_drawing_recorder.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_805_pycsg.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_811c_viewport_processing.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_806_acadctb.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_807_dwg_loader_basics.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_813_geo_interface.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_810_drawing_properties.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_814_text2path.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_811a_drawing_frontend.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_815_dxf_browser.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_811b_drawing_recorder.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_816_bin_packing.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_811c_viewport_processing.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_817_genetic_algorithm.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_818_meshex.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_813_geo_interface.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_819_menger_sponge.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_814_text2path.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_820_openscad.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_815_dxf_browser.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_821_hpgl2.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_816_bin_packing.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_817_genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_823_drawing_layout.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_818_meshex.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_824_svg_drawing_backend.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_819_menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_820_openscad.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_826_custom_json_backend.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_821_hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_08_addons/test_827_geojson_backend.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_823_drawing_layout.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_824_svg_drawing_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_826_custom_json_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Filename: ezdxf-1.3.0rc0/tests/test_08_addons/test_827_geojson_backend.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_10_issues/test_issue_574_flattening_error.py
+Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_10_issues/test_issue_749_text_layout.py
+Filename: ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
 Comment: 
 
-Filename: ezdxf-1.3.0b1/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
+Filename: ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Comment: 
+
+Filename: ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Comment: 
+
+Filename: ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_574_flattening_error.py
+Comment: 
+
+Filename: ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Comment: 
+
+Filename: ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_749_text_layout.py
+Comment: 
+
+Filename: ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ezdxf-1.3.0b1/LICENSE` & `ezdxf-1.3.0rc0/LICENSE`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/PKG-INFO` & `ezdxf-1.3.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.3.0b1
+Version: 1.3.0rc0
 Summary: A Python package to create/manipulate DXF drawings.
 Author-email: Manfred Moitzi <me@mozman.at>
 Project-URL: Repository, https://github.com/mozman/ezdxf
 Project-URL: Documentation, https://ezdxf.readthedocs.io
 Project-URL: Changelog, https://ezdxf.mozman.at/notes/#/page/changelog
 Project-URL: Forum, https://github.com/mozman/ezdxf/discussions
 Project-URL: Issues, https://github.com/mozman/ezdxf/issues
```

## Comparing `ezdxf-1.3.0b1/pyproject.toml` & `ezdxf-1.3.0rc0/pyproject.toml`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/README.md` & `ezdxf-1.3.0rc0/README.md`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/setup.py` & `ezdxf-1.3.0rc0/setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/check_disable_c_ext_by_config_file.py` & `ezdxf-1.3.0rc0/integration_tests/check_disable_c_ext_by_config_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/check_disable_c_ext_by_env_var.py` & `ezdxf-1.3.0rc0/integration_tests/check_disable_c_ext_by_env_var.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_acad_table.py` & `ezdxf-1.3.0rc0/integration_tests/test_acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_all_dimline_styles.py` & `ezdxf-1.3.0rc0/integration_tests/test_all_dimline_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_all_ellipse_transformations.py` & `ezdxf-1.3.0rc0/integration_tests/test_all_ellipse_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_anonymous_blocks.py` & `ezdxf-1.3.0rc0/integration_tests/test_anonymous_blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_appsettings.py` & `ezdxf-1.3.0rc0/integration_tests/test_appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_audit_critical_dxf_files.py` & `ezdxf-1.3.0rc0/integration_tests/test_audit_critical_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_audit_layouts.py` & `ezdxf-1.3.0rc0/integration_tests/test_audit_layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_complex_line_type_2.py` & `ezdxf-1.3.0rc0/integration_tests/test_complex_line_type_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_create_basic_graphics.py` & `ezdxf-1.3.0rc0/integration_tests/test_create_basic_graphics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_document_guid.py` & `ezdxf-1.3.0rc0/integration_tests/test_document_guid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_document_page_setup.py` & `ezdxf-1.3.0rc0/integration_tests/test_document_page_setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_dxf_info_scanning.py` & `ezdxf-1.3.0rc0/integration_tests/test_dxf_info_scanning.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_dynblkhelper.py` & `ezdxf-1.3.0rc0/integration_tests/test_dynblkhelper.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_entities_iterator.py` & `ezdxf-1.3.0rc0/integration_tests/test_entities_iterator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_fix_dulicate_handles.py` & `ezdxf-1.3.0rc0/integration_tests/test_fix_dulicate_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_geo.py` & `ezdxf-1.3.0rc0/integration_tests/test_geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_groups.py` & `ezdxf-1.3.0rc0/integration_tests/test_groups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_hpgl2_addon.py` & `ezdxf-1.3.0rc0/integration_tests/test_hpgl2_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_ignore_junk_beyond_EOF.py` & `ezdxf-1.3.0rc0/integration_tests/test_ignore_junk_beyond_EOF.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_launcher.py` & `ezdxf-1.3.0rc0/integration_tests/test_launcher.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_leica_disto_r12.py` & `ezdxf-1.3.0rc0/integration_tests/test_leica_disto_r12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_load_dxf_unicode_notation.py` & `ezdxf-1.3.0rc0/integration_tests/test_load_dxf_unicode_notation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_mapbox_earcut.py` & `ezdxf-1.3.0rc0/integration_tests/test_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_mtext_columns.py` & `ezdxf-1.3.0rc0/integration_tests/test_mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_mtext_explode_addon.py` & `ezdxf-1.3.0rc0/integration_tests/test_mtext_explode_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_mtext_text_frame.py` & `ezdxf-1.3.0rc0/integration_tests/test_mtext_text_frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_new_table_entries.py` & `ezdxf-1.3.0rc0/integration_tests/test_new_table_entries.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_none_ascii_read_write.py` & `ezdxf-1.3.0rc0/integration_tests/test_none_ascii_read_write.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_odafc.py` & `ezdxf-1.3.0rc0/integration_tests/test_odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_open_binary_DXF_files.py` & `ezdxf-1.3.0rc0/integration_tests/test_open_binary_DXF_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_open_coord_order_issue.py` & `ezdxf-1.3.0rc0/integration_tests/test_open_coord_order_issue.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_open_exotic_dxf_files.py` & `ezdxf-1.3.0rc0/integration_tests/test_open_exotic_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_open_R13_R14.py` & `ezdxf-1.3.0rc0/integration_tests/test_open_R13_R14.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_polyline_entity.py` & `ezdxf-1.3.0rc0/integration_tests/test_polyline_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_preserve_binary_data_in_xrecords.py` & `ezdxf-1.3.0rc0/integration_tests/test_preserve_binary_data_in_xrecords.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_r12export.py` & `ezdxf-1.3.0rc0/integration_tests/test_r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_r12strict.py` & `ezdxf-1.3.0rc0/integration_tests/test_r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_r12writer.py` & `ezdxf-1.3.0rc0/integration_tests/test_r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_read_file_without_handles.py` & `ezdxf-1.3.0rc0/integration_tests/test_read_file_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_read_write_modern_entites.py` & `ezdxf-1.3.0rc0/integration_tests/test_read_write_modern_entites.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_recover.py` & `ezdxf-1.3.0rc0/integration_tests/test_recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_redraw_order.py` & `ezdxf-1.3.0rc0/integration_tests/test_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_rotated_block_attributes.py` & `ezdxf-1.3.0rc0/integration_tests/test_rotated_block_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_surface_entities.py` & `ezdxf-1.3.0rc0/integration_tests/test_surface_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_write_fixed_meta_data.py` & `ezdxf-1.3.0rc0/integration_tests/test_write_fixed_meta_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_write_without_handles.py` & `ezdxf-1.3.0rc0/integration_tests/test_write_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/test_xref_detach.py` & `ezdxf-1.3.0rc0/integration_tests/test_xref_detach.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/AC1003_LINE_Example.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/AC1003_LINE_Example.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/acad_table_with_blk_ref.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/acad_table_with_blk_ref.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/ASCII_R12.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/ASCII_R12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/bin_dxf_r12.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/bin_dxf_r13.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/bin_dxf_r14.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/bin_dxf_r2000.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/bin_dxf_r2000.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/cc_dxflib.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/cc_dxflib.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/custom_blocks.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/custom_blocks.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/duplicate_handles.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/duplicate_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/dxf_unicode.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/dxf_unicode.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/dynblks.zip` & `ezdxf-1.3.0rc0/integration_tests/data/dynblks.zip`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/empty_handles.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/empty_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/groups.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/groups.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/layout_broken_links.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/layout_broken_links.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/layout_broken_links_2.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/layout_broken_links_2.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/layout_missing_block_definition.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/layout_missing_block_definition.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/layout_missing_block_record.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/layout_missing_block_record.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/Leica_Disto_S910.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/Leica_Disto_S910.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/MODEL.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/MODEL.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/mtext_columns_R2007.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/mtext_columns_R2007.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/mtext_columns_R2018.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/mtext_columns_R2018.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/mtext_framed_columns.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/mtext_framed_columns.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/mtext_text_frame.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/mtext_text_frame.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/no_layouts.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/no_layouts.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/PLOTFILE.plt` & `ezdxf-1.3.0rc0/integration_tests/data/PLOTFILE.plt`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/POLI-ALL210_12.DXF` & `ezdxf-1.3.0rc0/integration_tests/data/POLI-ALL210_12.DXF`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/recover01.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/recover01.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/recover02.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/recover02.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/small_r13.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/small_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/small_r14.dxf` & `ezdxf-1.3.0rc0/integration_tests/data/small_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/XRECORD_0.bin` & `ezdxf-1.3.0rc0/integration_tests/data/XRECORD_0.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/XRECORD_1.bin` & `ezdxf-1.3.0rc0/integration_tests/data/XRECORD_1.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/integration_tests/data/XRECORD_2.bin` & `ezdxf-1.3.0rc0/integration_tests/data/XRECORD_2.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/appsettings.py` & `ezdxf-1.3.0rc0/src/ezdxf/appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/audit.py` & `ezdxf-1.3.0rc0/src/ezdxf/audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/bbox.py` & `ezdxf-1.3.0rc0/src/ezdxf/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/blkrefs.py` & `ezdxf-1.3.0rc0/src/ezdxf/blkrefs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/colors.py` & `ezdxf-1.3.0rc0/src/ezdxf/colors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/commands.py` & `ezdxf-1.3.0rc0/src/ezdxf/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/comments.py` & `ezdxf-1.3.0rc0/src/ezdxf/comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/disassemble.py` & `ezdxf-1.3.0rc0/src/ezdxf/disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/document.py` & `ezdxf-1.3.0rc0/src/ezdxf/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Iterable,
     Iterator,
     Union,
     Callable,
     cast,
     Optional,
     Sequence,
-    Any
+    Any,
 )
 import abc
 import base64
 import io
 import logging
 import os
 import pathlib
@@ -48,14 +48,15 @@
 from ezdxf.lldxf.tagwriter import (
     AbstractTagWriter,
     TagWriter,
     BinaryTagWriter,
     JSONTagWriter,
 )
 from ezdxf.query import EntityQuery
+from ezdxf.protocols import SupportsTemporaryTransformation
 from ezdxf.render.dimension import DimensionRenderer
 from ezdxf.sections.acdsdata import AcDsDataSection, new_acds_data_section
 from ezdxf.sections.blocks import BlocksSection
 from ezdxf.sections.classes import ClassesSection
 from ezdxf.sections.entities import EntitySection, StoredSection
 from ezdxf.sections.header import HeaderSection
 from ezdxf.sections.objects import ObjectsSection
@@ -218,15 +219,15 @@
         self._create_required_linetypes()
         self._create_required_layers()
         self._create_required_styles()
         self._create_required_appids()
         self._create_required_dimstyles()
 
     def _set_required_layer_attributes(self):
-        for layer in self.layers:  # type: Layer
+        for layer in self.layers:
             layer.set_required_attributes()
 
     def _create_required_vports(self):
         if "*Active" not in self.viewports:
             self.viewports.new("*Active")
 
     def _create_required_appids(self):
@@ -581,14 +582,19 @@
             binary = doc.encode(stream.get_value())
 
         Args:
             stream: output text stream or binary stream
             fmt: "asc" for ASCII DXF (default) or "bin" for binary DXF
 
         """
+        # These changes may alter the document content (create new entities, blocks ...) 
+        # and have to be done before the export and the update of internal structures 
+        # can be done.
+        self.commit_pending_changes()
+
         dxfversion = self.dxfversion
         if dxfversion == DXF12:
             handles = bool(self.header.get("$HANDLING", 0))
         else:
             handles = True
         if dxfversion > DXF12:
             self.classes.add_required_classes(dxfversion)
@@ -636,14 +642,19 @@
         if self.acdsdata.is_valid:
             self.acdsdata.export_dxf(tagwriter)
         for section in self.stored_sections:
             section.export_dxf(tagwriter)
 
         tagwriter.write_tag2(0, "EOF")
 
+    def commit_pending_changes(self) -> None:
+        entities = list(self.entitydb.values())  # entitydb may change while iterating
+        for entity in entities:
+            entity.commit_pending_changes()
+
     def update_all(self) -> None:
         if self.dxfversion > DXF12:
             self.classes.add_required_classes(self.dxfversion)
         self._create_appids()
         self._update_header_vars()
         self.update_extents()
         self.update_limits()
@@ -1432,35 +1443,35 @@
         tagwriter.write_handles = True
     doc.update_all()
     doc.export_sections(tagwriter)
 
 
 def export_json_tags(doc: Drawing, compact=True) -> str:
     """Export a DXF document as JSON formatted tags.
-    
-    The `compact` format is a list of ``[group-code, value]`` pairs where each pair is 
-    a DXF tag. The group-code has to be an integer and the value has to be a string, 
-    integer, float or list of floats for vertices. 
 
-    The `verbose` format (`compact` is ``False``) is a list of ``[group-code, value]`` 
-    pairs where each pair is a 1:1 representation of a DXF tag. The group-code has to be 
+    The `compact` format is a list of ``[group-code, value]`` pairs where each pair is
+    a DXF tag. The group-code has to be an integer and the value has to be a string,
+    integer, float or list of floats for vertices.
+
+    The `verbose` format (`compact` is ``False``) is a list of ``[group-code, value]``
+    pairs where each pair is a 1:1 representation of a DXF tag. The group-code has to be
     an integer and the value has to be a string.
 
     """
     stream = io.StringIO()
     json_writer = JSONTagWriter(stream, dxfversion=doc.dxfversion, compact=compact)
     custom_export(doc, json_writer)
     return stream.getvalue()
 
 
 def load_json_tags(data: Sequence[Any]) -> Drawing:
     """Load DXF document from JSON formatted tags.
-    
-    The expected JSON format is a list of [group-code, value] pairs where each pair is 
-    a DXF tag. The `compact` and the `verbose` format is supported. 
+
+    The expected JSON format is a list of [group-code, value] pairs where each pair is
+    a DXF tag. The `compact` and the `verbose` format is supported.
 
     Args:
         data: JSON data structure as a sequence of [group-code, value] pairs
 
     """
     from ezdxf.lldxf.tagger import json_tag_loader
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/dwginfo.py` & `ezdxf-1.3.0rc0/src/ezdxf/dwginfo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/dynblkhelper.py` & `ezdxf-1.3.0rc0/src/ezdxf/dynblkhelper.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entitydb.py` & `ezdxf-1.3.0rc0/src/ezdxf/entitydb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/enums.py` & `ezdxf-1.3.0rc0/src/ezdxf/enums.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/explode.py` & `ezdxf-1.3.0rc0/src/ezdxf/explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/eztypes.py` & `ezdxf-1.3.0rc0/src/ezdxf/eztypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/filemanagement.py` & `ezdxf-1.3.0rc0/src/ezdxf/filemanagement.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/gfxattribs.py` & `ezdxf-1.3.0rc0/src/ezdxf/gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/graphicsfactory.py` & `ezdxf-1.3.0rc0/src/ezdxf/graphicsfactory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/groupby.py` & `ezdxf-1.3.0rc0/src/ezdxf/groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/npshapes.py` & `ezdxf-1.3.0rc0/src/ezdxf/npshapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/protocols.py` & `ezdxf-1.3.0rc0/src/ezdxf/protocols.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-#  Copyright (c) 2021-2023, Manfred Moitzi
+#  Copyright (c) 2021-2024, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterator, Iterable
 from typing_extensions import Protocol, runtime_checkable
 from ezdxf.query import EntityQuery
 
 if TYPE_CHECKING:
     from ezdxf.entities import DXFGraphic, DXFEntity
+    from ezdxf.entities.temporary_transform import TemporaryTransformation
     from ezdxf.math import Matrix44, AbstractBoundingBox
 
 
 # Protocol implemented for:
 # - DXFTagStorage
 # - ACAD_PROXY_ENTITY
 # - INSERT
 # - DIMENSION
 # - LEADER
+# - MLEADER
 # - MLINE
 # - ProxyGraphic
 # - DXFGraphicProxy (drawing add-on)
-#
-# TODO: MLEADER, virtual_entities() not implemented yet
+# - DXFTagStorage
+# - ACAD_TABLE (table content loader)
 
 
 @runtime_checkable
 class SupportsVirtualEntities(Protocol):
     """The virtual entities protocol is used to disassemble complex entities
     into DXF primitives like LINE, ARC, ... as REQUIREMENT to render these
     entities. Which means the entity does not have :func:`ezdxf.path.make_path`
@@ -34,16 +36,15 @@
     into LINE and ARC entities is NOT the intended usage of this protocol!
 
     This protocol is for consistent internal usage and does not replace
     the :meth:`virtual_entities` methods!
 
     """
 
-    def __virtual_entities__(self) -> Iterator[DXFGraphic]:
-        ...
+    def __virtual_entities__(self) -> Iterator[DXFGraphic]: ...
 
 
 def virtual_entities(entity: SupportsVirtualEntities) -> Iterator[DXFGraphic]:
     if isinstance(entity, SupportsVirtualEntities):
         return entity.__virtual_entities__()
     else:
         raise TypeError(
@@ -57,21 +58,19 @@
 
 @runtime_checkable
 class ReferencedBlocks(Protocol):
     def __referenced_blocks__(self) -> Iterable[str]:
         """Returns the handles to the BLOCK_RECORD entities for all BLOCK
         definitions used by an entity.
         """
-        ...
 
 
 class SupportsTransform(Protocol):
     def transform(self, m: Matrix44) -> DXFGraphic:
         """Raises NotImplementedError() if transformation is not supported."""
-        ...
 
 
 _EMPTY_TUPLE: tuple = tuple()
 
 
 def referenced_blocks(entity: DXFEntity) -> Iterable[str]:
     """Returns the handles to the BLOCK_RECORD entities for all BLOCK
@@ -80,11 +79,13 @@
     if isinstance(entity, ReferencedBlocks):
         return entity.__referenced_blocks__()
     else:
         return _EMPTY_TUPLE
 
 
 class SupportsBoundingBox(Protocol):
-    def bbox(self) -> AbstractBoundingBox:
-        """Returns the bounding box of an object."""
-        ...
+    def bbox(self) -> AbstractBoundingBox: ...
+
 
+@runtime_checkable
+class SupportsTemporaryTransformation(Protocol):
+    def temporary_transformation(self) -> TemporaryTransformation: ...
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/proxygraphic.py` & `ezdxf-1.3.0rc0/src/ezdxf/proxygraphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/query.py` & `ezdxf-1.3.0rc0/src/ezdxf/query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/queryparser.py` & `ezdxf-1.3.0rc0/src/ezdxf/queryparser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/r12strict.py` & `ezdxf-1.3.0rc0/src/ezdxf/r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/recover.py` & `ezdxf-1.3.0rc0/src/ezdxf/recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/reorder.py` & `ezdxf-1.3.0rc0/src/ezdxf/reorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/revcloud.py` & `ezdxf-1.3.0rc0/src/ezdxf/revcloud.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/select.py` & `ezdxf-1.3.0rc0/src/ezdxf/select.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/transform.py` & `ezdxf-1.3.0rc0/src/ezdxf/transform.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,63 @@
-#  Copyright (c) 2023, Manfred Moitzi
+#  Copyright (c) 2023-2024, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
-from typing import Iterable, Iterator, NamedTuple, Optional, Tuple, List
+from typing import (
+    Iterable,
+    Iterator,
+    NamedTuple,
+    Optional,
+    Tuple,
+    List,
+    TYPE_CHECKING,
+    Sequence,
+)
 import enum
+import logging
 
-
-from ezdxf import const
 from ezdxf.math import (
     Matrix44,
     UVec,
     Vec3,
     NonUniformScalingError,
     InsertTransformationError,
 )
-from ezdxf.entities import DXFEntity, DXFGraphic, Circle, LWPolyline, Polyline, Ellipse
+from ezdxf.entities import (
+    DXFEntity,
+    DXFGraphic,
+    Circle,
+    LWPolyline,
+    Polyline,
+    Ellipse,
+    is_graphic_entity,
+)
 from ezdxf.entities.copy import default_copy, CopyNotSupported
+from ezdxf.protocols import SupportsTemporaryTransformation
+from ezdxf.document import Drawing
+
+if TYPE_CHECKING:
+    from ezdxf.layouts import BlockLayout
+
+__all__ = [
+    "Logger",
+    "Error",
+    "inplace",
+    "copies",
+    "translate",
+    "scale_uniform",
+    "scale",
+    "x_rotate",
+    "y_rotate",
+    "z_rotate",
+    "axis_rotate",
+    "transform_entity_by_blockref",
+    "transform_entities_by_blockref",
+]
 MIN_SCALING_FACTOR = 1e-12
+logger = logging.getLogger("ezdxf")
 
 
 class Error(enum.Enum):
     NONE = 0
     TRANSFORMATION_NOT_SUPPORTED = enum.auto()
     COPY_NOT_SUPPORTED = enum.auto()
     NON_UNIFORM_SCALING_ERROR = enum.auto()
@@ -297,7 +335,64 @@
     if not a:
         return Logger()
 
     v = Vec3(axis)
     if not v.is_null:
         return _inplace(entities, m=Matrix44.axis_rotate(v, a))
     return Logger()
+
+
+def transform_entity_by_blockref(entity: DXFEntity, m: Matrix44) -> bool:
+    """Apply a transformation by moving an entity into a block and replacing the entity
+    by a block reference with the applied transformation.
+    """
+    return _transform_by_blockref([entity], m) is not None
+
+
+def transform_entities_by_blockref(
+    entities: Iterable[DXFEntity], m: Matrix44
+) -> BlockLayout | None:
+    """Apply a transformation by moving entities into a block and replacing the entities
+    by a block reference with the applied transformation.
+    """
+    return _transform_by_blockref(list(entities), m)
+
+
+def _transform_by_blockref(
+    entities: Sequence[DXFEntity], m: Matrix44
+) -> BlockLayout | None:
+    if len(entities) == 0:
+        return None
+
+    first_entity = entities[0]
+    if not is_graphic_entity(first_entity):
+        return None
+
+    doc = first_entity.doc
+    if doc is None:
+        return None
+
+    layout = first_entity.get_layout()
+    if layout is None:
+        return None
+
+    block = doc.blocks.new_anonymous_block()
+    insert = layout.add_blockref(block.name, (0, 0, 0))
+    try:
+        insert.transform(m)
+    except InsertTransformationError:
+        logger.warning(f"cannot apply invalid transformation")
+        layout.delete_entity(insert)
+        doc.blocks.delete_block(block.name, safe=False)
+        return None
+
+    for e in entities:
+        if is_graphic_entity(e):
+            layout.move_to_layout(e, block)
+    return block
+
+
+def apply_temporary_transformations(entities: Iterable[DXFEntity]) -> None:
+    for entity in entities:
+        if isinstance(entity, SupportsTemporaryTransformation):
+            tt = entity.temporary_transformation()
+            tt.apply_transformation(entity)
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/units.py` & `ezdxf-1.3.0rc0/src/ezdxf/units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/upright.py` & `ezdxf-1.3.0rc0/src/ezdxf/upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/urecord.py` & `ezdxf-1.3.0rc0/src/ezdxf/urecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/version.py` & `ezdxf-1.3.0rc0/src/ezdxf/version.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # examples:
 #   major pre-release alpha 2: VERSION = "0.9.0a2"; version = (0, 9, 0, 'a2')
 #   major release candidate 0: VERSION = "0.9.0rc0"; version = (0, 9, 0, 'rc0')
 #   major release: VERSION = "0.9.0"; version = (0, 9, 0, 'release')
 #   1. bug fix release beta0: VERSION = "0.9.1b0"; version = (0, 9, 1, 'b0')
 #   2. bug fix release: VERSION = "0.9.2"; version = (0, 9, 2, 'release')
 
-version = (1, 3, 0, "b1")
-__version__ = "1.3.0b1"
+version = (1, 3, 0, "rc0")
+__version__ = "1.3.0rc0"
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/xclip.py` & `ezdxf-1.3.0rc0/src/ezdxf/xclip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/xref.py` & `ezdxf-1.3.0rc0/src/ezdxf/xref.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2023, Manfred Moitzi
+#  Copyright (c) 2023-2024, Manfred Moitzi
 #  License: MIT License
 """ Resource management module for transferring DXF resources between documents.
 """
 from __future__ import annotations
 from typing import Optional, Sequence, Callable, Iterable
 from typing_extensions import Protocol, TypeAlias
 import enum
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/zoom.py` & `ezdxf-1.3.0rc0/src/ezdxf/zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/_options.py` & `ezdxf-1.3.0rc0/src/ezdxf/_options.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/__init__.py` & `ezdxf-1.3.0rc0/src/ezdxf/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/__main__.py` & `ezdxf-1.3.0rc0/src/ezdxf/__main__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acc/bezier3p.pyx` & `ezdxf-1.3.0rc0/src/ezdxf/acc/bezier3p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acc/bezier4p.pyx` & `ezdxf-1.3.0rc0/src/ezdxf/acc/bezier4p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acc/bspline.pyx` & `ezdxf-1.3.0rc0/src/ezdxf/acc/bspline.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acc/construct.pyx` & `ezdxf-1.3.0rc0/src/ezdxf/acc/construct.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acc/linetypes.pyx` & `ezdxf-1.3.0rc0/src/ezdxf/acc/linetypes.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acc/mapbox_earcut.pyx` & `ezdxf-1.3.0rc0/src/ezdxf/acc/mapbox_earcut.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acc/matrix44.pyx` & `ezdxf-1.3.0rc0/src/ezdxf/acc/matrix44.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acc/np_support.pyx` & `ezdxf-1.3.0rc0/src/ezdxf/acc/np_support.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acc/vector.pxd` & `ezdxf-1.3.0rc0/src/ezdxf/acc/vector.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acc/vector.pyx` & `ezdxf-1.3.0rc0/src/ezdxf/acc/vector.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acc/__init__.py` & `ezdxf-1.3.0rc0/src/ezdxf/acc/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acis/abstract.py` & `ezdxf-1.3.0rc0/src/ezdxf/acis/abstract.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acis/api.py` & `ezdxf-1.3.0rc0/src/ezdxf/acis/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acis/const.py` & `ezdxf-1.3.0rc0/src/ezdxf/acis/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acis/dbg.py` & `ezdxf-1.3.0rc0/src/ezdxf/acis/dbg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acis/dxf.py` & `ezdxf-1.3.0rc0/src/ezdxf/acis/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acis/entities.py` & `ezdxf-1.3.0rc0/src/ezdxf/acis/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,17 +115,15 @@
         return f"{self.type}({self.id})"
 
     def load(self, loader: DataLoader, entity_factory: Factory) -> None:
         """Load the ACIS entity content from `loader`."""
         self.restore_common(loader, entity_factory)
         self.restore_data(loader)
 
-    def restore_common(
-        self, loader: DataLoader, entity_factory: Factory
-    ) -> None:
+    def restore_common(self, loader: DataLoader, entity_factory: Factory) -> None:
         """Load the common part of an ACIS entity."""
         pass
 
     def restore_data(self, loader: DataLoader) -> None:
         """Load the data part of an ACIS entity."""
         pass
 
@@ -145,15 +143,15 @@
         raise const.ExportError(f"unsupported entity type: {self.type}")
 
     def write_data(self, exporter: DataExporter) -> None:
         """Write the data part of the ACIS entity."""
         pass
 
     def entities(self) -> Iterator[AcisEntity]:
-        """Yield all attributes of this entity of type AcisEntity. """
+        """Yield all attributes of this entity of type AcisEntity."""
         for e in vars(self).values():
             if isinstance(e, AcisEntity):
                 yield e
 
 
 def restore_entity(
     expected_type: str, loader: DataLoader, entity_factory: Factory
@@ -206,47 +204,41 @@
 @register
 class AsmHeader(AcisEntity):
     type: str = "asmheader"
 
     def __init__(self, version: str = ""):
         self.version = version
 
-    def restore_common(
-        self, loader: DataLoader, entity_factory: Factory
-    ) -> None:
+    def restore_common(self, loader: DataLoader, entity_factory: Factory) -> None:
         self.version = loader.read_str()
 
     def write_common(self, exporter: DataExporter) -> None:
         exporter.write_str(self.version)
 
 
 class SupportsPattern(AcisEntity):
     pattern: Pattern = NONE_REF
 
-    def restore_common(
-        self, loader: DataLoader, entity_factory: Factory
-    ) -> None:
+    def restore_common(self, loader: DataLoader, entity_factory: Factory) -> None:
         if loader.version >= Features.PATTERN:
             self.pattern = restore_entity("pattern", loader, entity_factory)
 
     def write_common(self, exporter: DataExporter) -> None:
         exporter.write_ptr(self.pattern)
 
 
 @register
 class Body(SupportsPattern):
     type: str = "body"
     pattern: Pattern = NONE_REF
     lump: Lump = NONE_REF
     wire: Wire = NONE_REF
-    transform: "Transform" = NONE_REF
+    transform: Transform = NONE_REF
 
-    def restore_common(
-        self, loader: DataLoader, entity_factory: Factory
-    ) -> None:
+    def restore_common(self, loader: DataLoader, entity_factory: Factory) -> None:
         super().restore_common(loader, entity_factory)
         self.lump = restore_entity("lump", loader, entity_factory)
         self.wire = restore_entity("wire", loader, entity_factory)
         self.transform = restore_entity("transform", loader, entity_factory)
 
     def write_common(self, exporter: DataExporter) -> None:
         super().write_common(exporter)
@@ -288,17 +280,15 @@
 @register
 class Lump(SupportsPattern):
     type: str = "lump"
     next_lump: Lump = NONE_REF
     shell: Shell = NONE_REF
     body: Body = NONE_REF
 
-    def restore_common(
-        self, loader: DataLoader, entity_factory: Factory
-    ) -> None:
+    def restore_common(self, loader: DataLoader, entity_factory: Factory) -> None:
         super().restore_common(loader, entity_factory)
         self.next_lump = restore_entity("lump", loader, entity_factory)
         self.shell = restore_entity("shell", loader, entity_factory)
         self.body = restore_entity("body", loader, entity_factory)
 
     def write_common(self, exporter: DataExporter) -> None:
         super().write_common(exporter)
@@ -332,17 +322,15 @@
     type: str = "shell"
     next_shell: Shell = NONE_REF
     subshell: Subshell = NONE_REF
     face: Face = NONE_REF
     wire: Wire = NONE_REF
     lump: Lump = NONE_REF
 
-    def restore_common(
-        self, loader: DataLoader, entity_factory: Factory
-    ) -> None:
+    def restore_common(self, loader: DataLoader, entity_factory: Factory) -> None:
         super().restore_common(loader, entity_factory)
         self.next_shell = restore_entity("next_shell", loader, entity_factory)
         self.subshell = restore_entity("subshell", loader, entity_factory)
         self.face = restore_entity("face", loader, entity_factory)
         self.wire = restore_entity("wire", loader, entity_factory)
         self.lump = restore_entity("lump", loader, entity_factory)
 
@@ -386,22 +374,18 @@
     next_face: "Face" = NONE_REF
     loop: Loop = NONE_REF
     shell: Shell = NONE_REF
     subshell: Subshell = NONE_REF
     surface: Surface = NONE_REF
     # sense: face normal with respect to the surface
     sense = False  # True = reversed; False = forward
-    double_sided = (
-        False  # True = double (hollow body); False = single (solid body)
-    )
+    double_sided = False  # True = double (hollow body); False = single (solid body)
     containment = False  # if double_sided: True = in, False = out
 
-    def restore_common(
-        self, loader: DataLoader, entity_factory: Factory
-    ) -> None:
+    def restore_common(self, loader: DataLoader, entity_factory: Factory) -> None:
         super().restore_common(loader, entity_factory)
         self.next_face = restore_entity("face", loader, entity_factory)
         self.loop = restore_entity("loop", loader, entity_factory)
         self.shell = restore_entity("shell", loader, entity_factory)
         self.subshell = restore_entity("subshell", loader, entity_factory)
         self.surface = restore_entity("surface", loader, entity_factory)
         self.sense = loader.read_bool("reversed", "forward")
@@ -475,17 +459,15 @@
     u_dir = Vec3(1, 0, 0)  # unit vector!
     v_dir = Vec3(0, 1, 0)  # unit vector!
     # reverse_v:
     # True: "reverse_v" - the normal vector does not follow the right-hand rule
     # False: "forward_v" - the normal vector follows right-hand rule
     reverse_v = False
 
-    def restore_common(
-        self, loader: DataLoader, entity_factory: Factory
-    ) -> None:
+    def restore_common(self, loader: DataLoader, entity_factory: Factory) -> None:
         super().restore_common(loader, entity_factory)
         self.origin = Vec3(loader.read_vec3())
         self.normal = Vec3(loader.read_vec3())
         self.u_dir = Vec3(loader.read_vec3())
         self.reverse_v = loader.read_bool("reverse_v", "forward_v")
         self.update_v_dir()
 
@@ -510,17 +492,15 @@
 @register
 class Loop(SupportsPattern):
     type: str = "loop"
     next_loop: Loop = NONE_REF
     coedge: Coedge = NONE_REF
     face: Face = NONE_REF  # parent/owner
 
-    def restore_common(
-        self, loader: DataLoader, entity_factory: Factory
-    ) -> None:
+    def restore_common(self, loader: DataLoader, entity_factory: Factory) -> None:
         super().restore_common(loader, entity_factory)
         self.next_loop = restore_entity("loop", loader, entity_factory)
         self.coedge = restore_entity("coedge", loader, entity_factory)
         self.face = restore_entity("face", loader, entity_factory)
 
     def write_common(self, exporter: DataExporter) -> None:
         super().write_common(exporter)
@@ -573,17 +553,15 @@
     # sense: True = reversed; False = forward;
     # coedge has the same direction as the underlying edge
     sense: bool = True
     loop: Loop = NONE_REF  # parent/owner
     unknown: int = 0  # only in SAB file!?
     pcurve: PCurve = NONE_REF
 
-    def restore_common(
-        self, loader: DataLoader, entity_factory: Factory
-    ) -> None:
+    def restore_common(self, loader: DataLoader, entity_factory: Factory) -> None:
         super().restore_common(loader, entity_factory)
         self.next_coedge = restore_entity("coedge", loader, entity_factory)
         self.prev_coedge = restore_entity("coedge", loader, entity_factory)
         self.partner_coedge = restore_entity("coedge", loader, entity_factory)
         self.edge = restore_entity("edge", loader, entity_factory)
         self.sense = loader.read_bool("reversed", "forward")
         self.loop = restore_entity("loop", loader, entity_factory)
@@ -614,15 +592,15 @@
 
     def order_partner_coedges(self) -> None:
         # todo: the referenced faces of non-manifold coedges have to be ordered
         #  by the right-hand rule around this edge.
         pass
 
     def partner_coedges(self) -> list[Coedge]:
-        """Returns all partner coedges of this coedge without `self`. """
+        """Returns all partner coedges of this coedge without `self`."""
         coedges: list[Coedge] = []
         partner_coedge = self.partner_coedge
         if partner_coedge.is_none:
             return coedges
         while True:
             coedges.append(partner_coedge)
             partner_coedge = partner_coedge.partner_coedge
@@ -645,17 +623,15 @@
     coedge: Coedge = NONE_REF
     curve: Curve = NONE_REF
     # sense: True = reversed; False = forward;
     # forward: edge has the same direction as the underlying curve
     sense: bool = False
     convexity: str = "unknown"
 
-    def restore_common(
-        self, loader: DataLoader, entity_factory: Factory
-    ) -> None:
+    def restore_common(self, loader: DataLoader, entity_factory: Factory) -> None:
         super().restore_common(loader, entity_factory)
         self.start_vertex = restore_entity("vertex", loader, entity_factory)
         if loader.version >= Features.TOL_MODELING:
             self.start_param = loader.read_double()
         self.end_vertex = restore_entity("vertex", loader, entity_factory)
         if loader.version >= Features.TOL_MODELING:
             self.end_param = loader.read_double()
@@ -686,17 +662,15 @@
 @register
 class Vertex(SupportsPattern):
     type: str = "vertex"
     edge: Edge = NONE_REF
     ref_count: int = 0  # only in SAB files
     point: Point = NONE_REF
 
-    def restore_common(
-        self, loader: DataLoader, entity_factory: Factory
-    ) -> None:
+    def restore_common(self, loader: DataLoader, entity_factory: Factory) -> None:
         super().restore_common(loader, entity_factory)
         self.edge = restore_entity("edge", loader, entity_factory)
         self.ref_count = loader.read_int(skip_sat=0)
         self.point = restore_entity("point", loader, entity_factory)
 
     def write_common(self, exporter: DataExporter) -> None:
         super().write_common(exporter)
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acis/hdr.py` & `ezdxf-1.3.0rc0/src/ezdxf/acis/hdr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acis/mesh.py` & `ezdxf-1.3.0rc0/src/ezdxf/acis/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acis/sab.py` & `ezdxf-1.3.0rc0/src/ezdxf/acis/sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/acis/sat.py` & `ezdxf-1.3.0rc0/src/ezdxf/acis/sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/acadctb.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/binpacking.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/binpacking.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/dimlines.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/dimlines.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/dxf2code.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/dxf2code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/genetic_algorithm.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/geo.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/gerber_D6673.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/gerber_D6673.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/importer.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/iterdxf.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/iterdxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/menger_sponge.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/meshex.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/mtextsurrogate.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/mtextsurrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/mtxpl.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/mtxpl.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/odafc.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/openscad.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/pycsg.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/r12export.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/r12writer.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/sierpinski_pyramid.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/sierpinski_pyramid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/tablepainter.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/tablepainter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/text2path.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/xplayer.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/xplayer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/xqt.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/xqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/acisbrowser/browser.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/acisbrowser/data.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/acisbrowser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/browser/bookmarks.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/bookmarks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/browser/browser.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/browser/data.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/browser/find_dialog.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/find_dialog.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/browser/loader.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/browser/model.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/model.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/browser/reflinks.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/reflinks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/browser/tags.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/browser/views.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/browser/views.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/backend.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/config.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/config.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/debug_backend.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/debug_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/debug_utils.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/debug_utils.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/dxf.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/file_output.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/file_output.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/frontend.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/frontend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/gfxproxy.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/gfxproxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/hpgl2.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/hpgl2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/json.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/json.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/layout.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/matplotlib.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/matplotlib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/mtext_complex.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/mtext_complex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/pipeline.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 #  License: MIT License
 from __future__ import annotations
 from typing import (
     Sequence,
     Optional,
     Iterable,
     Tuple,
-    TYPE_CHECKING,
     Iterator,
     Callable,
 )
 from typing_extensions import TypeAlias
 import abc
 
 import numpy as np
@@ -29,25 +28,22 @@
 from ezdxf.entities import DXFGraphic, Viewport
 from ezdxf.tools.text import replace_non_printable_characters
 from ezdxf.tools.clipping_portal import (
     ClippingPortal,
     ClippingShape,
     find_best_clipping_shape,
 )
-
+from ezdxf.layouts import Layout
 from .backend import BackendInterface, BkPath2d, BkPoints2d, ImageData
 from .config import LinePolicy, TextPolicy, ColorPolicy, Configuration
 from .properties import BackendProperties, Filling
 from .properties import Properties, RenderContext
 from .type_hints import Color
 from .unified_text_renderer import UnifiedTextRenderer
 
-if TYPE_CHECKING:
-    from ezdxf.layouts import Layout
-
 PatternKey: TypeAlias = Tuple[str, float]
 DrawEntitiesCallback: TypeAlias = Callable[[RenderContext, Iterable[DXFGraphic]], None]
 
 __all__ = ["AbstractPipeline", "RenderPipeline2d"]
 
 
 class AbstractPipeline(abc.ABC):
@@ -238,15 +234,15 @@
         )
 
     def set_draw_entities_callback(self, callback: DrawEntitiesCallback) -> None:
         self.draw_entities = callback
 
     def set_config(self, config: Configuration) -> None:
         self.backend.configure(config)
-        self.config = config      
+        self.config = config
         stage = self._pipeline
         while True:
             stage.set_config(config)
             if not hasattr(stage, "next_stage"):  # BackendStage2d
                 return
             stage = stage.next_stage
 
@@ -284,16 +280,26 @@
 
     def enter_viewport(self, vp: Viewport) -> bool:
         """Set current viewport, returns ``True`` for valid viewports."""
         self.current_vp_scale = vp.get_scale()
         m = vp.get_transformation_matrix()
         clipping_path = make_path(vp)
         if len(clipping_path):
-            # TODO: flatten clipping path! max_sagitta = ?
-            clipping_shape = find_best_clipping_shape(clipping_path.control_vertices())
+            vertices = clipping_path.control_vertices()
+            if clipping_path.has_curves:
+                layout = vp.get_layout()
+                if isinstance(layout, Layout):
+                    # plot paper units:
+                    #   0: inches, max sagitta = 1/254 = 0.1 mm
+                    #   1: millimeters, max sagitta = 0.1 mm
+                    #   2: pixels, max sagitta = 0.1 pixel
+                    units = layout.dxf.get("plot_paper_units", 1)
+                    max_sagitta = 1.0 / 254.0 if units == 0 else 0.1
+                    vertices = list(clipping_path.flattening(max_sagitta))
+            clipping_shape = find_best_clipping_shape(vertices)
             self.clipping_portal.push(clipping_shape, m)
             return True
         return False
 
     def exit_viewport(self):
         self.clipping_portal.pop()
         # Reset viewport scaling: viewports cannot be nested!
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/properties.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/pymupdf.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pymupdf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/pyqt.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/pyqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/qtviewer.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/qtviewer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/recorder.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/recorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/svg.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/svg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/text.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/text_renderer.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/drawing/unified_text_renderer.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/drawing/unified_text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/dwg/classes_section.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/classes_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/dwg/const.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/dwg/crc.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/crc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/dwg/fileheader.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/fileheader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/dwg/header_section.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/header_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/dwg/loader.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/dwg/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/api.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/backend.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/deps.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/deps.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/interpreter.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/interpreter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/page.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/page.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/plotter.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/plotter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/polygon_buffer.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/polygon_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/properties.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/tokenizer.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/tokenizer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/addons/hpgl2/viewer.py` & `ezdxf-1.3.0rc0/src/ezdxf/addons/hpgl2/viewer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/acad_proxy_entity.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/acad_table.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/acad_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Optional, Iterator
+from typing_extensions import Self
 import copy
 from ezdxf.math import Vec3, Matrix44
 from ezdxf.lldxf.tags import Tags, group_tags
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
@@ -245,15 +246,15 @@
     )
     MIN_DXF_VERSION_FOR_EXPORT = const.DXF2007
 
     def __init__(self):
         super().__init__()
         self.data = None
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy data."""
         assert isinstance(entity, AcadTable)
         entity.data = copy.deepcopy(self.data)
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/acad_xrec_roundtrip.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/acad_xrec_roundtrip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/acis.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/acis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,56 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Union, Optional, Sequence
 from typing_extensions import Self
+import logging
+
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     XType,
     group_code_mapping,
 )
-from ezdxf.lldxf.const import (
-    SUBCLASS_MARKER,
-    DXF2000,
-    DXF2004,
-    DXFTypeError,
-    DXF2013,
-    DXFStructureError,
-)
+from ezdxf.lldxf import const
 from ezdxf.lldxf.tags import Tags, DXFTag
 from ezdxf.math import Matrix44
-from ezdxf.tools import crypt
+from ezdxf.tools import crypt, guid
+
 from .dxfentity import base_class, SubclassProcessor
 from .dxfgfx import DXFGraphic, acdb_entity
 from .factory import register_entity
-from .copy import default_copy, CopyNotSupported
+from .copy import default_copy
+from .temporary_transform import TransformByBlockReference
 
 if TYPE_CHECKING:
     from ezdxf.entities import DXFNamespace
     from ezdxf.lldxf.tagwriter import AbstractTagWriter
+    from ezdxf import xref
 
 
 __all__ = [
     "Body",
     "Solid3d",
     "Region",
     "Surface",
     "ExtrudedSurface",
     "LoftedSurface",
     "RevolvedSurface",
     "SweptSurface",
 ]
 
+logger = logging.getLogger("ezdxf")
 acdb_modeler_geometry = DefSubclass(
     "AcDbModelerGeometry",
     {
         "version": DXFAttr(70, default=1),
-        "flags": DXFAttr(290, dxfversion=DXF2013),
-        "uid": DXFAttr(2, dxfversion=DXF2013),
+        "flags": DXFAttr(290, dxfversion=const.DXF2013),
+        "uid": DXFAttr(2, dxfversion=const.DXF2013),
     },
 )
 acdb_modeler_geometry_group_codes = group_code_mapping(acdb_modeler_geometry)
 
 # with R2013/AC1027 Modeler Geometry of ACIS data is stored in the ACDSDATA
 # section as binary encoded information detection:
 # group code 70, 1, 3 is missing
@@ -79,23 +78,24 @@
 
 @register_entity
 class Body(DXFGraphic):
     """DXF BODY entity - container entity for embedded ACIS data."""
 
     DXFTYPE = "BODY"
     DXFATTRIBS = DXFAttributes(base_class, acdb_entity, acdb_modeler_geometry)
-    MIN_DXF_VERSION_FOR_EXPORT = DXF2000
+    MIN_DXF_VERSION_FOR_EXPORT = const.DXF2000
 
     def __init__(self) -> None:
         super().__init__()
         # Store SAT data as immutable sequence of strings, so the data can be shared
         # across multiple copies of an ACIS entity.
         self._sat: Sequence[str] = tuple()
         self._sab: bytes = b""
         self._update = False
+        self._temporary_transformation = TransformByBlockReference()
 
     @property
     def acis_data(self) -> Union[bytes, Sequence[str]]:
         """Returns :term:`SAT` data  for DXF R2000 up to R2010 and :term:`SAB`
         data for DXF R2013 and later
         """
         if self.has_binary_data:
@@ -129,22 +129,64 @@
 
     @property
     def has_binary_data(self):
         """Returns ``True`` if the entity contains :term:`SAB` data and
         ``False`` if the entity contains :term:`SAT` data.
         """
         if self.doc:
-            return self.doc.dxfversion >= DXF2013
+            return self.doc.dxfversion >= const.DXF2013
         else:
             return False
 
-    def copy(self, copy_strategy=default_copy):
-        """Prevent copying. (internal interface)"""
-        # TODO: copying of ACIS data is possible
-        raise CopyNotSupported("Copying of ACIS data not supported.")
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
+        assert isinstance(entity, Body)
+        entity.sat = self.sat
+        entity.sab = self.sab  # load SAB on demand
+        entity.dxf.uid = guid()
+        entity._temporary_transformation = self._temporary_transformation
+
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
+        """Translate resources from self to the copied entity."""
+        super().map_resources(clone, mapping)
+        clone.convert_acis_data()
+
+    def convert_acis_data(self) -> None:
+        if self.doc is None:
+            return
+        msg = ""
+        dxfversion = self.doc.dxfversion
+        if dxfversion < const.DXF2013:
+            if self._sab:
+                self._sab = b""
+                msg = "DXF version mismatch, can't convert ACIS data from SAB to SAT, SAB data removed."
+        else:
+            if self._sat:
+                self._sat = tuple()
+                msg = "DXF version mismatch, can't convert ACIS data from SAT to SAB, SAT data removed."
+        if msg:
+            logger.info(msg)
+
+    def commit_pending_changes(self) -> None:
+        self._temporary_transformation.apply_transformation(self)
+
+    def preprocess_export(self, tagwriter: AbstractTagWriter) -> bool:
+        msg = ""
+        if tagwriter.dxfversion < const.DXF2013:
+            valid = len(self.sat) > 0
+            if not valid:
+                msg = f"{str(self)} doesn't have SAT data, skipping DXF export"
+        else:
+            valid = len(self.sab) > 0
+            if not valid:
+                msg = f"{str(self)} doesn't have SAB data, skipping DXF export"
+        if not valid:
+            logger.info(msg)
+        if valid and self._temporary_transformation.get_matrix() is not None:
+            logger.warning(f"{str(self)} has unapplied temporary transformations.")
+        return valid
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         """Loading interface. (internal API)"""
         dxf = super().load_dxf_attribs(processor)
         if processor:
@@ -159,16 +201,16 @@
         """Loading interface. (internal API)"""
         text_lines = tags2textlines(tag for tag in tags if tag.code in (1, 3))
         self._sat = tuple(crypt.decode(text_lines))
 
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags. (internal API)"""
         super().export_entity(tagwriter)
-        tagwriter.write_tag2(SUBCLASS_MARKER, acdb_modeler_geometry.name)
-        if tagwriter.dxfversion >= DXF2013:
+        tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_modeler_geometry.name)
+        if tagwriter.dxfversion >= const.DXF2013:
             # ACIS data is stored in the ACDSDATA section as SAB
             if self.doc and self._update:
                 # write back changed SAB data into AcDsDataSection or create
                 # a new ACIS record:
                 self.doc.acdsdata.set_acis_data(self.dxf.handle, self.sab)
             if self.dxf.hasattr("version"):
                 tagwriter.write_tag2(70, self.dxf.version)
@@ -199,15 +241,19 @@
 
     def destroy(self) -> None:
         if self.has_binary_data:
             self.doc.acdsdata.del_acis_data(self.dxf.handle)  # type: ignore
         super().destroy()
 
     def transform(self, m: Matrix44) -> Self:
-        raise NotImplementedError("cannot transform ACIS entities")
+        self._temporary_transformation.add_matrix(m)
+        return self
+
+    def temporary_transformation(self) -> TransformByBlockReference:
+        return self._temporary_transformation
 
 
 def tags2textlines(tags: Iterable) -> Iterable[str]:
     """Yields text lines from code 1 and 3 tags, code 1 starts a line following
     code 3 tags are appended to the line.
     """
     line = None
@@ -271,23 +317,23 @@
 
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         # base class export is done by parent class
         super().export_entity(tagwriter)
         # AcDbEntity export is done by parent class
         # AcDbModelerGeometry export is done by parent class
-        if tagwriter.dxfversion > DXF2004:
-            tagwriter.write_tag2(SUBCLASS_MARKER, acdb_3dsolid.name)
+        if tagwriter.dxfversion > const.DXF2004:
+            tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_3dsolid.name)
             self.dxf.export_dxf_attribs(tagwriter, "history_handle")
 
 
 def load_matrix(subclass: Tags, code: int) -> Matrix44:
     values = [tag.value for tag in subclass.find_all(code)]
     if len(values) != 16:
-        raise DXFStructureError("Invalid transformation matrix.")
+        raise const.DXFStructureError("Invalid transformation matrix.")
     return Matrix44(values)
 
 
 def export_matrix(tagwriter: AbstractTagWriter, code: int, matrix: Matrix44) -> None:
     for value in list(matrix):
         tagwriter.write_tag2(code, value)
 
@@ -321,15 +367,15 @@
 
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         # base class export is done by parent class
         super().export_entity(tagwriter)
         # AcDbEntity export is done by parent class
         # AcDbModelerGeometry export is done by parent class
-        tagwriter.write_tag2(SUBCLASS_MARKER, acdb_surface.name)
+        tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_surface.name)
         self.dxf.export_dxf_attribs(tagwriter, ["u_count", "v_count"])
 
 
 acdb_extruded_surface = DefSubclass(
     "AcDbExtrudedSurface",
     {
         "class_id": DXFAttr(90),
@@ -377,14 +423,27 @@
 
     def __init__(self):
         super().__init__()
         self.transformation_matrix_extruded_entity = Matrix44()
         self.sweep_entity_transformation_matrix = Matrix44()
         self.path_entity_transformation_matrix = Matrix44()
 
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
+        assert isinstance(entity, ExtrudedSurface)
+        super().copy_data(entity, copy_strategy)
+        entity.transformation_matrix_extruded_entity = (
+            self.transformation_matrix_extruded_entity.copy()
+        )
+        entity.sweep_entity_transformation_matrix = (
+            self.sweep_entity_transformation_matrix.copy()
+        )
+        entity.path_entity_transformation_matrix = (
+            self.path_entity_transformation_matrix.copy()
+        )
+
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
         if processor:
             processor.fast_load_dxfattribs(
                 dxf, acdb_extruded_surface_group_codes, 4, log=False
@@ -399,15 +458,15 @@
 
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         # base class export is done by parent class
         super().export_entity(tagwriter)
         # AcDbEntity export is done by parent class
         # AcDbModelerGeometry export is done by parent class
-        tagwriter.write_tag2(SUBCLASS_MARKER, acdb_extruded_surface.name)
+        tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_extruded_surface.name)
         self.dxf.export_dxf_attribs(tagwriter, ["class_id", "sweep_vector"])
         export_matrix(
             tagwriter,
             code=40,
             matrix=self.transformation_matrix_extruded_entity,
         )
         self.dxf.export_dxf_attribs(
@@ -477,14 +536,21 @@
         acdb_lofted_surface,
     )
 
     def __init__(self):
         super().__init__()
         self.transformation_matrix_lofted_entity = Matrix44()
 
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
+        assert isinstance(entity, LoftedSurface)
+        super().copy_data(entity, copy_strategy)
+        entity.transformation_matrix_lofted_entity = (
+            self.transformation_matrix_lofted_entity.copy()
+        )
+
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
         if processor:
             processor.fast_load_dxfattribs(
                 dxf, acdb_lofted_surface_group_codes, 4, log=False
@@ -497,15 +563,15 @@
 
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         # base class export is done by parent class
         super().export_entity(tagwriter)
         # AcDbEntity export is done by parent class
         # AcDbModelerGeometry export is done by parent class
-        tagwriter.write_tag2(SUBCLASS_MARKER, acdb_lofted_surface.name)
+        tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_lofted_surface.name)
         export_matrix(
             tagwriter, code=40, matrix=self.transformation_matrix_lofted_entity
         )
         self.dxf.export_dxf_attribs(tagwriter, acdb_lofted_surface.attribs.keys())
 
 
 acdb_revolved_surface = DefSubclass(
@@ -542,14 +608,21 @@
         acdb_revolved_surface,
     )
 
     def __init__(self):
         super().__init__()
         self.transformation_matrix_revolved_entity = Matrix44()
 
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
+        assert isinstance(entity, RevolvedSurface)
+        super().copy_data(entity, copy_strategy)
+        entity.transformation_matrix_revolved_entity = (
+            self.transformation_matrix_revolved_entity.copy()
+        )
+
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
         if processor:
             processor.fast_load_dxfattribs(
                 dxf, acdb_revolved_surface_group_codes, 4, log=False
@@ -562,15 +635,15 @@
 
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         # base class export is done by parent class
         super().export_entity(tagwriter)
         # AcDbEntity export is done by parent class
         # AcDbModelerGeometry export is done by parent class
-        tagwriter.write_tag2(SUBCLASS_MARKER, acdb_revolved_surface.name)
+        tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_revolved_surface.name)
         self.dxf.export_dxf_attribs(
             tagwriter,
             [
                 "class_id",
                 "axis_point",
                 "axis_vector",
                 "revolve_angle",
@@ -651,14 +724,30 @@
     def __init__(self):
         super().__init__()
         self.transformation_matrix_sweep_entity = Matrix44()
         self.transformation_matrix_path_entity = Matrix44()
         self.sweep_entity_transformation_matrix = Matrix44()
         self.path_entity_transformation_matrix = Matrix44()
 
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
+        assert isinstance(entity, SweptSurface)
+        super().copy_data(entity, copy_strategy)
+        entity.transformation_matrix_sweep_entity = (
+            self.transformation_matrix_sweep_entity.copy()
+        )
+        entity.transformation_matrix_path_entity = (
+            self.transformation_matrix_path_entity.copy()
+        )
+        entity.sweep_entity_transformation_matrix = (
+            self.sweep_entity_transformation_matrix.copy()
+        )
+        entity.path_entity_transformation_matrix = (
+            self.path_entity_transformation_matrix.copy()
+        )
+
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
         if processor:
             processor.fast_load_dxfattribs(
                 dxf, acdb_swept_surface_group_codes, 4, log=False
@@ -674,15 +763,15 @@
 
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         # base class export is done by parent class
         super().export_entity(tagwriter)
         # AcDbEntity export is done by parent class
         # AcDbModelerGeometry export is done by parent class
-        tagwriter.write_tag2(SUBCLASS_MARKER, acdb_swept_surface.name)
+        tagwriter.write_tag2(const.SUBCLASS_MARKER, acdb_swept_surface.name)
         self.dxf.export_dxf_attribs(
             tagwriter,
             [
                 "swept_entity_id",
                 "path_entity_id",
             ],
         )
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/appdata.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/appid.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/appid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/arc.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/attrib.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/attrib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
 from typing_extensions import Self
 import copy
 from ezdxf.lldxf import validator
 from ezdxf.math import NULLVEC, Vec3, Z_AXIS, OCS, Matrix44
@@ -214,15 +214,15 @@
 
     def __init__(self) -> None:
         super().__init__()
         # Does subclass AcDbXrecord really exist?
         self._xrecord: Optional[Tags] = None
         self._embedded_mtext: Optional[EmbeddedMText] = None
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy entity data, xrecord data and embedded MTEXT are not stored
         in the entity database.
         """
         assert isinstance(entity, BaseAttrib)
         entity._xrecord = copy.deepcopy(self._xrecord)
         entity._embedded_mtext = copy.deepcopy(self._embedded_mtext)
 
@@ -372,15 +372,15 @@
 
     def register_resources(self, registry: xref.Registry) -> None:
         """Register required resources to the resource registry."""
         super().register_resources(registry)
         if self._embedded_mtext:
             self._embedded_mtext.register_resources(registry)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, BaseAttrib)
         super().map_resources(clone, mapping)
         if self._embedded_mtext and clone._embedded_mtext:
             self._embedded_mtext.map_resources(clone._embedded_mtext, mapping)
         # todo: map handles in embedded XRECORD if a real world example shows up
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/block.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) 2019-2022 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
+from typing_extensions import Self
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     XType,
     RETURN_DEFAULT,
@@ -196,15 +197,15 @@
         block_name = self.dxf.get("name", "").upper()
         if owner_name != block_name:
             auditor.add_error(
                 AuditError.BLOCK_NAME_MISMATCH,
                 f"{str(self)} name '{block_name}' and {str(owner)} name '{owner_name}' mismatch",
             )
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, Block)
         super().map_resources(clone, mapping)
         clone.dxf.name = mapping.get_block_name(self.dxf.name)
 
 
 acdb_block_end = DefSubclass("AcDbBlockEnd", {})
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/blockrecord.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/blockrecord.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) 2019-2023, Manfred Moitzi
+# Copyright (c) 2019-2024, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
+from typing_extensions import Self
 import logging
 
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
@@ -185,15 +186,15 @@
         else:
             raise DXFInternalEzdxfError(
                 f"ENDBLK entity in BLOCK_RECORD #{key} is invalid"
             )
         for e in self.entity_space:
             registry.add_entity(e, block_key=key)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, BlockRecord)
         super().map_resources(clone, mapping)
 
         assert self.block is not None
         mapping.map_resources_of_copy(self.block)
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/boundary_paths.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/circle.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/copy.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/copy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/dictionary.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/dictionary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) 2019-2023, Manfred Moitzi
+# Copyright (c) 2019-2024, Manfred Moitzi
 # License: MIT-License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union, Optional
+from typing_extensions import Self
 import logging
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.const import (
     SUBCLASS_MARKER,
     DXFKeyError,
     DXFValueError,
     DXFTypeError,
@@ -96,15 +97,15 @@
     DXFATTRIBS = DXFAttributes(base_class, acdb_dictionary)
 
     def __init__(self) -> None:
         super().__init__()
         self._data: dict[str, Union[str, DXFObject]] = dict()
         self._value_code = VALUE_CODE
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy hard owned entities but do not store the copies in the entity
         database, this is a second step (factory.bind), this is just real copying.
         """
         assert isinstance(entity, Dictionary)
         entity._value_code = self._value_code
         if self.dxf.hard_owned:
             # Reactors are removed from the cloned DXF objects.
@@ -136,15 +137,15 @@
             if not isinstance(entity, DXFEntity):
                 continue
             copied_entry = clone.get(key)
             if copied_entry:
                 handle_mapping[entity.dxf.handle] = copied_entry.dxf.handle
         return handle_mapping
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, Dictionary)
         super().map_resources(clone, mapping)
         if self.is_hard_owner:
             return
         data = dict()
         for key, entity in self.items():
@@ -549,15 +550,15 @@
     DXFTYPE = "ACDBDICTIONARYWDFLT"
     DXFATTRIBS = DXFAttributes(base_class, acdb_dictionary, acdb_dict_with_default)
 
     def __init__(self) -> None:
         super().__init__()
         self._default: Optional[DXFObject] = None
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         super().copy_data(entity, copy_strategy=copy_strategy)
         assert isinstance(entity, DictionaryWithDefault)
         entity._default = self._default
 
     def post_load_hook(self, doc: Drawing) -> None:
         # Set _default to None if default object not exist - audit() replaces
         # a not existing default object by a placeholder object.
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/dimension.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/dimension.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional, Union, Iterable, Iterator
 from typing_extensions import Self
 
 import math
 import logging
@@ -489,15 +489,15 @@
     def copy(self, copy_strategy=default_copy) -> Dimension:
         virtual_copy = super().copy(copy_strategy=copy_strategy)
         # The new virtual copy can not reference the same geometry block as the
         # original dimension entity:
         virtual_copy.dxf.discard("geometry")
         return virtual_copy
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, Dimension)
         if self.virtual_block_content:
             # another copy of a virtual entity:
             virtual_content = EntitySpace(
                 copy_strategy.copy(e) for e in self.virtual_block_content
             )
         else:
@@ -645,15 +645,15 @@
         if self.doc.dxfversion > const.DXF12:
             # overridden resources are referenced by handle
             register_override_handles(self, registry)
         else:
             # overridden resources are referenced by name
             self.override().register_resources_r12(registry)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         super().map_resources(clone, mapping)
         clone.dxf.dimstyle = mapping.get_dim_style(self.dxf.dimstyle)
         clone.dxf.geometry = mapping.get_block_name(self.dxf.geometry)
 
         # DXF R2000+ references overridden resources by group code 1005 handles in the
         # XDATA section, which are automatically mapped by the parent class DXFEntity!
         assert self.doc is not None
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/dimstyle.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/dimstyle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) 2019-2022, Manfred Moitzi
+# Copyright (c) 2019-2024, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Optional
+from typing_extensions import Self
 import logging
 from ezdxf.enums import MTextLineAlignment
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     VIRTUAL_TAG,
@@ -504,15 +505,15 @@
             arrow_name = self.dxf.get(attr_name)
             if arrow_name is None:
                 continue
             if not ARROWS.is_acad_arrow(arrow_name):
                 # user defined arrow head block
                 registry.add_block_name(arrow_name)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, DimStyle)
         super().map_resources(clone, mapping)
         # ezdxf uses names for blocks, linetypes and text style as internal data
         # map text style
         text_style = self.dxf.get(DIM_TEXT_STYLE_ATTR)
         if text_style:
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/dimstyleoverride.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/dimstyleoverride.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/dxfclass.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/dxfentity.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/dxfentity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 """ :class:`DXFEntity` is the super class of all DXF entities.
 
 The current entity system uses the features of the latest supported DXF version.
 
 The stored DXF version of the document is used to warn users if they use
 unsupported DXF features of the current DXF version.
@@ -21,15 +21,16 @@
     Iterable,
     Iterator,
     Optional,
     Type,
     TypeVar,
     Callable,
 )
-import copy
+from typing_extensions import Self
+
 import logging
 import uuid
 from ezdxf import options
 from ezdxf.lldxf import const
 from ezdxf.lldxf.tags import Tags
 from ezdxf.lldxf.types import DXFTag
 from ezdxf.lldxf.extendedtags import ExtendedTags
@@ -298,28 +299,28 @@
         entity.appdata = other.appdata
         entity.xdata = other.xdata
         entity.proxy_graphic = other.proxy_graphic
         entity.dxf.rewire(entity)
         # Do not set copy state, this is not a real copy!
         return entity
 
-    def copy(self: T, copy_strategy=default_copy) -> T:
+    def copy(self, copy_strategy=default_copy) -> Self:
         """Internal entity copy for usage in the same document or as virtual entity.
 
         Returns a copy of `self` but without handle, owner and reactors.
         This copy is NOT stored in the entity database and does NOT reside
         in any layout, block, table or objects section!
         The extension dictionary will be copied for entities bound to a valid
         DXF document. The reactors are not copied.
 
         (internal API)
         """
         return copy_strategy.copy(self)
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy entity data like vertices or attribs to the copy of the entity.
 
         This is the second stage of the copy process, see copy() method.
 
         (internal API)
         """
         pass
@@ -615,14 +616,21 @@
         del self.extension_dict
         del self.appdata
         del self.reactors
         del self.xdata
         del self.doc
         del self.dxf  # check mark for is_alive
 
+    def commit_pending_changes(self) -> None:
+        """Commit all unapplied changes like temporary transformations of ACIS entities.
+
+        (internal API)
+        """
+        pass
+
     def preprocess_export(self, tagwriter: AbstractTagWriter) -> bool:
         """Pre requirement check and pre-processing for export.
 
         Returns ``False``  if entity should not be exported at all.
 
         (internal API)
         """
@@ -927,15 +935,15 @@
             for name in self.xdata.data.keys():
                 registry.add_appid(name)
         if self.appdata:  # add hard owned entities
             for tags in self.appdata.tags():
                 for tag in tags.get_hard_owner_handles():
                     registry.add_handle(tag.value)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
 
         def map_xdata_resources():
             for index, (code, value) in enumerate(tags):
                 if code == 1005:  # map soft-pointer handles
                     tags[index] = DXFTag(code, mapping.get_handle(value))
                 elif code == 1003:  # map layer name
@@ -969,20 +977,20 @@
 
     def __init__(self) -> None:
         """Default constructor"""
         super().__init__()
         self.xtags = ExtendedTags()
         self.embedded_objects: Optional[list[Tags]] = None
 
-    def copy(self: T, copy_strategy=default_copy) -> T:
+    def copy(self, copy_strategy=default_copy) -> Self:
         raise CopyNotSupported(
             f"Copying of tag storage {self.dxftype()} not supported."
         )
 
-    def transform(self, m: Matrix44) -> DXFGraphic:
+    def transform(self, m: Matrix44) -> Self:
         raise NotImplementedError("cannot transform DXF tag storage")
 
     @property
     def base_class(self):
         return self.xtags.subclasses[0]
 
     @property
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/dxfgfx.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/dxfgfx.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional, Iterable, Any
-from typing_extensions import Self
+from typing_extensions import Self, TypeGuard
 
 from ezdxf.entities import factory
 from ezdxf import options
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
@@ -643,15 +643,15 @@
         registry.add_layer(dxf.layer)
         registry.add_linetype(dxf.linetype)
         registry.add_handle(dxf.get("material_handle"))
         # unsupported resource attributes:
         # - visualstyle_handle
         # - plotstyle_handle
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         super().map_resources(clone, mapping)
         clone.dxf.layer = mapping.get_layer(self.dxf.layer)
         attrib_exist = self.dxf.hasattr
         if attrib_exist("linetype"):
             clone.dxf.linetype = mapping.get_linetype(self.dxf.linetype)
         if attrib_exist("material_handle"):
@@ -699,15 +699,15 @@
         if layout.doc:
             factory.bind(target, layout.doc)
         layout.add_entity(target)
     else:
         source.destroy()
 
 
-def is_graphic_entity(entity: DXFEntity) -> bool:
+def is_graphic_entity(entity: DXFEntity) -> TypeGuard[DXFGraphic]:
     """Returns ``True`` if the `entity` has a graphical representations and
     can reside in the model space, a paper space or a block layout,
     otherwise the entity is a table or class entry or a DXF object from the
     OBJECTS section.
     """
     if isinstance(entity, DXFGraphic):
         return True
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/dxfgroups.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/dxfns.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/dxfns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/dxfobj.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/dxfobj.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Union, Any, Optional
+from typing_extensions import Self, TypeGuard
 import logging
 import array
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.const import DXF2000, DXFStructureError, SUBCLASS_MARKER
 from ezdxf.lldxf.tags import Tags
 from ezdxf.lldxf.types import dxftag, DXFTag, DXFBinaryTag
 from ezdxf.lldxf.attributes import (
@@ -82,15 +83,15 @@
     DXFTYPE = "XRECORD"
     DXFATTRIBS = DXFAttributes(base_class, acdb_xrecord)
 
     def __init__(self):
         super().__init__()
         self.tags = Tags()
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, XRecord)
         entity.tags = Tags(self.tags)
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
@@ -157,15 +158,15 @@
     DXFTYPE = "VBA_PROJECT"
     DXFATTRIBS = DXFAttributes(base_class, acdb_vba_project)
 
     def __init__(self):
         super().__init__()
         self.data = b""
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, VBAProject)
         entity.data = entity.data
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
@@ -240,15 +241,15 @@
     DXFTYPE = "SORTENTSTABLE"
     DXFATTRIBS = DXFAttributes(base_class, acdb_sort_ents_table)
 
     def __init__(self) -> None:
         super().__init__()
         self.table: dict[str, str] = dict()
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, SortEntsTable)
         entity.table = dict(entity.table)
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
@@ -383,15 +384,15 @@
 class Field(DXFObject):
     """DXF FIELD entity"""
 
     DXFTYPE = "FIELD"
     DXFATTRIBS = DXFAttributes(base_class, acdb_field)
 
 
-def is_dxf_object(entity: DXFEntity) -> bool:
+def is_dxf_object(entity: DXFEntity) -> TypeGuard[DXFObject]:
     """Returns ``True`` if the `entity` is a DXF object from the OBJECTS section,
     otherwise the entity is a table or class entry or a graphic entity which can
     not reside in the OBJECTS section.
     """
     if isinstance(entity, DXFObject):
         return True
     if isinstance(entity, DXFTagStorage) and not entity.is_graphic_entity:
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/ellipse.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/factory.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/geodata.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/geodata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/gradient.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/gradient.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/hatch.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/hatch.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/helix.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/idbuffer.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/idbuffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) 2019-2023, Manfred Moitzi
 # License: MIT-License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
+from typing_extensions import Self
 from ezdxf.lldxf.const import SUBCLASS_MARKER, DXFStructureError
 from ezdxf.lldxf.attributes import (
     DXFAttributes,
     DefSubclass,
     DXFAttr,
     group_code_mapping,
 )
@@ -31,15 +32,15 @@
     DXFTYPE = "IDBUFFER"
     DXFATTRIBS = DXFAttributes(base_class, acdb_id_buffer)
 
     def __init__(self) -> None:
         super().__init__()
         self.handles: list[str] = []
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy handles"""
         assert isinstance(entity, IDBuffer)
         entity.handles = list(self.handles)
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/image.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 
 import os
 import pathlib
 from typing import (
     TYPE_CHECKING,
@@ -63,15 +63,15 @@
         # Boundary/Clipping path coordinates:
         # 0/0 is in the Left/Top corner of the image!
         # x-coordinates increases in u_pixel vector direction
         # y-coordinates increases against the v_pixel vector!
         # see also WCS coordinate calculation
         self._boundary_path: list[Vec2] = []
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, ImageBase)
         entity._boundary_path = list(self._boundary_path)
 
     def post_new_hook(self) -> None:
         super().post_new_hook()
         self.reset_boundary_path()
 
@@ -346,15 +346,15 @@
             image_size = image_def.dxf.image_size
         dxfattribs.setdefault("image_size", image_size)
 
         image = cast("Image", super().new(handle, owner, dxfattribs, doc))
         image.image_def = image_def
         return image
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, Image)
         super().copy_data(entity, copy_strategy=copy_strategy)
         # Each IMAGE has its own ImageDefReactor object, which will be created by
         # binding the copy to the document.
         entity.dxf.discard("image_def_reactor_handle")
         entity._image_def_reactor = None
         # shared IMAGE_DEF
@@ -415,15 +415,15 @@
 
     def register_resources(self, registry: xref.Registry) -> None:
         """Register required resources to the resource registry."""
         super().register_resources(registry)
         if isinstance(self.image_def, ImageDef):
             registry.add_handle(self.image_def.dxf.handle)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, Image)
         super().map_resources(clone, mapping)
         source_image_def = self.image_def
         if isinstance(source_image_def, ImageDef):
             name = self.get_image_def_name()
             name, clone_image_def = mapping.map_acad_dict_entry(
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/insert.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import (
     TYPE_CHECKING,
     Iterable,
     Iterator,
     cast,
     Union,
     Optional,
     Callable,
 )
+from typing_extensions import Self
 import math
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     XType,
@@ -230,15 +231,15 @@
             self.process_sub_entities(lambda e: e.export_dxf(tagwriter))
 
     def register_resources(self, registry: xref.Registry) -> None:
         # The attached ATTRIB entities are registered by the parent class LinkedEntities
         super().register_resources(registry)
         registry.add_block_name(self.dxf.name)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         # The attached ATTRIB entities are mapped by the parent class LinkedEntities
         super().map_resources(clone, mapping)
         clone.dxf.name = mapping.get_block_name(self.dxf.name)
 
     @property
     def has_scaling(self) -> bool:
         """Returns ``True`` if scaling is applied to any axis."""
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/layer.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) 2019-2024, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional, cast, Any
+from typing_extensions import Self
 import logging
 from dataclasses import dataclass
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
@@ -384,15 +385,15 @@
         """Register required resources to the resource registry."""
         assert self.doc is not None, "LAYER entity must be assigned to a document"
         super().register_resources(registry)
         registry.add_linetype(self.dxf.linetype)
         registry.add_handle(self.dxf.get("material_handle"))
         # current plot style will be replaced by default plot style "Normal"
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, Layer)
         super().map_resources(clone, mapping)
         self.dxf.linetype = mapping.get_linetype(self.dxf.linetype)
 
         mapping.map_existing_handle(self, clone, "material_handle", optional=True)
         # remove handles pointing to the source document:
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/layout.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-#  Copyright (c) 2020-2023, Manfred Moitzi
+#  Copyright (c) 2020-2024, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
+from typing_extensions import Self
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.const import SUBCLASS_MARKER
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     XType,
@@ -251,15 +252,15 @@
             ],
         )
 
     def register_resources(self, registry: xref.Registry) -> None:
         super().register_resources(registry)
         registry.add_handle(self.dxf.get("shade_plot_handle"))
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         super().map_resources(clone, mapping)
         shade_plot_handle = self.dxf.get("shade_plot_handle")
         if shade_plot_handle and shade_plot_handle != "0":
             clone.dxf.shade_plot_handle = mapping.get_handle(shade_plot_handle)
         else:
             clone.dxf.discard("shade_plot_handle")
 
@@ -377,15 +378,15 @@
         )
 
     def register_resources(self, registry: xref.Registry) -> None:
         super().register_resources(registry)
         registry.add_handle(self.dxf.get("ucs_handle"))
         registry.add_handle(self.dxf.get("base_ucs_handle"))
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         super().map_resources(clone, mapping)
 
         # The content of paperspace layouts is not copied automatically and the
         # associated BLOCK_RECORD is created and assigned in a special method.
         mapping.map_existing_handle(self, clone, "ucs_handle", optional=True)
         mapping.map_existing_handle(self, clone, "base_ucs_handle", optional=True)
         mapping.map_existing_handle(self, clone, "viewport_handle", optional=True)
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/leader.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/leader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Optional, Iterator
+from typing_extensions import Self
 import logging
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     XType,
@@ -167,15 +168,15 @@
     DXFATTRIBS = DXFAttributes(base_class, acdb_entity, acdb_leader)
     MIN_DXF_VERSION_FOR_EXPORT = const.DXF2000
 
     def __init__(self) -> None:
         super().__init__()
         self.vertices: list[Vec3] = []
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy vertices."""
         assert isinstance(entity, Leader)
         entity.vertices = Vec3.list(self.vertices)
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
@@ -259,15 +260,15 @@
         if self.doc.dxfversion > const.DXF12:
             # overridden resources are referenced by handle
             register_override_handles(self, registry)
         else:
             # overridden resources are referenced by name
             self.override().register_resources_r12(registry)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         super().map_resources(clone, mapping)
         if self.dxf.hasattr("annotation_handle"):
             clone.dxf.annotation_handle = mapping.get_handle(self.dxf.annotation_handle)
 
         # DXF R2000+ references overridden resources by group code 1005 handles in the
         # XDATA section, which are automatically mapped by the parent class DXFEntity!
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/light.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/line.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/ltype.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/ltype.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# Copyright (c) 2019-2023, Manfred Moitzi
+# Copyright (c) 2019-2024, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import (
     TYPE_CHECKING,
     Union,
     Iterable,
     Sequence,
     Optional,
 )
+from typing_extensions import Self
 from copy import deepcopy
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     group_code_mapping,
 )
@@ -158,15 +159,15 @@
     )
 
     def __init__(self):
         """Default constructor"""
         super().__init__()
         self.pattern_tags = LinetypePattern(Tags())
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy pattern_tags."""
         assert isinstance(entity, Linetype)
         entity.pattern_tags = deepcopy(self.pattern_tags)
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
@@ -255,15 +256,15 @@
         super().register_resources(registry)
         # register text styles and shape files for complex linetypes
         style_handle = self.pattern_tags.get_style_handle()
         style = self.doc.styles.get_entry_by_handle(style_handle)
         if style is not None:
             registry.add_entity(style)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate registered resources from self to the copied entity."""
         assert isinstance(clone, Linetype)
         super().map_resources(clone, mapping)
         style_handle = self.pattern_tags.get_style_handle()
         if style_handle != "0":
             # map text style or shape file handle of complex linetype
             clone.pattern_tags.set_style_handle(mapping.get_handle(style_handle))
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/lwpolyline.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/lwpolyline.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     DXFATTRIBS = DXFAttributes(base_class, acdb_entity, acdb_lwpolyline)
     MIN_DXF_VERSION_FOR_EXPORT = DXF2000
 
     def __init__(self):
         super().__init__()
         self.lwpoints = LWPolylinePoints()
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy lwpoints."""
         assert isinstance(entity, LWPolyline)
         entity.lwpoints = copy.deepcopy(self.lwpoints)
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/material.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/material.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) 2018-2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
+from typing_extensions import Self
 from ezdxf.lldxf.const import SUBCLASS_MARKER
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     group_code_mapping,
 )
@@ -229,15 +230,15 @@
         self.specular_mapper_matrix: Optional[Matrix44] = None  # code 47
         self.reflexion_mapper_matrix: Optional[Matrix44] = None  # code 49
         self.opacity_mapper_matrix: Optional[Matrix44] = None  # group 142
         self.bump_mapper_matrix: Optional[Matrix44] = None  # group 144
         self.refraction_mapper_matrix: Optional[Matrix44] = None  # code 147
         self.normal_mapper_matrix: Optional[Matrix44] = None  # code 43 ???
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy material mapper matrices"""
 
         def copy(matrix):
             return None if matrix is None else matrix.copy()
 
         assert isinstance(entity, Material)
         entity.diffuse_mapper_matrix = copy(self.diffuse_mapper_matrix)
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/mesh.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     TYPE_CHECKING,
     Iterable,
     Sequence,
     Union,
     Iterator,
     Optional,
 )
+from typing_extensions import Self
 import array
 import copy
 from itertools import chain
 from contextlib import contextmanager
 
 from ezdxf.audit import AuditError
 from ezdxf.lldxf import validator
@@ -207,15 +208,15 @@
     def __init__(self):
         super().__init__()
         self._vertices = VertexArray()  # vertices stored as array.array('d')
         self._faces = FaceList()  # face lists data
         self._edges = EdgeArray()  # edge indices stored as array.array('L')
         self._creases = array.array("f")  # creases stored as array.array('f')
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy data: vertices, faces, edges, creases."""
         assert isinstance(entity, Mesh)
         entity._vertices = copy.deepcopy(self._vertices)
         entity._faces = copy.deepcopy(self._faces)
         entity._edges = copy.deepcopy(self._edges)
         entity._creases = copy.deepcopy(self._creases)
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/mleader.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/mleader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) 2018-2023, Manfred Moitzi
+# Copyright (c) 2018-2024, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union, Optional, Iterable, Any, Iterator
+from typing_extensions import Self
 import copy
 import logging
 import math
 from collections import namedtuple
 
 from ezdxf.lldxf import const
 from ezdxf.lldxf.types import cast_value
@@ -537,15 +538,15 @@
         registry.add_handle(dxf.text_style_handle)
         registry.add_handle(dxf.block_record_handle)
         for arrow_head in self.arrow_heads:
             registry.add_handle(arrow_head.handle)
         # block attdef entities are included in the block definition!
         self.context.register_resources(registry)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, MultiLeader)
         super().map_resources(clone, mapping)
         dxf = self.dxf
         clone_dxf = clone.dxf
         clone_dxf.style_handle = mapping.get_handle(dxf.style_handle)
         clone_dxf.leader_linetype_handle = mapping.get_handle(
@@ -1347,15 +1348,15 @@
 
     def register_resources(self, registry: xref.Registry) -> None:
         super().register_resources(registry)
         dxf = self.dxf
         for attrib_name in MLEADER_STYLE_HANDLE_ATTRIBS:
             registry.add_handle(dxf.get(attrib_name, "0"))
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         super().map_resources(clone, mapping)
         dxf = self.dxf
         for attrib_name in MLEADER_STYLE_HANDLE_ATTRIBS:
             if dxf.hasattr(attrib_name):
                 clone.dxf.set(attrib_name, mapping.get_handle(dxf.get(attrib_name)))
             else:
                 clone.dxf.discard(attrib_name)
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/mline.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/mline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2023, Manfred Moitzi
+# Copyright (c) 2018-2024, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import (
     TYPE_CHECKING,
     Iterable,
     Optional,
     Sequence,
@@ -328,15 +328,15 @@
         # change is applied.
         self.vertices: list[MLineVertex] = []
 
     def __len__(self):
         """Count of MLINE vertices."""
         return len(self.vertices)
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, MLine)
         entity.vertices = [v.copy() for v in self.vertices]
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
@@ -372,15 +372,15 @@
             vertex.export_dxf(tagwriter)
 
     def register_resources(self, registry: xref.Registry) -> None:
         """Register required resources to the resource registry."""
         super().register_resources(registry)
         registry.add_handle(self.dxf.style_handle)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         super().map_resources(clone, mapping)
         style = mapping.get_reference_of_copy(self.dxf.style_handle)
         if not isinstance(style, MLineStyle):
             assert clone.doc is not None
             style = clone.doc.mline_styles.get("Standard")
         if isinstance(style, MLineStyle):
@@ -871,15 +871,15 @@
     END_INNER_ARC = const.MLINESTYLE_END_INNER_ARC
     END_ROUND = const.MLINESTYLE_END_ROUND
 
     def __init__(self):
         super().__init__()
         self.elements = MLineStyleElements()
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, MLineStyle)
         entity.elements = self.elements.copy()
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
@@ -937,15 +937,15 @@
 
     def register_resources(self, registry: xref.Registry) -> None:
         """Register required resources to the resource registry."""
         super().register_resources(registry)
         for element in self.elements:
             registry.add_linetype(element.linetype)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, MLineStyle)
         super().map_resources(clone, mapping)
         self.elements.elements = [
             MLineStyleElement(
                 element.offset,
                 element.color,
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/mpolygon.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/mtext.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/mtext.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import (
     TYPE_CHECKING,
     Union,
     Iterable,
     Iterator,
     Optional,
     Callable,
     cast,
 )
+from typing_extensions import Self
 import enum
 import math
 import logging
 
 from ezdxf.lldxf import const, validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
@@ -679,15 +680,15 @@
         # Can't prevent access to _columns, but you are on your own if do this!
         return self._columns.shallow_copy() if self._columns else None
 
     @property
     def has_columns(self) -> bool:
         return self._columns is not None
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, MText)
         entity.text = self.text
         if self.has_columns:
             # copies also the linked MTEXT column entities!
             entity._columns = self._columns.deep_copy()  # type: ignore
 
     def load_dxf_attribs(
@@ -1232,15 +1233,15 @@
         super().register_resources(registry)
         if self.dxf.hasattr("style"):
             registry.add_text_style(self.dxf.style)
         if self._columns:
             for mtext in self._columns.linked_columns:
                 mtext.register_resources(registry)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, MText)
         super().map_resources(clone, mapping)
 
         if clone.dxf.hasattr("style"):
             clone.dxf.style = mapping.get_text_style(clone.dxf.style)
         if self._columns and clone._columns:
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/mtext_columns.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/objectcollection.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/objectcollection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/oleframe.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/oleframe.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/pattern.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/point.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/polygon.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/polygon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import Sequence, Optional, Union, TYPE_CHECKING, Iterator
+from typing_extensions import Self
 import abc
 import copy
 
 from ezdxf.lldxf import const
 from ezdxf.lldxf.tags import Tags
 from ezdxf import colors
 from ezdxf.tools import pattern
@@ -58,15 +59,15 @@
     def __init__(self) -> None:
         super().__init__()
         self.paths = BoundaryPaths()
         self.pattern: Optional[Pattern] = None
         self.gradient: Optional[Gradient] = None
         self.seeds: list[tuple[float, float]] = []  # not supported/exported by MPOLYGON
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy paths, pattern, gradient, seeds."""
         assert isinstance(entity, DXFPolygon)
         entity.paths = copy.deepcopy(self.paths)
         entity.pattern = copy.deepcopy(self.pattern)
         entity.gradient = copy.deepcopy(self.gradient)
         entity.seeds = copy.deepcopy(self.seeds)
 
@@ -136,15 +137,15 @@
 
         # Gradient data is always at the end of the AcDbHatch subclass.
         self.gradient = Gradient.load_tags(tags[index:])  # type: ignore
         # Remove gradient data from tags
         del tags[index:]
         return tags
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, DXFPolygon)
         assert clone.doc is not None
 
         super().map_resources(clone, mapping)
         db = clone.doc.entitydb
         for path in clone.paths:
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/polyline.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/shape.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/solid.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/spatial_filter.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/spatial_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Copyright (c) 2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional, Iterable
+from typing_extensions import Self
 import logging
 
 from ezdxf.lldxf import const, validator
 from ezdxf.lldxf.attributes import (
     DXFAttributes,
     DefSubclass,
     DXFAttr,
     XType,
     RETURN_DEFAULT,
     group_code_mapping,
 )
 from ezdxf.math import UVec, Vec2, Matrix44, Z_AXIS, NULLVEC
 from ezdxf.entities import factory
-from .dxfentity import SubclassProcessor, base_class, DXFEntity
+from .dxfentity import SubclassProcessor, base_class
 from .dxfobj import DXFObject
 from .copy import default_copy
 
 if TYPE_CHECKING:
     from ezdxf.lldxf.tags import Tags
     from ezdxf.entities import DXFNamespace
     from ezdxf.lldxf.tagwriter import AbstractTagWriter
@@ -79,15 +80,15 @@
         # transformation.  The original block reference transformation is the one that
         # is applied to all entities in the block when the block reference is regenerated.
         self._inverse_insert_matrix = Matrix44()
 
         # This matrix transforms points into the coordinate system of the clip boundary.
         self._transform_matrix = Matrix44()
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, SpatialFilter)
         # immutable data
         entity._boundary_vertices = self._boundary_vertices
         entity._inverse_insert_matrix = self._inverse_insert_matrix
         entity._transform_matrix = self._transform_matrix
 
     @property
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/spline.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/spline.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     List,
     Iterable,
     Sequence,
     cast,
     Iterator,
     Optional,
 )
-from typing_extensions import TypeAlias
+from typing_extensions import TypeAlias, Self
 import array
 import copy
 from ezdxf.audit import AuditError
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
@@ -158,15 +158,15 @@
     def __init__(self):
         super().__init__()
         self.fit_points = VertexArray()
         self.control_points = VertexArray()
         self.knots = []
         self.weights = []
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy data: control_points, fit_points, weights, knot_values."""
         assert isinstance(entity, Spline)
         entity._control_points = copy.deepcopy(self._control_points)
         entity._fit_points = copy.deepcopy(self._fit_points)
         entity._knots = copy.deepcopy(self._knots)
         entity._weights = copy.deepcopy(self._weights)
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/subentity.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/subentity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) 2020-2023, Manfred Moitzi
+# Copyright (c) 2020-2024, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Callable, Optional
+from typing_extensions import Self
 
 from ezdxf.entities import factory, DXFGraphic, SeqEnd, DXFEntity
 from ezdxf.lldxf import const
 from .copy import default_copy
 import logging
 
 if TYPE_CHECKING:
@@ -27,15 +28,15 @@
     """
 
     def __init__(self) -> None:
         super().__init__()
         self._sub_entities: list[DXFGraphic] = []
         self.seqend: Optional[SeqEnd] = None
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy all sub-entities ands SEQEND. (internal API)"""
         assert isinstance(entity, LinkedEntities)
         entity._sub_entities = [
             copy_strategy.copy(e) for e in self._sub_entities
         ]
         if self.seqend:
             entity.seqend = copy_strategy.copy(self.seqend)
@@ -127,15 +128,15 @@
         super().destroy()
 
     def register_resources(self, registry: xref.Registry) -> None:
         """Register required resources to the resource registry."""
         super().register_resources(registry)
         self.process_sub_entities(lambda e: e.register_resources(registry))
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         assert isinstance(clone, LinkedEntities)
         super().map_resources(clone, mapping)
         for source, _clone in zip(self.all_sub_entities(), clone.all_sub_entities()):
             source.map_resources(_clone, mapping)
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/sun.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/table.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/text.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
+from typing_extensions import Self
 import math
 
 from ezdxf.lldxf import validator
 from ezdxf.lldxf import const
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
@@ -377,15 +378,15 @@
 
     def register_resources(self, registry: xref.Registry) -> None:
         """Register required resources to the resource registry."""
         super().register_resources(registry)
         if self.dxf.hasattr("style"):
             registry.add_text_style(self.dxf.style)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         """Translate resources from self to the copied entity."""
         super().map_resources(clone, mapping)
         if clone.dxf.hasattr("style"):
             clone.dxf.style = mapping.get_text_style(clone.dxf.style)
 
     def plain_text(self) -> str:
         """Returns text content without formatting codes."""
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/textstyle.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/textstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/tolerance.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/tolerance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
+from typing_extensions import Self
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     XType,
     RETURN_DEFAULT,
     group_code_mapping,
 )
 from ezdxf.lldxf.const import SUBCLASS_MARKER, DXF2000
 from ezdxf.math import NULLVEC, Z_AXIS, X_AXIS
 from ezdxf.math.transformtools import transform_extrusion
-from .dxfentity import base_class, SubclassProcessor, DXFEntity
+from .dxfentity import base_class, SubclassProcessor
 from .dxfgfx import DXFGraphic, acdb_entity
 from .factory import register_entity
 
 if TYPE_CHECKING:
     from ezdxf.entities import DXFNamespace
     from ezdxf.lldxf.tagwriter import AbstractTagWriter
     from ezdxf.math import Matrix44
@@ -87,15 +88,15 @@
             ["dimstyle", "insert", "content", "extrusion", "x_axis_vector"],
         )
 
     def register_resources(self, registry: xref.Registry) -> None:
         super().register_resources(registry)
         registry.add_dim_style(self.dxf.dimstyle)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         super().map_resources(clone, mapping)
         clone.dxf.dimstyle = mapping.get_dim_style(self.dxf.dimstyle)
 
     def transform(self, m: Matrix44) -> Tolerance:
         """Transform the TOLERANCE entity by transformation matrix `m` inplace."""
         self.dxf.insert = m.transform(self.dxf.insert)
         self.dxf.x_axis_vector = m.transform_direction(self.dxf.x_axis_vector)
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/ucs.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/underlay.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/underlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union, Iterable, Optional
+from typing_extensions import Self
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     XType,
     RETURN_DEFAULT,
@@ -113,15 +114,15 @@
     MIN_DXF_VERSION_FOR_EXPORT = DXF2000
 
     def __init__(self) -> None:
         super().__init__()
         self._boundary_path: list[UVec] = []
         self._underlay_def: Optional[UnderlayDefinition] = None
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, Underlay)
         entity._boundary_path = list(self._boundary_path)
         entity._underlay_def = self._underlay_def
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
@@ -193,15 +194,15 @@
             tagwriter.write_vertex(11, vertex[:2])
 
     def register_resources(self, registry: xref.Registry) -> None:
         super().register_resources(registry)
         if isinstance(self._underlay_def, UnderlayDefinition):
             registry.add_handle(self._underlay_def.dxf.handle)
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         assert isinstance(clone, Underlay)
         super().map_resources(clone, mapping)
         underlay_def_copy = self.map_underlay_def(clone, mapping)
         clone._underlay_def = underlay_def_copy
         clone.dxf.underlay_def_handle = underlay_def_copy.dxf.handle
         underlay_def_copy.append_reactor_handle(clone.dxf.handle)
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/view.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/view.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/viewport.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/viewport.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterable, Optional
+from typing_extensions import Self
 import math
 from ezdxf.lldxf import validator
 from ezdxf.lldxf import const
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
@@ -261,15 +262,15 @@
     # paper space. For the following viewports it seems only important, that
     # the id is greater than 1.
 
     def __init__(self) -> None:
         super().__init__()
         self._frozen_layers: list[str] = []
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         assert isinstance(entity, Viewport)
         entity._frozen_layers = list(self._frozen_layers)
 
     @property
     def frozen_layers(self) -> list[str]:
         """Set/get frozen layers as list of layer names."""
         return self._frozen_layers
@@ -537,15 +538,15 @@
         registry.add_handle(self.dxf.get("ucs_handle"))
         registry.add_handle(self.dxf.get("base_ucs_handle"))
         registry.add_handle(self.dxf.get("visual_style_handle"))
         registry.add_handle(self.dxf.get("background_handle"))
         registry.add_handle(self.dxf.get("shade_plot_handle"))
         registry.add_handle(self.dxf.get("sun_handle"))
 
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+    def map_resources(self, clone: Self, mapping: xref.ResourceMapper) -> None:
         assert isinstance(clone, Viewport)
         super().map_resources(clone, mapping)
 
         mapping.map_existing_handle(
             self, clone, "clipping_boundary_handle", optional=True
         )
         mapping.map_existing_handle(self, clone, "ucs_handle", optional=True)
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/visualstyle.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/visualstyle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) 2019-2023, Manfred Moitzi
 # License: MIT-License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
+from typing_extensions import Self
 import copy
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.const import SUBCLASS_MARKER, DXF2000, DXFStructureError
 from ezdxf.lldxf.attributes import (
     DXFAttributes,
     DefSubclass,
     DXFAttr,
@@ -147,15 +148,15 @@
     DXFATTRIBS = DXFAttributes(base_class, acdb_visualstyle)
     MIN_DXF_VERSION_FOR_EXPORT = DXF2000  # official supported in R2007
 
     def __init__(self):
         super().__init__()
         self.acad_xdata = None  # to preserve AutoCAD xdata
 
-    def copy_data(self, entity: DXFEntity, copy_strategy=default_copy) -> None:
+    def copy_data(self, entity: Self, copy_strategy=default_copy) -> None:
         """Copy acad internal data."""
         assert isinstance(entity, VisualStyle)
         entity.acad_xdata = copy.deepcopy(self.acad_xdata)
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/vport.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/vport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/xdata.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/xdict.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/xdict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/xline.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/entities/__init__.py` & `ezdxf-1.3.0rc0/src/ezdxf/entities/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/fonts/fonts.py` & `ezdxf-1.3.0rc0/src/ezdxf/fonts/fonts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/fonts/font_face.py` & `ezdxf-1.3.0rc0/src/ezdxf/fonts/font_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/fonts/font_manager.py` & `ezdxf-1.3.0rc0/src/ezdxf/fonts/font_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/fonts/font_measurements.py` & `ezdxf-1.3.0rc0/src/ezdxf/fonts/font_measurements.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/fonts/glyphs.py` & `ezdxf-1.3.0rc0/src/ezdxf/fonts/glyphs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/fonts/lff.py` & `ezdxf-1.3.0rc0/src/ezdxf/fonts/lff.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/fonts/shapefile.py` & `ezdxf-1.3.0rc0/src/ezdxf/fonts/shapefile.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/fonts/ttfonts.py` & `ezdxf-1.3.0rc0/src/ezdxf/fonts/ttfonts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/layouts/base.py` & `ezdxf-1.3.0rc0/src/ezdxf/layouts/base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/layouts/blocklayout.py` & `ezdxf-1.3.0rc0/src/ezdxf/layouts/blocklayout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/layouts/layout.py` & `ezdxf-1.3.0rc0/src/ezdxf/layouts/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/layouts/layouts.py` & `ezdxf-1.3.0rc0/src/ezdxf/layouts/layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/attributes.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/const.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/encoding.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/extendedtags.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/extendedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/fileindex.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/fileindex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/hdrvars.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/hdrvars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/loader.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/packedtags.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/packedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/repair.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/repair.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/tagger.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/tagger.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/tags.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/tagwriter.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/tagwriter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/types.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/lldxf/validator.py` & `ezdxf-1.3.0rc0/src/ezdxf/lldxf/validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/arc.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/bbox.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/bezier.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/bezier_interpolation.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/bezier_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/box.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/bspline.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/bulge.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/circle.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/clipping.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/clustering.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/clustering.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/construct2d.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/construct2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/construct3d.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/construct3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/cspline.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/cspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/curvetools.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/curvetools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/ellipse.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/eulerspiral.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/eulerspiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/legacy.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/legacy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/linalg.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/line.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/offset2d.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/offset2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/parametrize.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/parametrize.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/perlin.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/perlin.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/polyline.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/rtree.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/shape.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/transformtools.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/transformtools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/triangulation.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/triangulation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/ucs.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/_bezier3p.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/_bezier4p.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/_bspline.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/_construct.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/_construct.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/_ctypes.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/_ctypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/_mapbox_earcut.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/_matrix44.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/_vector.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/_vector.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/math/__init__.py` & `ezdxf-1.3.0rc0/src/ezdxf/math/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/path/commands.py` & `ezdxf-1.3.0rc0/src/ezdxf/path/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/path/converter.py` & `ezdxf-1.3.0rc0/src/ezdxf/path/converter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/path/nesting.py` & `ezdxf-1.3.0rc0/src/ezdxf/path/nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/path/path.py` & `ezdxf-1.3.0rc0/src/ezdxf/path/path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/path/shapes.py` & `ezdxf-1.3.0rc0/src/ezdxf/path/shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/path/tools.py` & `ezdxf-1.3.0rc0/src/ezdxf/path/tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/abstract_mtext_renderer.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/abstract_mtext_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/arrows.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/curves.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/curves.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/dimension.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/dim_base.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/dim_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/dim_curved.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/dim_curved.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/dim_diameter.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/dim_diameter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/dim_linear.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/dim_linear.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/dim_ordinate.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/dim_ordinate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/dim_radius.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/dim_radius.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/forms.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/hatching.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/leader.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/linetypes.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/mesh.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/mleader.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/mline.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/point.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/polyline.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/r12spline.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/trace.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/_linetypes.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/_linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/render/__init__.py` & `ezdxf-1.3.0rc0/src/ezdxf/render/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/16x16.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/16x16.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/24x24.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/24x24.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/256x256.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/256x256.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/32x32.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/32x32.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/48x48.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/48x48.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/64x64.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/64x64.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/icon-copy-64px.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-copy-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/icon-find-64px.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-find-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/icon-goto-bookmark-64px.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/icon-goto-handle-64px.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-handle-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/icon-goto-line-64px.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-goto-line-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/icon-left-arrow-64px.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-left-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/icon-next-entity-64px.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-next-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/icon-prev-entity-64px.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-prev-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/icon-right-arrow-64px.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-right-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/icon-show-in-tree-64px.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-show-in-tree-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/resources/icon-store-bookmark-64px.png` & `ezdxf-1.3.0rc0/src/ezdxf/resources/icon-store-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/sections/acdsdata.py` & `ezdxf-1.3.0rc0/src/ezdxf/sections/acdsdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/sections/blocks.py` & `ezdxf-1.3.0rc0/src/ezdxf/sections/blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/sections/classes.py` & `ezdxf-1.3.0rc0/src/ezdxf/sections/classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/sections/entities.py` & `ezdxf-1.3.0rc0/src/ezdxf/sections/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/sections/header.py` & `ezdxf-1.3.0rc0/src/ezdxf/sections/header.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/sections/headervars.py` & `ezdxf-1.3.0rc0/src/ezdxf/sections/headervars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/sections/objects.py` & `ezdxf-1.3.0rc0/src/ezdxf/sections/objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/sections/table.py` & `ezdxf-1.3.0rc0/src/ezdxf/sections/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/sections/tables.py` & `ezdxf-1.3.0rc0/src/ezdxf/sections/tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/analyze.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/analyze.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/binarydata.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/binarydata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/clipping_portal.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/clipping_portal.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/codepage.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/codepage.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/complex_ltype.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/complex_ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/crypt.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/debug.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/debug.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/difftags.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/handle.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/indexing.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/juliandate.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/pattern.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/rawloader.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/rawloader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/standards.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/standards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/strip.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/strip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/test.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/test.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/text.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/text_layout.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/text_size.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/zipmanager.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/zipmanager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/_iso_pattern.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/_iso_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf/tools/__init__.py` & `ezdxf-1.3.0rc0/src/ezdxf/tools/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/src/ezdxf.egg-info/PKG-INFO` & `ezdxf-1.3.0rc0/src/ezdxf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.3.0b1
+Version: 1.3.0rc0
 Summary: A Python package to create/manipulate DXF drawings.
 Author-email: Manfred Moitzi <me@mozman.at>
 Project-URL: Repository, https://github.com/mozman/ezdxf
 Project-URL: Documentation, https://ezdxf.readthedocs.io
 Project-URL: Changelog, https://ezdxf.mozman.at/notes/#/page/changelog
 Project-URL: Forum, https://github.com/mozman/ezdxf/discussions
 Project-URL: Issues, https://github.com/mozman/ezdxf/issues
```

## Comparing `ezdxf-1.3.0b1/src/ezdxf.egg-info/SOURCES.txt` & `ezdxf-1.3.0rc0/src/ezdxf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 pyproject.toml
 requirements.txt
 setup.py
 integration_tests/check_disable_c_ext_by_config_file.py
 integration_tests/check_disable_c_ext_by_env_var.py
 integration_tests/conftest.py
 integration_tests/test_acad_table.py
+integration_tests/test_acis_entites.py
 integration_tests/test_all_dimline_styles.py
 integration_tests/test_all_ellipse_transformations.py
 integration_tests/test_anonymous_blocks.py
 integration_tests/test_appsettings.py
 integration_tests/test_audit_critical_dxf_files.py
 integration_tests/test_audit_layouts.py
 integration_tests/test_complex_line_type_2.py
@@ -50,14 +51,15 @@
 integration_tests/test_recover.py
 integration_tests/test_redraw_order.py
 integration_tests/test_rotated_block_attributes.py
 integration_tests/test_surface_entities.py
 integration_tests/test_write_fixed_meta_data.py
 integration_tests/test_write_without_handles.py
 integration_tests/test_xref_detach.py
+integration_tests/test_xref_load_acis.py
 integration_tests/data/AC1003_LINE_Example.dxf
 integration_tests/data/ASCII_R12.dxf
 integration_tests/data/Leica_Disto_S910.dxf
 integration_tests/data/MODEL.dxf
 integration_tests/data/PLOTFILE.plt
 integration_tests/data/POLI-ALL210_12.DXF
 integration_tests/data/R12_with_trash_beyond_EOF.dxf
@@ -298,14 +300,15 @@
 src/ezdxf/entities/shape.py
 src/ezdxf/entities/solid.py
 src/ezdxf/entities/spatial_filter.py
 src/ezdxf/entities/spline.py
 src/ezdxf/entities/subentity.py
 src/ezdxf/entities/sun.py
 src/ezdxf/entities/table.py
+src/ezdxf/entities/temporary_transform.py
 src/ezdxf/entities/text.py
 src/ezdxf/entities/textstyle.py
 src/ezdxf/entities/tolerance.py
 src/ezdxf/entities/ucs.py
 src/ezdxf/entities/underlay.py
 src/ezdxf/entities/view.py
 src/ezdxf/entities/viewport.py
@@ -574,17 +577,19 @@
 tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
 tests/test_02_dxf_graphics/test_229b_hatch_extended.py
 tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
 tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
 tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
 tests/test_02_dxf_graphics/test_231_underlay.py
 tests/test_02_dxf_graphics/test_231_underlay_2.py
-tests/test_02_dxf_graphics/test_232_acis.py
-tests/test_02_dxf_graphics/test_232_acis_2.py
-tests/test_02_dxf_graphics/test_232_surface.py
+tests/test_02_dxf_graphics/test_232a_add_acis.py
+tests/test_02_dxf_graphics/test_232b_acis_export.py
+tests/test_02_dxf_graphics/test_232c_acis_surface.py
+tests/test_02_dxf_graphics/test_232d_acis_copy.py
+tests/test_02_dxf_graphics/test_232e_acis_transform.py
 tests/test_02_dxf_graphics/test_233_helix.py
 tests/test_02_dxf_graphics/test_234_light.py
 tests/test_02_dxf_graphics/test_235_leader.py
 tests/test_02_dxf_graphics/test_236_multileader.py
 tests/test_02_dxf_graphics/test_237_mline.py
 tests/test_02_dxf_graphics/test_238_tolerance.py
 tests/test_02_dxf_graphics/test_239_proxy_graphic.py
```

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_012_crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_016_encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_018_handle.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_018_handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_040_tags.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_040_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_056_special_string_decoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_00_dxf_low_level_structs/test_058_json_tags.py` & `ezdxf-1.3.0rc0/tests/test_00_dxf_low_level_structs/test_058_json_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_101_dxfnamespace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_102_appdata.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_102_appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_103_reactors.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_103_reactors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_104_extension_dict.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_104_extension_dict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_105_xdata.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_105_xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_110_dxfentity.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_110_dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_112a_dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_112b_dxfobj.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_112b_dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_113_dxfclass.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_113_dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_114_factory.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_114_factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_116_dictionary.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_116_dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_117_layer_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_120_style_table_entry.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_120_style_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_123_view_table_entry.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_123_view_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_125_image_def.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_125_image_def.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_126_image_def_reactor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_127_raster_variables.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_127_raster_variables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_128_pdf_definition.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_128_pdf_definition.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_129_xrecord.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_129_xrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_130_id_buffer.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_130_id_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_131_field_list.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_131_field_list.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_132_layer_filter.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_132_layer_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_133_sun.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_133_sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_134_material.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_134_material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_135_geo_data.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_135_geo_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_136_vba_project.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_136_vba_project.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_137_sortentstable.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_137_sortentstable.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_139_user_record.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_139_user_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_140_block_record.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_140_block_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_141_layer_vp_override.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_142_copy_strategy.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_142_copy_strategy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_143_spatial_filter.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_143_spatial_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py` & `ezdxf-1.3.0rc0/tests/test_01_dxf_entities/test_144_roundtrip_xrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/conftest.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_200_line.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_200_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_201_point.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_201_point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_202_circle.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_202_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_203_arc.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_203_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_204_shape.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_204_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_205_solid.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_205_solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_206_text.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_206_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_207_attdef.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_207_attdef.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_208_attrib.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_208_attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_209_vertex.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_209_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_210_polyline_1.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_210_polyline_2.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_211_viewport.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_211_viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_212_insert.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_212_insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_213_minsert.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_213_minsert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_214_block.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_214_block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_215_dimension.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_215_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_221_ellipse.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_221_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_222_xline.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_222_xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_223_ray.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_223_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_224_group.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_224_group.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_225_mtext.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_225_mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_226_spline.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_226_spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_228_mesh.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_228_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_231_underlay.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_231_underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_231_underlay_2.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_231_underlay_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_232_acis.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232a_add_acis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2014-2022, Manfred Moitzi
+# Copyright (c) 2014-2024, Manfred Moitzi
 # License: MIT License
 import pytest
 import ezdxf
 
 from ezdxf.entities.acis import tags2textlines, textlines2tags
```

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_232_acis_2.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232b_acis_export.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-# Copyright (c) 2019 Manfred Moitzi
+# Copyright (c) 2019-2024 Manfred Moitzi
 # License: MIT License
-# created 2019-02-15
 import pytest
-import math
 
 from ezdxf.entities.acis import (
     Body,
     Solid3d,
     Region,
     Surface,
     ExtrudedSurface,
     LoftedSurface,
     RevolvedSurface,
     SweptSurface,
 )
+from ezdxf.entities import DXFEntity
 from ezdxf.lldxf.tagwriter import TagCollector, basic_tags_from_text
+from ezdxf.lldxf.tags import Tags
+from ezdxf.lldxf.const import DXF2010
 
 BODY = """0
 BODY
 5
 0
 330
 0
@@ -31,22 +32,32 @@
 70
 1
 """
 
 
 class MockDoc:
     def __init__(self):
-        self.dxfversion = "AC1024"
+        self.dxfversion = DXF2010
 
 
 @pytest.fixture
 def entity():
     return Body.from_text(BODY, doc=MockDoc())
 
 
+def special_export(entity: DXFEntity, dxfversion=DXF2010):
+    """These ACIS entities do not contain any ACIS data, which the regular export method
+    does not export.
+    """
+    collector = TagCollector(dxfversion=dxfversion)
+    entity.export_base_class(collector)
+    entity.export_entity(collector)
+    return Tags(collector.tags)
+
+
 def test_registered():
     from ezdxf.entities.factory import ENTITY_CLASSES
 
     assert "BODY" in ENTITY_CLASSES
     assert "3DSOLID" in ENTITY_CLASSES
     assert "REGION" in ENTITY_CLASSES
     assert "SURFACE" in ENTITY_CLASSES
@@ -96,24 +107,31 @@
 
 def test_load_from_text(entity):
     assert entity.dxf.layer == "0"
     assert entity.dxf.color == 256, "default color is 256 (by layer)"
     assert entity.dxf.version == 1
 
 
+def test_regular_dxf_export_of_empty_acis_entities():
+    entity = Body.from_text(BODY, doc=MockDoc())
+    assert (
+        len(TagCollector.dxftags(entity, DXF2010)) == 0
+    ), "do not export ACIS entities without content"
+
+
 def test_body_write_dxf():
     entity = Body.from_text(BODY, doc=MockDoc())
-    result = TagCollector.dxftags(entity)
+    result = special_export(entity)
     expected = basic_tags_from_text(BODY)
     assert result == expected
 
 
 def test_region_write_dxf():
     entity = Region.from_text(REGION, doc=MockDoc())
-    result = TagCollector.dxftags(entity)
+    result = special_export(entity, dxfversion=DXF2010)
     expected = basic_tags_from_text(REGION)
     assert result == expected
 
 
 REGION = """0
 REGION
 5
@@ -129,15 +147,15 @@
 70
 1
 """
 
 
 def test_3dsolid_write_dxf():
     entity = Solid3d.from_text(SOLID3D, doc=MockDoc())
-    result = TagCollector.dxftags(entity)
+    result = special_export(entity, dxfversion=DXF2010)
     expected = basic_tags_from_text(SOLID3D)
     assert result == expected
 
 
 SOLID3D = """0
 3DSOLID
 5
@@ -157,15 +175,15 @@
 350
 0
 """
 
 
 def test_surface_write_dxf():
     entity = Surface.from_text(SURFACE, doc=MockDoc())
-    result = TagCollector.dxftags(entity)
+    result = special_export(entity, dxfversion=DXF2010)
     expected = basic_tags_from_text(SURFACE)
     assert result == expected
 
 
 SURFACE = """0
 SURFACE
 5
@@ -187,15 +205,15 @@
 72
 0
 """
 
 
 def test_extruded_surface_write_dxf():
     entity = ExtrudedSurface.from_text(EXTRUDEDSURFACE, doc=MockDoc())
-    result = TagCollector.dxftags(entity)
+    result = special_export(entity, dxfversion=DXF2010)
     expected = basic_tags_from_text(EXTRUDEDSURFACE)
     assert result == expected
 
 
 EXTRUDEDSURFACE = """0
 EXTRUDEDSURFACE
 5
@@ -357,15 +375,15 @@
 31
 0.0
 """
 
 
 def test_lofted_surface_write_dxf():
     entity = LoftedSurface.from_text(LOFTEDSURFACE, doc=MockDoc())
-    result = TagCollector.dxftags(entity)
+    result = special_export(entity, dxfversion=DXF2010)
     expected = basic_tags_from_text(LOFTEDSURFACE)
     assert result == expected
 
 
 LOFTEDSURFACE = """0
 LOFTEDSURFACE
 5
@@ -447,15 +465,15 @@
 297
 1
 """
 
 
 def test_revolved_surface_write_dxf():
     entity = RevolvedSurface.from_text(REVOLVEDSURFACE, doc=MockDoc())
-    result = TagCollector.dxftags(entity)
+    result = special_export(entity, dxfversion=DXF2010)
     expected = basic_tags_from_text(REVOLVEDSURFACE)
     assert result == expected
 
 
 REVOLVEDSURFACE = """0
 REVOLVEDSURFACE
 5
@@ -541,15 +559,15 @@
 291
 0
 """
 
 
 def test_swept_surface_write_dxf():
     entity = SweptSurface.from_text(SWEPTSURFACE, doc=MockDoc())
-    result = TagCollector.dxftags(entity)
+    result = special_export(entity, dxfversion=DXF2010)
     expected = basic_tags_from_text(SWEPTSURFACE)
     assert result == expected
 
 
 SWEPTSURFACE = """0
 SWEPTSURFACE
 5
@@ -735,7 +753,10 @@
 11
 0.0
 21
 0.0
 31
 0.0
 """
+
+if __name__ == "__main__":
+    pytest.main([__file__])
```

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_232_surface.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_232c_acis_surface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2018-2019 Manfred Moitzi
+# Copyright (c) 2018-2024 Manfred Moitzi
 # License: MIT License
 import ezdxf
 from ezdxf.math import Matrix44
 import pytest
 
 IDENTITY_MATRIX = list(list(Matrix44()))
```

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_233_helix.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_233_helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_234_light.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_234_light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_235_leader.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_235_leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_236_multileader.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_236_multileader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_237_mline.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_237_mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_238_tolerance.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_238_tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_240_arc_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_241_hyperlink.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_241_hyperlink.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_242_random_transform.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_242_random_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_243_replace_entity.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_243_replace_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_245_wipeout.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_245_wipeout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_246_spline_audit.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_246_spline_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_248_mpolygon.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_248_mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_249_boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_251_upright.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_251_upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_253_ole2frame.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_253_ole2frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_02_dxf_graphics/test_254_get_font_name.py` & `ezdxf-1.3.0rc0/tests/test_02_dxf_graphics/test_254_get_font_name.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_300_layout.py` & `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_300_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py` & `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_302_block_references.py` & `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_302_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py` & `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_303_auto_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py` & `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_304_new_entity_space.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py` & `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py` & `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_307_groupby.py` & `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_307_groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_308_query.py` & `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_308_query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_309_query_parser.py` & `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_309_query_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py` & `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py` & `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_312_virtual_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_03_dxf_layouts/test_313_redraw_order.py` & `ezdxf-1.3.0rc0/tests/test_03_dxf_layouts/test_313_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_401_headersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_402_classessection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_404a_tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_405_classes.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_405_classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_410_table.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_410_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_417_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_424_audit.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_424_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_04_dxf_high_level_structs/test_429_xclip.py` & `ezdxf-1.3.0rc0/tests/test_04_dxf_high_level_structs/test_429_xclip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/conftest.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_500_units.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_500_units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_501_truecolor.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_501_truecolor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_502_raw_color.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_502_raw_color.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_503_indexing.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_503_indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_504_suppress_zeros.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_504_suppress_zeros.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_508_read_zip.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_508_read_zip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_509_comments.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_509_comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_510_byte_stream.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_510_byte_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_511_bit_stream.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_511_bit_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_512_pattern.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_512_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_513_reorder_entities.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_513_reorder_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_514_text.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_514_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_515a_fonts_truetype.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_515a_fonts_truetype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_515b_fonts_shapefiles.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_515b_fonts_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_515c_fonts_lff.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_515c_fonts_lff.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_516_zoom.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_516_zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_517_text_layout.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_517_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_519_mtext_editor.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_519_mtext_editor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_520_mtext_context.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_520_mtext_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_521_mtext_parser.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_521_mtext_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_522_text_scanner.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_522_text_scanner.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_523_text_size.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_523_text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_524_block_reference_manager.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_524_block_reference_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_525_transparency.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_525_transparency.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_526_explode.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_526_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_527_gfxattribs.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_527_gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_528_difftags.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_528_difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_529_acis_sat.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_529_acis_sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_530_acis_sab.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_530_acis_sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_531_acis_entities.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_531_acis_entities.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-#  Copyright (c) 2022, Manfred Moitzi
+#  Copyright (c) 2022-2024, Manfred Moitzi
 #  License: MIT License
 
 import pytest
-import ezdxf
 from ezdxf.acis.api import load, export_sat, export_sab, ExportError
 from ezdxf.acis import sat, sab, entities, hdr, const, mesh
 from ezdxf.math import Matrix44
 import math
 
 
 def test_load_any_format(any_cube):
```

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_532_acis_mesh.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_532_acis_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_533_shapefiles.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_533_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_534_dwg_info.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_534_dwg_info.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_535_xref_basic.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_535_xref_basic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_536_xref_conflict.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_536_xref_conflict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_537_transform.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_537_transform.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,20 +54,29 @@
         from ezdxf.entities import Layer
 
         m = transform.Matrix44.translate(1, 0, 0)
         log = transform.inplace([Layer.new()], m)
         assert log[0].error == transform.Error.TRANSFORMATION_NOT_SUPPORTED
 
     def test_acis_entities(self):
-        # ACIS entities do not have transformation support yet, but maybe in the future!
+        # new in v1.3.0: ACIS entities support a temporary transformation
+        #
+        # This way a temporary transformation of ACIS entities is stored by ezdxf.
+        # This temp. transformation has to be applied before export otherwise a warning 
+        # will be logged.
+
         msp = VirtualLayout()
-        msp.add_body()  # ACIS entity
-        m = transform.Matrix44.translate(1, 0, 0)
+        body = msp.add_body()  # ACIS entity
+        m = transform.Matrix44.translate(1, 2, 3)
         log = transform.inplace(msp, m)
-        assert log[0].error == transform.Error.TRANSFORMATION_NOT_SUPPORTED
+        assert len(log) == 0
+
+        m2 = body.temporary_transformation().get_matrix()
+        v = (3, 2, 1)
+        assert m.transform(v).isclose(m2.transform(v))
 
 
 class TestConvenientFunctions:
     @pytest.fixture
     def msp(self):
         msp = VirtualLayout()
         msp.add_point((1, 1, 1))
```

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_539_npshapes.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_539_npshapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_540_lff_parser.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_540_lff_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_541_clipping_portal.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_541_clipping_portal.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_542_itertools.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_542_itertools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_543_select.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_543_select.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_05_tools/test_544_revcloud.py` & `ezdxf-1.3.0rc0/tests/test_05_tools/test_544_revcloud.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/conftest.py` & `ezdxf-1.3.0rc0/tests/test_06_math/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_600_base.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_600_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_601_bulge.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_601_bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_602_vec3.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_602_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_603_vec2.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_603_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_604_banded_matrix.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_604_banded_matrix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_604_linalg.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_604_linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_605_matrix44.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_605_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_606_convexhull.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_606_convexhull.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_607_perlin_noise.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_607_perlin_noise.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_608_intersection_line_line_2d.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_608_intersection_line_line_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_609_point_on_line.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_609_point_on_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_610_ocs.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_610_ocs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_611_ucs.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_611_ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_612_ucs_pass_trough.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_612_ucs_pass_trough.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_613_is_point_in_polygon_2d.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_613_is_point_in_polygon_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_614_construct_3d.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_614_construct_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_615_rytz_axis.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_615_rytz_axis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_616_plane.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_616_plane.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_617_clockwise_orientation.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_617_clockwise_orientation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_618_clipping.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_618_clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_619_greiner_hormann.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_619_greiner_hormann.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_620_knot.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_620_knot.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_621_bspline.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_621_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_622_bsplineu.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_622_bsplineu.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_623_rbspline.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_623_rbspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_624_global_bspline_interpolation.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_624_global_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_626_local_bspline_interpolation.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_626_local_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_627_bspline_basis.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_627_bspline_basis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_629_bezier.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_629_bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_630a_bezier4p_base.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_630a_bezier4p_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_630b_bezier4p_functions.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_630b_bezier4p_functions.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_631_euler_spiral.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_631_euler_spiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_632_bezier3p.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_632_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_640_bbox.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_640_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_641_construction_ray.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_641_construction_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_642_construction_line.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_642_construction_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_643_construction_box.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_643_construction_box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_644_construction_circle.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_644_construction_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_645_construction_arc.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_645_construction_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_646_offset_vertices_2d.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_646_offset_vertices_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_647_transform_tools.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_647_transform_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_648_construction_ellipse.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_648_construction_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_650_elliptic_arc_span.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_650_elliptic_arc_span.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_651_construction_polyline.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_651_construction_polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_652_approx_param_t.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_652_approx_param_t.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_653_polyline_intersection.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_653_polyline_intersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_654_rtree.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_654_rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_655_dbscan.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_655_dbscan.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_656_k_means.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_656_k_means.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_657_mapbox_earcut.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_657_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_658_bevel_tools.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_658_bevel_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_659_intersection_line_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_662_is_convex_polygon_2d.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_662_is_convex_polygon_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_663_is_axes_aligned_rectange.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_663_is_axes_aligned_rectange.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_664_concave_clipping_polygon.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_664_concave_clipping_polygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_665_inverted_clipping_polygon.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_665_inverted_clipping_polygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_06_math/test_666_wgs84_transform.py` & `ezdxf-1.3.0rc0/tests/test_06_math/test_666_wgs84_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_701_arrows.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_701_arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_702_render_forms.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_702_render_forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_703_mesh_builder.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_703_mesh_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_704_render_linear_dimension.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_704_render_linear_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_705_shape.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_705_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_707_trace.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_707_trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_708a_path.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_708a_path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_708b_path_tools.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_708b_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_708c_matplotlib_path_tools.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_708c_matplotlib_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_708d_qpainter_path_tools.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_708d_qpainter_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_708e_path_shapes.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_708e_path_shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_708f_path_nesting.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_708f_path_nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_709_linetype_renderer.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_709_linetype_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_711_points.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_711_points.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_712_render_curved_dimension.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_712_render_curved_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_713_mleader_builder.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_713_mleader_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_714_mleader_render_engine.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_714_mleader_render_engine.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_715_hatching.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_715_hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py` & `ezdxf-1.3.0rc0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_800_mtext_surrogate.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_800_mtext_surrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_801_r12spline.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_801_r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_802_table_painter.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_802_table_painter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_803_entities_to_code.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_803_entities_to_code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_804_importer.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_804_importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_805_pycsg.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_805_pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_806_acadctb.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_806_acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_807_dwg_loader_basics.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_807_dwg_loader_basics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_810_drawing_properties.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_810_drawing_properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_811a_drawing_frontend.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_811a_drawing_frontend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_811b_drawing_recorder.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_811b_drawing_recorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_811c_viewport_processing.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_811c_viewport_processing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_812_drawing_graphic_proxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_813_geo_interface.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_813_geo_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_814_text2path.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_814_text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_815_dxf_browser.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_815_dxf_browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_816_bin_packing.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_816_bin_packing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_817_genetic_algorithm.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_817_genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_818_meshex.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_818_meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_819_menger_sponge.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_819_menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_820_openscad.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_820_openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_821_hpgl2.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_821_hpgl2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_823_drawing_layout.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_823_drawing_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_824_svg_drawing_backend.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_824_svg_drawing_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_825_hpgl2_drawing_backend.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_825_hpgl2_drawing_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_826_custom_json_backend.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_826_custom_json_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_08_addons/test_827_geojson_backend.py` & `ezdxf-1.3.0rc0/tests/test_08_addons/test_827_geojson_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py` & `ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_901_acc_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py` & `ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_902_acc_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py` & `ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py` & `ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py` & `ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py` & `ezdxf-1.3.0rc0/tests/test_09_cython_acceleration/test_906_acc_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_10_issues/test_issue_414_bbox_calculation.py` & `ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_414_bbox_calculation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py` & `ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_10_issues/test_issue_574_flattening_error.py` & `ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_574_flattening_error.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py` & `ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_10_issues/test_issue_749_text_layout.py` & `ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_749_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.3.0b1/tests/test_10_issues/test_issue_873_circle_inverted_normal.py` & `ezdxf-1.3.0rc0/tests/test_10_issues/test_issue_873_circle_inverted_normal.py`

 * *Files identical despite different names*

