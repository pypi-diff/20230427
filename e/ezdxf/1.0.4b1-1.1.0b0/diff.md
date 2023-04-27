# Comparing `tmp/ezdxf-1.0.4b1.zip` & `tmp/ezdxf-1.1.0b0.zip`

## zipinfo {}

```diff
@@ -1,821 +1,821 @@
-Zip file size: 2070357 bytes, number of entries: 819
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/integration_tests/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/
--rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/LICENSE
--rw-rw-rw-  2.0 fat      302 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/MANIFEST.in
--rw-rw-rw-  2.0 fat    99978 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/NEWS.md
--rw-rw-rw-  2.0 fat    67799 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/PKG-INFO
--rw-rw-rw-  2.0 fat     6045 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/README.md
--rw-rw-rw-  2.0 fat       37 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/requirements.txt
--rw-rw-rw-  2.0 fat       74 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/setup.cfg
--rw-rw-rw-  2.0 fat     5563 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/integration_tests/data/
--rw-rw-rw-  2.0 fat      567 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/check_disable_c_ext_by_config_file.py
--rw-rw-rw-  2.0 fat      541 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/check_disable_c_ext_by_env_var.py
--rw-rw-rw-  2.0 fat     1054 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_acad_table.py
--rw-rw-rw-  2.0 fat     4686 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_all_dimline_styles.py
--rw-rw-rw-  2.0 fat     4133 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_all_ellipse_transformations.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_anonymous_blocks.py
--rw-rw-rw-  2.0 fat      871 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_audit_critical_dxf_files.py
--rw-rw-rw-  2.0 fat     1603 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_audit_layouts.py
--rw-rw-rw-  2.0 fat     1726 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_complex_line_type_2.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_create_basic_graphics.py
--rw-rw-rw-  2.0 fat     1921 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_document_guid.py
--rw-rw-rw-  2.0 fat     1832 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_document_page_setup.py
--rw-rw-rw-  2.0 fat      698 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_drawing_matplotlib_backend.py
--rw-rw-rw-  2.0 fat      829 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_drawing_qt_backend.py
--rw-rw-rw-  2.0 fat      998 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_dxf_info_scanning.py
--rw-rw-rw-  2.0 fat     1558 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_entities_iterator.py
--rw-rw-rw-  2.0 fat      934 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_fix_dulicate_handles.py
--rw-rw-rw-  2.0 fat     1901 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_geo.py
--rw-rw-rw-  2.0 fat     1250 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_groups.py
--rw-rw-rw-  2.0 fat      630 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_ignore_junk_beyond_EOF.py
--rw-rw-rw-  2.0 fat     1155 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_launcher.py
--rw-rw-rw-  2.0 fat      631 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_leica_disto_r12.py
--rw-rw-rw-  2.0 fat      737 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_load_dxf_unicode_notation.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_mapbox_earcut.py
--rw-rw-rw-  2.0 fat     1062 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_matplotlib_font_support.py
--rw-rw-rw-  2.0 fat     2230 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_mtext_columns.py
--rw-rw-rw-  2.0 fat     2310 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_mtext_explode_addon.py
--rw-rw-rw-  2.0 fat     1846 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_mtext_text_frame.py
--rw-rw-rw-  2.0 fat     1053 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_new_table_entries.py
--rw-rw-rw-  2.0 fat      887 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_none_ascii_read_write.py
--rw-rw-rw-  2.0 fat     3435 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_odafc.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_open_binary_DXF_files.py
--rw-rw-rw-  2.0 fat      751 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_open_coord_order_issue.py
--rw-rw-rw-  2.0 fat     3842 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_open_exotic_dxf_files.py
--rw-rw-rw-  2.0 fat      879 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_open_R13_R14.py
--rw-rw-rw-  2.0 fat     3152 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_polyline_entity.py
--rw-rw-rw-  2.0 fat     1749 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_preserve_binary_data_in_xrecords.py
--rw-rw-rw-  2.0 fat     6892 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_r12export.py
--rw-rw-rw-  2.0 fat     6256 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_r12strict.py
--rw-rw-rw-  2.0 fat     3410 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_r12writer.py
--rw-rw-rw-  2.0 fat      567 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_read_file_without_handles.py
--rw-rw-rw-  2.0 fat     1121 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_read_write_modern_entites.py
--rw-rw-rw-  2.0 fat     5375 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_recover.py
--rw-rw-rw-  2.0 fat     1959 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_redraw_order.py
--rw-rw-rw-  2.0 fat     1819 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_rotated_block_attributes.py
--rw-rw-rw-  2.0 fat      774 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_surface_entities.py
--rw-rw-rw-  2.0 fat      928 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_write_fixed_meta_data.py
--rw-rw-rw-  2.0 fat     1806 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_write_without_handles.py
--rw-rw-rw-  2.0 fat     3638 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/test_xref_detach.py
--rw-rw-rw-  2.0 fat     3060 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/AC1003_LINE_Example.dxf
--rw-rw-rw-  2.0 fat   179505 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/acad_table_with_blk_ref.dxf
--rw-rw-rw-  2.0 fat     7956 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/ASCII_R12.dxf
--rw-rw-rw-  2.0 fat     3761 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r12.dxf
--rw-rw-rw-  2.0 fat    20914 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r13.dxf
--rw-rw-rw-  2.0 fat    21137 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r14.dxf
--rw-rw-rw-  2.0 fat    11564 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r2000.dxf
--rw-rw-rw-  2.0 fat     6424 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/cc_dxflib.dxf
--rw-rw-rw-  2.0 fat   173753 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/custom_blocks.dxf
--rw-rw-rw-  2.0 fat    32203 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/duplicate_handles.dxf
--rw-rw-rw-  2.0 fat    18554 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/dxf_unicode.dxf
--rw-rw-rw-  2.0 fat     1592 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/empty_handles.dxf
--rw-rw-rw-  2.0 fat    97103 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/groups.dxf
--rw-rw-rw-  2.0 fat     9146 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/Leica_Disto_S910.dxf
--rw-rw-rw-  2.0 fat    17986 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/MODEL.dxf
--rw-rw-rw-  2.0 fat    25799 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/mtext_columns_R2007.dxf
--rw-rw-rw-  2.0 fat    23927 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/mtext_columns_R2018.dxf
--rw-rw-rw-  2.0 fat    98230 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/mtext_framed_columns.dxf
--rw-rw-rw-  2.0 fat   106574 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/mtext_text_frame.dxf
--rw-rw-rw-  2.0 fat    12001 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/no_layouts.dxf
--rw-rw-rw-  2.0 fat    28788 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/POLI-ALL210_12.DXF
--rw-rw-rw-  2.0 fat      144 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/R12_with_trash_beyond_EOF.dxf
--rw-rw-rw-  2.0 fat   212407 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/recover01.dxf
--rw-rw-rw-  2.0 fat   115423 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/recover02.dxf
--rw-rw-rw-  2.0 fat    21178 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/small_r13.dxf
--rw-rw-rw-  2.0 fat    10326 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/small_r14.dxf
--rw-rw-rw-  2.0 fat    11286 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/XRECORD_0.bin
--rw-rw-rw-  2.0 fat    11662 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/XRECORD_1.bin
--rw-rw-rw-  2.0 fat    15337 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/integration_tests/data/XRECORD_2.bin
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/acc/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/acis/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/lldxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/path/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/pp/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/resources/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/sections/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/tools/
--rw-rw-rw-  2.0 fat     4710 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/appsettings.py
--rw-rw-rw-  2.0 fat    19818 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/audit.py
--rw-rw-rw-  2.0 fat     5912 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/bbox.py
--rw-rw-rw-  2.0 fat     7888 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/blkrefs.py
--rw-rw-rw-  2.0 fat    13157 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/colors.py
--rw-rw-rw-  2.0 fat    38502 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/commands.py
--rw-rw-rw-  2.0 fat     1549 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/comments.py
--rw-rw-rw-  2.0 fat    22100 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/disassemble.py
--rw-rw-rw-  2.0 fat    52604 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/document.py
--rw-rw-rw-  2.0 fat      832 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/dwginfo.py
--rw-rw-rw-  2.0 fat    16248 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entitydb.py
--rw-rw-rw-  2.0 fat     7495 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/enums.py
--rw-rw-rw-  2.0 fat    13948 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/explode.py
--rw-rw-rw-  2.0 fat     1653 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/eztypes.py
--rw-rw-rw-  2.0 fat    10289 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/filemanagement.py
--rw-rw-rw-  2.0 fat    12157 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/gfxattribs.py
--rw-rw-rw-  2.0 fat   107500 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/graphicsfactory.py
--rw-rw-rw-  2.0 fat     3416 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/groupby.py
--rw-rw-rw-  2.0 fat     2567 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/protocols.py
--rw-rw-rw-  2.0 fat    32672 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/proxygraphic.py
--rw-rw-rw-  2.0 fat       95 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/py.typed
--rw-rw-rw-  2.0 fat    22499 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/query.py
--rw-rw-rw-  2.0 fat     2780 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/queryparser.py
--rw-rw-rw-  2.0 fat     9580 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/r12strict.py
--rw-rw-rw-  2.0 fat    30769 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/recover.py
--rw-rw-rw-  2.0 fat     3515 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/reorder.py
--rw-rw-rw-  2.0 fat    30244 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/shapefile.py
--rw-rw-rw-  2.0 fat    10364 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/transform.py
--rw-rw-rw-  2.0 fat     5648 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/units.py
--rw-rw-rw-  2.0 fat     8280 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/upright.py
--rw-rw-rw-  2.0 fat     9875 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/urecord.py
--rw-rw-rw-  2.0 fat     1024 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/version.py
--rw-rw-rw-  2.0 fat    63359 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/xref.py
--rw-rw-rw-  2.0 fat     2853 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/zoom.py
--rw-rw-rw-  2.0 fat    12060 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/_options.py
--rw-rw-rw-  2.0 fat     2667 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/__init__.py
--rw-rw-rw-  2.0 fat     2781 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/__main__.py
--rw-rw-rw-  2.0 fat     6072 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/bezier3p.pyx
--rw-rw-rw-  2.0 fat     9983 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/bezier4p.pyx
--rw-rw-rw-  2.0 fat    12964 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/bspline.pyx
--rw-rw-rw-  2.0 fat       90 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/construct.pxd
--rw-rw-rw-  2.0 fat     6584 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/construct.pyx
--rw-rw-rw-  2.0 fat     3113 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/linetypes.pyx
--rw-rw-rw-  2.0 fat    23989 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/mapbox_earcut.pyx
--rw-rw-rw-  2.0 fat      381 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/matrix44.pxd
--rw-rw-rw-  2.0 fat    20892 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/matrix44.pyx
--rw-rw-rw-  2.0 fat     2014 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/vector.pxd
--rw-rw-rw-  2.0 fat    23705 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/vector.pyx
--rw-rw-rw-  2.0 fat     1784 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.cpp
--rw-rw-rw-  2.0 fat      599 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.hpp
--rw-rw-rw-  2.0 fat      424 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.pxd
--rw-rw-rw-  2.0 fat      960 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.cpp
--rw-rw-rw-  2.0 fat      464 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.hpp
--rw-rw-rw-  2.0 fat      407 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.pxd
--rw-rw-rw-  2.0 fat     2135 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_vec3.hpp
--rw-rw-rw-  2.0 fat      572 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_vec3.pxd
--rw-rw-rw-  2.0 fat     1265 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acc/__init__.py
--rw-rw-rw-  2.0 fat     6393 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/abstract.py
--rw-rw-rw-  2.0 fat      884 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/api.py
--rw-rw-rw-  2.0 fat     5484 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/const.py
--rw-rw-rw-  2.0 fat     6726 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/dbg.py
--rw-rw-rw-  2.0 fat     2980 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/dxf.py
--rw-rw-rw-  2.0 fat    28991 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/entities.py
--rw-rw-rw-  2.0 fat     4088 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/hdr.py
--rw-rw-rw-  2.0 fat    12823 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/mesh.py
--rw-rw-rw-  2.0 fat    18690 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/sab.py
--rw-rw-rw-  2.0 fat    13184 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/sat.py
--rw-rw-rw-  2.0 fat      115 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/acis/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/addons/browser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/
--rw-rw-rw-  2.0 fat    26402 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/acadctb.py
--rw-rw-rw-  2.0 fat    22229 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/binpacking.py
--rw-rw-rw-  2.0 fat    27692 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dimlines.py
--rw-rw-rw-  2.0 fat    31371 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dxf2code.py
--rw-rw-rw-  2.0 fat    22037 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/genetic_algorithm.py
--rw-rw-rw-  2.0 fat    36445 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/geo.py
--rw-rw-rw-  2.0 fat     2674 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/gerber_D6673.py
--rw-rw-rw-  2.0 fat    25472 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/importer.py
--rw-rw-rw-  2.0 fat    17355 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/iterdxf.py
--rw-rw-rw-  2.0 fat     8940 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/menger_sponge.py
--rw-rw-rw-  2.0 fat    24787 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/meshex.py
--rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/mixins.py
--rw-rw-rw-  2.0 fat     6203 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/mtextsurrogate.py
--rw-rw-rw-  2.0 fat    13494 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/mtxpl.py
--rw-rw-rw-  2.0 fat    16400 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/odafc.py
--rw-rw-rw-  2.0 fat     9456 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/openscad.py
--rw-rw-rw-  2.0 fat    15878 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/pycsg.py
--rw-rw-rw-  2.0 fat    22496 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/r12export.py
--rw-rw-rw-  2.0 fat    27198 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/r12writer.py
--rw-rw-rw-  2.0 fat     7615 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/sierpinski_pyramid.py
--rw-rw-rw-  2.0 fat    33167 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/tablepainter.py
--rw-rw-rw-  2.0 fat    13174 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/text2path.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/xqt.py
--rw-rw-rw-  2.0 fat      453 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/__init__.py
--rw-rw-rw-  2.0 fat    10023 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/browser.py
--rw-rw-rw-  2.0 fat     1907 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/data.py
--rw-rw-rw-  2.0 fat       64 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/__init__.py
--rw-rw-rw-  2.0 fat      820 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/bookmarks.py
--rw-rw-rw-  2.0 fat    29403 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/browser.py
--rw-rw-rw-  2.0 fat    14891 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/data.py
--rw-rw-rw-  2.0 fat    10993 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/find_dialog.py
--rw-rw-rw-  2.0 fat     1281 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/loader.py
--rw-rw-rw-  2.0 fat    20974 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/model.py
--rw-rw-rw-  2.0 fat     2214 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/tags.py
--rw-rw-rw-  2.0 fat     1382 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/views.py
--rw-rw-rw-  2.0 fat      133 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/browser/__init__.py
--rw-rw-rw-  2.0 fat     9960 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/backend.py
--rw-rw-rw-  2.0 fat     6737 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/config.py
--rw-rw-rw-  2.0 fat     2058 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/debug_backend.py
--rw-rw-rw-  2.0 fat      503 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/debug_utils.py
--rw-rw-rw-  2.0 fat    39832 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/frontend.py
--rw-rw-rw-  2.0 fat     1823 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/gfxproxy.py
--rw-rw-rw-  2.0 fat    15999 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/matplotlib.py
--rw-rw-rw-  2.0 fat     5477 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/mpl_text_renderer.py
--rw-rw-rw-  2.0 fat     9840 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/mtext_complex.py
--rw-rw-rw-  2.0 fat    14024 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/pillow.py
--rw-rw-rw-  2.0 fat    38021 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/properties.py
--rw-rw-rw-  2.0 fat    13449 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/pyqt.py
--rw-rw-rw-  2.0 fat    16757 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/qtviewer.py
--rw-rw-rw-  2.0 fat     5119 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/qt_text_renderer.py
--rw-rw-rw-  2.0 fat    13658 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/text.py
--rw-rw-rw-  2.0 fat     1132 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/text_renderer.py
--rw-rw-rw-  2.0 fat      344 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/type_hints.py
--rw-rw-rw-  2.0 fat      171 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/drawing/__init__.py
--rw-rw-rw-  2.0 fat     3112 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/classes_section.py
--rw-rw-rw-  2.0 fat      763 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/const.py
--rw-rw-rw-  2.0 fat     6091 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/crc.py
--rw-rw-rw-  2.0 fat     3160 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/fileheader.py
--rw-rw-rw-  2.0 fat    14851 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/header_section.py
--rw-rw-rw-  2.0 fat     2976 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/loader.py
--rw-rw-rw-  2.0 fat      141 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/dwg/__init__.py
--rw-rw-rw-  2.0 fat     5227 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/api.py
--rw-rw-rw-  2.0 fat     4863 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/backend.py
--rw-rw-rw-  2.0 fat      513 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/compiler.py
--rw-rw-rw-  2.0 fat      571 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/deps.py
--rw-rw-rw-  2.0 fat     3658 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/dxf_backend.py
--rw-rw-rw-  2.0 fat    14520 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/interpreter.py
--rw-rw-rw-  2.0 fat     4835 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/page.py
--rw-rw-rw-  2.0 fat     3130 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/pdf_backend.py
--rw-rw-rw-  2.0 fat    11435 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/plotter.py
--rw-rw-rw-  2.0 fat     1411 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/polygon_buffer.py
--rw-rw-rw-  2.0 fat     4442 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/properties.py
--rw-rw-rw-  2.0 fat     3349 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/svg_backend.py
--rw-rw-rw-  2.0 fat     5291 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/tokenizer.py
--rw-rw-rw-  2.0 fat      164 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/__init__.py
--rw-rw-rw-  2.0 fat     4757 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/acad_proxy_entity.py
--rw-rw-rw-  2.0 fat    18315 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/acad_table.py
--rw-rw-rw-  2.0 fat    25923 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/acis.py
--rw-rw-rw-  2.0 fat     4890 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/appdata.py
--rw-rw-rw-  2.0 fat     1954 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/appid.py
--rw-rw-rw-  2.0 fat     4942 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/arc.py
--rw-rw-rw-  2.0 fat    26138 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/attrib.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/block.py
--rw-rw-rw-  2.0 fat    10536 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/blockrecord.py
--rw-rw-rw-  2.0 fat    50143 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/boundary_paths.py
--rw-rw-rw-  2.0 fat     7961 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/circle.py
--rw-rw-rw-  2.0 fat    23664 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dictionary.py
--rw-rw-rw-  2.0 fat    48743 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dimension.py
--rw-rw-rw-  2.0 fat    35012 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dimstyle.py
--rw-rw-rw-  2.0 fat    23829 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dimstyleoverride.py
--rw-rw-rw-  2.0 fat     4399 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dxfclass.py
--rw-rw-rw-  2.0 fat    42404 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dxfentity.py
--rw-rw-rw-  2.0 fat    26923 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dxfgfx.py
--rw-rw-rw-  2.0 fat    15279 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dxfgroups.py
--rw-rw-rw-  2.0 fat    23699 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dxfns.py
--rw-rw-rw-  2.0 fat    13746 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/dxfobj.py
--rw-rw-rw-  2.0 fat    11186 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/ellipse.py
--rw-rw-rw-  2.0 fat     4170 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/factory.py
--rw-rw-rw-  2.0 fat    23785 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/geodata.py
--rw-rw-rw-  2.0 fat     4020 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/gradient.py
--rw-rw-rw-  2.0 fat    12263 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/hatch.py
--rw-rw-rw-  2.0 fat     3944 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/helix.py
--rw-rw-rw-  2.0 fat     4747 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/idbuffer.py
--rw-rw-rw-  2.0 fat    26057 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/image.py
--rw-rw-rw-  2.0 fat    27932 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/insert.py
--rw-rw-rw-  2.0 fat    27834 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/layer.py
--rw-rw-rw-  2.0 fat    14252 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/layout.py
--rw-rw-rw-  2.0 fat    12978 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/leader.py
--rw-rw-rw-  2.0 fat     4718 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/light.py
--rw-rw-rw-  2.0 fat     3718 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/line.py
--rw-rw-rw-  2.0 fat     9677 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/ltype.py
--rw-rw-rw-  2.0 fat    18878 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/lwpolyline.py
--rw-rw-rw-  2.0 fat    19653 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/material.py
--rw-rw-rw-  2.0 fat    18435 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/mesh.py
--rw-rw-rw-  2.0 fat    57367 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/mleader.py
--rw-rw-rw-  2.0 fat    37144 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/mline.py
--rw-rw-rw-  2.0 fat     8385 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/mpolygon.py
--rw-rw-rw-  2.0 fat    48153 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/mtext.py
--rw-rw-rw-  2.0 fat     4351 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/mtext_columns.py
--rw-rw-rw-  2.0 fat     6284 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/objectcollection.py
--rw-rw-rw-  2.0 fat     2111 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/oleframe.py
--rw-rw-rw-  2.0 fat     4332 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/pattern.py
--rw-rw-rw-  2.0 fat     5238 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/point.py
--rw-rw-rw-  2.0 fat    16416 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/polygon.py
--rw-rw-rw-  2.0 fat    40087 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/polyline.py
--rw-rw-rw-  2.0 fat     4822 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/shape.py
--rw-rw-rw-  2.0 fat    10443 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/solid.py
--rw-rw-rw-  2.0 fat    24085 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/spline.py
--rw-rw-rw-  2.0 fat     8246 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/subentity.py
--rw-rw-rw-  2.0 fat     5196 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/sun.py
--rw-rw-rw-  2.0 fat     2449 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/table.py
--rw-rw-rw-  2.0 fat    17602 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/text.py
--rw-rw-rw-  2.0 fat     9105 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/textstyle.py
--rw-rw-rw-  2.0 fat     3597 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/tolerance.py
--rw-rw-rw-  2.0 fat     2703 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/ucs.py
--rw-rw-rw-  2.0 fat    14366 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/underlay.py
--rw-rw-rw-  2.0 fat     6040 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/view.py
--rw-rw-rw-  2.0 fat    27893 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/viewport.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/visualstyle.py
--rw-rw-rw-  2.0 fat     9970 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/vport.py
--rw-rw-rw-  2.0 fat    17024 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/xdata.py
--rw-rw-rw-  2.0 fat     8495 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/xdict.py
--rw-rw-rw-  2.0 fat     3062 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/xline.py
--rw-rw-rw-  2.0 fat     3127 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/entities/__init__.py
--rw-rw-rw-  2.0 fat    16696 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/layouts/base.py
--rw-rw-rw-  2.0 fat     4343 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/layouts/blocklayout.py
--rw-rw-rw-  2.0 fat    29014 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/layouts/layout.py
--rw-rw-rw-  2.0 fat    15314 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/layouts/layouts.py
--rw-rw-rw-  2.0 fat      232 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/layouts/__init__.py
--rw-rw-rw-  2.0 fat     8327 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/attributes.py
--rw-rw-rw-  2.0 fat    16500 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/const.py
--rw-rw-rw-  2.0 fat     1614 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/encoding.py
--rw-rw-rw-  2.0 fat    17013 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/extendedtags.py
--rw-rw-rw-  2.0 fat     5363 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/fileindex.py
--rw-rw-rw-  2.0 fat      727 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/hdrvars.py
--rw-rw-rw-  2.0 fat     5469 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/loader.py
--rw-rw-rw-  2.0 fat     7447 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/packedtags.py
--rw-rw-rw-  2.0 fat     6355 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/repair.py
--rw-rw-rw-  2.0 fat    13058 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/tagger.py
--rw-rw-rw-  2.0 fat    14336 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/tags.py
--rw-rw-rw-  2.0 fat     8952 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/tagwriter.py
--rw-rw-rw-  2.0 fat    12064 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/types.py
--rw-rw-rw-  2.0 fat    17069 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/validator.py
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/lldxf/__init__.py
--rw-rw-rw-  2.0 fat    19193 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/arc.py
--rw-rw-rw-  2.0 fat    16270 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/bbox.py
--rw-rw-rw-  2.0 fat     9318 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/bezier.py
--rw-rw-rw-  2.0 fat     2452 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/bezier_interpolation.py
--rw-rw-rw-  2.0 fat     8730 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/box.py
--rw-rw-rw-  2.0 fat    53488 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/bspline.py
--rw-rw-rw-  2.0 fat     5608 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/bulge.py
--rw-rw-rw-  2.0 fat     9002 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/circle.py
--rw-rw-rw-  2.0 fat    24003 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/clipping.py
--rw-rw-rw-  2.0 fat     4319 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/clustering.py
--rw-rw-rw-  2.0 fat    12236 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/construct2d.py
--rw-rw-rw-  2.0 fat    26265 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/construct3d.py
--rw-rw-rw-  2.0 fat     1283 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/cspline.py
--rw-rw-rw-  2.0 fat     9114 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/curvetools.py
--rw-rw-rw-  2.0 fat    22048 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/ellipse.py
--rw-rw-rw-  2.0 fat     4406 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/eulerspiral.py
--rw-rw-rw-  2.0 fat    38883 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/linalg.py
--rw-rw-rw-  2.0 fat    10231 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/line.py
--rw-rw-rw-  2.0 fat     3053 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/offset2d.py
--rw-rw-rw-  2.0 fat     8256 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/parametrize.py
--rw-rw-rw-  2.0 fat    15602 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/perlin.py
--rw-rw-rw-  2.0 fat    15921 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/polyline.py
--rw-rw-rw-  2.0 fat    11867 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/rtree.py
--rw-rw-rw-  2.0 fat     3910 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/shape.py
--rw-rw-rw-  2.0 fat     2568 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/surfaces.py
--rw-rw-rw-  2.0 fat    12155 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/transformtools.py
--rw-rw-rw-  2.0 fat     3631 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/triangulation.py
--rw-rw-rw-  2.0 fat    16971 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/ucs.py
--rw-rw-rw-  2.0 fat     7253 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_bezier3p.py
--rw-rw-rw-  2.0 fat    12957 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_bezier4p.py
--rw-rw-rw-  2.0 fat     9440 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_bspline.py
--rw-rw-rw-  2.0 fat     7272 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_construct.py
--rw-rw-rw-  2.0 fat     2261 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_ctypes.py
--rw-rw-rw-  2.0 fat    24954 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    24783 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_matrix44.py
--rw-rw-rw-  2.0 fat    25912 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/_vector.py
--rw-rw-rw-  2.0 fat     2003 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/math/__init__.py
--rw-rw-rw-  2.0 fat     1229 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/commands.py
--rw-rw-rw-  2.0 fat    38526 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/converter.py
--rw-rw-rw-  2.0 fat     6663 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/nesting.py
--rw-rw-rw-  2.0 fat    16984 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/path.py
--rw-rw-rw-  2.0 fat    10140 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/shapes.py
--rw-rw-rw-  2.0 fat    34069 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/tools.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/path/__init__.py
--rw-rw-rw-  2.0 fat     2987 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.css
--rw-rw-rw-  2.0 fat     1148 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.html
--rw-rw-rw-  2.0 fat    11304 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.js
--rw-rw-rw-  2.0 fat    17144 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.py
--rw-rw-rw-  2.0 fat     3770 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/pprint.py
--rw-rw-rw-  2.0 fat      812 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.css
--rw-rw-rw-  2.0 fat      316 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.html
--rw-rw-rw-  2.0 fat     2545 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.py
--rw-rw-rw-  2.0 fat     6896 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/reflinks.py
--rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/pp/__init__.py
--rw-rw-rw-  2.0 fat    10070 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/abstract_mtext_renderer.py
--rw-rw-rw-  2.0 fat    20495 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/arrows.py
--rw-rw-rw-  2.0 fat    17749 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/curves.py
--rw-rw-rw-  2.0 fat     4041 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dimension.py
--rw-rw-rw-  2.0 fat    52028 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dim_base.py
--rw-rw-rw-  2.0 fat    35702 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dim_curved.py
--rw-rw-rw-  2.0 fat     6894 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dim_diameter.py
--rw-rw-rw-  2.0 fat    24751 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dim_linear.py
--rw-rw-rw-  2.0 fat     8084 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dim_ordinate.py
--rw-rw-rw-  2.0 fat    20295 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/dim_radius.py
--rw-rw-rw-  2.0 fat    47170 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/forms.py
--rw-rw-rw-  2.0 fat    24198 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/hatching.py
--rw-rw-rw-  2.0 fat     4728 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/leader.py
--rw-rw-rw-  2.0 fat      664 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/linetypes.py
--rw-rw-rw-  2.0 fat    64121 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/mesh.py
--rw-rw-rw-  2.0 fat    60923 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/mleader.py
--rw-rw-rw-  2.0 fat     8437 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/mline.py
--rw-rw-rw-  2.0 fat     2964 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/point.py
--rw-rw-rw-  2.0 fat     8736 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/polyline.py
--rw-rw-rw-  2.0 fat     7886 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/r12spline.py
--rw-rw-rw-  2.0 fat    22541 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/trace.py
--rw-rw-rw-  2.0 fat     2881 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/_linetypes.py
--rw-rw-rw-  2.0 fat      778 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/render/__init__.py
--rw-rw-rw-  2.0 fat     1050 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/16x16.png
--rw-rw-rw-  2.0 fat     1420 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/24x24.png
--rw-rw-rw-  2.0 fat    10638 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/256x256.png
--rw-rw-rw-  2.0 fat     1758 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/32x32.png
--rw-rw-rw-  2.0 fat     2335 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/48x48.png
--rw-rw-rw-  2.0 fat     3050 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/64x64.png
--rw-rw-rw-  2.0 fat     2090 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-copy-64px.png
--rw-rw-rw-  2.0 fat     3109 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-find-64px.png
--rw-rw-rw-  2.0 fat     2388 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-bookmark-64px.png
--rw-rw-rw-  2.0 fat     2519 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-handle-64px.png
--rw-rw-rw-  2.0 fat     2409 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-line-64px.png
--rw-rw-rw-  2.0 fat     2231 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-left-arrow-64px.png
--rw-rw-rw-  2.0 fat     2322 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-next-entity-64px.png
--rw-rw-rw-  2.0 fat     2320 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-prev-entity-64px.png
--rw-rw-rw-  2.0 fat     2244 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-right-arrow-64px.png
--rw-rw-rw-  2.0 fat     2553 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-show-in-tree-64px.png
--rw-rw-rw-  2.0 fat     2373 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/resources/icon-store-bookmark-64px.png
--rw-rw-rw-  2.0 fat    10650 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/acdsdata.py
--rw-rw-rw-  2.0 fat    16508 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/blocks.py
--rw-rw-rw-  2.0 fat    11639 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/classes.py
--rw-rw-rw-  2.0 fat     4137 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/entities.py
--rw-rw-rw-  2.0 fat    11953 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/header.py
--rw-rw-rw-  2.0 fat    60696 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/headervars.py
--rw-rw-rw-  2.0 fat    27009 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/objects.py
--rw-rw-rw-  2.0 fat    26581 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/table.py
--rw-rw-rw-  2.0 fat     5270 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/tables.py
--rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/sections/__init__.py
--rw-rw-rw-  2.0 fat    19711 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/analyze.py
--rw-rw-rw-  2.0 fat    20434 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/binarydata.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/codepage.py
--rw-rw-rw-  2.0 fat     7645 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/complex_ltype.py
--rw-rw-rw-  2.0 fat     1782 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/crypt.py
--rw-rw-rw-  2.0 fat     1511 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/debug.py
--rw-rw-rw-  2.0 fat     2341 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/difftags.py
--rw-rw-rw-  2.0 fat    19686 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/fonts.py
--rw-rw-rw-  2.0 fat    59833 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/font_face_cache.json
--rw-rw-rw-  2.0 fat    75485 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/font_measurement_cache.json
--rw-rw-rw-  2.0 fat     1235 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/handle.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/indexing.py
--rw-rw-rw-  2.0 fat     2145 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/juliandate.py
--rw-rw-rw-  2.0 fat     6166 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/pattern.py
--rw-rw-rw-  2.0 fat     1256 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/rawloader.py
--rw-rw-rw-  2.0 fat   129174 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/standards.py
--rw-rw-rw-  2.0 fat     6049 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/strip.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/test.py
--rw-rw-rw-  2.0 fat    65395 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/text.py
--rw-rw-rw-  2.0 fat    54234 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/text_layout.py
--rw-rw-rw-  2.0 fat     6916 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/text_size.py
--rw-rw-rw-  2.0 fat     3077 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/zipmanager.py
--rw-rw-rw-  2.0 fat   142734 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/_iso_pattern.py
--rw-rw-rw-  2.0 fat     4232 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/_matplotlib_font_support.py
--rw-rw-rw-  2.0 fat     3564 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/src/ezdxf/tools/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       47 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/entry_points.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat    67799 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      342 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/requires.txt
--rw-rw-rw-  2.0 fat    31202 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-15 08:42 ezdxf-1.0.4b1/src/ezdxf.egg-info/top_level.txt
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_01_dxf_entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_05_tools/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_06_math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_07_render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_08_addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/
-drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-15 08:42 ezdxf-1.0.4b1/tests/test_10_issues/
--rw-rw-rw-  2.0 fat     2336 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
--rw-rw-rw-  2.0 fat     2599 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
--rw-rw-rw-  2.0 fat     1124 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
--rw-rw-rw-  2.0 fat     5456 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
--rw-rw-rw-  2.0 fat      582 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
--rw-rw-rw-  2.0 fat      473 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_011_codepage.py
--rw-rw-rw-  2.0 fat    11593 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py
--rw-rw-rw-  2.0 fat     1191 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
--rw-rw-rw-  2.0 fat     1033 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
--rw-rw-rw-  2.0 fat     4792 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
--rw-rw-rw-  2.0 fat      989 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py
--rw-rw-rw-  2.0 fat     1383 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_018_handle.py
--rw-rw-rw-  2.0 fat     5518 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
--rw-rw-rw-  2.0 fat     8168 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
--rw-rw-rw-  2.0 fat     3787 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
--rw-rw-rw-  2.0 fat      401 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
--rw-rw-rw-  2.0 fat      539 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
--rw-rw-rw-  2.0 fat     2092 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_040_tags.py
--rw-rw-rw-  2.0 fat     3073 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
--rw-rw-rw-  2.0 fat     6419 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
--rw-rw-rw-  2.0 fat     1632 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
--rw-rw-rw-  2.0 fat    11265 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
--rw-rw-rw-  2.0 fat     3363 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
--rw-rw-rw-  2.0 fat     1974 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
--rw-rw-rw-  2.0 fat     2321 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
--rw-rw-rw-  2.0 fat      568 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
--rw-rw-rw-  2.0 fat     8682 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
--rw-rw-rw-  2.0 fat     1051 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
--rw-rw-rw-  2.0 fat     1500 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
--rw-rw-rw-  2.0 fat    11689 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py
--rw-rw-rw-  2.0 fat     2893 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_102_appdata.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_103_reactors.py
--rw-rw-rw-  2.0 fat     4001 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_104_extension_dict.py
--rw-rw-rw-  2.0 fat    20860 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_105_xdata.py
--rw-rw-rw-  2.0 fat    14169 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_110_dxfentity.py
--rw-rw-rw-  2.0 fat     2433 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
--rw-rw-rw-  2.0 fat     6781 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py
--rw-rw-rw-  2.0 fat      695 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_112b_dxfobj.py
--rw-rw-rw-  2.0 fat     2431 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_113_dxfclass.py
--rw-rw-rw-  2.0 fat     4044 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_114_factory.py
--rw-rw-rw-  2.0 fat     2256 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
--rw-rw-rw-  2.0 fat    15794 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_116_dictionary.py
--rw-rw-rw-  2.0 fat     4999 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_118_appid_table_entry.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
--rw-rw-rw-  2.0 fat     3003 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_120_style_table_entry.py
--rw-rw-rw-  2.0 fat     2943 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
--rw-rw-rw-  2.0 fat      379 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_122_vport_table_entry.py
--rw-rw-rw-  2.0 fat     1113 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_123_view_table_entry.py
--rw-rw-rw-  2.0 fat     8757 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
--rw-rw-rw-  2.0 fat     1698 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_125_image_def.py
--rw-rw-rw-  2.0 fat     1312 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py
--rw-rw-rw-  2.0 fat     1430 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_127_raster_variables.py
--rw-rw-rw-  2.0 fat     1540 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_128_pdf_definition.py
--rw-rw-rw-  2.0 fat     2778 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_129_xrecord.py
--rw-rw-rw-  2.0 fat     2423 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_130_id_buffer.py
--rw-rw-rw-  2.0 fat     2470 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_131_field_list.py
--rw-rw-rw-  2.0 fat     2435 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_132_layer_filter.py
--rw-rw-rw-  2.0 fat     2153 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_133_sun.py
--rw-rw-rw-  2.0 fat      852 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_134_material.py
--rw-rw-rw-  2.0 fat    11497 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_135_geo_data.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_136_vba_project.py
--rw-rw-rw-  2.0 fat     3099 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_137_sortentstable.py
--rw-rw-rw-  2.0 fat      704 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
--rw-rw-rw-  2.0 fat     7570 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_139_user_record.py
--rw-rw-rw-  2.0 fat      714 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_140_block_record.py
--rw-rw-rw-  2.0 fat     9153 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py
--rw-rw-rw-  2.0 fat     2231 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/conftest.py
--rw-rw-rw-  2.0 fat     6532 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_200_line.py
--rw-rw-rw-  2.0 fat     4273 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_201_point.py
--rw-rw-rw-  2.0 fat     6827 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_202_circle.py
--rw-rw-rw-  2.0 fat     8949 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_203_arc.py
--rw-rw-rw-  2.0 fat     2852 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_204_shape.py
--rw-rw-rw-  2.0 fat     8242 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_205_solid.py
--rw-rw-rw-  2.0 fat     8476 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_206_text.py
--rw-rw-rw-  2.0 fat     4947 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_207_attdef.py
--rw-rw-rw-  2.0 fat     6312 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_208_attrib.py
--rw-rw-rw-  2.0 fat     2671 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_209_vertex.py
--rw-rw-rw-  2.0 fat     5930 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_1.py
--rw-rw-rw-  2.0 fat    13489 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_2.py
--rw-rw-rw-  2.0 fat     6650 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py
--rw-rw-rw-  2.0 fat     1780 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
--rw-rw-rw-  2.0 fat     7847 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_211_viewport.py
--rw-rw-rw-  2.0 fat    12629 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_212_insert.py
--rw-rw-rw-  2.0 fat     6024 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_213_minsert.py
--rw-rw-rw-  2.0 fat     3284 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_214_block.py
--rw-rw-rw-  2.0 fat     6882 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_215_dimension.py
--rw-rw-rw-  2.0 fat     4907 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
--rw-rw-rw-  2.0 fat    13186 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
--rw-rw-rw-  2.0 fat     6471 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
--rw-rw-rw-  2.0 fat     5535 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
--rw-rw-rw-  2.0 fat     3056 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
--rw-rw-rw-  2.0 fat     7181 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
--rw-rw-rw-  2.0 fat     2066 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
--rw-rw-rw-  2.0 fat     3615 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
--rw-rw-rw-  2.0 fat     6919 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_221_ellipse.py
--rw-rw-rw-  2.0 fat     2223 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_222_xline.py
--rw-rw-rw-  2.0 fat     1493 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_223_ray.py
--rw-rw-rw-  2.0 fat     2176 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_224_group.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_225_mtext.py
--rw-rw-rw-  2.0 fat    12020 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_226_spline.py
--rw-rw-rw-  2.0 fat     5529 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
--rw-rw-rw-  2.0 fat    10893 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
--rw-rw-rw-  2.0 fat    15116 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_228_mesh.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
--rw-rw-rw-  2.0 fat    21421 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
--rw-rw-rw-  2.0 fat     6587 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
--rw-rw-rw-  2.0 fat     3140 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
--rw-rw-rw-  2.0 fat    12486 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
--rw-rw-rw-  2.0 fat     2274 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_231_underlay.py
--rw-rw-rw-  2.0 fat     5243 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_231_underlay_2.py
--rw-rw-rw-  2.0 fat     2294 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_acis.py
--rw-rw-rw-  2.0 fat     6799 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_acis_2.py
--rw-rw-rw-  2.0 fat     1854 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_surface.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_233_helix.py
--rw-rw-rw-  2.0 fat     2040 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_234_light.py
--rw-rw-rw-  2.0 fat     3806 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_235_leader.py
--rw-rw-rw-  2.0 fat    20392 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_236_multileader.py
--rw-rw-rw-  2.0 fat    10992 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_237_mline.py
--rw-rw-rw-  2.0 fat     2356 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_238_tolerance.py
--rw-rw-rw-  2.0 fat    27392 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
--rw-rw-rw-  2.0 fat     4347 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py
--rw-rw-rw-  2.0 fat     1069 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_241_hyperlink.py
--rw-rw-rw-  2.0 fat    11313 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_242_random_transform.py
--rw-rw-rw-  2.0 fat     3725 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_243_replace_entity.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
--rw-rw-rw-  2.0 fat     4456 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_245_wipeout.py
--rw-rw-rw-  2.0 fat     6175 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_246_spline_audit.py
--rw-rw-rw-  2.0 fat     8165 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
--rw-rw-rw-  2.0 fat     6003 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_248_mpolygon.py
--rw-rw-rw-  2.0 fat    13682 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
--rw-rw-rw-  2.0 fat     5713 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py
--rw-rw-rw-  2.0 fat     8331 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
--rw-rw-rw-  2.0 fat     7331 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_251_upright.py
--rw-rw-rw-  2.0 fat     4795 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
--rw-rw-rw-  2.0 fat     2082 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_253_ole2frame.py
--rw-rw-rw-  2.0 fat      821 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_254_get_font_name.py
--rw-rw-rw-  2.0 fat     5149 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_300_layout.py
--rw-rw-rw-  2.0 fat     4274 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
--rw-rw-rw-  2.0 fat     5582 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_302_block_references.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py
--rw-rw-rw-  2.0 fat      913 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py
--rw-rw-rw-  2.0 fat     3279 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
--rw-rw-rw-  2.0 fat     2609 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
--rw-rw-rw-  2.0 fat     2343 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_307_groupby.py
--rw-rw-rw-  2.0 fat    17748 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_308_query.py
--rw-rw-rw-  2.0 fat     6382 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_309_query_parser.py
--rw-rw-rw-  2.0 fat     5031 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
--rw-rw-rw-  2.0 fat     5782 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py
--rw-rw-rw-  2.0 fat      647 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_313_redraw_order.py
--rw-rw-rw-  2.0 fat     6128 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py
--rw-rw-rw-  2.0 fat     2750 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py
--rw-rw-rw-  2.0 fat     5208 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
--rw-rw-rw-  2.0 fat     6795 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py
--rw-rw-rw-  2.0 fat     4981 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
--rw-rw-rw-  2.0 fat     2450 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_405_classes.py
--rw-rw-rw-  2.0 fat     9094 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
--rw-rw-rw-  2.0 fat      848 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
--rw-rw-rw-  2.0 fat     3375 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
--rw-rw-rw-  2.0 fat     1433 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
--rw-rw-rw-  2.0 fat     5736 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_410_table.py
--rw-rw-rw-  2.0 fat     6607 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
--rw-rw-rw-  2.0 fat     2246 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
--rw-rw-rw-  2.0 fat    18072 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
--rw-rw-rw-  2.0 fat     4638 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
--rw-rw-rw-  2.0 fat    12336 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
--rw-rw-rw-  2.0 fat     6509 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
--rw-rw-rw-  2.0 fat     5656 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py
--rw-rw-rw-  2.0 fat     5434 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
--rw-rw-rw-  2.0 fat      733 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
--rw-rw-rw-  2.0 fat     1240 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
--rw-rw-rw-  2.0 fat     5007 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
--rw-rw-rw-  2.0 fat      769 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
--rw-rw-rw-  2.0 fat     7289 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_424_audit.py
--rw-rw-rw-  2.0 fat     3737 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
--rw-rw-rw-  2.0 fat     2981 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
--rw-rw-rw-  2.0 fat     2416 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
--rw-rw-rw-  2.0 fat     2533 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
--rw-rw-rw-  2.0 fat   112800 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/conftest.py
--rw-rw-rw-  2.0 fat     5510 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_500_units.py
--rw-rw-rw-  2.0 fat     1052 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_501_truecolor.py
--rw-rw-rw-  2.0 fat     1021 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_502_raw_color.py
--rw-rw-rw-  2.0 fat     1695 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_503_indexing.py
--rw-rw-rw-  2.0 fat     1442 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_504_suppress_zeros.py
--rw-rw-rw-  2.0 fat      216 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_506_version.py
--rw-rw-rw-  2.0 fat      579 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_507_dxf_pretty_printer.py
--rw-rw-rw-  2.0 fat      657 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_508_read_zip.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_509_comments.py
--rw-rw-rw-  2.0 fat     1185 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_510_byte_stream.py
--rw-rw-rw-  2.0 fat     4239 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_511_bit_stream.py
--rw-rw-rw-  2.0 fat     5595 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_512_pattern.py
--rw-rw-rw-  2.0 fat     2372 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_513_reorder_entities.py
--rw-rw-rw-  2.0 fat    17710 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_514_text.py
--rw-rw-rw-  2.0 fat     5519 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_515_fonts.py
--rw-rw-rw-  2.0 fat     4002 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_516_zoom.py
--rw-rw-rw-  2.0 fat    34209 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_517_text_layout.py
--rw-rw-rw-  2.0 fat      474 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_518_header_guid.py
--rw-rw-rw-  2.0 fat     3716 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_519_mtext_editor.py
--rw-rw-rw-  2.0 fat     3205 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_520_mtext_context.py
--rw-rw-rw-  2.0 fat    24506 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_521_mtext_parser.py
--rw-rw-rw-  2.0 fat     3863 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_522_text_scanner.py
--rw-rw-rw-  2.0 fat     6202 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_523_text_size.py
--rw-rw-rw-  2.0 fat     5063 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_524_block_reference_manager.py
--rw-rw-rw-  2.0 fat      773 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_525_transparency.py
--rw-rw-rw-  2.0 fat     2133 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_526_explode.py
--rw-rw-rw-  2.0 fat    13521 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_527_gfxattribs.py
--rw-rw-rw-  2.0 fat     2748 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_528_difftags.py
--rw-rw-rw-  2.0 fat     6700 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_529_acis_sat.py
--rw-rw-rw-  2.0 fat     2062 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_530_acis_sab.py
--rw-rw-rw-  2.0 fat    12366 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_531_acis_entities.py
--rw-rw-rw-  2.0 fat     7533 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_532_acis_mesh.py
--rw-rw-rw-  2.0 fat    42518 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_533_shapefiles.py
--rw-rw-rw-  2.0 fat     1034 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_534_dwg_info.py
--rw-rw-rw-  2.0 fat    47915 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_535_xref_basic.py
--rw-rw-rw-  2.0 fat    27614 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_536_xref_conflict.py
--rw-rw-rw-  2.0 fat     6887 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_537_transform.py
--rw-rw-rw-  2.0 fat     2246 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
--rw-rw-rw-  2.0 fat     4026 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/conftest.py
--rw-rw-rw-  2.0 fat     7460 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_600_base.py
--rw-rw-rw-  2.0 fat     2098 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_601_bulge.py
--rw-rw-rw-  2.0 fat    14651 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_602_vec3.py
--rw-rw-rw-  2.0 fat     8956 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_603_vec2.py
--rw-rw-rw-  2.0 fat     2801 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_604_banded_matrix.py
--rw-rw-rw-  2.0 fat     9738 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_604_linalg.py
--rw-rw-rw-  2.0 fat    11458 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_605_matrix44.py
--rw-rw-rw-  2.0 fat     5888 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_606_convexhull.py
--rw-rw-rw-  2.0 fat     1010 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_607_perlin_noise.py
--rw-rw-rw-  2.0 fat     3833 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_608_intersection_line_line_2d.py
--rw-rw-rw-  2.0 fat     1676 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_609_point_on_line.py
--rw-rw-rw-  2.0 fat     3171 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_610_ocs.py
--rw-rw-rw-  2.0 fat     7529 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_611_ucs.py
--rw-rw-rw-  2.0 fat     1831 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_612_ucs_pass_trough.py
--rw-rw-rw-  2.0 fat     2586 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_613_point_in_poygon.py
--rw-rw-rw-  2.0 fat    10913 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_614_construct_3d.py
--rw-rw-rw-  2.0 fat      602 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_615_rytz_axis.py
--rw-rw-rw-  2.0 fat     5215 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_616_plane.py
--rw-rw-rw-  2.0 fat      772 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_617_clockwise_orientation.py
--rw-rw-rw-  2.0 fat     6384 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_618_clipping.py
--rw-rw-rw-  2.0 fat    10108 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_619_greiner_hormann.py
--rw-rw-rw-  2.0 fat     2669 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_620_knot.py
--rw-rw-rw-  2.0 fat    19780 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_621_bspline.py
--rw-rw-rw-  2.0 fat     7652 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_622_bsplineu.py
--rw-rw-rw-  2.0 fat    12197 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_623_rbspline.py
--rw-rw-rw-  2.0 fat    10809 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_624_global_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1247 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_626_local_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1967 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_627_bspline_basis.py
--rw-rw-rw-  2.0 fat    10545 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_629_bezier.py
--rw-rw-rw-  2.0 fat    10714 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_630a_bezier4p_base.py
--rw-rw-rw-  2.0 fat    10204 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_630b_bezier4p_functions.py
--rw-rw-rw-  2.0 fat     1683 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_631_euler_spiral.py
--rw-rw-rw-  2.0 fat     4021 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_632_bezier3p.py
--rw-rw-rw-  2.0 fat    19463 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_640_bbox.py
--rw-rw-rw-  2.0 fat     5393 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_641_construction_ray.py
--rw-rw-rw-  2.0 fat     3673 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_642_construction_line.py
--rw-rw-rw-  2.0 fat     9459 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_643_construction_box.py
--rw-rw-rw-  2.0 fat    10941 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_644_construction_circle.py
--rw-rw-rw-  2.0 fat    10988 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_645_construction_arc.py
--rw-rw-rw-  2.0 fat     3422 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_646_offset_vertices_2d.py
--rw-rw-rw-  2.0 fat     7672 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_647_transform_tools.py
--rw-rw-rw-  2.0 fat     8993 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_648_construction_ellipse.py
--rw-rw-rw-  2.0 fat     1991 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_649_nurbs_python_interface.py
--rw-rw-rw-  2.0 fat     4243 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_650_elliptic_arc_span.py
--rw-rw-rw-  2.0 fat     9011 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_651_construction_polyline.py
--rw-rw-rw-  2.0 fat     3168 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_652_approx_param_t.py
--rw-rw-rw-  2.0 fat     5806 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_653_polyline_intersection.py
--rw-rw-rw-  2.0 fat     5193 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_654_rtree.py
--rw-rw-rw-  2.0 fat      788 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_655_dbscan.py
--rw-rw-rw-  2.0 fat      834 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_656_k_means.py
--rw-rw-rw-  2.0 fat     4654 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_657_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    11628 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_658_bevel_tools.py
--rw-rw-rw-  2.0 fat     1875 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py
--rw-rw-rw-  2.0 fat     1428 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
--rw-rw-rw-  2.0 fat     1741 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
--rw-rw-rw-  2.0 fat     3307 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_06_math/test_662_is_convex_polygon_2d.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_701_arrows.py
--rw-rw-rw-  2.0 fat    17245 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_702_render_forms.py
--rw-rw-rw-  2.0 fat    34220 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_703_mesh_builder.py
--rw-rw-rw-  2.0 fat     3852 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_704_render_linear_dimension.py
--rw-rw-rw-  2.0 fat     1345 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_705_shape.py
--rw-rw-rw-  2.0 fat      483 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_706_random_path.py
--rw-rw-rw-  2.0 fat     5603 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_707_trace.py
--rw-rw-rw-  2.0 fat    33834 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_708a_path.py
--rw-rw-rw-  2.0 fat    27351 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_708b_path_tools.py
--rw-rw-rw-  2.0 fat     3633 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_708c_matplotlib_path_tools.py
--rw-rw-rw-  2.0 fat     4725 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_708d_qpainter_path_tools.py
--rw-rw-rw-  2.0 fat     4589 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_708e_path_shapes.py
--rw-rw-rw-  2.0 fat     4118 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_708f_path_nesting.py
--rw-rw-rw-  2.0 fat     1308 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_709_linetype_renderer.py
--rw-rw-rw-  2.0 fat     2815 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_711_points.py
--rw-rw-rw-  2.0 fat     6594 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_712_render_curved_dimension.py
--rw-rw-rw-  2.0 fat     1472 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_713_mleader_builder.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_714_mleader_render_engine.py
--rw-rw-rw-  2.0 fat    11778 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_715_hatching.py
--rw-rw-rw-  2.0 fat     2626 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
--rw-rw-rw-  2.0 fat     4771 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_800_mtext_surrogate.py
--rw-rw-rw-  2.0 fat     1352 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_801_r12spline.py
--rw-rw-rw-  2.0 fat     7881 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_802_table_painter.py
--rw-rw-rw-  2.0 fat    12386 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_803_entities_to_code.py
--rw-rw-rw-  2.0 fat     6844 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_804_importer.py
--rw-rw-rw-  2.0 fat     2362 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_805_pycsg.py
--rw-rw-rw-  2.0 fat    15467 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_806_acadctb.py
--rw-rw-rw-  2.0 fat     4860 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_807_dwg_loader_basics.py
--rw-rw-rw-  2.0 fat    10862 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_810_drawing_properties.py
--rw-rw-rw-  2.0 fat    14074 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_811_drawing_frontend.py
--rw-rw-rw-  2.0 fat     4157 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py
--rw-rw-rw-  2.0 fat    12547 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_813_geo_interface.py
--rw-rw-rw-  2.0 fat    16289 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_814_text2path.py
--rw-rw-rw-  2.0 fat    16239 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_815_dxf_browser.py
--rw-rw-rw-  2.0 fat    11275 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_816_bin_packing.py
--rw-rw-rw-  2.0 fat    12554 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_817_genetic_algorithm.py
--rw-rw-rw-  2.0 fat     9008 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_818_meshex.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_819_menger_sponge.py
--rw-rw-rw-  2.0 fat     4433 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_820_openscad.py
--rw-rw-rw-  2.0 fat    15352 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_821_hpgl2.py
--rw-rw-rw-  2.0 fat     1322 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
--rw-rw-rw-  2.0 fat     2527 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py
--rw-rw-rw-  2.0 fat     2199 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py
--rw-rw-rw-  2.0 fat     1732 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
--rw-rw-rw-  2.0 fat     3158 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
--rw-rw-rw-  2.0 fat     1452 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
--rw-rw-rw-  2.0 fat     4755 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py
--rw-rw-rw-  2.0 fat     2656 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_10_issues/test_issue_414_bbox_calculation.py
--rw-rw-rw-  2.0 fat     1213 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
--rw-rw-rw-  2.0 fat     2268 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_10_issues/test_issue_574_flattening_error.py
--rw-rw-rw-  2.0 fat     1754 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
--rw-rw-rw-  2.0 fat      682 b- defN 23-Apr-15 08:41 ezdxf-1.0.4b1/tests/test_10_issues/test_issue_749_text_layout.py
-819 files, 8621198 bytes uncompressed, 1922889 bytes compressed:  77.7%
+Zip file size: 2055057 bytes, number of entries: 819
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/LICENSE
+-rw-rw-rw-  2.0 fat      302 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/MANIFEST.in
+-rw-rw-rw-  2.0 fat   101099 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/NEWS.md
+-rw-rw-rw-  2.0 fat    68966 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/PKG-INFO
+-rw-rw-rw-  2.0 fat     6142 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/README.md
+-rw-rw-rw-  2.0 fat       55 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/requirements.txt
+-rw-rw-rw-  2.0 fat       74 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/setup.cfg
+-rw-rw-rw-  2.0 fat     5402 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/
+-rw-rw-rw-  2.0 fat      567 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/check_disable_c_ext_by_config_file.py
+-rw-rw-rw-  2.0 fat      541 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/check_disable_c_ext_by_env_var.py
+-rw-rw-rw-  2.0 fat      402 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/conftest.py
+-rw-rw-rw-  2.0 fat     1054 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_acad_table.py
+-rw-rw-rw-  2.0 fat     4686 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_all_dimline_styles.py
+-rw-rw-rw-  2.0 fat     4133 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_all_ellipse_transformations.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_anonymous_blocks.py
+-rw-rw-rw-  2.0 fat      871 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_audit_critical_dxf_files.py
+-rw-rw-rw-  2.0 fat     1603 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_audit_layouts.py
+-rw-rw-rw-  2.0 fat     1726 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_complex_line_type_2.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_create_basic_graphics.py
+-rw-rw-rw-  2.0 fat     1921 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_document_guid.py
+-rw-rw-rw-  2.0 fat     1832 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_document_page_setup.py
+-rw-rw-rw-  2.0 fat      998 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_dxf_info_scanning.py
+-rw-rw-rw-  2.0 fat     1558 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_entities_iterator.py
+-rw-rw-rw-  2.0 fat      934 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_fix_dulicate_handles.py
+-rw-rw-rw-  2.0 fat     1901 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_geo.py
+-rw-rw-rw-  2.0 fat     1250 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_groups.py
+-rw-rw-rw-  2.0 fat      630 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_ignore_junk_beyond_EOF.py
+-rw-rw-rw-  2.0 fat     1155 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_launcher.py
+-rw-rw-rw-  2.0 fat      631 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_leica_disto_r12.py
+-rw-rw-rw-  2.0 fat      737 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_load_dxf_unicode_notation.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat     2230 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_mtext_columns.py
+-rw-rw-rw-  2.0 fat     2392 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_mtext_explode_addon.py
+-rw-rw-rw-  2.0 fat     1846 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_mtext_text_frame.py
+-rw-rw-rw-  2.0 fat     1053 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_new_table_entries.py
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_none_ascii_read_write.py
+-rw-rw-rw-  2.0 fat     3435 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_odafc.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_open_binary_DXF_files.py
+-rw-rw-rw-  2.0 fat      751 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_open_coord_order_issue.py
+-rw-rw-rw-  2.0 fat     3842 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_open_exotic_dxf_files.py
+-rw-rw-rw-  2.0 fat      879 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_open_R13_R14.py
+-rw-rw-rw-  2.0 fat     3152 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_polyline_entity.py
+-rw-rw-rw-  2.0 fat     1749 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_preserve_binary_data_in_xrecords.py
+-rw-rw-rw-  2.0 fat     6944 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_r12export.py
+-rw-rw-rw-  2.0 fat     6256 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_r12strict.py
+-rw-rw-rw-  2.0 fat     3410 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_r12writer.py
+-rw-rw-rw-  2.0 fat      567 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_read_file_without_handles.py
+-rw-rw-rw-  2.0 fat     1121 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_read_write_modern_entites.py
+-rw-rw-rw-  2.0 fat     5375 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_recover.py
+-rw-rw-rw-  2.0 fat     1959 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_redraw_order.py
+-rw-rw-rw-  2.0 fat     1819 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_rotated_block_attributes.py
+-rw-rw-rw-  2.0 fat      774 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_surface_entities.py
+-rw-rw-rw-  2.0 fat      928 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_write_fixed_meta_data.py
+-rw-rw-rw-  2.0 fat     1806 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_write_without_handles.py
+-rw-rw-rw-  2.0 fat     3638 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/test_xref_detach.py
+-rw-rw-rw-  2.0 fat     3060 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/AC1003_LINE_Example.dxf
+-rw-rw-rw-  2.0 fat   179505 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/acad_table_with_blk_ref.dxf
+-rw-rw-rw-  2.0 fat     7956 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/ASCII_R12.dxf
+-rw-rw-rw-  2.0 fat     3761 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r12.dxf
+-rw-rw-rw-  2.0 fat    20914 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r13.dxf
+-rw-rw-rw-  2.0 fat    21137 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r14.dxf
+-rw-rw-rw-  2.0 fat    11564 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r2000.dxf
+-rw-rw-rw-  2.0 fat     6424 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/cc_dxflib.dxf
+-rw-rw-rw-  2.0 fat   173753 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/custom_blocks.dxf
+-rw-rw-rw-  2.0 fat    32203 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/duplicate_handles.dxf
+-rw-rw-rw-  2.0 fat    18554 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/dxf_unicode.dxf
+-rw-rw-rw-  2.0 fat     1592 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/empty_handles.dxf
+-rw-rw-rw-  2.0 fat    97103 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/groups.dxf
+-rw-rw-rw-  2.0 fat     9146 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/Leica_Disto_S910.dxf
+-rw-rw-rw-  2.0 fat    17986 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/MODEL.dxf
+-rw-rw-rw-  2.0 fat    25799 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/mtext_columns_R2007.dxf
+-rw-rw-rw-  2.0 fat    23927 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/mtext_columns_R2018.dxf
+-rw-rw-rw-  2.0 fat    98230 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/mtext_framed_columns.dxf
+-rw-rw-rw-  2.0 fat   106574 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/mtext_text_frame.dxf
+-rw-rw-rw-  2.0 fat    12001 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/no_layouts.dxf
+-rw-rw-rw-  2.0 fat    28788 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/POLI-ALL210_12.DXF
+-rw-rw-rw-  2.0 fat      144 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+-rw-rw-rw-  2.0 fat   212407 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/recover01.dxf
+-rw-rw-rw-  2.0 fat   115423 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/recover02.dxf
+-rw-rw-rw-  2.0 fat    21178 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/small_r13.dxf
+-rw-rw-rw-  2.0 fat    10326 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/small_r14.dxf
+-rw-rw-rw-  2.0 fat    11286 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/XRECORD_0.bin
+-rw-rw-rw-  2.0 fat    11662 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/XRECORD_1.bin
+-rw-rw-rw-  2.0 fat    15337 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/integration_tests/data/XRECORD_2.bin
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/
+-rw-rw-rw-  2.0 fat     4710 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/appsettings.py
+-rw-rw-rw-  2.0 fat    19818 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/audit.py
+-rw-rw-rw-  2.0 fat     5324 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/bbox.py
+-rw-rw-rw-  2.0 fat     7888 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/blkrefs.py
+-rw-rw-rw-  2.0 fat    13157 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/colors.py
+-rw-rw-rw-  2.0 fat    31737 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/commands.py
+-rw-rw-rw-  2.0 fat     1549 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/comments.py
+-rw-rw-rw-  2.0 fat    22100 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/disassemble.py
+-rw-rw-rw-  2.0 fat    52708 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/document.py
+-rw-rw-rw-  2.0 fat      832 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/dwginfo.py
+-rw-rw-rw-  2.0 fat    16248 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entitydb.py
+-rw-rw-rw-  2.0 fat     7495 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/enums.py
+-rw-rw-rw-  2.0 fat    13948 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/explode.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/eztypes.py
+-rw-rw-rw-  2.0 fat    10289 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/filemanagement.py
+-rw-rw-rw-  2.0 fat    12157 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/gfxattribs.py
+-rw-rw-rw-  2.0 fat   107500 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/graphicsfactory.py
+-rw-rw-rw-  2.0 fat     3416 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/groupby.py
+-rw-rw-rw-  2.0 fat     2942 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/npshapes.py
+-rw-rw-rw-  2.0 fat     2567 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/protocols.py
+-rw-rw-rw-  2.0 fat    32672 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/proxygraphic.py
+-rw-rw-rw-  2.0 fat       95 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/py.typed
+-rw-rw-rw-  2.0 fat    22499 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/query.py
+-rw-rw-rw-  2.0 fat     2780 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/queryparser.py
+-rw-rw-rw-  2.0 fat     9580 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/r12strict.py
+-rw-rw-rw-  2.0 fat    30769 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/recover.py
+-rw-rw-rw-  2.0 fat     3515 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/reorder.py
+-rw-rw-rw-  2.0 fat    30244 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/shapefile.py
+-rw-rw-rw-  2.0 fat    10364 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/transform.py
+-rw-rw-rw-  2.0 fat     5648 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/units.py
+-rw-rw-rw-  2.0 fat     8280 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/upright.py
+-rw-rw-rw-  2.0 fat     9875 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/urecord.py
+-rw-rw-rw-  2.0 fat     1024 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/version.py
+-rw-rw-rw-  2.0 fat    63359 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/xref.py
+-rw-rw-rw-  2.0 fat     2853 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/zoom.py
+-rw-rw-rw-  2.0 fat    11516 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/_options.py
+-rw-rw-rw-  2.0 fat     2583 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/__init__.py
+-rw-rw-rw-  2.0 fat     2781 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/__main__.py
+-rw-rw-rw-  2.0 fat     6072 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/bezier3p.pyx
+-rw-rw-rw-  2.0 fat     9983 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/bezier4p.pyx
+-rw-rw-rw-  2.0 fat    12964 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/bspline.pyx
+-rw-rw-rw-  2.0 fat       90 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/construct.pxd
+-rw-rw-rw-  2.0 fat     6584 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/construct.pyx
+-rw-rw-rw-  2.0 fat     3113 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/linetypes.pyx
+-rw-rw-rw-  2.0 fat    23989 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/mapbox_earcut.pyx
+-rw-rw-rw-  2.0 fat      381 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/matrix44.pxd
+-rw-rw-rw-  2.0 fat    21938 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/matrix44.pyx
+-rw-rw-rw-  2.0 fat     2014 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/vector.pxd
+-rw-rw-rw-  2.0 fat    23705 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/vector.pyx
+-rw-rw-rw-  2.0 fat     1784 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+-rw-rw-rw-  2.0 fat      599 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+-rw-rw-rw-  2.0 fat      424 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+-rw-rw-rw-  2.0 fat      960 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.cpp
+-rw-rw-rw-  2.0 fat      464 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.hpp
+-rw-rw-rw-  2.0 fat      407 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.pxd
+-rw-rw-rw-  2.0 fat     2135 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_vec3.hpp
+-rw-rw-rw-  2.0 fat      572 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_vec3.pxd
+-rw-rw-rw-  2.0 fat     1265 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acc/__init__.py
+-rw-rw-rw-  2.0 fat     6393 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/abstract.py
+-rw-rw-rw-  2.0 fat      884 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/api.py
+-rw-rw-rw-  2.0 fat     5484 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/const.py
+-rw-rw-rw-  2.0 fat     6726 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/dbg.py
+-rw-rw-rw-  2.0 fat     2980 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/dxf.py
+-rw-rw-rw-  2.0 fat    28991 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/entities.py
+-rw-rw-rw-  2.0 fat     4088 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/hdr.py
+-rw-rw-rw-  2.0 fat    12823 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/mesh.py
+-rw-rw-rw-  2.0 fat    18690 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/sab.py
+-rw-rw-rw-  2.0 fat    13184 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/sat.py
+-rw-rw-rw-  2.0 fat      115 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/acis/__init__.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/
+-rw-rw-rw-  2.0 fat    26415 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/acadctb.py
+-rw-rw-rw-  2.0 fat    22229 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/binpacking.py
+-rw-rw-rw-  2.0 fat    27692 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dimlines.py
+-rw-rw-rw-  2.0 fat    31371 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dxf2code.py
+-rw-rw-rw-  2.0 fat    22037 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/genetic_algorithm.py
+-rw-rw-rw-  2.0 fat    36445 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/geo.py
+-rw-rw-rw-  2.0 fat     2674 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/gerber_D6673.py
+-rw-rw-rw-  2.0 fat    25472 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/importer.py
+-rw-rw-rw-  2.0 fat    17355 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/iterdxf.py
+-rw-rw-rw-  2.0 fat     8940 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/menger_sponge.py
+-rw-rw-rw-  2.0 fat    24787 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/meshex.py
+-rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/mixins.py
+-rw-rw-rw-  2.0 fat     6203 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/mtextsurrogate.py
+-rw-rw-rw-  2.0 fat    13499 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/mtxpl.py
+-rw-rw-rw-  2.0 fat    16400 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/odafc.py
+-rw-rw-rw-  2.0 fat     9456 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/openscad.py
+-rw-rw-rw-  2.0 fat    15878 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/pycsg.py
+-rw-rw-rw-  2.0 fat    22496 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/r12export.py
+-rw-rw-rw-  2.0 fat    27198 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/r12writer.py
+-rw-rw-rw-  2.0 fat     7615 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/sierpinski_pyramid.py
+-rw-rw-rw-  2.0 fat    33167 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/tablepainter.py
+-rw-rw-rw-  2.0 fat    12766 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/text2path.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/xqt.py
+-rw-rw-rw-  2.0 fat      453 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/__init__.py
+-rw-rw-rw-  2.0 fat    10023 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/browser.py
+-rw-rw-rw-  2.0 fat     1907 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/data.py
+-rw-rw-rw-  2.0 fat       64 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/__init__.py
+-rw-rw-rw-  2.0 fat      820 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/bookmarks.py
+-rw-rw-rw-  2.0 fat    29367 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/browser.py
+-rw-rw-rw-  2.0 fat    14891 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/data.py
+-rw-rw-rw-  2.0 fat    10993 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/find_dialog.py
+-rw-rw-rw-  2.0 fat     1281 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/loader.py
+-rw-rw-rw-  2.0 fat    20974 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/model.py
+-rw-rw-rw-  2.0 fat     2214 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/tags.py
+-rw-rw-rw-  2.0 fat     1382 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/views.py
+-rw-rw-rw-  2.0 fat      133 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/browser/__init__.py
+-rw-rw-rw-  2.0 fat     7094 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/backend.py
+-rw-rw-rw-  2.0 fat     3611 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/clipper.py
+-rw-rw-rw-  2.0 fat     6737 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/config.py
+-rw-rw-rw-  2.0 fat     1392 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/debug_backend.py
+-rw-rw-rw-  2.0 fat      503 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/debug_utils.py
+-rw-rw-rw-  2.0 fat    41820 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/frontend.py
+-rw-rw-rw-  2.0 fat     1823 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/gfxproxy.py
+-rw-rw-rw-  2.0 fat    12613 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/matplotlib.py
+-rw-rw-rw-  2.0 fat     9854 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/mtext_complex.py
+-rw-rw-rw-  2.0 fat    37741 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/properties.py
+-rw-rw-rw-  2.0 fat    10774 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/pyqt.py
+-rw-rw-rw-  2.0 fat    16738 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/qtviewer.py
+-rw-rw-rw-  2.0 fat    13011 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/text.py
+-rw-rw-rw-  2.0 fat      860 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/text_renderer.py
+-rw-rw-rw-  2.0 fat      344 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/type_hints.py
+-rw-rw-rw-  2.0 fat     2461 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/unified_text_renderer.py
+-rw-rw-rw-  2.0 fat      171 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/drawing/__init__.py
+-rw-rw-rw-  2.0 fat     3112 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/classes_section.py
+-rw-rw-rw-  2.0 fat      763 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/const.py
+-rw-rw-rw-  2.0 fat     6091 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/crc.py
+-rw-rw-rw-  2.0 fat     3160 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/fileheader.py
+-rw-rw-rw-  2.0 fat    14851 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/header_section.py
+-rw-rw-rw-  2.0 fat     2976 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/loader.py
+-rw-rw-rw-  2.0 fat      141 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/dwg/__init__.py
+-rw-rw-rw-  2.0 fat     9531 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/api.py
+-rw-rw-rw-  2.0 fat     6651 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/backend.py
+-rw-rw-rw-  2.0 fat      513 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/compiler.py
+-rw-rw-rw-  2.0 fat      571 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/deps.py
+-rw-rw-rw-  2.0 fat     4720 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/dxf_backend.py
+-rw-rw-rw-  2.0 fat    16087 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/interpreter.py
+-rw-rw-rw-  2.0 fat     4836 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/page.py
+-rw-rw-rw-  2.0 fat     3527 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/pdf_backend.py
+-rw-rw-rw-  2.0 fat    11957 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/plotter.py
+-rw-rw-rw-  2.0 fat     1411 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/polygon_buffer.py
+-rw-rw-rw-  2.0 fat     5953 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/properties.py
+-rw-rw-rw-  2.0 fat     3731 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/svg_backend.py
+-rw-rw-rw-  2.0 fat     6258 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/tokenizer.py
+-rw-rw-rw-  2.0 fat      164 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/__init__.py
+-rw-rw-rw-  2.0 fat     4757 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat    18315 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/acad_table.py
+-rw-rw-rw-  2.0 fat    25923 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/acis.py
+-rw-rw-rw-  2.0 fat     4890 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/appdata.py
+-rw-rw-rw-  2.0 fat     1954 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/appid.py
+-rw-rw-rw-  2.0 fat     4942 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/arc.py
+-rw-rw-rw-  2.0 fat    26138 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/attrib.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/block.py
+-rw-rw-rw-  2.0 fat    10536 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/blockrecord.py
+-rw-rw-rw-  2.0 fat    50143 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/boundary_paths.py
+-rw-rw-rw-  2.0 fat     7961 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/circle.py
+-rw-rw-rw-  2.0 fat    23664 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dictionary.py
+-rw-rw-rw-  2.0 fat    48743 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dimension.py
+-rw-rw-rw-  2.0 fat    35012 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dimstyle.py
+-rw-rw-rw-  2.0 fat    23829 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dimstyleoverride.py
+-rw-rw-rw-  2.0 fat     4399 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dxfclass.py
+-rw-rw-rw-  2.0 fat    42404 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dxfentity.py
+-rw-rw-rw-  2.0 fat    26923 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dxfgfx.py
+-rw-rw-rw-  2.0 fat    15279 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dxfgroups.py
+-rw-rw-rw-  2.0 fat    23699 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dxfns.py
+-rw-rw-rw-  2.0 fat    13746 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/dxfobj.py
+-rw-rw-rw-  2.0 fat    11186 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/ellipse.py
+-rw-rw-rw-  2.0 fat     4170 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/factory.py
+-rw-rw-rw-  2.0 fat    23785 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/geodata.py
+-rw-rw-rw-  2.0 fat     4020 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/gradient.py
+-rw-rw-rw-  2.0 fat    12263 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/hatch.py
+-rw-rw-rw-  2.0 fat     3944 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/helix.py
+-rw-rw-rw-  2.0 fat     4747 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/idbuffer.py
+-rw-rw-rw-  2.0 fat    26057 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/image.py
+-rw-rw-rw-  2.0 fat    27932 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/insert.py
+-rw-rw-rw-  2.0 fat    27834 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/layer.py
+-rw-rw-rw-  2.0 fat    14252 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/layout.py
+-rw-rw-rw-  2.0 fat    12978 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/leader.py
+-rw-rw-rw-  2.0 fat     4718 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/light.py
+-rw-rw-rw-  2.0 fat     3718 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/line.py
+-rw-rw-rw-  2.0 fat     9677 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/ltype.py
+-rw-rw-rw-  2.0 fat    18878 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/lwpolyline.py
+-rw-rw-rw-  2.0 fat    19653 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/material.py
+-rw-rw-rw-  2.0 fat    18435 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/mesh.py
+-rw-rw-rw-  2.0 fat    57367 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/mleader.py
+-rw-rw-rw-  2.0 fat    37144 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/mline.py
+-rw-rw-rw-  2.0 fat     8385 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/mpolygon.py
+-rw-rw-rw-  2.0 fat    48153 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/mtext.py
+-rw-rw-rw-  2.0 fat     4351 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/mtext_columns.py
+-rw-rw-rw-  2.0 fat     6284 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/objectcollection.py
+-rw-rw-rw-  2.0 fat     2111 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/oleframe.py
+-rw-rw-rw-  2.0 fat     4332 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/pattern.py
+-rw-rw-rw-  2.0 fat     5238 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/point.py
+-rw-rw-rw-  2.0 fat    16416 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/polygon.py
+-rw-rw-rw-  2.0 fat    40087 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/polyline.py
+-rw-rw-rw-  2.0 fat     4822 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/shape.py
+-rw-rw-rw-  2.0 fat    10443 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/solid.py
+-rw-rw-rw-  2.0 fat    24085 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/spline.py
+-rw-rw-rw-  2.0 fat     8246 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/subentity.py
+-rw-rw-rw-  2.0 fat     5196 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/sun.py
+-rw-rw-rw-  2.0 fat     2449 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/table.py
+-rw-rw-rw-  2.0 fat    17602 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/text.py
+-rw-rw-rw-  2.0 fat     9042 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/textstyle.py
+-rw-rw-rw-  2.0 fat     3597 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/tolerance.py
+-rw-rw-rw-  2.0 fat     2703 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/ucs.py
+-rw-rw-rw-  2.0 fat    14366 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/underlay.py
+-rw-rw-rw-  2.0 fat     6040 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/view.py
+-rw-rw-rw-  2.0 fat    27893 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/viewport.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/visualstyle.py
+-rw-rw-rw-  2.0 fat     9970 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/vport.py
+-rw-rw-rw-  2.0 fat    17024 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/xdata.py
+-rw-rw-rw-  2.0 fat     8495 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/xdict.py
+-rw-rw-rw-  2.0 fat     3062 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/xline.py
+-rw-rw-rw-  2.0 fat     3127 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/entities/__init__.py
+-rw-rw-rw-  2.0 fat    16696 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/layouts/base.py
+-rw-rw-rw-  2.0 fat     4343 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/layouts/blocklayout.py
+-rw-rw-rw-  2.0 fat    29014 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/layouts/layout.py
+-rw-rw-rw-  2.0 fat    15314 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/layouts/layouts.py
+-rw-rw-rw-  2.0 fat      232 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/layouts/__init__.py
+-rw-rw-rw-  2.0 fat     8327 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/attributes.py
+-rw-rw-rw-  2.0 fat    16500 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/const.py
+-rw-rw-rw-  2.0 fat     1614 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/encoding.py
+-rw-rw-rw-  2.0 fat    17013 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/extendedtags.py
+-rw-rw-rw-  2.0 fat     5363 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/fileindex.py
+-rw-rw-rw-  2.0 fat      727 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/hdrvars.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/loader.py
+-rw-rw-rw-  2.0 fat     7447 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/packedtags.py
+-rw-rw-rw-  2.0 fat     6355 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/repair.py
+-rw-rw-rw-  2.0 fat    13058 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/tagger.py
+-rw-rw-rw-  2.0 fat    14336 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/tags.py
+-rw-rw-rw-  2.0 fat     8952 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/tagwriter.py
+-rw-rw-rw-  2.0 fat    12064 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/types.py
+-rw-rw-rw-  2.0 fat    17069 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/validator.py
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/lldxf/__init__.py
+-rw-rw-rw-  2.0 fat    19193 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/arc.py
+-rw-rw-rw-  2.0 fat    16270 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/bbox.py
+-rw-rw-rw-  2.0 fat     9318 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/bezier.py
+-rw-rw-rw-  2.0 fat     2452 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/bezier_interpolation.py
+-rw-rw-rw-  2.0 fat     8730 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/box.py
+-rw-rw-rw-  2.0 fat    52916 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/bspline.py
+-rw-rw-rw-  2.0 fat     5608 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/bulge.py
+-rw-rw-rw-  2.0 fat     9002 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/circle.py
+-rw-rw-rw-  2.0 fat    24003 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/clipping.py
+-rw-rw-rw-  2.0 fat     4319 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/clustering.py
+-rw-rw-rw-  2.0 fat    12236 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/construct2d.py
+-rw-rw-rw-  2.0 fat    26265 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/construct3d.py
+-rw-rw-rw-  2.0 fat     1283 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/cspline.py
+-rw-rw-rw-  2.0 fat     9114 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/curvetools.py
+-rw-rw-rw-  2.0 fat    22048 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/ellipse.py
+-rw-rw-rw-  2.0 fat     4406 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/eulerspiral.py
+-rw-rw-rw-  2.0 fat    38883 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/linalg.py
+-rw-rw-rw-  2.0 fat    10231 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/line.py
+-rw-rw-rw-  2.0 fat     3053 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/offset2d.py
+-rw-rw-rw-  2.0 fat     8256 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/parametrize.py
+-rw-rw-rw-  2.0 fat    15602 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/perlin.py
+-rw-rw-rw-  2.0 fat    15921 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/polyline.py
+-rw-rw-rw-  2.0 fat    11867 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/rtree.py
+-rw-rw-rw-  2.0 fat     3910 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/shape.py
+-rw-rw-rw-  2.0 fat     2568 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/surfaces.py
+-rw-rw-rw-  2.0 fat    12155 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/transformtools.py
+-rw-rw-rw-  2.0 fat     3631 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/triangulation.py
+-rw-rw-rw-  2.0 fat    16971 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/ucs.py
+-rw-rw-rw-  2.0 fat     7213 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_bezier3p.py
+-rw-rw-rw-  2.0 fat    12967 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_bezier4p.py
+-rw-rw-rw-  2.0 fat     9440 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_bspline.py
+-rw-rw-rw-  2.0 fat     7272 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_construct.py
+-rw-rw-rw-  2.0 fat     2261 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_ctypes.py
+-rw-rw-rw-  2.0 fat    24954 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    26418 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_matrix44.py
+-rw-rw-rw-  2.0 fat    25912 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/_vector.py
+-rw-rw-rw-  2.0 fat     2003 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/math/__init__.py
+-rw-rw-rw-  2.0 fat     1306 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/commands.py
+-rw-rw-rw-  2.0 fat    39194 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/converter.py
+-rw-rw-rw-  2.0 fat     6748 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/nesting.py
+-rw-rw-rw-  2.0 fat    20453 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/path.py
+-rw-rw-rw-  2.0 fat    10140 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/shapes.py
+-rw-rw-rw-  2.0 fat    34692 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/tools.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/path/__init__.py
+-rw-rw-rw-  2.0 fat     2987 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.css
+-rw-rw-rw-  2.0 fat     1148 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.html
+-rw-rw-rw-  2.0 fat    11304 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.js
+-rw-rw-rw-  2.0 fat    17144 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.py
+-rw-rw-rw-  2.0 fat     3770 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/pprint.py
+-rw-rw-rw-  2.0 fat      812 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.css
+-rw-rw-rw-  2.0 fat      316 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.html
+-rw-rw-rw-  2.0 fat     2545 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.py
+-rw-rw-rw-  2.0 fat     6896 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/reflinks.py
+-rw-rw-rw-  2.0 fat      123 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/pp/__init__.py
+-rw-rw-rw-  2.0 fat    10076 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/abstract_mtext_renderer.py
+-rw-rw-rw-  2.0 fat    20495 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/arrows.py
+-rw-rw-rw-  2.0 fat    17749 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/curves.py
+-rw-rw-rw-  2.0 fat     4041 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dimension.py
+-rw-rw-rw-  2.0 fat    52028 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dim_base.py
+-rw-rw-rw-  2.0 fat    35702 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dim_curved.py
+-rw-rw-rw-  2.0 fat     6894 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dim_diameter.py
+-rw-rw-rw-  2.0 fat    24751 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dim_linear.py
+-rw-rw-rw-  2.0 fat     8084 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dim_ordinate.py
+-rw-rw-rw-  2.0 fat    20295 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/dim_radius.py
+-rw-rw-rw-  2.0 fat    47170 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/forms.py
+-rw-rw-rw-  2.0 fat    24213 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/hatching.py
+-rw-rw-rw-  2.0 fat     4728 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/leader.py
+-rw-rw-rw-  2.0 fat      664 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/linetypes.py
+-rw-rw-rw-  2.0 fat    64121 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/mesh.py
+-rw-rw-rw-  2.0 fat    60923 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/mleader.py
+-rw-rw-rw-  2.0 fat     8437 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/mline.py
+-rw-rw-rw-  2.0 fat     2964 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/point.py
+-rw-rw-rw-  2.0 fat     8736 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/polyline.py
+-rw-rw-rw-  2.0 fat     7886 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/r12spline.py
+-rw-rw-rw-  2.0 fat    22541 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/trace.py
+-rw-rw-rw-  2.0 fat     2881 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/_linetypes.py
+-rw-rw-rw-  2.0 fat      778 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/render/__init__.py
+-rw-rw-rw-  2.0 fat     1050 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/16x16.png
+-rw-rw-rw-  2.0 fat     1420 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/24x24.png
+-rw-rw-rw-  2.0 fat    10638 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/256x256.png
+-rw-rw-rw-  2.0 fat     1758 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/32x32.png
+-rw-rw-rw-  2.0 fat     2335 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/48x48.png
+-rw-rw-rw-  2.0 fat     3050 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/64x64.png
+-rw-rw-rw-  2.0 fat     2090 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-copy-64px.png
+-rw-rw-rw-  2.0 fat     3109 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-find-64px.png
+-rw-rw-rw-  2.0 fat     2388 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-bookmark-64px.png
+-rw-rw-rw-  2.0 fat     2519 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-handle-64px.png
+-rw-rw-rw-  2.0 fat     2409 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-line-64px.png
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-left-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2322 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-next-entity-64px.png
+-rw-rw-rw-  2.0 fat     2320 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-prev-entity-64px.png
+-rw-rw-rw-  2.0 fat     2244 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-right-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2553 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-show-in-tree-64px.png
+-rw-rw-rw-  2.0 fat     2373 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/resources/icon-store-bookmark-64px.png
+-rw-rw-rw-  2.0 fat    10650 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/acdsdata.py
+-rw-rw-rw-  2.0 fat    16508 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/blocks.py
+-rw-rw-rw-  2.0 fat    11639 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/classes.py
+-rw-rw-rw-  2.0 fat     4137 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/entities.py
+-rw-rw-rw-  2.0 fat    11953 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/header.py
+-rw-rw-rw-  2.0 fat    60696 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/headervars.py
+-rw-rw-rw-  2.0 fat    27009 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/objects.py
+-rw-rw-rw-  2.0 fat    26581 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/table.py
+-rw-rw-rw-  2.0 fat     5270 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/tables.py
+-rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/sections/__init__.py
+-rw-rw-rw-  2.0 fat    19711 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/analyze.py
+-rw-rw-rw-  2.0 fat    20434 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/binarydata.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/codepage.py
+-rw-rw-rw-  2.0 fat     7645 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/complex_ltype.py
+-rw-rw-rw-  2.0 fat     1782 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/crypt.py
+-rw-rw-rw-  2.0 fat     1511 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/debug.py
+-rw-rw-rw-  2.0 fat     2341 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/difftags.py
+-rw-rw-rw-  2.0 fat    15940 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/fonts.py
+-rw-rw-rw-  2.0 fat     2233 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/font_face.py
+-rw-rw-rw-  2.0 fat    10887 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/font_manager.py
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/handle.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/indexing.py
+-rw-rw-rw-  2.0 fat     2145 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/juliandate.py
+-rw-rw-rw-  2.0 fat     6166 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/pattern.py
+-rw-rw-rw-  2.0 fat     1256 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/rawloader.py
+-rw-rw-rw-  2.0 fat   129174 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/standards.py
+-rw-rw-rw-  2.0 fat     6049 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/strip.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/test.py
+-rw-rw-rw-  2.0 fat    65388 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/text.py
+-rw-rw-rw-  2.0 fat    54234 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/text_layout.py
+-rw-rw-rw-  2.0 fat     6883 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/text_size.py
+-rw-rw-rw-  2.0 fat     6678 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/ttfonts.py
+-rw-rw-rw-  2.0 fat     3077 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/zipmanager.py
+-rw-rw-rw-  2.0 fat   142734 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/_iso_pattern.py
+-rw-rw-rw-  2.0 fat     3564 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf/tools/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat       47 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat    68966 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      302 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat    31075 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/src/ezdxf.egg-info/top_level.txt
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_10_issues/
+-rw-rw-rw-  2.0 fat      402 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/conftest.py
+-rw-rw-rw-  2.0 fat     2336 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+-rw-rw-rw-  2.0 fat     2599 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+-rw-rw-rw-  2.0 fat     1124 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+-rw-rw-rw-  2.0 fat     5456 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+-rw-rw-rw-  2.0 fat      582 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+-rw-rw-rw-  2.0 fat    11593 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+-rw-rw-rw-  2.0 fat     1191 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+-rw-rw-rw-  2.0 fat     1033 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+-rw-rw-rw-  2.0 fat     4792 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+-rw-rw-rw-  2.0 fat      989 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+-rw-rw-rw-  2.0 fat     1383 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_018_handle.py
+-rw-rw-rw-  2.0 fat     5518 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+-rw-rw-rw-  2.0 fat     8168 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+-rw-rw-rw-  2.0 fat     3787 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+-rw-rw-rw-  2.0 fat      401 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+-rw-rw-rw-  2.0 fat      539 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+-rw-rw-rw-  2.0 fat     2092 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_040_tags.py
+-rw-rw-rw-  2.0 fat     3073 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+-rw-rw-rw-  2.0 fat     6419 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+-rw-rw-rw-  2.0 fat     1632 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+-rw-rw-rw-  2.0 fat    11265 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+-rw-rw-rw-  2.0 fat     3363 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+-rw-rw-rw-  2.0 fat     1974 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+-rw-rw-rw-  2.0 fat     2321 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+-rw-rw-rw-  2.0 fat      568 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+-rw-rw-rw-  2.0 fat     8682 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+-rw-rw-rw-  2.0 fat     1051 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+-rw-rw-rw-  2.0 fat     1500 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+-rw-rw-rw-  2.0 fat    11689 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+-rw-rw-rw-  2.0 fat     2893 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_102_appdata.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_103_reactors.py
+-rw-rw-rw-  2.0 fat     4001 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_104_extension_dict.py
+-rw-rw-rw-  2.0 fat    20860 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_105_xdata.py
+-rw-rw-rw-  2.0 fat    14169 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_110_dxfentity.py
+-rw-rw-rw-  2.0 fat     2433 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+-rw-rw-rw-  2.0 fat     6781 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+-rw-rw-rw-  2.0 fat      695 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_112b_dxfobj.py
+-rw-rw-rw-  2.0 fat     2431 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_113_dxfclass.py
+-rw-rw-rw-  2.0 fat     4044 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_114_factory.py
+-rw-rw-rw-  2.0 fat     2256 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+-rw-rw-rw-  2.0 fat    15794 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_116_dictionary.py
+-rw-rw-rw-  2.0 fat     4999 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+-rw-rw-rw-  2.0 fat     3003 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_120_style_table_entry.py
+-rw-rw-rw-  2.0 fat     2943 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+-rw-rw-rw-  2.0 fat      379 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+-rw-rw-rw-  2.0 fat     1113 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_123_view_table_entry.py
+-rw-rw-rw-  2.0 fat     8757 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_125_image_def.py
+-rw-rw-rw-  2.0 fat     1312 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+-rw-rw-rw-  2.0 fat     1430 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_127_raster_variables.py
+-rw-rw-rw-  2.0 fat     1540 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_128_pdf_definition.py
+-rw-rw-rw-  2.0 fat     2778 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_129_xrecord.py
+-rw-rw-rw-  2.0 fat     2423 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_130_id_buffer.py
+-rw-rw-rw-  2.0 fat     2470 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_131_field_list.py
+-rw-rw-rw-  2.0 fat     2435 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_132_layer_filter.py
+-rw-rw-rw-  2.0 fat     2153 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_133_sun.py
+-rw-rw-rw-  2.0 fat      852 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_134_material.py
+-rw-rw-rw-  2.0 fat    11497 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_135_geo_data.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_136_vba_project.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_137_sortentstable.py
+-rw-rw-rw-  2.0 fat      704 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+-rw-rw-rw-  2.0 fat     7570 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_139_user_record.py
+-rw-rw-rw-  2.0 fat      714 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_140_block_record.py
+-rw-rw-rw-  2.0 fat     9153 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/conftest.py
+-rw-rw-rw-  2.0 fat     6532 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_200_line.py
+-rw-rw-rw-  2.0 fat     4273 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_201_point.py
+-rw-rw-rw-  2.0 fat     6827 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_202_circle.py
+-rw-rw-rw-  2.0 fat     8949 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_203_arc.py
+-rw-rw-rw-  2.0 fat     2852 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_204_shape.py
+-rw-rw-rw-  2.0 fat     8242 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_205_solid.py
+-rw-rw-rw-  2.0 fat     8476 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_206_text.py
+-rw-rw-rw-  2.0 fat     4947 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_207_attdef.py
+-rw-rw-rw-  2.0 fat     6312 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_208_attrib.py
+-rw-rw-rw-  2.0 fat     2671 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_209_vertex.py
+-rw-rw-rw-  2.0 fat     5930 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_1.py
+-rw-rw-rw-  2.0 fat    13489 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_2.py
+-rw-rw-rw-  2.0 fat     6650 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+-rw-rw-rw-  2.0 fat     1780 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+-rw-rw-rw-  2.0 fat     7847 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_211_viewport.py
+-rw-rw-rw-  2.0 fat    12629 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_212_insert.py
+-rw-rw-rw-  2.0 fat     6024 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_213_minsert.py
+-rw-rw-rw-  2.0 fat     3284 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_214_block.py
+-rw-rw-rw-  2.0 fat     6882 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_215_dimension.py
+-rw-rw-rw-  2.0 fat     4907 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+-rw-rw-rw-  2.0 fat    13186 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+-rw-rw-rw-  2.0 fat     6471 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+-rw-rw-rw-  2.0 fat     5535 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+-rw-rw-rw-  2.0 fat     3056 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+-rw-rw-rw-  2.0 fat     7181 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+-rw-rw-rw-  2.0 fat     2066 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+-rw-rw-rw-  2.0 fat     3615 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+-rw-rw-rw-  2.0 fat     6919 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_221_ellipse.py
+-rw-rw-rw-  2.0 fat     2223 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_222_xline.py
+-rw-rw-rw-  2.0 fat     1493 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_223_ray.py
+-rw-rw-rw-  2.0 fat     2176 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_224_group.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_225_mtext.py
+-rw-rw-rw-  2.0 fat    12020 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_226_spline.py
+-rw-rw-rw-  2.0 fat     5529 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+-rw-rw-rw-  2.0 fat    10893 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+-rw-rw-rw-  2.0 fat    15116 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_228_mesh.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+-rw-rw-rw-  2.0 fat    21421 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+-rw-rw-rw-  2.0 fat     6587 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+-rw-rw-rw-  2.0 fat     3140 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+-rw-rw-rw-  2.0 fat    12486 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+-rw-rw-rw-  2.0 fat     2274 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_231_underlay.py
+-rw-rw-rw-  2.0 fat     5243 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_231_underlay_2.py
+-rw-rw-rw-  2.0 fat     2294 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_acis.py
+-rw-rw-rw-  2.0 fat     6799 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_acis_2.py
+-rw-rw-rw-  2.0 fat     1854 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_surface.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_233_helix.py
+-rw-rw-rw-  2.0 fat     2040 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_234_light.py
+-rw-rw-rw-  2.0 fat     3806 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_235_leader.py
+-rw-rw-rw-  2.0 fat    20392 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_236_multileader.py
+-rw-rw-rw-  2.0 fat    10992 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_237_mline.py
+-rw-rw-rw-  2.0 fat     2356 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_238_tolerance.py
+-rw-rw-rw-  2.0 fat    27392 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+-rw-rw-rw-  2.0 fat     4347 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_241_hyperlink.py
+-rw-rw-rw-  2.0 fat    11313 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_242_random_transform.py
+-rw-rw-rw-  2.0 fat     3725 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_243_replace_entity.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+-rw-rw-rw-  2.0 fat     4456 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_245_wipeout.py
+-rw-rw-rw-  2.0 fat     6175 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_246_spline_audit.py
+-rw-rw-rw-  2.0 fat     8165 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+-rw-rw-rw-  2.0 fat     6003 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_248_mpolygon.py
+-rw-rw-rw-  2.0 fat    13682 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+-rw-rw-rw-  2.0 fat     5713 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+-rw-rw-rw-  2.0 fat     8331 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+-rw-rw-rw-  2.0 fat     7331 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_251_upright.py
+-rw-rw-rw-  2.0 fat     4795 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat     2082 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_253_ole2frame.py
+-rw-rw-rw-  2.0 fat      821 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_254_get_font_name.py
+-rw-rw-rw-  2.0 fat     5149 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_300_layout.py
+-rw-rw-rw-  2.0 fat     4274 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+-rw-rw-rw-  2.0 fat     5582 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_302_block_references.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+-rw-rw-rw-  2.0 fat      913 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+-rw-rw-rw-  2.0 fat     3279 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+-rw-rw-rw-  2.0 fat     2609 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+-rw-rw-rw-  2.0 fat     2343 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_307_groupby.py
+-rw-rw-rw-  2.0 fat    17748 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_308_query.py
+-rw-rw-rw-  2.0 fat     6382 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_309_query_parser.py
+-rw-rw-rw-  2.0 fat     5031 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+-rw-rw-rw-  2.0 fat     5782 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+-rw-rw-rw-  2.0 fat      647 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_313_redraw_order.py
+-rw-rw-rw-  2.0 fat     6128 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+-rw-rw-rw-  2.0 fat     2750 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+-rw-rw-rw-  2.0 fat     5208 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+-rw-rw-rw-  2.0 fat     6795 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+-rw-rw-rw-  2.0 fat     4981 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+-rw-rw-rw-  2.0 fat     2450 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_405_classes.py
+-rw-rw-rw-  2.0 fat     9094 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+-rw-rw-rw-  2.0 fat      848 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+-rw-rw-rw-  2.0 fat     3375 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+-rw-rw-rw-  2.0 fat     1433 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+-rw-rw-rw-  2.0 fat     5736 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_410_table.py
+-rw-rw-rw-  2.0 fat     6607 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+-rw-rw-rw-  2.0 fat    18072 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+-rw-rw-rw-  2.0 fat     4638 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+-rw-rw-rw-  2.0 fat    12354 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+-rw-rw-rw-  2.0 fat     6509 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+-rw-rw-rw-  2.0 fat     5656 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+-rw-rw-rw-  2.0 fat     5434 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+-rw-rw-rw-  2.0 fat      733 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+-rw-rw-rw-  2.0 fat     1240 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+-rw-rw-rw-  2.0 fat     5007 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+-rw-rw-rw-  2.0 fat      769 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+-rw-rw-rw-  2.0 fat     7289 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_424_audit.py
+-rw-rw-rw-  2.0 fat     3737 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+-rw-rw-rw-  2.0 fat     2981 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+-rw-rw-rw-  2.0 fat     2416 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+-rw-rw-rw-  2.0 fat     2533 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+-rw-rw-rw-  2.0 fat   112800 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/conftest.py
+-rw-rw-rw-  2.0 fat     5510 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_500_units.py
+-rw-rw-rw-  2.0 fat     1052 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_501_truecolor.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_502_raw_color.py
+-rw-rw-rw-  2.0 fat     1695 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_503_indexing.py
+-rw-rw-rw-  2.0 fat     1442 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_504_suppress_zeros.py
+-rw-rw-rw-  2.0 fat      216 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_506_version.py
+-rw-rw-rw-  2.0 fat      579 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_507_dxf_pretty_printer.py
+-rw-rw-rw-  2.0 fat      657 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_508_read_zip.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_509_comments.py
+-rw-rw-rw-  2.0 fat     1185 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_510_byte_stream.py
+-rw-rw-rw-  2.0 fat     4239 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_511_bit_stream.py
+-rw-rw-rw-  2.0 fat     5595 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_512_pattern.py
+-rw-rw-rw-  2.0 fat     2372 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_513_reorder_entities.py
+-rw-rw-rw-  2.0 fat    17710 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_514_text.py
+-rw-rw-rw-  2.0 fat     6261 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_515_fonts.py
+-rw-rw-rw-  2.0 fat     4002 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_516_zoom.py
+-rw-rw-rw-  2.0 fat    34209 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_517_text_layout.py
+-rw-rw-rw-  2.0 fat      474 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_518_header_guid.py
+-rw-rw-rw-  2.0 fat     3716 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_519_mtext_editor.py
+-rw-rw-rw-  2.0 fat     3205 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_520_mtext_context.py
+-rw-rw-rw-  2.0 fat    24496 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_521_mtext_parser.py
+-rw-rw-rw-  2.0 fat     3863 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_522_text_scanner.py
+-rw-rw-rw-  2.0 fat     5207 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_523_text_size.py
+-rw-rw-rw-  2.0 fat     5063 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_524_block_reference_manager.py
+-rw-rw-rw-  2.0 fat      773 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_525_transparency.py
+-rw-rw-rw-  2.0 fat     2133 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_526_explode.py
+-rw-rw-rw-  2.0 fat    13521 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_527_gfxattribs.py
+-rw-rw-rw-  2.0 fat     2748 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_528_difftags.py
+-rw-rw-rw-  2.0 fat     6700 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_529_acis_sat.py
+-rw-rw-rw-  2.0 fat     2062 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_530_acis_sab.py
+-rw-rw-rw-  2.0 fat    12366 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_531_acis_entities.py
+-rw-rw-rw-  2.0 fat     7533 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_532_acis_mesh.py
+-rw-rw-rw-  2.0 fat    42518 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_533_shapefiles.py
+-rw-rw-rw-  2.0 fat     1034 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_534_dwg_info.py
+-rw-rw-rw-  2.0 fat    47915 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_535_xref_basic.py
+-rw-rw-rw-  2.0 fat    27614 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_536_xref_conflict.py
+-rw-rw-rw-  2.0 fat     6887 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_537_transform.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+-rw-rw-rw-  2.0 fat     2763 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_05_tools/test_539_npshapes.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/conftest.py
+-rw-rw-rw-  2.0 fat     7460 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_600_base.py
+-rw-rw-rw-  2.0 fat     2098 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_601_bulge.py
+-rw-rw-rw-  2.0 fat    14651 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_602_vec3.py
+-rw-rw-rw-  2.0 fat     8956 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_603_vec2.py
+-rw-rw-rw-  2.0 fat     2801 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_604_banded_matrix.py
+-rw-rw-rw-  2.0 fat     9738 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_604_linalg.py
+-rw-rw-rw-  2.0 fat    13007 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_605_matrix44.py
+-rw-rw-rw-  2.0 fat     5888 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_606_convexhull.py
+-rw-rw-rw-  2.0 fat     1010 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_607_perlin_noise.py
+-rw-rw-rw-  2.0 fat     3833 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_608_intersection_line_line_2d.py
+-rw-rw-rw-  2.0 fat     1676 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_609_point_on_line.py
+-rw-rw-rw-  2.0 fat     3171 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_610_ocs.py
+-rw-rw-rw-  2.0 fat     7529 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_611_ucs.py
+-rw-rw-rw-  2.0 fat     1831 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_612_ucs_pass_trough.py
+-rw-rw-rw-  2.0 fat     2586 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_613_point_in_poygon.py
+-rw-rw-rw-  2.0 fat    10913 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_614_construct_3d.py
+-rw-rw-rw-  2.0 fat      602 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_615_rytz_axis.py
+-rw-rw-rw-  2.0 fat     5215 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_616_plane.py
+-rw-rw-rw-  2.0 fat      772 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_617_clockwise_orientation.py
+-rw-rw-rw-  2.0 fat     6384 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_618_clipping.py
+-rw-rw-rw-  2.0 fat    10108 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_619_greiner_hormann.py
+-rw-rw-rw-  2.0 fat     2669 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_620_knot.py
+-rw-rw-rw-  2.0 fat    18821 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_621_bspline.py
+-rw-rw-rw-  2.0 fat     7652 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_622_bsplineu.py
+-rw-rw-rw-  2.0 fat    11327 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_623_rbspline.py
+-rw-rw-rw-  2.0 fat    10809 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_624_global_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1247 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_626_local_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1967 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_627_bspline_basis.py
+-rw-rw-rw-  2.0 fat    10545 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_629_bezier.py
+-rw-rw-rw-  2.0 fat    10714 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_630a_bezier4p_base.py
+-rw-rw-rw-  2.0 fat    10204 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_630b_bezier4p_functions.py
+-rw-rw-rw-  2.0 fat     1683 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_631_euler_spiral.py
+-rw-rw-rw-  2.0 fat     4021 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_632_bezier3p.py
+-rw-rw-rw-  2.0 fat    19463 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_640_bbox.py
+-rw-rw-rw-  2.0 fat     5393 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_641_construction_ray.py
+-rw-rw-rw-  2.0 fat     3673 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_642_construction_line.py
+-rw-rw-rw-  2.0 fat     9459 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_643_construction_box.py
+-rw-rw-rw-  2.0 fat    10941 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_644_construction_circle.py
+-rw-rw-rw-  2.0 fat    10988 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_645_construction_arc.py
+-rw-rw-rw-  2.0 fat     3422 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_646_offset_vertices_2d.py
+-rw-rw-rw-  2.0 fat     7672 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_647_transform_tools.py
+-rw-rw-rw-  2.0 fat     8993 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_648_construction_ellipse.py
+-rw-rw-rw-  2.0 fat     4243 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_650_elliptic_arc_span.py
+-rw-rw-rw-  2.0 fat     9011 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_651_construction_polyline.py
+-rw-rw-rw-  2.0 fat     3168 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_652_approx_param_t.py
+-rw-rw-rw-  2.0 fat     5806 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_653_polyline_intersection.py
+-rw-rw-rw-  2.0 fat     5193 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_654_rtree.py
+-rw-rw-rw-  2.0 fat      788 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_655_dbscan.py
+-rw-rw-rw-  2.0 fat      834 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_656_k_means.py
+-rw-rw-rw-  2.0 fat     4654 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_657_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    11628 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_658_bevel_tools.py
+-rw-rw-rw-  2.0 fat     1875 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1428 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1741 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+-rw-rw-rw-  2.0 fat     3307 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_06_math/test_662_is_convex_polygon_2d.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_701_arrows.py
+-rw-rw-rw-  2.0 fat    17245 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_702_render_forms.py
+-rw-rw-rw-  2.0 fat    34220 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_703_mesh_builder.py
+-rw-rw-rw-  2.0 fat     3852 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_704_render_linear_dimension.py
+-rw-rw-rw-  2.0 fat     1345 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_705_shape.py
+-rw-rw-rw-  2.0 fat      483 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_706_random_path.py
+-rw-rw-rw-  2.0 fat     5603 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_707_trace.py
+-rw-rw-rw-  2.0 fat    33834 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_708a_path.py
+-rw-rw-rw-  2.0 fat    27351 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_708b_path_tools.py
+-rw-rw-rw-  2.0 fat     3633 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_708c_matplotlib_path_tools.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_708d_qpainter_path_tools.py
+-rw-rw-rw-  2.0 fat     4589 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_708e_path_shapes.py
+-rw-rw-rw-  2.0 fat     4118 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_708f_path_nesting.py
+-rw-rw-rw-  2.0 fat     1308 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_709_linetype_renderer.py
+-rw-rw-rw-  2.0 fat     2815 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_711_points.py
+-rw-rw-rw-  2.0 fat     6594 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_712_render_curved_dimension.py
+-rw-rw-rw-  2.0 fat     1472 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_713_mleader_builder.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_714_mleader_render_engine.py
+-rw-rw-rw-  2.0 fat    11778 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_715_hatching.py
+-rw-rw-rw-  2.0 fat     2626 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+-rw-rw-rw-  2.0 fat     4771 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_800_mtext_surrogate.py
+-rw-rw-rw-  2.0 fat     1352 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_801_r12spline.py
+-rw-rw-rw-  2.0 fat     7881 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_802_table_painter.py
+-rw-rw-rw-  2.0 fat    12386 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_803_entities_to_code.py
+-rw-rw-rw-  2.0 fat     6844 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_804_importer.py
+-rw-rw-rw-  2.0 fat     2362 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_805_pycsg.py
+-rw-rw-rw-  2.0 fat    15467 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_806_acadctb.py
+-rw-rw-rw-  2.0 fat     4860 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_807_dwg_loader_basics.py
+-rw-rw-rw-  2.0 fat    10862 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_810_drawing_properties.py
+-rw-rw-rw-  2.0 fat    11175 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_811_drawing_frontend.py
+-rw-rw-rw-  2.0 fat     4157 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+-rw-rw-rw-  2.0 fat    12547 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_813_geo_interface.py
+-rw-rw-rw-  2.0 fat    15590 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_814_text2path.py
+-rw-rw-rw-  2.0 fat    16239 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_815_dxf_browser.py
+-rw-rw-rw-  2.0 fat    11275 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_816_bin_packing.py
+-rw-rw-rw-  2.0 fat    12554 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_817_genetic_algorithm.py
+-rw-rw-rw-  2.0 fat     9008 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_818_meshex.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_819_menger_sponge.py
+-rw-rw-rw-  2.0 fat     4433 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_820_openscad.py
+-rw-rw-rw-  2.0 fat    15527 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_821_hpgl2.py
+-rw-rw-rw-  2.0 fat     1322 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+-rw-rw-rw-  2.0 fat      976 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_08_addons/test_822_clipper.py
+-rw-rw-rw-  2.0 fat     2527 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+-rw-rw-rw-  2.0 fat     2199 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+-rw-rw-rw-  2.0 fat     1732 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+-rw-rw-rw-  2.0 fat     3158 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+-rw-rw-rw-  2.0 fat     1452 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+-rw-rw-rw-  2.0 fat     4755 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+-rw-rw-rw-  2.0 fat     2656 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_10_issues/test_issue_414_bbox_calculation.py
+-rw-rw-rw-  2.0 fat     1213 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_10_issues/test_issue_574_flattening_error.py
+-rw-rw-rw-  2.0 fat     1754 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+-rw-rw-rw-  2.0 fat      682 b- defN 23-Apr-27 05:13 ezdxf-1.1.0b0/tests/test_10_issues/test_issue_749_text_layout.py
+819 files, 8482167 bytes uncompressed, 1907843 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -1,2458 +1,2458 @@
-Filename: ezdxf-1.0.4b1/
+Filename: ezdxf-1.1.0b0/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/
+Filename: ezdxf-1.1.0b0/integration_tests/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/
+Filename: ezdxf-1.1.0b0/src/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/
+Filename: ezdxf-1.1.0b0/tests/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/LICENSE
+Filename: ezdxf-1.1.0b0/LICENSE
 Comment: 
 
-Filename: ezdxf-1.0.4b1/MANIFEST.in
+Filename: ezdxf-1.1.0b0/MANIFEST.in
 Comment: 
 
-Filename: ezdxf-1.0.4b1/NEWS.md
+Filename: ezdxf-1.1.0b0/NEWS.md
 Comment: 
 
-Filename: ezdxf-1.0.4b1/PKG-INFO
+Filename: ezdxf-1.1.0b0/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.0.4b1/README.md
+Filename: ezdxf-1.1.0b0/README.md
 Comment: 
 
-Filename: ezdxf-1.0.4b1/requirements.txt
+Filename: ezdxf-1.1.0b0/requirements.txt
 Comment: 
 
-Filename: ezdxf-1.0.4b1/setup.cfg
+Filename: ezdxf-1.1.0b0/setup.cfg
 Comment: 
 
-Filename: ezdxf-1.0.4b1/setup.py
+Filename: ezdxf-1.1.0b0/setup.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/
+Filename: ezdxf-1.1.0b0/integration_tests/data/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/check_disable_c_ext_by_config_file.py
+Filename: ezdxf-1.1.0b0/integration_tests/check_disable_c_ext_by_config_file.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/check_disable_c_ext_by_env_var.py
+Filename: ezdxf-1.1.0b0/integration_tests/check_disable_c_ext_by_env_var.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_acad_table.py
+Filename: ezdxf-1.1.0b0/integration_tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_all_dimline_styles.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_acad_table.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_all_ellipse_transformations.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_all_dimline_styles.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_anonymous_blocks.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_all_ellipse_transformations.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_audit_critical_dxf_files.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_anonymous_blocks.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_audit_layouts.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_audit_critical_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_complex_line_type_2.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_audit_layouts.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_create_basic_graphics.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_complex_line_type_2.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_document_guid.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_create_basic_graphics.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_document_page_setup.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_document_guid.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_drawing_matplotlib_backend.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_document_page_setup.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_drawing_qt_backend.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_dxf_info_scanning.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_dxf_info_scanning.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_entities_iterator.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_entities_iterator.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_fix_dulicate_handles.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_fix_dulicate_handles.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_geo.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_geo.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_groups.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_groups.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_ignore_junk_beyond_EOF.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_ignore_junk_beyond_EOF.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_launcher.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_launcher.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_leica_disto_r12.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_leica_disto_r12.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_load_dxf_unicode_notation.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_load_dxf_unicode_notation.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_mapbox_earcut.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_matplotlib_font_support.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_mtext_explode_addon.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_mtext_columns.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_mtext_text_frame.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_mtext_explode_addon.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_new_table_entries.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_mtext_text_frame.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_none_ascii_read_write.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_new_table_entries.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_odafc.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_none_ascii_read_write.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_open_binary_DXF_files.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_odafc.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_open_coord_order_issue.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_open_binary_DXF_files.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_open_exotic_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_open_coord_order_issue.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_open_R13_R14.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_open_exotic_dxf_files.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_polyline_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_open_R13_R14.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_preserve_binary_data_in_xrecords.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_polyline_entity.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_r12export.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_preserve_binary_data_in_xrecords.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_r12strict.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_r12export.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_r12writer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_r12strict.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_read_file_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_r12writer.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_read_write_modern_entites.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_read_file_without_handles.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_recover.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_read_write_modern_entites.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_recover.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_rotated_block_attributes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_redraw_order.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_surface_entities.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_rotated_block_attributes.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_write_fixed_meta_data.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_surface_entities.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_write_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_write_fixed_meta_data.py
+Filename: ezdxf-1.1.0b0/integration_tests/test_xref_detach.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_write_without_handles.py
+Filename: ezdxf-1.1.0b0/integration_tests/data/AC1003_LINE_Example.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/test_xref_detach.py
+Filename: ezdxf-1.1.0b0/integration_tests/data/acad_table_with_blk_ref.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/AC1003_LINE_Example.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/ASCII_R12.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/acad_table_with_blk_ref.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r12.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/ASCII_R12.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r12.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r13.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r2000.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r14.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/cc_dxflib.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r2000.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/custom_blocks.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/cc_dxflib.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/duplicate_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/custom_blocks.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/dxf_unicode.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/duplicate_handles.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/empty_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/dxf_unicode.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/groups.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/empty_handles.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/Leica_Disto_S910.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/groups.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/MODEL.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/Leica_Disto_S910.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/mtext_columns_R2007.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/MODEL.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/mtext_columns_R2018.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/mtext_columns_R2007.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/mtext_framed_columns.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/mtext_columns_R2018.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/mtext_text_frame.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/mtext_framed_columns.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/no_layouts.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/mtext_text_frame.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/POLI-ALL210_12.DXF
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/no_layouts.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/R12_with_trash_beyond_EOF.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/POLI-ALL210_12.DXF
+Filename: ezdxf-1.1.0b0/integration_tests/data/recover01.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/recover02.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/recover01.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/small_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/recover02.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/small_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/small_r13.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/XRECORD_0.bin
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/small_r14.dxf
+Filename: ezdxf-1.1.0b0/integration_tests/data/XRECORD_1.bin
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/XRECORD_0.bin
+Filename: ezdxf-1.1.0b0/integration_tests/data/XRECORD_2.bin
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/XRECORD_1.bin
+Filename: ezdxf-1.1.0b0/src/ezdxf/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/integration_tests/data/XRECORD_2.bin
+Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/
+Filename: ezdxf-1.1.0b0/src/ezdxf/acis/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acis/
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/
+Filename: ezdxf-1.1.0b0/src/ezdxf/layouts/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/layouts/
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/
+Filename: ezdxf-1.1.0b0/src/ezdxf/path/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/
+Filename: ezdxf-1.1.0b0/src/ezdxf/pp/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/path/
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/pp/
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/
+Filename: ezdxf-1.1.0b0/src/ezdxf/sections/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/sections/
+Filename: ezdxf-1.1.0b0/src/ezdxf/appsettings.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/
+Filename: ezdxf-1.1.0b0/src/ezdxf/audit.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/appsettings.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/bbox.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/audit.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/blkrefs.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/bbox.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/colors.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/blkrefs.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/commands.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/colors.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/comments.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/commands.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/disassemble.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/comments.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/document.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/disassemble.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/dwginfo.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/document.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entitydb.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/dwginfo.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/enums.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entitydb.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/explode.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/enums.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/eztypes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/explode.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/filemanagement.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/eztypes.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/filemanagement.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/graphicsfactory.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/gfxattribs.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/groupby.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/graphicsfactory.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/npshapes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/groupby.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/protocols.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/protocols.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/proxygraphic.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/proxygraphic.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/py.typed
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/py.typed
+Filename: ezdxf-1.1.0b0/src/ezdxf/query.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/query.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/queryparser.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/queryparser.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/r12strict.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/r12strict.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/recover.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/recover.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/reorder.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/reorder.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/shapefile.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/shapefile.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/transform.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/transform.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/units.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/units.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/upright.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/upright.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/urecord.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/urecord.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/version.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/version.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/xref.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/xref.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/zoom.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/zoom.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/_options.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/_options.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/__main__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/__main__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/bezier3p.pyx
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/bezier3p.pyx
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/bezier4p.pyx
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/bezier4p.pyx
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/bspline.pyx
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/bspline.pyx
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/construct.pxd
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/construct.pxd
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/construct.pyx
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/construct.pyx
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/linetypes.pyx
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/linetypes.pyx
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/mapbox_earcut.pyx
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/mapbox_earcut.pyx
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/matrix44.pxd
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/matrix44.pxd
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/matrix44.pyx
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/matrix44.pyx
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/vector.pxd
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/vector.pxd
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/vector.pyx
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/vector.pyx
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.cpp
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.hpp
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.pxd
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_vec3.hpp
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_vec3.hpp
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_vec3.pxd
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_vec3.pxd
+Filename: ezdxf-1.1.0b0/src/ezdxf/acc/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acc/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/acis/abstract.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acis/abstract.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/acis/api.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acis/api.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/acis/const.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acis/const.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/acis/dbg.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acis/dbg.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/acis/dxf.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acis/dxf.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/acis/entities.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acis/entities.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/acis/hdr.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acis/hdr.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/acis/mesh.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acis/mesh.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/acis/sab.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acis/sab.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/acis/sat.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acis/sat.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/acis/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/acis/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/acadctb.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/acadctb.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/binpacking.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/binpacking.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dimlines.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dimlines.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dxf2code.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dxf2code.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/genetic_algorithm.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/geo.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/geo.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/gerber_D6673.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/gerber_D6673.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/importer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/importer.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/iterdxf.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/iterdxf.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/menger_sponge.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/meshex.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/meshex.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/mixins.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/mixins.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/mtextsurrogate.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/mtextsurrogate.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/mtxpl.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/mtxpl.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/odafc.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/odafc.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/openscad.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/openscad.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/pycsg.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/pycsg.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/r12export.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/r12export.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/r12writer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/r12writer.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/sierpinski_pyramid.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/sierpinski_pyramid.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/tablepainter.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/tablepainter.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/text2path.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/text2path.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/xqt.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/xqt.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/browser.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/browser.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/data.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/data.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/bookmarks.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/bookmarks.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/browser.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/browser.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/data.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/data.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/find_dialog.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/find_dialog.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/loader.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/loader.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/model.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/model.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/tags.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/tags.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/views.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/views.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/browser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/browser/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/backend.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/backend.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/clipper.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/config.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/config.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/debug_backend.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/debug_backend.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/debug_utils.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/debug_utils.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/frontend.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/frontend.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/gfxproxy.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/gfxproxy.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/matplotlib.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/matplotlib.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/mpl_text_renderer.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/mtext_complex.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/mtext_complex.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/properties.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/pillow.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/pyqt.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/properties.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/qtviewer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/pyqt.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/text.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/qtviewer.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/qt_text_renderer.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/type_hints.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/text.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/unified_text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/text_renderer.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/drawing/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/type_hints.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/classes_section.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/drawing/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/const.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/classes_section.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/crc.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/const.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/fileheader.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/crc.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/header_section.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/fileheader.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/loader.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/header_section.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/dwg/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/loader.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/api.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/dwg/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/backend.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/api.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/compiler.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/backend.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/deps.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/compiler.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/dxf_backend.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/deps.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/interpreter.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/dxf_backend.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/page.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/interpreter.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/pdf_backend.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/page.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/plotter.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/pdf_backend.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/polygon_buffer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/plotter.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/properties.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/polygon_buffer.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/svg_backend.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/properties.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/tokenizer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/svg_backend.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/tokenizer.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/acad_table.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/acad_proxy_entity.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/acis.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/acad_table.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/appdata.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/acis.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/appid.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/appdata.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/arc.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/appid.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/attrib.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/arc.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/block.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/attrib.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/blockrecord.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/block.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/blockrecord.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/circle.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/boundary_paths.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dictionary.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/circle.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dictionary.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dimstyle.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dimension.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dimstyleoverride.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dimstyle.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dimstyleoverride.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dxfclass.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dxfentity.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dxfgfx.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dxfns.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dxfgroups.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dxfns.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/dxfobj.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/factory.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/ellipse.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/geodata.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/factory.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/gradient.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/geodata.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/hatch.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/gradient.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/helix.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/hatch.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/idbuffer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/helix.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/image.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/idbuffer.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/insert.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/image.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/layer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/insert.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/layout.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/layer.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/leader.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/layout.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/light.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/leader.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/line.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/light.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/ltype.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/line.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/lwpolyline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/ltype.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/material.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/lwpolyline.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/mesh.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/material.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/mleader.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/mesh.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/mline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/mleader.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/mline.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/mtext.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/mpolygon.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/mtext.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/objectcollection.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/mtext_columns.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/oleframe.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/objectcollection.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/pattern.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/oleframe.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/point.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/pattern.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/polygon.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/point.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/polyline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/polygon.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/shape.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/polyline.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/solid.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/shape.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/spline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/solid.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/subentity.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/spline.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/sun.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/subentity.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/table.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/sun.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/text.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/table.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/textstyle.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/text.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/tolerance.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/textstyle.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/ucs.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/tolerance.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/underlay.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/ucs.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/view.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/underlay.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/viewport.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/view.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/visualstyle.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/viewport.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/vport.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/visualstyle.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/xdata.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/vport.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/xdict.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/xdata.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/xline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/xdict.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/entities/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/xline.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/layouts/base.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/entities/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/layouts/blocklayout.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/layouts/base.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/layouts/layout.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/layouts/blocklayout.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/layouts/layouts.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/layouts/layout.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/layouts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/layouts/layouts.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/attributes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/layouts/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/const.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/attributes.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/encoding.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/const.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/extendedtags.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/encoding.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/fileindex.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/extendedtags.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/hdrvars.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/fileindex.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/loader.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/hdrvars.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/packedtags.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/loader.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/repair.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/packedtags.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/tagger.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/repair.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/tags.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/tagger.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/tagwriter.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/tags.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/types.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/tagwriter.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/validator.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/types.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/lldxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/validator.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/arc.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/lldxf/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/bbox.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/arc.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/bezier.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/bbox.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/bezier_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/bezier.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/box.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/bezier_interpolation.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/bspline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/box.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/bulge.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/bspline.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/circle.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/bulge.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/clipping.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/circle.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/clustering.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/clipping.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/construct2d.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/clustering.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/construct3d.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/construct2d.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/cspline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/construct3d.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/curvetools.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/cspline.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/curvetools.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/eulerspiral.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/ellipse.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/linalg.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/eulerspiral.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/line.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/linalg.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/offset2d.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/line.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/parametrize.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/offset2d.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/perlin.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/parametrize.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/polyline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/perlin.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/rtree.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/polyline.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/shape.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/rtree.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/surfaces.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/shape.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/transformtools.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/surfaces.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/triangulation.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/transformtools.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/ucs.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/triangulation.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/ucs.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/_bezier3p.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/_bspline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/_bezier4p.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/_construct.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/_bspline.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/_ctypes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/_construct.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/_ctypes.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/_mapbox_earcut.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/_vector.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/_matrix44.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/math/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/_vector.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/path/commands.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/math/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/path/converter.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/path/commands.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/path/nesting.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/path/converter.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/path/path.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/path/nesting.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/path/shapes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/path/path.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/path/tools.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/path/shapes.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/path/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/path/tools.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.css
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/path/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.html
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.css
+Filename: ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.js
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.html
+Filename: ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.js
+Filename: ezdxf-1.1.0b0/src/ezdxf/pp/pprint.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.css
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/pp/pprint.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.html
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.css
+Filename: ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.html
+Filename: ezdxf-1.1.0b0/src/ezdxf/pp/reflinks.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/pp/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/pp/reflinks.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/abstract_mtext_renderer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/pp/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/arrows.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/abstract_mtext_renderer.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/curves.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/arrows.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/curves.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/dim_base.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/dimension.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/dim_curved.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/dim_base.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/dim_diameter.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/dim_curved.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/dim_linear.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/dim_diameter.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/dim_ordinate.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/dim_linear.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/dim_radius.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/dim_ordinate.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/forms.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/dim_radius.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/hatching.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/forms.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/leader.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/hatching.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/linetypes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/leader.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/mesh.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/linetypes.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/mleader.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/mesh.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/mline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/mleader.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/point.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/mline.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/polyline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/point.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/r12spline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/polyline.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/trace.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/r12spline.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/_linetypes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/trace.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/render/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/_linetypes.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/16x16.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/render/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/24x24.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/16x16.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/256x256.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/24x24.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/32x32.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/256x256.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/48x48.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/32x32.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/64x64.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/48x48.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-copy-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/64x64.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-find-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-copy-64px.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-find-64px.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-handle-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-bookmark-64px.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-line-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-handle-64px.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-left-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-line-64px.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-next-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-left-arrow-64px.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-prev-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-next-entity-64px.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-right-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-prev-entity-64px.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-show-in-tree-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-right-arrow-64px.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/resources/icon-store-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-show-in-tree-64px.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/sections/acdsdata.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/resources/icon-store-bookmark-64px.png
+Filename: ezdxf-1.1.0b0/src/ezdxf/sections/blocks.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/sections/acdsdata.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/sections/classes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/sections/blocks.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/sections/entities.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/sections/classes.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/sections/header.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/sections/entities.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/sections/headervars.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/sections/header.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/sections/objects.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/sections/headervars.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/sections/table.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/sections/objects.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/sections/tables.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/sections/table.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/sections/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/sections/tables.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/analyze.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/sections/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/binarydata.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/analyze.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/codepage.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/binarydata.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/complex_ltype.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/codepage.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/crypt.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/complex_ltype.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/debug.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/crypt.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/difftags.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/debug.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/fonts.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/difftags.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/font_face.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/fonts.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/font_manager.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/font_face_cache.json
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/handle.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/font_measurement_cache.json
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/indexing.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/handle.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/juliandate.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/indexing.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/pattern.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/juliandate.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/rawloader.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/pattern.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/standards.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/rawloader.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/strip.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/standards.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/test.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/strip.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/text.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/test.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/text_layout.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/text.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/text_size.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/text_layout.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/ttfonts.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/text_size.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/zipmanager.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/zipmanager.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/_iso_pattern.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/_iso_pattern.py
+Filename: ezdxf-1.1.0b0/src/ezdxf/tools/__init__.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/_matplotlib_font_support.py
+Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf/tools/__init__.py
+Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/entry_points.txt
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/dependency_links.txt
+Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/not-zip-safe
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/entry_points.txt
+Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/not-zip-safe
+Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/requires.txt
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/PKG-INFO
+Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/requires.txt
+Filename: ezdxf-1.1.0b0/src/ezdxf.egg-info/top_level.txt
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/SOURCES.txt
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/src/ezdxf.egg-info/top_level.txt
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/
+Filename: ezdxf-1.1.0b0/tests/test_06_math/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/
+Filename: ezdxf-1.1.0b0/tests/test_07_render/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/
+Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/
+Filename: ezdxf-1.1.0b0/tests/test_10_issues/
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/
+Filename: ezdxf-1.1.0b0/tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_10_issues/
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_011_codepage.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_018_handle.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_018_handle.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_040_tags.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_040_tags.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+Filename: ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_102_appdata.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_102_appdata.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_103_reactors.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_103_reactors.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_104_extension_dict.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_104_extension_dict.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_105_xdata.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_105_xdata.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_110_dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_110_dxfentity.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_112b_dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_112b_dxfobj.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_113_dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_113_dxfclass.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_114_factory.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_114_factory.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_116_dictionary.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_116_dictionary.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_118_appid_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_120_style_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_120_style_table_entry.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_122_vport_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_123_view_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_123_view_table_entry.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_125_image_def.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_125_image_def.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_127_raster_variables.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_127_raster_variables.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_128_pdf_definition.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_128_pdf_definition.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_129_xrecord.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_129_xrecord.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_130_id_buffer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_130_id_buffer.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_131_field_list.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_131_field_list.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_132_layer_filter.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_132_layer_filter.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_133_sun.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_133_sun.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_134_material.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_134_material.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_135_geo_data.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_135_geo_data.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_136_vba_project.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_136_vba_project.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_137_sortentstable.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_137_sortentstable.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_139_user_record.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_139_user_record.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_140_block_record.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_140_block_record.py
+Filename: ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/conftest.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/conftest.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_200_line.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_200_line.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_201_point.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_201_point.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_202_circle.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_202_circle.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_203_arc.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_203_arc.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_204_shape.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_204_shape.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_205_solid.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_205_solid.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_206_text.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_206_text.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_207_attdef.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_207_attdef.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_208_attrib.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_208_attrib.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_209_vertex.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_209_vertex.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_1.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_1.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_2.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_2.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_211_viewport.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_211_viewport.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_212_insert.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_212_insert.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_213_minsert.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_213_minsert.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_214_block.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_214_block.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_215_dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_215_dimension.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_221_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_221_ellipse.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_222_xline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_222_xline.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_223_ray.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_223_ray.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_224_group.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_224_group.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_225_mtext.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_225_mtext.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_226_spline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_226_spline.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_228_mesh.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_228_mesh.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_231_underlay.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_231_underlay.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_231_underlay_2.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_231_underlay_2.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_acis.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_acis.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_acis_2.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_acis_2.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_surface.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_surface.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_233_helix.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_233_helix.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_234_light.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_234_light.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_235_leader.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_235_leader.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_236_multileader.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_236_multileader.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_237_mline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_237_mline.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_238_tolerance.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_238_tolerance.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_241_hyperlink.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_241_hyperlink.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_242_random_transform.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_242_random_transform.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_243_replace_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_243_replace_entity.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_245_wipeout.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_245_wipeout.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_246_spline_audit.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_246_spline_audit.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_248_mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_248_mpolygon.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_251_upright.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_251_upright.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_253_ole2frame.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_253_ole2frame.py
+Filename: ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_254_get_font_name.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_254_get_font_name.py
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_300_layout.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_300_layout.py
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_302_block_references.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_302_block_references.py
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_307_groupby.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_307_groupby.py
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_308_query.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_308_query.py
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_309_query_parser.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_309_query_parser.py
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+Filename: ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_313_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_313_redraw_order.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_405_classes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_405_classes.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_410_table.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_410_table.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_424_audit.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_424_audit.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+Filename: ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/conftest.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/conftest.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_500_units.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_500_units.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_501_truecolor.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_501_truecolor.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_502_raw_color.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_502_raw_color.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_503_indexing.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_503_indexing.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_504_suppress_zeros.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_504_suppress_zeros.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_506_version.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_506_version.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_507_dxf_pretty_printer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_507_dxf_pretty_printer.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_508_read_zip.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_508_read_zip.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_509_comments.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_509_comments.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_510_byte_stream.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_510_byte_stream.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_511_bit_stream.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_511_bit_stream.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_512_pattern.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_512_pattern.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_513_reorder_entities.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_513_reorder_entities.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_514_text.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_514_text.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_515_fonts.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_515_fonts.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_516_zoom.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_516_zoom.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_517_text_layout.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_517_text_layout.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_518_header_guid.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_518_header_guid.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_519_mtext_editor.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_519_mtext_editor.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_520_mtext_context.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_520_mtext_context.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_521_mtext_parser.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_521_mtext_parser.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_522_text_scanner.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_522_text_scanner.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_523_text_size.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_523_text_size.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_524_block_reference_manager.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_524_block_reference_manager.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_525_transparency.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_525_transparency.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_526_explode.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_526_explode.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_527_gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_527_gfxattribs.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_528_difftags.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_528_difftags.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_529_acis_sat.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_529_acis_sat.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_530_acis_sab.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_530_acis_sab.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_531_acis_entities.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_531_acis_entities.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_532_acis_mesh.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_532_acis_mesh.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_533_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_533_shapefiles.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_534_dwg_info.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_534_dwg_info.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_535_xref_basic.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_535_xref_basic.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_536_xref_conflict.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_536_xref_conflict.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_537_transform.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_537_transform.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+Filename: ezdxf-1.1.0b0/tests/test_05_tools/test_539_npshapes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/conftest.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/conftest.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_600_base.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_600_base.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_601_bulge.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_601_bulge.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_602_vec3.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_602_vec3.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_603_vec2.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_603_vec2.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_604_banded_matrix.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_604_banded_matrix.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_604_linalg.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_604_linalg.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_605_matrix44.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_605_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_606_convexhull.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_606_convexhull.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_607_perlin_noise.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_607_perlin_noise.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_608_intersection_line_line_2d.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_608_intersection_line_line_2d.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_609_point_on_line.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_609_point_on_line.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_610_ocs.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_610_ocs.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_611_ucs.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_611_ucs.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_612_ucs_pass_trough.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_612_ucs_pass_trough.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_613_point_in_poygon.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_613_point_in_poygon.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_614_construct_3d.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_614_construct_3d.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_615_rytz_axis.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_615_rytz_axis.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_616_plane.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_616_plane.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_617_clockwise_orientation.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_617_clockwise_orientation.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_618_clipping.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_618_clipping.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_619_greiner_hormann.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_619_greiner_hormann.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_620_knot.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_620_knot.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_621_bspline.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_621_bspline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_622_bsplineu.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_622_bsplineu.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_623_rbspline.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_623_rbspline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_624_global_bspline_interpolation.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_624_global_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_626_local_bspline_interpolation.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_626_local_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_627_bspline_basis.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_627_bspline_basis.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_629_bezier.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_629_bezier.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_630a_bezier4p_base.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_630a_bezier4p_base.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_630b_bezier4p_functions.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_630b_bezier4p_functions.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_631_euler_spiral.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_631_euler_spiral.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_632_bezier3p.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_632_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_640_bbox.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_640_bbox.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_641_construction_ray.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_641_construction_ray.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_642_construction_line.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_642_construction_line.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_643_construction_box.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_643_construction_box.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_644_construction_circle.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_644_construction_circle.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_645_construction_arc.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_645_construction_arc.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_646_offset_vertices_2d.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_646_offset_vertices_2d.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_647_transform_tools.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_647_transform_tools.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_648_construction_ellipse.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_648_construction_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_649_nurbs_python_interface.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_650_elliptic_arc_span.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_650_elliptic_arc_span.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_651_construction_polyline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_651_construction_polyline.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_652_approx_param_t.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_652_approx_param_t.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_653_polyline_intersection.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_653_polyline_intersection.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_654_rtree.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_654_rtree.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_655_dbscan.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_655_dbscan.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_656_k_means.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_656_k_means.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_657_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_657_mapbox_earcut.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_658_bevel_tools.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_658_bevel_tools.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+Filename: ezdxf-1.1.0b0/tests/test_06_math/test_662_is_convex_polygon_2d.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_06_math/test_662_is_convex_polygon_2d.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_701_arrows.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_701_arrows.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_702_render_forms.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_702_render_forms.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_703_mesh_builder.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_703_mesh_builder.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_704_render_linear_dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_704_render_linear_dimension.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_705_shape.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_705_shape.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_706_random_path.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_706_random_path.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_707_trace.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_707_trace.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_708a_path.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_708a_path.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_708b_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_708b_path_tools.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_708c_matplotlib_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_708c_matplotlib_path_tools.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_708d_qpainter_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_708d_qpainter_path_tools.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_708e_path_shapes.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_708e_path_shapes.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_708f_path_nesting.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_708f_path_nesting.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_709_linetype_renderer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_709_linetype_renderer.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_711_points.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_711_points.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_712_render_curved_dimension.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_712_render_curved_dimension.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_713_mleader_builder.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_713_mleader_builder.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_714_mleader_render_engine.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_714_mleader_render_engine.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_715_hatching.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_715_hatching.py
+Filename: ezdxf-1.1.0b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_800_mtext_surrogate.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_800_mtext_surrogate.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_801_r12spline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_801_r12spline.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_802_table_painter.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_802_table_painter.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_803_entities_to_code.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_803_entities_to_code.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_804_importer.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_804_importer.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_805_pycsg.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_805_pycsg.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_806_acadctb.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_806_acadctb.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_807_dwg_loader_basics.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_807_dwg_loader_basics.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_810_drawing_properties.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_810_drawing_properties.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_811_drawing_frontend.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_811_drawing_frontend.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_813_geo_interface.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_813_geo_interface.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_814_text2path.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_814_text2path.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_815_dxf_browser.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_815_dxf_browser.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_816_bin_packing.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_816_bin_packing.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_817_genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_817_genetic_algorithm.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_818_meshex.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_818_meshex.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_819_menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_819_menger_sponge.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_820_openscad.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_820_openscad.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_821_hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_821_hpgl2.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+Filename: ezdxf-1.1.0b0/tests/test_08_addons/test_822_clipper.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Filename: ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Filename: ezdxf-1.1.0b0/tests/test_10_issues/test_issue_414_bbox_calculation.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Filename: ezdxf-1.1.0b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_10_issues/test_issue_574_flattening_error.py
+Filename: ezdxf-1.1.0b0/tests/test_10_issues/test_issue_574_flattening_error.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Filename: ezdxf-1.1.0b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
 Comment: 
 
-Filename: ezdxf-1.0.4b1/tests/test_10_issues/test_issue_749_text_layout.py
+Filename: ezdxf-1.1.0b0/tests/test_10_issues/test_issue_749_text_layout.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ezdxf-1.0.4b1/LICENSE` & `ezdxf-1.1.0b0/LICENSE`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/NEWS.md` & `ezdxf-1.1.0b0/NEWS.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,42 @@
 
 News
 ====
 
-Version 1.0.4b1 - dev
+Version 1.1.0b0 - dev
 ---------------------
 
-- Release notes: https://ezdxf.mozman.at/release-v1-0.html
+- Release notes: https://ezdxf.mozman.at/release-v1-1.html
+- WARNING: The font support changed drastically in this version, if you use the 
+  `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
+  v1.0.3 in your `requirements.txt` file to use the previous version!
+- NEW: `numpy` is a hard dependency, requires Python version >= 3.8
+- NEW: `fontTools` is a hard dependency
+- NEW: `Matrix44.Path2d()` class, `Path` class with `Vec2` vertices
+- NEW: optimized `Matrix44.fast_2d_transform()` method
 - NEW: added setter to `BlockLayout.base_point` property
+- NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
+- NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG
+- NEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF
+- NEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG
+- NEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF
+- CHANGED: refactoring of `ezdxf.tools.fonts`
+- CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
+  renamed to `width` and is also an int value (1-9) now
+- REMOVED: replaced `matplotlib` font support module by `fontTools`
+- REMOVED: configuration option `use_matplotlib`
+- CHANGED: text rendering for the `drawing` add-on and text measurement is done by the
+  `fontTools` package
+- CHANGED: moved text rendering from backend classes to the `Frontend` class
+- CHANGED: moved clipping support from backend classes to the `Frontend` class
+- REMOVED: `PillowBackend` and the `pillow` command
+- REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
 - BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
   scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
-- PREVIEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG,  
-  final release in v1.1
-- PREVIEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF, final release in v1.1
-- PREVIEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG, final release in v1.1
-- PREVIEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF, final release in v1.1
 
 Version 1.0.3 - 2023-03-26
 --------------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: [#833](https://github.com/mozman/ezdxf/issues/833)
   logging non-unique entity handles when loading a DXF document as warnings, auditing
```

## Comparing `ezdxf-1.0.4b1/PKG-INFO` & `ezdxf-1.1.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.0.4b1
+Version: 1.1.0b0
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides: ezdxf
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: draw
 Provides-Extra: draw5
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
 Provides-Extra: all5
@@ -51,21 +50,23 @@
 Quick-Info
 ----------
 
 - *ezdxf* is a Python package to create new DXF files and read/modify/write 
   existing DXF documents
 - MIT-License
 - the intended audience are programmers
-- requires at least Python 3.7
+- requires at least Python 3.8
 - OS independent
 - tested with CPython and pypy3
 - has type annotations and passes `mypy --ignore-missing-imports -p ezdxf` successful
 - additional required packages for the core package without add-ons: 
   [typing_extensions](https://pypi.org/project/typing-extensions/), 
-  [pyparsing](https://pypi.org/project/pyparsing/) 
+  [pyparsing](https://pypi.org/project/pyparsing/),
+  [numpy](https://pypi.org/project/numpy/),
+  [fontTools](https://pypi.org/project/fonttools/)
 - read/write/new support for DXF versions: R12, R2000, R2004, R2007, R2010, R2013 and R2018
 - additional read-only support for DXF versions R13/R14 (upgraded to R2000)
 - additional read-only support for older DXF versions than R12 (upgraded to R12)
 - read/write support for ASCII DXF and Binary DXF
 - retains third-party DXF content
 - optional C-extensions for CPython are included in the binary wheels, available 
   on [PyPI](https://pypi.org/project/ezdxf/) for Windows, Linux and macOS
@@ -210,27 +211,45 @@
 Feedback is greatly appreciated.
 
 Manfred
 
 News
 ====
 
-Version 1.0.4b1 - dev
+Version 1.1.0b0 - dev
 ---------------------
 
-- Release notes: https://ezdxf.mozman.at/release-v1-0.html
+- Release notes: https://ezdxf.mozman.at/release-v1-1.html
+- WARNING: The font support changed drastically in this version, if you use the 
+  `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
+  v1.0.3 in your `requirements.txt` file to use the previous version!
+- NEW: `numpy` is a hard dependency, requires Python version >= 3.8
+- NEW: `fontTools` is a hard dependency
+- NEW: `Matrix44.Path2d()` class, `Path` class with `Vec2` vertices
+- NEW: optimized `Matrix44.fast_2d_transform()` method
 - NEW: added setter to `BlockLayout.base_point` property
+- NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
+- NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG
+- NEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF
+- NEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG
+- NEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF
+- CHANGED: refactoring of `ezdxf.tools.fonts`
+- CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
+  renamed to `width` and is also an int value (1-9) now
+- REMOVED: replaced `matplotlib` font support module by `fontTools`
+- REMOVED: configuration option `use_matplotlib`
+- CHANGED: text rendering for the `drawing` add-on and text measurement is done by the
+  `fontTools` package
+- CHANGED: moved text rendering from backend classes to the `Frontend` class
+- CHANGED: moved clipping support from backend classes to the `Frontend` class
+- REMOVED: `PillowBackend` and the `pillow` command
+- REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
 - BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
   scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
-- PREVIEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG,  
-  final release in v1.1
-- PREVIEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF, final release in v1.1
-- PREVIEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG, final release in v1.1
-- PREVIEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF, final release in v1.1
 
 Version 1.0.3 - 2023-03-26
 --------------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: [#833](https://github.com/mozman/ezdxf/issues/833)
   logging non-unique entity handles when loading a DXF document as warnings, auditing
```

## Comparing `ezdxf-1.0.4b1/README.md` & `ezdxf-1.1.0b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 Quick-Info
 ----------
 
 - *ezdxf* is a Python package to create new DXF files and read/modify/write 
   existing DXF documents
 - MIT-License
 - the intended audience are programmers
-- requires at least Python 3.7
+- requires at least Python 3.8
 - OS independent
 - tested with CPython and pypy3
 - has type annotations and passes `mypy --ignore-missing-imports -p ezdxf` successful
 - additional required packages for the core package without add-ons: 
   [typing_extensions](https://pypi.org/project/typing-extensions/), 
-  [pyparsing](https://pypi.org/project/pyparsing/) 
+  [pyparsing](https://pypi.org/project/pyparsing/),
+  [numpy](https://pypi.org/project/numpy/),
+  [fontTools](https://pypi.org/project/fonttools/)
 - read/write/new support for DXF versions: R12, R2000, R2004, R2007, R2010, R2013 and R2018
 - additional read-only support for DXF versions R13/R14 (upgraded to R2000)
 - additional read-only support for older DXF versions than R12 (upgraded to R12)
 - read/write support for ASCII DXF and Binary DXF
 - retains third-party DXF content
 - optional C-extensions for CPython are included in the binary wheels, available 
   on [PyPI](https://pypi.org/project/ezdxf/) for Windows, Linux and macOS
```

## Comparing `ezdxf-1.0.4b1/setup.py` & `ezdxf-1.1.0b0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python3
-# Copyright (c) 2011-2021 Manfred Moitzi
+# Copyright (c) 2011-2023 Manfred Moitzi
 # License: MIT License
 import os
 import sys
 from setuptools import setup, find_packages
 from setuptools import Extension
 
 # setuptools docs: https://setuptools.readthedocs.io/en/latest/setuptools.html
@@ -117,53 +117,51 @@
     try:
         with open(os.path.join(os.path.dirname(__file__), fname)) as f:
             return read_until(f.readlines()) if until else f.read()
     except IOError:
         return "File '%s' not found.\n" % fname
 
 
-DRAW = ["matplotlib", "PySide6", "Pillow", "PyMuPDF"]
-DRAW5 = ["matplotlib", "PyQt5", "Pillow", "PyMuPDF"]
-TEST = ["pytest", "geomdl"]
+DRAW = ["matplotlib", "PySide6", "PyMuPDF"]
+DRAW5 = ["matplotlib", "PyQt5", "PyMuPDF"]
+TEST = ["pytest"]
 DEV = ["setuptools", "wheel", "Cython"]
 
 setup(
     name="ezdxf",
     version=get_version(),
     description="A Python package to create/manipulate DXF drawings.",
     author="Manfred Moitzi",
     url="https://ezdxf.mozman.at",
     download_url="https://pypi.org/project/ezdxf/",
     author_email="me@mozman.at",
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     package_dir={"": "src"},
     packages=find_packages("src"),
     zip_safe=False,
     package_data={
         "ezdxf": [
             "pp/*.html",
             "pp/*.js",
             "pp/*.css",
-            "tools/font_face_cache.json",
-            "tools/font_measurement_cache.json",
             "resources/*.png",
             "py.typed",
         ]
     },
     entry_points={
         "console_scripts": [
             "ezdxf = ezdxf.__main__:main",  # ezdxf launcher
         ]
     },
     provides=["ezdxf"],
     cmdclass=commands,
     ext_modules=ext_modules,
-    install_requires=["pyparsing>=2.0.1", "typing_extensions"],
+    install_requires=["pyparsing>=2.0.1", "typing_extensions", "numpy", "fonttools"],
     setup_requires=["wheel"],
-    tests_require=["pytest", "geomdl"],
+    tests_require=["pytest"],
     extras_require={
         "draw": DRAW,
         "draw5": DRAW5,
         "test": TEST,
         "dev": DEV + TEST,
         "all": DRAW + DEV + TEST,
         "all5": DRAW5 + DEV + TEST,
@@ -175,15 +173,14 @@
     platforms="OS Independent",
     license="MIT License",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Intended Audience :: Developers",
```

## Comparing `ezdxf-1.0.4b1/integration_tests/check_disable_c_ext_by_config_file.py` & `ezdxf-1.1.0b0/integration_tests/check_disable_c_ext_by_config_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/check_disable_c_ext_by_env_var.py` & `ezdxf-1.1.0b0/integration_tests/check_disable_c_ext_by_env_var.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_acad_table.py` & `ezdxf-1.1.0b0/integration_tests/test_acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_all_dimline_styles.py` & `ezdxf-1.1.0b0/integration_tests/test_all_dimline_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_all_ellipse_transformations.py` & `ezdxf-1.1.0b0/integration_tests/test_all_ellipse_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_anonymous_blocks.py` & `ezdxf-1.1.0b0/integration_tests/test_anonymous_blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_audit_critical_dxf_files.py` & `ezdxf-1.1.0b0/integration_tests/test_audit_critical_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_audit_layouts.py` & `ezdxf-1.1.0b0/integration_tests/test_audit_layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_complex_line_type_2.py` & `ezdxf-1.1.0b0/integration_tests/test_complex_line_type_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_create_basic_graphics.py` & `ezdxf-1.1.0b0/integration_tests/test_create_basic_graphics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_document_guid.py` & `ezdxf-1.1.0b0/integration_tests/test_document_guid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_document_page_setup.py` & `ezdxf-1.1.0b0/integration_tests/test_document_page_setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_dxf_info_scanning.py` & `ezdxf-1.1.0b0/integration_tests/test_dxf_info_scanning.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_entities_iterator.py` & `ezdxf-1.1.0b0/integration_tests/test_entities_iterator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_fix_dulicate_handles.py` & `ezdxf-1.1.0b0/integration_tests/test_fix_dulicate_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_geo.py` & `ezdxf-1.1.0b0/integration_tests/test_geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_groups.py` & `ezdxf-1.1.0b0/integration_tests/test_groups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_ignore_junk_beyond_EOF.py` & `ezdxf-1.1.0b0/integration_tests/test_ignore_junk_beyond_EOF.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_launcher.py` & `ezdxf-1.1.0b0/integration_tests/test_launcher.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_leica_disto_r12.py` & `ezdxf-1.1.0b0/integration_tests/test_leica_disto_r12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_load_dxf_unicode_notation.py` & `ezdxf-1.1.0b0/integration_tests/test_load_dxf_unicode_notation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_mapbox_earcut.py` & `ezdxf-1.1.0b0/integration_tests/test_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_mtext_columns.py` & `ezdxf-1.1.0b0/integration_tests/test_mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_mtext_explode_addon.py` & `ezdxf-1.1.0b0/integration_tests/test_mtext_explode_addon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #  Copyright (c) 2021, Manfred Moitzi
 #  License: MIT License
+import pytest
 import ezdxf
 from ezdxf.addons import MTextExplode
 
 LOREM_IPSUM = (
     r"Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam "
     r"nonumy eirmod tempor {\C1invidunt ut labore} et dolore mag{\C3na al}iquyam "
     r"erat, sed {\C5diam voluptua.} At vero eos et accusam et justo duo dolores "
@@ -46,21 +47,21 @@
 def test_created_text_styles_exists():
     from ezdxf.tools.text import MTextEditor
 
     doc = ezdxf.new()
     msp = doc.modelspace()
     editor = MTextEditor()
     editor.append("LINE0\n")
-    editor.font("Arial")
+    editor.font("Open Sans")
     editor.append("LINE1")
     mtext = msp.add_mtext(editor.text)
     with MTextExplode(msp) as xpl:
         xpl.explode(mtext)
-    assert doc.styles.has_entry("MtXpl_Arial")
-    assert doc.styles.has_entry("MtXpl_Txt")
+    assert doc.styles.has_entry("MtXpl_DejaVu Sans Condensed")  # default font
+    assert doc.styles.has_entry("MtXpl_Open Sans")  # MTEXT inline set font
 
 
 def test_addon_is_still_working():
     # Testing only the basic functionality!
     # The text layout engine has its own test suite in test file 517!
     # The MTextParser has its own test suite in test file 521!
     doc = new_doc(LEFT + CENTER + RIGHT + JUSTIFIED)
```

## Comparing `ezdxf-1.0.4b1/integration_tests/test_mtext_text_frame.py` & `ezdxf-1.1.0b0/integration_tests/test_mtext_text_frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_new_table_entries.py` & `ezdxf-1.1.0b0/integration_tests/test_new_table_entries.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_none_ascii_read_write.py` & `ezdxf-1.1.0b0/integration_tests/test_none_ascii_read_write.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_odafc.py` & `ezdxf-1.1.0b0/integration_tests/test_odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_open_binary_DXF_files.py` & `ezdxf-1.1.0b0/integration_tests/test_open_binary_DXF_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_open_coord_order_issue.py` & `ezdxf-1.1.0b0/integration_tests/test_open_coord_order_issue.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_open_exotic_dxf_files.py` & `ezdxf-1.1.0b0/integration_tests/test_open_exotic_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_open_R13_R14.py` & `ezdxf-1.1.0b0/integration_tests/test_open_R13_R14.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_polyline_entity.py` & `ezdxf-1.1.0b0/integration_tests/test_polyline_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_preserve_binary_data_in_xrecords.py` & `ezdxf-1.1.0b0/integration_tests/test_preserve_binary_data_in_xrecords.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_r12export.py` & `ezdxf-1.1.0b0/integration_tests/test_r12export.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     assert isinstance(polyline, ents.Polyline)
     assert polyline.is_3d_polyline is True
     assert len(polyline.vertices) > 10
     assert polyline.dxf.layer == "EZDXF"
     assert polyline.dxf.color == 144
 
 
+
 def test_export_proxy_graphic():
     from ezdxf.lldxf.tags import Tags
     from ezdxf.proxygraphic import load_proxy_graphic
 
     doc = ezdxf.new("R2018")
     msp = doc.modelspace()
     proxy_entity = ents.ACADProxyEntity.new()
@@ -111,25 +112,25 @@
 
 
 def test_export_mtext():
     doc = ezdxf.new("R2018")
     msp = doc.modelspace()
     editor = MTextEditor()
     editor.append("LINE0\n")
-    editor.font("Arial")
+    editor.font("Open Sans")
     editor.append("LINE1")
     msp.add_mtext(editor.text, dxfattribs=DXFATTRIBS)
 
     doc_r12 = r12export.convert(doc)
     text0, text1 = doc_r12.modelspace()
 
     assert text0.dxf.text == "LINE0"
     assert text1.dxf.text == "LINE1"
-    assert doc_r12.styles.has_entry("MTXPL_ARIAL")
-    assert doc_r12.styles.has_entry("MTXPL_TXT")
+    assert doc_r12.styles.has_entry("MTXPL_OPEN_SANS")
+    assert doc_r12.styles.has_entry("MTXPL_DEJAVU_SANS_CONDENSED")  # default font for TXT
 
 
 def test_export_virtual_entities():
     doc = ezdxf.new(setup=True)
     mleaderstyle = doc.mleader_styles.duplicate_entry("Standard", "EZDXF")
     mleaderstyle.set_mtext_style("OpenSans")
     msp = doc.modelspace()
```

## Comparing `ezdxf-1.0.4b1/integration_tests/test_r12strict.py` & `ezdxf-1.1.0b0/integration_tests/test_r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_r12writer.py` & `ezdxf-1.1.0b0/integration_tests/test_r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_read_file_without_handles.py` & `ezdxf-1.1.0b0/integration_tests/test_read_file_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_read_write_modern_entites.py` & `ezdxf-1.1.0b0/integration_tests/test_read_write_modern_entites.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_recover.py` & `ezdxf-1.1.0b0/integration_tests/test_recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_redraw_order.py` & `ezdxf-1.1.0b0/integration_tests/test_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_rotated_block_attributes.py` & `ezdxf-1.1.0b0/integration_tests/test_rotated_block_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_surface_entities.py` & `ezdxf-1.1.0b0/integration_tests/test_surface_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_write_fixed_meta_data.py` & `ezdxf-1.1.0b0/integration_tests/test_write_fixed_meta_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_write_without_handles.py` & `ezdxf-1.1.0b0/integration_tests/test_write_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/test_xref_detach.py` & `ezdxf-1.1.0b0/integration_tests/test_xref_detach.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/AC1003_LINE_Example.dxf` & `ezdxf-1.1.0b0/integration_tests/data/AC1003_LINE_Example.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/acad_table_with_blk_ref.dxf` & `ezdxf-1.1.0b0/integration_tests/data/acad_table_with_blk_ref.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/ASCII_R12.dxf` & `ezdxf-1.1.0b0/integration_tests/data/ASCII_R12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r12.dxf` & `ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r13.dxf` & `ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r14.dxf` & `ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/bin_dxf_r2000.dxf` & `ezdxf-1.1.0b0/integration_tests/data/bin_dxf_r2000.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/cc_dxflib.dxf` & `ezdxf-1.1.0b0/integration_tests/data/cc_dxflib.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/custom_blocks.dxf` & `ezdxf-1.1.0b0/integration_tests/data/custom_blocks.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/duplicate_handles.dxf` & `ezdxf-1.1.0b0/integration_tests/data/duplicate_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/dxf_unicode.dxf` & `ezdxf-1.1.0b0/integration_tests/data/dxf_unicode.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/empty_handles.dxf` & `ezdxf-1.1.0b0/integration_tests/data/empty_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/groups.dxf` & `ezdxf-1.1.0b0/integration_tests/data/groups.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/Leica_Disto_S910.dxf` & `ezdxf-1.1.0b0/integration_tests/data/Leica_Disto_S910.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/MODEL.dxf` & `ezdxf-1.1.0b0/integration_tests/data/MODEL.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/mtext_columns_R2007.dxf` & `ezdxf-1.1.0b0/integration_tests/data/mtext_columns_R2007.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/mtext_columns_R2018.dxf` & `ezdxf-1.1.0b0/integration_tests/data/mtext_columns_R2018.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/mtext_framed_columns.dxf` & `ezdxf-1.1.0b0/integration_tests/data/mtext_framed_columns.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/mtext_text_frame.dxf` & `ezdxf-1.1.0b0/integration_tests/data/mtext_text_frame.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/no_layouts.dxf` & `ezdxf-1.1.0b0/integration_tests/data/no_layouts.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/POLI-ALL210_12.DXF` & `ezdxf-1.1.0b0/integration_tests/data/POLI-ALL210_12.DXF`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/recover01.dxf` & `ezdxf-1.1.0b0/integration_tests/data/recover01.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/recover02.dxf` & `ezdxf-1.1.0b0/integration_tests/data/recover02.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/small_r13.dxf` & `ezdxf-1.1.0b0/integration_tests/data/small_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/small_r14.dxf` & `ezdxf-1.1.0b0/integration_tests/data/small_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/XRECORD_0.bin` & `ezdxf-1.1.0b0/integration_tests/data/XRECORD_0.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/XRECORD_1.bin` & `ezdxf-1.1.0b0/integration_tests/data/XRECORD_1.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/integration_tests/data/XRECORD_2.bin` & `ezdxf-1.1.0b0/integration_tests/data/XRECORD_2.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/appsettings.py` & `ezdxf-1.1.0b0/src/ezdxf/appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/audit.py` & `ezdxf-1.1.0b0/src/ezdxf/audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/bbox.py` & `ezdxf-1.1.0b0/src/ezdxf/bbox.py`

 * *Files 10% similar despite different names*

```diff
@@ -130,32 +130,19 @@
     fast=False,
     cache: Optional[Cache] = None,
 ) -> BoundingBox:
     """Returns a single bounding box for all given `entities`.
 
     If argument `fast` is ``True`` the calculation of Bézier curves is based on
     their control points, this may return a slightly larger bounding box.
-    The `fast` mode also uses a simpler and mostly inaccurate text size
-    calculation instead of the more precise but very slow calculation by
-    `matplotlib`.
-
-    .. hint::
-
-        The fast mode is not much faster for non-text based entities, so using
-        the slower default mode is not a big disadvantage if a more precise text
-        size calculation is important.
 
     """
-    use_matplotlib = ezdxf.options.use_matplotlib  # save current state
-    if fast:
-        ezdxf.options.use_matplotlib = False
     _extends = BoundingBox()
     for box in multi_flat(entities, fast=fast, cache=cache):
         _extends.extend(box)
-    ezdxf.options.use_matplotlib = use_matplotlib  # restore state
     return _extends
 
 
 def multi_flat(
     entities: Iterable[DXFEntity],
     *,
     fast=False,
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/blkrefs.py` & `ezdxf-1.1.0b0/src/ezdxf/blkrefs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/colors.py` & `ezdxf-1.1.0b0/src/ezdxf/colors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/commands.py` & `ezdxf-1.1.0b0/src/ezdxf/commands.py`

 * *Files 12% similar despite different names*

```diff
@@ -464,202 +464,14 @@
                 auditor,
                 layout=args.layout,
             )
         sys.exit(app.exec())
 
 
 @register
-class Pillow(Command):
-    """Launcher sub-command: pil"""
-
-    NAME = "pillow"
-
-    @staticmethod
-    def add_parser(subparsers):
-        parser = subparsers.add_parser(
-            Pillow.NAME, help="draw and convert DXF files by Pillow"
-        )
-        parser.add_argument(
-            "file",
-            metavar="FILE",
-            nargs="?",
-            help="DXF file to draw",
-        )
-        parser.add_argument(
-            "-o",
-            "--out",
-            required=False,
-            help="output filename, the filename extension defines the image format "
-            "(.png, .jpg, .tif, .bmp, ...)",
-        )
-        parser.add_argument(
-            "-l",
-            "--layout",
-            type=str,
-            default="Model",
-            help='name of the layout to draw, default is "Model"',
-        )
-        parser.add_argument(
-            "-i",
-            "--image_size",
-            type=str,
-            default="1920,1080",
-            help='image size in pixels as "width,height", default is "1920,1080", '
-            'supports also "x" as delimiter like "1920x1080". A single integer '
-            'is used for both directions e.g. "2000" defines an image size of '
-            "2000x2000. The image is centered for the smaller DXF drawing extent.",
-        )
-        parser.add_argument(
-            "-b",
-            "--background",
-            default=None,
-            help='override background color in hex format "RRGGBB" or "RRGGBBAA", '
-            'e.g. use "FFFFFF00" to get a white transparent background and a black '
-            "foreground color (ACI=7), because a light background gets a "
-            'black foreground color or vice versa  "00000000" for a black transparent '
-            "background and a white foreground color.",
-        ),
-        parser.add_argument(
-            "-r",
-            "--oversampling",
-            type=int,
-            default=2,
-            help="oversampling factor, default is 2, use 0 or 1 to disable oversampling",
-        )
-        parser.add_argument(
-            "-m",
-            "--margin",
-            type=int,
-            default=10,
-            help="minimal margin around the image in pixels, default is 10",
-        )
-        parser.add_argument(
-            "-t",
-            "--text-mode",
-            type=int,
-            choices=[0, 1, 2, 3],
-            default=2,
-            help="text mode: 0=ignore, 1=placeholder, 2=outline, 3=filled, default is 2",
-        )
-        parser.add_argument(
-            "--dpi",
-            type=int,
-            default=300,
-            help="output resolution in pixels/inch which is significant for the "
-            "linewidth, default is 300",
-        )
-        parser.add_argument(
-            "-v",
-            "--verbose",
-            action="store_true",
-            help="give more output",
-        )
-
-    @staticmethod
-    def run(args):
-        # Import on demand for a quicker startup:
-        from ezdxf import bbox
-        from ezdxf.addons.drawing import RenderContext, Frontend
-        from ezdxf.addons.drawing.config import Configuration, LinePolicy
-        from ezdxf.addons.drawing.pillow import (
-            PillowBackend,
-            PillowBackendException,
-        )
-        from ezdxf.addons.drawing.properties import LayoutProperties
-
-        verbose = args.verbose
-        if args.file:
-            filename = args.file
-        else:
-            print("argument FILE is required")
-            sys.exit(1)
-        print(f'loading file "{filename}"...')
-        doc, _ = load_document(filename)
-        try:
-            layout = doc.layout(args.layout)
-        except KeyError:
-            print(f'layout "{args.layout}" not found')
-            sys.exit(4)
-
-        bg = args.background
-        layout_properties = LayoutProperties.from_layout(layout)
-        if bg is not None:
-            if not bg.startswith("#"):
-                bg = "#" + bg
-            try:
-                layout_properties.set_colors(bg)
-            except ValueError:
-                print(f'ERROR: invalid background color value "{args.background}"')
-                sys.exit(4)
-
-        ctx = RenderContext(doc)
-        # force accurate linetype rendering by the frontend
-        config = Configuration.defaults().with_changes(line_policy=LinePolicy.ACCURATE)
-        if verbose:
-            print(f"detecting extents...\n")
-        bbox_cache = bbox.Cache()
-        if layout.is_any_paperspace:
-            # get entity bounding boxes in modelspace for faster paperspace
-            # rendering
-            bbox.extents(doc.modelspace(), fast=True, cache=bbox_cache)
-        extents = bbox.extents(layout, fast=True, cache=bbox_cache)
-        img_x, img_y = parse_image_size(args.image_size)
-        if verbose:
-            print(f"    units: {units.unit_name(layout.units)}")
-            print(f"    modelspace size: {extents.size.x:.3f} x {extents.size.y:.3f}")
-            print(f"    min extents: ({extents.extmin.x:.3f}, {extents.extmin.y:.3f})")
-            print(f"    max extents: ({extents.extmax.x:.3f}, {extents.extmax.y:.3f})")
-            print(f"\nimage size: {img_x} x {img_y}")
-        try:
-            out = PillowBackend(
-                extents,
-                image_size=(img_x, img_y),
-                oversampling=args.oversampling,
-                margin=args.margin,
-                dpi=args.dpi,
-                text_mode=args.text_mode,
-            )
-        except PillowBackendException as e:
-            print(str(e))
-            sys.exit(5)
-
-        t0 = time.perf_counter()
-        if verbose:
-            print(f'drawing layout "{layout.name}"...')
-        Frontend(ctx, out, config=config, bbox_cache=bbox_cache).draw_layout(
-            layout, layout_properties=layout_properties
-        )
-        t1 = time.perf_counter()
-        if verbose:
-            print(f"took {t1-t0:.4f} seconds")
-        if args.out is not None:
-            print(f'exporting to "{args.out}"')
-            t0 = time.perf_counter()
-            out.export(args.out)
-            t1 = time.perf_counter()
-            if verbose:
-                print(f"took {t1 - t0:.4f} seconds")
-        else:
-            if verbose:
-                print("opening image with the default system viewer...")
-            out.resize().show(args.file)
-
-
-def parse_image_size(image_size: str) -> tuple[int, int]:
-    if "," in image_size:
-        sx, sy = image_size.split(",")
-    elif "x" in image_size:
-        sx, sy = image_size.split("x")
-    else:
-        sx = int(image_size)  # type: ignore
-        sy = sx
-    return int(sx), int(sy)
-
-
-@register
 class Browse(Command):
     """Launcher sub-command: browse"""
 
     NAME = "browse"
 
     @staticmethod
     def add_parser(subparsers):
@@ -1037,15 +849,17 @@
     """Launcher sub-command: plt2dxf"""
 
     NAME = "plt2dxf"
 
     @staticmethod
     def add_parser(subparsers):
         parser = make_plt2fmt_parser(subparsers, Plt2Dxf.NAME, "DXF")
-        parser.epilog = "Note that plot files are intended to be plotted on white paper."
+        parser.epilog = (
+            "Note that plot files are intended to be plotted on white paper."
+        )
         parser.add_argument(
             "--aci",
             action="store_true",
             required=False,
             help="use pen numbers as ACI colors",
         )
         parser.add_argument(
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/comments.py` & `ezdxf-1.1.0b0/src/ezdxf/comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/disassemble.py` & `ezdxf-1.1.0b0/src/ezdxf/disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/document.py` & `ezdxf-1.1.0b0/src/ezdxf/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1338,14 +1338,16 @@
     data.append(f"DXF Version: {doc.dxfversion}")
     if verbose:
         data.append(
             f"Maintenance Version: {header.get('$ACADMAINTVER', '<undefined>')}"
         )
     data.append(f"Codepage: {header.get('$DWGCODEPAGE', 'ANSI_1252')}")
     data.append(f"Encoding: {doc.output_encoding}")
+    data.append("Layouts:")
+    data.extend([f"  '{name}'" for name in doc.layout_names_in_taborder()])
 
     measurement = "Metric" if header.get("$MEASUREMENT", 0) else "Imperial"
     if verbose:
         data.append(f"Unit system: {measurement}")
         data.append(f"Modelspace units: {unit_name(doc.units)}")
         append_header_var("$LASTSAVEDBY")
         append_header_var("$HANDSEED")
@@ -1374,15 +1376,14 @@
         append_container(doc.appids, "APPID")
         append_container(doc.ucs, "UCS")
         append_container(doc.views, "VIEW")
         append_container(doc.viewports, "VPORT")
         append_container(doc.block_records, "BLOCK_RECORD")
         if doc.dxfversion > DXF12:
             append_container(list(doc.classes), "CLASS", container="section")  # type: ignore
-
         data.append(f"Entities in modelspace: {len(doc.modelspace())}")
         if verbose:
             data.extend(count(doc.modelspace()))
 
         data.append(f"Entities in OBJECTS section: {len(doc.objects)}")
         if verbose:
             data.extend(count(doc.objects))
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/dwginfo.py` & `ezdxf-1.1.0b0/src/ezdxf/dwginfo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entitydb.py` & `ezdxf-1.1.0b0/src/ezdxf/entitydb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/enums.py` & `ezdxf-1.1.0b0/src/ezdxf/enums.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/explode.py` & `ezdxf-1.1.0b0/src/ezdxf/explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/eztypes.py` & `ezdxf-1.1.0b0/src/ezdxf/eztypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/filemanagement.py` & `ezdxf-1.1.0b0/src/ezdxf/filemanagement.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/gfxattribs.py` & `ezdxf-1.1.0b0/src/ezdxf/gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/graphicsfactory.py` & `ezdxf-1.1.0b0/src/ezdxf/graphicsfactory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/groupby.py` & `ezdxf-1.1.0b0/src/ezdxf/groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/protocols.py` & `ezdxf-1.1.0b0/src/ezdxf/protocols.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/proxygraphic.py` & `ezdxf-1.1.0b0/src/ezdxf/proxygraphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/query.py` & `ezdxf-1.1.0b0/src/ezdxf/query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/queryparser.py` & `ezdxf-1.1.0b0/src/ezdxf/queryparser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/r12strict.py` & `ezdxf-1.1.0b0/src/ezdxf/r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/recover.py` & `ezdxf-1.1.0b0/src/ezdxf/recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/reorder.py` & `ezdxf-1.1.0b0/src/ezdxf/reorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/shapefile.py` & `ezdxf-1.1.0b0/src/ezdxf/shapefile.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/transform.py` & `ezdxf-1.1.0b0/src/ezdxf/transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/units.py` & `ezdxf-1.1.0b0/src/ezdxf/units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/upright.py` & `ezdxf-1.1.0b0/src/ezdxf/upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/urecord.py` & `ezdxf-1.1.0b0/src/ezdxf/urecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/version.py` & `ezdxf-1.1.0b0/src/ezdxf/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # examples:
 #   major pre-release alpha 2: VERSION = "0.9.0a2"; version = (0, 9, 0, 'a2')
 #   major release candidate 0: VERSION = "0.9.0rc0"; version = (0, 9, 0, 'rc0')
 #   major release: VERSION = "0.9.0"; version = (0, 9, 0, 'release')
 #   1. bug fix release beta0: VERSION = "0.9.1b0"; version = (0, 9, 1, 'b0')
 #   2. bug fix release: VERSION = "0.9.2"; version = (0, 9, 2, 'release')
 
-version = (1, 0, 4, "b1")
-__version__ = "1.0.4b1"
+version = (1, 0, 4, "b0")
+__version__ = "1.1.0b0"
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/xref.py` & `ezdxf-1.1.0b0/src/ezdxf/xref.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/zoom.py` & `ezdxf-1.1.0b0/src/ezdxf/zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/_options.py` & `ezdxf-1.1.0b0/src/ezdxf/_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,21 +11,14 @@
 # import ezdxf
 # value = ezdxf.options.<attribute>
 #
 # If the import of "ezdxf" is not wanted:
 # from ezdxf._options import options
 
 # The MATPLOTLIB global shows that Matplotlib is installed:
-try:
-    import matplotlib
-
-    MATPLOTLIB = True
-except ImportError:
-    MATPLOTLIB = False
-
 TRUE_STATE = {"True", "true", "On", "on", "1"}
 CORE = "core"
 BROWSE_COMMAND = "browse-command"
 VIEW_COMMAND = "view-command"
 DRAW_COMMAND = "draw-command"
 EZDXF_INI = "ezdxf.ini"
 EZDXF = "ezdxf"
@@ -148,15 +141,14 @@
     def __init__(self) -> None:
         paths = config_files()
         self._loaded_paths: list[Path] = [p for p in paths if p.exists()]
         self._config = load_config_files(paths)
         # needs fast access:
         self.log_unprocessed_tags = True
         # Activate/deactivate Matplotlib support (e.g. for testing)
-        self._use_matplotlib = MATPLOTLIB
         self._use_c_ext = False  # set ezdxf.acc.__init__!
         self.debug = False
         self.update_cached_options()
 
     def set(self, section: str, key: str, value: str) -> None:
         self._config.set(section, key, value)
 
@@ -296,26 +288,14 @@
 
     @property
     def disable_c_ext(self) -> bool:
         """Disable C-extensions if ``True``."""
         return self.get_bool(CORE, "DISABLE_C_EXT", default=False)
 
     @property
-    def use_matplotlib(self) -> bool:
-        """Activate/deactivate Matplotlib support e.g. for testing"""
-        return self._use_matplotlib
-
-    @use_matplotlib.setter
-    def use_matplotlib(self, state: bool) -> None:
-        if MATPLOTLIB:
-            self._use_matplotlib = state
-        else:  # Matplotlib is not installed
-            self._use_matplotlib = False
-
-    @property
     def use_c_ext(self) -> bool:
         """Returns ``True`` if the C-extensions are in use."""
         return self._use_c_ext
 
     def preserve_proxy_graphics(self, state: bool = True) -> None:
         """Enable/disable proxy graphic load/store support."""
         value = boolstr(state)
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/__init__.py` & `ezdxf-1.1.0b0/src/ezdxf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     has_dxf_unicode,
     decode_dxf_unicode,
 )
 
 # setup DXF unicode encoder -> '\U+nnnn'
 codecs.register_error("dxfreplace", dxf_backslash_replace)
 
-fonts.load()
 EZDXF_TEST_FILES = options.test_files
 
 YES_NO = {True: "yes", False: "no"}
 
 
 def print_config(
     verbose: bool = False, stream: Optional[TextIO] = None
@@ -81,15 +80,14 @@
     if stream is None:
         stream = sys.stdout
     stream.writelines(
         [
             f"ezdxf {__version__} from {Path(__file__).parent}\n",
             f"Python version: {sys.version}\n",
             f"using C-extensions: {YES_NO[options.use_c_ext]}\n",
-            f"using Matplotlib: {YES_NO[options.use_matplotlib]}\n",
         ]
     )
     if verbose:
         stream.write("\nConfiguration:\n")
         options.write(stream)
         stream.write("\nEnvironment Variables:\n")
         for v in options.CONFIG_VARS:
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/__main__.py` & `ezdxf-1.1.0b0/src/ezdxf/__main__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/bezier3p.pyx` & `ezdxf-1.1.0b0/src/ezdxf/acc/bezier3p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/bezier4p.pyx` & `ezdxf-1.1.0b0/src/ezdxf/acc/bezier4p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/bspline.pyx` & `ezdxf-1.1.0b0/src/ezdxf/acc/bspline.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/construct.pyx` & `ezdxf-1.1.0b0/src/ezdxf/acc/construct.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/linetypes.pyx` & `ezdxf-1.1.0b0/src/ezdxf/acc/linetypes.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/mapbox_earcut.pyx` & `ezdxf-1.1.0b0/src/ezdxf/acc/mapbox_earcut.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/matrix44.pyx` & `ezdxf-1.1.0b0/src/ezdxf/acc/matrix44.pyx`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # cython: language_level=3
 # distutils: language = c++
 # Copyright (c) 2020-2021, Manfred Moitzi
 # License: MIT License
-from typing import Sequence, Iterable, Tuple, TYPE_CHECKING
+from typing import Sequence, Iterable, Tuple, TYPE_CHECKING, Iterator
 from itertools import chain
 import math
 from .vector cimport (
-Vec3, v3_normalize, v3_isclose, v3_cross, v3_dot,
+Vec2, Vec3, v3_normalize, v3_isclose, v3_cross, v3_dot,
 )
 from .vector import X_AXIS, Y_AXIS, Z_AXIS, NULLVEC
 
 from libc.math cimport fabs, sin, cos, tan
 
 if TYPE_CHECKING:
     from ezdxf.math import UVec
@@ -82,14 +82,30 @@
         return "Matrix44(%s)" % \
                ", ".join(format_row(row) for row in self.rows())
 
     def get_2d_transformation(self) -> Tuple[float, ...]:
         cdef double *m = self.m
         return m[0], m[1], 0.0, m[4], m[5], 0.0, m[12], m[13], 1.0
 
+    @staticmethod
+    def from_2d_transformation(components: Sequence[float]) -> Matrix44:
+        if len(components) != 6:
+            raise ValueError(
+                "First 2 columns of a 3x3 matrix required: m11, m12, m21, m22, m31, m32"
+            )
+
+        m44 = Matrix44()
+        m44.m[0] = components[0]
+        m44.m[1] = components[1]
+        m44.m[4] = components[2]
+        m44.m[5] = components[3]
+        m44.m[12] = components[4]
+        m44.m[13] = components[5]
+        return m44
+
     def get_row(self, int row) -> Tuple[float, ...]:
         cdef index = row * 4
         if 0 <= index < 13:
             return self.m[index], self.m[index + 1], self.m[index + 2], self.m[
                 index + 3]
         else:
             raise IndexError(f'invalid row index: {row}')
@@ -120,29 +136,29 @@
             if count > 4:
                 count = 4
             for i in range(count):
                 self.m[col + i * 4] = values[i]
         else:
             raise IndexError(f'invalid col index: {col}')
 
-    def rows(self) -> Iterable[Tuple[float, ...]]:
+    def rows(self) -> Iterator[Tuple[float, ...]]:
         return (self.get_row(index) for index in (0, 1, 2, 3))
 
-    def columns(self) -> Iterable[Tuple[float, ...]]:
+    def columns(self) -> Iterator[Tuple[float, ...]]:
         return (self.get_col(index) for index in (0, 1, 2, 3))
 
-    def copy(self) -> 'Matrix44':
+    def copy(self) -> Matrix44:
         cdef Matrix44 _copy = Matrix44()
         _copy.m = self.m
         return _copy
 
     __copy__ = copy
 
     @property
-    def origin(self) -> 'Vec3':
+    def origin(self) -> Vec3:
         cdef Vec3 v = Vec3()
         v.x = self.m[12]
         v.y = self.m[13]
         v.z = self.m[14]
         return v
 
     @origin.setter
@@ -196,64 +212,64 @@
         cdef Vec3 uy = v3_normalize(self.get_uy(), 1.0)
         cdef Vec3 uz = v3_normalize(self.get_uz(), 1.0)
         return fabs(v3_dot(ux, uy)) < 1e-9 and \
                fabs(v3_dot(ux, uz)) < 1e-9 and \
                fabs(v3_dot(uy, uz)) < 1e-9
 
     @staticmethod
-    def scale(double sx, sy = None, sz = None) -> 'Matrix44':
+    def scale(double sx, sy = None, sz = None) -> Matrix44:
         cdef Matrix44 mat = Matrix44()
         mat.m[0] = sx
         mat.m[5] = sx if sy is None else sy
         mat.m[10] = sx if sz is None else sz
         return mat
 
     @staticmethod
-    def translate(double dx, double dy, double dz) -> 'Matrix44':
+    def translate(double dx, double dy, double dz) -> Matrix44:
         cdef Matrix44 mat = Matrix44()
         mat.m[12] = dx
         mat.m[13] = dy
         mat.m[14] = dz
         return mat
 
     @staticmethod
-    def x_rotate(double angle) -> 'Matrix44':
+    def x_rotate(double angle) -> Matrix44:
         cdef Matrix44 mat = Matrix44()
         cdef double cos_a = cos(angle)
         cdef double sin_a = sin(angle)
         mat.m[5] = cos_a
         mat.m[6] = sin_a
         mat.m[9] = -sin_a
         mat.m[10] = cos_a
         return mat
 
     @staticmethod
-    def y_rotate(double angle) -> 'Matrix44':
+    def y_rotate(double angle) -> Matrix44:
         cdef Matrix44 mat = Matrix44()
         cdef double cos_a = cos(angle)
         cdef double sin_a = sin(angle)
         mat.m[0] = cos_a
         mat.m[2] = -sin_a
         mat.m[8] = sin_a
         mat.m[10] = cos_a
         return mat
 
     @staticmethod
-    def z_rotate(double angle) -> 'Matrix44':
+    def z_rotate(double angle) -> Matrix44:
         cdef Matrix44 mat = Matrix44()
         cdef double cos_a = cos(angle)
         cdef double sin_a = sin(angle)
         mat.m[0] = cos_a
         mat.m[1] = sin_a
         mat.m[4] = -sin_a
         mat.m[5] = cos_a
         return mat
 
     @staticmethod
-    def axis_rotate(axis: UVec, double angle) -> 'Matrix44':
+    def axis_rotate(axis: UVec, double angle) -> Matrix44:
         cdef Matrix44 mat = Matrix44()
         cdef double cos_a = cos(angle)
         cdef double sin_a = sin(angle)
         cdef double one_m_cos = 1.0 - cos_a
         cdef Vec3 _axis = Vec3(axis).normalize()
         cdef double x = _axis.x
         cdef double y = _axis.y
@@ -271,15 +287,15 @@
         mat.m[9] = y * z * one_m_cos - x * sin_a
         mat.m[10] = z * z * one_m_cos + cos_a
 
         return mat
 
     @staticmethod
     def xyz_rotate(double angle_x, double angle_y,
-                   double angle_z) -> 'Matrix44':
+                   double angle_z) -> Matrix44:
         cdef Matrix44 mat = Matrix44()
         cdef double cx = cos(angle_x)
         cdef double sx = sin(angle_x)
         cdef double cy = cos(angle_y)
         cdef double sy = sin(angle_y)
         cdef double cz = cos(angle_z)
         cdef double sz = sin(angle_z)
@@ -294,55 +310,55 @@
         mat.m[6] = cxsy * sz + sx * cz
         mat.m[8] = sy
         mat.m[9] = -sx * cy
         mat.m[10] = cx * cy
         return mat
 
     @staticmethod
-    def shear_xy(double angle_x = 0, double angle_y = 0) -> 'Matrix44':
+    def shear_xy(double angle_x = 0, double angle_y = 0) -> Matrix44:
         cdef Matrix44 mat = Matrix44()
         cdef double tx = tan(angle_x)
         cdef double ty = tan(angle_y)
         mat.m[1] = ty
         mat.m[4] = tx
         return mat
 
     @staticmethod
     def perspective_projection(double left, double right, double top,
                                double bottom, double near,
-                               double far) -> 'Matrix44':
+                               double far) -> Matrix44:
         cdef Matrix44 mat = Matrix44()
         mat.m[0] = (2. * near) / (right - left)
         mat.m[5] = (2. * near) / (top - bottom)
         mat.m[8] = (right + left) / (right - left)
         mat.m[9] = (top + bottom) / (top - bottom)
         mat.m[10] = -((far + near) / (far - near))
         mat.m[11] = -1
         mat.m[14] = -((2. * far * near) / (far - near))
         return mat
 
     @staticmethod
     def perspective_projection_fov(fov: float, aspect: float, near: float,
-                                   far: float) -> 'Matrix44':
+                                   far: float) -> Matrix44:
         vrange = near * math.tan(fov / 2.)
         left = -vrange * aspect
         right = vrange * aspect
         bottom = -vrange
         top = vrange
         return Matrix44.perspective_projection(left, right, bottom, top, near,
                                                far)
 
     @staticmethod
-    def chain(*matrices: 'Matrix44') -> 'Matrix44':
+    def chain(*matrices: Matrix44) -> Matrix44:
         cdef Matrix44 transformation = Matrix44()
         for matrix in matrices:
             transformation *= matrix
         return transformation
 
-    def __imul__(self, Matrix44 other) -> 'Matrix44':
+    def __imul__(self, Matrix44 other) -> Matrix44:
         cdef double[16] m1 = self.m
         cdef double *m2 = other.m
 
         self.m[0] = m1[0] * m2[0] + m1[1] * m2[4] + m1[2] * m2[8] + \
                     m1[3] * m2[12]
         self.m[1] = m1[0] * m2[1] + m1[1] * m2[5] + m1[2] * m2[9] + \
                     m1[3] * m2[13]
@@ -375,21 +391,21 @@
                      m1[15] * m2[13]
         self.m[14] = m1[12] * m2[2] + m1[13] * m2[6] + m1[14] * m2[10] + \
                      m1[15] * m2[14]
         self.m[15] = m1[12] * m2[3] + m1[13] * m2[7] + m1[14] * m2[11] + \
                      m1[15] * m2[15]
         return self
 
-    def __mul__(self, Matrix44 other) -> 'Matrix44':
+    def __mul__(self, Matrix44 other) -> Matrix44:
         cdef Matrix44 res_matrix = self.copy()
         return res_matrix.__imul__(other)
 
     # __matmul__ = __mul__ does not work!
 
-    def __matmul__(self, Matrix44 other) -> 'Matrix44':
+    def __matmul__(self, Matrix44 other) -> Matrix44:
         cdef Matrix44 res_matrix = self.copy()
         return res_matrix.__imul__(other)
 
     def transpose(self) -> None:
         swap(&self.m[1], &self.m[4])
         swap(&self.m[2], &self.m[8])
         swap(&self.m[3], &self.m[12])
@@ -476,15 +492,15 @@
                       m[14] - m[0] * m[5] * m[14]) * f
 
         self.m[15] = (m[1] * m[6] * m[8] - m[2] * m[5] * m[8] + m[2] * m[4] *
                       m[9] - m[0] * m[6] * m[9] - m[1] * m[4] * m[10] +
                       m[0] * m[5] * m[10]) * f
 
     @staticmethod
-    def ucs(ux=X_AXIS, uy=Y_AXIS, uz=Z_AXIS, origin=NULLVEC) -> 'Matrix44':
+    def ucs(ux=X_AXIS, uy=Y_AXIS, uz=Z_AXIS, origin=NULLVEC) -> Matrix44:
         cdef Matrix44 mat = Matrix44()
         cdef Vec3 _ux = Vec3(ux)
         cdef Vec3 _uy = Vec3(uy)
         cdef Vec3 _uz = Vec3(uz)
         cdef Vec3 _origin = Vec3(origin)
 
         mat.m[0] = _ux.x
@@ -530,15 +546,15 @@
         if normalize:
             return v3_normalize(res, 1.0)
         else:
             return res
 
     ocs_to_wcs = transform_direction
 
-    def transform_vertices(self, vectors: Iterable[UVec]) -> Iterable[Vec3]:
+    def transform_vertices(self, vectors: Iterable[UVec]) -> Iterator[Vec3]:
         cdef double *m = self.m
         cdef Vec3 res
         cdef double x, y, z
 
         for vector in vectors:
             res = Vec3(vector)
             x = res.x
@@ -546,16 +562,35 @@
             z = res.z
 
             res.x = x * m[0] + y * m[4] + z * m[8] + m[12]
             res.y = x * m[1] + y * m[5] + z * m[9] + m[13]
             res.z = x * m[2] + y * m[6] + z * m[10] + m[14]
             yield res
 
-    def transform_directions(self, vectors: Iterable[UVec],
-                             normalize=False) -> Iterable[Vec3]:
+    def fast_2d_transform(self, points: Iterable[UVec]) -> Iterator[Vec2]:
+        cdef double m0 = self.m[0]
+        cdef double m1 = self.m[1]
+        cdef double m4 = self.m[4]
+        cdef double m5 = self.m[5]
+        cdef double m12 = self.m[12]
+        cdef double m13 = self.m[13]
+        cdef double x, y
+        cdef Vec2 res
+
+        for pnt in points:
+            res = Vec2(pnt)
+            x = res.x
+            y = res.y
+            res.x = x * m0 + y * m4 + m12
+            res.y = x * m1 + y * m5 + m13
+            yield res
+
+    def transform_directions(
+        self, vectors: Iterable[UVec], normalize=False
+    ) -> Iterator[Vec3]:
         cdef double *m = self.m
         cdef Vec3 res
         cdef double x, y, z
         cdef bint _normalize = normalize
 
         for vector in vectors:
             res = Vec3(vector)
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/vector.pxd` & `ezdxf-1.1.0b0/src/ezdxf/acc/vector.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/vector.pyx` & `ezdxf-1.1.0b0/src/ezdxf/acc/vector.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.cpp` & `ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_cubic_bezier.hpp` & `ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_cubic_bezier.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_quad_bezier.cpp` & `ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_quad_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_vec3.hpp` & `ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_vec3.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/_cpp_vec3.pxd` & `ezdxf-1.1.0b0/src/ezdxf/acc/_cpp_vec3.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acc/__init__.py` & `ezdxf-1.1.0b0/src/ezdxf/acc/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acis/abstract.py` & `ezdxf-1.1.0b0/src/ezdxf/acis/abstract.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acis/api.py` & `ezdxf-1.1.0b0/src/ezdxf/acis/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acis/const.py` & `ezdxf-1.1.0b0/src/ezdxf/acis/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acis/dbg.py` & `ezdxf-1.1.0b0/src/ezdxf/acis/dbg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acis/dxf.py` & `ezdxf-1.1.0b0/src/ezdxf/acis/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acis/entities.py` & `ezdxf-1.1.0b0/src/ezdxf/acis/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acis/hdr.py` & `ezdxf-1.1.0b0/src/ezdxf/acis/hdr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acis/mesh.py` & `ezdxf-1.1.0b0/src/ezdxf/acis/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acis/sab.py` & `ezdxf-1.1.0b0/src/ezdxf/acis/sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/acis/sat.py` & `ezdxf-1.1.0b0/src/ezdxf/acis/sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/acadctb.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/acadctb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Purpose: read and write AutoCAD CTB files
-# Copyright (c) 2010-2022, Manfred Moitzi
+# Copyright (c) 2010-2023, Manfred Moitzi
 # License: MIT License
 # IMPORTANT: use only standard 7-Bit ascii code
 from __future__ import annotations
 from typing import (
     Union,
     Optional,
     BinaryIO,
     TextIO,
     Iterable,
     Iterator,
     Any,
 )
+import os
 from abc import abstractmethod
 from io import StringIO
 from array import array
 from struct import pack
 import zlib
 
 END_STYLE_BUTT = 0
@@ -130,17 +131,15 @@
         # do not set _color, _mode_color or _color_policy directly
         # use set_color() method, and the properties dithering and grayscale
         self._color = int(data.get("color", OBJECT_COLOR))
         self._color_type = COLOR_RGB
         if self._color != OBJECT_COLOR:
             self._mode_color = int(data.get("mode_color", self._color))
         self._color_policy = int(data.get("color_policy", DITHERING_ON))
-        self.physical_pen_number = int(
-            data.get("physical_pen_number", AUTOMATIC)
-        )
+        self.physical_pen_number = int(data.get("physical_pen_number", AUTOMATIC))
         self.virtual_pen_number = int(data.get("virtual_pen_number", AUTOMATIC))
         self.screen = int(data.get("screen", 100))
         self.linepattern_size = float(data.get("linepattern_size", 0.5))
         self.linetype = int(data.get("linetype", OBJECT_LINETYPE))  # 0 .. 30
         self.adaptive_linetype = get_bool(data.get("adaptive_linetype", True))
 
         # lineweight index
@@ -269,16 +268,15 @@
         stream.write("  color_policy=%d\n" % self._color_policy)
         stream.write("  physical_pen_number=%d\n" % self.physical_pen_number)
         stream.write("  virtual_pen_number=%d\n" % self.virtual_pen_number)
         stream.write("  screen=%d\n" % self.screen)
         stream.write("  linepattern_size=%s\n" % str(self.linepattern_size))
         stream.write("  linetype=%d\n" % self.linetype)
         stream.write(
-            "  adaptive_linetype=%s\n"
-            % str(bool(self.adaptive_linetype)).upper()
+            "  adaptive_linetype=%s\n" % str(bool(self.adaptive_linetype)).upper()
         )
         stream.write("  lineweight=%s\n" % str(self.lineweight))
         stream.write("  fill_style=%d\n" % self.fill_style)
         stream.write("  end_style=%d\n" % self.end_style)
         stream.write("  join_style=%d\n" % self.join_style)
         stream.write(" }\n")
 
@@ -292,16 +290,16 @@
         scale_factor: float = 1.0,
         apply_factor: bool = False,
     ):
         self.description = description
         self.scale_factor = scale_factor
         self.apply_factor = apply_factor
 
-        # set custom_lineweight_display_units to 1 for showing lineweight in inch in AutoCAD CTB editor window, but
-        # lineweight is always defined in mm
+        # set custom_lineweight_display_units to 1 for showing lineweight in inch in
+        # AutoCAD CTB editor window, but lineweight is always defined in mm
         self.custom_lineweight_display_units = 0
         self.lineweights = array("f", DEFAULT_LINE_WEIGHTS)
 
     def get_lineweight_index(self, lineweight: float) -> int:
         """Get index of `lineweight` in the lineweight table or append
         `lineweight` to lineweight table.
         """
@@ -334,15 +332,15 @@
 
         Returns:
             lineweight in mm or ``0.0`` for use entity lineweight
 
         """
         return self.lineweights[index]
 
-    def save(self, filename: str) -> None:
+    def save(self, filename: str | os.PathLike) -> None:
         """Save CTB or STB file as `filename` to the file system."""
         with open(filename, "wb") as stream:
             self.write(stream)
 
     def write(self, stream: BinaryIO) -> None:
         """Compress and write the CTB or STB file to binary `stream`."""
         memfile = StringIO()
@@ -629,17 +627,19 @@
     """Read a STB-file from binary `stream`."""
     content: bytes = _decompress(stream)
     styles = NamedPlotStyles()
     styles.parse(content.decode())
     return styles
 
 
-def load(filename: str) -> Union[ColorDependentPlotStyles, NamedPlotStyles]:
+def load(
+    filename: str | os.PathLike,
+) -> Union[ColorDependentPlotStyles, NamedPlotStyles]:
     """Load the CTB or STB file `filename` from file system."""
-
+    filename = str(filename)
     with open(filename, "rb") as stream:
         if filename.lower().endswith(".ctb"):
             return _read_ctb(stream)
         elif filename.lower().endswith(".stb"):
             return _read_stb(stream)
         else:
             raise ValueError('Invalid file type: "{}"'.format(filename))
@@ -753,19 +753,15 @@
     color_type = (color & 0xFF000000) >> 24
     red = (color & 0xFF0000) >> 16
     green = (color & 0xFF00) >> 8
     blue = color & 0xFF
     return red, green, blue, color_type
 
 
-def mode_color2int(
-    red: int, green: int, blue: int, color_type=COLOR_RGB
-) -> int:
+def mode_color2int(red: int, green: int, blue: int, color_type=COLOR_RGB) -> int:
     """Convert mode_color (r, g, b, color_type) tuple to integer."""
     return -color2int(red, green, blue, color_type)
 
 
 def color2int(red: int, green: int, blue: int, color_type: int) -> int:
     """Convert color (r, g, b, color_type) to integer."""
-    return (
-        -((color_type << 24) + (red << 16) + (green << 8) + blue) & 0xFFFFFFFF
-    )
+    return -((color_type << 24) + (red << 16) + (green << 8) + blue) & 0xFFFFFFFF
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/binpacking.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/binpacking.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/dimlines.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/dimlines.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/dxf2code.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/dxf2code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/genetic_algorithm.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/geo.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/gerber_D6673.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/gerber_D6673.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/importer.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/iterdxf.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/iterdxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/menger_sponge.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/meshex.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/mtextsurrogate.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/mtextsurrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/mtxpl.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/mtxpl.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,16 +148,16 @@
         style_name = entity.dxf.style
 
     font_face = fonts.FontFace()
     if style_name and doc is not None:
         style = cast(Textstyle, doc.styles.get(style_name))
         family, italic, bold = style.get_extended_font_data()
         if family:
-            text_style = "italic" if italic else "normal"
-            text_weight = "bold" if bold else "normal"
+            text_style = "Italic" if italic else "Regular"
+            text_weight = 700 if bold else 400
             font_face = fonts.FontFace(
                 family=family, style=text_style, weight=text_weight
             )
         else:
             ttf = style.dxf.font
             if ttf:
                 font_face = fonts.get_font_face(ttf)
@@ -302,15 +302,15 @@
         style_str = str(style) if style > 0 else ""
         # BricsCAD naming convention for exploded MTEXT styles:
         text_style = f"MtXpl_{font_face.family}" + style_str
         self._required_text_styles[text_style] = font_face
         return text_style
 
     def get_font(self, ctx: MTextContext) -> fonts.AbstractFont:
-        ttf = fonts.find_ttf_path(ctx.font_face)
+        ttf = fonts.find_font_file_name(ctx.font_face)
         key = (ttf, ctx.cap_height, ctx.width_factor)
         font = self._font_cache.get(key)
         if font is None:
             font = fonts.make_font(ttf, ctx.cap_height, ctx.width_factor)
             self._font_cache[key] = font
         return font
 
@@ -357,15 +357,15 @@
             except ezdxf.DXFTableEntryError:
                 pass
 
     def make_required_style_table_entries(self) -> list[Textstyle]:
         def ttf_path(font_face: fonts.FontFace) -> str:
             ttf = font_face.ttf
             if not ttf:
-                ttf = fonts.find_ttf_path(font_face)
+                ttf = fonts.find_font_file_name(font_face)
             else:
                 # remapping SHX replacement fonts to SHX fonts,
                 # like "txt_____.ttf" to "TXT.SHX":
                 shx = fonts.map_ttf_to_shx(ttf)
                 if shx:
                     ttf = shx
             return ttf
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/odafc.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/openscad.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/pycsg.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/r12export.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/r12writer.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/sierpinski_pyramid.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/sierpinski_pyramid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/tablepainter.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/tablepainter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/text2path.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/text2path.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #  Copyright (c) 2021-2022, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Union
 import enum
-from matplotlib.textpath import TextPath
-from matplotlib.font_manager import FontProperties, findfont
 
 from ezdxf.entities import Text, Attrib, Hatch, DXFGraphic
 from ezdxf.lldxf import const
 from ezdxf.enums import TextEntityAlignment, MAP_TEXT_ENUM_TO_ALIGN_FLAGS
 from ezdxf.math import Matrix44, BoundingBox
 from ezdxf import path
 from ezdxf.path import Path
 from ezdxf.tools import fonts
+from ezdxf.tools.ttfonts import TTFontRenderer
 from ezdxf.query import EntityQuery
 
 __all__ = [
     "make_path_from_str",
     "make_paths_from_str",
     "make_hatches_from_str",
     "make_path_from_entity",
@@ -52,23 +51,22 @@
             default is :attr:`LEFT`
          length: target length for the :attr:`ALIGNED` and :attr:`FIT` alignments
          m: transformation :class:`~ezdxf.math.Matrix44`
 
     """
     if len(s) == 0:
         return Path()
-    font_properties, font_measurements = _get_font_data(font)
+    render_engine = get_render_engine(font)
     # scale font rendering units to drawing units:
-    render_size = size / font_measurements.cap_height
-    p = _str_to_path(s, font_properties, render_size)
+    p = _str_to_path(s, render_engine, size)
     bbox = path.bbox([p], fast=True)
 
     # Text is rendered in drawing units,
     # therefore do alignment in drawing units:
-    draw_units_fm = font_measurements.scale_from_baseline(size)
+    draw_units_fm = render_engine.font_measurements.scale_from_baseline(size)
     matrix = alignment_transformation(draw_units_fm, bbox, align, length)
     if m is not None:
         matrix *= m
     return p.transform(matrix)
 
 
 def make_paths_from_str(
@@ -98,33 +96,24 @@
     """
     if len(s) == 0:
         return []
     p = make_path_from_str(s, font, size, align, length, m)
     return list(p.sub_paths())
 
 
-def _get_font_data(
+def get_render_engine(
     font: fonts.FontFace,
-) -> tuple[FontProperties, fonts.FontMeasurements]:
-    fp = FontProperties(
-        family=font.family,
-        style=font.style,
-        stretch=font.stretch,
-        weight=font.weight,
-    )
-    ttf_path = findfont(fp)
-    fonts.load()  # not expensive if already loaded
-    # The ttf file path is the cache key for font measurements:
-    fm = fonts.get_font_measurements(ttf_path)
-    return fp, fm
-
-
-def _str_to_path(s: str, fp: FontProperties, size: float = 1.0) -> Path:
-    text_path = TextPath((0, 0), s, size=size, prop=fp, usetex=False)
-    return path.multi_path_from_matplotlib_path(text_path)
+) -> TTFontRenderer:
+    font_name = fonts.font_manager.find_font_file_name(font)
+    ttfont = fonts.font_manager.get_ttf_font(font_name)
+    return TTFontRenderer(ttfont)
+
+
+def _str_to_path(s: str, render_engine: TTFontRenderer, size: float = 1.0) -> Path:
+    return render_engine.get_text_path(s, cap_height=size).to_3d_path()
 
 
 def alignment_transformation(
     fm: fonts.FontMeasurements,
     bbox: BoundingBox,
     align: TextEntityAlignment,
     length: float,
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/xqt.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/xqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/browser.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/acisbrowser/data.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/acisbrowser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/browser/bookmarks.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/browser/bookmarks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/browser/browser.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/browser/browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
         toolbar.addAction(self._goto_handle_action)
         toolbar.addAction(self._store_bookmark)
         toolbar.addAction(self._go_to_bookmark)
         toolbar.addAction(self._copy_selected_tags_action)
         self.addToolBar(toolbar)
 
     def create_find_dialog(self) -> "FindDialog":
-        dialog = FindDialog(self)
+        dialog = FindDialog()
         dialog.setModal(True)
         dialog.find_forward_button.clicked.connect(self.find_forward)
         dialog.find_backwards_button.clicked.connect(self.find_backwards)
         dialog.find_forward_button.setShortcut("F3")
         dialog.find_backwards_button.setShortcut("F4")
         return dialog
 
@@ -751,16 +751,16 @@
         mode = clipboard.Mode.Clipboard
     except AttributeError:
         mode = clipboard.Clipboard  # type: ignore  # legacy location
     clipboard.setText(dxfstr(tags), mode=mode)
 
 
 class FindDialog(QtWidgets.QDialog, Ui_FindDialog):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(self):
+        super().__init__()
         self.setupUi(self)
         self.close_button.clicked.connect(lambda: self.close())
         self.settings = QSettings("ezdxf", "DXFBrowser")
 
     def restore_geometry(self):
         geometry = self.settings.value("find.dialog.geometry")
         if geometry is not None:
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/browser/data.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/browser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/browser/find_dialog.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/browser/find_dialog.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/browser/loader.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/browser/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/browser/model.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/browser/model.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/browser/tags.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/browser/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/browser/views.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/browser/views.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/backend.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/pyqt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,289 +1,298 @@
-# Copyright (c) 2020-2022, Matthew Broadway
+# Copyright (c) 2020-2023, Matthew Broadway
 # License: MIT License
+# mypy: ignore_errors=True
 from __future__ import annotations
-from abc import ABC, abstractmethod, ABCMeta
-from typing import (
-    Optional,
-    TYPE_CHECKING,
-    Iterable,
-)
+from typing import Optional, Iterable, Tuple
+from typing_extensions import TypeAlias
+import math
 
+from ezdxf.addons.xqt import QtCore as qc, QtGui as qg, QtWidgets as qw
+from ezdxf.addons.drawing.backend import Backend
 from ezdxf.addons.drawing.config import Configuration
-from ezdxf.addons.drawing.properties import Properties
 from ezdxf.addons.drawing.type_hints import Color
-from ezdxf.entities import DXFGraphic
-from ezdxf.tools.text import replace_non_printable_characters
+from ezdxf.addons.drawing.properties import Properties
 from ezdxf.math import Vec3, Matrix44
-from ezdxf.path import Path
-
-if TYPE_CHECKING:
-    from ezdxf.tools.fonts import FontFace, FontMeasurements
+from ezdxf.path import Path, to_qpainter_path
 
+PatternKey: TypeAlias = Tuple[str, float]
 
-class BackendInterface(ABC):
-    """the public interface for the rendering backend."""
-
-    @abstractmethod
-    def configure(self, config: Configuration) -> None:
-        raise NotImplementedError
 
-    @abstractmethod
-    def enter_entity(self, entity: DXFGraphic, properties: Properties) -> None:
-        raise NotImplementedError
+class _Point(qw.QAbstractGraphicsShapeItem):
+    """A dimensionless point which is drawn 'cosmetically' (scale depends on
+    view)
+    """
 
-    @abstractmethod
-    def exit_entity(self, entity: DXFGraphic) -> None:
-        raise NotImplementedError
+    def __init__(self, x: float, y: float, brush: qg.QBrush):
+        super().__init__()
+        self.location = qc.QPointF(x, y)
+        self.radius = 1.0
+        self.setPen(qg.QPen(qc.Qt.NoPen))
+        self.setBrush(brush)
 
-    @abstractmethod
-    def set_background(self, color: Color) -> None:
-        raise NotImplementedError
-
-    @abstractmethod
-    def draw_point(self, pos: Vec3, properties: Properties) -> None:
-        raise NotImplementedError
-
-    @abstractmethod
-    def draw_line(self, start: Vec3, end: Vec3, properties: Properties) -> None:
-        raise NotImplementedError
-
-    @abstractmethod
-    def draw_solid_lines(
-        self, lines: Iterable[tuple[Vec3, Vec3]], properties: Properties
-    ) -> None:
-        raise NotImplementedError
-
-    @abstractmethod
-    def draw_path(self, path: Path, properties: Properties) -> None:
-        raise NotImplementedError
-
-    @abstractmethod
-    def draw_filled_paths(
+    def paint(
         self,
-        paths: Iterable[Path],
-        holes: Iterable[Path],
-        properties: Properties,
-    ) -> None:
-        raise NotImplementedError
-
-    @abstractmethod
-    def draw_filled_polygon(
-        self, points: Iterable[Vec3], properties: Properties
+        painter: qg.QPainter,
+        option: qw.QStyleOptionGraphicsItem,
+        widget: Optional[qw.QWidget] = None,
     ) -> None:
-        raise NotImplementedError
+        view_scale = _get_x_scale(painter.transform())
+        radius = self.radius / view_scale
+        painter.setBrush(self.brush())
+        painter.setPen(qc.Qt.NoPen)
+        painter.drawEllipse(self.location, radius, radius)
+
+    def boundingRect(self) -> qc.QRectF:
+        return qc.QRectF(self.location, qc.QSizeF(1, 1))
+
+
+class ViewportGroup(qw.QGraphicsItemGroup):
+    def __init__(self, clipping_path: Path):
+        super().__init__()
+        self.setFlag(
+            qw.QGraphicsItemGroup.GraphicsItemFlag.ItemClipsChildrenToShape,
+            True,
+        )
+        self._clipping_path = to_qpainter_path([clipping_path])
+
+    def shape(self):
+        return self._clipping_path
+
+
+# The key used to store the dxf entity corresponding to each graphics element
+CorrespondingDXFEntity = qc.Qt.UserRole + 0  # type: ignore
+CorrespondingDXFParentStack = qc.Qt.UserRole + 1  # type: ignore
+
+
+class PyQtBackend(Backend):
+    """
+    Backend which uses the :mod:`PySide6` package to implement an interactive
+    viewer. The :mod:`PyQt5` package can be used as fallback if the :mod:`PySide6`
+    package is not available.
+
+    Args:
+        scene: drawing canvas of type :class:`QtWidgets.QGraphicsScene`,
+            if ``None`` a new canvas will be created
+        extra_lineweight_scaling: compared to other backends,
+            PyQt draws lines which appear thinner
+    """
 
-    @abstractmethod
-    def draw_text(
+    def __init__(
         self,
-        text: str,
-        transform: Matrix44,
-        properties: Properties,
-        cap_height: float,
-    ) -> None:
-        raise NotImplementedError
+        scene: Optional[qw.QGraphicsScene] = None,
+        *,
+        debug_draw_rect: bool = False,
+        extra_lineweight_scaling: float = 2.0,
+    ):
+        super().__init__()
+        self._scene = scene or qw.QGraphicsScene()  # avoids many type errors
+        self._color_cache: dict[Color, qg.QColor] = {}
+        self._pattern_cache: dict[PatternKey, int] = {}
+        self._no_line = qg.QPen(qc.Qt.NoPen)
+        self._no_fill = qg.QBrush(qc.Qt.NoBrush)
+        self._extra_lineweight_scaling = extra_lineweight_scaling
+        self._debug_draw_rect = debug_draw_rect
 
-    @abstractmethod
-    def get_font_measurements(
-        self, cap_height: float, font: Optional[FontFace] = None
-    ) -> FontMeasurements:
-        raise NotImplementedError
-
-    @abstractmethod
-    def get_text_line_width(
-        self, text: str, cap_height: float, font: Optional[FontFace] = None
-    ) -> float:
-        raise NotImplementedError
-
-    @abstractmethod
-    def clear(self) -> None:
-        raise NotImplementedError
+    def configure(self, config: Configuration) -> None:
+        if config.min_lineweight is None:
+            config = config.with_changes(min_lineweight=0.24)
+        super().configure(config)
+
+    def set_scene(self, scene: qw.QGraphicsScene):
+        self._scene = scene
+
+    def _add_item(self, item):
+        self._set_item_data(item)
+        self._scene.addItem(item)
+
+    def _get_color(self, color: Color) -> qg.QColor:
+        qt_color = self._color_cache.get(color, None)
+        if qt_color is None:
+            if len(color) == 7:
+                qt_color = qg.QColor(color)  # '#RRGGBB'
+            elif len(color) == 9:
+                rgb = color[1:7]
+                alpha = color[7:9]
+                qt_color = qg.QColor(f"#{alpha}{rgb}")  # '#AARRGGBB'
+            else:
+                raise TypeError(color)
 
-    @abstractmethod
-    def finalize(self) -> None:
-        raise NotImplementedError
+            self._color_cache[color] = qt_color
+        return qt_color
 
-    @abstractmethod
-    def set_clipping_path(
-        self, path: Optional[Path] = None, scale: float = 1.0
-    ) -> bool:
-        """Set the current clipping path.
-        Returns True if a clipping path is supported.
-        An empty path or None removes the clipping path.
-        The `scale` is the scaling factor from modelspace to viewport.
+    def _get_pen(self, properties: Properties) -> qg.QPen:
+        """Returns a cosmetic pen with applied lineweight but without line type
+        support.
         """
-        raise NotImplementedError
-
+        px = (
+            properties.lineweight
+            / 0.3527
+            * self.config.lineweight_scaling
+            * self._extra_lineweight_scaling
+        )
+        pen = qg.QPen(self._get_color(properties.color), px)
+        # Use constant width in pixel:
+        pen.setCosmetic(True)
+        pen.setJoinStyle(qc.Qt.RoundJoin)
+        return pen
+
+    def _get_brush(self, properties: Properties) -> qg.QBrush:
+        # Hatch patterns are handled by the frontend since v0.18.1
+        filling = properties.filling
+        if filling:
+            return qg.QBrush(self._get_color(properties.color), qc.Qt.SolidPattern)  # type: ignore
+        return self._no_fill
+
+    def _set_item_data(self, item: qw.QGraphicsItem) -> None:
+        parent_stack = tuple(e for e, props in self.entity_stack[:-1])
+        current_entity = self.current_entity
+        if isinstance(item, list):
+            for item_ in item:
+                item_.setData(CorrespondingDXFEntity, current_entity)
+                item_.setData(CorrespondingDXFParentStack, parent_stack)
+        else:
+            item.setData(CorrespondingDXFEntity, current_entity)
+            item.setData(CorrespondingDXFParentStack, parent_stack)
 
-class Backend(BackendInterface, metaclass=ABCMeta):
-    def __init__(self) -> None:
-        self.entity_stack: list[tuple[DXFGraphic, Properties]] = []
-        self.config: Configuration
-
-    def configure(self, config: Configuration) -> None:
-        self.config = config
+    def set_background(self, color: Color):
+        self._scene.setBackgroundBrush(qg.QBrush(self._get_color(color)))
 
-    def enter_entity(self, entity: DXFGraphic, properties: Properties) -> None:
-        self.entity_stack.append((entity, properties))
-
-    def exit_entity(self, entity: DXFGraphic) -> None:
-        e, p = self.entity_stack.pop()
-        assert e is entity, "entity stack mismatch"
-
-    @property
-    def current_entity(self) -> Optional[DXFGraphic]:
-        """Obtain the current entity being drawn"""
-        return self.entity_stack[-1][0] if self.entity_stack else None
-
-    @abstractmethod
-    def set_background(self, color: Color) -> None:
-        raise NotImplementedError
-
-    def set_clipping_path(
-        self, path: Optional[Path] = None, scale: float = 1.0
-    ) -> bool:
-        """Clipping path is not supported by default."""
-        return False
-
-    @abstractmethod
     def draw_point(self, pos: Vec3, properties: Properties) -> None:
-        """Draw a real dimensionless point, because not all backends support
-        zero-length lines!
-        """
-        raise NotImplementedError
+        """Draw a real dimensionless point."""
+        brush = qg.QBrush(self._get_color(properties.color), qc.Qt.SolidPattern)
+        item = _Point(pos.x, pos.y, brush)
+        self._set_item_data(item)
+        self._add_item(item)
 
-    @abstractmethod
     def draw_line(self, start: Vec3, end: Vec3, properties: Properties) -> None:
-        raise NotImplementedError
+        # PyQt draws a long line for a zero-length line:
+        if start.isclose(end):
+            self.draw_point(start, properties)
+        else:
+            item = qw.QGraphicsLineItem(start.x, start.y, end.x, end.y)
+            item.setPen(self._get_pen(properties))
+            self._add_item(item)
 
     def draw_solid_lines(
-        self, lines: Iterable[tuple[Vec3, Vec3]], properties: Properties
-    ) -> None:
+        self,
+        lines: Iterable[tuple[Vec3, Vec3]],
+        properties: Properties,
+    ):
         """Fast method to draw a bunch of solid lines with the same properties."""
-        # Must be overridden by the backend to gain a performance benefit.
-        # This is the default implementation to ensure compatibility with
-        # existing backends.
+        pen = self._get_pen(properties)
+        add_line = self._add_item
         for s, e in lines:
-            if e.isclose(s):
+            if s.isclose(e):
                 self.draw_point(s, properties)
             else:
-                self.draw_line(s, e, properties)
+                item = qw.QGraphicsLineItem(s.x, s.y, e.x, e.y)
+                item.setPen(pen)
+                add_line(item)
 
     def draw_path(self, path: Path, properties: Properties) -> None:
-        """Draw an outline path (connected string of line segments and Bezier
-        curves).
-
-        The :meth:`draw_path` implementation is a fall-back implementation
-        which approximates Bezier curves by flattening as line segments.
-        Backends can override this method if better path drawing functionality
-        is available for that backend.
-
-        """
-        if len(path):
-            vertices = iter(
-                path.flattening(distance=self.config.max_flattening_distance)
-            )
-            prev = next(vertices)
-            for vertex in vertices:
-                self.draw_line(prev, vertex, properties)
-                prev = vertex
+        item = qw.QGraphicsPathItem(to_qpainter_path([path]))
+        item.setPen(self._get_pen(properties))
+        item.setBrush(self._no_fill)
+        self._add_item(item)
 
     def draw_filled_paths(
         self,
         paths: Iterable[Path],
         holes: Iterable[Path],
         properties: Properties,
     ) -> None:
-        """Draw multiple filled paths (connected string of line segments and
-        Bezier curves) with holes.
-
-        The strategy to draw multiple paths at once was chosen, because a HATCH
-        entity can contain multiple unconnected areas and the holes are not easy
-        to assign to an external path.
-
-        The idea is to put all filled areas into `paths` (counter-clockwise
-        winding) and all holes into `holes` (clockwise winding) and look what
-        the backend does with this information.
-
-        The HATCH fill strategies ("ignore", "outermost", "ignore") are resolved
-        by the frontend e.g. the holes sequence is empty for the "ignore"
-        strategy and for the "outermost" strategy, holes do not contain nested
-        holes.
-
-        The default implementation draws all paths as filled polygon without
-        holes by the :meth:`draw_filled_polygon` method. Backends can override
-        this method if filled polygon with hole support is available.
-
-        Args:
-            paths: sequence of exterior paths (counter-clockwise winding)
-            holes: sequence of holes (clockwise winding)
-            properties: HATCH properties
-
-        """
+        oriented_paths: list[Path] = []
         for path in paths:
-            self.draw_filled_polygon(
-                path.flattening(distance=self.config.max_flattening_distance),
-                properties,
-            )
+            try:
+                path = path.counter_clockwise()
+            except ValueError:  # cannot detect path orientation
+                continue
+            oriented_paths.append(path)
+        for path in holes:
+            try:
+                path = path.clockwise()
+            except ValueError:  # cannot detect path orientation
+                continue
+            oriented_paths.append(path)
+        if len(oriented_paths) == 0:
+            return
+        item = _CosmeticPath(to_qpainter_path(oriented_paths))
+        item.setPen(self._get_pen(properties))
+        item.setBrush(self._get_brush(properties))
+        self._add_item(item)
 
-    @abstractmethod
     def draw_filled_polygon(
         self, points: Iterable[Vec3], properties: Properties
     ) -> None:
-        """Fill a polygon whose outline is defined by the given points.
-        Used to draw entities with simple outlines where :meth:`draw_path` may
-        be an inefficient way to draw such a polygon.
-        """
-        raise NotImplementedError
+        brush = self._get_brush(properties)
+        polygon = qg.QPolygonF()
+        for p in points:
+            polygon.append(qc.QPointF(p.x, p.y))
+        item = _CosmeticPolygon(polygon)
+        item.setPen(self._no_line)
+        item.setBrush(brush)
+        self._add_item(item)
+
+    def clear(self) -> None:
+        self._scene.clear()
+
+    def finalize(self) -> None:
+        super().finalize()
+        self._scene.setSceneRect(self._scene.itemsBoundingRect())
+        if self._debug_draw_rect:
+            properties = Properties()
+            properties.color = "#000000"
+            self._scene.addRect(
+                self._scene.sceneRect(),
+                self._get_pen(properties),
+                self._no_fill,
+            )
 
-    @abstractmethod
-    def draw_text(
+
+class _CosmeticPath(qw.QGraphicsPathItem):
+    def paint(
         self,
-        text: str,
-        transform: Matrix44,
-        properties: Properties,
-        cap_height: float,
+        painter: qg.QPainter,
+        option: qw.QStyleOptionGraphicsItem,
+        widget: Optional[qw.QWidget] = None,
     ) -> None:
-        """Draw a single line of text with the anchor point at the baseline
-        left point.
-        """
-        raise NotImplementedError
+        _set_cosmetic_brush(self, painter)
+        super().paint(painter, option, widget)
 
-    @abstractmethod
-    def get_font_measurements(
-        self, cap_height: float, font: Optional[FontFace] = None
-    ) -> "FontMeasurements":
-        """Note: backends might want to cache the results of these calls"""
-        raise NotImplementedError
-
-    @abstractmethod
-    def get_text_line_width(
-        self, text: str, cap_height: float, font: Optional[FontFace] = None
-    ) -> float:
-        """Get the width of a single line of text."""
-        # https://stackoverflow.com/questions/32555015/how-to-get-the-visual-length-of-a-text-string-in-python
-        # https://stackoverflow.com/questions/4190667/how-to-get-width-of-a-truetype-font-character-in-1200ths-of-an-inch-with-python
-        raise NotImplementedError
 
-    @abstractmethod
-    def clear(self) -> None:
-        """Clear the canvas. Does not reset the internal state of the backend.
-        Make sure that the previous drawing is finished before clearing.
+class _CosmeticPolygon(qw.QGraphicsPolygonItem):
+    def paint(
+        self,
+        painter: qg.QPainter,
+        option: qw.QStyleOptionGraphicsItem,
+        widget: Optional[qw.QWidget] = None,
+    ) -> None:
+        _set_cosmetic_brush(self, painter)
+        super().paint(painter, option, widget)
 
-        """
-        raise NotImplementedError
 
-    def finalize(self) -> None:
-        pass
+def _set_cosmetic_brush(
+    item: qw.QAbstractGraphicsShapeItem, painter: qg.QPainter
+) -> None:
+    """like a cosmetic pen, this sets the brush pattern to appear the same independent of the view"""
+    brush = item.brush()
+    # scale by -1 in y because the view is always mirrored in y and undoing the view transformation entirely would make
+    # the hatch mirrored w.r.t the view
+    brush.setTransform(painter.transform().inverted()[0].scale(1, -1))  # type: ignore
+    item.setBrush(brush)
+
+
+def _get_x_scale(t: qg.QTransform) -> float:
+    return math.sqrt(t.m11() * t.m11() + t.m21() * t.m21())
+
+
+def _matrix_to_qtransform(matrix: Matrix44) -> qg.QTransform:
+    """Qt also uses row-vectors so the translation elements are placed in the
+    bottom row.
 
+    This is only a simple conversion which assumes that although the
+    transformation is 4x4,it does not involve the z axis.
 
-def prepare_string_for_rendering(text: str, dxftype: str) -> str:
-    assert "\n" not in text, "not a single line of text"
-    if dxftype in {"TEXT", "ATTRIB", "ATTDEF"}:
-        text = replace_non_printable_characters(text, replacement="?")
-        text = text.replace("\t", "?")
-    elif dxftype == "MTEXT":
-        text = replace_non_printable_characters(text, replacement="▯")
-        text = text.replace("\t", "        ")
-    else:
-        raise TypeError(dxftype)
-    return text
+    A more correct transformation could be implemented like so:
+    https://stackoverflow.com/questions/10629737/convert-3d-4x4-rotation-matrix-into-2d
+    """
+    return qg.QTransform(*matrix.get_2d_transformation())
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/config.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/config.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/frontend.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/frontend.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,27 +21,29 @@
 import ezdxf.bbox
 from ezdxf.addons.drawing.config import (
     Configuration,
     ProxyGraphicPolicy,
     HatchPolicy,
 )
 from ezdxf.addons.drawing.backend import BackendInterface
+from ezdxf.addons.drawing.clipper import ClippingRect
 from ezdxf.addons.drawing.properties import (
     RenderContext,
     VIEWPORT_COLOR,
     OLE2FRAME_COLOR,
     Properties,
     Filling,
     LayoutProperties,
 )
 from ezdxf.addons.drawing.config import LinePolicy
 from ezdxf.addons.drawing.text import simplified_text_chunks
 from ezdxf.addons.drawing.type_hints import FilterFunc
 from ezdxf.addons.drawing.gfxproxy import DXFGraphicProxy
 from ezdxf.addons.drawing.mtext_complex import complex_mtext_renderer
+from ezdxf.addons.drawing.unified_text_renderer import UnifiedTextRenderer
 from ezdxf.entities import (
     DXFEntity,
     DXFGraphic,
     Insert,
     MText,
     Polyline,
     LWPolyline,
@@ -54,30 +56,37 @@
     Point,
     Viewport,
 )
 from ezdxf.entities.attrib import BaseAttrib
 from ezdxf.entities.polygon import DXFPolygon
 from ezdxf.entities.boundary_paths import AbstractBoundaryPath
 from ezdxf.layouts import Layout
-from ezdxf.math import Vec2, Vec3, OCS, NULLVEC, Matrix44
+from ezdxf.math import Vec2, Vec3, OCS, NULLVEC, Matrix44, AnyVec
 from ezdxf.path import (
     Path,
+    Path2d,
     make_path,
     from_hatch_boundary_path,
     fast_bbox_detection,
     winding_deconstruction,
     from_vertices,
+    single_paths,
 )
 from ezdxf.render import MeshBuilder, TraceBuilder, linetypes
 from ezdxf import reorder
 from ezdxf.proxygraphic import ProxyGraphic, ProxyGraphicError
 from ezdxf.protocols import SupportsVirtualEntities, virtual_entities
-from ezdxf.tools.text import has_inline_formatting_codes
+from ezdxf.tools.text import (
+    has_inline_formatting_codes,
+    replace_non_printable_characters,
+)
 from ezdxf.lldxf import const
 from ezdxf.render import hatching
+from ezdxf.tools import fonts
+
 
 __all__ = ["Frontend"]
 
 
 TDispatchTable: TypeAlias = Dict[str, Callable[[DXFGraphic, Properties], None]]
 PatternKey: TypeAlias = Tuple[str, float]
 
@@ -146,14 +155,18 @@
         # this can speed up rendering time if multiple viewports are present.
         # If the bbox_cache is not ``None``, entities not in cache will be
         # added dynamically. This is only beneficial when rendering multiple
         # viewports, as the upfront bounding box calculation adds some rendering
         # time.
         self._bbox_cache = bbox_cache
 
+    @property
+    def text_engine(self):
+        return self._designer.text_engine
+
     def _build_dispatch_table(self) -> TDispatchTable:
         dispatch_table: TDispatchTable = {
             "POINT": self.draw_point_entity,
             "HATCH": self.draw_hatch_entity,
             "MPOLYGON": self.draw_mpolygon_entity,
             "MESH": self.draw_mesh_entity,
             "VIEWPORT": self.draw_viewport_entity,
@@ -179,17 +192,15 @@
         """Log given message - override to alter behavior."""
         logger.info(message)
 
     def skip_entity(self, entity: DXFEntity, msg: str) -> None:
         """Called for skipped entities - override to alter behavior."""
         self.log_message(f'skipped entity {str(entity)}. Reason: "{msg}"')
 
-    def override_properties(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def override_properties(self, entity: DXFGraphic, properties: Properties) -> None:
         """The :meth:`override_properties` filter can change the properties of
         an entity independent of the DXF attributes.
 
         This filter has access to the DXF attributes by the `entity` object,
         the current render context, and the resolved properties by the
         `properties` object. It is recommended to modify only the `properties`
         object in this filter.
@@ -224,17 +235,15 @@
         """
         if layout_properties is not None:
             # TODO: this does not work, layer properties have to be re-evaluated!
             self.ctx.current_layout_properties = layout_properties
         else:
             self.ctx.set_current_layout(layout)
         # set background before drawing entities
-        self.out.set_background(
-            self.ctx.current_layout_properties.background_color
-        )
+        self.out.set_background(self.ctx.current_layout_properties.background_color)
         self.parent_stack = []
         handle_mapping = list(layout.get_redraw_order())
         if handle_mapping:
             self.draw_entities(
                 reorder.ascending(layout, handle_mapping),
                 filter_func=filter_func,
             )
@@ -286,27 +295,24 @@
                 # The __virtual_entities__() protocol does not distinguish
                 # content from DXF entities or from proxy graphic.
                 # In the long run ACAD_PROXY_ENTITY should be the only
                 # supported DXF entity which uses proxy graphic. Unsupported
                 # DXF entities (DXFGraphicProxy) do not get to this point if
                 # proxy graphic is ignored.
                 if (
-                    self.config.proxy_graphic_policy
-                    != ProxyGraphicPolicy.IGNORE
+                    self.config.proxy_graphic_policy != ProxyGraphicPolicy.IGNORE
                     or entity.dxftype() not in self._proxy_graphic_only_entities
                 ):
                     self.draw_composite_entity(entity, properties)
             else:
                 self.skip_entity(entity, "unsupported")
 
         self.out.exit_entity(entity)
 
-    def draw_line_entity(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def draw_line_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         d, dxftype = entity.dxf, entity.dxftype()
         if dxftype == "LINE":
             self._designer.draw_line(d.start, d.end, properties)
 
         elif dxftype in ("XLINE", "RAY"):
             start = d.start
             delta = d.unit_vector * self.config.infinite_line_length
@@ -315,78 +321,74 @@
                     start - delta / 2, start + delta / 2, properties
                 )
             elif dxftype == "RAY":
                 self._designer.draw_line(start, start + delta, properties)
         else:
             raise TypeError(dxftype)
 
-    def draw_text_entity(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def draw_text_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         # Draw embedded MTEXT entity as virtual MTEXT entity:
         if isinstance(entity, BaseAttrib) and entity.has_embedded_mtext_entity:
             self.draw_mtext_entity(entity.virtual_mtext_entity(), properties)
         elif is_spatial_text(Vec3(entity.dxf.extrusion)):
             self.draw_text_entity_3d(entity, properties)
         else:
             self.draw_text_entity_2d(entity, properties)
 
-    def draw_text_entity_2d(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def get_font_face(self, properties: Properties) -> fonts.FontFace:
+        font_face = properties.font
+        if font_face is None:
+            return self._designer.default_font_face
+        return font_face
+
+    def draw_text_entity_2d(self, entity: DXFGraphic, properties: Properties) -> None:
         if isinstance(entity, Text):
             for line, transform, cap_height in simplified_text_chunks(
-                entity, self.out, font=properties.font
+                entity, self.text_engine, font_face=self.get_font_face(properties)
             ):
                 self._designer.draw_text(
-                    line, transform, properties, cap_height
+                    line, transform, properties, cap_height, entity.dxftype()
                 )
         else:
             raise TypeError(entity.dxftype())
 
-    def draw_text_entity_3d(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def draw_text_entity_3d(self, entity: DXFGraphic, properties: Properties) -> None:
         self.skip_entity(entity, "3D text not supported")
 
-    def draw_mtext_entity(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def draw_mtext_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         mtext = cast(MText, entity)
         if is_spatial_text(Vec3(mtext.dxf.extrusion)):
             self.skip_entity(mtext, "3D MTEXT not supported")
             return
         if mtext.has_columns or has_inline_formatting_codes(mtext.text):
             self.draw_complex_mtext(mtext, properties)
         else:
             self.draw_simple_mtext(mtext, properties)
 
     def draw_simple_mtext(self, mtext: MText, properties: Properties) -> None:
         """Draw the content of a MTEXT entity without inline formatting codes."""
         for line, transform, cap_height in simplified_text_chunks(
-            mtext, self.out, font=properties.font
+            mtext, self.text_engine, font_face=self.get_font_face(properties)
         ):
-            self._designer.draw_text(line, transform, properties, cap_height)
+            self._designer.draw_text(
+                line, transform, properties, cap_height, mtext.dxftype()
+            )
 
     def draw_complex_mtext(self, mtext: MText, properties: Properties) -> None:
         """Draw the content of a MTEXT entity including inline formatting codes."""
         complex_mtext_renderer(self.ctx, self._designer, mtext, properties)
 
-    def draw_curve_entity(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def draw_curve_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         try:
             path = make_path(entity)
         except AttributeError:  # API usage error
             raise TypeError(f"Unsupported DXF type {entity.dxftype()}")
         self._designer.draw_path(path, properties)
 
-    def draw_point_entity(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def draw_point_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         point = cast(Point, entity)
         pdmode = self.config.pdmode
         pdsize = self.config.pdsize
         assert pdmode is not None
         assert pdsize is not None
 
         # Defpoints are regular POINT entities located at the "defpoints" layer:
@@ -410,17 +412,15 @@
                         self._designer.draw_line(start, end, properties)
                     pass
                 elif dxftype == "CIRCLE":
                     self.draw_curve_entity(entity, properties)
                 else:
                     raise ValueError(dxftype)
 
-    def draw_solid_entity(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def draw_solid_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         if isinstance(entity, Face3d):
             dxf = entity.dxf
             try:
                 # this implementation supports all features of example file:
                 # examples_dxf/3dface.dxf without changing the behavior of
                 # Face3d.wcs_vertices() which removes the last vertex if
                 # duplicated.
@@ -442,17 +442,15 @@
             # set solid fill type for SOLID and TRACE
             properties.filling = Filling()
             self._designer.draw_filled_polygon(
                 entity.wcs_vertices(close=False), properties
             )
 
         else:
-            raise TypeError(
-                "API error, requires a SOLID, TRACE or 3DFACE entity"
-            )
+            raise TypeError("API error, requires a SOLID, TRACE or 3DFACE entity")
 
     def draw_hatch_pattern(
         self, polygon: DXFPolygon, paths: list[Path], properties: Properties
     ):
         if polygon.pattern is None or len(polygon.pattern.lines) == 0:
             return
         ocs = polygon.ocs()
@@ -500,39 +498,37 @@
         elif self.config.hatch_policy == HatchPolicy.SHOW_OUTLINE:
             filling = Filling()  # solid filling
             show_only_outline = True
 
         polygon = cast(DXFPolygon, entity)
         if filling.type == Filling.PATTERN:
             if loops is None:
-                loops = hatching.hatch_boundary_paths(
-                    polygon, filter_text_boxes=True
-                )
+                loops = hatching.hatch_boundary_paths(polygon, filter_text_boxes=True)
             self.draw_hatch_pattern(polygon, loops, properties)
             return
 
         # draw SOLID filling
         ocs = polygon.ocs()
         # all OCS coordinates have the same z-axis stored as vector (0, 0, z),
         # default (0, 0, 0)
         elevation = entity.dxf.elevation.z
 
         external_paths: list[Path]
         holes: list[Path]
 
         if loops is not None:  # only MPOLYGON
-            external_paths, holes = winding_deconstruction(
+            external_paths, holes = winding_deconstruction(  # type: ignore
                 fast_bbox_detection(loops)
             )
         else:  # only HATCH
             paths = polygon.paths.rendering_paths(polygon.dxf.hatch_style)
             polygons: list = fast_bbox_detection(
                 closed_loops(paths, ocs, elevation)  # type: ignore
             )
-            external_paths, holes = winding_deconstruction(polygons)
+            external_paths, holes = winding_deconstruction(polygons)  # type: ignore
 
         if show_only_outline:
             for p in itertools.chain(ignore_text_boxes(external_paths), holes):
                 self._designer.draw_path(p, properties)
             return
 
         if external_paths:
@@ -542,35 +538,30 @@
         elif holes:
             # The first path is considered the exterior path, everything else is
             # holes.
             self._designer.draw_filled_paths([holes[0]], holes[1:], properties)
 
     def draw_mpolygon_entity(self, entity: DXFGraphic, properties: Properties):
         def resolve_fill_color() -> str:
-            return self.ctx.resolve_aci_color(
-                entity.dxf.fill_color, properties.layer
-            )
+            return self.ctx.resolve_aci_color(entity.dxf.fill_color, properties.layer)
 
         polygon = cast(DXFPolygon, entity)
         ocs = polygon.ocs()
         elevation: float = polygon.dxf.elevation.z
         offset = Vec3(polygon.dxf.get("offset_vector", NULLVEC))
         # MPOLYGON does not support hatch styles, all paths are rendered.
         loops = closed_loops(polygon.paths, ocs, elevation, offset)  # type: ignore
 
         line_color: str = properties.color
         assert properties.filling is not None
         pattern_name: str = properties.filling.name  # normalized pattern name
         # 1. draw filling
         if polygon.dxf.solid_fill:
             properties.filling.type = Filling.SOLID
-            if (
-                polygon.gradient is not None
-                and polygon.gradient.number_of_colors > 0
-            ):
+            if polygon.gradient is not None and polygon.gradient.number_of_colors > 0:
                 # true color filling is stored as gradient
                 properties.color = str(properties.filling.gradient_color1)
             else:
                 properties.color = resolve_fill_color()
             self.draw_hatch_entity(entity, properties, loops=loops)
 
         # checking properties.filling.type == Filling.PATTERN is not sufficient:
@@ -580,26 +571,22 @@
 
         # 2. draw boundary paths
         properties.color = line_color
         # draw boundary paths as lines
         for loop in loops:
             self._designer.draw_path(loop, properties)
 
-    def draw_wipeout_entity(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def draw_wipeout_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         wipeout = cast(Wipeout, entity)
         properties.filling = Filling()
         properties.color = self.ctx.current_layout_properties.background_color
         path = wipeout.boundary_path_wcs()
         self._designer.draw_filled_polygon(path, properties)
 
-    def draw_viewport_entity(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def draw_viewport_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         assert isinstance(entity, Viewport)
         vp = entity
         # Special VIEWPORT id == 1, this viewport defines the "active viewport"
         # which is the area currently shown in the layout tab by the CAD
         # application.
         # BricsCAD set id to -1 if the viewport is off and 'status' (group
         # code 68) is not present.
@@ -608,17 +595,15 @@
         if not vp.is_top_view:
             self.log_message("Cannot render non top-view viewports")
             return
         if not self._designer.draw_viewport(vp, self.ctx, self._bbox_cache):
             # viewports are not supported by the backend
             self._draw_filled_rect(vp.clipping_rect_corners(), VIEWPORT_COLOR)
 
-    def draw_ole2frame_entity(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def draw_ole2frame_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         ole2frame = cast(OLE2Frame, entity)
         bbox = ole2frame.bbox()
         if not bbox.is_empty:
             self._draw_filled_rect(bbox.rect_vertices(), OLE2FRAME_COLOR)
 
     def _draw_filled_rect(
         self,
@@ -627,31 +612,27 @@
     ) -> None:
         props = Properties()
         props.color = color
         # default SOLID filling
         props.filling = Filling()
         self._designer.draw_filled_polygon(Vec3.list(points), props)
 
-    def draw_mesh_entity(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def draw_mesh_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         builder = MeshBuilder.from_mesh(entity)  # type: ignore
         self.draw_mesh_builder_entity(builder, properties)
 
     def draw_mesh_builder_entity(
         self, builder: MeshBuilder, properties: Properties
     ) -> None:
         for face in builder.faces_as_vertices():
             self._designer.draw_path(
                 from_vertices(face, close=True), properties=properties
             )
 
-    def draw_polyline_entity(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def draw_polyline_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         dxftype = entity.dxftype()
         if dxftype == "POLYLINE":
             e = cast(Polyface, entity)
             if e.is_polygon_mesh or e.is_poly_face_mesh:
                 # draw 3D mesh or poly-face entity
                 self.draw_mesh_builder_entity(
                     MeshBuilder.from_polyface(e),
@@ -686,17 +667,15 @@
                 properties.filling = Filling()
                 self._designer.draw_filled_polygon(points, properties)
             return
 
         path = make_path(entity)
         self._designer.draw_path(path, properties)
 
-    def draw_composite_entity(
-        self, entity: DXFGraphic, properties: Properties
-    ) -> None:
+    def draw_composite_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         def draw_insert(insert: Insert):
             self.draw_entities(insert.attribs)
             # draw_entities() includes the visibility check:
             self.draw_entities(
                 insert.virtual_entities(
                     skipped_entity_callback=self.skip_entity
                     # TODO: redraw_order=True?
@@ -777,25 +756,25 @@
     """
 
     def __init__(self, frontend: Frontend, backend: BackendInterface):
         self.frontend = frontend
         self.backend = backend
         self.config = frontend.config
         self.pattern_cache: dict[PatternKey, Sequence[float]] = dict()
-        self.transformation: Optional[Matrix44] = None
-        # scaling factor from modelspace to viewport
-        self.scale: float = 1.0
-        self.clipping_path: Path = Path()
+        self.text_engine = UnifiedTextRenderer()
+        self.default_font_face = self.text_engine.default_font_face
+        self.clipper = ClippingRect()
+        self.current_vp_scale = 1.0
 
     @property
     def vp_ltype_scale(self) -> float:
         """The linetype pattern should look the same in all viewports
         independent of the viewport scaling.
         """
-        return 1.0 / max(self.scale, 0.0001)  # max out at 1:10000
+        return 1.0 / max(self.current_vp_scale, 0.0001)  # max out at 1:10000
 
     def draw_viewport(
         self,
         vp: Viewport,
         layout_ctx: RenderContext,
         bbox_cache: Optional[ezdxf.bbox.Cache] = None,
     ) -> bool:
@@ -804,150 +783,175 @@
         """
         if vp.doc is None:
             return False
         try:
             msp_limits = vp.get_modelspace_limits()
         except ValueError:  # modelspace limits not detectable
             return False
-        if self.set_viewport(vp):
+        if self.enter_viewport(vp):
             _draw_entities(
                 self.frontend,
                 layout_ctx.from_viewport(vp),
                 filter_vp_entities(vp.doc.modelspace(), msp_limits, bbox_cache),
             )
-            self.reset_viewport()
+            self.exit_viewport()
             return True
         return False
 
-    def set_viewport(self, vp: Viewport) -> bool:
+    def enter_viewport(self, vp: Viewport) -> bool:
         """Set current viewport. Returns ``False`` if the backend doesn't
         support viewports.
         """
-        self.scale = vp.get_scale()
-        self.transformation = vp.get_transformation_matrix()
-        self.clipping_path = make_path(vp)
-        if not self.backend.set_clipping_path(self.clipping_path, self.scale):
-            self.reset_viewport()
-            return False
-        return True
+        self.current_vp_scale = vp.get_scale()
+        m = vp.get_transformation_matrix()
+        clipping_path = make_path(vp)
+        if len(clipping_path):
+            self.clipper.push(clipping_path, m)
+            return True
+        return False
 
-    def reset_viewport(self) -> None:
-        self.scale = 1.0
-        self.transformation = None
-        self.clipping_path = Path()
-        self.backend.set_clipping_path(None)
-
-    def draw_point(self, pos: Vec3, properties: Properties) -> None:
-        if self.transformation:
-            pos = self.transformation.transform(pos)
+    def exit_viewport(self):
+        self.clipper.pop()
+        self.current_vp_scale = 1.0
+
+    def draw_point(self, pos: AnyVec, properties: Properties) -> None:
+        if self.clipper.is_active:
+            point = self.clipper.clip_point(pos)
+            if point is None:
+                return
+            pos = point
         self.backend.draw_point(pos, properties)
 
-    def draw_line(self, start: Vec3, end: Vec3, properties: Properties):
+    def draw_line(self, start: AnyVec, end: AnyVec, properties: Properties):
         if (
             self.config.line_policy == LinePolicy.SOLID
             or len(properties.linetype_pattern) < 2  # CONTINUOUS
         ):
-            if self.transformation:
-                start = self.transformation.transform(start)
-                end = self.transformation.transform(end)
-            self.backend.draw_line(start, end, properties)
+            if self.clipper.is_active:
+                points = self.clipper.clip_line(start, end)
+                if points:
+                    self.backend.draw_line(start, end, properties)
+            else:
+                self.backend.draw_line(start, end, properties)
         else:
             renderer = linetypes.LineTypeRenderer(self.pattern(properties))
             self.draw_solid_lines(  # including transformation
                 ((s, e) for s, e in renderer.line_segment(start, end)),
                 properties,
             )
 
     def draw_solid_lines(
-        self, lines: Iterable[tuple[Vec3, Vec3]], properties: Properties
+        self, lines: Iterable[tuple[AnyVec, AnyVec]], properties: Properties
     ) -> None:
-        if self.transformation:
-            t = self.transformation.transform
-            lines = [(t(p0), t(p1)) for p0, p1 in lines]
+        if self.clipper.is_active:
+            clipped_lines: list[Sequence[AnyVec]] = []
+            for start, end in lines:
+                points = self.clipper.clip_line(start, end)
+                if points:
+                    clipped_lines.append(points)
+            lines = clipped_lines  # type: ignore
         self.backend.draw_solid_lines(lines, properties)
 
-    def draw_path(self, path: Path, properties: Properties):
+    def draw_path(self, path: Path | Path2d, properties: Properties):
         if (
             self.config.line_policy == LinePolicy.SOLID
             or len(properties.linetype_pattern) < 2  # CONTINUOUS
         ):
-            if self.transformation:
-                path = path.transform(self.transformation)
+            if self.clipper.is_active:
+                for clipped_path in self.clipper.clip_paths(
+                    [path], self.config.max_flattening_distance
+                ):
+                    self.backend.draw_path(clipped_path, properties)
+                return
             self.backend.draw_path(path, properties)
         else:
             renderer = linetypes.LineTypeRenderer(self.pattern(properties))
-            vertices = path.flattening(
-                self.config.max_flattening_distance, segments=16
-            )
+            vertices = path.flattening(self.config.max_flattening_distance, segments=16)
             self.draw_solid_lines(
                 ((s, e) for s, e in renderer.line_segments(vertices)),
                 properties,
             )
 
     def draw_filled_paths(
         self,
-        paths: Iterable[Path],
-        holes: Iterable[Path],
+        paths: Iterable[Path | Path2d],
+        holes: Iterable[Path | Path2d],
         properties: Properties,
     ) -> None:
-        if self.transformation:
-            paths = [p.transform(self.transformation) for p in paths]
-            holes = [h.transform(self.transformation) for h in holes]
+        if self.clipper.is_active:
+            m = self.clipper.m
+            max_sagitta = self.config.max_flattening_distance
+            paths = self.clipper.clip_filled_paths(
+                (p.transform(m) for p in paths), max_sagitta
+            )
+            holes = self.clipper.clip_filled_paths(
+                (h.transform(m) for h in holes), max_sagitta
+            )
         self.backend.draw_filled_paths(paths, holes, properties)
 
     def draw_filled_polygon(
-        self, points: Iterable[Vec3], properties: Properties
+        self, points: Iterable[AnyVec], properties: Properties
     ) -> None:
-        if self.transformation:
-            t = self.transformation.transform
-            points = [t(p) for p in points]
+        if self.clipper.is_active:
+            points = self.clipper.clip_polygon(points)
         self.backend.draw_filled_polygon(points, properties)
 
-    def draw_text(
-        self,
-        text: str,
-        transform: Matrix44,
-        properties: Properties,
-        cap_height: float,
-    ) -> None:
-        if self.transformation:
-            transform *= self.transformation
-        self.backend.draw_text(text, transform, properties, cap_height)
-
     def pattern(self, properties: Properties) -> Sequence[float]:
         """Get pattern - implements pattern caching."""
         if self.config.line_policy == LinePolicy.SOLID:
             scale = 0.0
         else:
             scale = properties.linetype_scale * self.vp_ltype_scale
 
         key: PatternKey = (properties.linetype_name, scale)
         pattern_ = self.pattern_cache.get(key)
         if pattern_ is None:
             pattern_ = self.create_pattern(properties, scale)
             self.pattern_cache[key] = pattern_
         return pattern_
 
-    def create_pattern(
-        self, properties: Properties, scale: float
-    ) -> Sequence[float]:
+    def create_pattern(self, properties: Properties, scale: float) -> Sequence[float]:
         """Returns simplified linetype tuple: on-off sequence"""
         if len(properties.linetype_pattern) < 2:
             # Do not return None -> None indicates: "not cached"
             return tuple()
         else:
             min_dash_length = self.config.min_dash_length * self.vp_ltype_scale
             pattern = [
-                max(e * scale, min_dash_length)
-                for e in properties.linetype_pattern
+                max(e * scale, min_dash_length) for e in properties.linetype_pattern
             ]
             if len(pattern) % 2:
                 pattern.pop()
             return pattern
 
+    def draw_text(
+        self,
+        text: str,
+        transform: Matrix44,
+        properties: Properties,
+        cap_height: float,
+        dxftype: str = "TEXT",
+    ) -> None:
+        if not text.strip():
+            return  # no point rendering empty strings
+        text = prepare_string_for_rendering(text, dxftype)
+        font_face = properties.font
+        if font_face is None:
+            font_face = self.default_font_face
+        try:
+            text_path = self.text_engine.get_text_path(text, font_face, cap_height)
+        except (RuntimeError, ValueError):
+            return
+        transformed_path = text_path.transform(transform)
+        polygons = fast_bbox_detection(single_paths([transformed_path]))  # type: ignore
+        external_paths, holes = winding_deconstruction(polygons)  # type: ignore
+        if properties.filling is None:
+            properties.filling = Filling()
+        self.draw_filled_paths(external_paths, holes, properties)  # type: ignore
+
 
 def filter_vp_entities(
     msp: Layout,
     limits: Sequence[float],
     bbox_cache: Optional[ezdxf.bbox.Cache] = None,
 ) -> Iterator[DXFGraphic]:
     """Yields all DXF entities that need to be processed by the given viewport
@@ -967,14 +971,15 @@
 
     Args:
         msp: modelspace layout
         limits: modelspace limits of the viewport, as tuple (min_x, min_y, max_x, max_y)
         bbox_cache: the bounding box cache of the modelspace entities
 
     """
+
     # WARNING: this works only with top-view viewports
     # The current state of the drawing add-on supports only top-view viewports!
     def is_visible(e):
         entity_bbox = bbox_cache.get(e)
         if entity_bbox is None:
             # compute and add bounding box
             entity_bbox = ezdxf.bbox.extents((e,), fast=True, cache=bbox_cache)
@@ -1012,21 +1017,31 @@
     *,
     filter_func: Optional[FilterFunc] = None,
 ) -> None:
     if filter_func is not None:
         entities = filter(filter_func, entities)
     for entity in entities:
         if not isinstance(entity, DXFGraphic):
-            if (
-                frontend.config.proxy_graphic_policy
-                != ProxyGraphicPolicy.IGNORE
-            ):
+            if frontend.config.proxy_graphic_policy != ProxyGraphicPolicy.IGNORE:
                 entity = DXFGraphicProxy(entity)
             else:
                 frontend.skip_entity(entity, "Cannot parse DXF entity")
                 continue
         properties = ctx.resolve_all(entity)
         frontend.override_properties(entity, properties)
         if properties.is_visible:
             frontend.draw_entity(entity, properties)
         else:
             frontend.skip_entity(entity, "invisible")
+
+
+def prepare_string_for_rendering(text: str, dxftype: str) -> str:
+    assert "\n" not in text, "not a single line of text"
+    if dxftype in {"TEXT", "ATTRIB", "ATTDEF"}:
+        text = replace_non_printable_characters(text, replacement="?")
+        text = text.replace("\t", "?")
+    elif dxftype == "MTEXT":
+        text = replace_non_printable_characters(text, replacement="▯")
+        text = text.replace("\t", "        ")
+    else:
+        raise TypeError(dxftype)
+    return text
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/gfxproxy.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/gfxproxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/mpl_text_renderer.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/strip.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,154 +1,182 @@
-# Copyright (c) 2020-2022, Matthew Broadway
+# Copyright (c) 2021-2022, Manfred Moitzi
 # License: MIT License
-from __future__ import annotations
-from typing import Iterator, Optional, Sequence
-from collections import defaultdict
-from functools import lru_cache
-
-from matplotlib.font_manager import FontProperties
-from matplotlib.textpath import TextPath
-
-import ezdxf.path
-from ezdxf.tools.fonts import FontMeasurements
-from ezdxf.tools import fonts
-from ezdxf.math import Vec2
-from ezdxf.math.triangulation import mapbox_earcut_2d
-from .text_renderer import TextRenderer
-
-
-@lru_cache(maxsize=256)  # fonts.Font is a named tuple
-def _get_font_properties(font: fonts.FontFace) -> Optional[FontProperties]:
-    # Font-definitions are created by the matplotlib FontManager(),
-    # but stored as json file and could be altered by an user:
-    font_properties = None
-    try:
-        font_properties = FontProperties(
-            family=font.family,
-            style=font.style,
-            stretch=font.stretch,
-            weight=font.weight,
-        )
-    except ValueError:
-        pass
-    return font_properties
-
-
-class MplTextRenderer(TextRenderer[FontProperties]):
-    def __init__(self, font=FontProperties(), use_cache: bool = True):
-        self._default_font = font
-        self._use_cache = use_cache
-
-        # Each font has its own text path cache
-        # key is hash(FontProperties)
-        self._text_path_cache: dict[int, dict[str, TextPath]] = defaultdict(
-            dict
-        )
-
-        # Each font has its own font measurements cache
-        # key is hash(FontProperties)
-        self._font_measurement_cache: dict[int, FontMeasurements] = {}
-
-    @property
-    def default_font(self) -> FontProperties:
-        return self._default_font
-
-    def clear_cache(self):
-        self._text_path_cache.clear()
-
-    def get_scale(
-        self, desired_cap_height: float, font: FontProperties
-    ) -> float:
-        return desired_cap_height / self.get_font_measurements(font).cap_height
-
-    def get_font_properties(
-        self, font: Optional[fonts.FontFace]
-    ) -> FontProperties:
-        if font is None:
-            return self.default_font
-        font_properties = _get_font_properties(font)
-        if font_properties is None:
-            return self.default_font
-        return font_properties
-
-    def get_font_measurements(self, font: FontProperties) -> FontMeasurements:
-        # None is the default font.
-        key = hash(font)
-        measurements = self._font_measurement_cache.get(key)
-        if measurements is None:
-            upper_x = self.get_text_path("X", font).vertices[:, 1].tolist()
-            lower_x = self.get_text_path("x", font).vertices[:, 1].tolist()
-            lower_p = self.get_text_path("p", font).vertices[:, 1].tolist()
-            baseline = min(lower_x)
-            measurements = FontMeasurements(
-                baseline=baseline,
-                cap_height=max(upper_x) - baseline,
-                x_height=max(lower_x) - baseline,
-                descender_height=baseline - min(lower_p),
+from typing import BinaryIO, Optional
+from ezdxf.lldxf.validator import is_dxf_file, DXFStructureError
+from pathlib import Path
+
+
+class TagWriter:
+    def __init__(self, fp: BinaryIO):
+        self.fp = fp
+
+    def write(self, raw_code_str: bytes, raw_value_str: bytes):
+        self.fp.write(raw_code_str)
+        self.fp.write(raw_value_str)
+
+
+class ThumbnailRemover(TagWriter):
+    def __init__(self, fp: BinaryIO):
+        super().__init__(fp)
+        self._start_section = False
+        self._skip_tags = False
+        self._section_code: Optional[bytes] = None
+        self._section_value: Optional[bytes] = None
+        self.removed_thumbnail_image = False
+
+    def write(self, raw_code_str: bytes, raw_value_str: bytes):
+        code = raw_code_str.strip()
+        value = raw_value_str.strip()
+        if self._start_section:
+            self._start_section = False
+            if code == b"2" and value == b"THUMBNAILIMAGE":
+                self._skip_tags = True
+                self.removed_thumbnail_image = True
+            else:
+                # write buffered section tag:
+                super().write(self._section_code, self._section_value)  # type: ignore
+
+        if code == b"0":
+            if value == b"SECTION":
+                self._start_section = True
+                self._skip_tags = False
+                # buffer section tag:
+                self._section_code = raw_code_str
+                self._section_value = raw_value_str
+                return
+            elif value == b"ENDSEC":
+                skip = self._skip_tags
+                self._skip_tags = False
+                if skip:  # don't write ENDSEC
+                    return
+
+        if not self._skip_tags:
+            super().write(raw_code_str, raw_value_str)
+
+
+def strip_comments(
+    infile: BinaryIO, tagwriter: TagWriter, verbose=False
+) -> int:
+    line_number: int = 1
+    removed_tags: int = 0
+    while True:
+        try:
+            raw_code_str = infile.readline()
+        except EOFError:
+            raw_code_str = b""
+        if raw_code_str == b"":  # regular end of file
+            return removed_tags
+        try:
+            code = int(raw_code_str)
+        except ValueError:
+            code_str = raw_code_str.strip().decode(
+                encoding="utf8", errors="ignore"
+            )
+            raise DXFStructureError(
+                f'CANCELED: "{infile.name}" - found invalid '
+                f'group code "{code_str}" at line {line_number}'
             )
-            self._font_measurement_cache[key] = measurements
-        return measurements
 
-    def get_text_path(self, text: str, font: FontProperties) -> TextPath:
-        # None is the default font
-        cache = self._text_path_cache[hash(font)]  # defaultdict(dict)
-        path = cache.get(text, None)
-        if path is None:
-            if font is None:
-                font = self._default_font
-            # must replace $ with \$ to avoid matplotlib interpreting it as math text
-            path = TextPath(
-                (0, 0),
-                text.replace("$", "\\$"),
-                size=1,
-                prop=font,
-                usetex=False,
+        try:
+            raw_value_str = infile.readline()
+        except EOFError:
+            raw_value_str = b""
+
+        if raw_value_str == b"":
+            raise DXFStructureError(
+                f'CANCELED: "{infile.name}" - premature end of file'
             )
-            if self._use_cache:
-                cache[text] = path
-        return path
-
-    def get_text_line_width(
-        self,
-        text: str,
-        cap_height: float,
-        font: Optional[fonts.FontFace] = None,
-    ) -> float:
-        font_properties = self.get_font_properties(font)
+        line_number += 2
+        if code != 999:
+            tagwriter.write(raw_code_str, raw_value_str)
+        else:
+            if verbose:
+                value = raw_value_str.strip()
+                _value = value.decode(encoding="utf8", errors="ignore")
+                print(f'removing comment: "{_value}"')
+            removed_tags += 1
+
+
+def safe_rename(source: Path, target: Path, backup=True, verbose=False) -> bool:
+    backup_file = target.with_suffix(".bak")
+    backup_file.unlink(missing_ok=True)  # type: ignore
+    _target = Path(target)
+    if _target.exists():
+        if verbose:
+            print(f'renaming "{_target.name}" to "{backup_file.name}"')
         try:
-            path = self.get_text_path(text, font_properties)
-            max_x = max(x for x, y in path.vertices)
-        except (RuntimeError, ValueError):
-            return 0.0
-        return max_x * self.get_scale(cap_height, font_properties)
-
-    def get_ezdxf_path(
-        self, text: str, font: FontProperties
-    ) -> ezdxf.path.Path:
+            _target.rename(backup_file)
+        except IOError as e:
+            print(f"IOError: {str(e)}")
+            return False
+
+    if verbose:
+        print(f'renaming "{source.name}" to "{target.name}"')
+    try:
+        source.rename(target)
+    except IOError as e:
+        print(f"IOError: {str(e)}")
+        return False
+
+    if not backup:
+        if verbose:
+            print(f'deleting backup file "{backup_file.name}"')
+        backup_file.unlink(missing_ok=True)  # type: ignore
+    return True
+
+
+def strip(filename: str, backup=False, thumbnail=False, verbose=False):
+    def remove_tmp_file():
+        if tmp_file.exists():
+            if verbose:
+                print(f'deleting temp file: "{tmp_file.name}"')
+            tmp_file.unlink(missing_ok=True)
+
+    if verbose:
+        print(f'\nProcessing file: "{filename}"')
+    try:
+        if not is_dxf_file(filename):
+            print(
+                f'CANCELED: "{filename}" is not a DXF file, binary DXF files '
+                f"are not supported"
+            )
+            return
+    except IOError as e:
+        print(f"IOError: {str(e)}")
+        return
+    source_file = Path(filename)
+    tmp_file = source_file.with_suffix(".ezdxf.tmp")
+    error = False
+    tagwriter: TagWriter
+    if verbose:
+        print(f'make a temporary copy: "{tmp_file.name}"')
+    with open(tmp_file, "wb") as fp, open(source_file, "rb") as infile:
+        if thumbnail:
+            tagwriter = ThumbnailRemover(fp)
+        else:
+            tagwriter = TagWriter(fp)
         try:
-            text_path = self.get_text_path(text, font)
-        except (RuntimeError, ValueError):
-            return ezdxf.path.Path()
-        return ezdxf.path.multi_path_from_matplotlib_path(text_path)
-
-    def get_tessellation(
-        self,
-        text: str,
-        font: FontProperties,
-        *,
-        max_flattening_distance: float = 0.01,
-    ) -> Iterator[Sequence[Vec2]]:
-        """Triangulate text into faces.
-
-        !!! Does not work for any arbitrary text !!!
-        """
-        for polygon in ezdxf.path.nesting.group_paths(
-            list(self.get_ezdxf_path(text, font).sub_paths())
-        ):
-            if len(polygon) == 0:
-                continue
-            exterior = polygon[0]
-            holes = polygon[1:]
-            yield from mapbox_earcut_2d(
-                exterior.flattening(max_flattening_distance),
-                [hole.flattening(max_flattening_distance) for hole in holes],
+            removed_tags = strip_comments(infile, tagwriter, verbose)
+        except IOError as e:
+            print(f"IOError: {str(e)}")
+            error = True
+        except DXFStructureError as e:
+            print(str(e))
+            error = True
+
+    if not error:
+        rename = False
+        if thumbnail and tagwriter.removed_thumbnail_image:  # type: ignore
+            print(f'"{source_file.name}" - removed THUMBNAILIMAGE section')
+            rename = True
+
+        if removed_tags > 0:
+            tags = "tag" if removed_tags == 1 else "tags"
+            print(
+                f'"{source_file.name}" - {removed_tags} comment {tags} removed'
             )
+            rename = True
+
+        if rename:
+            safe_rename(tmp_file, source_file, backup, verbose)
+
+    remove_tmp_file()
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/mtext_complex.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/mtext_complex.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing_extensions import Protocol
 import copy
 import math
 
 from ezdxf import colors
 from ezdxf.entities import MText
 from ezdxf.lldxf import const
-from ezdxf.math import Matrix44, Vec3
+from ezdxf.math import Matrix44, Vec3, AnyVec
 from ezdxf.render.abstract_mtext_renderer import AbstractMTextRenderer
 from ezdxf.tools import text_layout as tl, fonts
 from ezdxf.tools.text import MTextContext
 from .properties import Properties, RenderContext, rgb_to_hex
 from .type_hints import Color
 
 __all__ = ["complex_mtext_renderer"]
@@ -36,19 +36,19 @@
     if m is None:
         return Vec3.generate(corners)
     else:
         return m.transform_vertices(corners)
 
 
 class DrawInterface(Protocol):
-    def draw_line(self, start: Vec3, end: Vec3, properties: Properties) -> None:
+    def draw_line(self, start: AnyVec, end: AnyVec, properties: Properties) -> None:
         ...
 
     def draw_filled_polygon(
-        self, points: Iterable[Vec3], properties: Properties
+        self, points: Iterable[AnyVec], properties: Properties
     ) -> None:
         ...
 
     def draw_text(
         self,
         text: str,
         transform: Matrix44,
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/properties.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,17 +245,15 @@
         return LayoutProperties(
             "Model",
             MODEL_SPACE_BG_COLOR,
             units=units,
         )
 
     @staticmethod
-    def from_layout(
-        layout: Layout, units: Optional[int] = None
-    ) -> LayoutProperties:
+    def from_layout(layout: Layout, units: Optional[int] = None) -> LayoutProperties:
         """Setup default layout properties."""
         if layout.name == "Model":
             bg = MODEL_SPACE_BG_COLOR
         else:
             bg = PAPER_SPACE_BG_COLOR
         if units is None:
             units = layout.units
@@ -274,17 +272,15 @@
             bg = bg[:7]
         self._has_dark_background = is_dark_color(bg)
         if fg is not None:
             if not is_valid_color(fg):
                 raise ValueError(f"Invalid foreground color: {fg}")
             self._default_color = fg
         else:
-            self._default_color = (
-                "#ffffff" if self._has_dark_background else "#000000"
-            )
+            self._default_color = "#ffffff" if self._has_dark_background else "#000000"
 
 
 LayerPropsOverride = Callable[[Sequence[LayerProperties]], None]
 
 
 class RenderContext:
     """The render context for the given DXF document. The
@@ -339,29 +335,25 @@
             self.pdmode = doc.header.get("$PDMODE", 0)
             self._setup_text_styles(doc)
             try:
                 self.units = InsertUnits(doc.header.get("$INSUNITS", 0))
             except ValueError:
                 self.units = InsertUnits.Unitless
             try:
-                self.measurement = Measurement(
-                    doc.header.get("$MEASUREMENT", 0)
-                )
+                self.measurement = Measurement(doc.header.get("$MEASUREMENT", 0))
             except ValueError:
                 self.measurement = Measurement.Imperial
             if self.units == InsertUnits.Unitless:
                 if self.measurement == Measurement.Metric:
                     self.units = InsertUnits.Meters
                 else:
                     self.units = InsertUnits.Inches
         self.current_layout_properties.units = self.units  # default modelspace
 
-    def set_layer_properties_override(
-        self, func: Optional[LayerPropsOverride] = None
-    ):
+    def set_layer_properties_override(self, func: Optional[LayerPropsOverride] = None):
         """The function `func` is called with the current layer properties as
         argument after resetting them, so the function can override the layer
         properties.
         """
         self._layer_properties_override = func
 
     def _override_layer_properties(self, layers: Sequence[LayerProperties]):
@@ -478,31 +470,31 @@
             properties.has_aci_color_7 = layer.dxf.color == 7
 
         # Normalize linetype names to UPPERCASE:
         properties.linetype_name = str(layer.dxf.linetype).upper()
         properties.linetype_pattern = self.line_pattern.get(
             properties.linetype_name, CONTINUOUS_PATTERN
         )
-        properties.lineweight = self._true_layer_lineweight(
-            layer.dxf.lineweight
-        )
+        properties.lineweight = self._true_layer_lineweight(layer.dxf.lineweight)
         properties.is_visible = layer.is_on() and not layer.is_frozen()
         if self.export_mode:
             properties.is_visible &= bool(layer.dxf.plot)
         return properties
 
     def add_text_style(self, text_style: Textstyle):
         """Setup text style properties."""
         name = table_key(text_style.dxf.name)
         font_file = text_style.dxf.font
         font_face = None
         if font_file == "":  # Font family stored in XDATA?
             family, italic, bold = text_style.get_extended_font_data()
             if family:
-                font_face = fonts.find_font_face_by_family(family, italic, bold)
+                font_face = fonts.find_best_match(
+                    family=family, weight=700 if bold else 400, italic=italic
+                )
         else:
             font_face = fonts.get_font_face(font_file, map_shx=True)
 
         if font_face is None:  # fall back to default font
             font_face = fonts.FontFace()
         self.fonts[name] = font_face
 
@@ -564,21 +556,17 @@
         p.layer = self.resolve_layer(entity)
         resolved_layer = layer_key(p.layer)
         p.units = self.resolve_units()
         p.color = self.resolve_color(entity, resolved_layer=resolved_layer)
         p.linetype_name, p.linetype_pattern = self.resolve_linetype(
             entity, resolved_layer=resolved_layer
         )
-        p.lineweight = self.resolve_lineweight(
-            entity, resolved_layer=resolved_layer
-        )
+        p.lineweight = self.resolve_lineweight(entity, resolved_layer=resolved_layer)
         p.linetype_scale = self.resolve_linetype_scale(entity)
-        p.is_visible = self.resolve_visible(
-            entity, resolved_layer=resolved_layer
-        )
+        p.is_visible = self.resolve_visible(entity, resolved_layer=resolved_layer)
         if entity.is_supported_dxf_attrib("style"):
             p.font = self.resolve_font(entity)
         if isinstance(entity, DXFPolygon):
             p.filling = self.resolve_filling(entity)
         return p
 
     def resolve_units(self) -> InsertUnits:
@@ -632,17 +620,15 @@
             # An existing true color value always overrides ACI color!
             # Do not default to BYLAYER or BYBLOCK, this ACI value is ignored!
             aci = 7
         else:
             aci = entity.dxf.color  # defaults to BYLAYER
 
         entity_layer = resolved_layer or layer_key(self.resolve_layer(entity))
-        layer_properties = self.layers.get(
-            entity_layer, DEFAULT_LAYER_PROPERTIES
-        )
+        layer_properties = self.layers.get(entity_layer, DEFAULT_LAYER_PROPERTIES)
 
         if aci == const.BYLAYER:
             color = layer_properties.get_entity_color_from_layer(
                 self.current_layout_properties.default_color
             )
         elif aci == const.BYBLOCK:
             if not self.inside_block_reference:
@@ -679,17 +665,15 @@
         if alpha < 255:
             return f"{alpha:02x}"
         return ""
 
     def resolve_aci_color(self, aci: int, resolved_layer: str) -> Color:
         """Resolve the `aci` color as hex color string: "#RRGGBB" """
         if aci == const.BYLAYER:
-            layer = self.layers.get(
-                layer_key(resolved_layer), DEFAULT_LAYER_PROPERTIES
-            )
+            layer = self.layers.get(layer_key(resolved_layer), DEFAULT_LAYER_PROPERTIES)
             color = layer.get_entity_color_from_layer(
                 self.current_layout_properties.default_color
             )
         elif aci == const.BYBLOCK:
             if not self.inside_block_reference:
                 color = self.current_layout_properties.default_color
             else:
@@ -706,17 +690,15 @@
         `true_color` has higher priority than `aci`.
         """
         if true_color is not None:
             return rgb_to_hex(true_color)
         elif 0 < aci < 256:
             return self._aci_to_true_color(aci)
         else:
-            return (
-                self.current_layout_properties.default_color
-            )  # unknown / invalid
+            return self.current_layout_properties.default_color  # unknown / invalid
 
     def _aci_to_true_color(self, aci: int) -> Color:
         """Returns the `aci` value (AutoCAD Color Index) as rgb value in
         hex format: "#RRGGBB".
         """
         if aci == 7:  # black/white; todo: this bypasses the plot style table
             if self.current_layout_properties.has_dark_background:
@@ -739,17 +721,15 @@
             aci
         ].linetype != acadctb.OBJECT_LINETYPE:
             # todo: return special line types - overriding linetypes by
             #  plotstyle table
             pass
         name = entity.dxf.linetype.upper()  # default is 'BYLAYER'
         if name == "BYLAYER":
-            entity_layer = resolved_layer or layer_key(
-                self.resolve_layer(entity)
-            )
+            entity_layer = resolved_layer or layer_key(self.resolve_layer(entity))
             layer = self.layers.get(entity_layer, DEFAULT_LAYER_PROPERTIES)
             name = layer.linetype_name
             pattern = layer.linetype_pattern
 
         elif name == "BYBLOCK":
             if self.inside_block_reference:
                 name = self.current_block_reference_properties.linetype_name  # type: ignore
@@ -786,17 +766,15 @@
             if (0 < aci < 256) and self.plot_styles[
                 aci
             ].lineweight != acadctb.OBJECT_LINEWEIGHT:
                 # overriding lineweight by plotstyle table
                 return self.plot_styles.get_lineweight(aci)
             lineweight = entity.dxf.lineweight  # default is BYLAYER
             if lineweight == const.LINEWEIGHT_BYLAYER:
-                entity_layer = resolved_layer or layer_key(
-                    self.resolve_layer(entity)
-                )
+                entity_layer = resolved_layer or layer_key(self.resolve_layer(entity))
                 return self.layers.get(
                     entity_layer, DEFAULT_LAYER_PROPERTIES
                 ).lineweight
 
             elif lineweight == const.LINEWEIGHT_BYBLOCK:
                 if self.inside_block_reference:
                     return self.current_block_reference_properties.lineweight
@@ -899,17 +877,15 @@
     if type(color) is not Color:
         raise TypeError(f"Invalid argument type: {type(color)}.")
     if len(color) in (7, 9):
         return bool(COLOR_PATTERN.fullmatch(color))
     return False
 
 
-def rgb_to_hex(
-    rgb: Union[tuple[int, int, int], tuple[float, float, float]]
-) -> Color:
+def rgb_to_hex(rgb: Union[tuple[int, int, int], tuple[float, float, float]]) -> Color:
     """Returns color in hex format: "#RRGGBB"."""
     assert all(0 <= x <= 255 for x in rgb), f"invalid RGB color: {rgb}"
     r, g, b = rgb
     return f"#{r:02x}{g:02x}{b:02x}"
 
 
 def hex_to_rgb(hex_string: Color) -> RGB:
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/pyqt.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/tags.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,369 +1,458 @@
-# Copyright (c) 2020-2022, Matthew Broadway
+# Copyright (c) 2011-2022, Manfred Moitzi
 # License: MIT License
-# mypy: ignore_errors=True
+"""
+Tags
+----
+
+A list of :class:`~ezdxf.lldxf.types.DXFTag`, inherits from Python standard list.
+Unlike the statement in the DXF Reference "Do not write programs that rely on
+the order given here", tag order is sometimes essential and some group codes
+may appear multiples times in one entity. At the worst case
+(:class:`~ezdxf.entities.material.Material`: normal map shares group codes with
+diffuse map) using same group codes with different meanings.
+
+"""
 from __future__ import annotations
-from typing import Optional, Iterable, Tuple
-from typing_extensions import TypeAlias
-import math
-
-from ezdxf.addons.xqt import QtCore as qc, QtGui as qg, QtWidgets as qw
-from ezdxf.addons.drawing.backend import Backend, prepare_string_for_rendering
-from ezdxf.addons.drawing.config import Configuration
-from ezdxf.tools.fonts import FontMeasurements
-from ezdxf.addons.drawing.type_hints import Color
-from ezdxf.addons.drawing.properties import Properties
-from ezdxf.addons.drawing.qt_text_renderer import QtTextRenderer
-from ezdxf.tools import fonts
-from ezdxf.math import Vec3, Matrix44
-from ezdxf.path import Path, to_qpainter_path
-
-PatternKey: TypeAlias = Tuple[str, float]
-
-
-class _Point(qw.QAbstractGraphicsShapeItem):
-    """A dimensionless point which is drawn 'cosmetically' (scale depends on
-    view)
+from typing import Iterable, Iterator, Any, Optional
+
+from .const import DXFStructureError, DXFValueError, STRUCTURE_MARKER
+from .types import DXFTag, EMBEDDED_OBJ_MARKER, EMBEDDED_OBJ_STR, dxftag
+from .tagger import internal_tag_compiler
+from . import types
+
+COMMENT_CODE = 999
+
+
+class Tags(list):
+    """Collection of :class:`~ezdxf.lldxf.types.DXFTag` as flat list.
+    Low level tag container, only required for advanced stuff.
+
     """
 
-    def __init__(self, x: float, y: float, brush: qg.QBrush):
-        super().__init__()
-        self.location = qc.QPointF(x, y)
-        self.radius = 1.0
-        self.setPen(qg.QPen(qc.Qt.NoPen))
-        self.setBrush(brush)
-
-    def paint(
-        self,
-        painter: qg.QPainter,
-        option: qw.QStyleOptionGraphicsItem,
-        widget: Optional[qw.QWidget] = None,
-    ) -> None:
-        view_scale = _get_x_scale(painter.transform())
-        radius = self.radius / view_scale
-        painter.setBrush(self.brush())
-        painter.setPen(qc.Qt.NoPen)
-        painter.drawEllipse(self.location, radius, radius)
-
-    def boundingRect(self) -> qc.QRectF:
-        return qc.QRectF(self.location, qc.QSizeF(1, 1))
-
-
-class ViewportGroup(qw.QGraphicsItemGroup):
-    def __init__(self, clipping_path: Path):
-        super().__init__()
-        self.setFlag(
-            qw.QGraphicsItemGroup.GraphicsItemFlag.ItemClipsChildrenToShape,
-            True,
-        )
-        self._clipping_path = to_qpainter_path([clipping_path])
+    @classmethod
+    def from_text(cls, text: str) -> Tags:
+        """Constructor from DXF string."""
+        return cls(internal_tag_compiler(text))
 
-    def shape(self):
-        return self._clipping_path
+    @classmethod
+    def from_tuples(cls, tags: Iterable[tuple[int, Any]]) -> Tags:
+        return cls(DXFTag(code, value) for code, value in tags)
 
+    def __copy__(self) -> Tags:
+        return self.__class__(tag.clone() for tag in self)
 
-# The key used to store the dxf entity corresponding to each graphics element
-CorrespondingDXFEntity = qc.Qt.UserRole + 0  # type: ignore
-CorrespondingDXFParentStack = qc.Qt.UserRole + 1  # type: ignore
+    clone = __copy__
 
+    def get_handle(self) -> str:
+        """Get DXF handle. Raises :class:`DXFValueError` if handle not exist.
 
-class PyQtBackend(Backend):
-    """
-    Backend which uses the :mod:`PySide6` package to implement an interactive
-    viewer. The :mod:`PyQt5` package can be used as fallback if the :mod:`PySide6`
-    package is not available.
+        Returns:
+            handle as plain hex string like ``'FF00'``
 
-    Args:
-        scene: drawing canvas of type :class:`QtWidgets.QGraphicsScene`,
-            if ``None`` a new canvas will be created
-        extra_lineweight_scaling: compared to other backends,
-            PyQt draws lines which appear thinner
-        use_text_cache: use caching for text path rendering
+        Raises:
+            DXFValueError: no handle found
 
-    """
+        """
+        try:
+            code, handle = self[1]  # fast path  for most common cases
+        except IndexError:
+            raise DXFValueError("No handle found.")
+
+        if code == 5 or code == 105:
+            return handle
+
+        for code, handle in self:
+            if code == 5 or code == 105:
+                return handle
+        raise DXFValueError("No handle found.")
+
+    def replace_handle(self, new_handle: str) -> None:
+        """Replace existing handle.
 
-    def __init__(
-        self,
-        scene: Optional[qw.QGraphicsScene] = None,
-        *,
-        use_text_cache: bool = True,
-        debug_draw_rect: bool = False,
-        extra_lineweight_scaling: float = 2.0,
-    ):
-        super().__init__()
-        self._scene = scene or qw.QGraphicsScene()  # avoids many type errors
-        self._color_cache: dict[Color, qg.QColor] = {}
-        self._pattern_cache: dict[PatternKey, int] = {}
-        self._no_line = qg.QPen(qc.Qt.NoPen)
-        self._no_fill = qg.QBrush(qc.Qt.NoBrush)
-
-        self._text_renderer = QtTextRenderer(use_cache=use_text_cache)
-        self._extra_lineweight_scaling = extra_lineweight_scaling
-        self._debug_draw_rect = debug_draw_rect
-        self._current_viewport: Optional[ViewportGroup] = None
-
-    def configure(self, config: Configuration) -> None:
-        if config.min_lineweight is None:
-            config = config.with_changes(min_lineweight=0.24)
-        super().configure(config)
-
-    def set_scene(self, scene: qw.QGraphicsScene):
-        self._scene = scene
-
-    def clear_text_cache(self):
-        self._text_renderer.clear_cache()
-
-    def set_clipping_path(
-        self, path: Optional[Path] = None, scale: float = 1.0
-    ) -> bool:
-        if path:
-            self._current_viewport = ViewportGroup(path)
-            self._scene.addItem(self._current_viewport)
+        Args:
+            new_handle: new handle as plain hex string e.g. ``'FF00'``
+
+        """
+        for index, tag in enumerate(self):
+            if tag.code in (5, 105):
+                self[index] = DXFTag(tag.code, new_handle)
+                return
+
+    def dxftype(self) -> str:
+        """Returns DXF type of entity, e.g. ``'LINE'``."""
+        return self[0].value
+
+    def has_tag(self, code: int) -> bool:
+        """Returns ``True`` if a :class:`~ezdxf.lldxf.types.DXFTag` with given
+        group `code` is present.
+
+        Args:
+            code: group code as int
+
+        """
+        return any(tag.code == code for tag in self)
+
+    def get_first_value(self, code: int, default=DXFValueError) -> Any:
+        """Returns value of first :class:`~ezdxf.lldxf.types.DXFTag` with given
+        group code or default if `default` != :class:`DXFValueError`, else
+        raises :class:`DXFValueError`.
+
+        Args:
+            code: group code as int
+            default: return value for default case or raises :class:`DXFValueError`
+
+        """
+        for tag in self:
+            if tag.code == code:
+                return tag.value
+        if default is DXFValueError:
+            raise DXFValueError(code)
         else:
-            self._current_viewport = None
-        return True  # confirm clipping support
+            return default
+
+    def get_first_tag(self, code: int, default=DXFValueError) -> DXFTag:
+        """Returns first :class:`~ezdxf.lldxf.types.DXFTag` with given group
+        code or `default`, if `default` != :class:`DXFValueError`, else raises
+        :class:`DXFValueError`.
+
+        Args:
+            code: group code as int
+            default: return value for default case or raises :class:`DXFValueError`
 
-    def _add_item(self, item):
-        self._set_item_data(item)
-        if self._current_viewport:
-            self._current_viewport.addToGroup(item)
+        """
+        for tag in self:
+            if tag.code == code:
+                return tag
+        if default is DXFValueError:
+            raise DXFValueError(code)
         else:
-            self._scene.addItem(item)
+            return default  # type: ignore
+
+    def find_all(self, code: int) -> Tags:
+        """Returns a list of :class:`~ezdxf.lldxf.types.DXFTag` with given
+        group code.
 
-    def _get_color(self, color: Color) -> qg.QColor:
-        qt_color = self._color_cache.get(color, None)
-        if qt_color is None:
-            if len(color) == 7:
-                qt_color = qg.QColor(color)  # '#RRGGBB'
-            elif len(color) == 9:
-                rgb = color[1:7]
-                alpha = color[7:9]
-                qt_color = qg.QColor(f"#{alpha}{rgb}")  # '#AARRGGBB'
+        Args:
+            code: group code as int
+
+        """
+        return self.__class__(tag for tag in self if tag.code == code)
+
+    def tag_index(self, code: int, start: int = 0, end: Optional[int] = None) -> int:
+        """Return index of first :class:`~ezdxf.lldxf.types.DXFTag` with given
+        group code.
+
+        Args:
+            code: group code as int
+            start: start index as int
+            end: end index as int, ``None`` for end index = ``len(self)``
+
+        """
+        if end is None:
+            end = len(self)
+        index = start
+        while index < end:
+            if self[index].code == code:
+                return index
+            index += 1
+        raise DXFValueError(code)
+
+    def update(self, tag: DXFTag) -> None:
+        """Update first existing tag with same group code as `tag`, raises
+        :class:`DXFValueError` if tag not exist.
+
+        """
+        index = self.tag_index(tag.code)
+        self[index] = tag
+
+    def set_first(self, tag: DXFTag) -> None:
+        """Update first existing tag with group code ``tag.code`` or append tag."""
+        try:
+            self.update(tag)
+        except DXFValueError:
+            self.append(tag)
+
+    def remove_tags(self, codes: Iterable[int]) -> None:
+        """Remove all tags inplace with group codes specified in `codes`.
+
+        Args:
+            codes: iterable of group codes as int
+
+        """
+        self[:] = [tag for tag in self if tag.code not in set(codes)]
+
+    def pop_tags(self, codes: Iterable[int]) -> Iterator[DXFTag]:
+        """Pop tags with group codes specified in `codes`.
+
+        Args:
+            codes: iterable of group codes
+
+        """
+        remaining = []
+        codes = set(codes)
+        for tag in self:
+            if tag.code in codes:
+                yield tag
             else:
-                raise TypeError(color)
+                remaining.append(tag)
+        self[:] = remaining
 
-            self._color_cache[color] = qt_color
-        return qt_color
+    def remove_tags_except(self, codes: Iterable[int]) -> None:
+        """Remove all tags inplace except those with group codes specified in
+        `codes`.
 
-    def _get_pen(self, properties: Properties) -> qg.QPen:
-        """Returns a cosmetic pen with applied lineweight but without line type
-        support.
-        """
-        px = (
-            properties.lineweight
-            / 0.3527
-            * self.config.lineweight_scaling
-            * self._extra_lineweight_scaling
-        )
-        pen = qg.QPen(self._get_color(properties.color), px)
-        # Use constant width in pixel:
-        pen.setCosmetic(True)
-        pen.setJoinStyle(qc.Qt.RoundJoin)
-        return pen
-
-    def _get_brush(self, properties: Properties) -> qg.QBrush:
-        # Hatch patterns are handled by the frontend since v0.18.1
-        filling = properties.filling
-        if filling:
-            return qg.QBrush(self._get_color(properties.color), qc.Qt.SolidPattern)  # type: ignore
-        return self._no_fill
-
-    def _set_item_data(self, item: qw.QGraphicsItem) -> None:
-        parent_stack = tuple(e for e, props in self.entity_stack[:-1])
-        current_entity = self.current_entity
-        if isinstance(item, list):
-            for item_ in item:
-                item_.setData(CorrespondingDXFEntity, current_entity)
-                item_.setData(CorrespondingDXFParentStack, parent_stack)
-        else:
-            item.setData(CorrespondingDXFEntity, current_entity)
-            item.setData(CorrespondingDXFParentStack, parent_stack)
+        Args:
+            codes: iterable of group codes
 
-    def set_background(self, color: Color):
-        self._scene.setBackgroundBrush(qg.QBrush(self._get_color(color)))
+        """
+        self[:] = [tag for tag in self if tag.code in set(codes)]
 
-    def draw_point(self, pos: Vec3, properties: Properties) -> None:
-        """Draw a real dimensionless point."""
-        brush = qg.QBrush(self._get_color(properties.color), qc.Qt.SolidPattern)
-        item = _Point(pos.x, pos.y, brush)
-        self._set_item_data(item)
-        self._add_item(item)
-
-    def draw_line(self, start: Vec3, end: Vec3, properties: Properties) -> None:
-        # PyQt draws a long line for a zero-length line:
-        if start.isclose(end):
-            self.draw_point(start, properties)
-        else:
-            item = qw.QGraphicsLineItem(start.x, start.y, end.x, end.y)
-            item.setPen(self._get_pen(properties))
-            self._add_item(item)
-
-    def draw_solid_lines(
-        self,
-        lines: Iterable[tuple[Vec3, Vec3]],
-        properties: Properties,
-    ):
-        """Fast method to draw a bunch of solid lines with the same properties."""
-        pen = self._get_pen(properties)
-        add_line = self._add_item
-        for s, e in lines:
-            if s.isclose(e):
-                self.draw_point(s, properties)
+    def filter(self, codes: Iterable[int]) -> Iterator[DXFTag]:
+        """Iterate and filter tags by group `codes`.
+
+        Args:
+            codes: group codes to filter
+
+        """
+        return (tag for tag in self if tag.code not in set(codes))
+
+    def collect_consecutive_tags(
+        self, codes: Iterable[int], start: int = 0, end: Optional[int] = None
+    ) -> Tags:
+        """Collect all consecutive tags with group code in `codes`, `start` and
+        `end` delimits the search range. A tag code not in codes ends the
+        process.
+
+        Args:
+            codes: iterable of group codes
+            start: start index as int
+            end: end index as int, ``None`` for end index = ``len(self)``
+
+        Returns:
+            collected tags as :class:`Tags`
+
+        """
+        codes = frozenset(codes)
+        index = int(start)
+        if end is None:
+            end = len(self)
+        bag = self.__class__()
+
+        while index < end:
+            tag = self[index]
+            if tag.code in codes:
+                bag.append(tag)
+                index += 1
             else:
-                item = qw.QGraphicsLineItem(s.x, s.y, e.x, e.y)
-                item.setPen(pen)
-                add_line(item)
-
-    def draw_path(self, path: Path, properties: Properties) -> None:
-        item = qw.QGraphicsPathItem(to_qpainter_path([path]))
-        item.setPen(self._get_pen(properties))
-        item.setBrush(self._no_fill)
-        self._add_item(item)
-
-    def draw_filled_paths(
-        self,
-        paths: Iterable[Path],
-        holes: Iterable[Path],
-        properties: Properties,
-    ) -> None:
-        oriented_paths: list[Path] = []
-        for path in paths:
-            try:
-                path = path.counter_clockwise()
-            except ValueError:  # cannot detect path orientation
-                continue
-            oriented_paths.append(path)
-        for path in holes:
-            try:
-                path = path.clockwise()
-            except ValueError:  # cannot detect path orientation
-                continue
-            oriented_paths.append(path)
-        item = _CosmeticPath(to_qpainter_path(oriented_paths))
-        item.setPen(self._get_pen(properties))
-        item.setBrush(self._get_brush(properties))
-        self._add_item(item)
-
-    def draw_filled_polygon(
-        self, points: Iterable[Vec3], properties: Properties
-    ) -> None:
-        brush = self._get_brush(properties)
-        polygon = qg.QPolygonF()
-        for p in points:
-            polygon.append(qc.QPointF(p.x, p.y))
-        item = _CosmeticPolygon(polygon)
-        item.setPen(self._no_line)
-        item.setBrush(brush)
-        self._add_item(item)
-
-    def draw_text(
-        self,
-        text: str,
-        transform: Matrix44,
-        properties: Properties,
-        cap_height: float,
-    ) -> None:
-        if not text.strip():
-            return  # no point rendering empty strings
-        text = prepare_string_for_rendering(text, self.current_entity.dxftype())  # type: ignore
-        qfont = self.get_qfont(properties.font)
-        scale = self._text_renderer.get_scale(cap_height, qfont)
-        transform = Matrix44.scale(scale, -scale, 0) @ transform
-
-        path = self._text_renderer.get_text_path(text, qfont)
-        path = _matrix_to_qtransform(transform).map(path)
-        item = qw.QGraphicsPathItem(path)
-        brush = qg.QBrush(self._get_color(properties.color), qc.Qt.SolidPattern)
-        item.setBrush(brush)
-        item.setPen(self._no_line)
-        self._add_item(item)
-
-    def get_qfont(self, font: Optional[fonts.FontFace]) -> qg.QFont:
-        return self._text_renderer.get_font_properties(font)
-
-    def get_font_measurements(
-        self, cap_height: float, font: Optional[fonts.FontFace] = None
-    ) -> FontMeasurements:
-        qfont = self.get_qfont(font)
-        return self._text_renderer.get_font_measurements(
-            qfont
-        ).scale_from_baseline(desired_cap_height=cap_height)
-
-    def get_text_line_width(
-        self,
-        text: str,
-        cap_height: float,
-        font: Optional[fonts.FontFace] = None,
-    ) -> float:
-        if not text.strip():
-            return 0
+                break
+        return bag
 
-        dxftype = (
-            self.current_entity.dxftype() if self.current_entity else "TEXT"
-        )
-        text = prepare_string_for_rendering(text, dxftype)
-        return self._text_renderer.get_text_line_width(text, cap_height, font)
+    def has_embedded_objects(self) -> bool:
+        for tag in self:
+            if tag.code == EMBEDDED_OBJ_MARKER and tag.value == EMBEDDED_OBJ_STR:
+                return True
+        return False
+
+    @classmethod
+    def strip(cls, tags: Tags, codes: Iterable[int]) -> Tags:
+        """Constructor from `tags`, strips all tags with group codes in `codes`
+        from tags.
+
+        Args:
+            tags: iterable of :class:`~ezdxf.lldxf.types.DXFTag`
+            codes: iterable of group codes as int
 
-    def clear(self) -> None:
-        self._scene.clear()
+        """
+        return cls((tag for tag in tags if tag.code not in frozenset(codes)))
 
-    def finalize(self) -> None:
-        super().finalize()
-        self._scene.setSceneRect(self._scene.itemsBoundingRect())
-        if self._debug_draw_rect:
-            properties = Properties()
-            properties.color = "#000000"
-            self._scene.addRect(
-                self._scene.sceneRect(),
-                self._get_pen(properties),
-                self._no_fill,
-            )
+    def get_soft_pointers(self) -> Tags:
+        """Returns all soft-pointer handles in group code range 330-339."""
+        return Tags(tag for tag in self if types.is_soft_pointer(tag))
+
+    def get_hard_pointers(self) -> Tags:
+        """Returns all hard-pointer handles in group code range 340-349, 390-399 and
+        480-481. Hard pointers protect an object from being purged.
+        """
+        return Tags(tag for tag in self if types.is_hard_pointer(tag))
 
+    def get_soft_owner_handles(self) -> Tags:
+        """Returns all soft-owner handles in group code range 350-359."""
+        return Tags(tag for tag in self if types.is_soft_owner(tag))
+
+    def get_hard_owner_handles(self) -> Tags:
+        """Returns all hard-owner handles in group code range 360-369."""
+        return Tags(tag for tag in self if types.is_hard_owner(tag))
+
+    def has_translatable_pointers(self) -> bool:
+        """Returns ``True`` if any pointer handle has to be translated during INSERT
+        and XREF operations.
+        """
+        return any(types.is_translatable_pointer(tag) for tag in self)
 
-class _CosmeticPath(qw.QGraphicsPathItem):
-    def paint(
-        self,
-        painter: qg.QPainter,
-        option: qw.QStyleOptionGraphicsItem,
-        widget: Optional[qw.QWidget] = None,
-    ) -> None:
-        _set_cosmetic_brush(self, painter)
-        super().paint(painter, option, widget)
-
-
-class _CosmeticPolygon(qw.QGraphicsPolygonItem):
-    def paint(
-        self,
-        painter: qg.QPainter,
-        option: qw.QStyleOptionGraphicsItem,
-        widget: Optional[qw.QWidget] = None,
-    ) -> None:
-        _set_cosmetic_brush(self, painter)
-        super().paint(painter, option, widget)
-
-
-def _set_cosmetic_brush(
-    item: qw.QAbstractGraphicsShapeItem, painter: qg.QPainter
-) -> None:
-    """like a cosmetic pen, this sets the brush pattern to appear the same independent of the view"""
-    brush = item.brush()
-    # scale by -1 in y because the view is always mirrored in y and undoing the view transformation entirely would make
-    # the hatch mirrored w.r.t the view
-    brush.setTransform(painter.transform().inverted()[0].scale(1, -1))  # type: ignore
-    item.setBrush(brush)
-
-
-def _get_x_scale(t: qg.QTransform) -> float:
-    return math.sqrt(t.m11() * t.m11() + t.m21() * t.m21())
-
-
-def _matrix_to_qtransform(matrix: Matrix44) -> qg.QTransform:
-    """Qt also uses row-vectors so the translation elements are placed in the
-    bottom row.
+    def get_translatable_pointers(self) -> Tags:
+        """Returns all pointer handles which should be translated during INSERT and XREF
+        operations.
+        """
+        return Tags(tag for tag in self if types.is_translatable_pointer(tag))
 
-    This is only a simple conversion which assumes that although the
-    transformation is 4x4,it does not involve the z axis.
 
-    A more correct transformation could be implemented like so:
-    https://stackoverflow.com/questions/10629737/convert-3d-4x4-rotation-matrix-into-2d
+def text2tags(text: str) -> Tags:
+    return Tags.from_text(text)
+
+
+def group_tags(
+    tags: Iterable[DXFTag], splitcode: int = STRUCTURE_MARKER
+) -> Iterable[Tags]:
+    """Group of tags starts with a SplitTag and ends before the next SplitTag.
+    A SplitTag is a tag with code == splitcode, like (0, 'SECTION') for
+    splitcode == 0.
+
+    Args:
+        tags: iterable of :class:`DXFTag`
+        splitcode: group code of split tag
+
     """
-    return qg.QTransform(*matrix.get_2d_transformation())
+
+    # first do nothing, skip tags in front of the first split tag
+    def append(tag):
+        pass
+
+    group = None
+    for tag in tags:
+        if tag.code == splitcode:
+            if group is not None:
+                yield group
+            group = Tags([tag])
+            append = group.append  # redefine append: add tags to this group
+        else:
+            append(tag)
+    if group is not None:
+        yield group
+
+
+def text_to_multi_tags(
+    text: str, code: int = 303, size: int = 255, line_ending: str = "^J"
+) -> Tags:
+    text = "".join(text).replace("\n", line_ending)
+
+    def chop():
+        start = 0
+        end = size
+        while start < len(text):
+            yield text[start:end]
+            start = end
+            end += size
+
+    return Tags(DXFTag(code, part) for part in chop())
+
+
+def multi_tags_to_text(tags: Tags, line_ending: str = "^J") -> str:
+    return "".join(tag.value for tag in tags).replace(line_ending, "\n")
+
+
+OPEN_LIST = (1002, "{")
+CLOSE_LIST = (1002, "}")
+
+
+def xdata_list(name: str, xdata_tags: Iterable) -> Tags:
+    tags = Tags()
+    if name:
+        tags.append((1000, name))
+    tags.append(OPEN_LIST)
+    tags.extend(xdata_tags)
+    tags.append(CLOSE_LIST)
+    return tags
+
+
+def remove_named_list_from_xdata(name: str, tags: Tags) -> Tags:
+    start, end = get_start_and_end_of_named_list_in_xdata(name, tags)
+    del tags[start:end]
+    return tags
+
+
+def get_named_list_from_xdata(name: str, tags: Tags) -> Tags:
+    start, end = get_start_and_end_of_named_list_in_xdata(name, tags)
+    return Tags(tags[start:end])
+
+
+class NotFoundException(Exception):
+    pass
+
+
+def get_start_and_end_of_named_list_in_xdata(name: str, tags: Tags) -> tuple[int, int]:
+    start = None
+    end = None
+    level = 0
+    for index in range(len(tags)):
+        tag = tags[index]
+
+        if start is None and tag == (1000, name):
+            next_tag = tags[index + 1]
+            if next_tag == OPEN_LIST:
+                start = index
+                continue
+        if start is not None:
+            if tag == OPEN_LIST:
+                level += 1
+            elif tag == CLOSE_LIST:
+                level -= 1
+            if level == 0:
+                end = index
+                break
+
+    if start is None:
+        raise NotFoundException
+    if end is None:
+        raise DXFStructureError('Invalid XDATA structure: missing  (1002, "}").')
+    return start, end + 1
+
+
+def find_begin_and_end_of_encoded_xdata_tags(name: str, tags: Tags) -> tuple[int, int]:
+    """Find encoded XDATA tags, surrounded by group code 1000 tags
+    name_BEGIN and name_END (e.g. MTEXT column specification).
+
+    Raises:
+        NotFoundError: tag group not found
+        DXFStructureError: missing begin- or end tag
+
+    """
+    begin_name = name + "_BEGIN"
+    end_name = name + "_END"
+    start = None
+    end = None
+    for index, (code, value) in enumerate(tags):
+        if code == 1000:
+            if value == begin_name:
+                start = index
+            elif value == end_name:
+                end = index + 1
+                break
+    if start is None:
+        if end is not None:  # end tag without begin tag!
+            raise DXFStructureError(
+                f"Invalid XDATA structure: missing begin tag (1000, {begin_name})."
+            )
+        raise NotFoundException
+    if end is None:
+        raise DXFStructureError(
+            f"Invalid XDATA structure: missing end tag (1000, {end_name})."
+        )
+    return start, end
+
+
+def binary_data_to_dxf_tags(
+    data: bytes,
+    length_group_code: int = 160,
+    value_group_code: int = 310,
+    value_size=127,
+) -> Tags:
+    """Convert binary data to DXF tags."""
+    tags = Tags()
+    length = len(data)
+    tags.append(dxftag(length_group_code, length))
+    index = 0
+    while index < length:
+        chunk = data[index : index + value_size]
+        tags.append(dxftag(value_group_code, chunk))
+        index += value_size
+    return tags
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/qtviewer.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/qtviewer.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 
         self.setWindowTitle("CAD Viewer")
         self.resize(1600, 900)
         self.show()
 
     def _reset_backend(self):
         # clear caches
-        self._backend = PyQtBackend(use_text_cache=True)
+        self._backend = PyQtBackend()
 
     def _select_doc(self):
         path, _ = qw.QFileDialog.getOpenFileName(
             self,
             caption="Select CAD Document",
             filter="CAD Documents (*.dxf *.DXF *.dwg *.DWG)",
         )
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/text.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,20 @@
 
 import ezdxf.lldxf.const as DXFConstants
 from ezdxf.enums import (
     TextEntityAlignment,
     MAP_TEXT_ENUM_TO_ALIGN_FLAGS,
     MTextEntityAlignment,
 )
-from ezdxf.addons.drawing.backend import BackendInterface
-from ezdxf.addons.drawing.debug_utils import draw_rect
 from ezdxf.entities import MText, Text, Attrib, AttDef
 from ezdxf.math import Matrix44, Vec3, sign
 from ezdxf.tools import fonts
 from ezdxf.tools.fonts import FontMeasurements
 from ezdxf.tools.text import plain_text, text_wrap
+from .text_renderer import TextRenderer
 
 """
 Search google for 'typography' or 'font anatomy' for explanations of terms like 
 'baseline' and 'x-height'
 
 A Visual Guide to the Anatomy of Typography: https://visme.co/blog/type-anatomy/
 Anatomy of a Character: https://www.fonts.com/content/learning/fontology/level-1/type-anatomy/anatomy
@@ -38,17 +37,15 @@
 
 @enum.unique
 class VAlignment(enum.Enum):
     TOP = 0  # the top of capital letters or letters with ascenders (like 'b')
     LOWER_CASE_CENTER = 1  # the midpoint between the baseline and the x-height
     BASELINE = 2  # the line which text rests on, characters with descenders (like 'p') are partially below this line
     BOTTOM = 3  # the lowest point on a character with a descender (like 'p')
-    UPPER_CASE_CENTER = (
-        4  # the midpoint between the baseline and the cap-height
-    )
+    UPPER_CASE_CENTER = 4  # the midpoint between the baseline and the cap-height
 
 
 Alignment: TypeAlias = Tuple[HAlignment, VAlignment]
 AnyText: TypeAlias = Union[Text, MText, Attrib, AttDef]
 
 # multiple of cap_height between the baseline of the previous line and the
 # baseline of the next line
@@ -79,18 +76,15 @@
         HAlignment.RIGHT,
         VAlignment.UPPER_CASE_CENTER,
     ),
     TextEntityAlignment.TOP_LEFT: (HAlignment.LEFT, VAlignment.TOP),
     TextEntityAlignment.TOP_CENTER: (HAlignment.CENTER, VAlignment.TOP),
     TextEntityAlignment.TOP_RIGHT: (HAlignment.RIGHT, VAlignment.TOP),
 }
-assert (
-    DXF_TEXT_ALIGNMENT_TO_ALIGNMENT.keys()
-    == MAP_TEXT_ENUM_TO_ALIGN_FLAGS.keys()
-)
+assert DXF_TEXT_ALIGNMENT_TO_ALIGNMENT.keys() == MAP_TEXT_ENUM_TO_ALIGN_FLAGS.keys()
 
 DXF_MTEXT_ALIGNMENT_TO_ALIGNMENT: dict[int, Alignment] = {
     DXFConstants.MTEXT_TOP_LEFT: (HAlignment.LEFT, VAlignment.TOP),
     DXFConstants.MTEXT_TOP_CENTER: (HAlignment.CENTER, VAlignment.TOP),
     DXFConstants.MTEXT_TOP_RIGHT: (HAlignment.RIGHT, VAlignment.TOP),
     DXFConstants.MTEXT_MIDDLE_LEFT: (
         HAlignment.LEFT,
@@ -240,16 +234,15 @@
     font_measurements: FontMeasurements,
 ) -> tuple[tuple[float, float], list[float], list[float]]:
     if not line_widths:
         return (0, 0), [], []
 
     halign, valign = alignment
     line_ys = [
-        -font_measurements.baseline
-        - (font_measurements.cap_height + i * line_spacing)
+        -font_measurements.baseline - (font_measurements.cap_height + i * line_spacing)
         for i in range(len(line_widths))
     ]
 
     if box_width is None:
         box_width = max(line_widths)
 
     last_baseline = line_ys[-1]
@@ -305,39 +298,38 @@
     else:
         return text.dxf.insert
 
 
 # Simple but fast MTEXT renderer:
 def simplified_text_chunks(
     text: AnyText,
-    out: BackendInterface,
+    render_engine: TextRenderer,
     *,
-    font: Optional[fonts.FontFace] = None,
-    debug_draw_rect: bool = False
+    font_face: fonts.FontFace,
 ) -> Iterable[tuple[str, Matrix44, float]]:
     """Splits a complex text entity into simple chunks of text which can all be
     rendered the same way:
     render the string (which will not contain any newlines) with the given
     cap_height with (left, baseline) at (0, 0) then transform it with the given
     matrix to move it into place.
     """
     alignment = _get_alignment(text)
     box_width = _get_text_width(text)
 
     cap_height = _get_cap_height(text)
     lines = _split_into_lines(
         text,
         box_width,
-        lambda s: out.get_text_line_width(s, cap_height, font=font),
+        lambda s: render_engine.get_text_line_width(s, font_face, cap_height),
     )
     line_spacing = _get_line_spacing(text, cap_height)
     line_widths = [
-        out.get_text_line_width(line, cap_height, font=font) for line in lines
+        render_engine.get_text_line_width(line, font_face, cap_height) for line in lines
     ]
-    font_measurements = out.get_font_measurements(cap_height, font=font)
+    font_measurements = render_engine.get_font_measurements(font_face, cap_height)
     anchor, line_xs, line_ys = _apply_alignment(
         alignment, line_widths, line_spacing, box_width, font_measurements
     )
     rotation = _get_rotation(text)
 
     # first_line_width is used for TEXT, ATTRIB and ATTDEF stretching
     if line_widths:
@@ -353,22 +345,7 @@
         @ extra_transform
         @ rotation
         @ Matrix44.translate(*insert.xyz)
     )
     for i, (line, line_x, line_y) in enumerate(zip(lines, line_xs, line_ys)):
         transform = Matrix44.translate(line_x, line_y, 0) @ whole_text_transform
         yield line, transform, cap_height
-
-        if debug_draw_rect:
-            width = out.get_text_line_width(line, cap_height, font)
-            ps = list(
-                transform.transform_vertices(
-                    [
-                        Vec3(0, 0, 0),
-                        Vec3(width, 0, 0),
-                        Vec3(width, cap_height, 0),
-                        Vec3(0, cap_height, 0),
-                        Vec3(0, 0, 0),
-                    ]
-                )
-            )
-            draw_rect(ps, "#ff0000", out)
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/drawing/text_renderer.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/drawing/text_renderer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,34 @@
-#  Copyright (c) 2022, Manfred Moitzi
+#  Copyright (c) 2022-2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
-from typing import TypeVar, Generic, Optional
+from typing import TypeVar
 import abc
 from ezdxf.tools.fonts import FontFace, FontMeasurements
-from ezdxf.path import Path
+from ezdxf.path import Path2d
 
 T = TypeVar("T")
 
 
-class TextRenderer(abc.ABC, Generic[T]):
-    """Minimal requirement to be usable as a universal text renderer, for more
-    information see usage in PillowBackend().
-
-    Implementations:
-
-        - MplTextRenderer
-        - QtTextRenderer
-
-    """
-    @abc.abstractmethod
-    def get_font_properties(self, font: FontFace) -> T:
-        ...
+class TextRenderer(abc.ABC):
+    """Minimal requirement to be usable as a universal text renderer"""
 
     @abc.abstractmethod
-    def get_font_measurements(self, font_properties: T) -> FontMeasurements:
-        ...
-
-    @abc.abstractmethod
-    def get_scale(self, cap_height: float, font_properties: T) -> float:
+    def get_font_measurements(
+        self, font_face: FontFace, cap_height: float = 1.0
+    ) -> FontMeasurements:
         ...
 
     @abc.abstractmethod
     def get_text_line_width(
-        self, text: str, cap_height: float, font: Optional[FontFace] = None
+        self,
+        text: str,
+        font_face: FontFace,
+        cap_height: float = 1.0,
     ) -> float:
         ...
 
     @abc.abstractmethod
-    def get_ezdxf_path(self, text: str, font_properties: T) -> Path:
+    def get_text_path(
+        self, text: str, font_face: FontFace, cap_height: float = 1.0
+    ) -> Path2d:
         ...
-
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/dwg/classes_section.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/dwg/classes_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/dwg/const.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/dwg/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/dwg/crc.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/dwg/crc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/dwg/fileheader.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/dwg/fileheader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/dwg/header_section.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/dwg/header_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/dwg/loader.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/dwg/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/compiler.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/compiler.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/deps.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/deps.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/interpreter.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/interpreter.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,34 +7,63 @@
 from .deps import Vec2, NULLVEC2
 from .properties import RGB
 from .plotter import Plotter
 from .tokenizer import Command, pe_decode
 
 
 class Interpreter:
+    """The :class:`Interpreter` is the frontend for the :class:`Plotter` class.
+    The :meth:`run` methods interprets the low level HPGL commands from the
+    :func:`hpgl2_commands` parser and sends the commands to the virtual plotter
+    device, which sends his output to a low level :class:`Backend` class.
+
+    Most CAD application send a very restricted subset of commands to plotters,
+    mostly just polylines and filled polygons. Implementing the whole HPGL/2 command set
+    is not worth the effort - unless reality proofs otherwise.
+
+    Not implemented commands:
+
+        - the whole character group - text is send as filled polygons or polylines
+        - configuration group: IN, DF, RO, IW - the plotter is initialized by creating a
+          new plotter and page rotation is handled by the add-on itself
+        - polygon group: EA, ER, EW, FA, RR, WG, the rectangle and wedge commands
+        - line and fill attributes group: LA, RF, SM, SV, TR, UL, WU, linetypes and
+          hatch patterns are decomposed into simple lines by CAD applications
+
+    Args:
+        plotter: virtual :class:`Plotter` device
+
+    """
     def __init__(self, plotter: Plotter) -> None:
         self.errors: list[str] = []
         self.not_implemented_commands: set[str] = set()
         self._disabled_commands: set[str] = set()
         self.plotter = plotter
 
     def add_error(self, error: str) -> None:
         self.errors.append(error)
 
     def run(self, commands: list[Command]) -> None:
+        """Interprets the low level HPGL commands from the :func:`hpgl2_commands` parser
+        and sends the commands to the virtual plotter device.
+        """
         for name, args in commands:
             if name in self._disabled_commands:
                 continue
             method = getattr(self, f"cmd_{name.lower()}", None)
             if method:
                 method(args)
             elif name[0] in string.ascii_letters:
                 self.not_implemented_commands.add(name)
 
     def disable_commands(self, commands: Iterable[str]) -> None:
+        """Disable commands manually, like the scaling command ["SC", "IP", "IR"].
+        This is a feature for experts, because disabling commands which changes the pen
+        location may distort or destroy the plotter output.
+        """
         self._disabled_commands.update(commands)
 
     # Configure pens, line types, fill types
     def cmd_ft(self, args: list[bytes]):
         """Set fill type."""
         fill_type = 1
         spacing = 0.0
@@ -201,15 +230,15 @@
             return
         self.plotter.push_pen_state()
         # implicit pen down!
         self.plotter.pen_down()
         radius = to_float(args[0], 1.0)
         chord_angle = 5.0
         if arg_count > 1:
-            chord_angle = to_float(args[0], chord_angle)
+            chord_angle = to_float(args[1], chord_angle)
         self.plotter.plot_abs_circle(radius, chord_angle)
         self.plotter.pop_pen_state()
 
     def cmd_aa(self, args: list[bytes]):
         """Plot arc absolute."""
         if len(args) < 3:
             self.add_error("invalid arguments for AR command")
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/page.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/page.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 # 1 plot unit (plu) = 0.025mm
-# 40 plu = 1mm
+# 40 plu = 1 mm
 # 1016 plu = 1 inch
 # 3.39 plu = 1 dot @300 dpi
 
 from __future__ import annotations
 from typing import Sequence
 import math
 from .deps import Vec2, NULLVEC2
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/pdf_backend.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/pdf_backend.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 except ImportError:
     print("Python module PyMuPDF is required: https://pypi.org/project/PyMuPDF/")
     fitz = None
     pdf_is_supported = False
 
 from ezdxf.version import __version__
 from .deps import Vec2, Path, BoundingBox2d
-from .properties import Properties
+from .properties import Properties, FillMethod
 from .backend import Backend
 
 # Page coordinates are always plot units:
 # 1 plot unit (plu) = 0.025mm
 # 40 plu = 1mm
 # 1016 plu = 1 inch
 # 3.39 plu = 1 dot @300 dpi
@@ -26,14 +26,24 @@
 
 # Plot units to PDF units 1 PU = 1/72 inch
 PLU2PU = 72.0 / 1016.0
 MM2PU = 72.0 / 25.4  # 1 inch = 25.4 mm
 
 
 class PDFBackend(Backend):
+    """PDF backend.
+
+    The plot units (1 plu = 0.025mm) are converted to PDF units (1/72 inch) so the size
+    of image is the size of the original plot file in millimeters.
+
+    .. important::
+
+        Python module PyMuPDF is required: https://pypi.org/project/PyMuPDF/
+
+    """
     def __init__(self, bbox: BoundingBox2d) -> None:
         assert bbox.has_data is True, "extents of page are required"
         assert (
             pdf_is_supported
         ), "Python module PyMuPDF is required: https://pypi.org/project/PyMuPDF/"
         self.doc = fitz.open()
         self.doc.set_metadata(
@@ -58,18 +68,19 @@
             shape.drawLine(points[0], points[0])
         elif count == 2:
             shape.drawLine(points[0], points[1])
         else:
             shape.drawPolyline(points)
         shape.finish(
             width=properties.pen_width,
-            color=properties.pen_color.to_floats(),
+            color=properties.resolve_pen_color().to_floats(),
             lineJoin=1,
             lineCap=1,
             closePath=False,
+            even_odd = properties.fill_method == FillMethod.EVEN_ODD,
         )
         shape.commit()
 
     def draw_filled_polygon(
         self, properties: Properties, paths: Sequence[Path]
     ) -> None:
         # input coordinates are page coordinates
@@ -79,15 +90,15 @@
         for path in paths:
             points = self.adjust_points(path.flattening(distance=10))
             if len(points) < 3:
                 continue
             shape.drawPolyline(points)
         shape.finish(
             width=properties.pen_width,
-            fill=properties.pen_color.to_floats(),
+            fill=properties.resolve_fill_color().to_floats(),
         )
         shape.commit()
 
     def get_bytes(self) -> bytes:
         return self.doc.tobytes()
 
     def adjust_points(self, points) -> list[Vec2]:
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/plotter.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/plotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,30 @@
 from .properties import RGB, Properties
 from .backend import Backend
 from .polygon_buffer import PolygonBuffer
 from .page import Page
 
 
 class Plotter:
+    """
+    The :class:`Plotter` class represents a virtual plotter device.
+
+    The HPGL/2 commands send by the :class:`Interpreter` are processed into simple
+    polylines and filled polygons and send to low level :class:`Backend`.
+
+    HPGL/2 uses a units system called "Plot Units":
+
+    - 1 plot unit (plu) = 0.025mm
+    - 40 plu = 1 mm
+    - 1016 plu = 1 inch
+
+    The Plotter device does not support font rendering and page rotation (RO).
+    The scaling commands IP, RP, SC are supported.
+
+    """
     def __init__(self, backend: Backend) -> None:
         self.backend = backend
         self._output_backend = backend
         self._polygon_buffer = PolygonBuffer()
         self.page = Page(1189, 841)
         self.properties = Properties()
         self.is_pen_down = False
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/polygon_buffer.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/polygon_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/addons/hpgl2/svg_backend.py` & `ezdxf-1.1.0b0/src/ezdxf/addons/hpgl2/svg_backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,20 +2,26 @@
 #  License: MIT License
 from __future__ import annotations
 from typing import Sequence, Iterable
 from xml.etree import ElementTree as ET
 
 from .deps import Vec2, Path, BoundingBox2d, AnyVec
 from .backend import Backend
-from .properties import Properties, RGB, RGB_NONE
+from .properties import Properties, RGB, RGB_NONE, FillMethod
 
 LENGTH_MM = "{0:.0f}mm"
 
 
 class SVGBackend(Backend):
+    """Pure Python SVG backend.
+
+    The plot units are mapped 1:1 to ``viewBox`` units and the size of image is the size
+    of the original plot file in millimeters.
+
+    """
     def __init__(self, bbox: BoundingBox2d) -> None:
         assert bbox.has_data
         size = bbox.size
         width = str(round(size.x))
         height = str(round(size.y))
 
         self.root = ET.Element(
@@ -27,42 +33,45 @@
         )
         self.background = ET.SubElement(
             self.root, "rect", fill="white", x="0", y="0", width=width, height=height
         )
         self.filled_polygons = ET.SubElement(
             self.root, "g", stroke="none", fill="black"
         )
+        self.filled_polygons.set("fill-rule", "evenodd")
         self.polylines = ET.SubElement(self.root, "g", stroke="black", fill="none")
         self.polylines.set("stroke-linecap", "round")
         self.polylines.set("stroke-linejoin", "round")
 
         self.max_y = bbox.extmax.y  # type: ignore
         self.min_x = bbox.extmin.x  # type: ignore
 
     def draw_polyline(self, properties: Properties, points: Sequence[Vec2]) -> None:
         if not points:
             return
         points = self.adjust_points(points)
         path = ET.SubElement(self.polylines, "path", d=make_path_str(points))
         path.set("stroke-width", str(round(properties.pen_width * 40)))
-        s = make_rgb(properties.pen_color)
+        s = make_rgb(properties.resolve_pen_color())
         if s:
             path.set("stroke", s)
 
     def draw_filled_polygon(
         self, properties: Properties, paths: Sequence[Path]
     ) -> None:
         polygons = []
         for p in paths:
             points = self.adjust_points(p.flattening(distance=10))
             s = make_path_str(points, close=True)
             if s:
                 polygons.append(s)
         polygon = ET.SubElement(self.filled_polygons, "path", d=" ".join(polygons))
-        s = make_rgb(properties.pen_color)
+        if properties.fill_method != FillMethod.EVEN_ODD:
+            polygon.set("fill-rule", "nonzero")
+        s = make_rgb(properties.resolve_fill_color())
         if s:
             polygon.set("fill", s)
 
     def get_string(self) -> str:
         return ET.tostring(self.root, encoding="unicode", xml_declaration=True)
 
     def adjust_points(self, points: Iterable[AnyVec]) -> Sequence[Vec2]:
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/acad_proxy_entity.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/acad_table.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/acis.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/appdata.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/appid.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/appid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/arc.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/attrib.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/block.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/blockrecord.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/blockrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/boundary_paths.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/circle.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/dictionary.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/dimension.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/dimstyle.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/dimstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/dimstyleoverride.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/dimstyleoverride.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/dxfclass.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/dxfentity.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/dxfgfx.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/dxfgroups.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/dxfns.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/dxfns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/dxfobj.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/ellipse.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/factory.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/geodata.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/geodata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/gradient.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/gradient.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/hatch.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/hatch.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/helix.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/idbuffer.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/idbuffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/image.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/image.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/insert.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/layer.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/layout.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/leader.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/light.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/line.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/ltype.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/lwpolyline.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/lwpolyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/material.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/mesh.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/mleader.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/mline.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/mpolygon.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/mtext.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/mtext_columns.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/objectcollection.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/objectcollection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/oleframe.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/oleframe.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/pattern.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/point.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/polygon.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/polygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/polyline.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/shape.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/solid.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/spline.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/subentity.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/subentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/sun.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/table.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/text.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/textstyle.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/textstyle.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,27 +219,26 @@
         for this text style. Returns a font for a cap height of 1, if the
         text style has auto height (:attr:`Textstyle.dxf.height` is 0) and
         the given `cap_height` is ``None`` or 0.
         Uses the :attr:`Textstyle.dxf.width` attribute if the given `width_factor`
         is ``None`` or 0, the default value is 1.
         The attribute :attr:`Textstyle.dxf.big_font` is ignored.
         """
-        from ezdxf import options
         from ezdxf.tools import fonts
 
         ttf = ""
-        if options.use_matplotlib and self.has_extended_font_data:
+        if self.has_extended_font_data:
             family, italic, bold = self.get_extended_font_data()
             if family:
-                text_style = "italic" if italic else "normal"
-                text_weight = "bold" if bold else "normal"
+                text_style = "Italic" if italic else "Regular"
+                text_weight = 700 if bold else 400
                 font_face = fonts.FontFace(
                     family=family, style=text_style, weight=text_weight
                 )
-                ttf = fonts.find_ttf_path(font_face)
+                ttf = fonts.find_font_file_name(font_face)
         else:
             ttf = self.dxf.get("font", const.DEFAULT_TTF)
         if ttf == "":
             ttf = const.DEFAULT_TTF
         if cap_height is None or cap_height == 0.0:
             cap_height = self.dxf.height
         if cap_height == 0.0:
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/tolerance.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/ucs.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/underlay.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/view.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/view.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/viewport.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/visualstyle.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/visualstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/vport.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/vport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/xdata.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/xdict.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/xdict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/xline.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/entities/__init__.py` & `ezdxf-1.1.0b0/src/ezdxf/entities/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/layouts/base.py` & `ezdxf-1.1.0b0/src/ezdxf/layouts/base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/layouts/blocklayout.py` & `ezdxf-1.1.0b0/src/ezdxf/layouts/blocklayout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/layouts/layout.py` & `ezdxf-1.1.0b0/src/ezdxf/layouts/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/layouts/layouts.py` & `ezdxf-1.1.0b0/src/ezdxf/layouts/layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/attributes.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/const.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/encoding.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/extendedtags.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/extendedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/fileindex.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/fileindex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/hdrvars.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/hdrvars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/loader.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/packedtags.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/packedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/repair.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/repair.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/tagger.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/tagger.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/tags.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,458 +1,472 @@
-# Copyright (c) 2011-2022, Manfred Moitzi
+# Copyright (c) 2014-2022, Manfred Moitzi
 # License: MIT License
 """
-Tags
-----
+DXF Types
+=========
 
-A list of :class:`~ezdxf.lldxf.types.DXFTag`, inherits from Python standard list.
-Unlike the statement in the DXF Reference "Do not write programs that rely on
-the order given here", tag order is sometimes essential and some group codes
-may appear multiples times in one entity. At the worst case
-(:class:`~ezdxf.entities.material.Material`: normal map shares group codes with
-diffuse map) using same group codes with different meanings.
+Required DXF tag interface:
+
+    - property :attr:`code`: group code as int
+    - property :attr:`value`: tag value of unspecific type
+    - :meth:`dxfstr`: returns the DXF string
+    - :meth:`clone`: returns a deep copy of tag
 
 """
 from __future__ import annotations
-from typing import Iterable, Iterator, Any, Optional
-
-from .const import DXFStructureError, DXFValueError, STRUCTURE_MARKER
-from .types import DXFTag, EMBEDDED_OBJ_MARKER, EMBEDDED_OBJ_STR, dxftag
-from .tagger import internal_tag_compiler
-from . import types
+from typing import (
+    Union,
+    Iterable,
+    Sequence,
+    Type,
+    Any,
+)
+from array import array
+from itertools import chain
+from binascii import unhexlify, hexlify
+import reprlib
+from ezdxf.math import Vec3
+
+
+TAG_STRING_FORMAT = "%3d\n%s\n"
+POINT_CODES = {
+    10,
+    11,
+    12,
+    13,
+    14,
+    15,
+    16,
+    17,
+    18,
+    110,
+    111,
+    112,
+    210,
+    211,
+    212,
+    213,
+    1010,
+    1011,
+    1012,
+    1013,
+}
+
+MAX_GROUP_CODE = 1071
+GENERAL_MARKER = 0
+SUBCLASS_MARKER = 100
+XDATA_MARKER = 1001
+EMBEDDED_OBJ_MARKER = 101
+APP_DATA_MARKER = 102
+EXT_DATA_MARKER = 1001
+GROUP_MARKERS = {
+    GENERAL_MARKER,
+    SUBCLASS_MARKER,
+    EMBEDDED_OBJ_MARKER,
+    APP_DATA_MARKER,
+    EXT_DATA_MARKER,
+}
+BINARY_FLAGS = {70, 90}
+HANDLE_CODES = {5, 105}
+POINTER_CODES = set(chain(range(320, 370), range(390, 400), (480, 481, 1005)))
+
+# pointer group codes 320-329 are not translated during INSERT and XREF operations
+TRANSLATABLE_POINTER_CODES = set(
+    chain(range(330, 370), range(390, 400), (480, 481, 1005))
+)
+HEX_HANDLE_CODES = set(chain(HANDLE_CODES, POINTER_CODES))
+BINARY_DATA = {310, 311, 312, 313, 314, 315, 316, 317, 318, 319, 1004}
+EMBEDDED_OBJ_STR = "Embedded Object"
+
+BYTES = set(range(290, 300))  # bool
+
+INT16 = set(
+    chain(
+        range(60, 80),
+        range(170, 180),
+        range(270, 290),
+        range(370, 390),
+        range(400, 410),
+        range(1060, 1071),
+    )
+)
+
+INT32 = set(
+    chain(
+        range(90, 100),
+        range(420, 430),
+        range(440, 450),
+        range(450, 460),  # Long in DXF reference, ->signed<- or unsigned?
+        [1071],
+    )
+)
+
+INT64 = set(range(160, 170))
+
+DOUBLE = set(
+    chain(
+        range(10, 60),
+        range(110, 150),
+        range(210, 240),
+        range(460, 470),
+        range(1010, 1060),
+    )
+)
+
+VALID_XDATA_GROUP_CODES = {
+    1000,
+    1001,
+    1002,
+    1003,
+    1004,
+    1005,
+    1010,
+    1011,
+    1012,
+    1013,
+    1040,
+    1041,
+    1042,
+    1070,
+    1071,
+}
+
+
+def _build_type_table(types):
+    table = {}
+    for caster, codes in types:
+        for code in codes:
+            table[code] = caster
+    return table
+
+
+TYPE_TABLE = _build_type_table(
+    [
+        # all group code < 0 are spacial tags for internal use
+        (float, DOUBLE),
+        (int, BYTES),
+        (int, INT16),
+        (int, INT32),
+        (int, INT64),
+    ]
+)
 
-COMMENT_CODE = 999
 
+class DXFTag:
+    """Immutable DXFTag class.
 
-class Tags(list):
-    """Collection of :class:`~ezdxf.lldxf.types.DXFTag` as flat list.
-    Low level tag container, only required for advanced stuff.
+    Args:
+        code: group code as int
+        value: tag value, type depends on group code
 
     """
 
-    @classmethod
-    def from_text(cls, text: str) -> Tags:
-        """Constructor from DXF string."""
-        return cls(internal_tag_compiler(text))
+    __slots__ = ("_code", "_value")
 
-    @classmethod
-    def from_tuples(cls, tags: Iterable[tuple[int, Any]]) -> Tags:
-        return cls(DXFTag(code, value) for code, value in tags)
+    def __init__(self, code: int, value: Any):
+        self._code: int = int(code)
+        # Do not use _value, always use property value - overwritten in subclasses
+        self._value = value
+
+    def __str__(self) -> str:
+        """Returns content string ``'(code, value)'``."""
+        return str((self._code, self.value))
 
-    def __copy__(self) -> Tags:
-        return self.__class__(tag.clone() for tag in self)
+    def __repr__(self) -> str:
+        """Returns representation string ``'DXFTag(code, value)'``."""
+        return f"DXFTag{str(self)}"
 
-    clone = __copy__
+    @property
+    def code(self) -> int:
+        return self._code
 
-    def get_handle(self) -> str:
-        """Get DXF handle. Raises :class:`DXFValueError` if handle not exist.
+    @property
+    def value(self) -> Any:
+        return self._value
 
-        Returns:
-            handle as plain hex string like ``'FF00'``
+    def __getitem__(self, index: int):
+        """Returns :attr:`code` for index 0 and :attr:`value` for index 1,
+        emulates a tuple.
+        """
+        return (self._code, self.value)[index]
 
-        Raises:
-            DXFValueError: no handle found
+    def __iter__(self):
+        """Returns (code, value) tuples."""
+        yield self._code
+        yield self.value
 
+    def __eq__(self, other) -> bool:
+        """``True`` if `other` and `self` has same content for :attr:`code`
+        and :attr:`value`.
         """
-        try:
-            code, handle = self[1]  # fast path  for most common cases
-        except IndexError:
-            raise DXFValueError("No handle found.")
-
-        if code == 5 or code == 105:
-            return handle
-
-        for code, handle in self:
-            if code == 5 or code == 105:
-                return handle
-        raise DXFValueError("No handle found.")
+        return (self._code, self.value) == other
 
-    def replace_handle(self, new_handle: str) -> None:
-        """Replace existing handle.
+    def __hash__(self):
+        """Hash support, :class:`DXFTag` can be used in sets and as dict key."""
+        return hash((self._code, self._value))
 
-        Args:
-            new_handle: new handle as plain hex string e.g. ``'FF00'``
+    def dxfstr(self) -> str:
+        """Returns the DXF string e.g. ``'  0\\nLINE\\n'``"""
+        return TAG_STRING_FORMAT % (self.code, self._value)
 
+    def clone(self) -> "DXFTag":
+        """Returns a clone of itself, this method is necessary for the more
+        complex (and not immutable) DXF tag types.
         """
-        for index, tag in enumerate(self):
-            if tag.code in (5, 105):
-                self[index] = DXFTag(tag.code, new_handle)
-                return
-
-    def dxftype(self) -> str:
-        """Returns DXF type of entity, e.g. ``'LINE'``."""
-        return self[0].value
-
-    def has_tag(self, code: int) -> bool:
-        """Returns ``True`` if a :class:`~ezdxf.lldxf.types.DXFTag` with given
-        group `code` is present.
+        return self  # immutable tags
 
-        Args:
-            code: group code as int
 
-        """
-        return any(tag.code == code for tag in self)
+# Special marker tag
+NONE_TAG = DXFTag(0, 0)
 
-    def get_first_value(self, code: int, default=DXFValueError) -> Any:
-        """Returns value of first :class:`~ezdxf.lldxf.types.DXFTag` with given
-        group code or default if `default` != :class:`DXFValueError`, else
-        raises :class:`DXFValueError`.
-
-        Args:
-            code: group code as int
-            default: return value for default case or raises :class:`DXFValueError`
 
-        """
-        for tag in self:
-            if tag.code == code:
-                return tag.value
-        if default is DXFValueError:
-            raise DXFValueError(code)
-        else:
-            return default
+def uniform_appid(appid: str) -> str:
+    if appid[0] == "{":
+        return appid
+    else:
+        return "{" + appid
 
-    def get_first_tag(self, code: int, default=DXFValueError) -> DXFTag:
-        """Returns first :class:`~ezdxf.lldxf.types.DXFTag` with given group
-        code or `default`, if `default` != :class:`DXFValueError`, else raises
-        :class:`DXFValueError`.
-
-        Args:
-            code: group code as int
-            default: return value for default case or raises :class:`DXFValueError`
 
-        """
-        for tag in self:
-            if tag.code == code:
-                return tag
-        if default is DXFValueError:
-            raise DXFValueError(code)
-        else:
-            return default  # type: ignore
+def is_app_data_marker(tag: DXFTag) -> bool:
+    return tag.code == APP_DATA_MARKER and tag.value.startswith("{")  # type: ignore
 
-    def find_all(self, code: int) -> Tags:
-        """Returns a list of :class:`~ezdxf.lldxf.types.DXFTag` with given
-        group code.
 
-        Args:
-            code: group code as int
+def is_embedded_object_marker(tag: DXFTag) -> bool:
+    return tag.code == EMBEDDED_OBJ_MARKER and tag.value == EMBEDDED_OBJ_STR
 
-        """
-        return self.__class__(tag for tag in self if tag.code == code)
 
-    def tag_index(self, code: int, start: int = 0, end: Optional[int] = None) -> int:
-        """Return index of first :class:`~ezdxf.lldxf.types.DXFTag` with given
-        group code.
-
-        Args:
-            code: group code as int
-            start: start index as int
-            end: end index as int, ``None`` for end index = ``len(self)``
+def is_arbitrary_pointer(tag: DXFTag) -> bool:
+    """Arbitrary object handles; handle values that are taken "as is".
+    They are not translated during INSERT and XREF operations.
+    """
+    return 319 < tag.code < 330
 
-        """
-        if end is None:
-            end = len(self)
-        index = start
-        while index < end:
-            if self[index].code == code:
-                return index
-            index += 1
-        raise DXFValueError(code)
-
-    def update(self, tag: DXFTag) -> None:
-        """Update first existing tag with same group code as `tag`, raises
-        :class:`DXFValueError` if tag not exist.
 
-        """
-        index = self.tag_index(tag.code)
-        self[index] = tag
+def is_soft_pointer(tag: DXFTag) -> bool:
+    """Soft-pointer handle; arbitrary soft pointers to other objects within same DXF
+    file or drawing. Translated during INSERT and XREF operations.
+    """
+    return 329 < tag.code < 340 or tag.code == 1005
 
-    def set_first(self, tag: DXFTag) -> None:
-        """Update first existing tag with group code ``tag.code`` or append tag."""
-        try:
-            self.update(tag)
-        except DXFValueError:
-            self.append(tag)
 
-    def remove_tags(self, codes: Iterable[int]) -> None:
-        """Remove all tags inplace with group codes specified in `codes`.
+def is_hard_pointer(tag: DXFTag) -> bool:
+    """Hard-pointer handle; arbitrary hard pointers to other objects within same DXF
+    file or drawing. Translated during INSERT and XREF operations. Hard pointers
+    protect an object from being purged.
+    """
+    code = tag.code
+    return 339 < code < 350 or 389 < code < 400 or 479 < code < 482
 
-        Args:
-            codes: iterable of group codes as int
 
-        """
-        self[:] = [tag for tag in self if tag.code not in set(codes)]
+def is_soft_owner(tag: DXFTag) -> bool:
+    """Soft-owner handle; arbitrary soft ownership links to other objects within same
+    DXF file or drawing. Translated during INSERT and XREF operations.
+    """
+    return 349 < tag.code < 360
 
-    def pop_tags(self, codes: Iterable[int]) -> Iterator[DXFTag]:
-        """Pop tags with group codes specified in `codes`.
 
-        Args:
-            codes: iterable of group codes
+def is_hard_owner(tag: DXFTag) -> bool:
+    """Hard-owner handle; arbitrary hard ownership links to other objects within same
+    DXF file or drawing. Translated during INSERT and XREF operations. Hard owner handle
+    protect an object from being purged.
+    """
+    return 359 < tag.code < 370
 
-        """
-        remaining = []
-        codes = set(codes)
-        for tag in self:
-            if tag.code in codes:
-                yield tag
-            else:
-                remaining.append(tag)
-        self[:] = remaining
-
-    def remove_tags_except(self, codes: Iterable[int]) -> None:
-        """Remove all tags inplace except those with group codes specified in
-        `codes`.
 
-        Args:
-            codes: iterable of group codes
+def is_translatable_pointer(tag: DXFTag) -> bool:
+    # pointer group codes 320-329 are not translated during INSERT and XREF operations
+    return tag.code in TRANSLATABLE_POINTER_CODES
 
-        """
-        self[:] = [tag for tag in self if tag.code in set(codes)]
 
-    def filter(self, codes: Iterable[int]) -> Iterator[DXFTag]:
-        """Iterate and filter tags by group `codes`.
+class DXFVertex(DXFTag):
+    """Represents a 2D or 3D vertex, stores only the group code of the
+    x-component of the vertex, because the y-group-code is x-group-code + 10
+    and z-group-code id x-group-code+20, this is a rule that ALWAYS applies.
+    This tag is `immutable` by design, not by implementation.
 
-        Args:
-            codes: group codes to filter
+    Args:
+        code: group code of x-component
+        value: sequence of x, y and optional z values
 
-        """
-        return (tag for tag in self if tag.code not in set(codes))
+    """
 
-    def collect_consecutive_tags(
-        self, codes: Iterable[int], start: int = 0, end: Optional[int] = None
-    ) -> Tags:
-        """Collect all consecutive tags with group code in `codes`, `start` and
-        `end` delimits the search range. A tag code not in codes ends the
-        process.
-
-        Args:
-            codes: iterable of group codes
-            start: start index as int
-            end: end index as int, ``None`` for end index = ``len(self)``
+    __slots__ = ()
 
-        Returns:
-            collected tags as :class:`Tags`
+    def __init__(self, code: int, value: Iterable[float]):
+        super(DXFVertex, self).__init__(code, array("d", value))
 
-        """
-        codes = frozenset(codes)
-        index = int(start)
-        if end is None:
-            end = len(self)
-        bag = self.__class__()
-
-        while index < end:
-            tag = self[index]
-            if tag.code in codes:
-                bag.append(tag)
-                index += 1
-            else:
-                break
-        return bag
-
-    def has_embedded_objects(self) -> bool:
-        for tag in self:
-            if tag.code == EMBEDDED_OBJ_MARKER and tag.value == EMBEDDED_OBJ_STR:
-                return True
-        return False
+    def __str__(self) -> str:
+        return str(self.value)
 
-    @classmethod
-    def strip(cls, tags: Tags, codes: Iterable[int]) -> Tags:
-        """Constructor from `tags`, strips all tags with group codes in `codes`
-        from tags.
-
-        Args:
-            tags: iterable of :class:`~ezdxf.lldxf.types.DXFTag`
-            codes: iterable of group codes as int
+    def __repr__(self) -> str:
+        return f"DXFVertex({self.code}, {str(self)})"
+
+    def __hash__(self):
+        x, y, *z = self._value
+        z = 0.0 if len(z) == 0 else z[0]
+        return hash((self.code, x, y, z))
+
+    @property
+    def value(self) -> tuple[float, ...]:
+        return tuple(self._value)  # type: ignore
+
+    def dxftags(self) -> Iterable[DXFTag]:
+        """Returns all vertex components as single :class:`DXFTag` objects."""
+        c = self.code
+        return (
+            DXFTag(code, value) for code, value in zip((c, c + 10, c + 20), self.value)
+        )
 
-        """
-        return cls((tag for tag in tags if tag.code not in frozenset(codes)))
+    def dxfstr(self) -> str:
+        """Returns the DXF string for all vertex components."""
+        return "".join(tag.dxfstr() for tag in self.dxftags())
 
-    def get_soft_pointers(self) -> Tags:
-        """Returns all soft-pointer handles in group code range 330-339."""
-        return Tags(tag for tag in self if types.is_soft_pointer(tag))
-
-    def get_hard_pointers(self) -> Tags:
-        """Returns all hard-pointer handles in group code range 340-349, 390-399 and
-        480-481. Hard pointers protect an object from being purged.
-        """
-        return Tags(tag for tag in self if types.is_hard_pointer(tag))
 
-    def get_soft_owner_handles(self) -> Tags:
-        """Returns all soft-owner handles in group code range 350-359."""
-        return Tags(tag for tag in self if types.is_soft_owner(tag))
-
-    def get_hard_owner_handles(self) -> Tags:
-        """Returns all hard-owner handles in group code range 360-369."""
-        return Tags(tag for tag in self if types.is_hard_owner(tag))
-
-    def has_translatable_pointers(self) -> bool:
-        """Returns ``True`` if any pointer handle has to be translated during INSERT
-        and XREF operations.
-        """
-        return any(types.is_translatable_pointer(tag) for tag in self)
+class DXFBinaryTag(DXFTag):
+    """Immutable BinaryTags class - immutable by design, not by implementation."""
 
-    def get_translatable_pointers(self) -> Tags:
-        """Returns all pointer handles which should be translated during INSERT and XREF
-        operations.
-        """
-        return Tags(tag for tag in self if types.is_translatable_pointer(tag))
+    __slots__ = ()
+
+    def __str__(self) -> str:
+        return f"({self.code}, {self.tostring()})"
+
+    def __repr__(self) -> str:
+        return f"DXFBinaryTag({self.code}, {reprlib.repr(self.tostring())})"
 
+    def tostring(self) -> str:
+        """Returns binary value as single hex-string."""
+        assert isinstance(self.value, bytes)
+        return hexlify(self.value).upper().decode()
 
-def text2tags(text: str) -> Tags:
-    return Tags.from_text(text)
+    def dxfstr(self) -> str:
+        """Returns the DXF string for all vertex components."""
+        return TAG_STRING_FORMAT % (self.code, self.tostring())
+
+    @classmethod
+    def from_string(cls, code: int, value: Union[str, bytes]):
+        return cls(code, unhexlify(value))
 
 
-def group_tags(
-    tags: Iterable[DXFTag], splitcode: int = STRUCTURE_MARKER
-) -> Iterable[Tags]:
-    """Group of tags starts with a SplitTag and ends before the next SplitTag.
-    A SplitTag is a tag with code == splitcode, like (0, 'SECTION') for
-    splitcode == 0.
+def dxftag(code: int, value: Any) -> DXFTag:
+    """DXF tag factory function.
 
     Args:
-        tags: iterable of :class:`DXFTag`
-        splitcode: group code of split tag
+        code: group code
+        value: tag value
+
+    Returns: :class:`DXFTag` or inherited
 
     """
+    if code in BINARY_DATA:
+        return DXFBinaryTag(code, value)
+    elif code in POINT_CODES:
+        return DXFVertex(code, value)  # type: ignore
+    else:
+        return DXFTag(code, cast_tag_value(code, value))
 
-    # first do nothing, skip tags in front of the first split tag
-    def append(tag):
-        pass
-
-    group = None
-    for tag in tags:
-        if tag.code == splitcode:
-            if group is not None:
-                yield group
-            group = Tags([tag])
-            append = group.append  # redefine append: add tags to this group
+
+def tuples_to_tags(iterable: Iterable[tuple[int, Any]]) -> Iterable[DXFTag]:
+    """Returns an iterable if :class:`DXFTag` or inherited, accepts an
+    iterable of (code, value) tuples as input.
+    """
+    for code, value in iterable:
+        if code in POINT_CODES:
+            yield DXFVertex(code, value)  # type: ignore
+        elif code in BINARY_DATA:
+            assert isinstance(value, (str, bytes))
+            yield DXFBinaryTag.from_string(code, value)
         else:
-            append(tag)
-    if group is not None:
-        yield group
+            yield DXFTag(code, value)
 
 
-def text_to_multi_tags(
-    text: str, code: int = 303, size: int = 255, line_ending: str = "^J"
-) -> Tags:
-    text = "".join(text).replace("\n", line_ending)
+def is_valid_handle(handle) -> bool:
+    if isinstance(handle, str):
+        try:
+            int(handle, 16)
+            return True
+        except (ValueError, TypeError):
+            pass
+    return False
 
-    def chop():
-        start = 0
-        end = size
-        while start < len(text):
-            yield text[start:end]
-            start = end
-            end += size
 
-    return Tags(DXFTag(code, part) for part in chop())
+def is_binary_data(code: int) -> bool:
+    return code in BINARY_DATA
 
 
-def multi_tags_to_text(tags: Tags, line_ending: str = "^J") -> str:
-    return "".join(tag.value for tag in tags).replace(line_ending, "\n")
+def is_pointer_code(code: int) -> bool:
+    return code in POINTER_CODES
 
 
-OPEN_LIST = (1002, "{")
-CLOSE_LIST = (1002, "}")
+def is_point_code(code: int) -> bool:
+    return code in POINT_CODES
 
 
-def xdata_list(name: str, xdata_tags: Iterable) -> Tags:
-    tags = Tags()
-    if name:
-        tags.append((1000, name))
-    tags.append(OPEN_LIST)
-    tags.extend(xdata_tags)
-    tags.append(CLOSE_LIST)
-    return tags
+def is_point_tag(tag: Sequence) -> bool:
+    return tag[0] in POINT_CODES
 
 
-def remove_named_list_from_xdata(name: str, tags: Tags) -> Tags:
-    start, end = get_start_and_end_of_named_list_in_xdata(name, tags)
-    del tags[start:end]
-    return tags
+def cast_tag_value(code: int, value: Any) -> Any:
+    return TYPE_TABLE.get(code, str)(value)
 
 
-def get_named_list_from_xdata(name: str, tags: Tags) -> Tags:
-    start, end = get_start_and_end_of_named_list_in_xdata(name, tags)
-    return Tags(tags[start:end])
+def tag_type(code: int) -> Type:
+    return TYPE_TABLE.get(code, str)
 
 
-class NotFoundException(Exception):
-    pass
+def strtag(tag: Union[DXFTag, tuple[int, Any]]) -> str:
+    return TAG_STRING_FORMAT % tuple(tag)
 
 
-def get_start_and_end_of_named_list_in_xdata(name: str, tags: Tags) -> tuple[int, int]:
-    start = None
-    end = None
-    level = 0
-    for index in range(len(tags)):
-        tag = tags[index]
+def get_xcode_for(code) -> int:
+    if code in HEX_HANDLE_CODES:
+        return 1005
+    if code in BINARY_DATA:
+        return 1004
+    type_ = TYPE_TABLE.get(code, str)
+    if type_ is int:
+        return 1070
+    if type_ is float:
+        return 1040
+    return 1000
 
-        if start is None and tag == (1000, name):
-            next_tag = tags[index + 1]
-            if next_tag == OPEN_LIST:
-                start = index
-                continue
-        if start is not None:
-            if tag == OPEN_LIST:
-                level += 1
-            elif tag == CLOSE_LIST:
-                level -= 1
-            if level == 0:
-                end = index
-                break
 
-    if start is None:
-        raise NotFoundException
-    if end is None:
-        raise DXFStructureError('Invalid XDATA structure: missing  (1002, "}").')
-    return start, end + 1
+def cast_value(code: int, value):
+    if value is not None:
+        if code in POINT_CODES:
+            return Vec3(value)
+        return TYPE_TABLE.get(code, str)(value)
+    else:
+        return None
 
 
-def find_begin_and_end_of_encoded_xdata_tags(name: str, tags: Tags) -> tuple[int, int]:
-    """Find encoded XDATA tags, surrounded by group code 1000 tags
-    name_BEGIN and name_END (e.g. MTEXT column specification).
+TAG_TYPES = {
+    int: "<int>",
+    float: "<float>",
+    str: "<str>",
+}
 
-    Raises:
-        NotFoundError: tag group not found
-        DXFStructureError: missing begin- or end tag
 
-    """
-    begin_name = name + "_BEGIN"
-    end_name = name + "_END"
-    start = None
-    end = None
-    for index, (code, value) in enumerate(tags):
-        if code == 1000:
-            if value == begin_name:
-                start = index
-            elif value == end_name:
-                end = index + 1
-                break
-    if start is None:
-        if end is not None:  # end tag without begin tag!
-            raise DXFStructureError(
-                f"Invalid XDATA structure: missing begin tag (1000, {begin_name})."
-            )
-        raise NotFoundException
-    if end is None:
-        raise DXFStructureError(
-            f"Invalid XDATA structure: missing end tag (1000, {end_name})."
-        )
-    return start, end
+def tag_type_str(code: int) -> str:
+    if code in GROUP_MARKERS:
+        return "<ctrl>"
+    elif code in HANDLE_CODES:
+        return "<handle>"
+    elif code in POINTER_CODES:
+        return "<ref>"
+    elif is_point_code(code):
+        return "<point>"
+    elif is_binary_data(code):
+        return "<bin>"
+    else:
+        return TAG_TYPES[tag_type(code)]
 
 
-def binary_data_to_dxf_tags(
-    data: bytes,
-    length_group_code: int = 160,
-    value_group_code: int = 310,
-    value_size=127,
-) -> Tags:
-    """Convert binary data to DXF tags."""
-    tags = Tags()
-    length = len(data)
-    tags.append(dxftag(length_group_code, length))
-    index = 0
-    while index < length:
-        chunk = data[index : index + value_size]
-        tags.append(dxftag(value_group_code, chunk))
-        index += value_size
-    return tags
+def render_tag(tag: DXFTag, col: int) -> Any:
+    code, value = tag
+    if col == 0:
+        return str(code)
+    elif col == 1:
+        return tag_type_str(code)
+    elif col == 2:
+        return str(value)
+    else:
+        raise IndexError(col)
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/tagwriter.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/tagwriter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/types.py` & `ezdxf-1.1.0b0/src/ezdxf/sections/header.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,472 +1,371 @@
-# Copyright (c) 2014-2022, Manfred Moitzi
+# Copyright (c) 2011-2022, Manfred Moitzi
 # License: MIT License
-"""
-DXF Types
-=========
-
-Required DXF tag interface:
-
-    - property :attr:`code`: group code as int
-    - property :attr:`value`: tag value of unspecific type
-    - :meth:`dxfstr`: returns the DXF string
-    - :meth:`clone`: returns a deep copy of tag
-
-"""
 from __future__ import annotations
 from typing import (
-    Union,
+    Any,
     Iterable,
+    Iterator,
+    KeysView,
+    Optional,
     Sequence,
-    Type,
-    Any,
-)
-from array import array
-from itertools import chain
-from binascii import unhexlify, hexlify
-import reprlib
-from ezdxf.math import Vec3
-
-
-TAG_STRING_FORMAT = "%3d\n%s\n"
-POINT_CODES = {
-    10,
-    11,
-    12,
-    13,
-    14,
-    15,
-    16,
-    17,
-    18,
-    110,
-    111,
-    112,
-    210,
-    211,
-    212,
-    213,
-    1010,
-    1011,
-    1012,
-    1013,
-}
-
-MAX_GROUP_CODE = 1071
-GENERAL_MARKER = 0
-SUBCLASS_MARKER = 100
-XDATA_MARKER = 1001
-EMBEDDED_OBJ_MARKER = 101
-APP_DATA_MARKER = 102
-EXT_DATA_MARKER = 1001
-GROUP_MARKERS = {
-    GENERAL_MARKER,
-    SUBCLASS_MARKER,
-    EMBEDDED_OBJ_MARKER,
-    APP_DATA_MARKER,
-    EXT_DATA_MARKER,
-}
-BINARY_FLAGS = {70, 90}
-HANDLE_CODES = {5, 105}
-POINTER_CODES = set(chain(range(320, 370), range(390, 400), (480, 481, 1005)))
-
-# pointer group codes 320-329 are not translated during INSERT and XREF operations
-TRANSLATABLE_POINTER_CODES = set(
-    chain(range(330, 370), range(390, 400), (480, 481, 1005))
-)
-HEX_HANDLE_CODES = set(chain(HANDLE_CODES, POINTER_CODES))
-BINARY_DATA = {310, 311, 312, 313, 314, 315, 316, 317, 318, 319, 1004}
-EMBEDDED_OBJ_STR = "Embedded Object"
-
-BYTES = set(range(290, 300))  # bool
-
-INT16 = set(
-    chain(
-        range(60, 80),
-        range(170, 180),
-        range(270, 290),
-        range(370, 390),
-        range(400, 410),
-        range(1060, 1071),
-    )
+    TYPE_CHECKING,
+    Union,
 )
+import logging
+from collections import OrderedDict
 
-INT32 = set(
-    chain(
-        range(90, 100),
-        range(420, 430),
-        range(440, 450),
-        range(450, 460),  # Long in DXF reference, ->signed<- or unsigned?
-        [1071],
-    )
+from ezdxf.lldxf import const
+from ezdxf.lldxf.tags import group_tags, Tags, DXFTag
+from ezdxf.lldxf.types import strtag
+from ezdxf.lldxf.validator import header_validator
+from ezdxf.sections.headervars import (
+    HEADER_VAR_MAP,
+    version_specific_group_code,
 )
 
-INT64 = set(range(160, 170))
+if TYPE_CHECKING:
+    from ezdxf.lldxf.tagwriter import AbstractTagWriter
 
-DOUBLE = set(
-    chain(
-        range(10, 60),
-        range(110, 150),
-        range(210, 240),
-        range(460, 470),
-        range(1010, 1060),
-    )
-)
-
-VALID_XDATA_GROUP_CODES = {
-    1000,
-    1001,
-    1002,
-    1003,
-    1004,
-    1005,
-    1010,
-    1011,
-    1012,
-    1013,
-    1040,
-    1041,
-    1042,
-    1070,
-    1071,
-}
-
-
-def _build_type_table(types):
-    table = {}
-    for caster, codes in types:
-        for code in codes:
-            table[code] = caster
-    return table
-
-
-TYPE_TABLE = _build_type_table(
-    [
-        # all group code < 0 are spacial tags for internal use
-        (float, DOUBLE),
-        (int, BYTES),
-        (int, INT16),
-        (int, INT32),
-        (int, INT64),
-    ]
-)
+logger = logging.getLogger("ezdxf")
 
+MIN_HEADER_TEXT = """  0
+SECTION
+  2
+HEADER
+  9
+$ACADVER
+  1
+AC1009
+  9
+$DWGCODEPAGE
+  3
+ANSI_1252
+  9
+$HANDSEED
+  5
+FF
+"""
 
-class DXFTag:
-    """Immutable DXFTag class.
-
-    Args:
-        code: group code as int
-        value: tag value, type depends on group code
+# Additional variables may be stored as DICTIONARYVAR in the OBJECTS
+# section in the DICTIONARY "AcDbVariableDictionary" of the root dict.
+# - CANNOSCALE
+# - CENTEREXE
+# - CENTERLTYPEFILE
+# - CETRANSPARENCY
+# - CMLEADERSTYLE
+# - CTABLESTYLE
+# - CVIEWDETAILSTYLE
+# - CVIEWSECTIONSTYLE
+# - LAYEREVAL
+# - LAYERNOTIFY
+# - LIGHTINGUNITS
+# - MSLTSCALE
+
+
+class CustomVars:
+    """The :class:`CustomVars` class stores custom properties in the DXF header as
+    $CUSTOMPROPERTYTAG and $CUSTOMPROPERTY values. Custom properties require DXF R2004
+    or later, `ezdxf` can create custom properties for older DXF versions as well, but
+    AutoCAD will not show that properties.
 
     """
 
-    __slots__ = ("_code", "_value")
+    def __init__(self) -> None:
+        self.properties: list[tuple[str, str]] = list()
 
-    def __init__(self, code: int, value: Any):
-        self._code: int = int(code)
-        # Do not use _value, always use property value - overwritten in subclasses
-        self._value = value
+    def __len__(self) -> int:
+        """Count of custom properties."""
+        return len(self.properties)
+
+    def __iter__(self) -> Iterator[tuple[str, str]]:
+        """Iterate over all custom properties as ``(tag, value)`` tuples."""
+        return iter(self.properties)
+
+    def clear(self) -> None:
+        """Remove all custom properties."""
+        self.properties.clear()
+
+    def append(self, tag: str, value: str) -> None:
+        """Add custom property as ``(tag, value)`` tuple."""
+        # custom properties always stored as strings
+        self.properties.append((tag, str(value)))
+
+    def get(self, tag: str, default: Optional[str] = None):
+        """Returns the value of the first custom property `tag`."""
+        for key, value in self.properties:
+            if key == tag:
+                return value
+        else:
+            return default
 
-    def __str__(self) -> str:
-        """Returns content string ``'(code, value)'``."""
-        return str((self._code, self.value))
+    def has_tag(self, tag: str) -> bool:
+        """Returns ``True`` if custom property `tag` exist."""
+        return self.get(tag) is not None
 
-    def __repr__(self) -> str:
-        """Returns representation string ``'DXFTag(code, value)'``."""
-        return f"DXFTag{str(self)}"
+    def remove(self, tag: str, all: bool = False) -> None:
+        """Removes the first occurrence of custom property `tag`, removes all
+        occurrences if `all` is ``True``.
 
-    @property
-    def code(self) -> int:
-        return self._code
+        Raises `:class:`DXFValueError` if `tag`  does not exist.
 
-    @property
-    def value(self) -> Any:
-        return self._value
-
-    def __getitem__(self, index: int):
-        """Returns :attr:`code` for index 0 and :attr:`value` for index 1,
-        emulates a tuple.
         """
-        return (self._code, self.value)[index]
+        found_tag = False
+        for item in self.properties:
+            if item[0] == tag:
+                self.properties.remove(item)
+                found_tag = True
+                if not all:
+                    return
+        if not found_tag:
+            raise const.DXFValueError(f"Tag '{tag}' does not exist")
+
+    def replace(self, tag: str, value: str) -> None:
+        """Replaces the value of the first custom property `tag` by a new
+        `value`.
 
-    def __iter__(self):
-        """Returns (code, value) tuples."""
-        yield self._code
-        yield self.value
-
-    def __eq__(self, other) -> bool:
-        """``True`` if `other` and `self` has same content for :attr:`code`
-        and :attr:`value`.
-        """
-        return (self._code, self.value) == other
+        Raises :class:`DXFValueError` if `tag`  does not exist.
 
-    def __hash__(self):
-        """Hash support, :class:`DXFTag` can be used in sets and as dict key."""
-        return hash((self._code, self._value))
-
-    def dxfstr(self) -> str:
-        """Returns the DXF string e.g. ``'  0\\nLINE\\n'``"""
-        return TAG_STRING_FORMAT % (self.code, self._value)
-
-    def clone(self) -> "DXFTag":
-        """Returns a clone of itself, this method is necessary for the more
-        complex (and not immutable) DXF tag types.
         """
-        return self  # immutable tags
-
-
-# Special marker tag
-NONE_TAG = DXFTag(0, 0)
-
-
-def uniform_appid(appid: str) -> str:
-    if appid[0] == "{":
-        return appid
-    else:
-        return "{" + appid
-
-
-def is_app_data_marker(tag: DXFTag) -> bool:
-    return tag.code == APP_DATA_MARKER and tag.value.startswith("{")  # type: ignore
-
-
-def is_embedded_object_marker(tag: DXFTag) -> bool:
-    return tag.code == EMBEDDED_OBJ_MARKER and tag.value == EMBEDDED_OBJ_STR
-
-
-def is_arbitrary_pointer(tag: DXFTag) -> bool:
-    """Arbitrary object handles; handle values that are taken "as is".
-    They are not translated during INSERT and XREF operations.
-    """
-    return 319 < tag.code < 330
-
-
-def is_soft_pointer(tag: DXFTag) -> bool:
-    """Soft-pointer handle; arbitrary soft pointers to other objects within same DXF
-    file or drawing. Translated during INSERT and XREF operations.
-    """
-    return 329 < tag.code < 340 or tag.code == 1005
-
-
-def is_hard_pointer(tag: DXFTag) -> bool:
-    """Hard-pointer handle; arbitrary hard pointers to other objects within same DXF
-    file or drawing. Translated during INSERT and XREF operations. Hard pointers
-    protect an object from being purged.
-    """
-    code = tag.code
-    return 339 < code < 350 or 389 < code < 400 or 479 < code < 482
-
-
-def is_soft_owner(tag: DXFTag) -> bool:
-    """Soft-owner handle; arbitrary soft ownership links to other objects within same
-    DXF file or drawing. Translated during INSERT and XREF operations.
-    """
-    return 349 < tag.code < 360
-
-
-def is_hard_owner(tag: DXFTag) -> bool:
-    """Hard-owner handle; arbitrary hard ownership links to other objects within same
-    DXF file or drawing. Translated during INSERT and XREF operations. Hard owner handle
-    protect an object from being purged.
-    """
-    return 359 < tag.code < 370
-
-
-def is_translatable_pointer(tag: DXFTag) -> bool:
-    # pointer group codes 320-329 are not translated during INSERT and XREF operations
-    return tag.code in TRANSLATABLE_POINTER_CODES
-
-
-class DXFVertex(DXFTag):
-    """Represents a 2D or 3D vertex, stores only the group code of the
-    x-component of the vertex, because the y-group-code is x-group-code + 10
-    and z-group-code id x-group-code+20, this is a rule that ALWAYS applies.
-    This tag is `immutable` by design, not by implementation.
-
-    Args:
-        code: group code of x-component
-        value: sequence of x, y and optional z values
-
-    """
+        properties = self.properties
+        for index in range(len(properties)):
+            name = properties[index][0]
+            if name == tag:
+                properties[index] = (name, value)
+                return
+
+        raise const.DXFValueError(f"Tag '{tag}' does not exist")
+
+    def write(self, tagwriter: AbstractTagWriter) -> None:
+        """Export custom properties as DXF tags. (internal API)"""
+        for tag, value in self.properties:
+            s = f"  9\n$CUSTOMPROPERTYTAG\n  1\n{tag}\n  9\n$CUSTOMPROPERTY\n  1\n{value}\n"
+            tagwriter.write_str(s)
+
+
+def default_vars() -> OrderedDict:
+    vars = OrderedDict()
+    for vardef in HEADER_VAR_MAP.values():
+        vars[vardef.name] = HeaderVar(DXFTag(vardef.code, vardef.default))
+    return vars
+
+
+class HeaderSection:
+    MIN_HEADER_TAGS = Tags.from_text(MIN_HEADER_TEXT)
+    name = "HEADER"
+
+    def __init__(self) -> None:
+        self.hdrvars: dict[str, HeaderVar] = OrderedDict()
+        self.custom_vars = CustomVars()
 
-    __slots__ = ()
-
-    def __init__(self, code: int, value: Iterable[float]):
-        super(DXFVertex, self).__init__(code, array("d", value))
-
-    def __str__(self) -> str:
-        return str(self.value)
-
-    def __repr__(self) -> str:
-        return f"DXFVertex({self.code}, {str(self)})"
-
-    def __hash__(self):
-        x, y, *z = self._value
-        z = 0.0 if len(z) == 0 else z[0]
-        return hash((self.code, x, y, z))
-
-    @property
-    def value(self) -> tuple[float, ...]:
-        return tuple(self._value)  # type: ignore
-
-    def dxftags(self) -> Iterable[DXFTag]:
-        """Returns all vertex components as single :class:`DXFTag` objects."""
-        c = self.code
-        return (
-            DXFTag(code, value) for code, value in zip((c, c + 10, c + 20), self.value)
-        )
-
-    def dxfstr(self) -> str:
-        """Returns the DXF string for all vertex components."""
-        return "".join(tag.dxfstr() for tag in self.dxftags())
-
-
-class DXFBinaryTag(DXFTag):
-    """Immutable BinaryTags class - immutable by design, not by implementation."""
-
-    __slots__ = ()
-
-    def __str__(self) -> str:
-        return f"({self.code}, {self.tostring()})"
+    @classmethod
+    def load(cls, tags: Optional[Iterable[DXFTag]] = None) -> HeaderSection:
+        """Constructor to generate header variables loaded from DXF files
+        (untrusted environment).
 
-    def __repr__(self) -> str:
-        return f"DXFBinaryTag({self.code}, {reprlib.repr(self.tostring())})"
+        Args:
+            tags: DXF tags as Tags() or ExtendedTags()
 
-    def tostring(self) -> str:
-        """Returns binary value as single hex-string."""
-        assert isinstance(self.value, bytes)
-        return hexlify(self.value).upper().decode()
-
-    def dxfstr(self) -> str:
-        """Returns the DXF string for all vertex components."""
-        return TAG_STRING_FORMAT % (self.code, self.tostring())
+        (internal API)
+        """
+        if tags is None:  # create default header
+            # files without a header have the default version: R12
+            return cls.new(dxfversion=const.DXF12)
+        section = cls()
+        section.load_tags(iter(tags))
+        return section
 
     @classmethod
-    def from_string(cls, code: int, value: Union[str, bytes]):
-        return cls(code, unhexlify(value))
-
-
-def dxftag(code: int, value: Any) -> DXFTag:
-    """DXF tag factory function.
+    def new(cls, dxfversion=const.LATEST_DXF_VERSION) -> HeaderSection:
+        section = HeaderSection()
+        section.hdrvars = default_vars()
+        section["$ACADVER"] = dxfversion
+        return section
+
+    def load_tags(self, tags: Iterable[DXFTag]) -> None:
+        """Constructor to generate header variables loaded from DXF files
+        (untrusted environment).
 
-    Args:
-        code: group code
-        value: tag value
+        Args:
+            tags: DXF tags as Tags() or ExtendedTags()
 
-    Returns: :class:`DXFTag` or inherited
+        """
+        _tags = iter(tags) or iter(self.MIN_HEADER_TAGS)
+        section_tag = next(_tags)
+        name_tag = next(_tags)
+
+        if section_tag != (0, "SECTION") or name_tag != (2, "HEADER"):
+            raise const.DXFStructureError("Critical structure error in HEADER section.")
+
+        groups = group_tags(header_validator(_tags), splitcode=9)
+        custom_property_stack = []  # collect $CUSTOMPROPERTY/TAG
+        for group in groups:
+            name = group[0].value
+            value = group[1]
+            if name in ("$CUSTOMPROPERTYTAG", "$CUSTOMPROPERTY"):
+                custom_property_stack.append(value.value)
+            else:
+                self.hdrvars[name] = HeaderVar(value)
+
+        custom_property_stack.reverse()
+        while len(custom_property_stack):
+            try:
+                self.custom_vars.append(
+                    tag=custom_property_stack.pop(),
+                    value=custom_property_stack.pop(),
+                )
+            except IndexError:  # internal exception
+                break
 
-    """
-    if code in BINARY_DATA:
-        return DXFBinaryTag(code, value)
-    elif code in POINT_CODES:
-        return DXFVertex(code, value)  # type: ignore
-    else:
-        return DXFTag(code, cast_tag_value(code, value))
+    @classmethod
+    def from_text(cls, text: str) -> HeaderSection:
+        """Load constructor from text for testing"""
+        return cls.load(Tags.from_text(text))  # type: ignore
+
+    def _headervar_factory(self, key: str, value: Any) -> DXFTag:
+        if key in HEADER_VAR_MAP:
+            factory = HEADER_VAR_MAP[key].factory
+            return factory(value)
+        else:
+            raise const.DXFKeyError(f"Invalid header variable {key}.")
 
+    def __len__(self) -> int:
+        """Returns count of header variables."""
+        return len(self.hdrvars)
+
+    def __contains__(self, key) -> bool:
+        """Returns ``True`` if header variable `key` exist."""
+        return key in self.hdrvars
+
+    def varnames(self) -> KeysView:
+        """Returns an iterable of all header variable names."""
+        return self.hdrvars.keys()
+
+    def export_dxf(self, tagwriter: AbstractTagWriter) -> None:
+        """Exports header section as DXF tags. (internal API)"""
+
+        def _write(name: str, value: Any) -> None:
+            if value.value is None:
+                logger.info(f"did not write header var {name}, value is None.")
+                return
+            tagwriter.write_tag2(9, name)
+            group_code = version_specific_group_code(name, dxfversion)
+            # fix invalid group codes
+            if group_code != value.code:
+                value = HeaderVar((group_code, value.value))
+            tagwriter.write_str(str(value))
+
+        dxfversion: str = tagwriter.dxfversion
+        write_handles = tagwriter.write_handles
+
+        tagwriter.write_str("  0\nSECTION\n  2\nHEADER\n")
+        save = self["$ACADVER"]
+        self["$ACADVER"] = dxfversion
+        for name, value in header_vars_by_priority(self.hdrvars, dxfversion):
+            if not write_handles and name == "$HANDSEED":
+                continue  # skip $HANDSEED
+            _write(name, value)
+            if name == "$LASTSAVEDBY":  # ugly hack, but necessary for AutoCAD
+                self.custom_vars.write(tagwriter)
+        self["$ACADVER"] = save
+        tagwriter.write_str("  0\nENDSEC\n")
+
+    def get(self, key: str, default: Any = None) -> Any:
+        """Returns value of header variable `key` if exist, else the `default`
+        value.
 
-def tuples_to_tags(iterable: Iterable[tuple[int, Any]]) -> Iterable[DXFTag]:
-    """Returns an iterable if :class:`DXFTag` or inherited, accepts an
-    iterable of (code, value) tuples as input.
-    """
-    for code, value in iterable:
-        if code in POINT_CODES:
-            yield DXFVertex(code, value)  # type: ignore
-        elif code in BINARY_DATA:
-            assert isinstance(value, (str, bytes))
-            yield DXFBinaryTag.from_string(code, value)
+        """
+        if key in self.hdrvars:
+            return self.__getitem__(key)
         else:
-            yield DXFTag(code, value)
+            return default
 
+    def __getitem__(self, key: str) -> Any:
+        """Get header variable `key` by index operator like:
+        :code:`drawing.header['$ACADVER']`
 
-def is_valid_handle(handle) -> bool:
-    if isinstance(handle, str):
+        """
         try:
-            int(handle, 16)
-            return True
-        except (ValueError, TypeError):
-            pass
-    return False
-
-
-def is_binary_data(code: int) -> bool:
-    return code in BINARY_DATA
-
-
-def is_pointer_code(code: int) -> bool:
-    return code in POINTER_CODES
-
-
-def is_point_code(code: int) -> bool:
-    return code in POINT_CODES
-
-
-def is_point_tag(tag: Sequence) -> bool:
-    return tag[0] in POINT_CODES
-
-
-def cast_tag_value(code: int, value: Any) -> Any:
-    return TYPE_TABLE.get(code, str)(value)
-
-
-def tag_type(code: int) -> Type:
-    return TYPE_TABLE.get(code, str)
-
-
-def strtag(tag: Union[DXFTag, tuple[int, Any]]) -> str:
-    return TAG_STRING_FORMAT % tuple(tag)
-
-
-def get_xcode_for(code) -> int:
-    if code in HEX_HANDLE_CODES:
-        return 1005
-    if code in BINARY_DATA:
-        return 1004
-    type_ = TYPE_TABLE.get(code, str)
-    if type_ is int:
-        return 1070
-    if type_ is float:
-        return 1040
-    return 1000
-
-
-def cast_value(code: int, value):
-    if value is not None:
-        if code in POINT_CODES:
-            return Vec3(value)
-        return TYPE_TABLE.get(code, str)(value)
-    else:
-        return None
+            return self.hdrvars[key].value
+        except KeyError:  # map exception
+            raise const.DXFKeyError(str(key))
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        """Set header variable `key` to `value` by index operator like:
+        :code:`drawing.header['$ANGDIR'] = 1`
 
+        """
+        try:
+            tags = self._headervar_factory(key, value)
+        except (IndexError, ValueError):
+            raise const.DXFValueError(str(value))
+        self.hdrvars[key] = HeaderVar(tags)
+
+    def __delitem__(self, key: str) -> None:
+        """Delete header variable `key` by index operator like:
+        :code:`del drawing.header['$ANGDIR']`
 
-TAG_TYPES = {
-    int: "<int>",
-    float: "<float>",
-    str: "<str>",
-}
+        """
+        try:
+            del self.hdrvars[key]
+        except KeyError:  # map exception
+            raise const.DXFKeyError(str(key))
+
+    def reset_wcs(self):
+        """Reset the current UCS settings to the :ref:`WCS`."""
+        self["$UCSBASE"] = ""
+        self["$UCSNAME"] = ""
+        self["$UCSORG"] = (0, 0, 0)
+        self["$UCSXDIR"] = (1, 0, 0)
+        self["$UCSYDIR"] = (0, 1, 0)
+        self["$UCSORTHOREF"] = ""
+        self["$UCSORTHOVIEW"] = 0
+        self["$UCSORGTOP"] = (0, 0, 0)
+        self["$UCSORGBOTTOM"] = (0, 0, 0)
+        self["$UCSORGLEFT"] = (0, 0, 0)
+        self["$UCSORGRIGHT"] = (0, 0, 0)
+        self["$UCSORGFRONT"] = (0, 0, 0)
+        self["$UCSORGBACK"] = (0, 0, 0)
+
+
+def header_vars_by_priority(
+    header_vars: dict[str, HeaderVar], dxfversion: str
+) -> Iterable[tuple]:
+    order = []
+    for name, value in header_vars.items():
+        vardef = HEADER_VAR_MAP.get(name, None)
+        if vardef is None:
+            logger.info(f"Header variable {name} ignored, dxfversion={dxfversion}.")
+            continue
+        if vardef.mindxf <= dxfversion <= vardef.maxdxf:
+            order.append((vardef.priority, (name, value)))
+    order.sort()
+    for priority, tag in order:
+        yield tag
+
+
+class HeaderVar:
+    def __init__(self, tag: Union[DXFTag, Sequence]):
+        self.tag = tag
 
+    @property
+    def code(self) -> int:
+        return self.tag[0]
 
-def tag_type_str(code: int) -> str:
-    if code in GROUP_MARKERS:
-        return "<ctrl>"
-    elif code in HANDLE_CODES:
-        return "<handle>"
-    elif code in POINTER_CODES:
-        return "<ref>"
-    elif is_point_code(code):
-        return "<point>"
-    elif is_binary_data(code):
-        return "<bin>"
-    else:
-        return TAG_TYPES[tag_type(code)]
+    @property
+    def value(self) -> Any:
+        return self.tag[1]
 
+    @property
+    def ispoint(self) -> bool:
+        return self.code == 10
 
-def render_tag(tag: DXFTag, col: int) -> Any:
-    code, value = tag
-    if col == 0:
-        return str(code)
-    elif col == 1:
-        return tag_type_str(code)
-    elif col == 2:
-        return str(value)
-    else:
-        raise IndexError(col)
+    def __str__(self) -> str:
+        if self.ispoint:
+            code, value = self.tag
+            s = []
+            for coord in value:
+                s.append(strtag((code, coord)))
+                code += 10
+            return "".join(s)
+        else:
+            return strtag(self.tag)  # type: ignore
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/lldxf/validator.py` & `ezdxf-1.1.0b0/src/ezdxf/lldxf/validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/arc.py` & `ezdxf-1.1.0b0/src/ezdxf/math/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/bbox.py` & `ezdxf-1.1.0b0/src/ezdxf/math/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/bezier.py` & `ezdxf-1.1.0b0/src/ezdxf/math/bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/bezier_interpolation.py` & `ezdxf-1.1.0b0/src/ezdxf/math/bezier_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/box.py` & `ezdxf-1.1.0b0/src/ezdxf/math/box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/bspline.py` & `ezdxf-1.1.0b0/src/ezdxf/math/bspline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1195,30 +1195,14 @@
         """Returns a new :class:`BSpline` object transformed by a
         :class:`Matrix44` transformation matrix.
 
         """
         cpoints = m.transform_vertices(self.control_points)
         return BSpline(cpoints, self.order, self.knots(), self.weights())
 
-    def to_nurbs_python_curve(self):
-        """Returns a :class:`geomdl.BSpline.Curve` object, if the
-        `NURBS-Python <https://pypi.org/project/geomdl/>`_ package is installed.
-
-        """
-        if self._basis.is_rational:
-            from geomdl.NURBS import Curve
-        else:
-            from geomdl.BSpline import Curve
-        curve = Curve()
-        curve.degree = self.degree
-        curve.ctrlpts = [v.xyz for v in self.control_points]
-        curve.knotvector = self.knots()
-        curve.weights = self.weights()
-        return curve
-
     def bezier_decomposition(self) -> Iterable[list[Vec3]]:
         """Decompose a non-rational B-spline into multiple Bézier curves.
 
         This is the preferred method to represent the most common non-rational
         B-splines of 3rd degree by cubic Bézier curves, which are often supported
         by render backends.
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/bulge.py` & `ezdxf-1.1.0b0/src/ezdxf/math/bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/circle.py` & `ezdxf-1.1.0b0/src/ezdxf/math/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/clipping.py` & `ezdxf-1.1.0b0/src/ezdxf/math/clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/clustering.py` & `ezdxf-1.1.0b0/src/ezdxf/math/clustering.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/construct2d.py` & `ezdxf-1.1.0b0/src/ezdxf/math/construct2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/construct3d.py` & `ezdxf-1.1.0b0/src/ezdxf/math/construct3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/cspline.py` & `ezdxf-1.1.0b0/src/ezdxf/math/cspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/curvetools.py` & `ezdxf-1.1.0b0/src/ezdxf/math/curvetools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/ellipse.py` & `ezdxf-1.1.0b0/src/ezdxf/math/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/eulerspiral.py` & `ezdxf-1.1.0b0/src/ezdxf/math/eulerspiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/linalg.py` & `ezdxf-1.1.0b0/src/ezdxf/math/linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/line.py` & `ezdxf-1.1.0b0/src/ezdxf/math/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/offset2d.py` & `ezdxf-1.1.0b0/src/ezdxf/math/offset2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/parametrize.py` & `ezdxf-1.1.0b0/src/ezdxf/math/parametrize.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/perlin.py` & `ezdxf-1.1.0b0/src/ezdxf/math/perlin.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/polyline.py` & `ezdxf-1.1.0b0/src/ezdxf/math/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/rtree.py` & `ezdxf-1.1.0b0/src/ezdxf/math/rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/shape.py` & `ezdxf-1.1.0b0/src/ezdxf/math/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/surfaces.py` & `ezdxf-1.1.0b0/src/ezdxf/math/surfaces.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/transformtools.py` & `ezdxf-1.1.0b0/src/ezdxf/math/transformtools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/triangulation.py` & `ezdxf-1.1.0b0/src/ezdxf/math/triangulation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/ucs.py` & `ezdxf-1.1.0b0/src/ezdxf/math/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/_bezier3p.py` & `ezdxf-1.1.0b0/src/ezdxf/math/_bezier3p.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) 2021-2022 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
-from typing import Iterable, Sequence, Type, Optional, TYPE_CHECKING
+from typing import Iterable, Iterator, Sequence, Type, Optional, TYPE_CHECKING
 import math
 
 # The pure Python implementation can't import from ._ctypes or ezdxf.math!
 from ._vector import Vec3, Vec2
 from ._matrix44 import Matrix44
 
 if TYPE_CHECKING:
@@ -35,57 +35,57 @@
 
     """
     __slots__ = ("_control_points", "_offset")
 
     def __init__(self, defpoints: Sequence[UVec]):
         if len(defpoints) == 3:
             is3d = any(len(p) > 2 for p in defpoints)
-            vector_class: Type["AnyVec"] = Vec3 if is3d else Vec2
+            vector_class: Type[AnyVec] = Vec3 if is3d else Vec2
             # The start point is the curve offset
-            offset: "AnyVec" = vector_class(defpoints[0])
-            self._offset: "AnyVec" = offset
+            offset: AnyVec = vector_class(defpoints[0])
+            self._offset: AnyVec = offset
             # moving the curve to the origin reduces floating point errors:
-            self._control_points: Sequence["AnyVec"] = tuple(
+            self._control_points: Sequence[AnyVec] = tuple(
                 vector_class(p) - offset for p in defpoints
             )
         else:
             raise ValueError("Three control points required.")
 
     @property
-    def control_points(self) -> Sequence["AnyVec"]:
+    def control_points(self) -> Sequence[AnyVec]:
         """Control points as tuple of :class:`~ezdxf.math.Vec3` or
         :class:`~ezdxf.math.Vec2` objects.
         """
         # ezdxf optimization: p0 is always (0, 0, 0)
         p0, p1, p2 = self._control_points
         offset = self._offset
         return offset, p1 + offset, p2 + offset
 
-    def tangent(self, t: float) -> "AnyVec":
+    def tangent(self, t: float) -> AnyVec:
         """Returns direction vector of tangent for location `t` at the
         Bèzier-curve.
 
         Args:
             t: curve position in the range ``[0, 1]``
 
         """
         check_if_in_valid_range(t)
         return self._get_curve_tangent(t)
 
-    def point(self, t: float) -> "AnyVec":
+    def point(self, t: float) -> AnyVec:
         """Returns point for location `t`` at the Bèzier-curve.
 
         Args:
             t: curve position in the range ``[0, 1]``
 
         """
         check_if_in_valid_range(t)
         return self._get_curve_point(t)
 
-    def approximate(self, segments: int) -> Iterable["AnyVec"]:
+    def approximate(self, segments: int) -> Iterator[AnyVec]:
         """Approximate `Bézier curve`_ by vertices, yields `segments` + 1
         vertices as ``(x, y[, z])`` tuples.
 
         Args:
             segments: count of segments for approximation
 
         """
@@ -99,105 +99,105 @@
         yield cp[2]
 
     def approximated_length(self, segments: int = 128) -> float:
         """Returns estimated length of Bèzier-curve as approximation by line
         `segments`.
         """
         length: float = 0.0
-        prev_point: Optional["AnyVec"] = None
+        prev_point: Optional[AnyVec] = None
         for point in self.approximate(segments):
             if prev_point is not None:
                 length += prev_point.distance(point)
             prev_point = point
         return length
 
     def flattening(
         self, distance: float, segments: int = 4
-    ) -> Iterable["AnyVec"]:
+    ) -> Iterator[AnyVec]:
         """Adaptive recursive flattening. The argument `segments` is the
         minimum count of approximation segments, if the distance from the center
         of the approximation segment to the curve is bigger than `distance` the
         segment will be subdivided.
 
         Args:
             distance: maximum distance from the center of the quadratic (C2)
                 curve to the center of the linear (C1) curve between two
                 approximation points to determine if a segment should be
                 subdivided.
             segments: minimum segment count
 
         """
         def subdiv(
-            start_point: "AnyVec",
-            end_point: "AnyVec",
+            start_point: AnyVec,
+            end_point: AnyVec,
             start_t: float,
             end_t: float,
-        ) -> Iterable["AnyVec"]:
+        ) -> Iterator[AnyVec]:
             mid_t: float = (start_t + end_t) * 0.5
-            mid_point: "AnyVec" = self._get_curve_point(mid_t)
-            chk_point: "AnyVec" = start_point.lerp(end_point)
-            # center point point is faster than projecting mid point onto
+            mid_point: AnyVec = self._get_curve_point(mid_t)
+            chk_point: AnyVec = start_point.lerp(end_point)
+            # center point is faster than projecting mid-point onto
             # vector start -> end:
             d = chk_point.distance(mid_point)
             if d < distance:
                 yield end_point
             else:
                 yield from subdiv(start_point, mid_point, start_t, mid_t)
                 yield from subdiv(mid_point, end_point, mid_t, end_t)
 
         dt: float = 1.0 / segments
         t0: float = 0.0
         t1: float
         cp = self.control_points
-        start_point: "AnyVec" = cp[0]
-        end_point: "AnyVec"
+        start_point: AnyVec = cp[0]
+        end_point: AnyVec
         yield start_point
         while t0 < 1.0:
             t1 = t0 + dt
             if math.isclose(t1, 1.0):
                 end_point = cp[2]
                 t1 = 1.0
             else:
                 end_point = self._get_curve_point(t1)
             yield from subdiv(start_point, end_point, t0, t1)
             t0 = t1
             start_point = end_point
 
-    def _get_curve_point(self, t: float) -> "AnyVec":
+    def _get_curve_point(self, t: float) -> AnyVec:
         # 1st control point (p0) is always (0, 0, 0)
         # => p0 * a is always (0, 0, 0)
         p0, p1, p2 = self._control_points
         _1_minus_t = 1.0 - t
         # a = _1_minus_t * _1_minus_t
         b = 2.0 * t * _1_minus_t
         c = t * t
         # add offset at last - it is maybe very large
         return p1 * b + p2 * c + self._offset
 
-    def _get_curve_tangent(self, t: float) -> "AnyVec":
+    def _get_curve_tangent(self, t: float) -> AnyVec:
         # tangent vector is independent from offset location!
         # 1st control point (p0) is always (0, 0, 0)
         # => p0 * a is always (0, 0, 0)
         p0, p1, p2 = self._control_points
         # a = -2.0 * (1.0 - t)
         b = 2.0 - 4.0 * t
         c = 2.0 * t
         return p1 * b + p2 * c
 
-    def reverse(self) -> "Bezier3P":
+    def reverse(self) -> Bezier3P:
         """Returns a new Bèzier-curve with reversed control point order."""
         return Bezier3P(list(reversed(self.control_points)))
 
-    def transform(self, m: Matrix44) -> "Bezier3P":
+    def transform(self, m: Matrix44) -> Bezier3P:
         """General transformation interface, returns a new :class:`Bezier3P`
         curve and it is always a 3D curve.
 
         Args:
              m: 4x4 transformation matrix (:class:`ezdxf.math.Matrix44`)
 
         """
-        defpoints: Iterable["AnyVec"]
+        defpoints: Iterable[AnyVec]
         if len(self._offset) == 2:
             defpoints = Vec3.generate(self.control_points)
         else:
             defpoints = self.control_points
         return Bezier3P(tuple(m.transform_vertices(defpoints)))
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/_bezier4p.py` & `ezdxf-1.1.0b0/src/ezdxf/math/_bezier4p.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) 2010-2022 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
-from typing import TYPE_CHECKING, Iterable, Union, Sequence, Type
+from typing import TYPE_CHECKING, Iterable, Iterator, Union, Sequence, Type
 import math
 from functools import lru_cache
 
 # The pure Python implementation can't import from ._ctypes or ezdxf.math!
 from ._vector import Vec3, Vec2
 from ._matrix44 import Matrix44
 from ._construct import arc_angle_span_deg
@@ -113,15 +113,15 @@
             t: curve position in the range ``[0, 1]``
 
         """
         if not (0 <= t <= 1.0):
             raise ValueError("t not in range [0 to 1]")
         return self._get_curve_point(t)
 
-    def approximate(self, segments: int) -> Iterable[AnyVec]:
+    def approximate(self, segments: int) -> Iterator[AnyVec]:
         """Approximate `Bézier curve`_ by vertices, yields `segments` + 1
         vertices as ``(x, y[, z])`` tuples.
 
         Args:
             segments: count of segments for approximation
 
         """
@@ -132,15 +132,15 @@
         yield cp[0]
         for segment in range(1, segments):
             yield self._get_curve_point(delta_t * segment)
         yield cp[3]
 
     def flattening(
         self, distance: float, segments: int = 4
-    ) -> Iterable[Union[Vec3, Vec2]]:
+    ) -> Iterator[Union[Vec3, Vec2]]:
         """Adaptive recursive flattening. The argument `segments` is the
         minimum count of approximation segments, if the distance from the center
         of the approximation segment to the curve is bigger than `distance` the
         segment will be subdivided.
 
         Args:
             distance: maximum distance from the center of the cubic (C3)
@@ -152,20 +152,20 @@
         """
 
         def subdiv(
             start_point: AnyVec,
             end_point: AnyVec,
             start_t: float,
             end_t: float,
-        ) -> Iterable[AnyVec]:
+        ) -> Iterator[AnyVec]:
             mid_t: float = (start_t + end_t) * 0.5
             mid_point: AnyVec = self._get_curve_point(mid_t)
             chk_point: AnyVec = start_point.lerp(end_point)
-            # center point point is faster than projecting mid point onto
-            # vector start -> end:
+            # center point is faster than projecting the mid-point on
+            # the vector start -> end:
             d = chk_point.distance(mid_point)
             if d < distance:
                 yield end_point
             else:
                 yield from subdiv(start_point, mid_point, start_t, mid_t)
                 yield from subdiv(mid_point, end_point, mid_t, end_t)
 
@@ -238,15 +238,15 @@
 
 def cubic_bezier_from_arc(
     center: UVec = (0, 0, 0),
     radius: float = 1,
     start_angle: float = 0,
     end_angle: float = 360,
     segments: int = 1,
-) -> Iterable[Bezier4P]:
+) -> Iterator[Bezier4P]:
     """Returns an approximation for a circular 2D arc by multiple cubic
     Bézier-curves.
 
     Args:
         center: circle center as :class:`Vec3` compatible object
         radius: circle radius
         start_angle: start angle in degrees
@@ -275,15 +275,15 @@
 
 
 PI_2: float = math.pi / 2.0
 
 
 def cubic_bezier_from_ellipse(
     ellipse: "ConstructionEllipse", segments: int = 1
-) -> Iterable[Bezier4P]:
+) -> Iterator[Bezier4P]:
     """Returns an approximation for an elliptic arc by multiple cubic
     Bézier-curves.
 
     Args:
         ellipse: ellipse parameters as :class:`~ezdxf.math.ConstructionEllipse`
             object
         segments: count of Bèzier-curve segments, at least one segment for each
@@ -294,15 +294,15 @@
     if abs(param_span) < 1e-9:
         return
     start_angle: float = ellipse.start_param % math.tau
     end_angle: float = start_angle + param_span
     while start_angle > end_angle:
         end_angle += math.tau
 
-    def transform(points: Iterable[Vec3]) -> Iterable[Vec3]:
+    def transform(points: Iterable[Vec3]) -> Iterator[Vec3]:
         center = Vec3(ellipse.center)
         x_axis: Vec3 = ellipse.major_axis
         y_axis: Vec3 = ellipse.minor_axis
         for p in points:
             yield center + x_axis * p.x + y_axis * p.y
 
     for defpoints in cubic_bezier_arc_parameters(
@@ -321,15 +321,15 @@
 # Not sure if this is the correct way to apply this optimization,
 # so i stick to the original version for now:
 TANGENT_FACTOR = DEFAULT_TANGENT_FACTOR
 
 
 def cubic_bezier_arc_parameters(
     start_angle: float, end_angle: float, segments: int = 1
-) -> Iterable[tuple[Vec3, Vec3, Vec3, Vec3]]:
+) -> Iterator[tuple[Vec3, Vec3, Vec3, Vec3]]:
     """Yields cubic Bézier-curve parameters for a circular 2D arc with center
     at (0, 0) and a radius of 1 in the form of [start point, 1. control point,
     2. control point, end point].
 
     Args:
         start_angle: start angle in radians
         end_angle: end angle in radians (end_angle > start_angle!)
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/_bspline.py` & `ezdxf-1.1.0b0/src/ezdxf/math/_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/_construct.py` & `ezdxf-1.1.0b0/src/ezdxf/math/_construct.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/_ctypes.py` & `ezdxf-1.1.0b0/src/ezdxf/math/_ctypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/_mapbox_earcut.py` & `ezdxf-1.1.0b0/src/ezdxf/math/_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/_matrix44.py` & `ezdxf-1.1.0b0/src/ezdxf/math/_matrix44.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # original code from package: gameobjects
 # Home-page: http://code.google.com/p/gameobjects/
 # Author: Will McGugan
 # Download-URL: http://code.google.com/p/gameobjects/downloads/list
-# Copyright (c) 2011-2022 Manfred Moitzi
+# Copyright (c) 2011-2023 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import Sequence, Iterable, Iterator, TYPE_CHECKING, Optional
 import math
 from math import sin, cos, tan
 from itertools import chain
 
 # The pure Python implementation can't import from ._ctypes or ezdxf.math!
-from ._vector import Vec3, X_AXIS, Y_AXIS, Z_AXIS, NULLVEC
+from ._vector import Vec3, X_AXIS, Y_AXIS, Z_AXIS, NULLVEC, Vec2
 
 if TYPE_CHECKING:
     from ezdxf.math import UVec
 
 __all__ = ["Matrix44"]
 
 
@@ -64,15 +64,15 @@
         Matrix44(values) values is an iterable with the 16 components of the matrix.
 
         Matrix44(row1, row2, row3, row4) four rows, each row with four values.
 
         """
         nargs = len(args)
         if nargs == 0:
-            self._matrix = floats(Matrix44._identity)
+            self._matrix = list(Matrix44._identity)
         elif nargs == 1:
             self._matrix = floats(args[0])
         elif nargs == 4:
             self._matrix = floats(chain(*args))
         else:
             raise ValueError(
                 "Invalid count of arguments (4 row vectors or one "
@@ -85,28 +85,46 @@
         """Returns the representation string of the matrix:
         ``Matrix44((col0, col1, col2, col3), (...), (...), (...))``
         """
 
         def format_row(row):
             return "(%s)" % ", ".join(str(value) for value in row)
 
-        return "Matrix44(%s)" % ", ".join(
-            format_row(row) for row in self.rows()
-        )
+        return "Matrix44(%s)" % ", ".join(format_row(row) for row in self.rows())
 
     def get_2d_transformation(self) -> tuple[float, ...]:
         """Returns a 2D transformation as a row-major matrix in a linear
         array (tuple).
 
         A more correct transformation could be implemented like so:
         https://stackoverflow.com/questions/10629737/convert-3d-4x4-rotation-matrix-into-2d
         """
         m = self._matrix
         return m[0], m[1], 0.0, m[4], m[5], 0.0, m[12], m[13], 1.0
 
+    @staticmethod
+    def from_2d_transformation(components: Sequence[float]) -> Matrix44:
+        """Returns the :class:`Matrix44` class for an affine 2D (3x3) transformation
+        matrix defined by 6 float values: m11, m12, m21, m22, m31, m32.
+        """
+        if len(components) != 6:
+            raise ValueError(
+                "First 2 columns of a 3x3 matrix required: m11, m12, m21, m22, m31, m32"
+            )
+
+        m44 = Matrix44()
+        m = m44._matrix
+        m[0] = components[0]
+        m[1] = components[1]
+        m[4] = components[2]
+        m[5] = components[3]
+        m[12] = components[4]
+        m[13] = components[5]
+        return m44
+
     def get_row(self, row: int) -> tuple[float, ...]:
         """Get row as list of four float values.
 
         Args:
             row: row index [0 .. 3]
 
         """
@@ -322,17 +340,15 @@
             x * y * omc - z * s, y * y * omc + c, y * z * omc + x * s, 0.,
             x * z * omc + y * s, y * z * omc - x * s, z * z * omc + c, 0.,
             0., 0., 0., 1.
         ])
         # fmt: on
 
     @classmethod
-    def xyz_rotate(
-        cls, angle_x: float, angle_y: float, angle_z: float
-    ) -> Matrix44:
+    def xyz_rotate(cls, angle_x: float, angle_y: float, angle_z: float) -> Matrix44:
         """Returns a rotation matrix for rotation about each axis.
 
         Args:
             angle_x: rotation angle about x-axis in radians
             angle_y: rotation angle about y-axis in radians
             angle_z: rotation angle about z-axis in radians
 
@@ -528,19 +544,19 @@
             m1[12] * m2[1] + m1[13] * m2[5] + m1[14] * m2[9] + m1[15] * m2[13],
             m1[12] * m2[2] + m1[13] * m2[6] + m1[14] * m2[10] + m1[15] * m2[14],
             m1[12] * m2[3] + m1[13] * m2[7] + m1[14] * m2[11] + m1[15] * m2[15]
         ]
         # fmt: on
         return self
 
-    def rows(self) -> Iterable[tuple[float, ...]]:
+    def rows(self) -> Iterator[tuple[float, ...]]:
         """Iterate over rows as 4-tuples."""
         return (self.get_row(index) for index in (0, 1, 2, 3))
 
-    def columns(self) -> Iterable[tuple[float, ...]]:
+    def columns(self) -> Iterator[tuple[float, ...]]:
         """Iterate over columns as 4-tuples."""
         return (self.get_col(index) for index in (0, 1, 2, 3))
 
     def transform(self, vector: UVec) -> Vec3:
         """Returns a transformed vertex."""
         m = self._matrix
         x, y, z = Vec3(vector)
@@ -563,15 +579,15 @@
             x * m[2] + y * m[6] + z * m[10]
         )
         # fmt: on
         return v.normalize() if normalize else v
 
     ocs_to_wcs = transform_direction
 
-    def transform_vertices(self, vectors: Iterable[UVec]) -> Iterable[Vec3]:
+    def transform_vertices(self, vectors: Iterable[UVec]) -> Iterator[Vec3]:
         """Returns an iterable of transformed vertices."""
         # fmt: off
         (
             m0, m1, m2, m3,
             m4, m5, m6, m7,
             m8, m9, m10, m11,
             m12, m13, m14, m15,
@@ -583,17 +599,47 @@
             yield Vec3(
                 x * m0 + y * m4 + z * m8 + m12,
                 x * m1 + y * m5 + z * m9 + m13,
                 x * m2 + y * m6 + z * m10 + m14
             )
             # fmt: on
 
+    def fast_2d_transform(self, points: Iterable[UVec]) -> Iterator[Vec2]:
+        """Fast transformation of 2D points. For 3D input points the z-axis will be
+        ignored.  This only works reliable if only 2D transformations have been applied
+        to the 4x4 matrix!
+
+        Profiling results - speed gains over :meth:`transform_vertices`:
+
+            - pure Python code: ~1.6x
+            - Python with C-extensions: less than 1.1x
+            - PyPy 3.8: ~4.3x
+
+        But speed isn't everything, returning the processed input points as :class:`Vec2`
+        instances is another advantage.
+
+        .. versionadded:: 1.0.4
+
+        """
+        m = self._matrix
+        m0 = m[0]
+        m1 = m[1]
+        m4 = m[4]
+        m5 = m[5]
+        m12 = m[12]
+        m13 = m[13]
+        for pnt in points:
+            v = Vec2(pnt)
+            x = v.x
+            y = v.y
+            yield Vec2(x * m0 + y * m4 + m12, x * m1 + y * m5 + m13)
+
     def transform_directions(
         self, vectors: Iterable[UVec], normalize=False
-    ) -> Iterable[Vec3]:
+    ) -> Iterator[Vec3]:
         """Returns an iterable of transformed direction vectors without
         translation.
 
         """
         m0, m1, m2, m3, m4, m5, m6, m7, m8, m9, m10, *_ = self._matrix
         for vector in vectors:
             x, y, z = Vec3(vector)
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/_vector.py` & `ezdxf-1.1.0b0/src/ezdxf/math/_vector.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/math/__init__.py` & `ezdxf-1.1.0b0/src/ezdxf/math/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/path/commands.py` & `ezdxf-1.1.0b0/src/ezdxf/path/commands.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) 2021-2022, Manfred Moitzi
 # License: MIT License
+from __future__ import annotations
 import enum
 from typing import NamedTuple, Union
 
-from ezdxf.math import Vec3
+from ezdxf.math import Vec2, Vec3
 
 __all__ = [
     "Command",
     "AnyCurve",
     "PathElement",
     "LineTo",
     "Curve3To",
@@ -21,42 +22,42 @@
     LINE_TO = 1  # (LINE_TO, end vertex)
     CURVE3_TO = 2  # (CURVE3_TO, end vertex, ctrl) quadratic bezier
     CURVE4_TO = 3  # (CURVE4_TO, end vertex, ctrl1, ctrl2) cubic bezier
     MOVE_TO = 4  # (MOVE_TO, end vertex), creates a gap and starts a sub-path
 
 
 class LineTo(NamedTuple):
-    end: Vec3
+    end: Vec2|Vec3
 
     @property
     def type(self):
         return Command.LINE_TO
 
 
 class MoveTo(NamedTuple):
-    end: Vec3
+    end: Vec2|Vec3
 
     @property
     def type(self):
         return Command.MOVE_TO
 
 
 class Curve3To(NamedTuple):
-    end: Vec3
-    ctrl: Vec3
+    end: Vec2|Vec3
+    ctrl: Vec2|Vec3
 
     @property
     def type(self):
         return Command.CURVE3_TO
 
 
 class Curve4To(NamedTuple):
-    end: Vec3
-    ctrl1: Vec3
-    ctrl2: Vec3
+    end: Vec2|Vec3
+    ctrl1: Vec2|Vec3
+    ctrl2: Vec2|Vec3
 
     @property
     def type(self):
         return Command.CURVE4_TO
 
 
 AnyCurve = (Command.CURVE3_TO, Command.CURVE4_TO)
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/path/converter.py` & `ezdxf-1.1.0b0/src/ezdxf/path/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     EdgePath,
     LineEdge,
     ArcEdge,
     EllipseEdge,
     SplineEdge,
 )
 from ezdxf.entities.polygon import DXFPolygon
-from .path import Path
+from .path import Path, AbstractPath, Path2d
 from .commands import Command
 from . import tools
 from .nesting import group_paths
 
 __all__ = [
     "make_path",
     "to_lines",
@@ -498,124 +498,122 @@
             path.line_to(vertex)
     if close:
         path.close()
     return path
 
 
 def to_lwpolylines(
-    paths: Iterable[Path],
+    paths: Iterable[Path | Path2d],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> Iterator[LWPolyline]:
     """Convert the given `paths` into :class:`~ezdxf.entities.LWPolyline`
     entities.
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector. The default extrusion vector
     is the WCS z-axis. The plane elevation is the distance from the WCS origin
     to the start point of the first path.
 
     Args:
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve
         extrusion: extrusion vector for all paths
         dxfattribs: additional DXF attribs
 
     Returns:
         iterable of :class:`~ezdxf.entities.LWPolyline` objects
 
     """
-    if isinstance(paths, Path):
+    if isinstance(paths, AbstractPath):
         paths = [paths]
     else:
         paths = list(paths)
     if len(paths) == 0:
         return []
-
     extrusion = Vec3(extrusion)
-    reference_point = paths[0].start
+    reference_point = Vec3(paths[0].start)
     dxfattribs = dict(dxfattribs or {})
     if not Z_AXIS.isclose(extrusion):
         ocs, elevation = _get_ocs(extrusion, reference_point)
         paths = tools.transform_paths_to_ocs(paths, ocs)
         dxfattribs["elevation"] = elevation
         dxfattribs["extrusion"] = extrusion
     elif reference_point.z != 0:
         dxfattribs["elevation"] = reference_point.z
 
-    for path in tools.single_paths(paths):
+    for path in tools.single_paths(paths):  # type: ignore
         if len(path) > 0:
             p = LWPolyline.new(dxfattribs=dxfattribs)
             p.append_points(path.flattening(distance, segments), format="xy")  # type: ignore
             yield p
 
 
 def _get_ocs(extrusion: Vec3, reference_point: Vec3) -> tuple[OCS, float]:
     ocs = OCS(extrusion)
     elevation = ocs.from_wcs(reference_point).z  # type: ignore
     return ocs, elevation
 
 
 def to_polylines2d(
-    paths: Iterable[Path],
+    paths: Iterable[Path | Path2d],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> Iterator[Polyline]:
     """Convert the given `paths` into 2D :class:`~ezdxf.entities.Polyline`
     entities.
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector. The default extrusion vector
     is the WCS z-axis. The plane elevation is the distance from the WCS origin
     to the start point of the first path.
 
     Args:
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve
         extrusion: extrusion vector for all paths
         dxfattribs: additional DXF attribs
 
     Returns:
         iterable of 2D :class:`~ezdxf.entities.Polyline` objects
 
     """
-    if isinstance(paths, Path):
+    if isinstance(paths, AbstractPath):
         paths = [paths]
     else:
         paths = list(paths)
     if len(paths) == 0:
         return []
-
     extrusion = Vec3(extrusion)
-    reference_point = paths[0].start
+    reference_point = Vec3(paths[0].start)
     dxfattribs = dict(dxfattribs or {})
     if not Z_AXIS.isclose(extrusion):
         ocs, elevation = _get_ocs(extrusion, reference_point)
         paths = tools.transform_paths_to_ocs(paths, ocs)
         dxfattribs["elevation"] = Vec3(0, 0, elevation)
         dxfattribs["extrusion"] = extrusion
     elif reference_point.z != 0:
         dxfattribs["elevation"] = Vec3(0, 0, reference_point.z)
 
-    for path in tools.single_paths(paths):
+    for path in tools.single_paths(paths):  # type: ignore
         if len(path) > 0:
             p = Polyline.new(dxfattribs=dxfattribs)
             p.append_vertices(path.flattening(distance, segments))
             p.new_seqend()
             yield p
 
 
 def to_hatches(
-    paths: Iterable[Path],
+    paths: Iterable[Path | Path2d],
     *,
     edge_path: bool = True,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     g1_tol: float = G1_TOL,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
@@ -625,15 +623,15 @@
     of LINE and SPLINE edges, as boundary paths for boundaries including curves.
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector. The default extrusion vector
     is the WCS z-axis. The plane elevation is the distance from the WCS origin
     to the start point of the first path.
 
     Args:
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d` objects
         edge_path: ``True`` for edge paths build of LINE and SPLINE edges,
             ``False`` for only LWPOLYLINE paths as boundary paths
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve to flatten LWPOLYLINE paths
         g1_tol: tolerance for G1 continuity check to separate SPLINE edges
         extrusion: extrusion vector to all paths
         dxfattribs: additional DXF attribs
@@ -650,19 +648,21 @@
         )
     else:
         # noinspection PyTypeChecker
         boundary_factory = partial(
             build_poly_path, distance=distance, segments=segments
         )
 
-    yield from _polygon_converter(Hatch, paths, boundary_factory, extrusion, dxfattribs)
+    yield from _polygon_converter(
+        Hatch, tools.to_3d_paths(paths), boundary_factory, extrusion, dxfattribs
+    )
 
 
 def to_mpolygons(
-    paths: Iterable[Path],
+    paths: Iterable[Path | Path2d],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> Iterator[MPolygon]:
     """Convert the given `paths` into :class:`~ezdxf.entities.MPolygon` entities.
@@ -671,15 +671,15 @@
 
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector. The default extrusion vector
     is the WCS z-axis. The plane elevation is the distance from the WCS origin
     to the start point of the first path.
 
     Args:
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve to flatten LWPOLYLINE paths
         extrusion: extrusion vector to all paths
         dxfattribs: additional DXF attribs
 
     Returns:
         iterable of :class:`~ezdxf.entities.MPolygon` objects
@@ -689,15 +689,15 @@
     boundary_factory: BoundaryFactory = partial(
         build_poly_path, distance=distance, segments=segments
     )
     dxfattribs = dict(dxfattribs or {})
     dxfattribs.setdefault("fill_color", const.BYLAYER)  # type: ignore
 
     yield from _polygon_converter(
-        MPolygon, paths, boundary_factory, extrusion, dxfattribs
+        MPolygon, tools.to_3d_paths(paths), boundary_factory, extrusion, dxfattribs
     )
 
 
 def build_edge_path(
     boundaries: BoundaryPaths,
     path: Path,
     flags: int,
@@ -742,15 +742,15 @@
 def _polygon_converter(
     cls: Type[TPolygon],
     paths: Iterable[Path],
     add_boundary: BoundaryFactory,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> Iterator[TPolygon]:
-    if isinstance(paths, Path):
+    if isinstance(paths, AbstractPath):
         paths = [paths]
     else:
         paths = list(paths)
     if len(paths) == 0:
         return []
 
     extrusion = Vec3(extrusion)
@@ -770,78 +770,78 @@
     for group in group_paths(tools.single_paths(paths)):
         if len(group) == 0:
             continue
         polygon = cls.new(dxfattribs=_dxfattribs)
         boundaries = polygon.paths
         external = group[0]
         external.close()
-        add_boundary(boundaries, external, 1)
+        add_boundary(boundaries, external, 1)  # type: ignore
         for hole in group[1:]:
             hole.close()
-            add_boundary(boundaries, hole, 0)
+            add_boundary(boundaries, hole, 0)  # type: ignore
         yield polygon
 
 
 def to_polylines3d(
-    paths: Iterable[Path],
+    paths: Iterable[Path | Path2d],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     dxfattribs=None,
 ) -> Iterator[Polyline]:
     """Convert the given `paths` into 3D :class:`~ezdxf.entities.Polyline`
     entities.
 
     Args:
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve
         dxfattribs: additional DXF attribs
 
     Returns:
         iterable of 3D :class:`~ezdxf.entities.Polyline` objects
 
     """
-    if isinstance(paths, Path):
+    if isinstance(paths, AbstractPath):
         paths = [paths]
 
     dxfattribs = dict(dxfattribs or {})
     dxfattribs["flags"] = const.POLYLINE_3D_POLYLINE
-    for path in tools.single_paths(paths):
+    for path in tools.single_paths(paths):  # type: ignore
         if len(path) > 0:
             p = Polyline.new(dxfattribs=dxfattribs)
             p.append_vertices(path.flattening(distance, segments))
             p.new_seqend()
             yield p
 
 
 def to_lines(
-    paths: Iterable[Path],
+    paths: Iterable[Path | Path2d],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     dxfattribs=None,
 ) -> Iterator[Line]:
     """Convert the given `paths` into :class:`~ezdxf.entities.Line` entities.
 
     Args:
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve
         dxfattribs: additional DXF attribs
 
     Returns:
         iterable of :class:`~ezdxf.entities.Line` objects
 
     """
-    if isinstance(paths, Path):
+    if isinstance(paths, AbstractPath):
         paths = [paths]
     dxfattribs = dict(dxfattribs or {})
     prev_vertex = None
-    for path in tools.single_paths(paths):
+    for path in tools.single_paths(paths):  # type: ignore
         if len(path) == 0:
             continue
         for vertex in path.flattening(distance, segments):
             if prev_vertex is None:
                 prev_vertex = vertex
                 continue
             dxfattribs["start"] = prev_vertex
@@ -850,21 +850,23 @@
             prev_vertex = vertex
         prev_vertex = None
 
 
 PathParts: TypeAlias = Union[BSpline, List[Vec3]]
 
 
-def to_bsplines_and_vertices(path: Path, g1_tol: float = G1_TOL) -> Iterator[PathParts]:
+def to_bsplines_and_vertices(
+    path: Path | Path2d, g1_tol: float = G1_TOL
+) -> Iterator[PathParts]:
     """Convert a :class:`Path` object into multiple cubic B-splines and
     polylines as lists of vertices. Breaks adjacent Bèzier without G1
     continuity into separated B-splines.
 
     Args:
-        path: :class:`Path` objects
+        path: :class:`Path` or :class:`Path2d` objects
         g1_tol: tolerance for G1 continuity check
 
     Returns:
         :class:`~ezdxf.math.BSpline` and lists of :class:`~ezdxf.math.Vec3`
 
     """
     from ezdxf.math import bezier_to_bspline
@@ -886,15 +888,15 @@
                 _g1_continuity_curves = [b2]
             b1 = b2
 
         if _g1_continuity_curves:
             yield bezier_to_bspline(_g1_continuity_curves)
 
     curves = []
-    for path in tools.single_paths([path]):
+    for path in tools.single_paths([path]):  # type: ignore
         prev = path.start
         for cmd in path:
             if cmd.type == Command.CURVE3_TO:
                 curve = Bezier3P([prev, cmd.ctrl, cmd.end])  # type: ignore
             elif cmd.type == Command.CURVE4_TO:
                 curve = Bezier4P([prev, cmd.ctrl1, cmd.ctrl2, cmd.end])  # type: ignore
             elif cmd.type == Command.LINE_TO:
@@ -921,15 +923,15 @@
     if bezier:
         yield from to_bspline()
     if polyline:
         yield to_vertices()
 
 
 def to_splines_and_polylines(
-    paths: Iterable[Path],
+    paths: Iterable[Path | Path2d],
     *,
     g1_tol: float = G1_TOL,
     dxfattribs=None,
 ) -> Iterator[Union[Spline, Polyline]]:
     """Convert the given `paths` into :class:`~ezdxf.entities.Spline` and 3D
     :class:`~ezdxf.entities.Polyline` entities.
 
@@ -938,19 +940,19 @@
         g1_tol: tolerance for G1 continuity check
         dxfattribs: additional DXF attribs
 
     Returns:
         iterable of :class:`~ezdxf.entities.Line` objects
 
     """
-    if isinstance(paths, Path):
+    if isinstance(paths, AbstractPath):
         paths = [paths]
     dxfattribs = dict(dxfattribs or {})
 
-    for path in tools.single_paths(paths):
+    for path in tools.single_paths(paths):  # type: ignore
         for data in to_bsplines_and_vertices(path, g1_tol):
             if isinstance(data, BSpline):
                 spline = Spline.new(dxfattribs=dxfattribs)
                 spline.apply_construction_tool(data)
                 yield spline
             else:
                 attribs = dict(dxfattribs)
@@ -970,14 +972,15 @@
     CURVE3 = 3
     CURVE4 = 4
     LINETO = 2
     MOVETO = 1
     STOP = 0
 
 
+# TODO: return Path2d
 def multi_path_from_matplotlib_path(mpath, curves=True) -> Path:
     """Returns a :class:`Path` object from a Matplotlib `Path`_
     (`TextPath`_)  object. (requires Matplotlib). Returns a multi-path object
     if necessary.
 
     .. _TextPath: https://matplotlib.org/3.1.1/api/textpath_api.html
     .. _Path: https://matplotlib.org/3.1.1/api/path_api.html#matplotlib.path.Path
@@ -1005,14 +1008,15 @@
             if not path.end.isclose(current_polyline_start):
                 path.line_to(current_polyline_start)
         elif cmd == MplCmd.STOP:  # not used
             pass
     return path
 
 
+# TODO: not used in ezdxf, remove?
 def from_matplotlib_path(mpath, curves=True) -> Iterator[Path]:
     """Yields multiple :class:`Path` objects from a Matplotlib `Path`_
     (`TextPath`_)  object. (requires Matplotlib)
 
     .. _TextPath: https://matplotlib.org/3.1.1/api/textpath_api.html
     .. _Path: https://matplotlib.org/3.1.1/api/path_api.html#matplotlib.path.Path
 
@@ -1020,40 +1024,40 @@
     path = multi_path_from_matplotlib_path(mpath, curves=curves)
     if path.has_sub_paths:
         return path.sub_paths()
     else:
         return iter([path])
 
 
-def to_matplotlib_path(paths: Iterable[Path], extrusion: UVec = Z_AXIS):
-    """Convert the given `paths` into a single :class:`matplotlib.path.Path`
-    object.
+def to_matplotlib_path(paths: Iterable[Path | Path2d], extrusion: UVec = Z_AXIS):
+    """Convert the given `paths` into a single :class:`matplotlib.path.Path` object.
+
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector.The default extrusion vector
     is the WCS z-axis. The Matplotlib :class:`Path` is a 2D object with
     :ref:`OCS` coordinates and the z-elevation is lost. (requires Matplotlib)
 
     Args:
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d` objects
         extrusion: extrusion vector for all paths
 
     Returns:
         matplotlib `Path`_ in OCS!
 
     """
     from matplotlib.path import Path as MatplotlibPath
 
     if not Z_AXIS.isclose(extrusion):
         paths = tools.transform_paths_to_ocs(paths, OCS(extrusion))
     else:
         paths = list(paths)
-    if len(paths) == 0:
+    if len(paths) == 0:  # type: ignore
         raise ValueError("one or more paths required")
 
-    def add_command(code: MplCmd, point: Vec3):
+    def add_command(code: MplCmd, point: Vec2 | Vec3):
         codes.append(code)
         vertices.append((point.x, point.y))
 
     vertices: list[tuple[float, float]] = []
     codes: list[MplCmd] = []
     for path in paths:
         add_command(MplCmd.MOVETO, path.start)
@@ -1074,14 +1078,15 @@
     assert len(vertices) == len(codes)
     return MatplotlibPath(vertices, codes)
 
 
 # Interface to QtGui.QPainterPath
 
 
+# TODO: return Path2d
 def multi_path_from_qpainter_path(qpath) -> Path:
     """Returns a :class:`Path` objects from a `QPainterPath`_.
     Returns a multi-path object if necessary. (requires Qt bindings)
 
     .. _QPainterPath: https://doc.qt.io/qt-5/qpainterpath.html
 
     """
@@ -1107,14 +1112,15 @@
                 path.curve4_to(v, vertices[0], vertices[1])
                 vertices.clear()
             else:
                 vertices.append(v)
     return path
 
 
+# TODO: not used in ezdxf, remove?
 def from_qpainter_path(qpath) -> Iterator[Path]:
     """Yields multiple :class:`Path` objects from a `QPainterPath`_.
     (requires Qt bindings)
 
     .. _QPainterPath: https://doc.qt.io/qt-5/qpainterpath.html
 
     """
@@ -1122,17 +1128,17 @@
     path = multi_path_from_qpainter_path(qpath)
     if path.has_sub_paths:
         return path.sub_paths()
     else:
         return iter([path])
 
 
-def to_qpainter_path(paths: Iterable[Path], extrusion: UVec = Z_AXIS):
-    """Convert the given `paths` into a :class:`QtGui.QPainterPath`
-    object.
+def to_qpainter_path(paths: Iterable[Path | Path2d], extrusion: UVec = Z_AXIS):
+    """Convert the given `paths` into a :class:`QtGui.QPainterPath` object.
+
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector. The default extrusion vector
     is the WCS z-axis. The :class:`QPainterPath` is a 2D object with :ref:`OCS`
     coordinates and the z-elevation is lost. (requires Qt bindings)
 
     Args:
         paths: iterable of :class:`Path` objects
@@ -1144,18 +1150,18 @@
     """
     from ezdxf.addons.xqt import QPainterPath, QPointF
 
     if not Z_AXIS.isclose(extrusion):
         paths = tools.transform_paths_to_ocs(paths, OCS(extrusion))
     else:
         paths = list(paths)
-    if len(paths) == 0:
+    if len(paths) == 0:  # type: ignore
         raise ValueError("one or more paths required")
 
-    def qpnt(v: Vec3):
+    def qpnt(v: Vec2 | Vec3):
         return QPointF(v.x, v.y)
 
     qpath = QPainterPath()
     for path in paths:
         qpath.moveTo(qpnt(path.start))
         for cmd in path.commands():
             if cmd.type == Command.LINE_TO:
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/path/nesting.py` & `ezdxf-1.1.0b0/src/ezdxf/path/nesting.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022, Manfred Moitzi
+# Copyright (c) 2020-2023, Manfred Moitzi
 # License: MIT License
 """
 This module provides "nested Polygon" detection for multiple paths.
 
 Terminology
 -----------
 
@@ -91,30 +91,30 @@
 It is not possible for a path to contain another path with a larger area.
 
 """
 from __future__ import annotations
 from typing import Tuple, Optional, List, Iterable
 from typing_extensions import TypeAlias
 from collections import namedtuple
-from .path import Path
+from .path import AbstractPath
 from ezdxf.math import BoundingBox2d
 
 __all__ = [
     "fast_bbox_detection",
     "winding_deconstruction",
     "group_paths",
     "flatten_polygons",
 ]
 
-Exterior: TypeAlias = Path
+Exterior: TypeAlias = AbstractPath
 Polygon: TypeAlias = Tuple[Exterior, Optional[List["Polygon"]]]
 BoxStruct = namedtuple("BoxStruct", "bbox, path")
 
 
-def fast_bbox_detection(paths: Iterable[Path]) -> list[Polygon]:
+def fast_bbox_detection(paths: Iterable[AbstractPath]) -> list[Polygon]:
     """Create a nested polygon structure from iterable `paths`, using 2D
     bounding boxes as fast detection objects.
 
     """
 
     # Implements fast bounding box construction and fast inside check.
     def area(item: BoxStruct) -> float:
@@ -124,17 +124,17 @@
     def separate(
         exterior: BoundingBox2d, candidates: list[BoxStruct]
     ) -> tuple[list[BoxStruct], list[BoxStruct]]:
         holes: list[BoxStruct] = []
         outside: list[BoxStruct] = []
         for candidate in candidates:
             # Fast inside check:
-            (
-                holes if exterior.inside(candidate.bbox.center) else outside
-            ).append(candidate)
+            (holes if exterior.inside(candidate.bbox.center) else outside).append(
+                candidate
+            )
         return holes, outside
 
     def polygon_structure(outside: list[BoxStruct]) -> list[list]:
         polygons = []
         while outside:
             exterior = outside.pop()  # path with largest area
             # Get holes inside of exterior and returns the remaining paths
@@ -146,17 +146,15 @@
                 # and so on ...
                 holes = polygon_structure(holes)  # type: ignore
             polygons.append([exterior, *holes])
         return polygons
 
     def as_nested_paths(polygons) -> list:
         return [
-            polygon.path
-            if isinstance(polygon, BoxStruct)
-            else as_nested_paths(polygon)
+            polygon.path if isinstance(polygon, BoxStruct) else as_nested_paths(polygon)
             for polygon in polygons
         ]
 
     boxed_paths = [
         # Fast bounding box construction:
         BoxStruct(BoundingBox2d(path.control_vertices()), path)
         for path in paths
@@ -164,44 +162,44 @@
     ]
     boxed_paths.sort(key=area)
     return as_nested_paths(polygon_structure(boxed_paths))
 
 
 def winding_deconstruction(
     polygons: list[Polygon],
-) -> tuple[list[Path], list[Path]]:
+) -> tuple[list[AbstractPath], list[AbstractPath]]:
     """Flatten the nested polygon structure in a tuple of two lists,
     the first list contains the paths which should be counter-clockwise oriented
     and the second list contains the paths which should be clockwise oriented.
 
     The paths are not converted to this orientation.
 
     """
 
     def deconstruct(polygons_, level):
         for polygon in polygons_:
-            if isinstance(polygon, Path):
+            if isinstance(polygon, AbstractPath):
                 # level 0 is the list of polygons
                 # level 1 = ccw, 2 = cw, 3 = ccw, 4 = cw, ...
-                (ccw_paths if (level % 2) else cw_paths).append(polygon)
+                (ccw_paths if (level % 2) else cw_paths).append(polygon)  # type:ignore
             else:
                 deconstruct(polygon, level + 1)
 
-    cw_paths: list[Path] = []
-    ccw_paths: list[Path] = []
+    cw_paths: list[AbstractPath] = []
+    ccw_paths: list[AbstractPath] = []
     deconstruct(polygons, 0)
     return ccw_paths, cw_paths
 
 
-def flatten_polygons(polygons: Polygon) -> Iterable[Path]:
+def flatten_polygons(polygons: Polygon) -> Iterable[AbstractPath]:
     """Yield a flat representation of the given nested polygons."""
     for polygon in polygons:  # type: ignore
-        if isinstance(polygon, Path):
+        if isinstance(polygon, AbstractPath):
             yield polygon
         else:
             yield from flatten_polygons(polygon)  # type: ignore
 
 
-def group_paths(paths: Iterable[Path]) -> list[list[Path]]:
+def group_paths(paths: Iterable[AbstractPath]) -> list[list[AbstractPath]]:
     """Group separated paths and their inner holes as flat lists."""
     polygons = fast_bbox_detection(paths)  # type: ignore
     return [list(flatten_polygons(polygon)) for polygon in polygons]
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/path/path.py` & `ezdxf-1.1.0b0/src/ezdxf/path/path.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-# Copyright (c) 2020-2022, Manfred Moitzi
+# Copyright (c) 2020-2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
+import abc
 from typing import (
-    Iterable,
     Optional,
     Iterator,
-    no_type_check,
     Any,
+    TypeVar,
+    Type,
+    Generic,
+    Callable,
+    Sequence,
 )
+from typing_extensions import Self
 from ezdxf.math import (
     Vec3,
+    Vec2,
     NULLVEC,
     OCS,
     Bezier3P,
     Bezier4P,
     Matrix44,
     has_clockwise_orientation,
     UVec,
@@ -25,82 +31,96 @@
     MoveTo,
     Curve3To,
     Curve4To,
     AnyCurve,
     PathElement,
 )
 
-__all__ = ["Path"]
+__all__ = ["AbstractPath", "Path", "Path2d"]
 
 MAX_DISTANCE = 0.01
 MIN_SEGMENTS = 4
 G1_TOL = 1e-4
 
+T = TypeVar("T", Vec2, Vec3)
 
-class Path:
-    __slots__ = (
-        "_vertices",
-        "_start_index",
-        "_commands",
-        "_has_sub_paths",
-        "_user_data",
-    )
+_slots = ("_vertices", "_start_index", "_commands", "_has_sub_paths", "_user_data")
+
+
+class AbstractPath(Generic[T], abc.ABC):
+    __slots__ = _slots
+    _pnt_class: Type[T]
 
     def __init__(self, start: UVec = NULLVEC):
-        # stores all command vertices in a contiguous list
-        self._vertices: list[Vec3] = [Vec3(start)]
+        # stores all command vertices in a contiguous list:
+        self._vertices: list[T] = [self._pnt_class(start)]
         # start index of each command
         self._start_index: list[int] = []
         self._commands: list[Command] = []
         self._has_sub_paths = False
         self._user_data: Any = None  # should be immutable data!
 
+    @abc.abstractmethod
+    def transform(self, m: Matrix44) -> Self:
+        """Returns a new transformed path.
+
+        Args:
+             m: transformation matrix of type :class:`~ezdxf.math.Matrix44`
+
+        """
+        ...
+
     def __len__(self) -> int:
         """Returns count of path elements."""
         return len(self._commands)
 
     def __getitem__(self, item) -> PathElement:
-        """Returns the path element at given index, slicing is not supported.
-        """
+        """Returns the path element at given index, slicing is not supported."""
         if isinstance(item, slice):
             raise TypeError("slicing not supported")
         cmd = self._commands[item]
         index = self._start_index[item]
         vertices = self._vertices
         if cmd == Command.MOVE_TO:
             return MoveTo(vertices[index])
         if cmd == Command.LINE_TO:
             return LineTo(vertices[index])
         if cmd == Command.CURVE3_TO:  # end, ctrl
             return Curve3To(vertices[index + 1], vertices[index])
         if cmd == Command.CURVE4_TO:
             return Curve4To(  # end, ctrl1, ctrl2
-                vertices[index + 2], vertices[index], vertices[index + 1]
+                vertices[index + 2],
+                vertices[index],
+                vertices[index + 1],
             )
         raise ValueError(f"Invalid command: {cmd}")
 
     def __iter__(self) -> Iterator[PathElement]:
         return (self[i] for i in range(len(self._commands)))
 
     def commands(self) -> list[PathElement]:
         """Returns all path elements as list."""
         return list(self.__iter__())
 
-    def __copy__(self) -> Path:
+    def __copy__(self) -> Self:
         """Returns a new copy of :class:`Path` with shared immutable data."""
-        copy = Path()
-        copy._commands = self._commands.copy()
-        # vertices are immutable - no copying required
+        copy = self.__class__()
+        # vertices itself are immutable - no copying required
         copy._vertices = self._vertices.copy()
-        copy._start_index = self._start_index.copy()
-        copy._has_sub_paths = self._has_sub_paths
-        # copy by reference: user data should be immutable data!
-        copy._user_data = self._user_data
+        self._copy_properties(copy)
         return copy
 
+    def _copy_properties(self, clone: AbstractPath) -> None:
+        assert len(self._vertices) == len(clone._vertices)
+        clone._commands = self._commands.copy()
+        clone._start_index = self._start_index.copy()
+        clone._has_sub_paths = self._has_sub_paths
+        # copy by reference: user data should be immutable data!
+        clone._user_data = self._user_data
+
     clone = __copy__
 
     @property
     def user_data(self) -> Any:
         """Attach arbitrary user data to a :class:`Path` object.
         The user data is copied by reference, no deep copy is applied
         therefore a mutable state is shared between copies.
@@ -108,38 +128,42 @@
         return self._user_data
 
     @user_data.setter
     def user_data(self, data: Any):
         self._user_data = data
 
     @property
-    def start(self) -> Vec3:
+    def start(self) -> T:
         """:class:`Path` start point, resetting the start point of an empty
         path is possible.
         """
         return self._vertices[0]
 
     @start.setter
     def start(self, location: UVec) -> None:
         if self._commands:
             raise ValueError("Requires an empty path.")
         else:
-            self._vertices[0] = Vec3(location)
+            self._vertices[0] = self._pnt_class(location)
 
     @property
-    def end(self) -> Vec3:
+    def end(self) -> T:
         """:class:`Path` end point."""
         return self._vertices[-1]
 
-    def control_vertices(self) -> list[Vec3]:
+    def control_vertices(self) -> list[T]:
         """Yields all path control vertices in consecutive order."""
         if self._commands:
             return list(self._vertices)
         return []
 
+    def command_codes(self) -> list[int]:
+        """Internal API."""
+        return list(self._commands)
+
     @property
     def is_closed(self) -> bool:
         """Returns ``True`` if the start point is close to the end point."""
         vertices = self._vertices
         if len(vertices) > 1:
             return vertices[0].isclose(vertices[-1])
         return False
@@ -188,54 +212,55 @@
         else:
             raise ValueError(f"Invalid command: {t}")
 
     def line_to(self, location: UVec) -> None:
         """Add a line from actual path end point to `location`."""
         self._commands.append(Command.LINE_TO)
         self._start_index.append(len(self._vertices))
-        self._vertices.append(Vec3(location))
+        self._vertices.append(self._pnt_class(location))
 
     def move_to(self, location: UVec) -> None:
         """Start a new sub-path at `location`. This creates a gap between the
         current end-point and the start-point of the new sub-path. This converts
         the instance into a :term:`Multi-Path` object.
 
         If the :meth:`move_to` command is the first command, the start point of
         the path will be reset to `location`.
 
         """
         commands = self._commands
         if not commands:
-            self._vertices[0] = Vec3(location)
+            self._vertices[0] = self._pnt_class(location)
             return
         self._has_sub_paths = True
         if commands[-1] == Command.MOVE_TO:
             # replace last move to command
             commands.pop()
             self._vertices.pop()
             self._start_index.pop()
         commands.append(Command.MOVE_TO)
         self._start_index.append(len(self._vertices))
-        self._vertices.append(Vec3(location))
+        self._vertices.append(self._pnt_class(location))
 
     def curve3_to(self, location: UVec, ctrl: UVec) -> None:
         """Add a quadratic Bèzier-curve from actual path end point to
         `location`, `ctrl` is the control point for the quadratic Bèzier-curve.
         """
         self._commands.append(Command.CURVE3_TO)
         self._start_index.append(len(self._vertices))
-        self._vertices.extend((Vec3(ctrl), Vec3(location)))
+        self._vertices.extend((self._pnt_class(ctrl), self._pnt_class(location)))
 
     def curve4_to(self, location: UVec, ctrl1: UVec, ctrl2: UVec) -> None:
         """Add a cubic Bèzier-curve from actual path end point to `location`,
         `ctrl1` and `ctrl2` are the control points for the cubic Bèzier-curve.
         """
         self._commands.append(Command.CURVE4_TO)
         self._start_index.append(len(self._vertices))
-        self._vertices.extend((Vec3(ctrl1), Vec3(ctrl2), Vec3(location)))
+        pnt = self._pnt_class
+        self._vertices.extend((pnt(ctrl1), pnt(ctrl2), pnt(location)))
 
     def close(self) -> None:
         """Close path by adding a line segment from the end point to the start
         point.
         """
         if not self.is_closed:
             self.line_to(self.start)
@@ -251,26 +276,26 @@
                 start_point is not None
             ), "internal error: required MOVE_TO command not found"
             if not self.end.isclose(start_point):
                 self.line_to(start_point)
         else:
             self.close()
 
-    def _start_of_last_sub_path(self) -> Optional[Vec3]:
+    def _start_of_last_sub_path(self) -> Optional[T]:
         move_to = Command.MOVE_TO
         commands = self._commands
         index = len(commands) - 1
         # The first command at index 0 is never MOVE_TO!
         while index > 0:
             if commands[index] == move_to:
                 return self._vertices[self._start_index[index]]
             index -= 1
         return None
 
-    def reversed(self) -> Path:
+    def reversed(self) -> Self:
         """Returns a new :class:`Path` with reversed segments and control
         vertices.
 
         """
         path = self.clone()
         if not path._commands:
             return path
@@ -301,60 +326,55 @@
             elif cmd == Command.CURVE4_TO:
                 start += 3
             elif cmd == Command.CURVE3_TO:
                 start += 2
             elif cmd == Command.MOVE_TO:
                 start += 1
 
-    def clockwise(self) -> Path:
+    def clockwise(self) -> Self:
         """Returns new :class:`Path` in clockwise orientation.
 
         Raises:
             TypeError: can't detect orientation of a :term:`Multi-Path` object
 
         """
         if self.has_clockwise_orientation():
             return self.clone()
         else:
             return self.reversed()
 
-    def counter_clockwise(self) -> Path:
+    def counter_clockwise(self) -> Self:
         """Returns new :class:`Path` in counter-clockwise orientation.
 
         Raises:
             TypeError: can't detect orientation of a :term:`Multi-Path` object
 
         """
 
         if self.has_clockwise_orientation():
             return self.reversed()
         else:
             return self.clone()
 
-    def approximate(self, segments: int = 20) -> Iterator[Vec3]:
+    @abc.abstractmethod
+    def approximate(self, segments: int = 20) -> Iterator[T]:
         """Approximate path by vertices, `segments` is the count of
         approximation segments for each Bézier curve.
 
         Does not yield any vertices for empty paths, where only a start point
         is present!
 
         Approximation of :term:`Multi-Path` objects is possible, but gaps are
         indistinguishable from line segments.
 
         """
+        ...
 
-        def approx_curve3(s, c, e) -> Iterable[Vec3]:
-            return Bezier3P((s, c, e)).approximate(segments)
-
-        def approx_curve4(s, c1, c2, e) -> Iterable[Vec3]:
-            return Bezier4P((s, c1, c2, e)).approximate(segments)
-
-        yield from self._approximate(approx_curve3, approx_curve4)
-
-    def flattening(self, distance: float, segments: int = 16) -> Iterator[Vec3]:
+    @abc.abstractmethod
+    def flattening(self, distance: float, segments: int = 16) -> Iterator[T]:
         """Approximate path by vertices and use adaptive recursive flattening
         to approximate Bèzier curves. The argument `segments` is the
         minimum count of approximation segments for each curve, if the distance
         from the center of the approximation segment to the curve is bigger than
         `distance` the segment will be subdivided.
 
         Does not yield any vertices for empty paths, where only a start point
@@ -366,74 +386,52 @@
         Args:
             distance: maximum distance from the center of the curve to the
                 center of the line segment between two approximation points to
                 determine if a segment should be subdivided.
             segments: minimum segment count per Bézier curve
 
         """
+        ...
 
-        def approx_curve3(s, c, e) -> Iterable[Vec3]:
-            if distance == 0.0:
-                raise ValueError(f"invalid max distance: {distance}")
-            return Bezier3P((s, c, e)).flattening(distance, segments)
-
-        def approx_curve4(s, c1, c2, e) -> Iterable[Vec3]:
-            if distance == 0.0:
-                raise ValueError(f"invalid max distance: {distance}")
-            return Bezier4P((s, c1, c2, e)).flattening(distance, segments)
-
-        yield from self._approximate(approx_curve3, approx_curve4)
-
-    @no_type_check
-    def _approximate(self, approx_curve3, approx_curve4) -> Iterator[Vec3]:
+    def _approximate(self, curve3: Callable, curve4: Callable) -> Iterator[T]:
         if not self._commands:
             return
 
         start = self._vertices[0]
         yield start
 
-        # localize variables:
-        line_to, curve3_to, curve4_to, move_to = Command
         vertices = self._vertices
         for si, cmd in zip(self._start_index, self._commands):
-            if cmd == line_to or cmd == move_to:
+            if cmd == Command.LINE_TO or cmd == Command.MOVE_TO:
                 end_location = vertices[si]
                 yield end_location
-            elif cmd == curve3_to:
+            elif cmd == Command.CURVE3_TO:
                 ctrl, end_location = vertices[si : si + 2]
-                pts = iter(approx_curve3(start, ctrl, end_location))
+                pts = curve3(start, ctrl, end_location)
                 next(pts)  # skip first vertex
                 yield from pts
-            elif cmd == curve4_to:
+            elif cmd == Command.CURVE4_TO:
                 ctrl1, ctrl2, end_location = vertices[si : si + 3]
-                pts = iter(approx_curve4(start, ctrl1, ctrl2, end_location))
+                pts = curve4(start, ctrl1, ctrl2, end_location)
                 next(pts)  # skip first vertex
                 yield from pts
             else:
                 raise ValueError(f"Invalid command: {cmd}")
             start = end_location
 
-    def transform(self, m: Matrix44) -> Path:
-        """Returns a new transformed path.
-
-        Args:
-             m: transformation matrix of type :class:`~ezdxf.math.Matrix44`
-
-        """
-        new_path = self.clone()
-        new_path._vertices = list(m.transform_vertices(self._vertices))
-        return new_path
-
     def to_wcs(self, ocs: OCS, elevation: float) -> None:
         """Transform path from given `ocs` to WCS coordinates inplace."""
+        # Important: requires a 3D path otherwise would change the type of path
+        if self._pnt_class is not Vec3:
+            raise TypeError("Not supported by 2D paths.")
         self._vertices = list(
             ocs.to_wcs(v.replace(z=elevation)) for v in self._vertices
         )
 
-    def sub_paths(self) -> Iterator[Path]:
+    def sub_paths(self) -> Iterator[Self]:
         """Yield sub-path as :term:`Single-Path` objects.
 
         It is safe to call :meth:`sub_paths` on any path-type:
         :term:`Single-Path`, :term:`Multi-Path` and :term:`Empty-Path`.
 
         """
         path = self.__class__(start=self.start)
@@ -444,33 +442,132 @@
                 yield path
                 path = self.__class__(start=cmd.end)
                 path._user_data = self._user_data
             else:
                 path.append_path_element(cmd)
         yield path
 
-    def extend_multi_path(self, path: Path) -> None:
+    def extend_multi_path(self, path: AbstractPath[T]) -> None:
         """Extend the path by another path. The source path is automatically a
         :term:`Multi-Path` object, even if the previous end point matches the
         start point of the appended path. Ignores paths without any commands
         (empty paths).
 
         """
         if len(path):
             self.move_to(path.start)
             for cmd in path.commands():
                 self.append_path_element(cmd)
 
-    def append_path(self, path: Path) -> None:
+    def append_path(self, path: AbstractPath[T]) -> None:
         """Append another path to this path. Adds a :code:`self.line_to(path.start)`
         if the end of this path != the start of appended path.
 
         """
         if len(path) == 0:
             return  # do not append an empty path
         if self._commands:
             if not self.end.isclose(path.start):
                 self.line_to(path.start)
         else:
             self.start = path.start
         for cmd in path.commands():
             self.append_path_element(cmd)
+
+
+class Path(AbstractPath[Vec3]):
+    __slots__ = _slots
+    _pnt_class = Vec3
+
+    def approximate(self, segments: int = 20) -> Iterator[Vec3]:
+        def curve3(p0: T, p1: T, p2: T) -> Iterator[Vec3]:
+            return iter(Bezier3P((p0, p1, p2)).approximate(segments))
+
+        def curve4(p0: T, p1: T, p2: T, p3: T) -> Iterator[Vec3]:
+            return iter(Bezier4P((p0, p1, p2, p3)).approximate(segments))
+
+        return self._approximate(curve3, curve4)
+
+    def flattening(self, distance: float, segments: int = 16) -> Iterator[Vec3]:
+        def curve3(p0: T, p1: T, p2: T) -> Iterator[Vec3]:
+            if distance == 0.0:
+                raise ValueError(f"invalid max distance: 0.0")
+            return iter(Bezier3P((p0, p1, p2)).flattening(distance, segments))
+
+        def curve4(p0: T, p1: T, p2: T, p3: T) -> Iterator[Vec3]:
+            if distance == 0.0:
+                raise ValueError(f"invalid max distance: 0.0")
+            return iter(Bezier4P((p0, p1, p2, p3)).flattening(distance, segments))
+
+        return self._approximate(curve3, curve4)
+
+    def to_2d_path(self) -> Path2d:
+        """Returns a new 2D path. The conversion is almost as fast as a copy.
+
+        .. versionadded:: 1.1
+
+        """
+        path2d = Path2d()
+        path2d._vertices = Vec2.list(self._vertices)
+        self._copy_properties(path2d)
+        return path2d
+
+    def transform(self, m: Matrix44) -> Self:
+        """Returns a new transformed 3D path.
+
+        Args:
+             m: transformation matrix of type :class:`~ezdxf.math.Matrix44`
+
+        """
+        new_path = self.clone()
+        new_path._vertices = list(m.transform_vertices(self._vertices))
+        return new_path
+
+
+class Path2d(AbstractPath[Vec2]):
+    __slots__ = _slots
+    _pnt_class = Vec2
+
+    def approximate(self, segments: int = 20) -> Iterator[Vec2]:
+        def curve3(p0: T, p1: T, p2: T) -> Iterator[Vec2]:
+            return Vec2.generate(Bezier3P((p0, p1, p2)).approximate(segments))
+
+        def curve4(p0: T, p1: T, p2: T, p3: T) -> Iterator[Vec2]:
+            return Vec2.generate(Bezier4P((p0, p1, p2, p3)).approximate(segments))
+
+        return self._approximate(curve3, curve4)
+
+    def flattening(self, distance: float, segments: int = 16) -> Iterator[Vec2]:
+        def curve3(p0: T, p1: T, p2: T) -> Iterator[Vec2]:
+            if distance == 0.0:
+                raise ValueError(f"invalid max distance: 0.0")
+            return Vec2.generate(Bezier3P((p0, p1, p2)).flattening(distance, segments))
+
+        def curve4(p0: T, p1: T, p2: T, p3: T) -> Iterator[Vec2]:
+            if distance == 0.0:
+                raise ValueError(f"invalid max distance: 0.0")
+            return Vec2.generate(
+                Bezier4P((p0, p1, p2, p3)).flattening(distance, segments)
+            )
+
+        return self._approximate(curve3, curve4)
+
+    def to_3d_path(self, elevation: float = 0.0) -> Path:
+        """Returns a new 3D path, the z-axis of all vertices is set to `elevation`.
+        The conversion is almost as fast as a copy.
+        """
+        path3d = Path()
+        elevation = float(elevation)
+        path3d._vertices = [Vec3(v.x, v.y, elevation) for v in self._vertices]
+        self._copy_properties(path3d)
+        return path3d
+
+    def transform(self, m: Matrix44) -> Self:
+        """Returns a new transformed 2D path.
+
+        Args:
+             m: transformation matrix of type :class:`~ezdxf.math.Matrix44`
+
+        """
+        new_path = self.clone()
+        new_path._vertices = list(m.fast_2d_transform(self._vertices))
+        return new_path
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/path/shapes.py` & `ezdxf-1.1.0b0/src/ezdxf/path/shapes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021-2022, Manfred Moitzi
+# Copyright (c) 2021-2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import Optional
 import math
 from ezdxf.math import (
     cubic_bezier_arc_parameters,
     Matrix44,
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/path/tools.py` & `ezdxf-1.1.0b0/src/ezdxf/path/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 from typing import (
     TYPE_CHECKING,
     Iterable,
     Iterator,
     Optional,
     Sequence,
+    TypeVar,
 )
-
 import math
 from ezdxf.math import (
     Vec2,
     Vec3,
     UVec,
     Z_AXIS,
     OCS,
@@ -32,15 +32,15 @@
     cubic_bezier_arc_parameters,
     cubic_bezier_bbox,
     quadratic_bezier_bbox,
 )
 from ezdxf.math.triangulation import mapbox_earcut_2d
 from ezdxf.query import EntityQuery
 
-from .path import Path
+from .path import Path, Path2d, AbstractPath
 from .commands import Command
 from . import converter, nesting
 
 if TYPE_CHECKING:
     from ezdxf.query import EntityQuery
     from ezdxf.eztypes import GenericLayoutType
 
@@ -60,14 +60,15 @@
     "render_splines_and_polylines",
     "add_bezier4p",
     "add_bezier3p",
     "add_ellipse",
     "add_2d_polyline",
     "add_spline",
     "to_multi_path",
+    "to_3d_paths",
     "single_paths",
     "have_close_control_vertices",
     "lines_to_curve3",
     "lines_to_curve4",
     "fillet",
     "polygonal_fillet",
     "chamfer",
@@ -77,65 +78,78 @@
 ]
 
 MAX_DISTANCE = 0.01
 MIN_SEGMENTS = 4
 G1_TOL = 1e-4
 IS_CLOSE_TOL = 1e-10
 
+T = TypeVar("T", Path, Path2d)
+
 
 def to_multi_path(paths: Iterable[Path]) -> Path:
     """Returns a multi-path object from all given paths and their sub-paths.
     Ignores paths without any commands (empty paths).
     """
     multi_path = Path()
     for p in paths:
         multi_path.extend_multi_path(p)
     return multi_path
 
 
-def single_paths(paths: Iterable[Path]) -> Iterable[Path]:
+def to_3d_paths(paths: Iterable[Path | Path2d]) -> Iterator[Path]:
+    """Yields all paths as 3D :class:`Path` instances."""
+    if isinstance(paths, AbstractPath):
+        paths = [paths]
+    for path in paths:
+        if isinstance(path, Path2d):
+            yield path.to_3d_path()
+        else:
+            yield path
+
+
+def single_paths(paths: Iterable[T]) -> Iterable[T]:
     """Yields all given paths and their sub-paths as single path objects."""
     for p in paths:
         if p.has_sub_paths:
             yield from p.sub_paths()
         else:
             yield p
 
 
-def transform_paths(paths: Iterable[Path], m: Matrix44) -> list[Path]:
-    """Transform multiple :class:`Path` objects at once by transformation
-    matrix `m`. Returns a list of the transformed :class:`Path` objects.
+def transform_paths(paths: Iterable[T], m: Matrix44) -> list[T]:
+    """Transform multiple path objects at once by transformation
+    matrix `m`. Returns a list of the transformed path objects.
 
     Args:
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d` objects
         m: transformation matrix of type :class:`~ezdxf.math.Matrix44`
 
     """
     return [p.transform(m) for p in paths]
 
 
-def transform_paths_to_ocs(paths: Iterable[Path], ocs: OCS) -> list[Path]:
+def transform_paths_to_ocs(paths: Iterable[Path|Path2d], ocs: OCS) -> list[Path]:
     """Transform multiple :class:`Path` objects at once from WCS to OCS.
     Returns a list of the transformed :class:`Path` objects.
 
     Args:
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d` objects
         ocs: OCS transformation of type :class:`~ezdxf.math.OCS`
 
     """
     t = ocs.matrix.copy()
     t.transpose()
-    return transform_paths(paths, t)
+    return transform_paths(to_3d_paths(paths), t)
 
 
-def bbox(paths: Iterable[Path], *, fast=False) -> BoundingBox:
+def bbox(paths: Iterable[Path | Path2d], *, fast=False) -> BoundingBox:
     """Returns the :class:`~ezdxf.math.BoundingBox` for the given paths.
 
     Args:
-        paths: iterable of :class:`~ezdxf.path.Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d` objects
         fast: calculates the precise bounding box of Bèzier curves if
             ``False``, otherwise uses the control points of Bézier curves to
             determine their bounding box.
 
     """
     box = BoundingBox()
     for p in paths:
@@ -144,19 +158,16 @@
         else:
             bb = precise_bbox(p)
             if bb.has_data:
                 box.extend((bb.extmin, bb.extmax))
     return box
 
 
-def precise_bbox(path: Path) -> BoundingBox:
-    """Returns the precise :class:`~ezdxf.math.BoundingBox` for the given
-    :class:`~ezdxf.path.Path`.
-
-    """
+def precise_bbox(path: Path | Path2d) -> BoundingBox:
+    """Returns the precise :class:`~ezdxf.math.BoundingBox` for the given paths."""
     if len(path) == 0:  # empty path
         return BoundingBox()
     start = path.start
     points: list[Vec3] = [start]
     for cmd in path:
         if cmd.type == Command.LINE_TO:
             points.append(cmd.end)
@@ -257,15 +268,15 @@
 
 
 # Path to entity converter and render utilities:
 
 
 def render_lwpolylines(
     layout: GenericLayoutType,
-    paths: Iterable[Path],
+    paths: Iterable[Path|Path2d],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as
@@ -273,15 +284,15 @@
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector. The default extrusion vector
     is the WCS z-axis. The plane elevation is the distance from the WCS origin
     to the start point of the first path.
 
     Args:
         layout: the modelspace, a paperspace layout or a block definition
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve
         extrusion: extrusion vector for all paths
         dxfattribs: additional DXF attribs
 
     Returns:
         created entities in an :class:`~ezdxf.query.EntityQuery` object
@@ -299,15 +310,15 @@
     for lwpolyline in lwpolylines:
         layout.add_entity(lwpolyline)
     return EntityQuery(lwpolylines)
 
 
 def render_polylines2d(
     layout: GenericLayoutType,
-    paths: Iterable[Path],
+    paths: Iterable[Path|Path2d],
     *,
     distance: float = 0.01,
     segments: int = 4,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as 2D
@@ -315,15 +326,15 @@
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector.The default extrusion vector
     is the WCS z-axis. The plane elevation is the distance from the WCS origin
     to the start point of the first path.
 
     Args:
         layout: the modelspace, a paperspace layout or a block definition
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve
         extrusion: extrusion vector for all paths
         dxfattribs: additional DXF attribs
 
     Returns:
         created entities in an :class:`~ezdxf.query.EntityQuery` object
@@ -341,15 +352,15 @@
     for polyline2d in polylines2d:
         layout.add_entity(polyline2d)
     return EntityQuery(polylines2d)
 
 
 def render_hatches(
     layout: GenericLayoutType,
-    paths: Iterable[Path],
+    paths: Iterable[Path|Path2d],
     *,
     edge_path: bool = True,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     g1_tol: float = G1_TOL,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
@@ -359,15 +370,15 @@
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector. The default extrusion vector
     is the WCS z-axis. The plane elevation is the distance from the WCS origin
     to the start point of the first path.
 
     Args:
         layout: the modelspace, a paperspace layout or a block definition
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d`  objects
         edge_path: ``True`` for edge paths build of LINE and SPLINE edges,
             ``False`` for only LWPOLYLINE paths as boundary paths
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve to flatten polyline paths
         g1_tol: tolerance for G1 continuity check to separate SPLINE edges
         extrusion: extrusion vector for all paths
         dxfattribs: additional DXF attribs
@@ -390,15 +401,15 @@
     for hatch in hatches:
         layout.add_entity(hatch)
     return EntityQuery(hatches)
 
 
 def render_mpolygons(
     layout: GenericLayoutType,
-    paths: Iterable[Path],
+    paths: Iterable[Path|Path2d],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as
@@ -408,15 +419,15 @@
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector. The default extrusion vector
     is the WCS z-axis. The plane elevation is the distance from the WCS origin
     to the start point of the first path.
 
     Args:
         layout: the modelspace, a paperspace layout or a block definition
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path` or :class:`Path2d` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve to flatten polyline paths
         extrusion: extrusion vector for all paths
         dxfattribs: additional DXF attribs
 
     Returns:
         created entities in an :class:`~ezdxf.query.EntityQuery` object
@@ -434,26 +445,26 @@
     for polygon in polygons:
         layout.add_entity(polygon)
     return EntityQuery(polygons)
 
 
 def render_polylines3d(
     layout: GenericLayoutType,
-    paths: Iterable[Path],
+    paths: Iterable[Path|Path2d],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as 3D
     :class:`~ezdxf.entities.Polyline` entities.
 
     Args:
         layout: the modelspace, a paperspace layout or a block definition
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path`or :class:`Path2d` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve
         dxfattribs: additional DXF attribs
 
     Returns:
         created entities in an :class:`~ezdxf.query.EntityQuery` object
 
@@ -470,26 +481,26 @@
     for polyline3d in polylines3d:
         layout.add_entity(polyline3d)
     return EntityQuery(polylines3d)
 
 
 def render_lines(
     layout: GenericLayoutType,
-    paths: Iterable[Path],
+    paths: Iterable[Path|Path2d],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as
     :class:`~ezdxf.entities.Line` entities.
 
     Args:
         layout: the modelspace, a paperspace layout or a block definition
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path`or :class:`Path2d` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve
         dxfattribs: additional DXF attribs
 
     Returns:
         created entities in an :class:`~ezdxf.query.EntityQuery` object
 
@@ -505,25 +516,25 @@
     for line in lines:
         layout.add_entity(line)
     return EntityQuery(lines)
 
 
 def render_splines_and_polylines(
     layout: GenericLayoutType,
-    paths: Iterable[Path],
+    paths: Iterable[Path|Path2d],
     *,
     g1_tol: float = G1_TOL,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as :class:`~ezdxf.entities.Spline`
     and 3D :class:`~ezdxf.entities.Polyline` entities.
 
     Args:
         layout: the modelspace, a paperspace layout or a block definition
-        paths: iterable of :class:`Path` objects
+        paths: iterable of :class:`Path`or :class:`Path2d` objects
         g1_tol: tolerance for G1 continuity check
         dxfattribs: additional DXF attribs
 
     Returns:
         created entities in an :class:`~ezdxf.query.EntityQuery` object
 
     """
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.css` & `ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.html` & `ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.html`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.js` & `ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.js`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/pp/dxfpp.py` & `ezdxf-1.1.0b0/src/ezdxf/pp/dxfpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/pp/pprint.py` & `ezdxf-1.1.0b0/src/ezdxf/pp/pprint.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.css` & `ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/pp/rawpp.py` & `ezdxf-1.1.0b0/src/ezdxf/pp/rawpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/pp/reflinks.py` & `ezdxf-1.1.0b0/src/ezdxf/pp/reflinks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/abstract_mtext_renderer.py` & `ezdxf-1.1.0b0/src/ezdxf/render/abstract_mtext_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
         ctx.aci = mtext.dxf.color
         rgb = mtext.rgb
         if rgb is not None:
             ctx.rgb = rgb
         return ctx
 
     def get_font(self, ctx: MTextContext) -> fonts.AbstractFont:
-        ttf = fonts.find_ttf_path(ctx.font_face)  # 1st call is very slow
+        ttf = fonts.find_font_file_name(ctx.font_face)  # 1st call is very slow
         key = (ttf, ctx.cap_height, ctx.width_factor)
         font = self._font_cache.get(key)
         if font is None:
             font = fonts.make_font(ttf, ctx.cap_height, ctx.width_factor)
             self._font_cache[key] = font
         return font
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/arrows.py` & `ezdxf-1.1.0b0/src/ezdxf/render/arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/curves.py` & `ezdxf-1.1.0b0/src/ezdxf/render/curves.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/dimension.py` & `ezdxf-1.1.0b0/src/ezdxf/render/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/dim_base.py` & `ezdxf-1.1.0b0/src/ezdxf/render/dim_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/dim_curved.py` & `ezdxf-1.1.0b0/src/ezdxf/render/dim_curved.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/dim_diameter.py` & `ezdxf-1.1.0b0/src/ezdxf/render/dim_diameter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/dim_linear.py` & `ezdxf-1.1.0b0/src/ezdxf/render/dim_linear.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/dim_ordinate.py` & `ezdxf-1.1.0b0/src/ezdxf/render/dim_ordinate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/dim_radius.py` & `ezdxf-1.1.0b0/src/ezdxf/render/dim_radius.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/forms.py` & `ezdxf-1.1.0b0/src/ezdxf/render/forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/hatching.py` & `ezdxf-1.1.0b0/src/ezdxf/render/hatching.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Vec3,
     Bezier3P,
     Bezier4P,
     intersection_ray_cubic_bezier_2d,
     quadratic_to_cubic_bezier,
 )
 from ezdxf import const
-from ezdxf.path import Path, LineTo, MoveTo, Curve3To, Curve4To
+from ezdxf.path import Path, Path2d, LineTo, MoveTo, Curve3To, Curve4To
 
 if TYPE_CHECKING:
     from ezdxf.entities.polygon import DXFPolygon
 
 MIN_HATCH_LINE_DISTANCE = 1e-4  # ??? what's a good choice
 NONE_VEC2 = Vec2(math.nan, math.nan)
 KEY_NDIGITS = 4
@@ -485,15 +485,15 @@
 
     if not path_start.isclose(start):  # close path
         yield start, path_start
 
 
 def hatch_paths(
     baseline: HatchBaseLine,
-    paths: Sequence[Path],
+    paths: Sequence[Path|Path2d],
     terminate: Optional[Callable[[], bool]] = None,
 ) -> Iterator[Line]:
     """Yields all pattern lines for all hatch lines generated by the given
     :class:`HatchBaseLine`, intersecting the given 2D :class:`~ezdxf.path.Path`
     instances as :class:`Line` instances. The paths are handled as projected
     into the xy-plane the z-axis of path vertices will be ignored if present.
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/leader.py` & `ezdxf-1.1.0b0/src/ezdxf/render/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/linetypes.py` & `ezdxf-1.1.0b0/src/ezdxf/render/linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/mesh.py` & `ezdxf-1.1.0b0/src/ezdxf/render/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/mleader.py` & `ezdxf-1.1.0b0/src/ezdxf/render/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/mline.py` & `ezdxf-1.1.0b0/src/ezdxf/render/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/point.py` & `ezdxf-1.1.0b0/src/ezdxf/render/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/polyline.py` & `ezdxf-1.1.0b0/src/ezdxf/render/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/r12spline.py` & `ezdxf-1.1.0b0/src/ezdxf/render/r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/trace.py` & `ezdxf-1.1.0b0/src/ezdxf/render/trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/_linetypes.py` & `ezdxf-1.1.0b0/src/ezdxf/render/_linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/render/__init__.py` & `ezdxf-1.1.0b0/src/ezdxf/render/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/16x16.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/16x16.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/24x24.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/24x24.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/256x256.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/256x256.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/32x32.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/32x32.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/48x48.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/48x48.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/64x64.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/64x64.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/icon-copy-64px.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/icon-copy-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/icon-find-64px.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/icon-find-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-bookmark-64px.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-handle-64px.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-handle-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/icon-goto-line-64px.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/icon-goto-line-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/icon-left-arrow-64px.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/icon-left-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/icon-next-entity-64px.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/icon-next-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/icon-prev-entity-64px.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/icon-prev-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/icon-right-arrow-64px.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/icon-right-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/icon-show-in-tree-64px.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/icon-show-in-tree-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/resources/icon-store-bookmark-64px.png` & `ezdxf-1.1.0b0/src/ezdxf/resources/icon-store-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/sections/acdsdata.py` & `ezdxf-1.1.0b0/src/ezdxf/sections/acdsdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/sections/blocks.py` & `ezdxf-1.1.0b0/src/ezdxf/sections/blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/sections/classes.py` & `ezdxf-1.1.0b0/src/ezdxf/sections/classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/sections/entities.py` & `ezdxf-1.1.0b0/src/ezdxf/sections/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/sections/headervars.py` & `ezdxf-1.1.0b0/src/ezdxf/sections/headervars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/sections/objects.py` & `ezdxf-1.1.0b0/src/ezdxf/sections/objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/sections/table.py` & `ezdxf-1.1.0b0/src/ezdxf/sections/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/sections/tables.py` & `ezdxf-1.1.0b0/src/ezdxf/sections/tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/analyze.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/analyze.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/binarydata.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/binarydata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/codepage.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/codepage.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/complex_ltype.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/complex_ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/crypt.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/debug.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/debug.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/difftags.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/handle.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/indexing.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/juliandate.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/pattern.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/rawloader.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/rawloader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/standards.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/standards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/test.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/test.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/text.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1630,23 +1630,23 @@
         )
 
     def parse_font_properties(self, ctx: MTextContext):
         parts = self.extract_expression().split("|")
         # an empty font family name does not change the font properties
         if parts and parts[0]:
             name = parts[0]
-            style = "normal"
-            weight = "normal"
+            style = "Regular"
+            weight = 400
             # ignore codepage and pitch - it seems not to be used in newer
             # CAD applications.
             for part in parts[1:]:
                 if part.startswith("b1"):
-                    weight = "bold"
+                    weight = 700
                 elif part.startswith("i1"):
-                    style = "italic"
+                    style = "Italic"
             ctx.font_face = FontFace(family=name, style=style, weight=weight)
 
     def consume_optional_terminator(self):
         if self.scanner.peek() == ";":
             self.scanner.consume(1)
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/text_layout.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/text_size.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/text_size.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     with the text path objects created by the `Matplotlib` package.
 
     """
     width_factor: float = text.dxf.get_default("width")
     text_width: float = 0.0
     cap_height: float = text.dxf.get_default("height")
     font: fonts.AbstractFont = fonts.MonospaceFont(cap_height, width_factor)
-    if ezdxf.options.use_matplotlib and text.doc is not None:
+    if text.doc is not None:
         style = text.doc.styles.get(text.dxf.get_default("style"))
         font_name = get_font_name(style)
         font = fonts.make_font(font_name, cap_height, width_factor)
 
     total_height = font.measurements.total_height
     content = text.plain_text()
     if content:
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/zipmanager.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/zipmanager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/_iso_pattern.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/_iso_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf/tools/__init__.py` & `ezdxf-1.1.0b0/src/ezdxf/tools/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/src/ezdxf.egg-info/PKG-INFO` & `ezdxf-1.1.0b0/src/ezdxf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.0.4b1
+Version: 1.1.0b0
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides: ezdxf
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: draw
 Provides-Extra: draw5
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: all
 Provides-Extra: all5
@@ -51,21 +50,23 @@
 Quick-Info
 ----------
 
 - *ezdxf* is a Python package to create new DXF files and read/modify/write 
   existing DXF documents
 - MIT-License
 - the intended audience are programmers
-- requires at least Python 3.7
+- requires at least Python 3.8
 - OS independent
 - tested with CPython and pypy3
 - has type annotations and passes `mypy --ignore-missing-imports -p ezdxf` successful
 - additional required packages for the core package without add-ons: 
   [typing_extensions](https://pypi.org/project/typing-extensions/), 
-  [pyparsing](https://pypi.org/project/pyparsing/) 
+  [pyparsing](https://pypi.org/project/pyparsing/),
+  [numpy](https://pypi.org/project/numpy/),
+  [fontTools](https://pypi.org/project/fonttools/)
 - read/write/new support for DXF versions: R12, R2000, R2004, R2007, R2010, R2013 and R2018
 - additional read-only support for DXF versions R13/R14 (upgraded to R2000)
 - additional read-only support for older DXF versions than R12 (upgraded to R12)
 - read/write support for ASCII DXF and Binary DXF
 - retains third-party DXF content
 - optional C-extensions for CPython are included in the binary wheels, available 
   on [PyPI](https://pypi.org/project/ezdxf/) for Windows, Linux and macOS
@@ -210,27 +211,45 @@
 Feedback is greatly appreciated.
 
 Manfred
 
 News
 ====
 
-Version 1.0.4b1 - dev
+Version 1.1.0b0 - dev
 ---------------------
 
-- Release notes: https://ezdxf.mozman.at/release-v1-0.html
+- Release notes: https://ezdxf.mozman.at/release-v1-1.html
+- WARNING: The font support changed drastically in this version, if you use the 
+  `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
+  v1.0.3 in your `requirements.txt` file to use the previous version!
+- NEW: `numpy` is a hard dependency, requires Python version >= 3.8
+- NEW: `fontTools` is a hard dependency
+- NEW: `Matrix44.Path2d()` class, `Path` class with `Vec2` vertices
+- NEW: optimized `Matrix44.fast_2d_transform()` method
 - NEW: added setter to `BlockLayout.base_point` property
+- NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
+- NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG
+- NEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF
+- NEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG
+- NEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF
+- CHANGED: refactoring of `ezdxf.tools.fonts`
+- CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
+  renamed to `width` and is also an int value (1-9) now
+- REMOVED: replaced `matplotlib` font support module by `fontTools`
+- REMOVED: configuration option `use_matplotlib`
+- CHANGED: text rendering for the `drawing` add-on and text measurement is done by the
+  `fontTools` package
+- CHANGED: moved text rendering from backend classes to the `Frontend` class
+- CHANGED: moved clipping support from backend classes to the `Frontend` class
+- REMOVED: `PillowBackend` and the `pillow` command
+- REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
 - BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
   scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
-- PREVIEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF or SVG,  
-  final release in v1.1
-- PREVIEW: `ezdxf plt2dxf` command to convert HPGL/2 plot files to DXF, final release in v1.1
-- PREVIEW: `ezdxf plt2svg` command to convert HPGL/2 plot files to SVG, final release in v1.1
-- PREVIEW: `ezdxf plt2pdf` command to convert HPGL/2 plot files to PDF, final release in v1.1
 
 Version 1.0.3 - 2023-03-26
 --------------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: [#833](https://github.com/mozman/ezdxf/issues/833)
   logging non-unique entity handles when loading a DXF document as warnings, auditing
```

## Comparing `ezdxf-1.0.4b1/src/ezdxf.egg-info/SOURCES.txt` & `ezdxf-1.1.0b0/src/ezdxf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 NEWS.md
 README.md
 requirements.txt
 setup.cfg
 setup.py
 integration_tests/check_disable_c_ext_by_config_file.py
 integration_tests/check_disable_c_ext_by_env_var.py
+integration_tests/conftest.py
 integration_tests/test_acad_table.py
 integration_tests/test_all_dimline_styles.py
 integration_tests/test_all_ellipse_transformations.py
 integration_tests/test_anonymous_blocks.py
 integration_tests/test_audit_critical_dxf_files.py
 integration_tests/test_audit_layouts.py
 integration_tests/test_complex_line_type_2.py
 integration_tests/test_create_basic_graphics.py
 integration_tests/test_document_guid.py
 integration_tests/test_document_page_setup.py
-integration_tests/test_drawing_matplotlib_backend.py
-integration_tests/test_drawing_qt_backend.py
 integration_tests/test_dxf_info_scanning.py
 integration_tests/test_entities_iterator.py
 integration_tests/test_fix_dulicate_handles.py
 integration_tests/test_geo.py
 integration_tests/test_groups.py
 integration_tests/test_ignore_junk_beyond_EOF.py
 integration_tests/test_launcher.py
 integration_tests/test_leica_disto_r12.py
 integration_tests/test_load_dxf_unicode_notation.py
 integration_tests/test_mapbox_earcut.py
-integration_tests/test_matplotlib_font_support.py
 integration_tests/test_mtext_columns.py
 integration_tests/test_mtext_explode_addon.py
 integration_tests/test_mtext_text_frame.py
 integration_tests/test_new_table_entries.py
 integration_tests/test_none_ascii_read_write.py
 integration_tests/test_odafc.py
 integration_tests/test_open_R13_R14.py
@@ -100,14 +98,15 @@
 src/ezdxf/enums.py
 src/ezdxf/explode.py
 src/ezdxf/eztypes.py
 src/ezdxf/filemanagement.py
 src/ezdxf/gfxattribs.py
 src/ezdxf/graphicsfactory.py
 src/ezdxf/groupby.py
+src/ezdxf/npshapes.py
 src/ezdxf/protocols.py
 src/ezdxf/proxygraphic.py
 src/ezdxf/py.typed
 src/ezdxf/query.py
 src/ezdxf/queryparser.py
 src/ezdxf/r12strict.py
 src/ezdxf/recover.py
@@ -192,30 +191,29 @@
 src/ezdxf/addons/browser/find_dialog.py
 src/ezdxf/addons/browser/loader.py
 src/ezdxf/addons/browser/model.py
 src/ezdxf/addons/browser/tags.py
 src/ezdxf/addons/browser/views.py
 src/ezdxf/addons/drawing/__init__.py
 src/ezdxf/addons/drawing/backend.py
+src/ezdxf/addons/drawing/clipper.py
 src/ezdxf/addons/drawing/config.py
 src/ezdxf/addons/drawing/debug_backend.py
 src/ezdxf/addons/drawing/debug_utils.py
 src/ezdxf/addons/drawing/frontend.py
 src/ezdxf/addons/drawing/gfxproxy.py
 src/ezdxf/addons/drawing/matplotlib.py
-src/ezdxf/addons/drawing/mpl_text_renderer.py
 src/ezdxf/addons/drawing/mtext_complex.py
-src/ezdxf/addons/drawing/pillow.py
 src/ezdxf/addons/drawing/properties.py
 src/ezdxf/addons/drawing/pyqt.py
-src/ezdxf/addons/drawing/qt_text_renderer.py
 src/ezdxf/addons/drawing/qtviewer.py
 src/ezdxf/addons/drawing/text.py
 src/ezdxf/addons/drawing/text_renderer.py
 src/ezdxf/addons/drawing/type_hints.py
+src/ezdxf/addons/drawing/unified_text_renderer.py
 src/ezdxf/addons/dwg/__init__.py
 src/ezdxf/addons/dwg/classes_section.py
 src/ezdxf/addons/dwg/const.py
 src/ezdxf/addons/dwg/crc.py
 src/ezdxf/addons/dwg/fileheader.py
 src/ezdxf/addons/dwg/header_section.py
 src/ezdxf/addons/dwg/loader.py
@@ -424,37 +422,38 @@
 src/ezdxf/sections/header.py
 src/ezdxf/sections/headervars.py
 src/ezdxf/sections/objects.py
 src/ezdxf/sections/table.py
 src/ezdxf/sections/tables.py
 src/ezdxf/tools/__init__.py
 src/ezdxf/tools/_iso_pattern.py
-src/ezdxf/tools/_matplotlib_font_support.py
 src/ezdxf/tools/analyze.py
 src/ezdxf/tools/binarydata.py
 src/ezdxf/tools/codepage.py
 src/ezdxf/tools/complex_ltype.py
 src/ezdxf/tools/crypt.py
 src/ezdxf/tools/debug.py
 src/ezdxf/tools/difftags.py
-src/ezdxf/tools/font_face_cache.json
-src/ezdxf/tools/font_measurement_cache.json
+src/ezdxf/tools/font_face.py
+src/ezdxf/tools/font_manager.py
 src/ezdxf/tools/fonts.py
 src/ezdxf/tools/handle.py
 src/ezdxf/tools/indexing.py
 src/ezdxf/tools/juliandate.py
 src/ezdxf/tools/pattern.py
 src/ezdxf/tools/rawloader.py
 src/ezdxf/tools/standards.py
 src/ezdxf/tools/strip.py
 src/ezdxf/tools/test.py
 src/ezdxf/tools/text.py
 src/ezdxf/tools/text_layout.py
 src/ezdxf/tools/text_size.py
+src/ezdxf/tools/ttfonts.py
 src/ezdxf/tools/zipmanager.py
+tests/conftest.py
 tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
 tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
 tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
 tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
 tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
 tests/test_00_dxf_low_level_structs/test_010_binary_data.py
 tests/test_00_dxf_low_level_structs/test_011_codepage.py
@@ -667,14 +666,15 @@
 tests/test_05_tools/test_532_acis_mesh.py
 tests/test_05_tools/test_533_shapefiles.py
 tests/test_05_tools/test_534_dwg_info.py
 tests/test_05_tools/test_535_xref_basic.py
 tests/test_05_tools/test_536_xref_conflict.py
 tests/test_05_tools/test_537_transform.py
 tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+tests/test_05_tools/test_539_npshapes.py
 tests/test_06_math/conftest.py
 tests/test_06_math/test_600_base.py
 tests/test_06_math/test_601_bulge.py
 tests/test_06_math/test_602_vec3.py
 tests/test_06_math/test_603_vec2.py
 tests/test_06_math/test_604_banded_matrix.py
 tests/test_06_math/test_604_linalg.py
@@ -710,15 +710,14 @@
 tests/test_06_math/test_642_construction_line.py
 tests/test_06_math/test_643_construction_box.py
 tests/test_06_math/test_644_construction_circle.py
 tests/test_06_math/test_645_construction_arc.py
 tests/test_06_math/test_646_offset_vertices_2d.py
 tests/test_06_math/test_647_transform_tools.py
 tests/test_06_math/test_648_construction_ellipse.py
-tests/test_06_math/test_649_nurbs_python_interface.py
 tests/test_06_math/test_650_elliptic_arc_span.py
 tests/test_06_math/test_651_construction_polyline.py
 tests/test_06_math/test_652_approx_param_t.py
 tests/test_06_math/test_653_polyline_intersection.py
 tests/test_06_math/test_654_rtree.py
 tests/test_06_math/test_655_dbscan.py
 tests/test_06_math/test_656_k_means.py
@@ -765,14 +764,15 @@
 tests/test_08_addons/test_816_bin_packing.py
 tests/test_08_addons/test_817_genetic_algorithm.py
 tests/test_08_addons/test_818_meshex.py
 tests/test_08_addons/test_819_menger_sponge.py
 tests/test_08_addons/test_820_openscad.py
 tests/test_08_addons/test_821_hpgl2.py
 tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+tests/test_08_addons/test_822_clipper.py
 tests/test_09_cython_acceleration/test_901_acc_vec2.py
 tests/test_09_cython_acceleration/test_902_acc_vec3.py
 tests/test_09_cython_acceleration/test_903_acc_matrix44.py
 tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
 tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
 tests/test_09_cython_acceleration/test_906_acc_bspline.py
 tests/test_10_issues/test_issue_414_bbox_calculation.py
```

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_010_binary_data.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_010_binary_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_012_crypt.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_012_crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_013_juliandate.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_013_juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_016_encoding.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_016_encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_018_handle.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_018_handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_024_render_tag.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_024_render_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_040_tags.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_040_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_041_group_tags.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_041_group_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py` & `ezdxf-1.1.0b0/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_101_dxfnamespace.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_101_dxfnamespace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_102_appdata.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_102_appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_103_reactors.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_103_reactors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_104_extension_dict.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_104_extension_dict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_105_xdata.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_105_xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_110_dxfentity.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_110_dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_112a_dxfgfx.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_112a_dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_112b_dxfobj.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_112b_dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_113_dxfclass.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_113_dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_114_factory.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_114_factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_115_new_empty_drawing.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_115_new_empty_drawing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_116_dictionary.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_116_dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_117_layer_table_entry.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_117_layer_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_119_ucs_table_entry.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_119_ucs_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_120_style_table_entry.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_120_style_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_121_ltype_table_entry.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_121_ltype_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_123_view_table_entry.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_123_view_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_125_image_def.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_125_image_def.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_126_image_def_reactor.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_126_image_def_reactor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_127_raster_variables.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_127_raster_variables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_128_pdf_definition.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_128_pdf_definition.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_129_xrecord.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_129_xrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_130_id_buffer.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_130_id_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_131_field_list.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_131_field_list.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_132_layer_filter.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_132_layer_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_133_sun.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_133_sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_134_material.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_134_material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_135_geo_data.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_135_geo_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_136_vba_project.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_136_vba_project.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_137_sortentstable.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_137_sortentstable.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_138_setup_visual_styles.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_138_setup_visual_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_139_user_record.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_139_user_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_140_block_record.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_140_block_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_01_dxf_entities/test_141_layer_vp_override.py` & `ezdxf-1.1.0b0/tests/test_01_dxf_entities/test_141_layer_vp_override.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/conftest.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_200_line.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_200_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_201_point.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_201_point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_202_circle.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_202_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_203_arc.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_203_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_204_shape.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_204_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_205_solid.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_205_solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_206_text.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_206_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_207_attdef.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_207_attdef.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_208_attrib.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_208_attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_209_vertex.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_209_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_1.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_2.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_explode.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_211_viewport.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_211_viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_212_insert.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_212_insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_213_minsert.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_213_minsert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_214_block.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_214_block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_215_dimension.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_215_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_216_dimlines_R12.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_216_dimlines_R12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_221_ellipse.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_221_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_222_xline.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_222_xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_223_ray.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_223_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_224_group.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_224_group.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_225_mtext.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_225_mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_226_spline.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_226_spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_228_mesh.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_228_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229b_hatch_extended.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229b_hatch_extended.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_231_underlay.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_231_underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_231_underlay_2.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_231_underlay_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_acis.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_acis_2.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_acis_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_232_surface.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_232_surface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_233_helix.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_233_helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_234_light.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_234_light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_235_leader.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_235_leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_236_multileader.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_236_multileader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_237_mline.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_237_mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_238_tolerance.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_238_tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_239_proxy_graphic.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_239_proxy_graphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_240_arc_dimension.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_240_arc_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_241_hyperlink.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_241_hyperlink.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_242_random_transform.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_242_random_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_243_replace_entity.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_243_replace_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_245_wipeout.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_245_wipeout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_246_spline_audit.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_246_spline_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_248_mpolygon.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_248_mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_249_boundary_paths.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_249_boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_251_upright.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_251_upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_253_ole2frame.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_253_ole2frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_02_dxf_graphics/test_254_get_font_name.py` & `ezdxf-1.1.0b0/tests/test_02_dxf_graphics/test_254_get_font_name.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_300_layout.py` & `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_300_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py` & `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_302_block_references.py` & `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_302_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_303_auto_block_references.py` & `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_303_auto_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_304_new_entity_space.py` & `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_304_new_entity_space.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py` & `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py` & `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_307_groupby.py` & `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_307_groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_308_query.py` & `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_308_query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_309_query_parser.py` & `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_309_query_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py` & `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_312_virtual_layout.py` & `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_312_virtual_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_03_dxf_layouts/test_313_redraw_order.py` & `ezdxf-1.1.0b0/tests/test_03_dxf_layouts/test_313_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_401_headersection.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_401_headersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_402_classessection.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_402_classessection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_403_entity_database.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_403_entity_database.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_404a_tables.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_404a_tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_405_classes.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_405_classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_407_entity_section.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_407_entity_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_408_objects_section.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_408_objects_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_409_create_objects.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_409_create_objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_410_table.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_410_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_411_acds_data.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_411_acds_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_415_layout_management.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_415_layout_management.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,15 +288,15 @@
     assert p.is_empty is False
     assert p.path is not None
     assert p.mesh is None
     assert len(list(p.vertices())) == 5, "expected closed box"
 
     box = p.bbox()
     # exact bounding box size depends on platform and matplotlib usage!
-    assert box.size.x > 20
+    assert 18 < box.size.x < 22
     assert box.size.y > 2.5
 
 
 def test_mtext_to_primitive():
     # Testing just the control flow, correct bounding boxes are visually tested.
     # see: ezdxf/examples/entities/mtext.py
     mtext = factory.new("MTEXT")
@@ -305,15 +305,15 @@
     assert p.is_empty is False
     assert p.path is not None
     assert p.mesh is None
     assert len(list(p.vertices())) == 5, "expected closed box"
 
     box = p.bbox()
     # exact bounding box size depends on platform and matplotlib usage!
-    assert box.size.x > 20
+    assert 18 < box.size.x < 22  # pypy
     assert box.size.y > 2.5
 
 
 def test_mtext_columns_to_primitive():
     from ezdxf.entities.mtext import MTextColumns
 
     mtext = factory.new("MTEXT")
```

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_417_bbox.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_417_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_424_audit.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_424_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_427_appsettings.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_427_appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py` & `ezdxf-1.1.0b0/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/conftest.py` & `ezdxf-1.1.0b0/tests/test_05_tools/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_500_units.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_500_units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_501_truecolor.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_501_truecolor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_502_raw_color.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_502_raw_color.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_503_indexing.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_503_indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_504_suppress_zeros.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_504_suppress_zeros.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_507_dxf_pretty_printer.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_507_dxf_pretty_printer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_508_read_zip.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_508_read_zip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_509_comments.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_509_comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_510_byte_stream.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_510_byte_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_511_bit_stream.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_511_bit_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_512_pattern.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_512_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_513_reorder_entities.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_513_reorder_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_514_text.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_514_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_516_zoom.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_516_zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_517_text_layout.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_517_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_519_mtext_editor.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_519_mtext_editor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_520_mtext_context.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_520_mtext_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_521_mtext_parser.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_521_mtext_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,29 +347,29 @@
         assert t0.ctx.align == 0
         assert t0.data == "word", "invalid argument should be removed"
 
     def test_font_b0_i0(self):
         t0 = list(MTextParser(r"\fArial Narrow;word"))[0]
         font_face = t0.ctx.font_face
         assert font_face.family == "Arial Narrow"
-        assert font_face.style == "normal"
-        assert font_face.weight == "normal"
+        assert font_face.style == "Regular"
+        assert font_face.weight == 400
 
     def test_font_b1_i0(self):
         t0 = list(MTextParser(r"\fArial Narrow|b1;word"))[0]
-        assert t0.ctx.font_face.weight == "bold"
+        assert t0.ctx.font_face.weight == 700
 
     def test_font_b0_i1(self):
         t0 = list(MTextParser(r"\fArial Narrow|i1;word"))[0]
-        assert t0.ctx.font_face.style == "italic"
+        assert t0.ctx.font_face.style == "Italic"
 
     def test_font_b1_i1(self):
         t0 = list(MTextParser(r"\fArial Narrow|i1|b1;word"))[0]
-        assert t0.ctx.font_face.style == "italic"
-        assert t0.ctx.font_face.weight == "bold"
+        assert t0.ctx.font_face.style == "Italic"
+        assert t0.ctx.font_face.weight == 700
 
     def test_font_uppercase_command(self):
         t0 = list(MTextParser(r"\FArial Narrow;word"))[0]
         assert t0.ctx.font_face.family == "Arial Narrow"
 
     def test_empty_font_command_does_not_change_font_properties(self):
         t0, t1 = list(MTextParser(r"\fArial;word\f;word"))
```

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_522_text_scanner.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_522_text_scanner.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_523_text_size.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_523_text_size.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,26 +11,18 @@
     mtext_size,
     WordSizeDetector,
     estimate_mtext_extents,
 )
 
 from ezdxf.tools.text_layout import leading
 
-# Exact text size checks are not possible if the used font is not available,
-# which cannot guaranteed for all platforms therefore the matplotlib support is
-# disabled deliberately by using a virtual layout, which has no text style
-# tables attached and the "MonospaceFont" based text measurements are used.
-
 
 @pytest.fixture
 def msp():
-    state = ezdxf.options.use_matplotlib
-    ezdxf.options.use_matplotlib = False
     yield VirtualLayout()
-    ezdxf.options.use_matplotlib = state
 
 
 H3W1 = {"height": 3.0, "width": 1.0}
 H2W2 = {"height": 2.0, "width": 2.0}
 
 
 def test_text_size_of_an_empty_string(msp):
@@ -77,24 +69,22 @@
 )
 def test_measurement_of_plain_text(msp, s):
     text = msp.add_text(s, dxfattribs=H3W1)
     size = text_size(text)
     assert size.width == 3.0 * size.cap_height
 
 
-def test_matplotlib_support_for_text_size():
-    if not ezdxf.options.use_matplotlib:
-        return
+def test_support_for_text_size():
     test_string = "TestString"
     doc = ezdxf.new()
-    doc.styles.add("ARIAL", font="arial.ttf")
+    doc.styles.add("OpenSans", font="OpenSans.ttf")
     text = doc.modelspace().add_text(
         test_string,
         dxfattribs={
-            "style": "ARIAL",
+            "style": "OpenSans",
             "height": 2.0,
         },
     )
     length = len(test_string)
     size = text_size(text)
     # Do not check exact measurements, "arial.ttf" is not available at all
     # platforms by default!
@@ -115,26 +105,26 @@
 
 
 def test_mtext_size_of_a_single_char(msp):
     # Matplotlib support disabled and using MonospaceFont()
     mtext = msp.add_mtext("X", dxfattribs={"char_height": 2.0})
     size = mtext_size(mtext)
     assert size.total_height == 2.0
-    assert size.total_width == 2.0
-    assert size.column_width == 2.0
+    assert size.total_width == pytest.approx(1.8794373744139317)
+    assert size.column_width == pytest.approx(1.8794373744139317)
     assert size.gutter_width == 0.0
     assert size.column_count == 1
 
 
 def test_mtext_size_of_a_string(msp):
     # Matplotlib support disabled and using MonospaceFont()
     mtext = msp.add_mtext("XXX", dxfattribs={"char_height": 2.0})
     size = mtext_size(mtext)
     assert size.total_height == 2.0
-    assert size.total_width == 6.0
+    assert size.total_width == pytest.approx(5.6383121232417945)
     assert size.column_width == size.total_width
     assert size.gutter_width == 0.0
     assert size.column_count == 1
 
 
 def test_estimate_mtext_extents(msp):
     # Matplotlib support disabled and using MonospaceFont()
@@ -146,44 +136,28 @@
         },
     )
     width, height = estimate_mtext_extents(mtext)
     assert height == pytest.approx(15.336)  # 5 lines!
     assert width == 8.0
 
 
-@pytest.mark.parametrize("cap_height", [2.0, 3.0])
-def test_mtext_size_of_2_lines(cap_height, msp):
+@pytest.mark.parametrize(
+    "cap_height, expected", [(2.0, 6.703281982585398), (3.0, 10.054922973878098)]
+)
+def test_mtext_size_of_2_lines(cap_height, expected, msp):
     # Matplotlib support disabled and using MonospaceFont()
     mtext = msp.add_mtext(
         "XXX\nYYYY",
         dxfattribs={
             "char_height": cap_height,
             "line_spacing_factor": 1.0,
         },
     )
     size = mtext_size(mtext)
     expected_total_height = leading(cap_height, line_spacing=1.0) + cap_height
     assert size.total_height == pytest.approx(expected_total_height)
-    assert size.total_width == 4 * cap_height, "expected width of 2nd line"
+    assert size.total_width == pytest.approx(expected), "expected width of 2nd line"
     assert size.column_width == size.total_width
 
 
-@pytest.mark.parametrize("cap_height", [2.0, 3.0])
-def test_measure_mtext_word_size(cap_height, msp):
-    # Matplotlib support disabled and using MonospaceFont()
-    mtext = msp.add_mtext(
-        "XXX\nYYYY",
-        dxfattribs={
-            "char_height": cap_height,
-            "line_spacing_factor": 1.0,
-        },
-    )
-    word_size_detector = WordSizeDetector()
-    mtext_size(mtext, tool=word_size_detector)
-    boxes = word_size_detector.word_boxes()
-    assert len(boxes) == 2
-    assert BoundingBox2d(boxes[0]).size.isclose((cap_height * 3, cap_height))
-    assert BoundingBox2d(boxes[1]).size.isclose((cap_height * 4, cap_height))
-
-
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_524_block_reference_manager.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_524_block_reference_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_525_transparency.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_525_transparency.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_526_explode.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_526_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_527_gfxattribs.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_527_gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_528_difftags.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_528_difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_529_acis_sat.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_529_acis_sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_530_acis_sab.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_530_acis_sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_531_acis_entities.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_531_acis_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_532_acis_mesh.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_532_acis_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_533_shapefiles.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_533_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_534_dwg_info.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_534_dwg_info.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_535_xref_basic.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_535_xref_basic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_536_xref_conflict.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_536_xref_conflict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_537_transform.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_537_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_05_tools/test_538_scale_mtext_inline_commands.py` & `ezdxf-1.1.0b0/tests/test_05_tools/test_538_scale_mtext_inline_commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/conftest.py` & `ezdxf-1.1.0b0/tests/test_06_math/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_600_base.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_600_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_601_bulge.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_601_bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_602_vec3.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_602_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_603_vec2.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_603_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_604_banded_matrix.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_604_banded_matrix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_604_linalg.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_604_linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_605_matrix44.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_605_matrix44.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2010-2020, Manfred Moitzi
+# Copyright (c) 2010-2023, Manfred Moitzi
 # License: MIT License
 import pytest
 import pickle
 from math import radians, sin, cos, pi, isclose
 
 # Import from 'ezdxf.math._matrix44' to test Python implementation
 from ezdxf.math import (
@@ -51,27 +51,23 @@
         matrix = m44([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15])
         assert matrix.get_row(0) == (0.0, 1.0, 2.0, 3.0)
         assert matrix.get_row(1) == (4.0, 5.0, 6.0, 7.0)
         assert matrix.get_row(2) == (8.0, 9.0, 10.0, 11.0)
         assert matrix.get_row(3) == (12.0, 13.0, 14.0, 15.0)
 
     def test_row_constructor(self, m44):
-        matrix = m44(
-            (0, 1, 2, 3), (4, 5, 6, 7), (8, 9, 10, 11), (12, 13, 14, 15)
-        )
+        matrix = m44((0, 1, 2, 3), (4, 5, 6, 7), (8, 9, 10, 11), (12, 13, 14, 15))
         assert matrix.get_row(0) == (0.0, 1.0, 2.0, 3.0)
         assert matrix.get_row(1) == (4.0, 5.0, 6.0, 7.0)
         assert matrix.get_row(2) == (8.0, 9.0, 10.0, 11.0)
         assert matrix.get_row(3) == (12.0, 13.0, 14.0, 15.0)
 
     def test_invalid_row_constructor(self, m44):
         with pytest.raises(ValueError):
-            m44(
-                (0, 1, 2, 3), (4, 5, 6, 7), (8, 9, 10, 11), (12, 13, 14, 15, 16)
-            )
+            m44((0, 1, 2, 3), (4, 5, 6, 7), (8, 9, 10, 11), (12, 13, 14, 15, 16))
         with pytest.raises(ValueError):
             m44(
                 (0, 1, 2, 3),
                 (4, 5, 6, 7),
                 (8, 9, 10, 11),
                 (
                     12,
@@ -265,17 +261,15 @@
         )
         assert equal_matrix(res, expected)
         # __matmul__()
         res = m1 @ m2
         assert equal_matrix(res, expected)
 
     def test_transpose(self, m44):
-        matrix = m44(
-            (0, 1, 2, 3), (4, 5, 6, 7), (8, 9, 10, 11), (12, 13, 14, 15)
-        )
+        matrix = m44((0, 1, 2, 3), (4, 5, 6, 7), (8, 9, 10, 11), (12, 13, 14, 15))
         matrix.transpose()
         assert matrix.get_row(0) == (0.0, 4.0, 8.0, 12.0)
         assert matrix.get_row(1) == (1.0, 5.0, 9.0, 13.0)
         assert matrix.get_row(2) == (2.0, 6.0, 10.0, 14.0)
         assert matrix.get_row(3) == (3.0, 7.0, 11.0, 15.0)
 
     def test_inverse_error(self, m44):
@@ -297,41 +291,83 @@
         values = list(range(16))
         matrix = m44(values)
         matrix[0, 0] = 12
         assert values[0] == 0
         assert matrix[0, 0] == 12
 
     def test_picklable(self, m44):
-        matrix = m44(
-            (0.1, 1, 2, 3), (4, 5, 6, 7), (8, 9, 10, 11), (12, 13, 14, 15)
-        )
+        matrix = m44((0.1, 1, 2, 3), (4, 5, 6, 7), (8, 9, 10, 11), (12, 13, 14, 15))
         pickled_matrix = pickle.loads(pickle.dumps(matrix))
         assert equal_matrix(matrix, pickled_matrix)
         assert type(matrix) is type(pickled_matrix)
         matrix[0, 0] = 12
         assert not equal_matrix(matrix, pickled_matrix)
 
     def test_shear_xy(self, m44):
         angle = pi / 4
         matrix = m44.shear_xy(angle_x=angle, angle_y=-angle)
         assert matrix[0, 1] == pytest.approx(-1.0)
         assert matrix[1, 0] == pytest.approx(1.0)
 
+    def test_from_2d_transformation(self, m44):
+        components = (2, 0, 0, 2, 10, 20)
+        matrix = m44.from_2d_transformation(components)
+        assert matrix.transform((1, 1)).isclose((12, 22))
+
+    @pytest.mark.parametrize(
+        "components",
+        [
+            [],
+            [0, 1, 2, 3, 4],
+            [0, 1, 2, 3, 4, 5, 6],
+        ],
+    )
+    def test_from_2d_transformation_checks_component_count(self, m44, components):
+        with pytest.raises(ValueError):
+            m44.from_2d_transformation(components)
+
 
 def test_has_matrix_2d_stretching():
     """Note: Uniform scaling is not stretching in this context."""
     assert has_matrix_2d_stretching(Matrix44.scale(1, 1, 1)) is False
     assert has_matrix_2d_stretching(Matrix44.scale(2, 2, 2)) is False
-    assert (
-        has_matrix_2d_stretching(Matrix44.scale(1, 1, 2)) is False
-    ), "ignore z-axis"
+    assert has_matrix_2d_stretching(Matrix44.scale(1, 1, 2)) is False, "ignore z-axis"
     assert has_matrix_2d_stretching(Matrix44.scale(2, 1, 1)) is True
     assert has_matrix_2d_stretching(Matrix44.scale(1, 2, 1)) is True
 
 
 def test_has_matrix_3d_stretching():
     """Note: Uniform scaling is not stretching in this context."""
     assert has_matrix_3d_stretching(Matrix44.scale(1, 1, 1)) is False
     assert has_matrix_3d_stretching(Matrix44.scale(2, 2, 2)) is False
     assert has_matrix_3d_stretching(Matrix44.scale(2, 1, 1)) is True
     assert has_matrix_3d_stretching(Matrix44.scale(1, 2, 1)) is True
     assert has_matrix_3d_stretching(Matrix44.scale(1, 1, 2)) is True
+
+
+class TestFast2dTransform:
+    def test_fast_translate(self, m44):
+        m = m44.translate(10, 20, 0)
+        points = list(m.fast_2d_transform([(0, 0), (1, 1, 1)]))
+        assert points[0].isclose((10, 20))
+        assert points[1].isclose((11, 21))
+
+    def test_fast_z_rotate(self, m44):
+        m = m44.z_rotate(radians(90))
+        points = list(m.fast_2d_transform([(10, 0), (0, 10, 1)]))
+        assert points[0].isclose((0, 10))
+        assert points[1].isclose((-10, 0))
+
+    def test_fast_scale(self, m44):
+        m = m44.scale(2, 3, 4)
+        points = list(m.fast_2d_transform([(10, 10), (-20, -20, 1)]))
+        assert points[0].isclose((20, 30))
+        assert points[1].isclose((-40, -60))
+
+    def test_fast_scale_rotate_translate(self, m44):
+        m = m44.scale(2, 3, 4) @ m44.z_rotate(radians(90)) @ m44.translate(10, 20, 0)
+        points = [(10, 10), (-20, -20, 1)]
+        res_3d = list(m.transform_vertices(points))
+        res_2d = list(m.fast_2d_transform(points))
+
+        assert res_2d[0].isclose(res_3d[0])
+        assert res_2d[1].isclose(res_3d[1])
```

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_606_convexhull.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_606_convexhull.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_607_perlin_noise.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_607_perlin_noise.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_608_intersection_line_line_2d.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_608_intersection_line_line_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_609_point_on_line.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_609_point_on_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_610_ocs.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_610_ocs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_611_ucs.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_611_ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_612_ucs_pass_trough.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_612_ucs_pass_trough.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_613_point_in_poygon.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_613_point_in_poygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_614_construct_3d.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_614_construct_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_615_rytz_axis.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_615_rytz_axis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_616_plane.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_616_plane.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_617_clockwise_orientation.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_617_clockwise_orientation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_618_clipping.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_618_clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_619_greiner_hormann.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_619_greiner_hormann.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_620_knot.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_620_knot.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_621_bspline.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_621_bspline.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,39 +508,14 @@
     Vec3(44.0, 6.000000000000001, 27.0),
     Vec3(46.0, 3.999999999999999, 28.0),
     Vec3(48.0, 2.0000000000000018, 28.999999999999996),
     Vec3(50.0, 0.0, 30.0),
 ]
 
 
-class TestNurbsPythonCorrectness:
-    # Test if package "geomdl" (a.k.a. NURBS Python) is still correct.
-    @pytest.mark.parametrize(
-        "order,results",
-        [
-            [2, POINTS_ORDER_2],
-            [3, POINTS_ORDER_3],
-            [4, POINTS_ORDER_4],
-        ],
-        ids=["degree=1", "degree=2", "degree=3"],
-    )
-    def test_point_calculation_is_correct(self, order, results):
-        curve = BSpline(DEFPOINTS, order=order).to_nurbs_python_curve()
-        points = curve.evaluate_list(PARAMS)
-        for expect, point in zip(results, points):
-            assert expect.isclose(point)
-
-    def test_derivative_calculation_is_correct(self):
-        spline = BSpline(DEFPOINTS, order=4).to_nurbs_python_curve()
-        for t, expected in zip(PARAMS, DERIVATIVES_ORDER_4):
-            results = spline.derivatives(t, order=2)
-            for e, p in zip(expected, results):
-                assert e.isclose(p)
-
-
 @pytest.mark.parametrize(
     "order,results",
     [
         [2, POINTS_ORDER_2],
         [3, POINTS_ORDER_3],
         [4, POINTS_ORDER_4],
     ],
```

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_622_bsplineu.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_622_bsplineu.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_623_rbspline.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_623_rbspline.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,39 +77,14 @@
     spline = rational_bspline_from_arc(
         start_angle=arc.start_angle, end_angle=arc.end_angle
     )
     assert arc.start_point.isclose(spline.control_points[0])
     assert arc.end_point.isclose(spline.control_points[-1])
 
 
-def test_rational_spline_curve_points_by_nurbs_python():
-    arc = ConstructionArc(end_angle=90)
-    spline = rational_bspline_from_arc(end_angle=arc.end_angle)
-    curve = spline.to_nurbs_python_curve()
-
-    t = list(linspace(0, 1, 10))
-    points = list(spline.points(t))
-    expected = list(curve.evaluate_list(t))
-    for p, e in zip(points, expected):
-        assert p.isclose(e)
-
-
-def test_rational_spline_derivatives_by_nurbs_python():
-    arc = ConstructionArc(end_angle=90)
-    spline = rational_bspline_from_arc(end_angle=arc.end_angle)
-    curve = spline.to_nurbs_python_curve()
-
-    t = list(linspace(0, 1, 10))
-    derivatives = list(spline.derivatives(t, n=1))
-    expected = [curve.derivatives(u, 1) for u in t]
-    for (p, d1), (e, ed1) in zip(derivatives, expected):
-        assert p.isclose(e)
-        assert d1.isclose(ed1)
-
-
 def test_rational_spline_from_elliptic_arc_has_expected_parameters():
     ellipse = ConstructionEllipse(
         center=(1, 1),
         major_axis=(2, 0),
         ratio=0.5,
         start_param=0,
         end_param=math.pi / 2,
```

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_624_global_bspline_interpolation.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_624_global_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_626_local_bspline_interpolation.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_626_local_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_627_bspline_basis.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_627_bspline_basis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_629_bezier.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_629_bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_630a_bezier4p_base.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_630a_bezier4p_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_630b_bezier4p_functions.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_630b_bezier4p_functions.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_631_euler_spiral.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_631_euler_spiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_632_bezier3p.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_632_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_640_bbox.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_640_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_641_construction_ray.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_641_construction_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_642_construction_line.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_642_construction_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_643_construction_box.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_643_construction_box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_644_construction_circle.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_644_construction_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_645_construction_arc.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_645_construction_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_646_offset_vertices_2d.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_646_offset_vertices_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_647_transform_tools.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_647_transform_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_648_construction_ellipse.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_648_construction_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_650_elliptic_arc_span.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_650_elliptic_arc_span.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_651_construction_polyline.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_651_construction_polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_652_approx_param_t.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_652_approx_param_t.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_653_polyline_intersection.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_653_polyline_intersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_654_rtree.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_654_rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_655_dbscan.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_655_dbscan.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_656_k_means.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_656_k_means.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_657_mapbox_earcut.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_657_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_658_bevel_tools.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_658_bevel_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_659_intersection_line_polygon_3d.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_659_intersection_line_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_660_intersection_ray_polygon_3d.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_660_intersection_ray_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_06_math/test_662_is_convex_polygon_2d.py` & `ezdxf-1.1.0b0/tests/test_06_math/test_662_is_convex_polygon_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_701_arrows.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_701_arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_702_render_forms.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_702_render_forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_703_mesh_builder.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_703_mesh_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_704_render_linear_dimension.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_704_render_linear_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_705_shape.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_705_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_707_trace.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_707_trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_708a_path.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_708a_path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_708b_path_tools.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_708b_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_708c_matplotlib_path_tools.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_708c_matplotlib_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_708d_qpainter_path_tools.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_708d_qpainter_path_tools.py`

 * *Files 26% similar despite different names*

```diff
@@ -90,63 +90,9 @@
         qpath = path.to_qpainter_path([p])
         assert qpath.elementCount() == 4
         assert qpath.elementAt(0).isMoveTo() is True
         assert qpath.elementAt(1).isLineTo() is True
         assert qpath.elementAt(2).isMoveTo() is True
         assert qpath.elementAt(3).isLineTo() is True
 
-
-@pytest.mark.skipif(
-    sys.version.startswith("3.11"),
-    reason="Does not work in CPython 3.11 and PySide6 6.4.0.1",
-    # But works in single step debug mode!
-)
-class TestFromQPainterPath:
-    def test_line_to(self):
-        qpath = QPainterPath(QPointF(1, 2))
-        qpath.lineTo(4, 5)
-
-        paths = list(path.from_qpainter_path(qpath))
-        p0 = paths[0]
-        assert p0.start == (1, 2)
-        assert p0[0].type == path.Command.LINE_TO
-        assert p0[0].end == (4, 5)
-
-    # Qt converts quadratic Bezier curves into cubic Bezier curves
-    # no need to test quadTo()
-    def test_cubic_to(self):
-        qpath = QPainterPath(QPointF(0, 0))
-        qpath.cubicTo(
-            QPointF(1, 1),
-            QPointF(3, 1),
-            QPointF(4, 0),
-        )
-
-        paths = list(path.from_qpainter_path(qpath))
-        p0 = paths[0]
-        assert p0.start == (0, 0)
-        assert p0[0].type == path.Command.CURVE4_TO
-        assert p0[0].ctrl1 == (1, 1)
-        assert p0[0].ctrl2 == (3, 1)
-        assert p0[0].end == (4, 0)
-
-    def test_two_lines(self):
-        qpath = QPainterPath(QPointF(1, 2))
-        qpath.lineTo(4, 5)
-        qpath.moveTo(3, 4)
-        qpath.lineTo(7, 9)
-        paths = list(path.from_qpainter_path(qpath))
-        assert len(paths) == 2
-
-        p0 = paths[0]
-        assert p0[0].type == path.Command.LINE_TO
-        assert p0.start == (1, 2)
-        assert p0[0].end == (4, 5)
-
-        p1 = paths[1]
-        assert p1[0].type == path.Command.LINE_TO
-        assert p1.start == (3, 4)
-        assert p1[0].end == (7, 9)
-
-
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_708e_path_shapes.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_708e_path_shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_708f_path_nesting.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_708f_path_nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_709_linetype_renderer.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_709_linetype_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_711_points.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_711_points.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_712_render_curved_dimension.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_712_render_curved_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_713_mleader_builder.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_713_mleader_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_714_mleader_render_engine.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_714_mleader_render_engine.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_715_hatching.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_715_hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_07_render/test_715_issue_747_explode_3d_dim.py` & `ezdxf-1.1.0b0/tests/test_07_render/test_715_issue_747_explode_3d_dim.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_800_mtext_surrogate.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_800_mtext_surrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_801_r12spline.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_801_r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_802_table_painter.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_802_table_painter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_803_entities_to_code.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_803_entities_to_code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_804_importer.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_804_importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_805_pycsg.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_805_pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_806_acadctb.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_806_acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_807_dwg_loader_basics.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_807_dwg_loader_basics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_810_drawing_properties.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_810_drawing_properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_811_drawing_frontend.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_811_drawing_frontend.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Copyright (c) 2020-2022, Manfred Moitzi
 # License: MIT License
-from typing import List, Set, Sequence
+
 import pytest
 import ezdxf
 from ezdxf.addons.drawing import Frontend, RenderContext
-from ezdxf.addons.drawing.properties import Properties, LayerProperties, set_layers_state
+from ezdxf.addons.drawing.properties import Properties
 
 from ezdxf.addons.drawing.backend import Backend
 from ezdxf.addons.drawing.debug_backend import BasicBackend, PathBackend
-from ezdxf.document import Drawing
 from ezdxf.entities import DXFGraphic
 from ezdxf.render.forms import cube
 from ezdxf.path import from_vertices
 
 
 @pytest.fixture
 def doc():
@@ -269,38 +268,38 @@
     path_backend.draw_entities(msp)
     result = path_backend.out.collector
     assert len(result) == 1
     assert unique_types(result) == {"path"}
 
 
 def test_2d_text(msp, basic):
+    # since v1.0.4 the frontend does the text rendering and passes only filled
+    # polygons to the backend
     msp.add_text("test\ntest")  # \n shouldn't be  problem. Will be ignored
     basic.draw_entities(msp)
     result = basic.out.collector
-    assert len(result) == 1
-    assert result[0][0] == "text"
-    assert result[0][1] == "testtest"
+    assert len(result) == 8
+    assert result[0][0] == "filled_polygon"
 
 
 def test_ignore_3d_text(msp, basic):
     msp.add_text("test", dxfattribs={"extrusion": (0, 1, 1)})
     basic.draw_entities(msp)
     result = basic.out.collector
     assert len(result) == 0
 
 
 def test_mtext(msp, basic):
+    # since v1.0.4 the frontend does the text rendering and passes only filled
+    # polygons to the backend
     msp.add_mtext("line1\nline2")
     basic.draw_entities(msp)
     result = basic.out.collector
-    assert len(result) == 2
-    assert result[0][0] == "text"
-    assert result[0][1] == "line1"
-    assert result[1][0] == "text"
-    assert result[1][1] == "line2"
+    assert len(result) == 12
+    assert result[0][0] == "filled_polygon"
 
 
 def test_hatch(msp, path_backend):
     hatch = msp.add_hatch()
     hatch.paths.add_polyline_path([(0, 0), (1, 0), (1, 1), (0, 1)])
     path_backend.draw_entities(msp)
     result = path_backend.out.collector
@@ -334,103 +333,14 @@
     basic.draw_entities(msp)
     result = basic.out.collector
     assert len(result) == 24
     entities = {e[0] for e in result}
     assert entities == {"line"}
 
 
-def _add_text_block(doc: Drawing):
-    doc.layers.new(name="Layer1")
-    doc.layers.new(name="Layer2")
-
-    text_block = doc.blocks.new(name="text-block")
-    text_block.add_text(
-        text="L0",
-        dxfattribs={
-            "layer": "0",
-            "insert": (0, 0, 0),
-            "height": 5.0,
-        },
-    )
-    text_block.add_text(
-        text="L1",
-        dxfattribs={
-            "layer": "Layer1",
-            "insert": (0, 0, 0),
-            "height": 5.0,
-        },
-    )
-
-
-def _get_text_visible_when(doc: Drawing, active_layers: Set[str]) -> List[str]:
-    def update_layers_state(layers: Sequence[LayerProperties]):
-        # set given layer to ON, others to OFF
-        set_layers_state(layers, active_layers, state=True)
-
-    ctx = RenderContext(doc)
-    ctx.set_layer_properties_override(update_layers_state)
-
-    backend = BasicBackend()
-    Frontend(ctx, backend).draw_layout(doc.modelspace())
-    visible_text = [x[1] for x in backend.collector if x[0] == "text"]
-    return visible_text
-
-
-def test_visibility_insert_0():
-    """see notes/drawing.md 'Layers and Draw Order'"""
-    doc = ezdxf.new()
-    _add_text_block(doc)
-    layout = doc.modelspace()
-    layout.add_blockref(
-        name="text-block",
-        insert=(0, 0, 0),
-        dxfattribs={"layer": "0"},
-    )
-    # INSERT on '0'
-    # 'L0' on '0'
-    # 'L1' on 'Layer1'
-    assert _get_text_visible_when(doc, {"0", "Layer1", "Layer2"}) == [
-        "L0",
-        "L1",
-    ]
-    assert _get_text_visible_when(doc, {"0", "Layer2"}) == ["L0"]
-    assert _get_text_visible_when(doc, {"0", "Layer1"}) == ["L0", "L1"]
-    assert _get_text_visible_when(doc, {"Layer1", "Layer2"}) == [
-        "L1"
-    ]  # result: []
-    assert _get_text_visible_when(doc, {"Layer2"}) == []
-    assert _get_text_visible_when(doc, {"Layer1"}) == ["L1"]  # result = []
-    assert _get_text_visible_when(doc, set()) == []
-
-
-def test_visibility_insert_2():
-    """see notes/drawing.md 'Layers and Draw Order'"""
-    doc = ezdxf.new()
-    _add_text_block(doc)
-    layout = doc.modelspace()
-    layout.add_blockref(
-        name="text-block",
-        insert=(0, 0, 0),
-        dxfattribs={"layer": "Layer2"},
-    )
-    # 'L0' on '0'
-    # 'L1' on 'Layer1'
-    # text-block on 'Layer2' -> 'L0' on '0' acts like on 'Layer2'
-    assert _get_text_visible_when(doc, {"0", "Layer1", "Layer2"}) == [
-        "L0",
-        "L1",
-    ]
-    assert _get_text_visible_when(doc, {"0", "Layer2"}) == ["L0"]
-    assert _get_text_visible_when(doc, {"0", "Layer1"}) == ["L1"]  # result = []
-    assert _get_text_visible_when(doc, {"Layer1", "Layer2"}) == ["L0", "L1"]
-    assert _get_text_visible_when(doc, {"Layer2"}) == ["L0"]
-    assert _get_text_visible_when(doc, {"Layer1"}) == ["L1"]  # result = []
-    assert _get_text_visible_when(doc, set()) == []
-
-
 def test_override_filter(msp, ctx):
     class FrontendWithOverride(Frontend):
         def __init__(self, ctx: RenderContext, out: Backend):
             super().__init__(ctx, out)
             self.override_enabled = True
 
         def override_properties(
@@ -451,41 +361,38 @@
     msp.add_text("T0", dxfattribs={"layer": "T0", "color": 7})
     msp.add_text("T1", dxfattribs={"layer": "T1", "color": 6})
     msp.add_text("T2", dxfattribs={"layer": "T2", "color": 5})
     frontend.draw_entities(msp)
     frontend.override_enabled = False
     frontend.draw_entities(msp)
 
-    assert len(backend.collector) == 5
+    # since v1.0.4 the frontend does the text rendering and passes only filled
+    # polygons to the backend
+    assert len(backend.collector) == 10
 
     # can modify color property
     result = backend.collector[0]
-    assert result[0] == "text"
-    assert result[1] == "T0"
-    assert result[3].color == "#000000"
+    assert result[0] == "filled_polygon"
+    assert result[2].color == "#000000"
 
     # can modify layer property
-    result = backend.collector[1]
-    assert result[0] == "text"
-    assert result[1] == "T1"
-    assert result[3].layer == "Tx"
+    result = backend.collector[2]
+    assert result[0] == "filled_polygon"
+    assert result[2].layer == "Tx"
 
     # with override disabled
 
-    result = backend.collector[2]
-    assert result[0] == "text"
-    assert result[1] == "T0"
-    assert result[3].color == "#ffffff"
-
-    result = backend.collector[3]
-    assert result[0] == "text"
-    assert result[1] == "T1"
-    assert result[3].layer == "T1"
-
     result = backend.collector[4]
-    assert result[0] == "text"
-    assert result[1] == "T2"
-    assert result[3].layer == "T2"
+    assert result[0] == "filled_polygon"
+    assert result[2].color == "#ffffff"
+
+    result = backend.collector[6]
+    assert result[0] == "filled_polygon"
+    assert result[2].layer == "T1"
+
+    result = backend.collector[8]
+    assert result[0] == "filled_polygon"
+    assert result[2].layer == "T2"
 
 
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_812_drawing_graphic_proxy.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_812_drawing_graphic_proxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_813_geo_interface.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_813_geo_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_814_text2path.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_814_text2path.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,73 @@
-#  Copyright (c) 2021, Manfred Moitzi
+#  Copyright (c) 2021-2023, Manfred Moitzi
 #  License: MIT License
 
 import pytest
+import platform
 
-pytest.importorskip("matplotlib")  # requires matplotlib!
+if platform.system() != "Windows":
+    pytest.skip(
+        reason="works for some reasons only on Windows", allow_module_level=True
+    )
+# These test do not work on my Linux Mint system.
+# The test file fails when started as a whole session, but passes if I start
+# failing test classes individually by the PyCharm debugger.
+# The problem is the font_manager:
+# When started as single test class or in debugger mode the repo fonts are loaded as it
+# should be. Started as normal session the system fonts are loaded, which shouldn't be
+# possible - I guess there is some pytest magic happening in the background which messes
+# things up.
+# On Windows everything works fine, so the module works as expected.
 
-from matplotlib.font_manager import FontProperties, findfont
-from ezdxf.tools.fonts import FontFace
+from ezdxf.tools.font_face import FontFace
 from ezdxf.addons import text2path
 from ezdxf.path import Path
 from ezdxf import path, bbox
 from ezdxf.entities import Text, Hatch
 from ezdxf.layouts import VirtualLayout
 from ezdxf.enums import TextEntityAlignment
 
-NOTO_SANS_SC = "Noto Sans SC"
-noto_sans_sc_not_found = (
-    "noto" not in findfont(FontProperties(family=NOTO_SANS_SC)).lower()
-)
-arial_not_found = (
-    "arial" not in findfont(FontProperties(family="Arial")).lower()
-)
+# always available in common test scenarios:
+DEFAULT = "LiberationSans-Regular.ttf"
+NOTO_SANS_SC = "NotoSansSC-Regular.otf"
 
 
-def _to_paths(s, f="Arial"):
-    return text2path.make_paths_from_str(s, font=FontFace(family=f))
+def _to_paths(s, f=DEFAULT):
+    return text2path.make_paths_from_str(s, font=FontFace(ttf=f))
 
 
 # Font 'Arial' required, a replacement fonts may return a different
 # path/hole configuration! issue #515
-if arial_not_found:
-    CHAR_TO_PATH = [
-        ["1", 1],
-        ["2", 1],
-        [".", 1],
-        ["0", 2],
-        ["a", 2],
-        ["!", 2],
-        ["@", 2],
-        ["8", 3],
-        ["ü", 3],
-    ]
-else:
-    CHAR_TO_PATH = [
-        ["1", 1],
-        ["2", 1],
-        [".", 1],
-        ["0", 2],
-        ["a", 2],
-        ["!", 2],
-        ["@", 2],
-        ["8", 3],
-        ["ü", 3],
-        ["&", 3],
-        ["ä", 4],
-        ["ö", 4],
-        ["%", 5],
-    ]
+CHAR_TO_PATH = [
+    ["1", 1],
+    ["2", 1],
+    [".", 1],
+    ["0", 2],
+    ["a", 2],
+    ["!", 2],
+    ["@", 2],
+    ["8", 3],
+    ["ü", 3],
+    ["&", 3],
+    ["ä", 4],
+    ["ö", 4],
+    ["%", 5],
+]
 
 
 @pytest.mark.parametrize("s,c", CHAR_TO_PATH)
 def test_make_paths_from_str(s: str, c: int):
     # change of assertion from == to >= is based on an error on RPi & Ubuntu
     # Server 21.10 & matplotlib
     # assert len(_to_paths("ü")) == 4  instead of 3
     # Do not test how matplotlib works here, the only important fact is:
     # do we get path objects
     assert len(_to_paths(s)) >= c
 
 
-@pytest.mark.skipif(
-    noto_sans_sc_not_found, reason=f'Font "{NOTO_SANS_SC}" not found'
-)
 @pytest.mark.parametrize("s,c", [["中", 3], ["国", 4], ["文", 3], ["字", 2]])
 def test_chinese_char_paths_from_str(s, c):
     assert len(_to_paths(s, f=NOTO_SANS_SC)) == c
 
 
 def contour_and_holes(group):
     return group[0], group[1:]
@@ -122,45 +114,26 @@
     paths = _to_paths(s)
     result = list(path.group_paths(paths))
     assert len(result) == 3
     contour, holes = contour_and_holes(result[0])
     assert isinstance(contour, Path)
 
 
-@pytest.mark.skipif(
-    arial_not_found,
-    reason="Font 'Arial' required, a replacement fonts may return different "
-    "paths, issue #515",
-)
-def test_group_percent_sign():
-    # Special case %: lower o is inside of the slash bounding box, but HATCH
-    # creation works as expected!
-    paths = _to_paths("%")
-    result = list(path.group_paths(paths))
-    assert len(result) == 2
-    contour, holes = contour_and_holes(result[0])
-    assert isinstance(contour, Path)
-    assert len(holes) == 2
-
-
-@pytest.mark.skipif(
-    noto_sans_sc_not_found, reason='Font "Noto Sans SC" not found'
-)
 @pytest.mark.parametrize("s,c", [["中", 1], ["国", 1], ["文", 2], ["字", 2]])
 def test_group_chinese_chars_and_ignore_holes(s, c):
     paths = _to_paths(s, f=NOTO_SANS_SC)
     result = list(path.group_paths(paths))
     assert len(result) == c
     contour, holes = contour_and_holes(result[0])
     assert isinstance(contour, Path)
 
 
 @pytest.fixture(scope="module")
 def ff():
-    return FontFace(family="Arial")
+    return FontFace(family=DEFAULT)
 
 
 class TestMakePathFromString:
     # Surprise - even 0 and negative values work without any exceptions!
     @pytest.mark.parametrize("size", [0, 0.05, 1, 2, 100, -1, -2, -100])
     def test_text_path_height_for_exact_drawing_units(self, size, ff):
         paths = text2path.make_paths_from_str("X", font=ff, size=size)
@@ -190,17 +163,15 @@
             font=ff,
             size=size,
             align=TextEntityAlignment.FIT,
             length=length,
         )
         bbox = path.bbox(paths)
         assert bbox.size.x == pytest.approx(length), "expect exact length"
-        assert bbox.size.y == pytest.approx(
-            size
-        ), "text height should be unscaled"
+        assert bbox.size.y == pytest.approx(size), "text height should be unscaled"
 
     @pytest.mark.parametrize("size", [0.05, 1, 2, 100])
     def test_scaled_height_and_length_for_aligned_text(self, size, ff):
         length = 3
         paths = text2path.make_paths_from_str(
             "XXX", font=ff, size=size, align=TextEntityAlignment.LEFT
         )
@@ -255,17 +226,15 @@
             "XXX", font=ff, align=TextEntityAlignment.FIT, length=length
         )
         paths = []
         for hatch in hatches:
             paths.extend(path.from_hatch(hatch))
         bbox = path.bbox(paths)
         assert bbox.size.x == pytest.approx(length), "expect exact length"
-        assert bbox.size.y == pytest.approx(
-            1.0
-        ), "text height should be unscaled"
+        assert bbox.size.y == pytest.approx(1.0), "text height should be unscaled"
 
 
 def test_check_entity_type():
     with pytest.raises(TypeError):
         text2path.check_entity_type(None)
     with pytest.raises(TypeError):
         text2path.check_entity_type(Hatch())
@@ -370,42 +339,32 @@
         text = make_text("X", (7, 7), TextEntityAlignment.TOP_CENTER)
         bbox = get_bbox(text)
         assert bbox.extmax.y == pytest.approx(7)
 
     def test_alignment_fit(self, get_bbox):
         length = 2
         height = 1
-        text = make_text(
-            "TEXT", (0, 0), TextEntityAlignment.LEFT, height=height
-        )
+        text = make_text("TEXT", (0, 0), TextEntityAlignment.LEFT, height=height)
         text.set_placement((1, 0), (1 + length, 0), TextEntityAlignment.FIT)
         bbox = get_bbox(text)
-        assert (
-            bbox.size.x == length
-        ), "expected text length fits into given length"
-        assert bbox.size.y == pytest.approx(
-            height
-        ), "expected unscaled text height"
+        assert bbox.size.x == length, "expected text length fits into given length"
+        assert bbox.size.y == pytest.approx(height), "expected unscaled text height"
         assert bbox.extmin.isclose((1, 0))
 
     def test_alignment_aligned(self, get_bbox):
         length = 2
         height = 1
-        text = make_text(
-            "TEXT", (0, 0), TextEntityAlignment.CENTER, height=height
-        )
+        text = make_text("TEXT", (0, 0), TextEntityAlignment.CENTER, height=height)
         bbox = get_bbox(text)
         ratio = bbox.size.x / bbox.size.y
 
         text.set_placement((1, 0), (1 + length, 0), TextEntityAlignment.ALIGNED)
         bbox = get_bbox(text)
 
-        assert (
-            bbox.size.x == length
-        ), "expected text length fits into given length"
+        assert bbox.size.x == length, "expected text length fits into given length"
         assert bbox.size.y != height, "expected scaled text height"
         assert bbox.extmin.isclose((1, 0))
         assert bbox.size.x / bbox.size.y == pytest.approx(
             ratio
         ), "expected same width/height ratio"
 
     def test_rotation_90(self, get_bbox):
@@ -460,28 +419,24 @@
     @pytest.fixture
     def text(self):
         return make_text("TEST", (0, 0), TextEntityAlignment.LEFT)
 
     def test_source_entity_is_destroyed(self, text):
         assert text.is_alive is True
         text2path.explode(text, kind=4)
-        assert (
-            text.is_alive is False
-        ), "source entity should always be destroyed"
+        assert text.is_alive is False, "source entity should always be destroyed"
 
     def test_explode_entity_into_layout(self, text):
         layout = VirtualLayout()
         entities = text2path.explode(text, kind=Kind.LWPOLYLINES, target=layout)
         assert len(entities) == len(
             layout
         ), "expected all entities added to the target layout"
 
     def test_explode_entity_into_the_void(self, text):
-        assert (
-            text.get_layout() is None
-        ), "source entity should not have a layout"
+        assert text.get_layout() is None, "source entity should not have a layout"
         entities = text2path.explode(text, kind=Kind.LWPOLYLINES, target=None)
         assert len(entities) == 4, "explode should work without a target layout"
 
 
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_815_dxf_browser.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_815_dxf_browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_816_bin_packing.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_816_bin_packing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_817_genetic_algorithm.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_817_genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_818_meshex.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_818_meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_819_menger_sponge.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_819_menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_820_openscad.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_820_openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_821_hpgl2.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_821_hpgl2.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,441 +520,452 @@
 00002070: 5d2e 6e61 6d65 203d 3d20 2253 5022 0d0a  ].name == "SP"..
 00002080: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
 00002090: 6573 756c 745b 315d 2e61 7267 735b 305d  esult[1].args[0]
 000020a0: 203d 3d20 6222 3022 0d0a 2020 2020 2020   == b"0"..      
 000020b0: 2020 6173 7365 7274 2072 6573 756c 745b    assert result[
 000020c0: 325d 2e6e 616d 6520 3d3d 2022 5047 220d  2].name == "PG".
 000020d0: 0a0d 0a20 2020 2064 6566 2074 6573 745f  ...    def test_
-000020e0: 6e6f 5f68 7067 6c32 5f64 6174 6128 7365  no_hpgl2_data(se
-000020f0: 6c66 293a 0d0a 2020 2020 2020 2020 2320  lf):..        # 
-00002100: 4563 6170 6520 7365 7175 656e 6365 2074  Ecape sequence t
-00002110: 6f20 656e 7465 7220 4850 474c 3220 6d6f  o enter HPGL2 mo
-00002120: 6465 2069 7320 6d69 7373 696e 673a 2020  de is missing:  
-00002130: 221b 2531 4222 0d0a 2020 2020 2020 2020  ".%1B"..        
-00002140: 6173 7365 7274 206c 656e 2873 656c 662e  assert len(self.
-00002150: 7061 7273 6528 6222 414e 5954 4558 543b  parse(b"ANYTEXT;
-00002160: 494e 3b42 503b 2229 2920 3d3d 2030 0d0a  IN;BP;")) == 0..
-00002170: 0d0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-00002180: 726b 2e70 6172 616d 6574 7269 7a65 2822  rk.parametrize("
-00002190: 6222 2c20 5b0d 0a20 2020 2020 2020 2062  b", [..        b
-000021a0: 224c 4220 4d59 206c 6162 656c 2003 5041  "LB MY label .PA
-000021b0: 3338 312c 3053 4930 2e31 3235 2c30 2e32  381,0SI0.125,0.2
-000021c0: 3544 4930 2c31 3b22 2c0d 0a20 2020 2020  5DI0,1;",..     
-000021d0: 2020 2062 224c 424d 5920 6c61 6265 6c20     b"LBMY label 
-000021e0: 0350 4133 3831 2c30 5349 302e 3132 352c  .PA381,0SI0.125,
-000021f0: 302e 3235 4449 302c 313b 220d 0a20 2020  0.25DI0,1;"..   
-00002200: 205d 290d 0a20 2020 2064 6566 2074 6573   ])..    def tes
-00002210: 745f 6c61 6265 6c5f 7769 7468 5f74 6572  t_label_with_ter
-00002220: 6d69 6e61 746f 7228 7365 6c66 2c20 6229  minator(self, b)
-00002230: 3a0d 0a20 2020 2020 2020 2063 6f6d 6d61  :..        comma
-00002240: 6e64 7320 3d20 7365 6c66 2e70 6172 7365  nds = self.parse
-00002250: 2868 7067 6c32 2862 2929 0d0a 2020 2020  (hpgl2(b))..    
-00002260: 2020 2020 6173 7365 7274 206c 656e 2863      assert len(c
-00002270: 6f6d 6d61 6e64 7329 203d 3d20 340d 0a0d  ommands) == 4...
-00002280: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-00002290: 6b2e 7061 7261 6d65 7472 697a 6528 0d0a  k.parametrize(..
-000022a0: 2020 2020 2020 2020 2262 222c 0d0a 2020          "b",..  
-000022b0: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
-000022c0: 2020 2020 2062 2244 545c 3034 4c42 2054       b"DT\04LB T
-000022d0: 7565 2044 6563 2031 3820 3136 3a32 303a  ue Dec 18 16:20:
-000022e0: 3035 2032 3030 3120 5c30 3450 4133 3831  05 2001 \04PA381
-000022f0: 2c30 5349 302e 3132 352c 302e 3235 4449  ,0SI0.125,0.25DI
-00002300: 302c 313b 222c 0d0a 2020 2020 2020 2020  0,1;",..        
-00002310: 2020 2020 6222 4454 5c30 342c 304c 4220      b"DT\04,0LB 
-00002320: 5475 6520 4465 6320 3138 2031 363a 3230  Tue Dec 18 16:20
-00002330: 3a30 3520 3230 3031 205c 3034 5041 3338  :05 2001 \04PA38
-00002340: 312c 3053 4930 2e31 3235 2c30 2e32 3544  1,0SI0.125,0.25D
-00002350: 4930 2c31 3b22 2c0d 0a20 2020 2020 2020  I0,1;",..       
-00002360: 2020 2020 2062 2244 545c 3034 2c31 3b4c       b"DT\04,1;L
-00002370: 4220 5475 6520 4465 6320 3138 2031 363a  B Tue Dec 18 16:
-00002380: 3230 3a30 3520 3230 3031 205c 3034 5041  20:05 2001 \04PA
-00002390: 3338 312c 3053 4930 2e31 3235 2c30 2e32  381,0SI0.125,0.2
-000023a0: 3544 4930 2c31 3b22 2c0d 0a20 2020 2020  5DI0,1;",..     
-000023b0: 2020 205d 2c0d 0a20 2020 2029 0d0a 2020     ],..    )..  
-000023c0: 2020 6465 6620 7465 7374 5f6c 6162 656c    def test_label
-000023d0: 5f77 6974 685f 6375 7374 6f6d 5f74 6572  _with_custom_ter
-000023e0: 6d69 6e61 746f 7228 7365 6c66 2c20 6229  minator(self, b)
-000023f0: 3a0d 0a20 2020 2020 2020 2063 6f6d 6d61  :..        comma
-00002400: 6e64 7320 3d20 7365 6c66 2e70 6172 7365  nds = self.parse
-00002410: 2868 7067 6c32 2862 2929 0d0a 2020 2020  (hpgl2(b))..    
-00002420: 2020 2020 6173 7365 7274 206c 656e 2863      assert len(c
-00002430: 6f6d 6d61 6e64 7329 203d 3d20 340d 0a0d  ommands) == 4...
-00002440: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-00002450: 6b2e 7061 7261 6d65 7472 697a 6528 0d0a  k.parametrize(..
-00002460: 2020 2020 2020 2020 2262 222c 0d0a 2020          "b",..  
-00002470: 2020 2020 2020 5b0d 0a20 2020 2020 2020        [..       
-00002480: 2020 2020 2062 2244 545c 3034 4c42 204d       b"DT\04LB M
-00002490: 5920 6c61 6265 6c5c 3034 4454 4c42 204d  Y label\04DTLB M
-000024a0: 7920 6f74 6865 7220 6c61 6265 6c20 0322  y other label ."
-000024b0: 2c0d 0a20 2020 2020 2020 2020 2020 2062  ,..            b
-000024c0: 2244 545c 3034 4c42 204d 5920 6c61 6265  "DT\04LB MY labe
-000024d0: 6c5c 3034 4454 3b4c 4220 4d79 206f 7468  l\04DT;LB My oth
-000024e0: 6572 206c 6162 656c 2003 222c 0d0a 2020  er label .",..  
-000024f0: 2020 2020 2020 5d2c 0d0a 2020 2020 290d        ],..    ).
-00002500: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
-00002510: 7365 745f 6375 7374 6f6d 5f74 6572 6d69  set_custom_termi
-00002520: 6e61 746f 7228 7365 6c66 2c20 6229 3a0d  nator(self, b):.
-00002530: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
-00002540: 7320 3d20 7365 6c66 2e70 6172 7365 2868  s = self.parse(h
-00002550: 7067 6c32 2862 2929 0d0a 2020 2020 2020  pgl2(b))..      
-00002560: 2020 6173 7365 7274 206c 656e 2863 6f6d    assert len(com
-00002570: 6d61 6e64 7329 203d 3d20 320d 0a0d 0a0d  mands) == 2.....
-00002580: 0a63 6c61 7373 2054 6573 7450 6167 6543  .class TestPageC
-00002590: 6f6f 7264 696e 6174 6573 3a0d 0a20 2020  oordinates:..   
-000025a0: 2040 7079 7465 7374 2e66 6978 7475 7265   @pytest.fixture
-000025b0: 2873 636f 7065 3d22 636c 6173 7322 290d  (scope="class").
-000025c0: 0a20 2020 2064 6566 2070 6167 6528 7365  .    def page(se
-000025d0: 6c66 293a 0d0a 2020 2020 2020 2020 7061  lf):..        pa
-000025e0: 6765 5f20 3d20 5061 6765 2831 3030 302c  ge_ = Page(1000,
-000025f0: 2031 3030 3029 0d0a 2020 2020 2020 2020   1000)..        
-00002600: 7061 6765 5f2e 7365 745f 7563 7328 5665  page_.set_ucs(Ve
-00002610: 6332 2835 3030 2c20 3530 3029 2c20 7378  c2(500, 500), sx
-00002620: 3d32 2c20 7379 3d33 290d 0a20 2020 2020  =2, sy=3)..     
-00002630: 2020 2072 6574 7572 6e20 7061 6765 5f0d     return page_.
-00002640: 0a0d 0a20 2020 2064 6566 2074 6573 745f  ...    def test_
-00002650: 7573 6572 5f74 6f5f 7061 6765 5f63 6f6f  user_to_page_coo
-00002660: 7264 696e 6174 6573 2873 656c 662c 2070  rdinates(self, p
-00002670: 6167 6529 3a0d 0a20 2020 2020 2020 2061  age):..        a
-00002680: 7373 6572 7420 7061 6765 2e70 6167 655f  ssert page.page_
-00002690: 706f 696e 7428 302c 2030 292e 6973 636c  point(0, 0).iscl
-000026a0: 6f73 6528 2835 3030 2c20 3530 3029 290d  ose((500, 500)).
-000026b0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000026c0: 7061 6765 2e70 6167 655f 706f 696e 7428  page.page_point(
-000026d0: 3130 2c20 3130 292e 6973 636c 6f73 6528  10, 10).isclose(
-000026e0: 2835 3230 2c20 3533 3029 290d 0a0d 0a20  (520, 530)).... 
-000026f0: 2020 2064 6566 2074 6573 745f 7573 6572     def test_user
-00002700: 5f76 6563 746f 725f 746f 5f70 6167 655f  _vector_to_page_
-00002710: 7665 6374 6f72 2873 656c 662c 2070 6167  vector(self, pag
-00002720: 6529 3a0d 0a20 2020 2020 2020 2061 7373  e):..        ass
-00002730: 6572 7420 7061 6765 2e70 6167 655f 7665  ert page.page_ve
-00002740: 6374 6f72 2830 2c20 3029 2e69 7363 6c6f  ctor(0, 0).isclo
-00002750: 7365 2828 302c 2030 2929 0d0a 2020 2020  se((0, 0))..    
-00002760: 2020 2020 6173 7365 7274 2070 6167 652e      assert page.
-00002770: 7061 6765 5f76 6563 746f 7228 3130 2c20  page_vector(10, 
-00002780: 3130 292e 6973 636c 6f73 6528 2832 302c  10).isclose((20,
-00002790: 2033 3029 290d 0a0d 0a0d 0a63 6c61 7373   30))......class
-000027a0: 2054 6573 7450 6167 6541 6e69 736f 7472   TestPageAnisotr
-000027b0: 6f70 6963 5363 616c 696e 673a 0d0a 2020  opicScaling:..  
-000027c0: 2020 6465 6620 7465 7374 5f69 736f 7472    def test_isotr
-000027d0: 6f70 6963 5f73 6361 6c69 6e67 2873 656c  opic_scaling(sel
-000027e0: 6629 3a0d 0a20 2020 2020 2020 2070 6167  f):..        pag
-000027f0: 6520 3d20 5061 6765 2831 3030 302c 2031  e = Page(1000, 1
-00002800: 3030 3029 0d0a 2020 2020 2020 2020 7061  000)..        pa
-00002810: 6765 2e73 6574 5f73 6361 6c69 6e67 5f70  ge.set_scaling_p
-00002820: 6f69 6e74 7328 5665 6332 2831 3030 2c20  oints(Vec2(100, 
-00002830: 3130 3029 2c20 5665 6332 2832 3030 2c20  100), Vec2(200, 
-00002840: 3230 3029 290d 0a20 2020 2020 2020 2070  200))..        p
-00002850: 6167 652e 7365 745f 616e 6973 6f74 726f  age.set_anisotro
-00002860: 7069 635f 7363 616c 696e 6728 2d31 302c  pic_scaling(-10,
-00002870: 2031 302c 202d 3130 2c20 3130 290d 0a20   10, -10, 10).. 
-00002880: 2020 2020 2020 2061 7373 6572 7420 7061         assert pa
-00002890: 6765 2e75 7365 725f 7363 616c 696e 6720  ge.user_scaling 
-000028a0: 6973 2054 7275 650d 0a20 2020 2020 2020  is True..       
-000028b0: 2061 7373 6572 7420 7061 6765 2e70 6167   assert page.pag
-000028c0: 655f 706f 696e 7428 302c 2030 292e 6973  e_point(0, 0).is
-000028d0: 636c 6f73 6528 2831 3530 2c20 3135 3029  close((150, 150)
-000028e0: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-000028f0: 7420 7061 6765 2e70 6167 655f 706f 696e  t page.page_poin
-00002900: 7428 2d31 302c 202d 3130 292e 6973 636c  t(-10, -10).iscl
-00002910: 6f73 6528 2831 3030 2c20 3130 3029 290d  ose((100, 100)).
-00002920: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00002930: 7061 6765 2e70 6167 655f 706f 696e 7428  page.page_point(
-00002940: 3130 2c20 3130 292e 6973 636c 6f73 6528  10, 10).isclose(
-00002950: 2832 3030 2c20 3230 3029 290d 0a0d 0a20  (200, 200)).... 
-00002960: 2020 2064 6566 2074 6573 745f 616e 6973     def test_anis
-00002970: 6f74 726f 7069 635f 7363 616c 696e 6728  otropic_scaling(
-00002980: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00002990: 7061 6765 203d 2050 6167 6528 3130 3030  page = Page(1000
-000029a0: 2c20 3130 3030 290d 0a20 2020 2020 2020  , 1000)..       
-000029b0: 2070 6167 652e 7365 745f 7363 616c 696e   page.set_scalin
-000029c0: 675f 706f 696e 7473 2856 6563 3228 3130  g_points(Vec2(10
-000029d0: 302c 2031 3030 292c 2056 6563 3228 3230  0, 100), Vec2(20
-000029e0: 302c 2032 3030 2929 0d0a 2020 2020 2020  0, 200))..      
-000029f0: 2020 7061 6765 2e73 6574 5f61 6e69 736f    page.set_aniso
-00002a00: 7472 6f70 6963 5f73 6361 6c69 6e67 282d  tropic_scaling(-
-00002a10: 3130 2c20 3130 2c20 2d32 302c 2032 3029  10, 10, -20, 20)
-00002a20: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-00002a30: 2070 6167 652e 7573 6572 5f73 6361 6c69   page.user_scali
-00002a40: 6e67 2069 7320 5472 7565 0d0a 2020 2020  ng is True..    
-00002a50: 2020 2020 6173 7365 7274 2070 6167 652e      assert page.
-00002a60: 7061 6765 5f70 6f69 6e74 2830 2c20 3029  page_point(0, 0)
-00002a70: 2e69 7363 6c6f 7365 2828 3135 302c 2031  .isclose((150, 1
-00002a80: 3530 2929 0d0a 2020 2020 2020 2020 6173  50))..        as
-00002a90: 7365 7274 2070 6167 652e 7061 6765 5f70  sert page.page_p
-00002aa0: 6f69 6e74 282d 3130 2c20 2d32 3029 2e69  oint(-10, -20).i
-00002ab0: 7363 6c6f 7365 2828 3130 302c 2031 3030  sclose((100, 100
-00002ac0: 2929 0d0a 2020 2020 2020 2020 6173 7365  ))..        asse
-00002ad0: 7274 2070 6167 652e 7061 6765 5f70 6f69  rt page.page_poi
-00002ae0: 6e74 2831 302c 2032 3029 2e69 7363 6c6f  nt(10, 20).isclo
-00002af0: 7365 2828 3230 302c 2032 3030 2929 0d0a  se((200, 200))..
-00002b00: 0d0a 2020 2020 6465 6620 7465 7374 5f72  ..    def test_r
-00002b10: 6576 6572 7365 5f61 6e69 736f 7472 6f70  everse_anisotrop
-00002b20: 6963 5f73 6361 6c69 6e67 2873 656c 6629  ic_scaling(self)
-00002b30: 3a0d 0a20 2020 2020 2020 2070 6167 6520  :..        page 
-00002b40: 3d20 5061 6765 2831 3030 302c 2031 3030  = Page(1000, 100
-00002b50: 3029 0d0a 2020 2020 2020 2020 7061 6765  0)..        page
-00002b60: 2e73 6574 5f73 6361 6c69 6e67 5f70 6f69  .set_scaling_poi
-00002b70: 6e74 7328 5665 6332 2831 3030 2c20 3130  nts(Vec2(100, 10
-00002b80: 3029 2c20 5665 6332 2832 3030 2c20 3230  0), Vec2(200, 20
-00002b90: 3029 290d 0a20 2020 2020 2020 2023 2072  0))..        # r
-00002ba0: 6576 6572 7365 2078 2061 6e64 2079 2061  everse x and y a
-00002bb0: 7869 733a 0d0a 2020 2020 2020 2020 7061  xis:..        pa
-00002bc0: 6765 2e73 6574 5f61 6e69 736f 7472 6f70  ge.set_anisotrop
-00002bd0: 6963 5f73 6361 6c69 6e67 2831 302c 202d  ic_scaling(10, -
-00002be0: 3130 2c20 3230 2c20 2d32 3029 0d0a 2020  10, 20, -20)..  
-00002bf0: 2020 2020 2020 6173 7365 7274 2070 6167        assert pag
-00002c00: 652e 7573 6572 5f73 6361 6c69 6e67 2069  e.user_scaling i
-00002c10: 7320 5472 7565 0d0a 2020 2020 2020 2020  s True..        
-00002c20: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
-00002c30: 5f70 6f69 6e74 2830 2c20 3029 2e69 7363  _point(0, 0).isc
-00002c40: 6c6f 7365 2828 3135 302c 2031 3530 2929  lose((150, 150))
-00002c50: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-00002c60: 2070 6167 652e 7061 6765 5f70 6f69 6e74   page.page_point
-00002c70: 2831 302c 2032 3029 2e69 7363 6c6f 7365  (10, 20).isclose
-00002c80: 2828 3130 302c 2031 3030 2929 0d0a 2020  ((100, 100))..  
-00002c90: 2020 2020 2020 6173 7365 7274 2070 6167        assert pag
-00002ca0: 652e 7061 6765 5f70 6f69 6e74 282d 3130  e.page_point(-10
-00002cb0: 2c20 2d32 3029 2e69 7363 6c6f 7365 2828  , -20).isclose((
-00002cc0: 3230 302c 2032 3030 2929 0d0a 0d0a 0d0a  200, 200))......
-00002cd0: 636c 6173 7320 5465 7374 5061 6765 4973  class TestPageIs
-00002ce0: 6f74 726f 7069 6353 6361 6c69 6e67 3a0d  otropicScaling:.
-00002cf0: 0a20 2020 2064 6566 2074 6573 745f 6973  .    def test_is
-00002d00: 6f74 726f 7069 635f 626f 7474 6f6d 5f77  otropic_bottom_w
-00002d10: 696e 646f 775f 3530 2873 656c 6629 3a0d  indow_50(self):.
-00002d20: 0a20 2020 2020 2020 2070 6167 6520 3d20  .        page = 
-00002d30: 5061 6765 2831 3030 302c 2031 3030 3029  Page(1000, 1000)
-00002d40: 0d0a 2020 2020 2020 2020 7061 6765 2e73  ..        page.s
-00002d50: 6574 5f73 6361 6c69 6e67 5f70 6f69 6e74  et_scaling_point
-00002d60: 7328 5665 6332 2831 3030 2c20 3130 3029  s(Vec2(100, 100)
-00002d70: 2c20 5665 6332 2832 3030 2c20 3230 3029  , Vec2(200, 200)
-00002d80: 290d 0a20 2020 2020 2020 2070 6167 652e  )..        page.
-00002d90: 7365 745f 6973 6f74 726f 7069 635f 7363  set_isotropic_sc
-00002da0: 616c 696e 6728 302c 2032 302c 2030 2c20  aling(0, 20, 0, 
-00002db0: 3130 290d 0a20 2020 2020 2020 2061 7373  10)..        ass
-00002dc0: 6572 7420 7061 6765 2e75 7365 725f 7363  ert page.user_sc
-00002dd0: 616c 696e 6720 6973 2054 7275 650d 0a20  aling is True.. 
-00002de0: 2020 2020 2020 2061 7373 6572 7420 7061         assert pa
-00002df0: 6765 2e70 6167 655f 706f 696e 7428 302c  ge.page_point(0,
-00002e00: 2030 292e 6973 636c 6f73 6528 2831 3030   0).isclose((100
-00002e10: 2c20 3132 3529 290d 0a20 2020 2020 2020  , 125))..       
-00002e20: 2061 7373 6572 7420 7061 6765 2e70 6167   assert page.pag
-00002e30: 655f 706f 696e 7428 3130 2c20 3529 2e69  e_point(10, 5).i
-00002e40: 7363 6c6f 7365 2828 3135 302c 2031 3530  sclose((150, 150
-00002e50: 2929 0d0a 2020 2020 2020 2020 6173 7365  ))..        asse
-00002e60: 7274 2070 6167 652e 7061 6765 5f70 6f69  rt page.page_poi
-00002e70: 6e74 2832 302c 2031 3029 2e69 7363 6c6f  nt(20, 10).isclo
-00002e80: 7365 2828 3230 302c 2031 3735 2929 0d0a  se((200, 175))..
-00002e90: 0d0a 2020 2020 6465 6620 7465 7374 5f69  ..    def test_i
-00002ea0: 736f 7472 6f70 6963 5f62 6f74 746f 6d5f  sotropic_bottom_
-00002eb0: 7769 6e64 6f77 5f30 2873 656c 6629 3a0d  window_0(self):.
-00002ec0: 0a20 2020 2020 2020 2070 6167 6520 3d20  .        page = 
-00002ed0: 5061 6765 2831 3030 302c 2031 3030 3029  Page(1000, 1000)
-00002ee0: 0d0a 2020 2020 2020 2020 7061 6765 2e73  ..        page.s
-00002ef0: 6574 5f73 6361 6c69 6e67 5f70 6f69 6e74  et_scaling_point
-00002f00: 7328 5665 6332 2831 3030 2c20 3130 3029  s(Vec2(100, 100)
-00002f10: 2c20 5665 6332 2832 3030 2c20 3230 3029  , Vec2(200, 200)
-00002f20: 290d 0a20 2020 2020 2020 2070 6167 652e  )..        page.
-00002f30: 7365 745f 6973 6f74 726f 7069 635f 7363  set_isotropic_sc
-00002f40: 616c 696e 6728 302c 2032 302c 2030 2c20  aling(0, 20, 0, 
-00002f50: 3130 2c20 302c 2030 290d 0a20 2020 2020  10, 0, 0)..     
-00002f60: 2020 2061 7373 6572 7420 7061 6765 2e70     assert page.p
-00002f70: 6167 655f 706f 696e 7428 302c 2030 292e  age_point(0, 0).
-00002f80: 6973 636c 6f73 6528 2831 3030 2c20 3130  isclose((100, 10
-00002f90: 3029 290d 0a20 2020 2020 2020 2061 7373  0))..        ass
-00002fa0: 6572 7420 7061 6765 2e70 6167 655f 706f  ert page.page_po
-00002fb0: 696e 7428 3130 2c20 3529 2e69 7363 6c6f  int(10, 5).isclo
-00002fc0: 7365 2828 3135 302c 2031 3235 2929 0d0a  se((150, 125))..
-00002fd0: 2020 2020 2020 2020 6173 7365 7274 2070          assert p
-00002fe0: 6167 652e 7061 6765 5f70 6f69 6e74 2832  age.page_point(2
-00002ff0: 302c 2031 3029 2e69 7363 6c6f 7365 2828  0, 10).isclose((
-00003000: 3230 302c 2031 3530 2929 0d0a 0d0a 2020  200, 150))....  
-00003010: 2020 6465 6620 7465 7374 5f69 736f 7472    def test_isotr
-00003020: 6f70 6963 5f62 6f74 746f 6d5f 7769 6e64  opic_bottom_wind
-00003030: 6f77 5f31 3030 2873 656c 6629 3a0d 0a20  ow_100(self):.. 
-00003040: 2020 2020 2020 2070 6167 6520 3d20 5061         page = Pa
-00003050: 6765 2831 3030 302c 2031 3030 3029 0d0a  ge(1000, 1000)..
-00003060: 2020 2020 2020 2020 7061 6765 2e73 6574          page.set
-00003070: 5f73 6361 6c69 6e67 5f70 6f69 6e74 7328  _scaling_points(
-00003080: 5665 6332 2831 3030 2c20 3130 3029 2c20  Vec2(100, 100), 
-00003090: 5665 6332 2832 3030 2c20 3230 3029 290d  Vec2(200, 200)).
-000030a0: 0a20 2020 2020 2020 2070 6167 652e 7365  .        page.se
-000030b0: 745f 6973 6f74 726f 7069 635f 7363 616c  t_isotropic_scal
-000030c0: 696e 6728 302c 2032 302c 2030 2c20 3130  ing(0, 20, 0, 10
-000030d0: 2c20 312c 2031 290d 0a20 2020 2020 2020  , 1, 1)..       
-000030e0: 2061 7373 6572 7420 7061 6765 2e70 6167   assert page.pag
-000030f0: 655f 706f 696e 7428 302c 2030 292e 6973  e_point(0, 0).is
-00003100: 636c 6f73 6528 2831 3030 2c20 3135 3029  close((100, 150)
-00003110: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00003120: 7420 7061 6765 2e70 6167 655f 706f 696e  t page.page_poin
-00003130: 7428 3130 2c20 3529 2e69 7363 6c6f 7365  t(10, 5).isclose
-00003140: 2828 3135 302c 2031 3735 2929 0d0a 2020  ((150, 175))..  
-00003150: 2020 2020 2020 6173 7365 7274 2070 6167        assert pag
-00003160: 652e 7061 6765 5f70 6f69 6e74 2832 302c  e.page_point(20,
-00003170: 2031 3029 2e69 7363 6c6f 7365 2828 3230   10).isclose((20
-00003180: 302c 2032 3030 2929 0d0a 0d0a 2020 2020  0, 200))....    
-00003190: 6465 6620 7465 7374 5f69 736f 7472 6f70  def test_isotrop
-000031a0: 6963 5f6c 6566 745f 7769 6e64 6f77 5f35  ic_left_window_5
-000031b0: 3028 7365 6c66 293a 0d0a 2020 2020 2020  0(self):..      
-000031c0: 2020 7061 6765 203d 2050 6167 6528 3130    page = Page(10
-000031d0: 3030 2c20 3130 3030 290d 0a20 2020 2020  00, 1000)..     
-000031e0: 2020 2070 6167 652e 7365 745f 7363 616c     page.set_scal
-000031f0: 696e 675f 706f 696e 7473 2856 6563 3228  ing_points(Vec2(
-00003200: 3130 302c 2031 3030 292c 2056 6563 3228  100, 100), Vec2(
-00003210: 3230 302c 2032 3030 2929 0d0a 2020 2020  200, 200))..    
-00003220: 2020 2020 7061 6765 2e73 6574 5f69 736f      page.set_iso
-00003230: 7472 6f70 6963 5f73 6361 6c69 6e67 2830  tropic_scaling(0
-00003240: 2c20 3130 2c20 302c 2032 3029 0d0a 2020  , 10, 0, 20)..  
-00003250: 2020 2020 2020 6173 7365 7274 2070 6167        assert pag
-00003260: 652e 7061 6765 5f70 6f69 6e74 2830 2c20  e.page_point(0, 
-00003270: 3029 2e69 7363 6c6f 7365 2828 3132 352c  0).isclose((125,
-00003280: 2031 3030 2929 0d0a 2020 2020 2020 2020   100))..        
-00003290: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
-000032a0: 5f70 6f69 6e74 2835 2c20 3130 292e 6973  _point(5, 10).is
-000032b0: 636c 6f73 6528 2831 3530 2c20 3135 3029  close((150, 150)
-000032c0: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-000032d0: 7420 7061 6765 2e70 6167 655f 706f 696e  t page.page_poin
-000032e0: 7428 3130 2c20 3230 292e 6973 636c 6f73  t(10, 20).isclos
-000032f0: 6528 2831 3735 2c20 3230 3029 290d 0a0d  e((175, 200))...
-00003300: 0a20 2020 2064 6566 2074 6573 745f 6973  .    def test_is
-00003310: 6f74 726f 7069 635f 6c65 6674 5f77 696e  otropic_left_win
-00003320: 646f 775f 3028 7365 6c66 293a 0d0a 2020  dow_0(self):..  
-00003330: 2020 2020 2020 7061 6765 203d 2050 6167        page = Pag
-00003340: 6528 3130 3030 2c20 3130 3030 290d 0a20  e(1000, 1000).. 
-00003350: 2020 2020 2020 2070 6167 652e 7365 745f         page.set_
-00003360: 7363 616c 696e 675f 706f 696e 7473 2856  scaling_points(V
-00003370: 6563 3228 3130 302c 2031 3030 292c 2056  ec2(100, 100), V
-00003380: 6563 3228 3230 302c 2032 3030 2929 0d0a  ec2(200, 200))..
-00003390: 2020 2020 2020 2020 7061 6765 2e73 6574          page.set
-000033a0: 5f69 736f 7472 6f70 6963 5f73 6361 6c69  _isotropic_scali
-000033b0: 6e67 2830 2c20 3130 2c20 302c 2032 302c  ng(0, 10, 0, 20,
-000033c0: 2030 2c20 3029 0d0a 2020 2020 2020 2020   0, 0)..        
-000033d0: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
-000033e0: 5f70 6f69 6e74 2830 2c20 3029 2e69 7363  _point(0, 0).isc
-000033f0: 6c6f 7365 2828 3130 302c 2031 3030 2929  lose((100, 100))
-00003400: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-00003410: 2070 6167 652e 7061 6765 5f70 6f69 6e74   page.page_point
-00003420: 2835 2c20 3130 292e 6973 636c 6f73 6528  (5, 10).isclose(
-00003430: 2831 3235 2c20 3135 3029 290d 0a20 2020  (125, 150))..   
-00003440: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
-00003450: 2e70 6167 655f 706f 696e 7428 3130 2c20  .page_point(10, 
-00003460: 3230 292e 6973 636c 6f73 6528 2831 3530  20).isclose((150
-00003470: 2c20 3230 3029 290d 0a0d 0a20 2020 2064  , 200))....    d
-00003480: 6566 2074 6573 745f 6973 6f74 726f 7069  ef test_isotropi
-00003490: 635f 6c65 6674 5f77 696e 646f 775f 3130  c_left_window_10
-000034a0: 3028 7365 6c66 293a 0d0a 2020 2020 2020  0(self):..      
-000034b0: 2020 7061 6765 203d 2050 6167 6528 3130    page = Page(10
-000034c0: 3030 2c20 3130 3030 290d 0a20 2020 2020  00, 1000)..     
-000034d0: 2020 2070 6167 652e 7365 745f 7363 616c     page.set_scal
-000034e0: 696e 675f 706f 696e 7473 2856 6563 3228  ing_points(Vec2(
-000034f0: 3130 302c 2031 3030 292c 2056 6563 3228  100, 100), Vec2(
-00003500: 3230 302c 2032 3030 2929 0d0a 2020 2020  200, 200))..    
-00003510: 2020 2020 7061 6765 2e73 6574 5f69 736f      page.set_iso
-00003520: 7472 6f70 6963 5f73 6361 6c69 6e67 2830  tropic_scaling(0
-00003530: 2c20 3130 2c20 302c 2032 302c 2031 2c20  , 10, 0, 20, 1, 
-00003540: 3129 0d0a 2020 2020 2020 2020 6173 7365  1)..        asse
-00003550: 7274 2070 6167 652e 7061 6765 5f70 6f69  rt page.page_poi
-00003560: 6e74 2830 2c20 3029 2e69 7363 6c6f 7365  nt(0, 0).isclose
-00003570: 2828 3135 302c 2031 3030 2929 0d0a 2020  ((150, 100))..  
-00003580: 2020 2020 2020 6173 7365 7274 2070 6167        assert pag
-00003590: 652e 7061 6765 5f70 6f69 6e74 2835 2c20  e.page_point(5, 
-000035a0: 3130 292e 6973 636c 6f73 6528 2831 3735  10).isclose((175
-000035b0: 2c20 3135 3029 290d 0a20 2020 2020 2020  , 150))..       
-000035c0: 2061 7373 6572 7420 7061 6765 2e70 6167   assert page.pag
-000035d0: 655f 706f 696e 7428 3130 2c20 3230 292e  e_point(10, 20).
-000035e0: 6973 636c 6f73 6528 2832 3030 2c20 3230  isclose((200, 20
-000035f0: 3029 290d 0a0d 0a0d 0a64 6566 2074 6573  0))......def tes
-00003600: 745f 6172 635f 616e 676c 6573 2829 3a0d  t_arc_angles():.
-00003610: 0a20 2020 2066 726f 6d20 657a 6478 662e  .    from ezdxf.
-00003620: 6164 646f 6e73 2e68 7067 6c32 2e70 6c6f  addons.hpgl2.plo
-00003630: 7474 6572 2069 6d70 6f72 7420 6172 635f  tter import arc_
-00003640: 616e 676c 6573 0d0a 0d0a 2020 2020 616e  angles....    an
-00003650: 676c 6573 203d 206c 6973 7428 6172 635f  gles = list(arc_
-00003660: 616e 676c 6573 2830 2c20 3336 302c 2035  angles(0, 360, 5
-00003670: 2929 0d0a 2020 2020 6173 7365 7274 206c  ))..    assert l
-00003680: 656e 2861 6e67 6c65 7329 203d 3d20 3733  en(angles) == 73
-00003690: 0d0a 2020 2020 6173 7365 7274 2061 6e67  ..    assert ang
-000036a0: 6c65 735b 2d31 5d20 3d3d 2070 7974 6573  les[-1] == pytes
-000036b0: 742e 6170 7072 6f78 2833 3630 290d 0a0d  t.approx(360)...
-000036c0: 0a20 2020 2061 6e67 6c65 7320 3d20 6c69  .    angles = li
-000036d0: 7374 2861 7263 5f61 6e67 6c65 7328 302c  st(arc_angles(0,
-000036e0: 202d 3336 302c 2035 2929 0d0a 2020 2020   -360, 5))..    
-000036f0: 6173 7365 7274 206c 656e 2861 6e67 6c65  assert len(angle
-00003700: 7329 203d 3d20 3733 0d0a 2020 2020 6173  s) == 73..    as
-00003710: 7365 7274 2061 6e67 6c65 735b 2d31 5d20  sert angles[-1] 
-00003720: 3d3d 2070 7974 6573 742e 6170 7072 6f78  == pytest.approx
-00003730: 282d 3336 3029 0d0a 0d0a 0d0a 6465 6620  (-360)......def 
-00003740: 7465 7374 5f73 7765 6570 696e 675f 616e  test_sweeping_an
-00003750: 676c 6528 293a 0d0a 2020 2020 6672 6f6d  gle():..    from
-00003760: 2065 7a64 7866 2e61 6464 6f6e 732e 6870   ezdxf.addons.hp
-00003770: 676c 322e 706c 6f74 7465 7220 696d 706f  gl2.plotter impo
-00003780: 7274 2073 7765 6570 696e 675f 616e 676c  rt sweeping_angl
-00003790: 650d 0a0d 0a20 2020 2061 7373 6572 7420  e....    assert 
-000037a0: 7377 6565 7069 6e67 5f61 6e67 6c65 2830  sweeping_angle(0
-000037b0: 2c20 3435 2c20 3930 2920 3d3d 2039 300d  , 45, 90) == 90.
-000037c0: 0a20 2020 2061 7373 6572 7420 7377 6565  .    assert swee
-000037d0: 7069 6e67 5f61 6e67 6c65 2839 302c 2034  ping_angle(90, 4
-000037e0: 352c 2030 2920 3d3d 202d 3930 0d0a 2020  5, 0) == -90..  
-000037f0: 2020 6173 7365 7274 2073 7765 6570 696e    assert sweepin
-00003800: 675f 616e 676c 6528 3333 302c 2030 2c20  g_angle(330, 0, 
-00003810: 3330 2920 3d3d 2036 300d 0a20 2020 2061  30) == 60..    a
-00003820: 7373 6572 7420 7377 6565 7069 6e67 5f61  ssert sweeping_a
-00003830: 6e67 6c65 2833 3330 2c20 3138 302c 2033  ngle(330, 180, 3
-00003840: 3029 203d 3d20 2d33 3030 0d0a 2020 2020  0) == -300..    
-00003850: 6173 7365 7274 2073 7765 6570 696e 675f  assert sweeping_
-00003860: 616e 676c 6528 3330 2c20 302c 2033 3330  angle(30, 0, 330
-00003870: 2920 3d3d 202d 3630 0d0a 2020 2020 6173  ) == -60..    as
-00003880: 7365 7274 2073 7765 6570 696e 675f 616e  sert sweeping_an
-00003890: 676c 6528 3330 2c20 3138 302c 2033 3330  gle(30, 180, 330
-000038a0: 2920 3d3d 2033 3030 0d0a 0d0a 0d0a 636c  ) == 300......cl
-000038b0: 6173 7320 5465 7374 506c 6163 656d 656e  ass TestPlacemen
-000038c0: 744d 6174 7269 783a 0d0a 2020 2020 6465  tMatrix:..    de
-000038d0: 6620 7465 7374 5f73 6869 6674 5f74 6f5f  f test_shift_to_
-000038e0: 6f72 6967 696e 5f51 3128 7365 6c66 293a  origin_Q1(self):
-000038f0: 0d0a 2020 2020 2020 2020 6262 6f78 203d  ..        bbox =
-00003900: 2042 6f75 6e64 696e 6742 6f78 3264 285b   BoundingBox2d([
-00003910: 2831 302c 2031 3029 2c20 2832 302c 2032  (10, 10), (20, 2
-00003920: 3029 5d29 0d0a 2020 2020 2020 2020 6d20  0)])..        m 
-00003930: 3d20 706c 6163 656d 656e 745f 6d61 7472  = placement_matr
-00003940: 6978 2862 626f 7829 0d0a 2020 2020 2020  ix(bbox)..      
-00003950: 2020 6173 7365 7274 206d 2e74 7261 6e73    assert m.trans
-00003960: 666f 726d 2828 3130 2c20 3130 2929 2e69  form((10, 10)).i
-00003970: 7363 6c6f 7365 2828 302c 2030 2929 0d0a  sclose((0, 0))..
-00003980: 2020 2020 2020 2020 6173 7365 7274 206d          assert m
-00003990: 2e74 7261 6e73 666f 726d 2828 3230 2c20  .transform((20, 
-000039a0: 3230 2929 2e69 7363 6c6f 7365 2828 3130  20)).isclose((10
-000039b0: 2c20 3130 2929 0d0a 0d0a 2020 2020 6465  , 10))....    de
-000039c0: 6620 7465 7374 5f73 6869 6674 5f74 6f5f  f test_shift_to_
-000039d0: 6f72 6967 696e 5f51 3328 7365 6c66 293a  origin_Q3(self):
-000039e0: 0d0a 2020 2020 2020 2020 6262 6f78 203d  ..        bbox =
-000039f0: 2042 6f75 6e64 696e 6742 6f78 3264 285b   BoundingBox2d([
-00003a00: 282d 3130 2c20 2d31 3029 2c20 282d 3230  (-10, -10), (-20
-00003a10: 2c20 2d32 3029 5d29 0d0a 2020 2020 2020  , -20)])..      
-00003a20: 2020 6d20 3d20 706c 6163 656d 656e 745f    m = placement_
-00003a30: 6d61 7472 6978 2862 626f 7829 0d0a 2020  matrix(bbox)..  
-00003a40: 2020 2020 2020 6173 7365 7274 206d 2e74        assert m.t
-00003a50: 7261 6e73 666f 726d 2828 2d31 302c 202d  ransform((-10, -
-00003a60: 3130 2929 2e69 7363 6c6f 7365 2828 3130  10)).isclose((10
-00003a70: 2c20 3130 2929 0d0a 2020 2020 2020 2020  , 10))..        
-00003a80: 6173 7365 7274 206d 2e74 7261 6e73 666f  assert m.transfo
-00003a90: 726d 2828 2d32 302c 202d 3230 2929 2e69  rm((-20, -20)).i
-00003aa0: 7363 6c6f 7365 2828 302c 2030 2929 0d0a  sclose((0, 0))..
-00003ab0: 0d0a 2020 2020 6465 6620 7465 7374 5f72  ..    def test_r
-00003ac0: 6f74 6174 6528 7365 6c66 293a 0d0a 2020  otate(self):..  
-00003ad0: 2020 2020 2020 2320 7369 7a65 203d 2031        # size = 1
-00003ae0: 3020 7820 3330 0d0a 2020 2020 2020 2020  0 x 30..        
-00003af0: 6262 6f78 203d 2042 6f75 6e64 696e 6742  bbox = BoundingB
-00003b00: 6f78 3264 285b 2831 302c 2031 3029 2c20  ox2d([(10, 10), 
-00003b10: 2832 302c 2034 3029 5d29 0d0a 2020 2020  (20, 40)])..    
-00003b20: 2020 2020 6d20 3d20 706c 6163 656d 656e      m = placemen
-00003b30: 745f 6d61 7472 6978 2862 626f 782c 2072  t_matrix(bbox, r
-00003b40: 6f74 6174 696f 6e3d 3930 290d 0a20 2020  otation=90)..   
-00003b50: 2020 2020 2061 7373 6572 7420 6d2e 7472       assert m.tr
-00003b60: 616e 7366 6f72 6d28 2831 302c 2031 3029  ansform((10, 10)
-00003b70: 292e 6973 636c 6f73 6528 2833 302c 2030  ).isclose((30, 0
-00003b80: 2929 0d0a 2020 2020 2020 2020 6173 7365  ))..        asse
-00003b90: 7274 206d 2e74 7261 6e73 666f 726d 2828  rt m.transform((
-00003ba0: 3230 2c20 3430 2929 2e69 7363 6c6f 7365  20, 40)).isclose
-00003bb0: 2828 302c 2031 3029 290d 0a0d 0a0d 0a69  ((0, 10))......i
-00003bc0: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 225f  f __name__ == "_
-00003bd0: 5f6d 6169 6e5f 5f22 3a0d 0a20 2020 2070  _main__":..    p
-00003be0: 7974 6573 742e 6d61 696e 285b 5f5f 6669  ytest.main([__fi
-00003bf0: 6c65 5f5f 5d29 0d0a                      le__])..
+000020e0: 6669 6c74 6572 5f6e 6f6e 5f70 7269 6e74  filter_non_print
+000020f0: 6162 6c65 5f63 6861 7273 5f66 726f 6d5f  able_chars_from_
+00002100: 7065 5f63 6f6d 6d61 6e64 2873 656c 6629  pe_command(self)
+00002110: 3a0d 0a20 2020 2020 2020 2072 6573 756c  :..        resul
+00002120: 7420 3d20 7365 6c66 2e70 6172 7365 2868  t = self.parse(h
+00002130: 7067 6c32 2862 2250 4578 7878 7878 5c72  pgl2(b"PExxxxx\r
+00002140: 5c6e 7878 7878 783b 2229 290d 0a20 2020  \nxxxxx;"))..   
+00002150: 2020 2020 2061 7373 6572 7420 7265 7375       assert resu
+00002160: 6c74 5b30 5d2e 6172 6773 5b30 5d20 3d3d  lt[0].args[0] ==
+00002170: 2062 2278 7878 7878 7878 7878 7822 0d0a   b"xxxxxxxxxx"..
+00002180: 0d0a 2020 2020 6465 6620 7465 7374 5f6e  ..    def test_n
+00002190: 6f5f 6870 676c 325f 6461 7461 2873 656c  o_hpgl2_data(sel
+000021a0: 6629 3a0d 0a20 2020 2020 2020 2023 2045  f):..        # E
+000021b0: 6361 7065 2073 6571 7565 6e63 6520 746f  cape sequence to
+000021c0: 2065 6e74 6572 2048 5047 4c32 206d 6f64   enter HPGL2 mod
+000021d0: 6520 6973 206d 6973 7369 6e67 3a20 2022  e is missing:  "
+000021e0: 1b25 3142 220d 0a20 2020 2020 2020 2061  .%1B"..        a
+000021f0: 7373 6572 7420 6c65 6e28 7365 6c66 2e70  ssert len(self.p
+00002200: 6172 7365 2862 2241 4e59 5445 5854 3b49  arse(b"ANYTEXT;I
+00002210: 4e3b 4250 3b22 2929 203d 3d20 300d 0a0d  N;BP;")) == 0...
+00002220: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+00002230: 6b2e 7061 7261 6d65 7472 697a 6528 2262  k.parametrize("b
+00002240: 222c 205b 0d0a 2020 2020 2020 2020 6222  ", [..        b"
+00002250: 4c42 204d 5920 6c61 6265 6c20 0350 4133  LB MY label .PA3
+00002260: 3831 2c30 5349 302e 3132 352c 302e 3235  81,0SI0.125,0.25
+00002270: 4449 302c 313b 222c 0d0a 2020 2020 2020  DI0,1;",..      
+00002280: 2020 6222 4c42 4d59 206c 6162 656c 2003    b"LBMY label .
+00002290: 5041 3338 312c 3053 4930 2e31 3235 2c30  PA381,0SI0.125,0
+000022a0: 2e32 3544 4930 2c31 3b22 0d0a 2020 2020  .25DI0,1;"..    
+000022b0: 5d29 0d0a 2020 2020 6465 6620 7465 7374  ])..    def test
+000022c0: 5f6c 6162 656c 5f77 6974 685f 7465 726d  _label_with_term
+000022d0: 696e 6174 6f72 2873 656c 662c 2062 293a  inator(self, b):
+000022e0: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
+000022f0: 6473 203d 2073 656c 662e 7061 7273 6528  ds = self.parse(
+00002300: 6870 676c 3228 6229 290d 0a20 2020 2020  hpgl2(b))..     
+00002310: 2020 2061 7373 6572 7420 6c65 6e28 636f     assert len(co
+00002320: 6d6d 616e 6473 2920 3d3d 2034 0d0a 0d0a  mmands) == 4....
+00002330: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+00002340: 2e70 6172 616d 6574 7269 7a65 280d 0a20  .parametrize(.. 
+00002350: 2020 2020 2020 2022 6222 2c0d 0a20 2020         "b",..   
+00002360: 2020 2020 205b 0d0a 2020 2020 2020 2020       [..        
+00002370: 2020 2020 6222 4454 5c30 344c 4220 5475      b"DT\04LB Tu
+00002380: 6520 4465 6320 3138 2031 363a 3230 3a30  e Dec 18 16:20:0
+00002390: 3520 3230 3031 205c 3034 5041 3338 312c  5 2001 \04PA381,
+000023a0: 3053 4930 2e31 3235 2c30 2e32 3544 4930  0SI0.125,0.25DI0
+000023b0: 2c31 3b22 2c0d 0a20 2020 2020 2020 2020  ,1;",..         
+000023c0: 2020 2062 2244 545c 3034 2c30 4c42 2054     b"DT\04,0LB T
+000023d0: 7565 2044 6563 2031 3820 3136 3a32 303a  ue Dec 18 16:20:
+000023e0: 3035 2032 3030 3120 5c30 3450 4133 3831  05 2001 \04PA381
+000023f0: 2c30 5349 302e 3132 352c 302e 3235 4449  ,0SI0.125,0.25DI
+00002400: 302c 313b 222c 0d0a 2020 2020 2020 2020  0,1;",..        
+00002410: 2020 2020 6222 4454 5c30 342c 313b 4c42      b"DT\04,1;LB
+00002420: 2054 7565 2044 6563 2031 3820 3136 3a32   Tue Dec 18 16:2
+00002430: 303a 3035 2032 3030 3120 5c30 3450 4133  0:05 2001 \04PA3
+00002440: 3831 2c30 5349 302e 3132 352c 302e 3235  81,0SI0.125,0.25
+00002450: 4449 302c 313b 222c 0d0a 2020 2020 2020  DI0,1;",..      
+00002460: 2020 5d2c 0d0a 2020 2020 290d 0a20 2020    ],..    )..   
+00002470: 2064 6566 2074 6573 745f 6c61 6265 6c5f   def test_label_
+00002480: 7769 7468 5f63 7573 746f 6d5f 7465 726d  with_custom_term
+00002490: 696e 6174 6f72 2873 656c 662c 2062 293a  inator(self, b):
+000024a0: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
+000024b0: 6473 203d 2073 656c 662e 7061 7273 6528  ds = self.parse(
+000024c0: 6870 676c 3228 6229 290d 0a20 2020 2020  hpgl2(b))..     
+000024d0: 2020 2061 7373 6572 7420 6c65 6e28 636f     assert len(co
+000024e0: 6d6d 616e 6473 2920 3d3d 2034 0d0a 0d0a  mmands) == 4....
+000024f0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+00002500: 2e70 6172 616d 6574 7269 7a65 280d 0a20  .parametrize(.. 
+00002510: 2020 2020 2020 2022 6222 2c0d 0a20 2020         "b",..   
+00002520: 2020 2020 205b 0d0a 2020 2020 2020 2020       [..        
+00002530: 2020 2020 6222 4454 5c30 344c 4220 4d59      b"DT\04LB MY
+00002540: 206c 6162 656c 5c30 3444 544c 4220 4d79   label\04DTLB My
+00002550: 206f 7468 6572 206c 6162 656c 2003 222c   other label .",
+00002560: 0d0a 2020 2020 2020 2020 2020 2020 6222  ..            b"
+00002570: 4454 5c30 344c 4220 4d59 206c 6162 656c  DT\04LB MY label
+00002580: 5c30 3444 543b 4c42 204d 7920 6f74 6865  \04DT;LB My othe
+00002590: 7220 6c61 6265 6c20 0322 2c0d 0a20 2020  r label .",..   
+000025a0: 2020 2020 205d 2c0d 0a20 2020 2029 0d0a       ],..    )..
+000025b0: 2020 2020 6465 6620 7465 7374 5f72 6573      def test_res
+000025c0: 6574 5f63 7573 746f 6d5f 7465 726d 696e  et_custom_termin
+000025d0: 6174 6f72 2873 656c 662c 2062 293a 0d0a  ator(self, b):..
+000025e0: 2020 2020 2020 2020 636f 6d6d 616e 6473          commands
+000025f0: 203d 2073 656c 662e 7061 7273 6528 6870   = self.parse(hp
+00002600: 676c 3228 6229 290d 0a20 2020 2020 2020  gl2(b))..       
+00002610: 2061 7373 6572 7420 6c65 6e28 636f 6d6d   assert len(comm
+00002620: 616e 6473 2920 3d3d 2032 0d0a 0d0a 0d0a  ands) == 2......
+00002630: 636c 6173 7320 5465 7374 5061 6765 436f  class TestPageCo
+00002640: 6f72 6469 6e61 7465 733a 0d0a 2020 2020  ordinates:..    
+00002650: 4070 7974 6573 742e 6669 7874 7572 6528  @pytest.fixture(
+00002660: 7363 6f70 653d 2263 6c61 7373 2229 0d0a  scope="class")..
+00002670: 2020 2020 6465 6620 7061 6765 2873 656c      def page(sel
+00002680: 6629 3a0d 0a20 2020 2020 2020 2070 6167  f):..        pag
+00002690: 655f 203d 2050 6167 6528 3130 3030 2c20  e_ = Page(1000, 
+000026a0: 3130 3030 290d 0a20 2020 2020 2020 2070  1000)..        p
+000026b0: 6167 655f 2e73 6574 5f75 6373 2856 6563  age_.set_ucs(Vec
+000026c0: 3228 3530 302c 2035 3030 292c 2073 783d  2(500, 500), sx=
+000026d0: 322c 2073 793d 3329 0d0a 2020 2020 2020  2, sy=3)..      
+000026e0: 2020 7265 7475 726e 2070 6167 655f 0d0a    return page_..
+000026f0: 0d0a 2020 2020 6465 6620 7465 7374 5f75  ..    def test_u
+00002700: 7365 725f 746f 5f70 6167 655f 636f 6f72  ser_to_page_coor
+00002710: 6469 6e61 7465 7328 7365 6c66 2c20 7061  dinates(self, pa
+00002720: 6765 293a 0d0a 2020 2020 2020 2020 6173  ge):..        as
+00002730: 7365 7274 2070 6167 652e 7061 6765 5f70  sert page.page_p
+00002740: 6f69 6e74 2830 2c20 3029 2e69 7363 6c6f  oint(0, 0).isclo
+00002750: 7365 2828 3530 302c 2035 3030 2929 0d0a  se((500, 500))..
+00002760: 2020 2020 2020 2020 6173 7365 7274 2070          assert p
+00002770: 6167 652e 7061 6765 5f70 6f69 6e74 2831  age.page_point(1
+00002780: 302c 2031 3029 2e69 7363 6c6f 7365 2828  0, 10).isclose((
+00002790: 3532 302c 2035 3330 2929 0d0a 0d0a 2020  520, 530))....  
+000027a0: 2020 6465 6620 7465 7374 5f75 7365 725f    def test_user_
+000027b0: 7665 6374 6f72 5f74 6f5f 7061 6765 5f76  vector_to_page_v
+000027c0: 6563 746f 7228 7365 6c66 2c20 7061 6765  ector(self, page
+000027d0: 293a 0d0a 2020 2020 2020 2020 6173 7365  ):..        asse
+000027e0: 7274 2070 6167 652e 7061 6765 5f76 6563  rt page.page_vec
+000027f0: 746f 7228 302c 2030 292e 6973 636c 6f73  tor(0, 0).isclos
+00002800: 6528 2830 2c20 3029 290d 0a20 2020 2020  e((0, 0))..     
+00002810: 2020 2061 7373 6572 7420 7061 6765 2e70     assert page.p
+00002820: 6167 655f 7665 6374 6f72 2831 302c 2031  age_vector(10, 1
+00002830: 3029 2e69 7363 6c6f 7365 2828 3230 2c20  0).isclose((20, 
+00002840: 3330 2929 0d0a 0d0a 0d0a 636c 6173 7320  30))......class 
+00002850: 5465 7374 5061 6765 416e 6973 6f74 726f  TestPageAnisotro
+00002860: 7069 6353 6361 6c69 6e67 3a0d 0a20 2020  picScaling:..   
+00002870: 2064 6566 2074 6573 745f 6973 6f74 726f   def test_isotro
+00002880: 7069 635f 7363 616c 696e 6728 7365 6c66  pic_scaling(self
+00002890: 293a 0d0a 2020 2020 2020 2020 7061 6765  ):..        page
+000028a0: 203d 2050 6167 6528 3130 3030 2c20 3130   = Page(1000, 10
+000028b0: 3030 290d 0a20 2020 2020 2020 2070 6167  00)..        pag
+000028c0: 652e 7365 745f 7363 616c 696e 675f 706f  e.set_scaling_po
+000028d0: 696e 7473 2856 6563 3228 3130 302c 2031  ints(Vec2(100, 1
+000028e0: 3030 292c 2056 6563 3228 3230 302c 2032  00), Vec2(200, 2
+000028f0: 3030 2929 0d0a 2020 2020 2020 2020 7061  00))..        pa
+00002900: 6765 2e73 6574 5f61 6e69 736f 7472 6f70  ge.set_anisotrop
+00002910: 6963 5f73 6361 6c69 6e67 282d 3130 2c20  ic_scaling(-10, 
+00002920: 3130 2c20 2d31 302c 2031 3029 0d0a 2020  10, -10, 10)..  
+00002930: 2020 2020 2020 6173 7365 7274 2070 6167        assert pag
+00002940: 652e 7573 6572 5f73 6361 6c69 6e67 2069  e.user_scaling i
+00002950: 7320 5472 7565 0d0a 2020 2020 2020 2020  s True..        
+00002960: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
+00002970: 5f70 6f69 6e74 2830 2c20 3029 2e69 7363  _point(0, 0).isc
+00002980: 6c6f 7365 2828 3135 302c 2031 3530 2929  lose((150, 150))
+00002990: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+000029a0: 2070 6167 652e 7061 6765 5f70 6f69 6e74   page.page_point
+000029b0: 282d 3130 2c20 2d31 3029 2e69 7363 6c6f  (-10, -10).isclo
+000029c0: 7365 2828 3130 302c 2031 3030 2929 0d0a  se((100, 100))..
+000029d0: 2020 2020 2020 2020 6173 7365 7274 2070          assert p
+000029e0: 6167 652e 7061 6765 5f70 6f69 6e74 2831  age.page_point(1
+000029f0: 302c 2031 3029 2e69 7363 6c6f 7365 2828  0, 10).isclose((
+00002a00: 3230 302c 2032 3030 2929 0d0a 0d0a 2020  200, 200))....  
+00002a10: 2020 6465 6620 7465 7374 5f61 6e69 736f    def test_aniso
+00002a20: 7472 6f70 6963 5f73 6361 6c69 6e67 2873  tropic_scaling(s
+00002a30: 656c 6629 3a0d 0a20 2020 2020 2020 2070  elf):..        p
+00002a40: 6167 6520 3d20 5061 6765 2831 3030 302c  age = Page(1000,
+00002a50: 2031 3030 3029 0d0a 2020 2020 2020 2020   1000)..        
+00002a60: 7061 6765 2e73 6574 5f73 6361 6c69 6e67  page.set_scaling
+00002a70: 5f70 6f69 6e74 7328 5665 6332 2831 3030  _points(Vec2(100
+00002a80: 2c20 3130 3029 2c20 5665 6332 2832 3030  , 100), Vec2(200
+00002a90: 2c20 3230 3029 290d 0a20 2020 2020 2020  , 200))..       
+00002aa0: 2070 6167 652e 7365 745f 616e 6973 6f74   page.set_anisot
+00002ab0: 726f 7069 635f 7363 616c 696e 6728 2d31  ropic_scaling(-1
+00002ac0: 302c 2031 302c 202d 3230 2c20 3230 290d  0, 10, -20, 20).
+00002ad0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00002ae0: 7061 6765 2e75 7365 725f 7363 616c 696e  page.user_scalin
+00002af0: 6720 6973 2054 7275 650d 0a20 2020 2020  g is True..     
+00002b00: 2020 2061 7373 6572 7420 7061 6765 2e70     assert page.p
+00002b10: 6167 655f 706f 696e 7428 302c 2030 292e  age_point(0, 0).
+00002b20: 6973 636c 6f73 6528 2831 3530 2c20 3135  isclose((150, 15
+00002b30: 3029 290d 0a20 2020 2020 2020 2061 7373  0))..        ass
+00002b40: 6572 7420 7061 6765 2e70 6167 655f 706f  ert page.page_po
+00002b50: 696e 7428 2d31 302c 202d 3230 292e 6973  int(-10, -20).is
+00002b60: 636c 6f73 6528 2831 3030 2c20 3130 3029  close((100, 100)
+00002b70: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00002b80: 7420 7061 6765 2e70 6167 655f 706f 696e  t page.page_poin
+00002b90: 7428 3130 2c20 3230 292e 6973 636c 6f73  t(10, 20).isclos
+00002ba0: 6528 2832 3030 2c20 3230 3029 290d 0a0d  e((200, 200))...
+00002bb0: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
+00002bc0: 7665 7273 655f 616e 6973 6f74 726f 7069  verse_anisotropi
+00002bd0: 635f 7363 616c 696e 6728 7365 6c66 293a  c_scaling(self):
+00002be0: 0d0a 2020 2020 2020 2020 7061 6765 203d  ..        page =
+00002bf0: 2050 6167 6528 3130 3030 2c20 3130 3030   Page(1000, 1000
+00002c00: 290d 0a20 2020 2020 2020 2070 6167 652e  )..        page.
+00002c10: 7365 745f 7363 616c 696e 675f 706f 696e  set_scaling_poin
+00002c20: 7473 2856 6563 3228 3130 302c 2031 3030  ts(Vec2(100, 100
+00002c30: 292c 2056 6563 3228 3230 302c 2032 3030  ), Vec2(200, 200
+00002c40: 2929 0d0a 2020 2020 2020 2020 2320 7265  ))..        # re
+00002c50: 7665 7273 6520 7820 616e 6420 7920 6178  verse x and y ax
+00002c60: 6973 3a0d 0a20 2020 2020 2020 2070 6167  is:..        pag
+00002c70: 652e 7365 745f 616e 6973 6f74 726f 7069  e.set_anisotropi
+00002c80: 635f 7363 616c 696e 6728 3130 2c20 2d31  c_scaling(10, -1
+00002c90: 302c 2032 302c 202d 3230 290d 0a20 2020  0, 20, -20)..   
+00002ca0: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
+00002cb0: 2e75 7365 725f 7363 616c 696e 6720 6973  .user_scaling is
+00002cc0: 2054 7275 650d 0a20 2020 2020 2020 2061   True..        a
+00002cd0: 7373 6572 7420 7061 6765 2e70 6167 655f  ssert page.page_
+00002ce0: 706f 696e 7428 302c 2030 292e 6973 636c  point(0, 0).iscl
+00002cf0: 6f73 6528 2831 3530 2c20 3135 3029 290d  ose((150, 150)).
+00002d00: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00002d10: 7061 6765 2e70 6167 655f 706f 696e 7428  page.page_point(
+00002d20: 3130 2c20 3230 292e 6973 636c 6f73 6528  10, 20).isclose(
+00002d30: 2831 3030 2c20 3130 3029 290d 0a20 2020  (100, 100))..   
+00002d40: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
+00002d50: 2e70 6167 655f 706f 696e 7428 2d31 302c  .page_point(-10,
+00002d60: 202d 3230 292e 6973 636c 6f73 6528 2832   -20).isclose((2
+00002d70: 3030 2c20 3230 3029 290d 0a0d 0a0d 0a63  00, 200))......c
+00002d80: 6c61 7373 2054 6573 7450 6167 6549 736f  lass TestPageIso
+00002d90: 7472 6f70 6963 5363 616c 696e 673a 0d0a  tropicScaling:..
+00002da0: 2020 2020 6465 6620 7465 7374 5f69 736f      def test_iso
+00002db0: 7472 6f70 6963 5f62 6f74 746f 6d5f 7769  tropic_bottom_wi
+00002dc0: 6e64 6f77 5f35 3028 7365 6c66 293a 0d0a  ndow_50(self):..
+00002dd0: 2020 2020 2020 2020 7061 6765 203d 2050          page = P
+00002de0: 6167 6528 3130 3030 2c20 3130 3030 290d  age(1000, 1000).
+00002df0: 0a20 2020 2020 2020 2070 6167 652e 7365  .        page.se
+00002e00: 745f 7363 616c 696e 675f 706f 696e 7473  t_scaling_points
+00002e10: 2856 6563 3228 3130 302c 2031 3030 292c  (Vec2(100, 100),
+00002e20: 2056 6563 3228 3230 302c 2032 3030 2929   Vec2(200, 200))
+00002e30: 0d0a 2020 2020 2020 2020 7061 6765 2e73  ..        page.s
+00002e40: 6574 5f69 736f 7472 6f70 6963 5f73 6361  et_isotropic_sca
+00002e50: 6c69 6e67 2830 2c20 3230 2c20 302c 2031  ling(0, 20, 0, 1
+00002e60: 3029 0d0a 2020 2020 2020 2020 6173 7365  0)..        asse
+00002e70: 7274 2070 6167 652e 7573 6572 5f73 6361  rt page.user_sca
+00002e80: 6c69 6e67 2069 7320 5472 7565 0d0a 2020  ling is True..  
+00002e90: 2020 2020 2020 6173 7365 7274 2070 6167        assert pag
+00002ea0: 652e 7061 6765 5f70 6f69 6e74 2830 2c20  e.page_point(0, 
+00002eb0: 3029 2e69 7363 6c6f 7365 2828 3130 302c  0).isclose((100,
+00002ec0: 2031 3235 2929 0d0a 2020 2020 2020 2020   125))..        
+00002ed0: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
+00002ee0: 5f70 6f69 6e74 2831 302c 2035 292e 6973  _point(10, 5).is
+00002ef0: 636c 6f73 6528 2831 3530 2c20 3135 3029  close((150, 150)
+00002f00: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00002f10: 7420 7061 6765 2e70 6167 655f 706f 696e  t page.page_poin
+00002f20: 7428 3230 2c20 3130 292e 6973 636c 6f73  t(20, 10).isclos
+00002f30: 6528 2832 3030 2c20 3137 3529 290d 0a0d  e((200, 175))...
+00002f40: 0a20 2020 2064 6566 2074 6573 745f 6973  .    def test_is
+00002f50: 6f74 726f 7069 635f 626f 7474 6f6d 5f77  otropic_bottom_w
+00002f60: 696e 646f 775f 3028 7365 6c66 293a 0d0a  indow_0(self):..
+00002f70: 2020 2020 2020 2020 7061 6765 203d 2050          page = P
+00002f80: 6167 6528 3130 3030 2c20 3130 3030 290d  age(1000, 1000).
+00002f90: 0a20 2020 2020 2020 2070 6167 652e 7365  .        page.se
+00002fa0: 745f 7363 616c 696e 675f 706f 696e 7473  t_scaling_points
+00002fb0: 2856 6563 3228 3130 302c 2031 3030 292c  (Vec2(100, 100),
+00002fc0: 2056 6563 3228 3230 302c 2032 3030 2929   Vec2(200, 200))
+00002fd0: 0d0a 2020 2020 2020 2020 7061 6765 2e73  ..        page.s
+00002fe0: 6574 5f69 736f 7472 6f70 6963 5f73 6361  et_isotropic_sca
+00002ff0: 6c69 6e67 2830 2c20 3230 2c20 302c 2031  ling(0, 20, 0, 1
+00003000: 302c 2030 2c20 3029 0d0a 2020 2020 2020  0, 0, 0)..      
+00003010: 2020 6173 7365 7274 2070 6167 652e 7061    assert page.pa
+00003020: 6765 5f70 6f69 6e74 2830 2c20 3029 2e69  ge_point(0, 0).i
+00003030: 7363 6c6f 7365 2828 3130 302c 2031 3030  sclose((100, 100
+00003040: 2929 0d0a 2020 2020 2020 2020 6173 7365  ))..        asse
+00003050: 7274 2070 6167 652e 7061 6765 5f70 6f69  rt page.page_poi
+00003060: 6e74 2831 302c 2035 292e 6973 636c 6f73  nt(10, 5).isclos
+00003070: 6528 2831 3530 2c20 3132 3529 290d 0a20  e((150, 125)).. 
+00003080: 2020 2020 2020 2061 7373 6572 7420 7061         assert pa
+00003090: 6765 2e70 6167 655f 706f 696e 7428 3230  ge.page_point(20
+000030a0: 2c20 3130 292e 6973 636c 6f73 6528 2832  , 10).isclose((2
+000030b0: 3030 2c20 3135 3029 290d 0a0d 0a20 2020  00, 150))....   
+000030c0: 2064 6566 2074 6573 745f 6973 6f74 726f   def test_isotro
+000030d0: 7069 635f 626f 7474 6f6d 5f77 696e 646f  pic_bottom_windo
+000030e0: 775f 3130 3028 7365 6c66 293a 0d0a 2020  w_100(self):..  
+000030f0: 2020 2020 2020 7061 6765 203d 2050 6167        page = Pag
+00003100: 6528 3130 3030 2c20 3130 3030 290d 0a20  e(1000, 1000).. 
+00003110: 2020 2020 2020 2070 6167 652e 7365 745f         page.set_
+00003120: 7363 616c 696e 675f 706f 696e 7473 2856  scaling_points(V
+00003130: 6563 3228 3130 302c 2031 3030 292c 2056  ec2(100, 100), V
+00003140: 6563 3228 3230 302c 2032 3030 2929 0d0a  ec2(200, 200))..
+00003150: 2020 2020 2020 2020 7061 6765 2e73 6574          page.set
+00003160: 5f69 736f 7472 6f70 6963 5f73 6361 6c69  _isotropic_scali
+00003170: 6e67 2830 2c20 3230 2c20 302c 2031 302c  ng(0, 20, 0, 10,
+00003180: 2031 2c20 3129 0d0a 2020 2020 2020 2020   1, 1)..        
+00003190: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
+000031a0: 5f70 6f69 6e74 2830 2c20 3029 2e69 7363  _point(0, 0).isc
+000031b0: 6c6f 7365 2828 3130 302c 2031 3530 2929  lose((100, 150))
+000031c0: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+000031d0: 2070 6167 652e 7061 6765 5f70 6f69 6e74   page.page_point
+000031e0: 2831 302c 2035 292e 6973 636c 6f73 6528  (10, 5).isclose(
+000031f0: 2831 3530 2c20 3137 3529 290d 0a20 2020  (150, 175))..   
+00003200: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
+00003210: 2e70 6167 655f 706f 696e 7428 3230 2c20  .page_point(20, 
+00003220: 3130 292e 6973 636c 6f73 6528 2832 3030  10).isclose((200
+00003230: 2c20 3230 3029 290d 0a0d 0a20 2020 2064  , 200))....    d
+00003240: 6566 2074 6573 745f 6973 6f74 726f 7069  ef test_isotropi
+00003250: 635f 6c65 6674 5f77 696e 646f 775f 3530  c_left_window_50
+00003260: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00003270: 2070 6167 6520 3d20 5061 6765 2831 3030   page = Page(100
+00003280: 302c 2031 3030 3029 0d0a 2020 2020 2020  0, 1000)..      
+00003290: 2020 7061 6765 2e73 6574 5f73 6361 6c69    page.set_scali
+000032a0: 6e67 5f70 6f69 6e74 7328 5665 6332 2831  ng_points(Vec2(1
+000032b0: 3030 2c20 3130 3029 2c20 5665 6332 2832  00, 100), Vec2(2
+000032c0: 3030 2c20 3230 3029 290d 0a20 2020 2020  00, 200))..     
+000032d0: 2020 2070 6167 652e 7365 745f 6973 6f74     page.set_isot
+000032e0: 726f 7069 635f 7363 616c 696e 6728 302c  ropic_scaling(0,
+000032f0: 2031 302c 2030 2c20 3230 290d 0a20 2020   10, 0, 20)..   
+00003300: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
+00003310: 2e70 6167 655f 706f 696e 7428 302c 2030  .page_point(0, 0
+00003320: 292e 6973 636c 6f73 6528 2831 3235 2c20  ).isclose((125, 
+00003330: 3130 3029 290d 0a20 2020 2020 2020 2061  100))..        a
+00003340: 7373 6572 7420 7061 6765 2e70 6167 655f  ssert page.page_
+00003350: 706f 696e 7428 352c 2031 3029 2e69 7363  point(5, 10).isc
+00003360: 6c6f 7365 2828 3135 302c 2031 3530 2929  lose((150, 150))
+00003370: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+00003380: 2070 6167 652e 7061 6765 5f70 6f69 6e74   page.page_point
+00003390: 2831 302c 2032 3029 2e69 7363 6c6f 7365  (10, 20).isclose
+000033a0: 2828 3137 352c 2032 3030 2929 0d0a 0d0a  ((175, 200))....
+000033b0: 2020 2020 6465 6620 7465 7374 5f69 736f      def test_iso
+000033c0: 7472 6f70 6963 5f6c 6566 745f 7769 6e64  tropic_left_wind
+000033d0: 6f77 5f30 2873 656c 6629 3a0d 0a20 2020  ow_0(self):..   
+000033e0: 2020 2020 2070 6167 6520 3d20 5061 6765       page = Page
+000033f0: 2831 3030 302c 2031 3030 3029 0d0a 2020  (1000, 1000)..  
+00003400: 2020 2020 2020 7061 6765 2e73 6574 5f73        page.set_s
+00003410: 6361 6c69 6e67 5f70 6f69 6e74 7328 5665  caling_points(Ve
+00003420: 6332 2831 3030 2c20 3130 3029 2c20 5665  c2(100, 100), Ve
+00003430: 6332 2832 3030 2c20 3230 3029 290d 0a20  c2(200, 200)).. 
+00003440: 2020 2020 2020 2070 6167 652e 7365 745f         page.set_
+00003450: 6973 6f74 726f 7069 635f 7363 616c 696e  isotropic_scalin
+00003460: 6728 302c 2031 302c 2030 2c20 3230 2c20  g(0, 10, 0, 20, 
+00003470: 302c 2030 290d 0a20 2020 2020 2020 2061  0, 0)..        a
+00003480: 7373 6572 7420 7061 6765 2e70 6167 655f  ssert page.page_
+00003490: 706f 696e 7428 302c 2030 292e 6973 636c  point(0, 0).iscl
+000034a0: 6f73 6528 2831 3030 2c20 3130 3029 290d  ose((100, 100)).
+000034b0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000034c0: 7061 6765 2e70 6167 655f 706f 696e 7428  page.page_point(
+000034d0: 352c 2031 3029 2e69 7363 6c6f 7365 2828  5, 10).isclose((
+000034e0: 3132 352c 2031 3530 2929 0d0a 2020 2020  125, 150))..    
+000034f0: 2020 2020 6173 7365 7274 2070 6167 652e      assert page.
+00003500: 7061 6765 5f70 6f69 6e74 2831 302c 2032  page_point(10, 2
+00003510: 3029 2e69 7363 6c6f 7365 2828 3135 302c  0).isclose((150,
+00003520: 2032 3030 2929 0d0a 0d0a 2020 2020 6465   200))....    de
+00003530: 6620 7465 7374 5f69 736f 7472 6f70 6963  f test_isotropic
+00003540: 5f6c 6566 745f 7769 6e64 6f77 5f31 3030  _left_window_100
+00003550: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00003560: 2070 6167 6520 3d20 5061 6765 2831 3030   page = Page(100
+00003570: 302c 2031 3030 3029 0d0a 2020 2020 2020  0, 1000)..      
+00003580: 2020 7061 6765 2e73 6574 5f73 6361 6c69    page.set_scali
+00003590: 6e67 5f70 6f69 6e74 7328 5665 6332 2831  ng_points(Vec2(1
+000035a0: 3030 2c20 3130 3029 2c20 5665 6332 2832  00, 100), Vec2(2
+000035b0: 3030 2c20 3230 3029 290d 0a20 2020 2020  00, 200))..     
+000035c0: 2020 2070 6167 652e 7365 745f 6973 6f74     page.set_isot
+000035d0: 726f 7069 635f 7363 616c 696e 6728 302c  ropic_scaling(0,
+000035e0: 2031 302c 2030 2c20 3230 2c20 312c 2031   10, 0, 20, 1, 1
+000035f0: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00003600: 7420 7061 6765 2e70 6167 655f 706f 696e  t page.page_poin
+00003610: 7428 302c 2030 292e 6973 636c 6f73 6528  t(0, 0).isclose(
+00003620: 2831 3530 2c20 3130 3029 290d 0a20 2020  (150, 100))..   
+00003630: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
+00003640: 2e70 6167 655f 706f 696e 7428 352c 2031  .page_point(5, 1
+00003650: 3029 2e69 7363 6c6f 7365 2828 3137 352c  0).isclose((175,
+00003660: 2031 3530 2929 0d0a 2020 2020 2020 2020   150))..        
+00003670: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
+00003680: 5f70 6f69 6e74 2831 302c 2032 3029 2e69  _point(10, 20).i
+00003690: 7363 6c6f 7365 2828 3230 302c 2032 3030  sclose((200, 200
+000036a0: 2929 0d0a 0d0a 0d0a 6465 6620 7465 7374  ))......def test
+000036b0: 5f61 7263 5f61 6e67 6c65 7328 293a 0d0a  _arc_angles():..
+000036c0: 2020 2020 6672 6f6d 2065 7a64 7866 2e61      from ezdxf.a
+000036d0: 6464 6f6e 732e 6870 676c 322e 706c 6f74  ddons.hpgl2.plot
+000036e0: 7465 7220 696d 706f 7274 2061 7263 5f61  ter import arc_a
+000036f0: 6e67 6c65 730d 0a0d 0a20 2020 2061 6e67  ngles....    ang
+00003700: 6c65 7320 3d20 6c69 7374 2861 7263 5f61  les = list(arc_a
+00003710: 6e67 6c65 7328 302c 2033 3630 2c20 3529  ngles(0, 360, 5)
+00003720: 290d 0a20 2020 2061 7373 6572 7420 6c65  )..    assert le
+00003730: 6e28 616e 676c 6573 2920 3d3d 2037 330d  n(angles) == 73.
+00003740: 0a20 2020 2061 7373 6572 7420 616e 676c  .    assert angl
+00003750: 6573 5b2d 315d 203d 3d20 7079 7465 7374  es[-1] == pytest
+00003760: 2e61 7070 726f 7828 3336 3029 0d0a 0d0a  .approx(360)....
+00003770: 2020 2020 616e 676c 6573 203d 206c 6973      angles = lis
+00003780: 7428 6172 635f 616e 676c 6573 2830 2c20  t(arc_angles(0, 
+00003790: 2d33 3630 2c20 3529 290d 0a20 2020 2061  -360, 5))..    a
+000037a0: 7373 6572 7420 6c65 6e28 616e 676c 6573  ssert len(angles
+000037b0: 2920 3d3d 2037 330d 0a20 2020 2061 7373  ) == 73..    ass
+000037c0: 6572 7420 616e 676c 6573 5b2d 315d 203d  ert angles[-1] =
+000037d0: 3d20 7079 7465 7374 2e61 7070 726f 7828  = pytest.approx(
+000037e0: 2d33 3630 290d 0a0d 0a0d 0a64 6566 2074  -360)......def t
+000037f0: 6573 745f 7377 6565 7069 6e67 5f61 6e67  est_sweeping_ang
+00003800: 6c65 2829 3a0d 0a20 2020 2066 726f 6d20  le():..    from 
+00003810: 657a 6478 662e 6164 646f 6e73 2e68 7067  ezdxf.addons.hpg
+00003820: 6c32 2e70 6c6f 7474 6572 2069 6d70 6f72  l2.plotter impor
+00003830: 7420 7377 6565 7069 6e67 5f61 6e67 6c65  t sweeping_angle
+00003840: 0d0a 0d0a 2020 2020 6173 7365 7274 2073  ....    assert s
+00003850: 7765 6570 696e 675f 616e 676c 6528 302c  weeping_angle(0,
+00003860: 2034 352c 2039 3029 203d 3d20 3930 0d0a   45, 90) == 90..
+00003870: 2020 2020 6173 7365 7274 2073 7765 6570      assert sweep
+00003880: 696e 675f 616e 676c 6528 3930 2c20 3435  ing_angle(90, 45
+00003890: 2c20 3029 203d 3d20 2d39 300d 0a20 2020  , 0) == -90..   
+000038a0: 2061 7373 6572 7420 7377 6565 7069 6e67   assert sweeping
+000038b0: 5f61 6e67 6c65 2833 3330 2c20 302c 2033  _angle(330, 0, 3
+000038c0: 3029 203d 3d20 3630 0d0a 2020 2020 6173  0) == 60..    as
+000038d0: 7365 7274 2073 7765 6570 696e 675f 616e  sert sweeping_an
+000038e0: 676c 6528 3333 302c 2031 3830 2c20 3330  gle(330, 180, 30
+000038f0: 2920 3d3d 202d 3330 300d 0a20 2020 2061  ) == -300..    a
+00003900: 7373 6572 7420 7377 6565 7069 6e67 5f61  ssert sweeping_a
+00003910: 6e67 6c65 2833 302c 2030 2c20 3333 3029  ngle(30, 0, 330)
+00003920: 203d 3d20 2d36 300d 0a20 2020 2061 7373   == -60..    ass
+00003930: 6572 7420 7377 6565 7069 6e67 5f61 6e67  ert sweeping_ang
+00003940: 6c65 2833 302c 2031 3830 2c20 3333 3029  le(30, 180, 330)
+00003950: 203d 3d20 3330 300d 0a0d 0a0d 0a63 6c61   == 300......cla
+00003960: 7373 2054 6573 7450 6c61 6365 6d65 6e74  ss TestPlacement
+00003970: 4d61 7472 6978 3a0d 0a20 2020 2064 6566  Matrix:..    def
+00003980: 2074 6573 745f 7368 6966 745f 746f 5f6f   test_shift_to_o
+00003990: 7269 6769 6e5f 5131 2873 656c 6629 3a0d  rigin_Q1(self):.
+000039a0: 0a20 2020 2020 2020 2062 626f 7820 3d20  .        bbox = 
+000039b0: 426f 756e 6469 6e67 426f 7832 6428 5b28  BoundingBox2d([(
+000039c0: 3130 2c20 3130 292c 2028 3230 2c20 3230  10, 10), (20, 20
+000039d0: 295d 290d 0a20 2020 2020 2020 206d 203d  )])..        m =
+000039e0: 2070 6c61 6365 6d65 6e74 5f6d 6174 7269   placement_matri
+000039f0: 7828 6262 6f78 290d 0a20 2020 2020 2020  x(bbox)..       
+00003a00: 2061 7373 6572 7420 6d2e 7472 616e 7366   assert m.transf
+00003a10: 6f72 6d28 2831 302c 2031 3029 292e 6973  orm((10, 10)).is
+00003a20: 636c 6f73 6528 2830 2c20 3029 290d 0a20  close((0, 0)).. 
+00003a30: 2020 2020 2020 2061 7373 6572 7420 6d2e         assert m.
+00003a40: 7472 616e 7366 6f72 6d28 2832 302c 2032  transform((20, 2
+00003a50: 3029 292e 6973 636c 6f73 6528 2831 302c  0)).isclose((10,
+00003a60: 2031 3029 290d 0a0d 0a20 2020 2064 6566   10))....    def
+00003a70: 2074 6573 745f 7368 6966 745f 746f 5f6f   test_shift_to_o
+00003a80: 7269 6769 6e5f 5133 2873 656c 6629 3a0d  rigin_Q3(self):.
+00003a90: 0a20 2020 2020 2020 2062 626f 7820 3d20  .        bbox = 
+00003aa0: 426f 756e 6469 6e67 426f 7832 6428 5b28  BoundingBox2d([(
+00003ab0: 2d31 302c 202d 3130 292c 2028 2d32 302c  -10, -10), (-20,
+00003ac0: 202d 3230 295d 290d 0a20 2020 2020 2020   -20)])..       
+00003ad0: 206d 203d 2070 6c61 6365 6d65 6e74 5f6d   m = placement_m
+00003ae0: 6174 7269 7828 6262 6f78 290d 0a20 2020  atrix(bbox)..   
+00003af0: 2020 2020 2061 7373 6572 7420 6d2e 7472       assert m.tr
+00003b00: 616e 7366 6f72 6d28 282d 3130 2c20 2d31  ansform((-10, -1
+00003b10: 3029 292e 6973 636c 6f73 6528 2831 302c  0)).isclose((10,
+00003b20: 2031 3029 290d 0a20 2020 2020 2020 2061   10))..        a
+00003b30: 7373 6572 7420 6d2e 7472 616e 7366 6f72  ssert m.transfor
+00003b40: 6d28 282d 3230 2c20 2d32 3029 292e 6973  m((-20, -20)).is
+00003b50: 636c 6f73 6528 2830 2c20 3029 290d 0a0d  close((0, 0))...
+00003b60: 0a20 2020 2064 6566 2074 6573 745f 726f  .    def test_ro
+00003b70: 7461 7465 2873 656c 6629 3a0d 0a20 2020  tate(self):..   
+00003b80: 2020 2020 2023 2073 697a 6520 3d20 3130       # size = 10
+00003b90: 2078 2033 300d 0a20 2020 2020 2020 2062   x 30..        b
+00003ba0: 626f 7820 3d20 426f 756e 6469 6e67 426f  box = BoundingBo
+00003bb0: 7832 6428 5b28 3130 2c20 3130 292c 2028  x2d([(10, 10), (
+00003bc0: 3230 2c20 3430 295d 290d 0a20 2020 2020  20, 40)])..     
+00003bd0: 2020 206d 203d 2070 6c61 6365 6d65 6e74     m = placement
+00003be0: 5f6d 6174 7269 7828 6262 6f78 2c20 726f  _matrix(bbox, ro
+00003bf0: 7461 7469 6f6e 3d39 3029 0d0a 2020 2020  tation=90)..    
+00003c00: 2020 2020 6173 7365 7274 206d 2e74 7261      assert m.tra
+00003c10: 6e73 666f 726d 2828 3130 2c20 3130 2929  nsform((10, 10))
+00003c20: 2e69 7363 6c6f 7365 2828 3330 2c20 3029  .isclose((30, 0)
+00003c30: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00003c40: 7420 6d2e 7472 616e 7366 6f72 6d28 2832  t m.transform((2
+00003c50: 302c 2034 3029 292e 6973 636c 6f73 6528  0, 40)).isclose(
+00003c60: 2830 2c20 3130 2929 0d0a 0d0a 0d0a 6966  (0, 10))......if
+00003c70: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
+00003c80: 6d61 696e 5f5f 223a 0d0a 2020 2020 7079  main__":..    py
+00003c90: 7465 7374 2e6d 6169 6e28 5b5f 5f66 696c  test.main([__fil
+00003ca0: 655f 5f5d 290d 0a                        e__])..
```

## Comparing `ezdxf-1.0.4b1/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py` & `ezdxf-1.1.0b0/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_901_acc_vec2.py` & `ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_901_acc_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_902_acc_vec3.py` & `ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_902_acc_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_903_acc_matrix44.py` & `ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_903_acc_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py` & `ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py` & `ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_09_cython_acceleration/test_906_acc_bspline.py` & `ezdxf-1.1.0b0/tests/test_09_cython_acceleration/test_906_acc_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_10_issues/test_issue_414_bbox_calculation.py` & `ezdxf-1.1.0b0/tests/test_10_issues/test_issue_414_bbox_calculation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py` & `ezdxf-1.1.0b0/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_10_issues/test_issue_574_flattening_error.py` & `ezdxf-1.1.0b0/tests/test_10_issues/test_issue_574_flattening_error.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py` & `ezdxf-1.1.0b0/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.0.4b1/tests/test_10_issues/test_issue_749_text_layout.py` & `ezdxf-1.1.0b0/tests/test_10_issues/test_issue_749_text_layout.py`

 * *Files identical despite different names*

