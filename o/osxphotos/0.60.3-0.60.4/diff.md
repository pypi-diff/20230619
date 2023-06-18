# Comparing `tmp/osxphotos-0.60.3.tar.gz` & `tmp/osxphotos-0.60.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osxphotos-0.60.3.tar", last modified: Sun Jun 18 16:54:53 2023, max compression
+gzip compressed data, was "osxphotos-0.60.4.tar", last modified: Sun Jun 18 23:12:12 2023, max compression
```

## Comparing `osxphotos-0.60.3.tar` & `osxphotos-0.60.4.tar`

### file list

```diff
@@ -1,233 +1,233 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.512133 osxphotos-0.60.3/
--rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.3/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.3/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-18 16:54:53.511935 osxphotos-0.60.3/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)   225512 2023-06-18 16:54:41.000000 osxphotos-0.60.3/README.md
--rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.3/README.rst
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.459861 osxphotos-0.60.3/osxphotos/
--rw-r--r--   0 rhet       (501) staff       (20)     1952 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.3/osxphotos/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15945 2023-05-07 15:00:00.000000 osxphotos-0.60.3/osxphotos/_constants.py
--rw-r--r--   0 rhet       (501) staff       (20)       45 2023-06-18 16:54:37.000000 osxphotos-0.60.3/osxphotos/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.3/osxphotos/adjustmentsinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.3/osxphotos/albuminfo.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.468156 osxphotos-0.60.3/osxphotos/cli/
--rw-r--r--   0 rhet       (501) staff       (20)     3565 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.3/osxphotos/cli/about.py
--rw-r--r--   0 rhet       (501) staff       (20)     6869 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/cli/add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/albums.py
--rw-r--r--   0 rhet       (501) staff       (20)     9933 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/cli/batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3802 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/cli/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/cli_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)    27384 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/cli/cli_params.py
--rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/cli/click_rich_echo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.3/osxphotos/cli/color_themes.py
--rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/common.py
--rw-r--r--   0 rhet       (501) staff       (20)      713 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/darkmode.py
--rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/debug_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/docs.py
--rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/cli/dump.py
--rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/exiftool_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)   107273 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/cli/export.py
--rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/grep.py
--rw-r--r--   0 rhet       (501) staff       (20)    22101 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/cli/help.py
--rw-r--r--   0 rhet       (501) staff       (20)    61649 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/cli/import_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/info.py
--rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/install_uninstall_run.py
--rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/keywords.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/kvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/labels.py
--rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/list.py
--rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.3/osxphotos/cli/orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/cli/param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/persons.py
--rw-r--r--   0 rhet       (501) staff       (20)    20564 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/cli/photo_inspect.py
--rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/places.py
--rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/print_photo_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     5674 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/query.py
--rw-r--r--   0 rhet       (501) staff       (20)     8754 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/cli/repl.py
--rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/cli/report_writer.py
--rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.3/osxphotos/cli/rich_progress.py
--rw-r--r--   0 rhet       (501) staff       (20)     3355 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/show_command.py
--rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/snap_diff.py
--rw-r--r--   0 rhet       (501) staff       (20)    26935 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/cli/sync.py
--rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/sync_results.py
--rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.3/osxphotos/cli/theme.py
--rw-r--r--   0 rhet       (501) staff       (20)    28044 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.3/osxphotos/cli/tutorial.py
--rw-r--r--   0 rhet       (501) staff       (20)      692 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/cli/uuid.py
--rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/cli/verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/cli/version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5089 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/compare_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/crash_reporter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.3/osxphotos/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/debug.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.476263 osxphotos-0.60.3/osxphotos/docs/
--rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.3/osxphotos/docs/README.md
--rw-r--r--   0 rhet       (501) staff       (20)  1471429 2023-06-18 16:54:49.000000 osxphotos-0.60.3/osxphotos/docs/docs.zip
--rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/exif_datetime_updater.py
--rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.3/osxphotos/exifinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.3/osxphotos/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.3/osxphotos/exiftool_filetypes.json
--rw-r--r--   0 rhet       (501) staff       (20)    51790 2023-06-17 04:33:59.000000 osxphotos-0.60.3/osxphotos/export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/export_db_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    10742 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/frozen_photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5121 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/imageconverter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.3/osxphotos/momentinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     3787 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/photodates.py
--rw-r--r--   0 rhet       (501) staff       (20)    91520 2023-06-17 14:14:35.000000 osxphotos-0.60.3/osxphotos/photoexporter.py
--rw-r--r--   0 rhet       (501) staff       (20)    84832 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    46258 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     5719 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/photosalbum.py
--rw-r--r--   0 rhet       (501) staff       (20)     5332 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/photoscript_utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.478990 osxphotos-0.60.3/osxphotos/photosdb/
--rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/photosdb/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)    10393 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7576 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)   149944 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/photosdb/photosdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/photosdb/photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.3/osxphotos/phototables.py
--rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.3/osxphotos/phototemplate.cog.md
--rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-06-18 16:54:41.000000 osxphotos-0.60.3/osxphotos/phototemplate.md
--rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/phototemplate.py
--rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.3/osxphotos/phototemplate.tx
--rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/phototz.py
--rw-r--r--   0 rhet       (501) staff       (20)    21858 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.3/osxphotos/pyrepl.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.480338 osxphotos-0.60.3/osxphotos/queries/
--rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.3/osxphotos/queries/README.md
--rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.3/osxphotos/queries/cloud_album_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.3/osxphotos/queries/shared_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.3/osxphotos/queries/title.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.3/osxphotos/query_builder.py
--rw-r--r--   0 rhet       (501) staff       (20)    14179 2023-06-18 16:54:17.000000 osxphotos-0.60.3/osxphotos/queryoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.3/osxphotos/rich_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/sqlgrep.py
--rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.3/osxphotos/sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/template_counter.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.481510 osxphotos-0.60.3/osxphotos/templates/
--rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.3/osxphotos/templates/DESCRIPTION.txt
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/templates/xmp_sidecar.mako
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/templates/xmp_sidecar_beta.mako
--rw-r--r--   0 rhet       (501) staff       (20)     3242 2023-05-07 13:56:16.000000 osxphotos-0.60.3/osxphotos/text_detection.py
--rw-r--r--   0 rhet       (501) staff       (20)     2282 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/timeutils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3442 2023-05-07 14:33:19.000000 osxphotos-0.60.3/osxphotos/timezones.py
--rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.3/osxphotos/tutorial.md
--rw-r--r--   0 rhet       (501) staff       (20)    27213 2023-06-16 15:10:56.000000 osxphotos-0.60.3/osxphotos/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)    18621 2023-06-17 14:12:56.000000 osxphotos-0.60.3/osxphotos/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.460691 osxphotos-0.60.3/osxphotos.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-18 16:54:53.000000 osxphotos-0.60.3/osxphotos.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     6400 2023-06-18 16:54:53.000000 osxphotos-0.60.3/osxphotos.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2023-06-18 16:54:53.000000 osxphotos-0.60.3/osxphotos.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       58 2023-06-18 16:54:53.000000 osxphotos-0.60.3/osxphotos.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      888 2023-06-18 16:54:53.000000 osxphotos-0.60.3/osxphotos.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)       16 2023-06-18 16:54:53.000000 osxphotos-0.60.3/osxphotos.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2023-06-18 16:54:53.512168 osxphotos-0.60.3/setup.cfg
--rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.3/setup.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.511520 osxphotos-0.60.3/tests/
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 16:54:53.511747 osxphotos-0.60.3/tests/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.3/tests/plugins/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.3/tests/plugins/env_vars.py
--rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_10_12_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    11012 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_albums_folders_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     4849 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_albums_folders_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     5334 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_albums_folders_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_bigsur_10_16_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    54731 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)   273142 2023-06-16 16:22:37.000000 osxphotos-0.60.3/tests/test_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     1798 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     4571 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_add_to_album.py
--rw-r--r--   0 rhet       (501) staff       (20)     2218 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_all_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)     6798 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.3/tests/test_cli_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_cli_export_cloud.py
--rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.3/tests/test_cli_export_projects.py
--rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_cli_exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)    29996 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_import.py
--rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_cli_orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     6397 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     3450 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_sync.py
--rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_cli_timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_cli_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_cli_verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.3/tests/test_cloud_owner_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.3/tests/test_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.3/tests/test_concurrent_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.3/tests/test_configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     1946 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2748 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_debug.py
--rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_empty_library_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.3/tests/test_exif_info.py
--rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.3/tests/test_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     9781 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_exiftool_caching.py
--rw-r--r--   0 rhet       (501) staff       (20)    18308 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_export_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     5910 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_export_catalina_10_15_7_use_photos_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.3/tests/test_export_convert_to_jpeg.py
--rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    10301 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_export_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_export_raw_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_exportresults.py
--rw-r--r--   0 rhet       (501) staff       (20)   155137 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.3/tests/test_fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_highsierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     4022 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_image_converter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_incloud_big_sur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.3/tests/test_incloud_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_incloud_catalina_10_15_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1270 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_incloud_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.3/tests/test_live_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)      859 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_modified_date_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)      930 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_modified_date_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.3/tests/test_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1205 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_mojave_10_14_6_path_edited.py
--rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_monterey_12_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    50393 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_monterey_dev_beta_12_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4731 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_movies_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4870 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_movies_5_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    13430 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5796 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_places_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.3/tests/test_places_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.3/tests/test_places_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.3/tests/test_projects_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.3/tests/test_projects_sierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     3376 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_score_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_search_info_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     7530 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_search_info_10_15_4.py
--rw-r--r--   0 rhet       (501) staff       (20)    10047 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_search_info_10_15_5.py
--rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_search_info_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_shared_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_shared_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_shared_ventura_13_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.3/tests/test_sidecar_xmp.py
--rw-r--r--   0 rhet       (501) staff       (20)     3017 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_specials_bigsur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.3/tests/test_specials_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.3/tests/test_specials_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.3/tests/test_specials_sierra_10_12.py
--rw-r--r--   0 rhet       (501) staff       (20)      489 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)    50016 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_template.py
--rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.3/tests/test_template_counter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.3/tests/test_template_today.py
--rw-r--r--   0 rhet       (501) staff       (20)     2032 2023-05-07 13:56:16.000000 osxphotos-0.60.3/tests/test_uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.3/tests/test_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.3/tests/test_ventura_13_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-06-16 15:10:52.000000 osxphotos-0.60.3/tests/test_ventura_dev_preview_13_0_0.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.857297 osxphotos-0.60.4/
+-rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.4/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.4/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-18 23:12:12.857120 osxphotos-0.60.4/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)   225512 2023-06-18 23:12:04.000000 osxphotos-0.60.4/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.4/README.rst
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.823534 osxphotos-0.60.4/osxphotos/
+-rw-r--r--   0 rhet       (501) staff       (20)     1952 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.4/osxphotos/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15962 2023-06-18 23:09:24.000000 osxphotos-0.60.4/osxphotos/_constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2023-06-18 23:11:07.000000 osxphotos-0.60.4/osxphotos/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.4/osxphotos/adjustmentsinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.4/osxphotos/albuminfo.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.830564 osxphotos-0.60.4/osxphotos/cli/
+-rw-r--r--   0 rhet       (501) staff       (20)     3565 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.4/osxphotos/cli/about.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6869 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/cli/add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/albums.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9933 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/cli/batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3802 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/cli/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/cli_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27384 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/cli/cli_params.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/cli/click_rich_echo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.4/osxphotos/cli/color_themes.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3555 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/common.py
+-rw-r--r--   0 rhet       (501) staff       (20)      713 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/darkmode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/debug_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/docs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/cli/dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/exiftool_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)   107273 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/cli/export.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/grep.py
+-rw-r--r--   0 rhet       (501) staff       (20)    22101 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/cli/help.py
+-rw-r--r--   0 rhet       (501) staff       (20)    61649 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/cli/import_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/install_uninstall_run.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/keywords.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/kvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/labels.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/list.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.4/osxphotos/cli/orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/cli/param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/persons.py
+-rw-r--r--   0 rhet       (501) staff       (20)    20564 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/cli/photo_inspect.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/places.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/print_photo_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5674 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/query.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8754 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/cli/repl.py
+-rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/cli/report_writer.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.4/osxphotos/cli/rich_progress.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3355 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/show_command.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/snap_diff.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26935 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/cli/sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/sync_results.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.4/osxphotos/cli/theme.py
+-rw-r--r--   0 rhet       (501) staff       (20)    28044 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.4/osxphotos/cli/tutorial.py
+-rw-r--r--   0 rhet       (501) staff       (20)      692 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/cli/uuid.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/cli/verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1260 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/cli/version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5089 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/compare_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/crash_reporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.4/osxphotos/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/debug.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.830953 osxphotos-0.60.4/osxphotos/docs/
+-rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.4/osxphotos/docs/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)  1460158 2023-06-18 23:12:09.000000 osxphotos-0.60.4/osxphotos/docs/docs.zip
+-rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/exif_datetime_updater.py
+-rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.4/osxphotos/exifinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.4/osxphotos/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.4/osxphotos/exiftool_filetypes.json
+-rw-r--r--   0 rhet       (501) staff       (20)    51790 2023-06-17 04:33:59.000000 osxphotos-0.60.4/osxphotos/export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/export_db_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10742 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/frozen_photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5121 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/imageconverter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.4/osxphotos/momentinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3787 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/photodates.py
+-rw-r--r--   0 rhet       (501) staff       (20)    91520 2023-06-17 14:14:35.000000 osxphotos-0.60.4/osxphotos/photoexporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)    84832 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    46258 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5719 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/photosalbum.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5332 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/photoscript_utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.832965 osxphotos-0.60.4/osxphotos/photosdb/
+-rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/photosdb/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5386 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10393 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7576 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)   149944 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/photosdb/photosdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/photosdb/photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.4/osxphotos/phototables.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.4/osxphotos/phototemplate.cog.md
+-rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-06-18 23:12:03.000000 osxphotos-0.60.4/osxphotos/phototemplate.md
+-rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/phototemplate.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.4/osxphotos/phototemplate.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/phototz.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21858 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.4/osxphotos/pyrepl.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.833967 osxphotos-0.60.4/osxphotos/queries/
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.4/osxphotos/queries/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.4/osxphotos/queries/cloud_album_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.4/osxphotos/queries/shared_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.4/osxphotos/queries/title.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.4/osxphotos/query_builder.py
+-rw-r--r--   0 rhet       (501) staff       (20)    14179 2023-06-18 16:54:17.000000 osxphotos-0.60.4/osxphotos/queryoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.4/osxphotos/rich_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/sqlgrep.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.4/osxphotos/sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/template_counter.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.834806 osxphotos-0.60.4/osxphotos/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.4/osxphotos/templates/DESCRIPTION.txt
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/templates/xmp_sidecar.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/templates/xmp_sidecar_beta.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     3242 2023-05-07 13:56:16.000000 osxphotos-0.60.4/osxphotos/text_detection.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2282 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/timeutils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3442 2023-05-07 14:33:19.000000 osxphotos-0.60.4/osxphotos/timezones.py
+-rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.4/osxphotos/tutorial.md
+-rw-r--r--   0 rhet       (501) staff       (20)    27213 2023-06-16 15:10:56.000000 osxphotos-0.60.4/osxphotos/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18621 2023-06-17 14:12:56.000000 osxphotos-0.60.4/osxphotos/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.824336 osxphotos-0.60.4/osxphotos.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-06-18 23:12:12.000000 osxphotos-0.60.4/osxphotos.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     6400 2023-06-18 23:12:12.000000 osxphotos-0.60.4/osxphotos.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2023-06-18 23:12:12.000000 osxphotos-0.60.4/osxphotos.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       58 2023-06-18 23:12:12.000000 osxphotos-0.60.4/osxphotos.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      888 2023-06-18 23:12:12.000000 osxphotos-0.60.4/osxphotos.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       16 2023-06-18 23:12:12.000000 osxphotos-0.60.4/osxphotos.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2023-06-18 23:12:12.857334 osxphotos-0.60.4/setup.cfg
+-rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.4/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.856639 osxphotos-0.60.4/tests/
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-06-18 23:12:12.856906 osxphotos-0.60.4/tests/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.4/tests/plugins/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.4/tests/plugins/env_vars.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4551 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_10_12_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11012 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_albums_folders_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4849 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_albums_folders_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5334 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_albums_folders_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43710 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_bigsur_10_16_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    54731 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)   273142 2023-06-16 16:22:37.000000 osxphotos-0.60.4/tests/test_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1798 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4571 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_add_to_album.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2218 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_all_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6798 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.4/tests/test_cli_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_cli_export_cloud.py
+-rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.4/tests/test_cli_export_projects.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_cli_exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)    29996 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_import.py
+-rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_cli_orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6397 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3450 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_cli_timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_cli_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3057 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_cli_verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.4/tests/test_cloud_owner_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.4/tests/test_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.4/tests/test_concurrent_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.4/tests/test_configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1946 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2748 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_debug.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2209 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_empty_library_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.4/tests/test_exif_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.4/tests/test_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9781 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_exiftool_caching.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18308 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_export_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5910 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_export_catalina_10_15_7_use_photos_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.4/tests/test_export_convert_to_jpeg.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10301 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_export_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_export_raw_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2484 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_exportresults.py
+-rw-r--r--   0 rhet       (501) staff       (20)   155137 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.4/tests/test_fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3634 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_highsierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4022 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_image_converter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_incloud_big_sur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.4/tests/test_incloud_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_incloud_catalina_10_15_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1270 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_incloud_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.4/tests/test_live_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)      859 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_modified_date_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)      930 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_modified_date_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.4/tests/test_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1205 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_mojave_10_14_6_path_edited.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43640 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_monterey_12_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50393 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_monterey_dev_beta_12_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4731 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_movies_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4870 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_movies_5_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3780 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13430 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5796 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_places_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.4/tests/test_places_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.4/tests/test_places_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.4/tests/test_projects_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.4/tests/test_projects_sierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3376 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_score_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3696 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_search_info_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7530 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_search_info_10_15_4.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10047 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_search_info_10_15_5.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_search_info_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_shared_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_shared_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_shared_ventura_13_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.4/tests/test_sidecar_xmp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3017 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_specials_bigsur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.4/tests/test_specials_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.4/tests/test_specials_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.4/tests/test_specials_sierra_10_12.py
+-rw-r--r--   0 rhet       (501) staff       (20)      489 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50016 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.4/tests/test_template_counter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.4/tests/test_template_today.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2032 2023-05-07 13:56:16.000000 osxphotos-0.60.4/tests/test_uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.4/tests/test_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.4/tests/test_ventura_13_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43504 2023-06-16 15:10:52.000000 osxphotos-0.60.4/tests/test_ventura_dev_preview_13_0_0.py
```

### Comparing `osxphotos-0.60.3/LICENSE` & `osxphotos-0.60.4/LICENSE`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/PKG-INFO` & `osxphotos-0.60.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.3
+Version: 0.60.4
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.3/README.md` & `osxphotos-0.60.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 The export and query CLI commands as well as the Python API will work on Linux which enables you to export photos
 from a Photos library on a Linux machine.
 
 Tested on macOS Sierra (10.12.6) through macOS Ventura (13.3). Tested on both x86 and Apple silicon (M1).
 
 | macOS Version     | macOS name | Photos.app version |
 | ----------------- |------------|:-------------------|
-| 13.0 - 13.3       | Ventura    | 8.0 ✅             |
+| 13.0 - 13.4       | Ventura    | 8.0 ✅             |
 | 12.0 - 12.6       | Monterey   | 7.0 ✅             |
 | 10.16, 11.0-11.4  | Big Sur    | 6.0 ✅             |
 | 10.15.1 - 10.15.7 | Catalina   | 5.0 ✅             |
 | 10.14.5, 10.14.6  | Mojave     | 4.0 ✅             |
 | 10.13.6           | High Sierra| 3.0 ✅             |
 | 10.12.6           | Sierra     | 2.0 ✅             |
 
@@ -2105,15 +2105,15 @@
 {openbracket}                   An open bracket: '['
 {closebracket}                  A close bracket: ']'
 {newline}                       A newline: '\n'
 {lf}                            A line feed: '\n', alias for {newline}
 {cr}                            A carriage return: '\r'
 {crlf}                          A carriage return + line feed: '\r\n'
 {tab}                           :A tab: '\t'
-{osxphotos_version}             The osxphotos version, e.g. '0.60.3'
+{osxphotos_version}             The osxphotos version, e.g. '0.60.4'
 {osxphotos_cmd_line}            The full command line used to run osxphotos
 
 The following substitutions may result in multiple values. Thus if specified
 for --directory these could result in multiple copies of a photo being being
 exported, one to each directory.  For example: --directory
 '{created.year}/{album}' could result in the same photo being exported to each
 of the following directories if the photos were created in 2019 and were in
@@ -2592,15 +2592,15 @@
 |{openbracket}|An open bracket: '['|
 |{closebracket}|A close bracket: ']'|
 |{newline}|A newline: '\n'|
 |{lf}|A line feed: '\n', alias for {newline}|
 |{cr}|A carriage return: '\r'|
 |{crlf}|A carriage return + line feed: '\r\n'|
 |{tab}|:A tab: '\t'|
-|{osxphotos_version}|The osxphotos version, e.g. '0.60.3'|
+|{osxphotos_version}|The osxphotos version, e.g. '0.60.4'|
 |{osxphotos_cmd_line}|The full command line used to run osxphotos|
 |{album}|Album(s) photo is contained in|
 |{folder_album}|Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{project}|Project(s) photo is contained in (such as greeting cards, calendars, slideshows)|
 |{album_project}|Album(s) and project(s) photo is contained in; treats projects as regular albums|
 |{folder_album_project}|Folder path + album (includes projects as albums) photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{keyword}|Keyword(s) assigned to photo|
```

### Comparing `osxphotos-0.60.3/README.rst` & `osxphotos-0.60.4/README.rst`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/__init__.py` & `osxphotos-0.60.4/osxphotos/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/_constants.py` & `osxphotos-0.60.4/osxphotos/_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
     ("12", "4"),
     ("12", "5"),
     ("12", "6"),
     ("13", "0"),
     ("13", "1"),
     ("13", "2"),
     ("13", "3"),
+    ("13", "4"),
 ]
 
 # Photos 5 has persons who are empty string if unidentified face
 _UNKNOWN_PERSON = "_UNKNOWN_"
 
 # photos with no reverse geolocation info (place)
 _UNKNOWN_PLACE = "_UNKNOWN_"
```

### Comparing `osxphotos-0.60.3/osxphotos/adjustmentsinfo.py` & `osxphotos-0.60.4/osxphotos/adjustmentsinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/albuminfo.py` & `osxphotos-0.60.4/osxphotos/albuminfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/__init__.py` & `osxphotos-0.60.4/osxphotos/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/about.py` & `osxphotos-0.60.4/osxphotos/cli/about.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/add_locations.py` & `osxphotos-0.60.4/osxphotos/cli/add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/albums.py` & `osxphotos-0.60.4/osxphotos/cli/albums.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/batch_edit.py` & `osxphotos-0.60.4/osxphotos/cli/batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/cli.py` & `osxphotos-0.60.4/osxphotos/cli/cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/cli_commands.py` & `osxphotos-0.60.4/osxphotos/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/cli_params.py` & `osxphotos-0.60.4/osxphotos/cli/cli_params.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/click_rich_echo.py` & `osxphotos-0.60.4/osxphotos/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/color_themes.py` & `osxphotos-0.60.4/osxphotos/cli/color_themes.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/common.py` & `osxphotos-0.60.4/osxphotos/cli/common.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/darkmode.py` & `osxphotos-0.60.4/osxphotos/cli/darkmode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/debug_dump.py` & `osxphotos-0.60.4/osxphotos/cli/debug_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/docs.py` & `osxphotos-0.60.4/osxphotos/cli/docs.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/dump.py` & `osxphotos-0.60.4/osxphotos/cli/dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/exiftool_cli.py` & `osxphotos-0.60.4/osxphotos/cli/exiftool_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/export.py` & `osxphotos-0.60.4/osxphotos/cli/export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/exportdb.py` & `osxphotos-0.60.4/osxphotos/cli/exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/grep.py` & `osxphotos-0.60.4/osxphotos/cli/grep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/help.py` & `osxphotos-0.60.4/osxphotos/cli/help.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/import_cli.py` & `osxphotos-0.60.4/osxphotos/cli/import_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/info.py` & `osxphotos-0.60.4/osxphotos/cli/info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/install_uninstall_run.py` & `osxphotos-0.60.4/osxphotos/cli/install_uninstall_run.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/keywords.py` & `osxphotos-0.60.4/osxphotos/cli/keywords.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/kvstore.py` & `osxphotos-0.60.4/osxphotos/cli/kvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/labels.py` & `osxphotos-0.60.4/osxphotos/cli/labels.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/list.py` & `osxphotos-0.60.4/osxphotos/cli/list.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/orphans.py` & `osxphotos-0.60.4/osxphotos/cli/orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/param_types.py` & `osxphotos-0.60.4/osxphotos/cli/param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/persons.py` & `osxphotos-0.60.4/osxphotos/cli/persons.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/photo_inspect.py` & `osxphotos-0.60.4/osxphotos/cli/photo_inspect.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/places.py` & `osxphotos-0.60.4/osxphotos/cli/places.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/print_photo_info.py` & `osxphotos-0.60.4/osxphotos/cli/print_photo_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/query.py` & `osxphotos-0.60.4/osxphotos/cli/query.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/repl.py` & `osxphotos-0.60.4/osxphotos/cli/repl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/report_writer.py` & `osxphotos-0.60.4/osxphotos/cli/report_writer.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/rich_progress.py` & `osxphotos-0.60.4/osxphotos/cli/rich_progress.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/show_command.py` & `osxphotos-0.60.4/osxphotos/cli/show_command.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/snap_diff.py` & `osxphotos-0.60.4/osxphotos/cli/snap_diff.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/sync.py` & `osxphotos-0.60.4/osxphotos/cli/sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/sync_results.py` & `osxphotos-0.60.4/osxphotos/cli/sync_results.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/theme.py` & `osxphotos-0.60.4/osxphotos/cli/theme.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/timewarp.py` & `osxphotos-0.60.4/osxphotos/cli/timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/tutorial.py` & `osxphotos-0.60.4/osxphotos/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/uuid.py` & `osxphotos-0.60.4/osxphotos/cli/uuid.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/verbose.py` & `osxphotos-0.60.4/osxphotos/cli/verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/cli/version.py` & `osxphotos-0.60.4/osxphotos/cli/version.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/compare_exif.py` & `osxphotos-0.60.4/osxphotos/compare_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/configoptions.py` & `osxphotos-0.60.4/osxphotos/configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/crash_reporter.py` & `osxphotos-0.60.4/osxphotos/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/datetime_formatter.py` & `osxphotos-0.60.4/osxphotos/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/datetime_utils.py` & `osxphotos-0.60.4/osxphotos/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/debug.py` & `osxphotos-0.60.4/osxphotos/debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/docs/docs.zip` & `osxphotos-0.60.4/osxphotos/docs/docs.zip`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1471429 bytes, number of entries: 99
+Zip file size: 1460158 bytes, number of entries: 99
 -rw-r--r--  3.0 unx   331458 tx defN 23-Feb-12 16:23 docs/API_README.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_modules/
--rw-r--r--  3.0 unx    11779 tx defN 23-Jun-18 16:54 docs/_modules/index.html
+-rw-r--r--  3.0 unx    11779 tx defN 23-Jun-18 23:12 docs/_modules/index.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:15 docs/_modules/osxphotos/
 -rw-r--r--  3.0 unx   324766 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/photoexporter.html
 -rw-r--r--  3.0 unx   296439 tx defN 23-May-07 14:38 docs/_modules/osxphotos/phototemplate.html
 -rw-r--r--  3.0 unx   201027 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/export_db.html
 -rw-r--r--  3.0 unx    14791 tx defN 23-Jun-17 14:16 docs/_modules/osxphotos/scoreinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:55 docs/_modules/osxphotos/photoinfo/
 -rw-r--r--  3.0 unx    14017 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
@@ -24,78 +24,78 @@
 -rw-r--r--  3.0 unx    92802 tx defN 23-May-07 14:38 docs/_modules/osxphotos/placeinfo.html
 -rw-r--r--  3.0 unx    21299 tx defN 22-May-06 00:24 docs/_modules/osxphotos/momentinfo.html
 -rw-r--r--  3.0 unx    82289 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/albuminfo.html
 -rw-r--r--  3.0 unx    78750 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/exiftool.html
 -rw-r--r--  3.0 unx    26012 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/debug.html
 -rw-r--r--  3.0 unx    61579 tx defN 23-Jun-18 16:54 docs/_modules/osxphotos/queryoptions.html
 -rw-r--r--  3.0 unx    80476 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/personinfo.html
--rw-r--r--  3.0 unx    61850 tx defN 23-May-14 15:28 docs/_modules/osxphotos/_constants.html
+-rw-r--r--  3.0 unx    62004 tx defN 23-Jun-18 23:11 docs/_modules/osxphotos/_constants.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-12 16:20 docs/_sources/
 -rw-r--r--  3.0 unx      198 tx defN 22-Apr-23 14:44 docs/_sources/cli.rst.txt
--rw-r--r--  3.0 unx    31854 tx defN 23-Jun-18 16:54 docs/_sources/template_help.rst.txt
+-rw-r--r--  3.0 unx    31854 tx defN 23-Jun-18 23:11 docs/_sources/template_help.rst.txt
 -rw-r--r--  3.0 unx    31240 tx defN 21-Apr-26 18:30 docs/_sources/tutorial.md.txt
 -rw-r--r--  3.0 unx       52 tx defN 21-Jan-24 17:13 docs/_sources/modules.rst.txt
 -rw-r--r--  3.0 unx    41238 tx defN 22-Aug-27 16:24 docs/_sources/tutorial.rst.txt
 -rw-r--r--  3.0 unx       93 tx defN 23-Feb-12 16:23 docs/_sources/reference.rst.txt
 -rw-r--r--  3.0 unx     7548 tx defN 22-Apr-23 18:28 docs/_sources/package_overview.rst.txt
 -rw-r--r--  3.0 unx      149 tx defN 22-Apr-21 04:29 docs/_sources/cli_export.rst.txt
 -rw-r--r--  3.0 unx   147706 tx defN 23-Feb-12 16:20 docs/_sources/API_README.rst.txt
 -rw-r--r--  3.0 unx      502 tx defN 23-Feb-12 16:24 docs/_sources/index.rst.txt
 -rw-r--r--  3.0 unx     4241 tx defN 22-May-01 15:46 docs/_sources/overview.rst.txt
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_static/
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/plus.png
 -rw-r--r--  3.0 unx     4712 tx defN 22-Nov-13 03:13 docs/_static/sphinx_highlight.js
 -rw-r--r--  3.0 unx    19530 tx defN 21-Jun-05 18:07 docs/_static/underscore.js
 -rw-r--r--  3.0 unx    11185 tx defN 21-Mar-22 05:50 docs/_static/alabaster.css
--rw-r--r--  3.0 unx      421 tx defN 23-Jun-18 16:54 docs/_static/documentation_options.js
+-rw-r--r--  3.0 unx      421 tx defN 23-Jun-18 23:12 docs/_static/documentation_options.js
 -rw-r--r--  3.0 unx    18215 tx defN 22-Nov-13 03:13 docs/_static/searchtools.js
 -rw-r--r--  3.0 unx     1266 tx defN 22-Nov-13 03:13 docs/_static/debug.css
 -rw-r--r--  3.0 unx      313 tx defN 22-Apr-21 05:12 docs/_static/check-solid.svg
 -rw-r--r--  3.0 unx     9031 tx defN 22-Apr-21 05:12 docs/_static/clipboard.min.js
 -rw-r--r--  3.0 unx      286 bx stor 21-Mar-14 19:14 docs/_static/file.png
 -rw-r--r--  3.0 unx     4418 tx defN 22-Nov-13 03:13 docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     8472 tx defN 23-Jun-18 16:54 docs/_static/copybutton.js
+-rw-r--r--  3.0 unx     8472 tx defN 23-Jun-18 23:12 docs/_static/copybutton.js
 -rw-r--r--  3.0 unx   287630 tx defN 21-Mar-14 19:14 docs/_static/jquery-3.5.1.js
 -rw-r--r--  3.0 unx       42 tx stor 21-Mar-14 19:14 docs/_static/custom.css
--rw-r--r--  3.0 unx     4758 tx defN 23-Jun-18 16:54 docs/_static/language_data.js
+-rw-r--r--  3.0 unx     4758 tx defN 23-Jun-18 23:12 docs/_static/language_data.js
 -rw-r--r--  3.0 unx      411 tx defN 22-Apr-21 05:12 docs/_static/copy-button.svg
 -rw-r--r--  3.0 unx     2698 tx defN 22-Dec-03 06:57 docs/_static/copybutton_funcs.js
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/minus.png
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-24 15:32 docs/_static/styles/
 -rw-r--r--  3.0 unx    72647 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css.map
 -rw-r--r--  3.0 unx     5529 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css
 -rw-r--r--  3.0 unx    48032 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css
 -rw-r--r--  3.0 unx     7809 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css.map
 -rw-r--r--  3.0 unx     6034 tx defN 22-Nov-13 03:13 docs/_static/skeleton.css
 -rw-r--r--  3.0 unx   288580 tx defN 22-Nov-13 03:13 docs/_static/jquery-3.6.0.js
--rw-r--r--  3.0 unx    14810 tx defN 23-Jun-18 16:54 docs/_static/basic.css
+-rw-r--r--  3.0 unx    14810 tx defN 23-Jun-18 23:12 docs/_static/basic.css
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:21 docs/_static/scripts/
 -rw-r--r--  3.0 unx      187 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js.LICENSE.txt
 -rw-r--r--  3.0 unx    28242 tx defN 22-Nov-13 03:13 docs/_static/scripts/furo.js.map
 -rw-r--r--  3.0 unx        0 bx stor 22-Apr-21 04:34 docs/_static/scripts/furo-extensions.js
 -rw-r--r--  3.0 unx     5265 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js
--rw-r--r--  3.0 unx    21072 tx defN 23-Jun-18 16:54 docs/_static/pygments.css
+-rw-r--r--  3.0 unx    21072 tx defN 23-Jun-18 23:12 docs/_static/pygments.css
 -rw-r--r--  3.0 unx     2060 tx defN 22-Dec-03 06:57 docs/_static/copybutton.css
 -rw-r--r--  3.0 unx     4472 tx defN 22-Nov-13 03:13 docs/_static/doctools.js
 -rw-r--r--  3.0 unx    67692 tx defN 21-Mar-14 19:14 docs/_static/underscore-1.12.0.js
 -rw-r--r--  3.0 unx    89501 tx defN 22-Nov-13 03:13 docs/_static/jquery.js
 -rw-r--r--  3.0 unx    68420 tx defN 21-Jun-05 18:07 docs/_static/underscore-1.13.1.js
--rw-r--r--  3.0 unx   423685 tx defN 23-Jun-18 16:54 docs/cli.html
+-rw-r--r--  3.0 unx   423685 tx defN 23-Jun-18 23:11 docs/cli.html
 -rw-r--r--  3.0 unx    85854 tx defN 22-Apr-21 04:30 docs/cli_export.html
--rw-r--r--  3.0 unx   249535 tx defN 23-Jun-18 16:54 docs/genindex.html
--rw-r--r--  3.0 unx   105318 tx defN 23-Jun-18 16:54 docs/index.html
+-rw-r--r--  3.0 unx   249535 tx defN 23-Jun-18 23:12 docs/genindex.html
+-rw-r--r--  3.0 unx   105318 tx defN 23-Jun-18 23:12 docs/index.html
 -rw-r--r--  3.0 unx     2984 tx defN 22-Apr-20 14:01 docs/modules.html
--rw-r--r--  3.0 unx     9610 bx stor 23-Jun-18 16:54 docs/objects.inv
+-rw-r--r--  3.0 unx     9610 bx stor 23-Jun-18 23:12 docs/objects.inv
 -rw-r--r--  3.0 unx   267506 bx defN 21-May-10 00:50 docs/osxphotos.pdf
--rw-r--r--  3.0 unx    26446 tx defN 23-Jun-18 16:54 docs/overview.html
--rw-r--r--  3.0 unx    32469 tx defN 23-Jun-18 16:54 docs/package_overview.html
--rw-r--r--  3.0 unx    10831 tx defN 23-Jun-18 16:54 docs/py-modindex.html
--rw-r--r--  3.0 unx   446001 tx defN 23-Jun-18 16:54 docs/reference.html
+-rw-r--r--  3.0 unx    26446 tx defN 23-Jun-18 23:11 docs/overview.html
+-rw-r--r--  3.0 unx    32469 tx defN 23-Jun-18 23:11 docs/package_overview.html
+-rw-r--r--  3.0 unx    10831 tx defN 23-Jun-18 23:12 docs/py-modindex.html
+-rw-r--r--  3.0 unx   446001 tx defN 23-Jun-18 23:11 docs/reference.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:53 docs/screencast/
 -rw-r--r--  3.0 unx     8007 tx defN 21-Jan-24 17:13 docs/screencast/terminalizer-demo.yml
 -rw-r--r--  3.0 unx    77927 bx defN 21-Jan-24 17:13 docs/screencast/osx-screenshot.png
 -rw-r--r--  3.0 unx   224316 bx defN 21-Jan-24 17:13 docs/screencast/demo.gif
--rw-r--r--  3.0 unx    10567 tx defN 23-Jun-18 16:54 docs/search.html
--rw-r--r--  3.0 unx   220592 tx defN 23-Jun-18 16:54 docs/searchindex.js
--rw-r--r--  3.0 unx    64566 tx defN 23-Jun-18 16:54 docs/template_help.html
--rw-r--r--  3.0 unx    84995 tx defN 23-Jun-18 16:54 docs/tutorial.html
-99 files, 6958938 bytes uncompressed, 1452697 bytes compressed:  79.1%
+-rw-r--r--  3.0 unx    10567 tx defN 23-Jun-18 23:12 docs/search.html
+-rw-r--r--  3.0 unx   113489 tx defN 23-Jun-18 23:12 docs/searchindex.js
+-rw-r--r--  3.0 unx    64566 tx defN 23-Jun-18 23:12 docs/template_help.html
+-rw-r--r--  3.0 unx    84995 tx defN 23-Jun-18 23:12 docs/tutorial.html
+99 files, 6851989 bytes uncompressed, 1441426 bytes compressed:  79.0%
```

#### docs/_modules/index.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>Overview: module code - osxphotos 0.60.3 documentation</title>
+        <title>Overview: module code - osxphotos 0.60.4 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="../index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/_constants.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos._constants - osxphotos 0.60.1 documentation</title>
+        <title>osxphotos._constants - osxphotos 0.60.4 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.1 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.1 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -322,14 +322,15 @@
     <span class="p">(</span><span class="s2">&quot;12&quot;</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;12&quot;</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;12&quot;</span><span class="p">,</span> <span class="s2">&quot;6&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;0&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;1&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">),</span>
+    <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">),</span>
 <span class="p">]</span>
 
 <span class="c1"># Photos 5 has persons who are empty string if unidentified face</span>
 <span class="n">_UNKNOWN_PERSON</span> <span class="o">=</span> <span class="s2">&quot;_UNKNOWN_&quot;</span>
 
 <span class="c1"># photos with no reverse geolocation info (place)</span>
 <span class="n">_UNKNOWN_PLACE</span> <span class="o">=</span> <span class="s2">&quot;_UNKNOWN_&quot;</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.4_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.1_documentation
+osxphotos_0.60.4_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -165,14 +165,15 @@
     ("12", "4"),
     ("12", "5"),
     ("12", "6"),
     ("13", "0"),
     ("13", "1"),
     ("13", "2"),
     ("13", "3"),
+    ("13", "4"),
 ]
 
 # Photos 5 has persons who are empty string if unidentified face
 _UNKNOWN_PERSON = "_UNKNOWN_"
 
 # photos with no reverse geolocation info (place)
 _UNKNOWN_PLACE = "_UNKNOWN_"
```

#### docs/_sources/template_help.rst.txt

```diff
@@ -357,15 +357,15 @@
    * - {cr}
      - A carriage return: '\r'
    * - {crlf}
      - A carriage return + line feed: '\r\n'
    * - {tab}
      - :A tab: '\t'
    * - {osxphotos_version}
-     - The osxphotos version, e.g. '0.60.3'
+     - The osxphotos version, e.g. '0.60.4'
    * - {osxphotos_cmd_line}
      - The full command line used to run osxphotos
    * - {album}
      - Album(s) photo is contained in
    * - {folder_album}
      - Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder
    * - {project}
```

#### docs/_static/documentation_options.js

##### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 var DOCUMENTATION_OPTIONS = {
     URL_ROOT: document.getElementById("documentation_options").getAttribute('data-url_root'),
-    VERSION: '0.60.3',
+    VERSION: '0.60.4',
     LANGUAGE: 'en',
     COLLAPSE_INDEX: false,
     BUILDER: 'html',
     FILE_SUFFIX: '.html',
     LINK_SUFFIX: '.html',
     HAS_SOURCE: true,
     SOURCELINK_SUFFIX: '.txt',
```

#### docs/cli.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Template System" href="template_help.html" /><link rel="prev" title="OSXPhotos Tutorial" href="tutorial.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.3 documentation</title>
+        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.4 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/genindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.3 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.4 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/index.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos 0.60.3 documentation</title>
+        <title>osxphotos 0.60.4 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="#"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="#"><div class="brand">osxphotos 0.60.4 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="#">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Tutorial" href="tutorial.html" /><link rel="prev" title="Welcome to OSXPhotos’s documentation!" href="index.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos - osxphotos 0.60.3 documentation</title>
+        <title>OSXPhotos - osxphotos 0.60.4 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/package_overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Reference" href="reference.html" /><link rel="prev" title="OSXPhotos Template System" href="template_help.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Package Overview - osxphotos 0.60.3 documentation</title>
+        <title>OSXPhotos Python Package Overview - osxphotos 0.60.4 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/py-modindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.3 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.4 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/reference.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="OSXPhotos Python Package Overview" href="package_overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Reference - osxphotos 0.60.3 documentation</title>
+        <title>OSXPhotos Python Reference - osxphotos 0.60.4 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/search.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.3 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.4 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
 
@@ -117,15 +117,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -140,15 +140,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="#" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/searchindex.js

##### js-beautify {}

```diff
@@ -4111,3275 +4111,9 @@
         "Color Themes": [
             [6, "color-themes"]
         ],
         "Conclusion": [
             [6, "conclusion"]
         ]
     },
-    "indexentries": {
-        "--add-exported-to-album": [
-            [0, "cmdoption-osxphotos-export-add-exported-to-album"]
-        ],
-        "--add-missing-to-album": [
-            [0, "cmdoption-osxphotos-export-add-missing-to-album"]
-        ],
-        "--add-skipped-to-album": [
-            [0, "cmdoption-osxphotos-export-add-skipped-to-album"]
-        ],
-        "--add-to-album": [
-            [0, "cmdoption-osxphotos-query-add-to-album"],
-            [0, "cmdoption-osxphotos-timewarp-a"]
-        ],
-        "--added-after": [
-            [0, "cmdoption-osxphotos-add-locations-added-after"],
-            [0, "cmdoption-osxphotos-export-added-after"],
-            [0, "cmdoption-osxphotos-query-added-after"],
-            [0, "cmdoption-osxphotos-repl-added-after"],
-            [0, "cmdoption-osxphotos-sync-added-after"]
-        ],
-        "--added-before": [
-            [0, "cmdoption-osxphotos-add-locations-added-before"],
-            [0, "cmdoption-osxphotos-export-added-before"],
-            [0, "cmdoption-osxphotos-query-added-before"],
-            [0, "cmdoption-osxphotos-repl-added-before"],
-            [0, "cmdoption-osxphotos-sync-added-before"]
-        ],
-        "--added-in-last": [
-            [0, "cmdoption-osxphotos-add-locations-added-in-last"],
-            [0, "cmdoption-osxphotos-export-added-in-last"],
-            [0, "cmdoption-osxphotos-query-added-in-last"],
-            [0, "cmdoption-osxphotos-repl-added-in-last"],
-            [0, "cmdoption-osxphotos-sync-added-in-last"]
-        ],
-        "--album": [
-            [0, "cmdoption-osxphotos-add-locations-album"],
-            [0, "cmdoption-osxphotos-export-album"],
-            [0, "cmdoption-osxphotos-import-a"],
-            [0, "cmdoption-osxphotos-query-album"],
-            [0, "cmdoption-osxphotos-repl-album"],
-            [0, "cmdoption-osxphotos-sync-album"]
-        ],
-        "--album-keyword": [
-            [0, "cmdoption-osxphotos-exiftool-album-keyword"],
-            [0, "cmdoption-osxphotos-export-album-keyword"]
-        ],
-        "--alt-copy": [
-            [0, "cmdoption-osxphotos-export-alt-copy"]
-        ],
-        "--append": [
-            [0, "cmdoption-osxphotos-exiftool-append"],
-            [0, "cmdoption-osxphotos-export-append"],
-            [0, "cmdoption-osxphotos-exportdb-append"],
-            [0, "cmdoption-osxphotos-import-append"],
-            [0, "cmdoption-osxphotos-sync-A"]
-        ],
-        "--burst": [
-            [0, "cmdoption-osxphotos-add-locations-burst"],
-            [0, "cmdoption-osxphotos-export-burst"],
-            [0, "cmdoption-osxphotos-query-burst"],
-            [0, "cmdoption-osxphotos-repl-burst"],
-            [0, "cmdoption-osxphotos-sync-burst"]
-        ],
-        "--check-signatures": [
-            [0, "cmdoption-osxphotos-exportdb-check-signatures"]
-        ],
-        "--check-templates": [
-            [0, "cmdoption-osxphotos-import-check-templates"]
-        ],
-        "--cleanup": [
-            [0, "cmdoption-osxphotos-export-cleanup"]
-        ],
-        "--clear-location": [
-            [0, "cmdoption-osxphotos-import-L"]
-        ],
-        "--clear-metadata": [
-            [0, "cmdoption-osxphotos-import-C"]
-        ],
-        "--clone": [
-            [0, "cmdoption-osxphotos-theme-clone"]
-        ],
-        "--cloudasset": [
-            [0, "cmdoption-osxphotos-add-locations-cloudasset"],
-            [0, "cmdoption-osxphotos-export-cloudasset"],
-            [0, "cmdoption-osxphotos-query-cloudasset"],
-            [0, "cmdoption-osxphotos-repl-cloudasset"],
-            [0, "cmdoption-osxphotos-sync-cloudasset"]
-        ],
-        "--compare-exif": [
-            [0, "cmdoption-osxphotos-timewarp-c"]
-        ],
-        "--config": [
-            [0, "cmdoption-osxphotos-theme-config"]
-        ],
-        "--config-only": [
-            [0, "cmdoption-osxphotos-export-config-only"]
-        ],
-        "--convert-to-jpeg": [
-            [0, "cmdoption-osxphotos-export-convert-to-jpeg"]
-        ],
-        "--current-name": [
-            [0, "cmdoption-osxphotos-export-current-name"]
-        ],
-        "--date": [
-            [0, "cmdoption-osxphotos-timewarp-d"]
-        ],
-        "--date-added": [
-            [0, "cmdoption-osxphotos-timewarp-date-added"]
-        ],
-        "--date-added-from-photo": [
-            [0, "cmdoption-osxphotos-timewarp-date-added-from-photo"]
-        ],
-        "--date-delta": [
-            [0, "cmdoption-osxphotos-timewarp-D"]
-        ],
-        "--db": [
-            [0, "cmdoption-osxphotos-albums-library"],
-            [0, "cmdoption-osxphotos-batch-edit-library"],
-            [0, "cmdoption-osxphotos-diff-library"],
-            [0, "cmdoption-osxphotos-dump-library"],
-            [0, "cmdoption-osxphotos-exiftool-library"],
-            [0, "cmdoption-osxphotos-export-library"],
-            [0, "cmdoption-osxphotos-info-library"],
-            [0, "cmdoption-osxphotos-inspect-library"],
-            [0, "cmdoption-osxphotos-keywords-library"],
-            [0, "cmdoption-osxphotos-labels-library"],
-            [0, "cmdoption-osxphotos-library"],
-            [0, "cmdoption-osxphotos-orphans-library"],
-            [0, "cmdoption-osxphotos-persons-library"],
-            [0, "cmdoption-osxphotos-places-library"],
-            [0, "cmdoption-osxphotos-query-library"],
-            [0, "cmdoption-osxphotos-repl-library"],
-            [0, "cmdoption-osxphotos-show-library"],
-            [0, "cmdoption-osxphotos-snap-library"],
-            [0, "cmdoption-osxphotos-sync-library"]
-        ],
-        "--db-config": [
-            [0, "cmdoption-osxphotos-exiftool-db-config"]
-        ],
-        "--default": [
-            [0, "cmdoption-osxphotos-theme-default"]
-        ],
-        "--delete": [
-            [0, "cmdoption-osxphotos-theme-delete"]
-        ],
-        "--delete-file": [
-            [0, "cmdoption-osxphotos-exportdb-delete-file"]
-        ],
-        "--delete-uuid": [
-            [0, "cmdoption-osxphotos-exportdb-delete-uuid"]
-        ],
-        "--deleted": [
-            [0, "cmdoption-osxphotos-dump-deleted"],
-            [0, "cmdoption-osxphotos-export-deleted"],
-            [0, "cmdoption-osxphotos-query-deleted"],
-            [0, "cmdoption-osxphotos-repl-deleted"]
-        ],
-        "--deleted-only": [
-            [0, "cmdoption-osxphotos-dump-deleted-only"],
-            [0, "cmdoption-osxphotos-export-deleted-only"],
-            [0, "cmdoption-osxphotos-query-deleted-only"],
-            [0, "cmdoption-osxphotos-repl-deleted-only"]
-        ],
-        "--description": [
-            [0, "cmdoption-osxphotos-add-locations-description"],
-            [0, "cmdoption-osxphotos-batch-edit-description"],
-            [0, "cmdoption-osxphotos-export-description"],
-            [0, "cmdoption-osxphotos-import-d"],
-            [0, "cmdoption-osxphotos-query-description"],
-            [0, "cmdoption-osxphotos-repl-description"],
-            [0, "cmdoption-osxphotos-sync-description"]
-        ],
-        "--description-template": [
-            [0, "cmdoption-osxphotos-exiftool-description-template"],
-            [0, "cmdoption-osxphotos-export-description-template"]
-        ],
-        "--detect-text": [
-            [0, "cmdoption-osxphotos-inspect-t"]
-        ],
-        "--directory": [
-            [0, "cmdoption-osxphotos-export-directory"]
-        ],
-        "--download-missing": [
-            [0, "cmdoption-osxphotos-export-download-missing"]
-        ],
-        "--dry-run": [
-            [0, "cmdoption-osxphotos-add-locations-dry-run"],
-            [0, "cmdoption-osxphotos-batch-edit-dry-run"],
-            [0, "cmdoption-osxphotos-exiftool-dry-run"],
-            [0, "cmdoption-osxphotos-export-dry-run"],
-            [0, "cmdoption-osxphotos-exportdb-dry-run"],
-            [0, "cmdoption-osxphotos-sync-dry-run"]
-        ],
-        "--dup-check": [
-            [0, "cmdoption-osxphotos-import-D"]
-        ],
-        "--duplicate": [
-            [0, "cmdoption-osxphotos-add-locations-duplicate"],
-            [0, "cmdoption-osxphotos-export-duplicate"],
-            [0, "cmdoption-osxphotos-query-duplicate"],
-            [0, "cmdoption-osxphotos-repl-duplicate"],
-            [0, "cmdoption-osxphotos-sync-duplicate"]
-        ],
-        "--edit": [
-            [0, "cmdoption-osxphotos-theme-edit"]
-        ],
-        "--edited": [
-            [0, "cmdoption-osxphotos-add-locations-edited"],
-            [0, "cmdoption-osxphotos-export-edited"],
-            [0, "cmdoption-osxphotos-query-edited"],
-            [0, "cmdoption-osxphotos-repl-edited"],
-            [0, "cmdoption-osxphotos-sync-edited"]
-        ],
-        "--edited-suffix": [
-            [0, "cmdoption-osxphotos-export-edited-suffix"]
-        ],
-        "--emacs": [
-            [0, "cmdoption-osxphotos-repl-emacs"]
-        ],
-        "--errors": [
-            [0, "cmdoption-osxphotos-exportdb-errors"]
-        ],
-        "--exif": [
-            [0, "cmdoption-osxphotos-add-locations-exif"],
-            [0, "cmdoption-osxphotos-export-exif"],
-            [0, "cmdoption-osxphotos-query-exif"],
-            [0, "cmdoption-osxphotos-repl-exif"],
-            [0, "cmdoption-osxphotos-sync-exif"]
-        ],
-        "--exiftool": [
-            [0, "cmdoption-osxphotos-export-exiftool"],
-            [0, "cmdoption-osxphotos-import-e"]
-        ],
-        "--exiftool-merge-keywords": [
-            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-keywords"],
-            [0, "cmdoption-osxphotos-export-exiftool-merge-keywords"]
-        ],
-        "--exiftool-merge-persons": [
-            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-persons"],
-            [0, "cmdoption-osxphotos-export-exiftool-merge-persons"]
-        ],
-        "--exiftool-option": [
-            [0, "cmdoption-osxphotos-exiftool-exiftool-option"],
-            [0, "cmdoption-osxphotos-export-exiftool-option"]
-        ],
-        "--exiftool-path": [
-            [0, "cmdoption-osxphotos-exiftool-exiftool-path"],
-            [0, "cmdoption-osxphotos-export-exiftool-path"],
-            [0, "cmdoption-osxphotos-import-0"],
-            [0, "cmdoption-osxphotos-timewarp-e"]
-        ],
-        "--export": [
-            [0, "cmdoption-osxphotos-orphans-export"],
-            [0, "cmdoption-osxphotos-sync-e"]
-        ],
-        "--export-as-hardlink": [
-            [0, "cmdoption-osxphotos-export-export-as-hardlink"]
-        ],
-        "--export-by-date": [
-            [0, "cmdoption-osxphotos-export-export-by-date"]
-        ],
-        "--export-dir": [
-            [0, "cmdoption-osxphotos-exportdb-export-dir"]
-        ],
-        "--exportdb": [
-            [0, "cmdoption-osxphotos-exiftool-exportdb"],
-            [0, "cmdoption-osxphotos-export-exportdb"]
-        ],
-        "--external-edit": [
-            [0, "cmdoption-osxphotos-add-locations-external-edit"],
-            [0, "cmdoption-osxphotos-export-external-edit"],
-            [0, "cmdoption-osxphotos-query-external-edit"],
-            [0, "cmdoption-osxphotos-repl-external-edit"],
-            [0, "cmdoption-osxphotos-sync-external-edit"]
-        ],
-        "--favorite": [
-            [0, "cmdoption-osxphotos-add-locations-favorite"],
-            [0, "cmdoption-osxphotos-export-favorite"],
-            [0, "cmdoption-osxphotos-query-favorite"],
-            [0, "cmdoption-osxphotos-repl-favorite"],
-            [0, "cmdoption-osxphotos-sync-favorite"]
-        ],
-        "--favorite-rating": [
-            [0, "cmdoption-osxphotos-export-favorite-rating"]
-        ],
-        "--field": [
-            [0, "cmdoption-osxphotos-dump-f"],
-            [0, "cmdoption-osxphotos-query-f"]
-        ],
-        "--filename": [
-            [0, "cmdoption-osxphotos-export-filename"],
-            [0, "cmdoption-osxphotos-uuid-f"]
-        ],
-        "--finder-tag-keywords": [
-            [0, "cmdoption-osxphotos-export-finder-tag-keywords"]
-        ],
-        "--finder-tag-template": [
-            [0, "cmdoption-osxphotos-export-finder-tag-template"]
-        ],
-        "--folder": [
-            [0, "cmdoption-osxphotos-add-locations-folder"],
-            [0, "cmdoption-osxphotos-export-folder"],
-            [0, "cmdoption-osxphotos-query-folder"],
-            [0, "cmdoption-osxphotos-repl-folder"],
-            [0, "cmdoption-osxphotos-sync-folder"]
-        ],
-        "--force": [
-            [0, "cmdoption-osxphotos-timewarp-force"]
-        ],
-        "--force-update": [
-            [0, "cmdoption-osxphotos-export-force-update"]
-        ],
-        "--from-date": [
-            [0, "cmdoption-osxphotos-add-locations-from-date"],
-            [0, "cmdoption-osxphotos-export-from-date"],
-            [0, "cmdoption-osxphotos-query-from-date"],
-            [0, "cmdoption-osxphotos-repl-from-date"],
-            [0, "cmdoption-osxphotos-sync-from-date"]
-        ],
-        "--from-time": [
-            [0, "cmdoption-osxphotos-add-locations-from-time"],
-            [0, "cmdoption-osxphotos-export-from-time"],
-            [0, "cmdoption-osxphotos-query-from-time"],
-            [0, "cmdoption-osxphotos-repl-from-time"],
-            [0, "cmdoption-osxphotos-sync-from-time"]
-        ],
-        "--function": [
-            [0, "cmdoption-osxphotos-timewarp-F"]
-        ],
-        "--glob": [
-            [0, "cmdoption-osxphotos-import-g"]
-        ],
-        "--has-comment": [
-            [0, "cmdoption-osxphotos-add-locations-has-comment"],
-            [0, "cmdoption-osxphotos-export-has-comment"],
-            [0, "cmdoption-osxphotos-query-has-comment"],
-            [0, "cmdoption-osxphotos-repl-has-comment"],
-            [0, "cmdoption-osxphotos-sync-has-comment"]
-        ],
-        "--has-likes": [
-            [0, "cmdoption-osxphotos-add-locations-has-likes"],
-            [0, "cmdoption-osxphotos-export-has-likes"],
-            [0, "cmdoption-osxphotos-query-has-likes"],
-            [0, "cmdoption-osxphotos-repl-has-likes"],
-            [0, "cmdoption-osxphotos-sync-has-likes"]
-        ],
-        "--has-raw": [
-            [0, "cmdoption-osxphotos-add-locations-has-raw"],
-            [0, "cmdoption-osxphotos-export-has-raw"],
-            [0, "cmdoption-osxphotos-query-has-raw"],
-            [0, "cmdoption-osxphotos-repl-has-raw"],
-            [0, "cmdoption-osxphotos-sync-has-raw"]
-        ],
-        "--hdr": [
-            [0, "cmdoption-osxphotos-add-locations-hdr"],
-            [0, "cmdoption-osxphotos-export-hdr"],
-            [0, "cmdoption-osxphotos-query-hdr"],
-            [0, "cmdoption-osxphotos-repl-hdr"],
-            [0, "cmdoption-osxphotos-sync-hdr"]
-        ],
-        "--help": [
-            [0, "cmdoption-osxphotos-run-h"]
-        ],
-        "--hidden": [
-            [0, "cmdoption-osxphotos-add-locations-hidden"],
-            [0, "cmdoption-osxphotos-export-hidden"],
-            [0, "cmdoption-osxphotos-query-hidden"],
-            [0, "cmdoption-osxphotos-repl-hidden"],
-            [0, "cmdoption-osxphotos-sync-hidden"]
-        ],
-        "--ignore-case": [
-            [0, "cmdoption-osxphotos-add-locations-i"],
-            [0, "cmdoption-osxphotos-export-i"],
-            [0, "cmdoption-osxphotos-query-i"],
-            [0, "cmdoption-osxphotos-repl-i"],
-            [0, "cmdoption-osxphotos-sync-0"]
-        ],
-        "--ignore-date-modified": [
-            [0, "cmdoption-osxphotos-exiftool-ignore-date-modified"],
-            [0, "cmdoption-osxphotos-export-ignore-date-modified"]
-        ],
-        "--ignore-signature": [
-            [0, "cmdoption-osxphotos-export-ignore-signature"]
-        ],
-        "--import": [
-            [0, "cmdoption-osxphotos-sync-i"]
-        ],
-        "--in-album": [
-            [0, "cmdoption-osxphotos-add-locations-in-album"],
-            [0, "cmdoption-osxphotos-export-in-album"],
-            [0, "cmdoption-osxphotos-query-in-album"],
-            [0, "cmdoption-osxphotos-repl-in-album"],
-            [0, "cmdoption-osxphotos-sync-in-album"]
-        ],
-        "--incloud": [
-            [0, "cmdoption-osxphotos-add-locations-incloud"],
-            [0, "cmdoption-osxphotos-export-incloud"],
-            [0, "cmdoption-osxphotos-query-incloud"],
-            [0, "cmdoption-osxphotos-repl-incloud"],
-            [0, "cmdoption-osxphotos-sync-incloud"]
-        ],
-        "--info": [
-            [0, "cmdoption-osxphotos-exportdb-info"]
-        ],
-        "--inspect": [
-            [0, "cmdoption-osxphotos-timewarp-i"]
-        ],
-        "--is-reference": [
-            [0, "cmdoption-osxphotos-add-locations-is-reference"],
-            [0, "cmdoption-osxphotos-export-is-reference"],
-            [0, "cmdoption-osxphotos-query-is-reference"],
-            [0, "cmdoption-osxphotos-repl-is-reference"],
-            [0, "cmdoption-osxphotos-sync-is-reference"]
-        ],
-        "--jpeg-ext": [
-            [0, "cmdoption-osxphotos-export-jpeg-ext"]
-        ],
-        "--jpeg-quality": [
-            [0, "cmdoption-osxphotos-export-jpeg-quality"]
-        ],
-        "--json": [
-            [0, "cmdoption-osxphotos-albums-json"],
-            [0, "cmdoption-osxphotos-dump-json"],
-            [0, "cmdoption-osxphotos-info-json"],
-            [0, "cmdoption-osxphotos-json"],
-            [0, "cmdoption-osxphotos-keywords-json"],
-            [0, "cmdoption-osxphotos-labels-json"],
-            [0, "cmdoption-osxphotos-list-json"],
-            [0, "cmdoption-osxphotos-persons-json"],
-            [0, "cmdoption-osxphotos-places-json"],
-            [0, "cmdoption-osxphotos-query-json"]
-        ],
-        "--keep": [
-            [0, "cmdoption-osxphotos-export-keep"]
-        ],
-        "--keyword": [
-            [0, "cmdoption-osxphotos-add-locations-keyword"],
-            [0, "cmdoption-osxphotos-batch-edit-keyword"],
-            [0, "cmdoption-osxphotos-export-keyword"],
-            [0, "cmdoption-osxphotos-import-k"],
-            [0, "cmdoption-osxphotos-query-keyword"],
-            [0, "cmdoption-osxphotos-repl-keyword"],
-            [0, "cmdoption-osxphotos-sync-keyword"]
-        ],
-        "--keyword-template": [
-            [0, "cmdoption-osxphotos-exiftool-keyword-template"],
-            [0, "cmdoption-osxphotos-export-keyword-template"]
-        ],
-        "--label": [
-            [0, "cmdoption-osxphotos-add-locations-label"],
-            [0, "cmdoption-osxphotos-export-label"],
-            [0, "cmdoption-osxphotos-query-label"],
-            [0, "cmdoption-osxphotos-repl-label"],
-            [0, "cmdoption-osxphotos-sync-label"]
-        ],
-        "--last-errors": [
-            [0, "cmdoption-osxphotos-exportdb-last-errors"]
-        ],
-        "--last-run": [
-            [0, "cmdoption-osxphotos-exportdb-last-run"]
-        ],
-        "--library": [
-            [0, "cmdoption-osxphotos-albums-library"],
-            [0, "cmdoption-osxphotos-batch-edit-library"],
-            [0, "cmdoption-osxphotos-diff-library"],
-            [0, "cmdoption-osxphotos-dump-library"],
-            [0, "cmdoption-osxphotos-exiftool-library"],
-            [0, "cmdoption-osxphotos-export-library"],
-            [0, "cmdoption-osxphotos-info-library"],
-            [0, "cmdoption-osxphotos-inspect-library"],
-            [0, "cmdoption-osxphotos-keywords-library"],
-            [0, "cmdoption-osxphotos-labels-library"],
-            [0, "cmdoption-osxphotos-library"],
-            [0, "cmdoption-osxphotos-orphans-library"],
-            [0, "cmdoption-osxphotos-persons-library"],
-            [0, "cmdoption-osxphotos-places-library"],
-            [0, "cmdoption-osxphotos-query-library"],
-            [0, "cmdoption-osxphotos-repl-library"],
-            [0, "cmdoption-osxphotos-show-library"],
-            [0, "cmdoption-osxphotos-snap-library"],
-            [0, "cmdoption-osxphotos-sync-library"],
-            [0, "cmdoption-osxphotos-timewarp-L"]
-        ],
-        "--limit": [
-            [0, "cmdoption-osxphotos-export-limit"]
-        ],
-        "--list": [
-            [0, "cmdoption-osxphotos-theme-list"]
-        ],
-        "--live": [
-            [0, "cmdoption-osxphotos-add-locations-live"],
-            [0, "cmdoption-osxphotos-export-live"],
-            [0, "cmdoption-osxphotos-query-live"],
-            [0, "cmdoption-osxphotos-repl-live"],
-            [0, "cmdoption-osxphotos-sync-live"]
-        ],
-        "--load-config": [
-            [0, "cmdoption-osxphotos-exiftool-load-config"],
-            [0, "cmdoption-osxphotos-export-load-config"]
-        ],
-        "--location": [
-            [0, "cmdoption-osxphotos-add-locations-location"],
-            [0, "cmdoption-osxphotos-batch-edit-location"],
-            [0, "cmdoption-osxphotos-export-location"],
-            [0, "cmdoption-osxphotos-import-l"],
-            [0, "cmdoption-osxphotos-query-location"],
-            [0, "cmdoption-osxphotos-repl-location"],
-            [0, "cmdoption-osxphotos-sync-location"]
-        ],
-        "--match-time": [
-            [0, "cmdoption-osxphotos-timewarp-0"]
-        ],
-        "--max-size": [
-            [0, "cmdoption-osxphotos-add-locations-max-size"],
-            [0, "cmdoption-osxphotos-export-max-size"],
-            [0, "cmdoption-osxphotos-query-max-size"],
-            [0, "cmdoption-osxphotos-repl-max-size"],
-            [0, "cmdoption-osxphotos-sync-max-size"]
-        ],
-        "--merge": [
-            [0, "cmdoption-osxphotos-sync-m"]
-        ],
-        "--merge-keywords": [
-            [0, "cmdoption-osxphotos-import-m"]
-        ],
-        "--migrate": [
-            [0, "cmdoption-osxphotos-exportdb-migrate"]
-        ],
-        "--migrate-photos-library": [
-            [0, "cmdoption-osxphotos-exportdb-migrate-photos-library"]
-        ],
-        "--min-size": [
-            [0, "cmdoption-osxphotos-add-locations-min-size"],
-            [0, "cmdoption-osxphotos-export-min-size"],
-            [0, "cmdoption-osxphotos-query-min-size"],
-            [0, "cmdoption-osxphotos-repl-min-size"],
-            [0, "cmdoption-osxphotos-sync-min-size"]
-        ],
-        "--missing": [
-            [0, "cmdoption-osxphotos-add-locations-missing"],
-            [0, "cmdoption-osxphotos-export-missing"],
-            [0, "cmdoption-osxphotos-query-missing"],
-            [0, "cmdoption-osxphotos-repl-missing"],
-            [0, "cmdoption-osxphotos-sync-missing"]
-        ],
-        "--name": [
-            [0, "cmdoption-osxphotos-add-locations-name"],
-            [0, "cmdoption-osxphotos-export-name"],
-            [0, "cmdoption-osxphotos-query-name"],
-            [0, "cmdoption-osxphotos-repl-name"],
-            [0, "cmdoption-osxphotos-sync-name"]
-        ],
-        "--no-comment": [
-            [0, "cmdoption-osxphotos-add-locations-no-comment"],
-            [0, "cmdoption-osxphotos-export-no-comment"],
-            [0, "cmdoption-osxphotos-query-no-comment"],
-            [0, "cmdoption-osxphotos-repl-no-comment"],
-            [0, "cmdoption-osxphotos-sync-no-comment"]
-        ],
-        "--no-description": [
-            [0, "cmdoption-osxphotos-add-locations-no-description"],
-            [0, "cmdoption-osxphotos-export-no-description"],
-            [0, "cmdoption-osxphotos-query-no-description"],
-            [0, "cmdoption-osxphotos-repl-no-description"],
-            [0, "cmdoption-osxphotos-sync-no-description"]
-        ],
-        "--no-keyword": [
-            [0, "cmdoption-osxphotos-add-locations-no-keyword"],
-            [0, "cmdoption-osxphotos-export-no-keyword"],
-            [0, "cmdoption-osxphotos-query-no-keyword"],
-            [0, "cmdoption-osxphotos-repl-no-keyword"],
-            [0, "cmdoption-osxphotos-sync-no-keyword"]
-        ],
-        "--no-likes": [
-            [0, "cmdoption-osxphotos-add-locations-no-likes"],
-            [0, "cmdoption-osxphotos-export-no-likes"],
-            [0, "cmdoption-osxphotos-query-no-likes"],
-            [0, "cmdoption-osxphotos-repl-no-likes"],
-            [0, "cmdoption-osxphotos-sync-no-likes"]
-        ],
-        "--no-location": [
-            [0, "cmdoption-osxphotos-add-locations-no-location"],
-            [0, "cmdoption-osxphotos-export-no-location"],
-            [0, "cmdoption-osxphotos-query-no-location"],
-            [0, "cmdoption-osxphotos-repl-no-location"],
-            [0, "cmdoption-osxphotos-sync-no-location"]
-        ],
-        "--no-place": [
-            [0, "cmdoption-osxphotos-add-locations-no-place"],
-            [0, "cmdoption-osxphotos-export-no-place"],
-            [0, "cmdoption-osxphotos-query-no-place"],
-            [0, "cmdoption-osxphotos-repl-no-place"],
-            [0, "cmdoption-osxphotos-sync-no-place"]
-        ],
-        "--no-progress": [
-            [0, "cmdoption-osxphotos-export-no-progress"],
-            [0, "cmdoption-osxphotos-import-no-progress"]
-        ],
-        "--no-title": [
-            [0, "cmdoption-osxphotos-add-locations-no-title"],
-            [0, "cmdoption-osxphotos-export-no-title"],
-            [0, "cmdoption-osxphotos-query-no-title"],
-            [0, "cmdoption-osxphotos-repl-no-title"],
-            [0, "cmdoption-osxphotos-sync-no-title"]
-        ],
-        "--not-burst": [
-            [0, "cmdoption-osxphotos-add-locations-not-burst"],
-            [0, "cmdoption-osxphotos-export-not-burst"],
-            [0, "cmdoption-osxphotos-query-not-burst"],
-            [0, "cmdoption-osxphotos-repl-not-burst"],
-            [0, "cmdoption-osxphotos-sync-not-burst"]
-        ],
-        "--not-cloudasset": [
-            [0, "cmdoption-osxphotos-add-locations-not-cloudasset"],
-            [0, "cmdoption-osxphotos-export-not-cloudasset"],
-            [0, "cmdoption-osxphotos-query-not-cloudasset"],
-            [0, "cmdoption-osxphotos-repl-not-cloudasset"],
-            [0, "cmdoption-osxphotos-sync-not-cloudasset"]
-        ],
-        "--not-edited": [
-            [0, "cmdoption-osxphotos-add-locations-not-edited"],
-            [0, "cmdoption-osxphotos-export-not-edited"],
-            [0, "cmdoption-osxphotos-query-not-edited"],
-            [0, "cmdoption-osxphotos-repl-not-edited"],
-            [0, "cmdoption-osxphotos-sync-not-edited"]
-        ],
-        "--not-favorite": [
-            [0, "cmdoption-osxphotos-add-locations-not-favorite"],
-            [0, "cmdoption-osxphotos-export-not-favorite"],
-            [0, "cmdoption-osxphotos-query-not-favorite"],
-            [0, "cmdoption-osxphotos-repl-not-favorite"],
-            [0, "cmdoption-osxphotos-sync-not-favorite"]
-        ],
-        "--not-hdr": [
-            [0, "cmdoption-osxphotos-add-locations-not-hdr"],
-            [0, "cmdoption-osxphotos-export-not-hdr"],
-            [0, "cmdoption-osxphotos-query-not-hdr"],
-            [0, "cmdoption-osxphotos-repl-not-hdr"],
-            [0, "cmdoption-osxphotos-sync-not-hdr"]
-        ],
-        "--not-hidden": [
-            [0, "cmdoption-osxphotos-add-locations-not-hidden"],
-            [0, "cmdoption-osxphotos-export-not-hidden"],
-            [0, "cmdoption-osxphotos-query-not-hidden"],
-            [0, "cmdoption-osxphotos-repl-not-hidden"],
-            [0, "cmdoption-osxphotos-sync-not-hidden"]
-        ],
-        "--not-in-album": [
-            [0, "cmdoption-osxphotos-add-locations-not-in-album"],
-            [0, "cmdoption-osxphotos-export-not-in-album"],
-            [0, "cmdoption-osxphotos-query-not-in-album"],
-            [0, "cmdoption-osxphotos-repl-not-in-album"],
-            [0, "cmdoption-osxphotos-sync-not-in-album"]
-        ],
-        "--not-incloud": [
-            [0, "cmdoption-osxphotos-add-locations-not-incloud"],
-            [0, "cmdoption-osxphotos-export-not-incloud"],
-            [0, "cmdoption-osxphotos-query-not-incloud"],
-            [0, "cmdoption-osxphotos-repl-not-incloud"],
-            [0, "cmdoption-osxphotos-sync-not-incloud"]
-        ],
-        "--not-live": [
-            [0, "cmdoption-osxphotos-add-locations-not-live"],
-            [0, "cmdoption-osxphotos-export-not-live"],
-            [0, "cmdoption-osxphotos-query-not-live"],
-            [0, "cmdoption-osxphotos-repl-not-live"],
-            [0, "cmdoption-osxphotos-sync-not-live"]
-        ],
-        "--not-missing": [
-            [0, "cmdoption-osxphotos-add-locations-not-missing"],
-            [0, "cmdoption-osxphotos-export-not-missing"],
-            [0, "cmdoption-osxphotos-query-not-missing"],
-            [0, "cmdoption-osxphotos-repl-not-missing"],
-            [0, "cmdoption-osxphotos-sync-not-missing"]
-        ],
-        "--not-panorama": [
-            [0, "cmdoption-osxphotos-add-locations-not-panorama"],
-            [0, "cmdoption-osxphotos-export-not-panorama"],
-            [0, "cmdoption-osxphotos-query-not-panorama"],
-            [0, "cmdoption-osxphotos-repl-not-panorama"],
-            [0, "cmdoption-osxphotos-sync-not-panorama"]
-        ],
-        "--not-portrait": [
-            [0, "cmdoption-osxphotos-add-locations-not-portrait"],
-            [0, "cmdoption-osxphotos-export-not-portrait"],
-            [0, "cmdoption-osxphotos-query-not-portrait"],
-            [0, "cmdoption-osxphotos-repl-not-portrait"],
-            [0, "cmdoption-osxphotos-sync-not-portrait"]
-        ],
-        "--not-reference": [
-            [0, "cmdoption-osxphotos-add-locations-not-reference"],
-            [0, "cmdoption-osxphotos-export-not-reference"],
-            [0, "cmdoption-osxphotos-query-not-reference"],
-            [0, "cmdoption-osxphotos-repl-not-reference"],
-            [0, "cmdoption-osxphotos-sync-not-reference"]
-        ],
-        "--not-saved-to-library": [
-            [0, "cmdoption-osxphotos-add-locations-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-export-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-query-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-repl-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-sync-not-saved-to-library"]
-        ],
-        "--not-screenshot": [
-            [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
-            [0, "cmdoption-osxphotos-export-not-screenshot"],
-            [0, "cmdoption-osxphotos-query-not-screenshot"],
-            [0, "cmdoption-osxphotos-repl-not-screenshot"],
-            [0, "cmdoption-osxphotos-sync-not-screenshot"]
-        ],
-        "--not-selfie": [
-            [0, "cmdoption-osxphotos-add-locations-not-selfie"],
-            [0, "cmdoption-osxphotos-export-not-selfie"],
-            [0, "cmdoption-osxphotos-query-not-selfie"],
-            [0, "cmdoption-osxphotos-repl-not-selfie"],
-            [0, "cmdoption-osxphotos-sync-not-selfie"]
-        ],
-        "--not-shared": [
-            [0, "cmdoption-osxphotos-add-locations-not-shared"],
-            [0, "cmdoption-osxphotos-export-not-shared"],
-            [0, "cmdoption-osxphotos-query-not-shared"],
-            [0, "cmdoption-osxphotos-repl-not-shared"]
-        ],
-        "--not-slow-mo": [
-            [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
-            [0, "cmdoption-osxphotos-export-not-slow-mo"],
-            [0, "cmdoption-osxphotos-query-not-slow-mo"],
-            [0, "cmdoption-osxphotos-repl-not-slow-mo"],
-            [0, "cmdoption-osxphotos-sync-not-slow-mo"]
-        ],
-        "--not-syndicated": [
-            [0, "cmdoption-osxphotos-add-locations-not-syndicated"],
-            [0, "cmdoption-osxphotos-export-not-syndicated"],
-            [0, "cmdoption-osxphotos-query-not-syndicated"],
-            [0, "cmdoption-osxphotos-repl-not-syndicated"],
-            [0, "cmdoption-osxphotos-sync-not-syndicated"]
-        ],
-        "--not-time-lapse": [
-            [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
-            [0, "cmdoption-osxphotos-export-not-time-lapse"],
-            [0, "cmdoption-osxphotos-query-not-time-lapse"],
-            [0, "cmdoption-osxphotos-repl-not-time-lapse"],
-            [0, "cmdoption-osxphotos-sync-not-time-lapse"]
-        ],
-        "--only-movies": [
-            [0, "cmdoption-osxphotos-add-locations-only-movies"],
-            [0, "cmdoption-osxphotos-export-only-movies"],
-            [0, "cmdoption-osxphotos-query-only-movies"],
-            [0, "cmdoption-osxphotos-repl-only-movies"],
-            [0, "cmdoption-osxphotos-sync-only-movies"]
-        ],
-        "--only-new": [
-            [0, "cmdoption-osxphotos-export-only-new"]
-        ],
-        "--only-photos": [
-            [0, "cmdoption-osxphotos-add-locations-only-photos"],
-            [0, "cmdoption-osxphotos-export-only-photos"],
-            [0, "cmdoption-osxphotos-query-only-photos"],
-            [0, "cmdoption-osxphotos-repl-only-photos"],
-            [0, "cmdoption-osxphotos-sync-only-photos"]
-        ],
-        "--original-suffix": [
-            [0, "cmdoption-osxphotos-export-original-suffix"]
-        ],
-        "--overwrite": [
-            [0, "cmdoption-osxphotos-export-overwrite"]
-        ],
-        "--panorama": [
-            [0, "cmdoption-osxphotos-add-locations-panorama"],
-            [0, "cmdoption-osxphotos-export-panorama"],
-            [0, "cmdoption-osxphotos-query-panorama"],
-            [0, "cmdoption-osxphotos-repl-panorama"],
-            [0, "cmdoption-osxphotos-sync-panorama"]
-        ],
-        "--parse-date": [
-            [0, "cmdoption-osxphotos-import-P"],
-            [0, "cmdoption-osxphotos-timewarp-M"]
-        ],
-        "--person": [
-            [0, "cmdoption-osxphotos-add-locations-person"],
-            [0, "cmdoption-osxphotos-export-person"],
-            [0, "cmdoption-osxphotos-query-person"],
-            [0, "cmdoption-osxphotos-repl-person"],
-            [0, "cmdoption-osxphotos-sync-person"]
-        ],
-        "--person-keyword": [
-            [0, "cmdoption-osxphotos-exiftool-person-keyword"],
-            [0, "cmdoption-osxphotos-export-person-keyword"]
-        ],
-        "--place": [
-            [0, "cmdoption-osxphotos-add-locations-place"],
-            [0, "cmdoption-osxphotos-export-place"],
-            [0, "cmdoption-osxphotos-query-place"],
-            [0, "cmdoption-osxphotos-repl-place"],
-            [0, "cmdoption-osxphotos-sync-place"]
-        ],
-        "--plain": [
-            [0, "cmdoption-osxphotos-timewarp-plain"]
-        ],
-        "--portrait": [
-            [0, "cmdoption-osxphotos-add-locations-portrait"],
-            [0, "cmdoption-osxphotos-export-portrait"],
-            [0, "cmdoption-osxphotos-query-portrait"],
-            [0, "cmdoption-osxphotos-repl-portrait"],
-            [0, "cmdoption-osxphotos-sync-portrait"]
-        ],
-        "--post-command": [
-            [0, "cmdoption-osxphotos-export-post-command"]
-        ],
-        "--post-function": [
-            [0, "cmdoption-osxphotos-export-post-function"],
-            [0, "cmdoption-osxphotos-import-post-function"]
-        ],
-        "--preview": [
-            [0, "cmdoption-osxphotos-export-preview"],
-            [0, "cmdoption-osxphotos-theme-preview"]
-        ],
-        "--preview-if-missing": [
-            [0, "cmdoption-osxphotos-export-preview-if-missing"]
-        ],
-        "--preview-suffix": [
-            [0, "cmdoption-osxphotos-export-preview-suffix"]
-        ],
-        "--print": [
-            [0, "cmdoption-osxphotos-dump-print"],
-            [0, "cmdoption-osxphotos-export-print"],
-            [0, "cmdoption-osxphotos-query-print"]
-        ],
-        "--pull-exif": [
-            [0, "cmdoption-osxphotos-timewarp-P"]
-        ],
-        "--push-exif": [
-            [0, "cmdoption-osxphotos-timewarp-p"]
-        ],
-        "--query-eval": [
-            [0, "cmdoption-osxphotos-add-locations-query-eval"],
-            [0, "cmdoption-osxphotos-export-query-eval"],
-            [0, "cmdoption-osxphotos-query-query-eval"],
-            [0, "cmdoption-osxphotos-repl-query-eval"],
-            [0, "cmdoption-osxphotos-sync-query-eval"]
-        ],
-        "--query-function": [
-            [0, "cmdoption-osxphotos-add-locations-query-function"],
-            [0, "cmdoption-osxphotos-export-query-function"],
-            [0, "cmdoption-osxphotos-query-query-function"],
-            [0, "cmdoption-osxphotos-repl-query-function"],
-            [0, "cmdoption-osxphotos-sync-query-function"]
-        ],
-        "--quiet": [
-            [0, "cmdoption-osxphotos-query-quiet"]
-        ],
-        "--ramdb": [
-            [0, "cmdoption-osxphotos-export-ramdb"]
-        ],
-        "--raw-output": [
-            [0, "cmdoption-osxphotos-diff-r"]
-        ],
-        "--regex": [
-            [0, "cmdoption-osxphotos-add-locations-regex"],
-            [0, "cmdoption-osxphotos-export-regex"],
-            [0, "cmdoption-osxphotos-query-regex"],
-            [0, "cmdoption-osxphotos-repl-regex"],
-            [0, "cmdoption-osxphotos-sync-regex"]
-        ],
-        "--relative-to": [
-            [0, "cmdoption-osxphotos-import-r"]
-        ],
-        "--replace-keywords": [
-            [0, "cmdoption-osxphotos-batch-edit-replace-keywords"],
-            [0, "cmdoption-osxphotos-exiftool-replace-keywords"],
-            [0, "cmdoption-osxphotos-export-replace-keywords"]
-        ],
-        "--report": [
-            [0, "cmdoption-osxphotos-exiftool-report"],
-            [0, "cmdoption-osxphotos-export-report"],
-            [0, "cmdoption-osxphotos-exportdb-report"],
-            [0, "cmdoption-osxphotos-import-report"],
-            [0, "cmdoption-osxphotos-sync-R"]
-        ],
-        "--resume": [
-            [0, "cmdoption-osxphotos-import-R"]
-        ],
-        "--retry": [
-            [0, "cmdoption-osxphotos-export-retry"]
-        ],
-        "--run": [
-            [0, "cmdoption-osxphotos-version-run"]
-        ],
-        "--save-config": [
-            [0, "cmdoption-osxphotos-exiftool-save-config"],
-            [0, "cmdoption-osxphotos-export-save-config"],
-            [0, "cmdoption-osxphotos-exportdb-save-config"]
-        ],
-        "--saved-to-library": [
-            [0, "cmdoption-osxphotos-add-locations-saved-to-library"],
-            [0, "cmdoption-osxphotos-export-saved-to-library"],
-            [0, "cmdoption-osxphotos-query-saved-to-library"],
-            [0, "cmdoption-osxphotos-repl-saved-to-library"],
-            [0, "cmdoption-osxphotos-sync-saved-to-library"]
-        ],
-        "--screenshot": [
-            [0, "cmdoption-osxphotos-add-locations-screenshot"],
-            [0, "cmdoption-osxphotos-export-screenshot"],
-            [0, "cmdoption-osxphotos-query-screenshot"],
-            [0, "cmdoption-osxphotos-repl-screenshot"],
-            [0, "cmdoption-osxphotos-sync-screenshot"]
-        ],
-        "--selected": [
-            [0, "cmdoption-osxphotos-add-locations-selected"],
-            [0, "cmdoption-osxphotos-export-selected"],
-            [0, "cmdoption-osxphotos-query-selected"],
-            [0, "cmdoption-osxphotos-repl-selected"],
-            [0, "cmdoption-osxphotos-sync-selected"]
-        ],
-        "--selfie": [
-            [0, "cmdoption-osxphotos-add-locations-selfie"],
-            [0, "cmdoption-osxphotos-export-selfie"],
-            [0, "cmdoption-osxphotos-query-selfie"],
-            [0, "cmdoption-osxphotos-repl-selfie"],
-            [0, "cmdoption-osxphotos-sync-selfie"]
-        ],
-        "--set": [
-            [0, "cmdoption-osxphotos-sync-s"]
-        ],
-        "--shared": [
-            [0, "cmdoption-osxphotos-add-locations-shared"],
-            [0, "cmdoption-osxphotos-export-shared"],
-            [0, "cmdoption-osxphotos-query-shared"],
-            [0, "cmdoption-osxphotos-repl-shared"]
-        ],
-        "--sidecar": [
-            [0, "cmdoption-osxphotos-export-sidecar"]
-        ],
-        "--sidecar-drop-ext": [
-            [0, "cmdoption-osxphotos-export-sidecar-drop-ext"]
-        ],
-        "--skip-bursts": [
-            [0, "cmdoption-osxphotos-export-skip-bursts"]
-        ],
-        "--skip-edited": [
-            [0, "cmdoption-osxphotos-export-skip-edited"]
-        ],
-        "--skip-live": [
-            [0, "cmdoption-osxphotos-export-skip-live"]
-        ],
-        "--skip-original-if-edited": [
-            [0, "cmdoption-osxphotos-export-skip-original-if-edited"]
-        ],
-        "--skip-raw": [
-            [0, "cmdoption-osxphotos-export-skip-raw"]
-        ],
-        "--skip-uuid": [
-            [0, "cmdoption-osxphotos-export-skip-uuid"]
-        ],
-        "--skip-uuid-from-file": [
-            [0, "cmdoption-osxphotos-export-skip-uuid-from-file"]
-        ],
-        "--slow-mo": [
-            [0, "cmdoption-osxphotos-add-locations-slow-mo"],
-            [0, "cmdoption-osxphotos-export-slow-mo"],
-            [0, "cmdoption-osxphotos-query-slow-mo"],
-            [0, "cmdoption-osxphotos-repl-slow-mo"],
-            [0, "cmdoption-osxphotos-sync-slow-mo"]
-        ],
-        "--split-folder": [
-            [0, "cmdoption-osxphotos-import-f"]
-        ],
-        "--sql": [
-            [0, "cmdoption-osxphotos-exportdb-sql"]
-        ],
-        "--strip": [
-            [0, "cmdoption-osxphotos-export-strip"]
-        ],
-        "--style": [
-            [0, "cmdoption-osxphotos-diff-s"]
-        ],
-        "--syndicated": [
-            [0, "cmdoption-osxphotos-add-locations-syndicated"],
-            [0, "cmdoption-osxphotos-export-syndicated"],
-            [0, "cmdoption-osxphotos-query-syndicated"],
-            [0, "cmdoption-osxphotos-repl-syndicated"],
-            [0, "cmdoption-osxphotos-sync-syndicated"]
-        ],
-        "--template": [
-            [0, "cmdoption-osxphotos-inspect-T"]
-        ],
-        "--theme": [
-            [0, "cmdoption-osxphotos-add-locations-theme"],
-            [0, "cmdoption-osxphotos-batch-edit-theme"],
-            [0, "cmdoption-osxphotos-exiftool-theme"],
-            [0, "cmdoption-osxphotos-export-theme"],
-            [0, "cmdoption-osxphotos-exportdb-theme"],
-            [0, "cmdoption-osxphotos-import-theme"],
-            [0, "cmdoption-osxphotos-inspect-theme"],
-            [0, "cmdoption-osxphotos-orphans-theme"],
-            [0, "cmdoption-osxphotos-sync-theme"],
-            [0, "cmdoption-osxphotos-timewarp-theme"]
-        ],
-        "--time": [
-            [0, "cmdoption-osxphotos-timewarp-t"]
-        ],
-        "--time-delta": [
-            [0, "cmdoption-osxphotos-timewarp-T"]
-        ],
-        "--time-lapse": [
-            [0, "cmdoption-osxphotos-add-locations-time-lapse"],
-            [0, "cmdoption-osxphotos-export-time-lapse"],
-            [0, "cmdoption-osxphotos-query-time-lapse"],
-            [0, "cmdoption-osxphotos-repl-time-lapse"],
-            [0, "cmdoption-osxphotos-sync-time-lapse"]
-        ],
-        "--timestamp": [
-            [0, "cmdoption-osxphotos-add-locations-timestamp"],
-            [0, "cmdoption-osxphotos-batch-edit-timestamp"],
-            [0, "cmdoption-osxphotos-diff-timestamp"],
-            [0, "cmdoption-osxphotos-exiftool-timestamp"],
-            [0, "cmdoption-osxphotos-export-timestamp"],
-            [0, "cmdoption-osxphotos-exportdb-timestamp"],
-            [0, "cmdoption-osxphotos-import-timestamp"],
-            [0, "cmdoption-osxphotos-orphans-timestamp"],
-            [0, "cmdoption-osxphotos-sync-timestamp"],
-            [0, "cmdoption-osxphotos-timewarp-2"],
-            [0, "cmdoption-osxphotos-timewarp-timestamp"]
-        ],
-        "--timezone": [
-            [0, "cmdoption-osxphotos-timewarp-z"]
-        ],
-        "--title": [
-            [0, "cmdoption-osxphotos-add-locations-title"],
-            [0, "cmdoption-osxphotos-batch-edit-title"],
-            [0, "cmdoption-osxphotos-export-title"],
-            [0, "cmdoption-osxphotos-import-t"],
-            [0, "cmdoption-osxphotos-query-title"],
-            [0, "cmdoption-osxphotos-repl-title"],
-            [0, "cmdoption-osxphotos-sync-title"]
-        ],
-        "--tmpdir": [
-            [0, "cmdoption-osxphotos-export-tmpdir"]
-        ],
-        "--to-date": [
-            [0, "cmdoption-osxphotos-add-locations-to-date"],
-            [0, "cmdoption-osxphotos-export-to-date"],
-            [0, "cmdoption-osxphotos-query-to-date"],
-            [0, "cmdoption-osxphotos-repl-to-date"],
-            [0, "cmdoption-osxphotos-sync-to-date"]
-        ],
-        "--to-time": [
-            [0, "cmdoption-osxphotos-add-locations-to-time"],
-            [0, "cmdoption-osxphotos-export-to-time"],
-            [0, "cmdoption-osxphotos-query-to-time"],
-            [0, "cmdoption-osxphotos-repl-to-time"],
-            [0, "cmdoption-osxphotos-sync-to-time"]
-        ],
-        "--touch-file": [
-            [0, "cmdoption-osxphotos-export-touch-file"],
-            [0, "cmdoption-osxphotos-exportdb-touch-file"]
-        ],
-        "--undo": [
-            [0, "cmdoption-osxphotos-batch-edit-undo"]
-        ],
-        "--unmatched": [
-            [0, "cmdoption-osxphotos-sync-U"]
-        ],
-        "--update": [
-            [0, "cmdoption-osxphotos-export-update"]
-        ],
-        "--update-errors": [
-            [0, "cmdoption-osxphotos-export-update-errors"]
-        ],
-        "--update-signatures": [
-            [0, "cmdoption-osxphotos-exportdb-update-signatures"]
-        ],
-        "--upgrade": [
-            [0, "cmdoption-osxphotos-install-U"]
-        ],
-        "--use-file-time": [
-            [0, "cmdoption-osxphotos-timewarp-1"]
-        ],
-        "--use-photokit": [
-            [0, "cmdoption-osxphotos-export-use-photokit"]
-        ],
-        "--use-photos-export": [
-            [0, "cmdoption-osxphotos-export-use-photos-export"]
-        ],
-        "--uti": [
-            [0, "cmdoption-osxphotos-add-locations-uti"],
-            [0, "cmdoption-osxphotos-export-uti"],
-            [0, "cmdoption-osxphotos-query-uti"],
-            [0, "cmdoption-osxphotos-repl-uti"],
-            [0, "cmdoption-osxphotos-sync-uti"]
-        ],
-        "--uuid": [
-            [0, "cmdoption-osxphotos-add-locations-uuid"],
-            [0, "cmdoption-osxphotos-export-uuid"],
-            [0, "cmdoption-osxphotos-query-uuid"],
-            [0, "cmdoption-osxphotos-repl-uuid"],
-            [0, "cmdoption-osxphotos-sync-uuid"]
-        ],
-        "--uuid-files": [
-            [0, "cmdoption-osxphotos-exportdb-uuid-files"]
-        ],
-        "--uuid-from-file": [
-            [0, "cmdoption-osxphotos-add-locations-uuid-from-file"],
-            [0, "cmdoption-osxphotos-export-uuid-from-file"],
-            [0, "cmdoption-osxphotos-query-uuid-from-file"],
-            [0, "cmdoption-osxphotos-repl-uuid-from-file"],
-            [0, "cmdoption-osxphotos-sync-uuid-from-file"]
-        ],
-        "--uuid-info": [
-            [0, "cmdoption-osxphotos-exportdb-uuid-info"]
-        ],
-        "--vacuum": [
-            [0, "cmdoption-osxphotos-exportdb-vacuum"]
-        ],
-        "--verbose": [
-            [0, "cmdoption-osxphotos-add-locations-V"],
-            [0, "cmdoption-osxphotos-batch-edit-V"],
-            [0, "cmdoption-osxphotos-diff-V"],
-            [0, "cmdoption-osxphotos-exiftool-V"],
-            [0, "cmdoption-osxphotos-export-V"],
-            [0, "cmdoption-osxphotos-exportdb-V"],
-            [0, "cmdoption-osxphotos-import-V"],
-            [0, "cmdoption-osxphotos-orphans-V"],
-            [0, "cmdoption-osxphotos-sync-V"],
-            [0, "cmdoption-osxphotos-timewarp-V"]
-        ],
-        "--version": [
-            [0, "cmdoption-osxphotos-exportdb-version"],
-            [0, "cmdoption-osxphotos-v"]
-        ],
-        "--walk": [
-            [0, "cmdoption-osxphotos-import-w"]
-        ],
-        "--window": [
-            [0, "cmdoption-osxphotos-add-locations-w"]
-        ],
-        "--xattr-template": [
-            [0, "cmdoption-osxphotos-export-xattr-template"]
-        ],
-        "--year": [
-            [0, "cmdoption-osxphotos-add-locations-year"],
-            [0, "cmdoption-osxphotos-export-year"],
-            [0, "cmdoption-osxphotos-query-year"],
-            [0, "cmdoption-osxphotos-repl-year"],
-            [0, "cmdoption-osxphotos-sync-year"]
-        ],
-        "--yes": [
-            [0, "cmdoption-osxphotos-uninstall-y"]
-        ],
-        "-a": [
-            [0, "cmdoption-osxphotos-sync-A"],
-            [0, "cmdoption-osxphotos-import-a"],
-            [0, "cmdoption-osxphotos-timewarp-a"]
-        ],
-        "-c": [
-            [0, "cmdoption-osxphotos-import-C"],
-            [0, "cmdoption-osxphotos-timewarp-c"]
-        ],
-        "-d": [
-            [0, "cmdoption-osxphotos-import-D"],
-            [0, "cmdoption-osxphotos-timewarp-D"],
-            [0, "cmdoption-osxphotos-import-d"],
-            [0, "cmdoption-osxphotos-timewarp-d"]
-        ],
-        "-f": [
-            [0, "cmdoption-osxphotos-timewarp-F"],
-            [0, "cmdoption-osxphotos-dump-f"],
-            [0, "cmdoption-osxphotos-import-f"],
-            [0, "cmdoption-osxphotos-query-f"],
-            [0, "cmdoption-osxphotos-timewarp-1"],
-            [0, "cmdoption-osxphotos-uuid-f"]
-        ],
-        "-l": [
-            [0, "cmdoption-osxphotos-import-L"],
-            [0, "cmdoption-osxphotos-timewarp-L"],
-            [0, "cmdoption-osxphotos-import-l"]
-        ],
-        "-m": [
-            [0, "cmdoption-osxphotos-timewarp-M"],
-            [0, "cmdoption-osxphotos-import-m"],
-            [0, "cmdoption-osxphotos-sync-m"],
-            [0, "cmdoption-osxphotos-timewarp-0"]
-        ],
-        "-p": [
-            [0, "cmdoption-osxphotos-import-P"],
-            [0, "cmdoption-osxphotos-timewarp-P"],
-            [0, "cmdoption-osxphotos-import-0"],
-            [0, "cmdoption-osxphotos-timewarp-p"]
-        ],
-        "-r": [
-            [0, "cmdoption-osxphotos-import-R"],
-            [0, "cmdoption-osxphotos-sync-R"],
-            [0, "cmdoption-osxphotos-diff-r"],
-            [0, "cmdoption-osxphotos-import-r"]
-        ],
-        "-t": [
-            [0, "cmdoption-osxphotos-inspect-T"],
-            [0, "cmdoption-osxphotos-timewarp-T"],
-            [0, "cmdoption-osxphotos-import-t"],
-            [0, "cmdoption-osxphotos-inspect-t"],
-            [0, "cmdoption-osxphotos-timewarp-t"]
-        ],
-        "-u": [
-            [0, "cmdoption-osxphotos-install-U"],
-            [0, "cmdoption-osxphotos-sync-U"]
-        ],
-        "-v": [
-            [0, "cmdoption-osxphotos-add-locations-V"],
-            [0, "cmdoption-osxphotos-batch-edit-V"],
-            [0, "cmdoption-osxphotos-diff-V"],
-            [0, "cmdoption-osxphotos-exiftool-V"],
-            [0, "cmdoption-osxphotos-export-V"],
-            [0, "cmdoption-osxphotos-exportdb-V"],
-            [0, "cmdoption-osxphotos-import-V"],
-            [0, "cmdoption-osxphotos-orphans-V"],
-            [0, "cmdoption-osxphotos-sync-V"],
-            [0, "cmdoption-osxphotos-timewarp-V"],
-            [0, "cmdoption-osxphotos-v"]
-        ],
-        "-e": [
-            [0, "cmdoption-osxphotos-import-e"],
-            [0, "cmdoption-osxphotos-sync-e"],
-            [0, "cmdoption-osxphotos-timewarp-e"]
-        ],
-        "-g": [
-            [0, "cmdoption-osxphotos-import-g"]
-        ],
-        "-h": [
-            [0, "cmdoption-osxphotos-run-h"]
-        ],
-        "-i": [
-            [0, "cmdoption-osxphotos-add-locations-i"],
-            [0, "cmdoption-osxphotos-export-i"],
-            [0, "cmdoption-osxphotos-query-i"],
-            [0, "cmdoption-osxphotos-repl-i"],
-            [0, "cmdoption-osxphotos-sync-0"],
-            [0, "cmdoption-osxphotos-sync-i"],
-            [0, "cmdoption-osxphotos-timewarp-i"]
-        ],
-        "-k": [
-            [0, "cmdoption-osxphotos-import-k"]
-        ],
-        "-s": [
-            [0, "cmdoption-osxphotos-diff-s"],
-            [0, "cmdoption-osxphotos-sync-s"]
-        ],
-        "-w": [
-            [0, "cmdoption-osxphotos-add-locations-w"],
-            [0, "cmdoption-osxphotos-import-w"]
-        ],
-        "-y": [
-            [0, "cmdoption-osxphotos-uninstall-y"]
-        ],
-        "-z": [
-            [0, "cmdoption-osxphotos-timewarp-z"]
-        ],
-        "args": [
-            [0, "cmdoption-osxphotos-run-arg-ARGS"]
-        ],
-        "db2": [
-            [0, "cmdoption-osxphotos-diff-arg-DB2"]
-        ],
-        "dest": [
-            [0, "cmdoption-osxphotos-export-arg-DEST"]
-        ],
-        "export_database": [
-            [0, "cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE"]
-        ],
-        "export_directory": [
-            [0, "cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY"]
-        ],
-        "files": [
-            [0, "cmdoption-osxphotos-import-arg-FILES"]
-        ],
-        "packages": [
-            [0, "cmdoption-osxphotos-install-arg-PACKAGES"],
-            [0, "cmdoption-osxphotos-uninstall-arg-PACKAGES"]
-        ],
-        "photos_library": [
-            [0, "cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY"]
-        ],
-        "python_file": [
-            [0, "cmdoption-osxphotos-run-arg-PYTHON_FILE"]
-        ],
-        "subtopic": [
-            [0, "cmdoption-osxphotos-help-arg-SUBTOPIC"]
-        ],
-        "topic": [
-            [0, "cmdoption-osxphotos-help-arg-TOPIC"]
-        ],
-        "uuid_or_name": [
-            [0, "cmdoption-osxphotos-show-arg-UUID_OR_NAME"]
-        ],
-        "width": [
-            [0, "cmdoption-osxphotos-tutorial-arg-WIDTH"]
-        ],
-        "osxphotos command line option": [
-            [0, "cmdoption-osxphotos-json"],
-            [0, "cmdoption-osxphotos-library"],
-            [0, "cmdoption-osxphotos-v"]
-        ],
-        "osxphotos-add-locations command line option": [
-            [0, "cmdoption-osxphotos-add-locations-V"],
-            [0, "cmdoption-osxphotos-add-locations-added-after"],
-            [0, "cmdoption-osxphotos-add-locations-added-before"],
-            [0, "cmdoption-osxphotos-add-locations-added-in-last"],
-            [0, "cmdoption-osxphotos-add-locations-album"],
-            [0, "cmdoption-osxphotos-add-locations-burst"],
-            [0, "cmdoption-osxphotos-add-locations-cloudasset"],
-            [0, "cmdoption-osxphotos-add-locations-description"],
-            [0, "cmdoption-osxphotos-add-locations-dry-run"],
-            [0, "cmdoption-osxphotos-add-locations-duplicate"],
-            [0, "cmdoption-osxphotos-add-locations-edited"],
-            [0, "cmdoption-osxphotos-add-locations-exif"],
-            [0, "cmdoption-osxphotos-add-locations-external-edit"],
-            [0, "cmdoption-osxphotos-add-locations-favorite"],
-            [0, "cmdoption-osxphotos-add-locations-folder"],
-            [0, "cmdoption-osxphotos-add-locations-from-date"],
-            [0, "cmdoption-osxphotos-add-locations-from-time"],
-            [0, "cmdoption-osxphotos-add-locations-has-comment"],
-            [0, "cmdoption-osxphotos-add-locations-has-likes"],
-            [0, "cmdoption-osxphotos-add-locations-has-raw"],
-            [0, "cmdoption-osxphotos-add-locations-hdr"],
-            [0, "cmdoption-osxphotos-add-locations-hidden"],
-            [0, "cmdoption-osxphotos-add-locations-i"],
-            [0, "cmdoption-osxphotos-add-locations-in-album"],
-            [0, "cmdoption-osxphotos-add-locations-incloud"],
-            [0, "cmdoption-osxphotos-add-locations-is-reference"],
-            [0, "cmdoption-osxphotos-add-locations-keyword"],
-            [0, "cmdoption-osxphotos-add-locations-label"],
-            [0, "cmdoption-osxphotos-add-locations-live"],
-            [0, "cmdoption-osxphotos-add-locations-location"],
-            [0, "cmdoption-osxphotos-add-locations-max-size"],
-            [0, "cmdoption-osxphotos-add-locations-min-size"],
-            [0, "cmdoption-osxphotos-add-locations-missing"],
-            [0, "cmdoption-osxphotos-add-locations-name"],
-            [0, "cmdoption-osxphotos-add-locations-no-comment"],
-            [0, "cmdoption-osxphotos-add-locations-no-description"],
-            [0, "cmdoption-osxphotos-add-locations-no-keyword"],
-            [0, "cmdoption-osxphotos-add-locations-no-likes"],
-            [0, "cmdoption-osxphotos-add-locations-no-location"],
-            [0, "cmdoption-osxphotos-add-locations-no-place"],
-            [0, "cmdoption-osxphotos-add-locations-no-title"],
-            [0, "cmdoption-osxphotos-add-locations-not-burst"],
-            [0, "cmdoption-osxphotos-add-locations-not-cloudasset"],
-            [0, "cmdoption-osxphotos-add-locations-not-edited"],
-            [0, "cmdoption-osxphotos-add-locations-not-favorite"],
-            [0, "cmdoption-osxphotos-add-locations-not-hdr"],
-            [0, "cmdoption-osxphotos-add-locations-not-hidden"],
-            [0, "cmdoption-osxphotos-add-locations-not-in-album"],
-            [0, "cmdoption-osxphotos-add-locations-not-incloud"],
-            [0, "cmdoption-osxphotos-add-locations-not-live"],
-            [0, "cmdoption-osxphotos-add-locations-not-missing"],
-            [0, "cmdoption-osxphotos-add-locations-not-panorama"],
-            [0, "cmdoption-osxphotos-add-locations-not-portrait"],
-            [0, "cmdoption-osxphotos-add-locations-not-reference"],
-            [0, "cmdoption-osxphotos-add-locations-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
-            [0, "cmdoption-osxphotos-add-locations-not-selfie"],
-            [0, "cmdoption-osxphotos-add-locations-not-shared"],
-            [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
-            [0, "cmdoption-osxphotos-add-locations-not-syndicated"],
-            [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
-            [0, "cmdoption-osxphotos-add-locations-only-movies"],
-            [0, "cmdoption-osxphotos-add-locations-only-photos"],
-            [0, "cmdoption-osxphotos-add-locations-panorama"],
-            [0, "cmdoption-osxphotos-add-locations-person"],
-            [0, "cmdoption-osxphotos-add-locations-place"],
-            [0, "cmdoption-osxphotos-add-locations-portrait"],
-            [0, "cmdoption-osxphotos-add-locations-query-eval"],
-            [0, "cmdoption-osxphotos-add-locations-query-function"],
-            [0, "cmdoption-osxphotos-add-locations-regex"],
-            [0, "cmdoption-osxphotos-add-locations-saved-to-library"],
-            [0, "cmdoption-osxphotos-add-locations-screenshot"],
-            [0, "cmdoption-osxphotos-add-locations-selected"],
-            [0, "cmdoption-osxphotos-add-locations-selfie"],
-            [0, "cmdoption-osxphotos-add-locations-shared"],
-            [0, "cmdoption-osxphotos-add-locations-slow-mo"],
-            [0, "cmdoption-osxphotos-add-locations-syndicated"],
-            [0, "cmdoption-osxphotos-add-locations-theme"],
-            [0, "cmdoption-osxphotos-add-locations-time-lapse"],
-            [0, "cmdoption-osxphotos-add-locations-timestamp"],
-            [0, "cmdoption-osxphotos-add-locations-title"],
-            [0, "cmdoption-osxphotos-add-locations-to-date"],
-            [0, "cmdoption-osxphotos-add-locations-to-time"],
-            [0, "cmdoption-osxphotos-add-locations-uti"],
-            [0, "cmdoption-osxphotos-add-locations-uuid"],
-            [0, "cmdoption-osxphotos-add-locations-uuid-from-file"],
-            [0, "cmdoption-osxphotos-add-locations-w"],
-            [0, "cmdoption-osxphotos-add-locations-year"]
-        ],
-        "osxphotos-albums command line option": [
-            [0, "cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-albums-json"],
-            [0, "cmdoption-osxphotos-albums-library"]
-        ],
-        "osxphotos-batch-edit command line option": [
-            [0, "cmdoption-osxphotos-batch-edit-V"],
-            [0, "cmdoption-osxphotos-batch-edit-description"],
-            [0, "cmdoption-osxphotos-batch-edit-dry-run"],
-            [0, "cmdoption-osxphotos-batch-edit-keyword"],
-            [0, "cmdoption-osxphotos-batch-edit-library"],
-            [0, "cmdoption-osxphotos-batch-edit-location"],
-            [0, "cmdoption-osxphotos-batch-edit-replace-keywords"],
-            [0, "cmdoption-osxphotos-batch-edit-theme"],
-            [0, "cmdoption-osxphotos-batch-edit-timestamp"],
-            [0, "cmdoption-osxphotos-batch-edit-title"],
-            [0, "cmdoption-osxphotos-batch-edit-undo"]
-        ],
-        "osxphotos-diff command line option": [
-            [0, "cmdoption-osxphotos-diff-V"],
-            [0, "cmdoption-osxphotos-diff-arg-DB2"],
-            [0, "cmdoption-osxphotos-diff-library"],
-            [0, "cmdoption-osxphotos-diff-r"],
-            [0, "cmdoption-osxphotos-diff-s"],
-            [0, "cmdoption-osxphotos-diff-timestamp"]
-        ],
-        "osxphotos-dump command line option": [
-            [0, "cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-dump-deleted"],
-            [0, "cmdoption-osxphotos-dump-deleted-only"],
-            [0, "cmdoption-osxphotos-dump-f"],
-            [0, "cmdoption-osxphotos-dump-json"],
-            [0, "cmdoption-osxphotos-dump-library"],
-            [0, "cmdoption-osxphotos-dump-print"]
-        ],
-        "osxphotos-exiftool command line option": [
-            [0, "cmdoption-osxphotos-exiftool-V"],
-            [0, "cmdoption-osxphotos-exiftool-album-keyword"],
-            [0, "cmdoption-osxphotos-exiftool-append"],
-            [0, "cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY"],
-            [0, "cmdoption-osxphotos-exiftool-db-config"],
-            [0, "cmdoption-osxphotos-exiftool-description-template"],
-            [0, "cmdoption-osxphotos-exiftool-dry-run"],
-            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-keywords"],
-            [0, "cmdoption-osxphotos-exiftool-exiftool-merge-persons"],
-            [0, "cmdoption-osxphotos-exiftool-exiftool-option"],
-            [0, "cmdoption-osxphotos-exiftool-exiftool-path"],
-            [0, "cmdoption-osxphotos-exiftool-exportdb"],
-            [0, "cmdoption-osxphotos-exiftool-ignore-date-modified"],
-            [0, "cmdoption-osxphotos-exiftool-keyword-template"],
-            [0, "cmdoption-osxphotos-exiftool-library"],
-            [0, "cmdoption-osxphotos-exiftool-load-config"],
-            [0, "cmdoption-osxphotos-exiftool-person-keyword"],
-            [0, "cmdoption-osxphotos-exiftool-replace-keywords"],
-            [0, "cmdoption-osxphotos-exiftool-report"],
-            [0, "cmdoption-osxphotos-exiftool-save-config"],
-            [0, "cmdoption-osxphotos-exiftool-theme"],
-            [0, "cmdoption-osxphotos-exiftool-timestamp"]
-        ],
-        "osxphotos-export command line option": [
-            [0, "cmdoption-osxphotos-export-V"],
-            [0, "cmdoption-osxphotos-export-add-exported-to-album"],
-            [0, "cmdoption-osxphotos-export-add-missing-to-album"],
-            [0, "cmdoption-osxphotos-export-add-skipped-to-album"],
-            [0, "cmdoption-osxphotos-export-added-after"],
-            [0, "cmdoption-osxphotos-export-added-before"],
-            [0, "cmdoption-osxphotos-export-added-in-last"],
-            [0, "cmdoption-osxphotos-export-album"],
-            [0, "cmdoption-osxphotos-export-album-keyword"],
-            [0, "cmdoption-osxphotos-export-alt-copy"],
-            [0, "cmdoption-osxphotos-export-append"],
-            [0, "cmdoption-osxphotos-export-arg-DEST"],
-            [0, "cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-export-burst"],
-            [0, "cmdoption-osxphotos-export-cleanup"],
-            [0, "cmdoption-osxphotos-export-cloudasset"],
-            [0, "cmdoption-osxphotos-export-config-only"],
-            [0, "cmdoption-osxphotos-export-convert-to-jpeg"],
-            [0, "cmdoption-osxphotos-export-current-name"],
-            [0, "cmdoption-osxphotos-export-deleted"],
-            [0, "cmdoption-osxphotos-export-deleted-only"],
-            [0, "cmdoption-osxphotos-export-description"],
-            [0, "cmdoption-osxphotos-export-description-template"],
-            [0, "cmdoption-osxphotos-export-directory"],
-            [0, "cmdoption-osxphotos-export-download-missing"],
-            [0, "cmdoption-osxphotos-export-dry-run"],
-            [0, "cmdoption-osxphotos-export-duplicate"],
-            [0, "cmdoption-osxphotos-export-edited"],
-            [0, "cmdoption-osxphotos-export-edited-suffix"],
-            [0, "cmdoption-osxphotos-export-exif"],
-            [0, "cmdoption-osxphotos-export-exiftool"],
-            [0, "cmdoption-osxphotos-export-exiftool-merge-keywords"],
-            [0, "cmdoption-osxphotos-export-exiftool-merge-persons"],
-            [0, "cmdoption-osxphotos-export-exiftool-option"],
-            [0, "cmdoption-osxphotos-export-exiftool-path"],
-            [0, "cmdoption-osxphotos-export-export-as-hardlink"],
-            [0, "cmdoption-osxphotos-export-export-by-date"],
-            [0, "cmdoption-osxphotos-export-exportdb"],
-            [0, "cmdoption-osxphotos-export-external-edit"],
-            [0, "cmdoption-osxphotos-export-favorite"],
-            [0, "cmdoption-osxphotos-export-favorite-rating"],
-            [0, "cmdoption-osxphotos-export-filename"],
-            [0, "cmdoption-osxphotos-export-finder-tag-keywords"],
-            [0, "cmdoption-osxphotos-export-finder-tag-template"],
-            [0, "cmdoption-osxphotos-export-folder"],
-            [0, "cmdoption-osxphotos-export-force-update"],
-            [0, "cmdoption-osxphotos-export-from-date"],
-            [0, "cmdoption-osxphotos-export-from-time"],
-            [0, "cmdoption-osxphotos-export-has-comment"],
-            [0, "cmdoption-osxphotos-export-has-likes"],
-            [0, "cmdoption-osxphotos-export-has-raw"],
-            [0, "cmdoption-osxphotos-export-hdr"],
-            [0, "cmdoption-osxphotos-export-hidden"],
-            [0, "cmdoption-osxphotos-export-i"],
-            [0, "cmdoption-osxphotos-export-ignore-date-modified"],
-            [0, "cmdoption-osxphotos-export-ignore-signature"],
-            [0, "cmdoption-osxphotos-export-in-album"],
-            [0, "cmdoption-osxphotos-export-incloud"],
-            [0, "cmdoption-osxphotos-export-is-reference"],
-            [0, "cmdoption-osxphotos-export-jpeg-ext"],
-            [0, "cmdoption-osxphotos-export-jpeg-quality"],
-            [0, "cmdoption-osxphotos-export-keep"],
-            [0, "cmdoption-osxphotos-export-keyword"],
-            [0, "cmdoption-osxphotos-export-keyword-template"],
-            [0, "cmdoption-osxphotos-export-label"],
-            [0, "cmdoption-osxphotos-export-library"],
-            [0, "cmdoption-osxphotos-export-limit"],
-            [0, "cmdoption-osxphotos-export-live"],
-            [0, "cmdoption-osxphotos-export-load-config"],
-            [0, "cmdoption-osxphotos-export-location"],
-            [0, "cmdoption-osxphotos-export-max-size"],
-            [0, "cmdoption-osxphotos-export-min-size"],
-            [0, "cmdoption-osxphotos-export-missing"],
-            [0, "cmdoption-osxphotos-export-name"],
-            [0, "cmdoption-osxphotos-export-no-comment"],
-            [0, "cmdoption-osxphotos-export-no-description"],
-            [0, "cmdoption-osxphotos-export-no-keyword"],
-            [0, "cmdoption-osxphotos-export-no-likes"],
-            [0, "cmdoption-osxphotos-export-no-location"],
-            [0, "cmdoption-osxphotos-export-no-place"],
-            [0, "cmdoption-osxphotos-export-no-progress"],
-            [0, "cmdoption-osxphotos-export-no-title"],
-            [0, "cmdoption-osxphotos-export-not-burst"],
-            [0, "cmdoption-osxphotos-export-not-cloudasset"],
-            [0, "cmdoption-osxphotos-export-not-edited"],
-            [0, "cmdoption-osxphotos-export-not-favorite"],
-            [0, "cmdoption-osxphotos-export-not-hdr"],
-            [0, "cmdoption-osxphotos-export-not-hidden"],
-            [0, "cmdoption-osxphotos-export-not-in-album"],
-            [0, "cmdoption-osxphotos-export-not-incloud"],
-            [0, "cmdoption-osxphotos-export-not-live"],
-            [0, "cmdoption-osxphotos-export-not-missing"],
-            [0, "cmdoption-osxphotos-export-not-panorama"],
-            [0, "cmdoption-osxphotos-export-not-portrait"],
-            [0, "cmdoption-osxphotos-export-not-reference"],
-            [0, "cmdoption-osxphotos-export-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-export-not-screenshot"],
-            [0, "cmdoption-osxphotos-export-not-selfie"],
-            [0, "cmdoption-osxphotos-export-not-shared"],
-            [0, "cmdoption-osxphotos-export-not-slow-mo"],
-            [0, "cmdoption-osxphotos-export-not-syndicated"],
-            [0, "cmdoption-osxphotos-export-not-time-lapse"],
-            [0, "cmdoption-osxphotos-export-only-movies"],
-            [0, "cmdoption-osxphotos-export-only-new"],
-            [0, "cmdoption-osxphotos-export-only-photos"],
-            [0, "cmdoption-osxphotos-export-original-suffix"],
-            [0, "cmdoption-osxphotos-export-overwrite"],
-            [0, "cmdoption-osxphotos-export-panorama"],
-            [0, "cmdoption-osxphotos-export-person"],
-            [0, "cmdoption-osxphotos-export-person-keyword"],
-            [0, "cmdoption-osxphotos-export-place"],
-            [0, "cmdoption-osxphotos-export-portrait"],
-            [0, "cmdoption-osxphotos-export-post-command"],
-            [0, "cmdoption-osxphotos-export-post-function"],
-            [0, "cmdoption-osxphotos-export-preview"],
-            [0, "cmdoption-osxphotos-export-preview-if-missing"],
-            [0, "cmdoption-osxphotos-export-preview-suffix"],
-            [0, "cmdoption-osxphotos-export-print"],
-            [0, "cmdoption-osxphotos-export-query-eval"],
-            [0, "cmdoption-osxphotos-export-query-function"],
-            [0, "cmdoption-osxphotos-export-ramdb"],
-            [0, "cmdoption-osxphotos-export-regex"],
-            [0, "cmdoption-osxphotos-export-replace-keywords"],
-            [0, "cmdoption-osxphotos-export-report"],
-            [0, "cmdoption-osxphotos-export-retry"],
-            [0, "cmdoption-osxphotos-export-save-config"],
-            [0, "cmdoption-osxphotos-export-saved-to-library"],
-            [0, "cmdoption-osxphotos-export-screenshot"],
-            [0, "cmdoption-osxphotos-export-selected"],
-            [0, "cmdoption-osxphotos-export-selfie"],
-            [0, "cmdoption-osxphotos-export-shared"],
-            [0, "cmdoption-osxphotos-export-sidecar"],
-            [0, "cmdoption-osxphotos-export-sidecar-drop-ext"],
-            [0, "cmdoption-osxphotos-export-skip-bursts"],
-            [0, "cmdoption-osxphotos-export-skip-edited"],
-            [0, "cmdoption-osxphotos-export-skip-live"],
-            [0, "cmdoption-osxphotos-export-skip-original-if-edited"],
-            [0, "cmdoption-osxphotos-export-skip-raw"],
-            [0, "cmdoption-osxphotos-export-skip-uuid"],
-            [0, "cmdoption-osxphotos-export-skip-uuid-from-file"],
-            [0, "cmdoption-osxphotos-export-slow-mo"],
-            [0, "cmdoption-osxphotos-export-strip"],
-            [0, "cmdoption-osxphotos-export-syndicated"],
-            [0, "cmdoption-osxphotos-export-theme"],
-            [0, "cmdoption-osxphotos-export-time-lapse"],
-            [0, "cmdoption-osxphotos-export-timestamp"],
-            [0, "cmdoption-osxphotos-export-title"],
-            [0, "cmdoption-osxphotos-export-tmpdir"],
-            [0, "cmdoption-osxphotos-export-to-date"],
-            [0, "cmdoption-osxphotos-export-to-time"],
-            [0, "cmdoption-osxphotos-export-touch-file"],
-            [0, "cmdoption-osxphotos-export-update"],
-            [0, "cmdoption-osxphotos-export-update-errors"],
-            [0, "cmdoption-osxphotos-export-use-photokit"],
-            [0, "cmdoption-osxphotos-export-use-photos-export"],
-            [0, "cmdoption-osxphotos-export-uti"],
-            [0, "cmdoption-osxphotos-export-uuid"],
-            [0, "cmdoption-osxphotos-export-uuid-from-file"],
-            [0, "cmdoption-osxphotos-export-xattr-template"],
-            [0, "cmdoption-osxphotos-export-year"]
-        ],
-        "osxphotos-exportdb command line option": [
-            [0, "cmdoption-osxphotos-exportdb-V"],
-            [0, "cmdoption-osxphotos-exportdb-append"],
-            [0, "cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE"],
-            [0, "cmdoption-osxphotos-exportdb-check-signatures"],
-            [0, "cmdoption-osxphotos-exportdb-delete-file"],
-            [0, "cmdoption-osxphotos-exportdb-delete-uuid"],
-            [0, "cmdoption-osxphotos-exportdb-dry-run"],
-            [0, "cmdoption-osxphotos-exportdb-errors"],
-            [0, "cmdoption-osxphotos-exportdb-export-dir"],
-            [0, "cmdoption-osxphotos-exportdb-info"],
-            [0, "cmdoption-osxphotos-exportdb-last-errors"],
-            [0, "cmdoption-osxphotos-exportdb-last-run"],
-            [0, "cmdoption-osxphotos-exportdb-migrate"],
-            [0, "cmdoption-osxphotos-exportdb-migrate-photos-library"],
-            [0, "cmdoption-osxphotos-exportdb-report"],
-            [0, "cmdoption-osxphotos-exportdb-save-config"],
-            [0, "cmdoption-osxphotos-exportdb-sql"],
-            [0, "cmdoption-osxphotos-exportdb-theme"],
-            [0, "cmdoption-osxphotos-exportdb-timestamp"],
-            [0, "cmdoption-osxphotos-exportdb-touch-file"],
-            [0, "cmdoption-osxphotos-exportdb-update-signatures"],
-            [0, "cmdoption-osxphotos-exportdb-uuid-files"],
-            [0, "cmdoption-osxphotos-exportdb-uuid-info"],
-            [0, "cmdoption-osxphotos-exportdb-vacuum"],
-            [0, "cmdoption-osxphotos-exportdb-version"]
-        ],
-        "osxphotos-help command line option": [
-            [0, "cmdoption-osxphotos-help-arg-SUBTOPIC"],
-            [0, "cmdoption-osxphotos-help-arg-TOPIC"]
-        ],
-        "osxphotos-import command line option": [
-            [0, "cmdoption-osxphotos-import-0"],
-            [0, "cmdoption-osxphotos-import-C"],
-            [0, "cmdoption-osxphotos-import-D"],
-            [0, "cmdoption-osxphotos-import-L"],
-            [0, "cmdoption-osxphotos-import-P"],
-            [0, "cmdoption-osxphotos-import-R"],
-            [0, "cmdoption-osxphotos-import-V"],
-            [0, "cmdoption-osxphotos-import-a"],
-            [0, "cmdoption-osxphotos-import-append"],
-            [0, "cmdoption-osxphotos-import-arg-FILES"],
-            [0, "cmdoption-osxphotos-import-check-templates"],
-            [0, "cmdoption-osxphotos-import-d"],
-            [0, "cmdoption-osxphotos-import-e"],
-            [0, "cmdoption-osxphotos-import-f"],
-            [0, "cmdoption-osxphotos-import-g"],
-            [0, "cmdoption-osxphotos-import-k"],
-            [0, "cmdoption-osxphotos-import-l"],
-            [0, "cmdoption-osxphotos-import-m"],
-            [0, "cmdoption-osxphotos-import-no-progress"],
-            [0, "cmdoption-osxphotos-import-post-function"],
-            [0, "cmdoption-osxphotos-import-r"],
-            [0, "cmdoption-osxphotos-import-report"],
-            [0, "cmdoption-osxphotos-import-t"],
-            [0, "cmdoption-osxphotos-import-theme"],
-            [0, "cmdoption-osxphotos-import-timestamp"],
-            [0, "cmdoption-osxphotos-import-w"]
-        ],
-        "osxphotos-info command line option": [
-            [0, "cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-info-json"],
-            [0, "cmdoption-osxphotos-info-library"]
-        ],
-        "osxphotos-inspect command line option": [
-            [0, "cmdoption-osxphotos-inspect-T"],
-            [0, "cmdoption-osxphotos-inspect-library"],
-            [0, "cmdoption-osxphotos-inspect-t"],
-            [0, "cmdoption-osxphotos-inspect-theme"]
-        ],
-        "osxphotos-install command line option": [
-            [0, "cmdoption-osxphotos-install-U"],
-            [0, "cmdoption-osxphotos-install-arg-PACKAGES"]
-        ],
-        "osxphotos-keywords command line option": [
-            [0, "cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-keywords-json"],
-            [0, "cmdoption-osxphotos-keywords-library"]
-        ],
-        "osxphotos-labels command line option": [
-            [0, "cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-labels-json"],
-            [0, "cmdoption-osxphotos-labels-library"]
-        ],
-        "osxphotos-list command line option": [
-            [0, "cmdoption-osxphotos-list-json"]
-        ],
-        "osxphotos-orphans command line option": [
-            [0, "cmdoption-osxphotos-orphans-V"],
-            [0, "cmdoption-osxphotos-orphans-export"],
-            [0, "cmdoption-osxphotos-orphans-library"],
-            [0, "cmdoption-osxphotos-orphans-theme"],
-            [0, "cmdoption-osxphotos-orphans-timestamp"]
-        ],
-        "osxphotos-persons command line option": [
-            [0, "cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-persons-json"],
-            [0, "cmdoption-osxphotos-persons-library"]
-        ],
-        "osxphotos-places command line option": [
-            [0, "cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-places-json"],
-            [0, "cmdoption-osxphotos-places-library"]
-        ],
-        "osxphotos-query command line option": [
-            [0, "cmdoption-osxphotos-query-add-to-album"],
-            [0, "cmdoption-osxphotos-query-added-after"],
-            [0, "cmdoption-osxphotos-query-added-before"],
-            [0, "cmdoption-osxphotos-query-added-in-last"],
-            [0, "cmdoption-osxphotos-query-album"],
-            [0, "cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY"],
-            [0, "cmdoption-osxphotos-query-burst"],
-            [0, "cmdoption-osxphotos-query-cloudasset"],
-            [0, "cmdoption-osxphotos-query-deleted"],
-            [0, "cmdoption-osxphotos-query-deleted-only"],
-            [0, "cmdoption-osxphotos-query-description"],
-            [0, "cmdoption-osxphotos-query-duplicate"],
-            [0, "cmdoption-osxphotos-query-edited"],
-            [0, "cmdoption-osxphotos-query-exif"],
-            [0, "cmdoption-osxphotos-query-external-edit"],
-            [0, "cmdoption-osxphotos-query-f"],
-            [0, "cmdoption-osxphotos-query-favorite"],
-            [0, "cmdoption-osxphotos-query-folder"],
-            [0, "cmdoption-osxphotos-query-from-date"],
-            [0, "cmdoption-osxphotos-query-from-time"],
-            [0, "cmdoption-osxphotos-query-has-comment"],
-            [0, "cmdoption-osxphotos-query-has-likes"],
-            [0, "cmdoption-osxphotos-query-has-raw"],
-            [0, "cmdoption-osxphotos-query-hdr"],
-            [0, "cmdoption-osxphotos-query-hidden"],
-            [0, "cmdoption-osxphotos-query-i"],
-            [0, "cmdoption-osxphotos-query-in-album"],
-            [0, "cmdoption-osxphotos-query-incloud"],
-            [0, "cmdoption-osxphotos-query-is-reference"],
-            [0, "cmdoption-osxphotos-query-json"],
-            [0, "cmdoption-osxphotos-query-keyword"],
-            [0, "cmdoption-osxphotos-query-label"],
-            [0, "cmdoption-osxphotos-query-library"],
-            [0, "cmdoption-osxphotos-query-live"],
-            [0, "cmdoption-osxphotos-query-location"],
-            [0, "cmdoption-osxphotos-query-max-size"],
-            [0, "cmdoption-osxphotos-query-min-size"],
-            [0, "cmdoption-osxphotos-query-missing"],
-            [0, "cmdoption-osxphotos-query-name"],
-            [0, "cmdoption-osxphotos-query-no-comment"],
-            [0, "cmdoption-osxphotos-query-no-description"],
-            [0, "cmdoption-osxphotos-query-no-keyword"],
-            [0, "cmdoption-osxphotos-query-no-likes"],
-            [0, "cmdoption-osxphotos-query-no-location"],
-            [0, "cmdoption-osxphotos-query-no-place"],
-            [0, "cmdoption-osxphotos-query-no-title"],
-            [0, "cmdoption-osxphotos-query-not-burst"],
-            [0, "cmdoption-osxphotos-query-not-cloudasset"],
-            [0, "cmdoption-osxphotos-query-not-edited"],
-            [0, "cmdoption-osxphotos-query-not-favorite"],
-            [0, "cmdoption-osxphotos-query-not-hdr"],
-            [0, "cmdoption-osxphotos-query-not-hidden"],
-            [0, "cmdoption-osxphotos-query-not-in-album"],
-            [0, "cmdoption-osxphotos-query-not-incloud"],
-            [0, "cmdoption-osxphotos-query-not-live"],
-            [0, "cmdoption-osxphotos-query-not-missing"],
-            [0, "cmdoption-osxphotos-query-not-panorama"],
-            [0, "cmdoption-osxphotos-query-not-portrait"],
-            [0, "cmdoption-osxphotos-query-not-reference"],
-            [0, "cmdoption-osxphotos-query-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-query-not-screenshot"],
-            [0, "cmdoption-osxphotos-query-not-selfie"],
-            [0, "cmdoption-osxphotos-query-not-shared"],
-            [0, "cmdoption-osxphotos-query-not-slow-mo"],
-            [0, "cmdoption-osxphotos-query-not-syndicated"],
-            [0, "cmdoption-osxphotos-query-not-time-lapse"],
-            [0, "cmdoption-osxphotos-query-only-movies"],
-            [0, "cmdoption-osxphotos-query-only-photos"],
-            [0, "cmdoption-osxphotos-query-panorama"],
-            [0, "cmdoption-osxphotos-query-person"],
-            [0, "cmdoption-osxphotos-query-place"],
-            [0, "cmdoption-osxphotos-query-portrait"],
-            [0, "cmdoption-osxphotos-query-print"],
-            [0, "cmdoption-osxphotos-query-query-eval"],
-            [0, "cmdoption-osxphotos-query-query-function"],
-            [0, "cmdoption-osxphotos-query-quiet"],
-            [0, "cmdoption-osxphotos-query-regex"],
-            [0, "cmdoption-osxphotos-query-saved-to-library"],
-            [0, "cmdoption-osxphotos-query-screenshot"],
-            [0, "cmdoption-osxphotos-query-selected"],
-            [0, "cmdoption-osxphotos-query-selfie"],
-            [0, "cmdoption-osxphotos-query-shared"],
-            [0, "cmdoption-osxphotos-query-slow-mo"],
-            [0, "cmdoption-osxphotos-query-syndicated"],
-            [0, "cmdoption-osxphotos-query-time-lapse"],
-            [0, "cmdoption-osxphotos-query-title"],
-            [0, "cmdoption-osxphotos-query-to-date"],
-            [0, "cmdoption-osxphotos-query-to-time"],
-            [0, "cmdoption-osxphotos-query-uti"],
-            [0, "cmdoption-osxphotos-query-uuid"],
-            [0, "cmdoption-osxphotos-query-uuid-from-file"],
-            [0, "cmdoption-osxphotos-query-year"]
-        ],
-        "osxphotos-repl command line option": [
-            [0, "cmdoption-osxphotos-repl-added-after"],
-            [0, "cmdoption-osxphotos-repl-added-before"],
-            [0, "cmdoption-osxphotos-repl-added-in-last"],
-            [0, "cmdoption-osxphotos-repl-album"],
-            [0, "cmdoption-osxphotos-repl-burst"],
-            [0, "cmdoption-osxphotos-repl-cloudasset"],
-            [0, "cmdoption-osxphotos-repl-deleted"],
-            [0, "cmdoption-osxphotos-repl-deleted-only"],
-            [0, "cmdoption-osxphotos-repl-description"],
-            [0, "cmdoption-osxphotos-repl-duplicate"],
-            [0, "cmdoption-osxphotos-repl-edited"],
-            [0, "cmdoption-osxphotos-repl-emacs"],
-            [0, "cmdoption-osxphotos-repl-exif"],
-            [0, "cmdoption-osxphotos-repl-external-edit"],
-            [0, "cmdoption-osxphotos-repl-favorite"],
-            [0, "cmdoption-osxphotos-repl-folder"],
-            [0, "cmdoption-osxphotos-repl-from-date"],
-            [0, "cmdoption-osxphotos-repl-from-time"],
-            [0, "cmdoption-osxphotos-repl-has-comment"],
-            [0, "cmdoption-osxphotos-repl-has-likes"],
-            [0, "cmdoption-osxphotos-repl-has-raw"],
-            [0, "cmdoption-osxphotos-repl-hdr"],
-            [0, "cmdoption-osxphotos-repl-hidden"],
-            [0, "cmdoption-osxphotos-repl-i"],
-            [0, "cmdoption-osxphotos-repl-in-album"],
-            [0, "cmdoption-osxphotos-repl-incloud"],
-            [0, "cmdoption-osxphotos-repl-is-reference"],
-            [0, "cmdoption-osxphotos-repl-keyword"],
-            [0, "cmdoption-osxphotos-repl-label"],
-            [0, "cmdoption-osxphotos-repl-library"],
-            [0, "cmdoption-osxphotos-repl-live"],
-            [0, "cmdoption-osxphotos-repl-location"],
-            [0, "cmdoption-osxphotos-repl-max-size"],
-            [0, "cmdoption-osxphotos-repl-min-size"],
-            [0, "cmdoption-osxphotos-repl-missing"],
-            [0, "cmdoption-osxphotos-repl-name"],
-            [0, "cmdoption-osxphotos-repl-no-comment"],
-            [0, "cmdoption-osxphotos-repl-no-description"],
-            [0, "cmdoption-osxphotos-repl-no-keyword"],
-            [0, "cmdoption-osxphotos-repl-no-likes"],
-            [0, "cmdoption-osxphotos-repl-no-location"],
-            [0, "cmdoption-osxphotos-repl-no-place"],
-            [0, "cmdoption-osxphotos-repl-no-title"],
-            [0, "cmdoption-osxphotos-repl-not-burst"],
-            [0, "cmdoption-osxphotos-repl-not-cloudasset"],
-            [0, "cmdoption-osxphotos-repl-not-edited"],
-            [0, "cmdoption-osxphotos-repl-not-favorite"],
-            [0, "cmdoption-osxphotos-repl-not-hdr"],
-            [0, "cmdoption-osxphotos-repl-not-hidden"],
-            [0, "cmdoption-osxphotos-repl-not-in-album"],
-            [0, "cmdoption-osxphotos-repl-not-incloud"],
-            [0, "cmdoption-osxphotos-repl-not-live"],
-            [0, "cmdoption-osxphotos-repl-not-missing"],
-            [0, "cmdoption-osxphotos-repl-not-panorama"],
-            [0, "cmdoption-osxphotos-repl-not-portrait"],
-            [0, "cmdoption-osxphotos-repl-not-reference"],
-            [0, "cmdoption-osxphotos-repl-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-repl-not-screenshot"],
-            [0, "cmdoption-osxphotos-repl-not-selfie"],
-            [0, "cmdoption-osxphotos-repl-not-shared"],
-            [0, "cmdoption-osxphotos-repl-not-slow-mo"],
-            [0, "cmdoption-osxphotos-repl-not-syndicated"],
-            [0, "cmdoption-osxphotos-repl-not-time-lapse"],
-            [0, "cmdoption-osxphotos-repl-only-movies"],
-            [0, "cmdoption-osxphotos-repl-only-photos"],
-            [0, "cmdoption-osxphotos-repl-panorama"],
-            [0, "cmdoption-osxphotos-repl-person"],
-            [0, "cmdoption-osxphotos-repl-place"],
-            [0, "cmdoption-osxphotos-repl-portrait"],
-            [0, "cmdoption-osxphotos-repl-query-eval"],
-            [0, "cmdoption-osxphotos-repl-query-function"],
-            [0, "cmdoption-osxphotos-repl-regex"],
-            [0, "cmdoption-osxphotos-repl-saved-to-library"],
-            [0, "cmdoption-osxphotos-repl-screenshot"],
-            [0, "cmdoption-osxphotos-repl-selected"],
-            [0, "cmdoption-osxphotos-repl-selfie"],
-            [0, "cmdoption-osxphotos-repl-shared"],
-            [0, "cmdoption-osxphotos-repl-slow-mo"],
-            [0, "cmdoption-osxphotos-repl-syndicated"],
-            [0, "cmdoption-osxphotos-repl-time-lapse"],
-            [0, "cmdoption-osxphotos-repl-title"],
-            [0, "cmdoption-osxphotos-repl-to-date"],
-            [0, "cmdoption-osxphotos-repl-to-time"],
-            [0, "cmdoption-osxphotos-repl-uti"],
-            [0, "cmdoption-osxphotos-repl-uuid"],
-            [0, "cmdoption-osxphotos-repl-uuid-from-file"],
-            [0, "cmdoption-osxphotos-repl-year"]
-        ],
-        "osxphotos-run command line option": [
-            [0, "cmdoption-osxphotos-run-arg-ARGS"],
-            [0, "cmdoption-osxphotos-run-arg-PYTHON_FILE"],
-            [0, "cmdoption-osxphotos-run-h"]
-        ],
-        "osxphotos-show command line option": [
-            [0, "cmdoption-osxphotos-show-arg-UUID_OR_NAME"],
-            [0, "cmdoption-osxphotos-show-library"]
-        ],
-        "osxphotos-snap command line option": [
-            [0, "cmdoption-osxphotos-snap-library"]
-        ],
-        "osxphotos-sync command line option": [
-            [0, "cmdoption-osxphotos-sync-0"],
-            [0, "cmdoption-osxphotos-sync-A"],
-            [0, "cmdoption-osxphotos-sync-R"],
-            [0, "cmdoption-osxphotos-sync-U"],
-            [0, "cmdoption-osxphotos-sync-V"],
-            [0, "cmdoption-osxphotos-sync-added-after"],
-            [0, "cmdoption-osxphotos-sync-added-before"],
-            [0, "cmdoption-osxphotos-sync-added-in-last"],
-            [0, "cmdoption-osxphotos-sync-album"],
-            [0, "cmdoption-osxphotos-sync-burst"],
-            [0, "cmdoption-osxphotos-sync-cloudasset"],
-            [0, "cmdoption-osxphotos-sync-description"],
-            [0, "cmdoption-osxphotos-sync-dry-run"],
-            [0, "cmdoption-osxphotos-sync-duplicate"],
-            [0, "cmdoption-osxphotos-sync-e"],
-            [0, "cmdoption-osxphotos-sync-edited"],
-            [0, "cmdoption-osxphotos-sync-exif"],
-            [0, "cmdoption-osxphotos-sync-external-edit"],
-            [0, "cmdoption-osxphotos-sync-favorite"],
-            [0, "cmdoption-osxphotos-sync-folder"],
-            [0, "cmdoption-osxphotos-sync-from-date"],
-            [0, "cmdoption-osxphotos-sync-from-time"],
-            [0, "cmdoption-osxphotos-sync-has-comment"],
-            [0, "cmdoption-osxphotos-sync-has-likes"],
-            [0, "cmdoption-osxphotos-sync-has-raw"],
-            [0, "cmdoption-osxphotos-sync-hdr"],
-            [0, "cmdoption-osxphotos-sync-hidden"],
-            [0, "cmdoption-osxphotos-sync-i"],
-            [0, "cmdoption-osxphotos-sync-in-album"],
-            [0, "cmdoption-osxphotos-sync-incloud"],
-            [0, "cmdoption-osxphotos-sync-is-reference"],
-            [0, "cmdoption-osxphotos-sync-keyword"],
-            [0, "cmdoption-osxphotos-sync-label"],
-            [0, "cmdoption-osxphotos-sync-library"],
-            [0, "cmdoption-osxphotos-sync-live"],
-            [0, "cmdoption-osxphotos-sync-location"],
-            [0, "cmdoption-osxphotos-sync-m"],
-            [0, "cmdoption-osxphotos-sync-max-size"],
-            [0, "cmdoption-osxphotos-sync-min-size"],
-            [0, "cmdoption-osxphotos-sync-missing"],
-            [0, "cmdoption-osxphotos-sync-name"],
-            [0, "cmdoption-osxphotos-sync-no-comment"],
-            [0, "cmdoption-osxphotos-sync-no-description"],
-            [0, "cmdoption-osxphotos-sync-no-keyword"],
-            [0, "cmdoption-osxphotos-sync-no-likes"],
-            [0, "cmdoption-osxphotos-sync-no-location"],
-            [0, "cmdoption-osxphotos-sync-no-place"],
-            [0, "cmdoption-osxphotos-sync-no-title"],
-            [0, "cmdoption-osxphotos-sync-not-burst"],
-            [0, "cmdoption-osxphotos-sync-not-cloudasset"],
-            [0, "cmdoption-osxphotos-sync-not-edited"],
-            [0, "cmdoption-osxphotos-sync-not-favorite"],
-            [0, "cmdoption-osxphotos-sync-not-hdr"],
-            [0, "cmdoption-osxphotos-sync-not-hidden"],
-            [0, "cmdoption-osxphotos-sync-not-in-album"],
-            [0, "cmdoption-osxphotos-sync-not-incloud"],
-            [0, "cmdoption-osxphotos-sync-not-live"],
-            [0, "cmdoption-osxphotos-sync-not-missing"],
-            [0, "cmdoption-osxphotos-sync-not-panorama"],
-            [0, "cmdoption-osxphotos-sync-not-portrait"],
-            [0, "cmdoption-osxphotos-sync-not-reference"],
-            [0, "cmdoption-osxphotos-sync-not-saved-to-library"],
-            [0, "cmdoption-osxphotos-sync-not-screenshot"],
-            [0, "cmdoption-osxphotos-sync-not-selfie"],
-            [0, "cmdoption-osxphotos-sync-not-slow-mo"],
-            [0, "cmdoption-osxphotos-sync-not-syndicated"],
-            [0, "cmdoption-osxphotos-sync-not-time-lapse"],
-            [0, "cmdoption-osxphotos-sync-only-movies"],
-            [0, "cmdoption-osxphotos-sync-only-photos"],
-            [0, "cmdoption-osxphotos-sync-panorama"],
-            [0, "cmdoption-osxphotos-sync-person"],
-            [0, "cmdoption-osxphotos-sync-place"],
-            [0, "cmdoption-osxphotos-sync-portrait"],
-            [0, "cmdoption-osxphotos-sync-query-eval"],
-            [0, "cmdoption-osxphotos-sync-query-function"],
-            [0, "cmdoption-osxphotos-sync-regex"],
-            [0, "cmdoption-osxphotos-sync-s"],
-            [0, "cmdoption-osxphotos-sync-saved-to-library"],
-            [0, "cmdoption-osxphotos-sync-screenshot"],
-            [0, "cmdoption-osxphotos-sync-selected"],
-            [0, "cmdoption-osxphotos-sync-selfie"],
-            [0, "cmdoption-osxphotos-sync-slow-mo"],
-            [0, "cmdoption-osxphotos-sync-syndicated"],
-            [0, "cmdoption-osxphotos-sync-theme"],
-            [0, "cmdoption-osxphotos-sync-time-lapse"],
-            [0, "cmdoption-osxphotos-sync-timestamp"],
-            [0, "cmdoption-osxphotos-sync-title"],
-            [0, "cmdoption-osxphotos-sync-to-date"],
-            [0, "cmdoption-osxphotos-sync-to-time"],
-            [0, "cmdoption-osxphotos-sync-uti"],
-            [0, "cmdoption-osxphotos-sync-uuid"],
-            [0, "cmdoption-osxphotos-sync-uuid-from-file"],
-            [0, "cmdoption-osxphotos-sync-year"]
-        ],
-        "osxphotos-theme command line option": [
-            [0, "cmdoption-osxphotos-theme-clone"],
-            [0, "cmdoption-osxphotos-theme-config"],
-            [0, "cmdoption-osxphotos-theme-default"],
-            [0, "cmdoption-osxphotos-theme-delete"],
-            [0, "cmdoption-osxphotos-theme-edit"],
-            [0, "cmdoption-osxphotos-theme-list"],
-            [0, "cmdoption-osxphotos-theme-preview"]
-        ],
-        "osxphotos-timewarp command line option": [
-            [0, "cmdoption-osxphotos-timewarp-0"],
-            [0, "cmdoption-osxphotos-timewarp-1"],
-            [0, "cmdoption-osxphotos-timewarp-2"],
-            [0, "cmdoption-osxphotos-timewarp-D"],
-            [0, "cmdoption-osxphotos-timewarp-F"],
-            [0, "cmdoption-osxphotos-timewarp-L"],
-            [0, "cmdoption-osxphotos-timewarp-M"],
-            [0, "cmdoption-osxphotos-timewarp-P"],
-            [0, "cmdoption-osxphotos-timewarp-T"],
-            [0, "cmdoption-osxphotos-timewarp-V"],
-            [0, "cmdoption-osxphotos-timewarp-a"],
-            [0, "cmdoption-osxphotos-timewarp-c"],
-            [0, "cmdoption-osxphotos-timewarp-d"],
-            [0, "cmdoption-osxphotos-timewarp-date-added"],
-            [0, "cmdoption-osxphotos-timewarp-date-added-from-photo"],
-            [0, "cmdoption-osxphotos-timewarp-e"],
-            [0, "cmdoption-osxphotos-timewarp-force"],
-            [0, "cmdoption-osxphotos-timewarp-i"],
-            [0, "cmdoption-osxphotos-timewarp-p"],
-            [0, "cmdoption-osxphotos-timewarp-plain"],
-            [0, "cmdoption-osxphotos-timewarp-t"],
-            [0, "cmdoption-osxphotos-timewarp-theme"],
-            [0, "cmdoption-osxphotos-timewarp-timestamp"],
-            [0, "cmdoption-osxphotos-timewarp-z"]
-        ],
-        "osxphotos-tutorial command line option": [
-            [0, "cmdoption-osxphotos-tutorial-arg-WIDTH"]
-        ],
-        "osxphotos-uninstall command line option": [
-            [0, "cmdoption-osxphotos-uninstall-arg-PACKAGES"],
-            [0, "cmdoption-osxphotos-uninstall-y"]
-        ],
-        "osxphotos-uuid command line option": [
-            [0, "cmdoption-osxphotos-uuid-f"]
-        ],
-        "osxphotos-version command line option": [
-            [0, "cmdoption-osxphotos-version-run"]
-        ],
-        "albuminfo (class in osxphotos)": [
-            [4, "osxphotos.AlbumInfo"]
-        ],
-        "albumsortorder (class in osxphotos)": [
-            [4, "osxphotos.AlbumSortOrder"]
-        ],
-        "commentinfo (class in osxphotos)": [
-            [4, "osxphotos.CommentInfo"]
-        ],
-        "exifinfo (class in osxphotos)": [
-            [4, "osxphotos.ExifInfo"]
-        ],
-        "exiftool (class in osxphotos)": [
-            [4, "osxphotos.ExifTool"]
-        ],
-        "exportdb (class in osxphotos)": [
-            [4, "osxphotos.ExportDB"]
-        ],
-        "exportdbtemp (class in osxphotos)": [
-            [4, "osxphotos.ExportDBTemp"]
-        ],
-        "exportoptions (class in osxphotos)": [
-            [4, "osxphotos.ExportOptions"]
-        ],
-        "exportresults (class in osxphotos)": [
-            [4, "osxphotos.ExportResults"]
-        ],
-        "fileutil (class in osxphotos)": [
-            [4, "osxphotos.FileUtil"]
-        ],
-        "fileutilnoop (class in osxphotos)": [
-            [4, "osxphotos.FileUtilNoOp"]
-        ],
-        "folderinfo (class in osxphotos)": [
-            [4, "osxphotos.FolderInfo"]
-        ],
-        "importinfo (class in osxphotos)": [
-            [4, "osxphotos.ImportInfo"]
-        ],
-        "likeinfo (class in osxphotos)": [
-            [4, "osxphotos.LikeInfo"]
-        ],
-        "momentinfo (class in osxphotos)": [
-            [4, "osxphotos.MomentInfo"]
-        ],
-        "personinfo (class in osxphotos)": [
-            [4, "osxphotos.PersonInfo"]
-        ],
-        "photoexporter (class in osxphotos)": [
-            [4, "osxphotos.PhotoExporter"]
-        ],
-        "photoinfo (class in osxphotos)": [
-            [4, "osxphotos.PhotoInfo"]
-        ],
-        "phototemplate (class in osxphotos)": [
-            [4, "osxphotos.PhotoTemplate"]
-        ],
-        "photosalbum (class in osxphotos)": [
-            [4, "osxphotos.PhotosAlbum"]
-        ],
-        "photosalbumphotoscript (class in osxphotos)": [
-            [4, "osxphotos.PhotosAlbumPhotoScript"]
-        ],
-        "photosdb (class in osxphotos)": [
-            [4, "osxphotos.PhotosDB"]
-        ],
-        "placeinfo (class in osxphotos)": [
-            [4, "osxphotos.PlaceInfo"]
-        ],
-        "projectinfo (class in osxphotos)": [
-            [4, "osxphotos.ProjectInfo"]
-        ],
-        "queryoptions (class in osxphotos)": [
-            [4, "osxphotos.QueryOptions"]
-        ],
-        "scoreinfo (class in osxphotos)": [
-            [4, "osxphotos.ScoreInfo"]
-        ],
-        "searchinfo (class in osxphotos)": [
-            [4, "osxphotos.SearchInfo"]
-        ],
-        "activities (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.activities"]
-        ],
-        "added_after (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.added_after"]
-        ],
-        "added_before (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.added_before"]
-        ],
-        "added_in_last (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.added_in_last"]
-        ],
-        "addvalues() (osxphotos.exiftool method)": [
-            [4, "osxphotos.ExifTool.addvalues"]
-        ],
-        "adjustments (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.adjustments"]
-        ],
-        "album (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.album"]
-        ],
-        "album_info (osxphotos.folderinfo property)": [
-            [4, "osxphotos.FolderInfo.album_info"]
-        ],
-        "album_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.album_info"]
-        ],
-        "album_info (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.album_info"]
-        ],
-        "album_info_shared (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.album_info_shared"]
-        ],
-        "albums (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.albums"]
-        ],
-        "albums (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.albums"]
-        ],
-        "albums_as_dict (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.albums_as_dict"]
-        ],
-        "albums_shared (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.albums_shared"]
-        ],
-        "albums_shared_as_dict (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.albums_shared_as_dict"]
-        ],
-        "all (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.all"]
-        ],
-        "all_files() (osxphotos.exportresults method)": [
-            [4, "osxphotos.ExportResults.all_files"]
-        ],
-        "asdict() (osxphotos.albuminfo method)": [
-            [4, "osxphotos.AlbumInfo.asdict"]
-        ],
-        "asdict() (osxphotos.exiftool method)": [
-            [4, "osxphotos.ExifTool.asdict"]
-        ],
-        "asdict() (osxphotos.folderinfo method)": [
-            [4, "osxphotos.FolderInfo.asdict"]
-        ],
-        "asdict() (osxphotos.importinfo method)": [
-            [4, "osxphotos.ImportInfo.asdict"]
-        ],
-        "asdict() (osxphotos.momentinfo method)": [
-            [4, "osxphotos.MomentInfo.asdict"]
-        ],
-        "asdict() (osxphotos.personinfo method)": [
-            [4, "osxphotos.PersonInfo.asdict"]
-        ],
-        "asdict() (osxphotos.photoinfo method)": [
-            [4, "osxphotos.PhotoInfo.asdict"]
-        ],
-        "asdict() (osxphotos.scoreinfo method)": [
-            [4, "osxphotos.ScoreInfo.asdict"]
-        ],
-        "asdict() (osxphotos.searchinfo method)": [
-            [4, "osxphotos.SearchInfo.asdict"]
-        ],
-        "attributes (osxphotos.exportresults property)": [
-            [4, "osxphotos.ExportResults.attributes"]
-        ],
-        "bit_flags (osxphotos.exportoptions property)": [
-            [4, "osxphotos.ExportOptions.bit_flags"]
-        ],
-        "bodies_of_water (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.bodies_of_water"]
-        ],
-        "burst (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst"]
-        ],
-        "burst (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.burst"]
-        ],
-        "burst_album_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst_album_info"]
-        ],
-        "burst_albums (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst_albums"]
-        ],
-        "burst_default_pick (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst_default_pick"]
-        ],
-        "burst_key (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst_key"]
-        ],
-        "burst_photos (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst_photos"]
-        ],
-        "burst_photos (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.burst_photos"]
-        ],
-        "burst_selected (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.burst_selected"]
-        ],
-        "camera (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.camera"]
-        ],
-        "city (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.city"]
-        ],
-        "close() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.close"]
-        ],
-        "cloud_guid (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.cloud_guid"]
-        ],
-        "cloud_metadata (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.cloud_metadata"]
-        ],
-        "cloud_owner_hashed_id (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.cloud_owner_hashed_id"]
-        ],
-        "cloudasset (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.cloudasset"]
-        ],
-        "comments (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.comments"]
-        ],
-        "connection (osxphotos.exportdb property)": [
-            [4, "osxphotos.ExportDB.connection"]
-        ],
-        "convert_to_jpeg (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.convert_to_jpeg"]
-        ],
-        "convert_to_jpeg() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.convert_to_jpeg"]
-        ],
-        "copy() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.copy"]
-        ],
-        "country (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.country"]
-        ],
-        "create_file_record() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.create_file_record"]
-        ],
-        "create_or_get_file_record() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.create_or_get_file_record"]
-        ],
-        "date (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.date"]
-        ],
-        "date (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.date"]
-        ],
-        "date_added (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.date_added"]
-        ],
-        "date_modified (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.date_modified"]
-        ],
-        "date_trashed (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.date_trashed"]
-        ],
-        "datetime (osxphotos.exportresults property)": [
-            [4, "osxphotos.ExportResults.datetime"]
-        ],
-        "db_path (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.db_path"]
-        ],
-        "db_version (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.db_version"]
-        ],
-        "delete_data_for_filepath() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.delete_data_for_filepath"]
-        ],
-        "delete_data_for_uuid() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.delete_data_for_uuid"]
-        ],
-        "deleted (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.deleted"]
-        ],
-        "deleted_only (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.deleted_only"]
-        ],
-        "description (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.description"]
-        ],
-        "description (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.description"]
-        ],
-        "description_template (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.description_template"]
-        ],
-        "detected_text (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.detected_text"]
-        ],
-        "detected_text() (osxphotos.photoinfo method)": [
-            [4, "osxphotos.PhotoInfo.detected_text"]
-        ],
-        "download_missing (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.download_missing"]
-        ],
-        "dry_run (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.dry_run"]
-        ],
-        "duplicate (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.duplicate"]
-        ],
-        "duplicates (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.duplicates"]
-        ],
-        "edited (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.edited"]
-        ],
-        "edited (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.edited"]
-        ],
-        "end_date (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.end_date"]
-        ],
-        "execute() (osxphotos.photosdb method)": [
-            [4, "osxphotos.PhotosDB.execute"]
-        ],
-        "exif (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.exif"]
-        ],
-        "exif_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.exif_info"]
-        ],
-        "exiftool (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.exiftool"]
-        ],
-        "exiftool (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.exiftool"]
-        ],
-        "exiftool_flags (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.exiftool_flags"]
-        ],
-        "exiftool_json_sidecar() (osxphotos.photoexporter method)": [
-            [4, "osxphotos.PhotoExporter.exiftool_json_sidecar"]
-        ],
-        "expand_variables() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.expand_variables"]
-        ],
-        "expand_variables_to_str() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.expand_variables_to_str"]
-        ],
-        "export() (osxphotos.photoexporter method)": [
-            [4, "osxphotos.PhotoExporter.export"]
-        ],
-        "export() (osxphotos.photoinfo method)": [
-            [4, "osxphotos.PhotoInfo.export"]
-        ],
-        "export_as_hardlink (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.export_as_hardlink"]
-        ],
-        "export_db (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.export_db"]
-        ],
-        "export_dir (osxphotos.exportdb property)": [
-            [4, "osxphotos.ExportDB.export_dir"]
-        ],
-        "external_edit (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.external_edit"]
-        ],
-        "external_edit (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.external_edit"]
-        ],
-        "face_info (osxphotos.personinfo property)": [
-            [4, "osxphotos.PersonInfo.face_info"]
-        ],
-        "face_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.face_info"]
-        ],
-        "face_regions (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.face_regions"]
-        ],
-        "favorite (osxphotos.personinfo property)": [
-            [4, "osxphotos.PersonInfo.favorite"]
-        ],
-        "favorite (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.favorite"]
-        ],
-        "favorite (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.favorite"]
-        ],
-        "favorite_rating (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.favorite_rating"]
-        ],
-        "feature_less (osxphotos.personinfo property)": [
-            [4, "osxphotos.PersonInfo.feature_less"]
-        ],
-        "file_sig() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.file_sig"]
-        ],
-        "filename (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.filename"]
-        ],
-        "fileutil (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.fileutil"]
-        ],
-        "filter_predicate() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.filter_predicate"]
-        ],
-        "fingerprint (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.fingerprint"]
-        ],
-        "folder (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.folder"]
-        ],
-        "folder_info (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.folder_info"]
-        ],
-        "folder_list (osxphotos.albuminfo property)": [
-            [4, "osxphotos.AlbumInfo.folder_list"]
-        ],
-        "folder_list (osxphotos.projectinfo property)": [
-            [4, "osxphotos.ProjectInfo.folder_list"]
-        ],
-        "folder_names (osxphotos.albuminfo property)": [
-            [4, "osxphotos.AlbumInfo.folder_names"]
-        ],
-        "folder_names (osxphotos.projectinfo property)": [
-            [4, "osxphotos.ProjectInfo.folder_names"]
-        ],
-        "folders (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.folders"]
-        ],
-        "force_update (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.force_update"]
-        ],
-        "from_date (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.from_date"]
-        ],
-        "function (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.function"]
-        ],
-        "get_db_connection() (osxphotos.photosdb method)": [
-            [4, "osxphotos.PhotosDB.get_db_connection"]
-        ],
-        "get_export_results() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_export_results"]
-        ],
-        "get_exported_files() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_exported_files"]
-        ],
-        "get_field_values() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_field_values"]
-        ],
-        "get_file_record() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_file_record"]
-        ],
-        "get_files_for_uuid() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_files_for_uuid"]
-        ],
-        "get_filter_values() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_filter_values"]
-        ],
-        "get_format_values() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_format_values"]
-        ],
-        "get_media_type() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_media_type"]
-        ],
-        "get_photo() (osxphotos.photosdb method)": [
-            [4, "osxphotos.PhotosDB.get_photo"]
-        ],
-        "get_photo_bool_attribute() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_photo_bool_attribute"]
-        ],
-        "get_photo_video_type() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_photo_video_type"]
-        ],
-        "get_photoinfo_for_uuid() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_photoinfo_for_uuid"]
-        ],
-        "get_previous_uuids() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_previous_uuids"]
-        ],
-        "get_target_for_file() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_target_for_file"]
-        ],
-        "get_template_value() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_template_value"]
-        ],
-        "get_template_value_exiftool() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_template_value_exiftool"]
-        ],
-        "get_template_value_filter_function() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_template_value_filter_function"]
-        ],
-        "get_template_value_function() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_template_value_function"]
-        ],
-        "get_template_value_multi() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_template_value_multi"]
-        ],
-        "get_template_value_pathlib() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.get_template_value_pathlib"]
-        ],
-        "get_uuid_for_file() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.get_uuid_for_file"]
-        ],
-        "hardlink() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.hardlink"]
-        ],
-        "has_comment (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.has_comment"]
-        ],
-        "has_likes (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.has_likes"]
-        ],
-        "has_raw (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.has_raw"]
-        ],
-        "has_raw (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.has_raw"]
-        ],
-        "hasadjustments (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.hasadjustments"]
-        ],
-        "hdr (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.hdr"]
-        ],
-        "hdr (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.hdr"]
-        ],
-        "height (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.height"]
-        ],
-        "hexdigest (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.hexdigest"]
-        ],
-        "hidden (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.hidden"]
-        ],
-        "hidden (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.hidden"]
-        ],
-        "holidays (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.holidays"]
-        ],
-        "ignore_case (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.ignore_case"]
-        ],
-        "ignore_date_modified (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.ignore_date_modified"]
-        ],
-        "ignore_signature (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.ignore_signature"]
-        ],
-        "import_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.import_info"]
-        ],
-        "import_info (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.import_info"]
-        ],
-        "in_album (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.in_album"]
-        ],
-        "incloud (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.incloud"]
-        ],
-        "incloud (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.incloud"]
-        ],
-        "increment (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.increment"]
-        ],
-        "intrash (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.intrash"]
-        ],
-        "is_debug() (in module osxphotos)": [
-            [4, "osxphotos.is_debug"]
-        ],
-        "is_reference (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.is_reference"]
-        ],
-        "iscloudasset (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.iscloudasset"]
-        ],
-        "ismissing (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.ismissing"]
-        ],
-        "ismovie (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.ismovie"]
-        ],
-        "isphoto (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.isphoto"]
-        ],
-        "israw (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.israw"]
-        ],
-        "isreference (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.isreference"]
-        ],
-        "jpeg_ext (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.jpeg_ext"]
-        ],
-        "jpeg_quality (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.jpeg_quality"]
-        ],
-        "json() (osxphotos.exiftool method)": [
-            [4, "osxphotos.ExifTool.json"]
-        ],
-        "json() (osxphotos.personinfo method)": [
-            [4, "osxphotos.PersonInfo.json"]
-        ],
-        "json() (osxphotos.photoinfo method)": [
-            [4, "osxphotos.PhotoInfo.json"]
-        ],
-        "keyword (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.keyword"]
-        ],
-        "keyword_template (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.keyword_template"]
-        ],
-        "keywords (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.keywords"]
-        ],
-        "keywords (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.keywords"]
-        ],
-        "keywords_as_dict (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.keywords_as_dict"]
-        ],
-        "label (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.label"]
-        ],
-        "labels (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.labels"]
-        ],
-        "labels (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.labels"]
-        ],
-        "labels (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.labels"]
-        ],
-        "labels_as_dict (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.labels_as_dict"]
-        ],
-        "labels_normalized (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.labels_normalized"]
-        ],
-        "labels_normalized (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.labels_normalized"]
-        ],
-        "labels_normalized_as_dict (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.labels_normalized_as_dict"]
-        ],
-        "library_path (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.library_path"]
-        ],
-        "likes (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.likes"]
-        ],
-        "live (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.live"]
-        ],
-        "live_photo (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.live_photo"]
-        ],
-        "live_photo (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.live_photo"]
-        ],
-        "locality_names (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.locality_names"]
-        ],
-        "location (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.location"]
-        ],
-        "location (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.location"]
-        ],
-        "location (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.location"]
-        ],
-        "location (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.location"]
-        ],
-        "max_size (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.max_size"]
-        ],
-        "media_types (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.media_types"]
-        ],
-        "merge_exif_keywords (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.merge_exif_keywords"]
-        ],
-        "merge_exif_persons (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.merge_exif_persons"]
-        ],
-        "min_size (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.min_size"]
-        ],
-        "missing (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.missing"]
-        ],
-        "missing_bursts (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.missing_bursts"]
-        ],
-        "modification_date (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.modification_date"]
-        ],
-        "module": [
-            [4, "module-osxphotos"]
-        ],
-        "moment_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.moment_info"]
-        ],
-        "month (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.month"]
-        ],
-        "movies (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.movies"]
-        ],
-        "name (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.name"]
-        ],
-        "neighborhoods (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.neighborhoods"]
-        ],
-        "no_comment (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_comment"]
-        ],
-        "no_description (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_description"]
-        ],
-        "no_keyword (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_keyword"]
-        ],
-        "no_likes (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_likes"]
-        ],
-        "no_location (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_location"]
-        ],
-        "no_place (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_place"]
-        ],
-        "no_title (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.no_title"]
-        ],
-        "not_burst (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_burst"]
-        ],
-        "not_cloudasset (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_cloudasset"]
-        ],
-        "not_edited (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_edited"]
-        ],
-        "not_favorite (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_favorite"]
-        ],
-        "not_hdr (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_hdr"]
-        ],
-        "not_hidden (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_hidden"]
-        ],
-        "not_in_album (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_in_album"]
-        ],
-        "not_incloud (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_incloud"]
-        ],
-        "not_live (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_live"]
-        ],
-        "not_missing (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_missing"]
-        ],
-        "not_panorama (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_panorama"]
-        ],
-        "not_portrait (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_portrait"]
-        ],
-        "not_reference (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_reference"]
-        ],
-        "not_saved_to_library (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_saved_to_library"]
-        ],
-        "not_screenshot (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_screenshot"]
-        ],
-        "not_selfie (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_selfie"]
-        ],
-        "not_shared (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_shared"]
-        ],
-        "not_slow_mo (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_slow_mo"]
-        ],
-        "not_syndicated (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_syndicated"]
-        ],
-        "not_time_lapse (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.not_time_lapse"]
-        ],
-        "orientation (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.orientation"]
-        ],
-        "original_filename (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.original_filename"]
-        ],
-        "original_filesize (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.original_filesize"]
-        ],
-        "original_height (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.original_height"]
-        ],
-        "original_orientation (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.original_orientation"]
-        ],
-        "original_width (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.original_width"]
-        ],
-        "osxphotos": [
-            [4, "module-osxphotos"]
-        ],
-        "overwrite (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.overwrite"]
-        ],
-        "owner (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.owner"]
-        ],
-        "panorama (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.panorama"]
-        ],
-        "panorama (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.panorama"]
-        ],
-        "parent (osxphotos.albuminfo property)": [
-            [4, "osxphotos.AlbumInfo.parent"]
-        ],
-        "parent (osxphotos.folderinfo property)": [
-            [4, "osxphotos.FolderInfo.parent"]
-        ],
-        "path (osxphotos.exportdb property)": [
-            [4, "osxphotos.ExportDB.path"]
-        ],
-        "path (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.path"]
-        ],
-        "path_derivatives (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.path_derivatives"]
-        ],
-        "path_edited (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.path_edited"]
-        ],
-        "path_edited_live_photo (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.path_edited_live_photo"]
-        ],
-        "path_live_photo (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.path_live_photo"]
-        ],
-        "path_raw (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.path_raw"]
-        ],
-        "person (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.person"]
-        ],
-        "person_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.person_info"]
-        ],
-        "person_info (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.person_info"]
-        ],
-        "persons (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.persons"]
-        ],
-        "persons (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.persons"]
-        ],
-        "persons (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.persons"]
-        ],
-        "persons_as_dict (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.persons_as_dict"]
-        ],
-        "photo_index() (osxphotos.albuminfo method)": [
-            [4, "osxphotos.AlbumInfo.photo_index"]
-        ],
-        "photos (osxphotos.albuminfo property)": [
-            [4, "osxphotos.AlbumInfo.photos"]
-        ],
-        "photos (osxphotos.importinfo property)": [
-            [4, "osxphotos.ImportInfo.photos"]
-        ],
-        "photos (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.photos"]
-        ],
-        "photos (osxphotos.personinfo property)": [
-            [4, "osxphotos.PersonInfo.photos"]
-        ],
-        "photos (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.photos"]
-        ],
-        "photos() (osxphotos.photosdb method)": [
-            [4, "osxphotos.PhotosDB.photos"]
-        ],
-        "photos_by_uuid() (osxphotos.photosdb method)": [
-            [4, "osxphotos.PhotosDB.photos_by_uuid"]
-        ],
-        "photos_version (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.photos_version"]
-        ],
-        "pid (osxphotos.exiftool property)": [
-            [4, "osxphotos.ExifTool.pid"]
-        ],
-        "pk (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.pk"]
-        ],
-        "place (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.place"]
-        ],
-        "place (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.place"]
-        ],
-        "place_names (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.place_names"]
-        ],
-        "portrait (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.portrait"]
-        ],
-        "portrait (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.portrait"]
-        ],
-        "preview (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.preview"]
-        ],
-        "preview_suffix (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.preview_suffix"]
-        ],
-        "project_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.project_info"]
-        ],
-        "project_info (osxphotos.photosdb property)": [
-            [4, "osxphotos.PhotosDB.project_info"]
-        ],
-        "query() (osxphotos.photosdb method)": [
-            [4, "osxphotos.PhotosDB.query"]
-        ],
-        "query_eval (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.query_eval"]
-        ],
-        "raw_original (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.raw_original"]
-        ],
-        "raw_photo (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.raw_photo"]
-        ],
-        "regex (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.regex"]
-        ],
-        "rename() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.rename"]
-        ],
-        "render() (osxphotos.phototemplate method)": [
-            [4, "osxphotos.PhotoTemplate.render"]
-        ],
-        "render_options (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.render_options"]
-        ],
-        "render_template() (osxphotos.photoinfo method)": [
-            [4, "osxphotos.PhotoInfo.render_template"]
-        ],
-        "replace_keywords (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.replace_keywords"]
-        ],
-        "rich (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.rich"]
-        ],
-        "rmdir() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.rmdir"]
-        ],
-        "run_commands() (osxphotos.exiftool method)": [
-            [4, "osxphotos.ExifTool.run_commands"]
-        ],
-        "saved_to_library (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.saved_to_library"]
-        ],
-        "saved_to_library (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.saved_to_library"]
-        ],
-        "score (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.score"]
-        ],
-        "screenshot (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.screenshot"]
-        ],
-        "screenshot (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.screenshot"]
-        ],
-        "search_info (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.search_info"]
-        ],
-        "search_info_normalized (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.search_info_normalized"]
-        ],
-        "season (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.season"]
-        ],
-        "selected (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.selected"]
-        ],
-        "selfie (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.selfie"]
-        ],
-        "selfie (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.selfie"]
-        ],
-        "set_config() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.set_config"]
-        ],
-        "set_debug() (in module osxphotos)": [
-            [4, "osxphotos.set_debug"]
-        ],
-        "set_export_results() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.set_export_results"]
-        ],
-        "set_photoinfo_for_uuid() (osxphotos.exportdb method)": [
-            [4, "osxphotos.ExportDB.set_photoinfo_for_uuid"]
-        ],
-        "setvalue() (osxphotos.exiftool method)": [
-            [4, "osxphotos.ExifTool.setvalue"]
-        ],
-        "shared (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.shared"]
-        ],
-        "shared (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.shared"]
-        ],
-        "sidecar (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.sidecar"]
-        ],
-        "sidecar_drop_ext (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.sidecar_drop_ext"]
-        ],
-        "slow_mo (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.slow_mo"]
-        ],
-        "slow_mo (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.slow_mo"]
-        ],
-        "sort_order (osxphotos.albuminfo property)": [
-            [4, "osxphotos.AlbumInfo.sort_order"]
-        ],
-        "sort_order (osxphotos.personinfo property)": [
-            [4, "osxphotos.PersonInfo.sort_order"]
-        ],
-        "source (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.source"]
-        ],
-        "start_date (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.start_date"]
-        ],
-        "state (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.state"]
-        ],
-        "state_abbreviation (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.state_abbreviation"]
-        ],
-        "streets (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.streets"]
-        ],
-        "strip (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.strip"]
-        ],
-        "subfolders (osxphotos.folderinfo property)": [
-            [4, "osxphotos.FolderInfo.subfolders"]
-        ],
-        "subtitle (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.subtitle"]
-        ],
-        "syndicated (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.syndicated"]
-        ],
-        "syndicated (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.syndicated"]
-        ],
-        "tables() (osxphotos.photoinfo method)": [
-            [4, "osxphotos.PhotoInfo.tables"]
-        ],
-        "text_found (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.text_found"]
-        ],
-        "time_lapse (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.time_lapse"]
-        ],
-        "time_lapse (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.time_lapse"]
-        ],
-        "timeout (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.timeout"]
-        ],
-        "title (osxphotos.albuminfo property)": [
-            [4, "osxphotos.AlbumInfo.title"]
-        ],
-        "title (osxphotos.folderinfo property)": [
-            [4, "osxphotos.FolderInfo.title"]
-        ],
-        "title (osxphotos.importinfo property)": [
-            [4, "osxphotos.ImportInfo.title"]
-        ],
-        "title (osxphotos.momentinfo property)": [
-            [4, "osxphotos.MomentInfo.title"]
-        ],
-        "title (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.title"]
-        ],
-        "title (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.title"]
-        ],
-        "tmpdir (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.tmpdir"]
-        ],
-        "tmpdir() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.tmpdir"]
-        ],
-        "to_date (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.to_date"]
-        ],
-        "touch_file (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.touch_file"]
-        ],
-        "tzoffset (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.tzoffset"]
-        ],
-        "unlink() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.unlink"]
-        ],
-        "update (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.update"]
-        ],
-        "update_errors (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.update_errors"]
-        ],
-        "use_albums_as_keywords (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.use_albums_as_keywords"]
-        ],
-        "use_persons_as_keywords (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.use_persons_as_keywords"]
-        ],
-        "use_photokit (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.use_photokit"]
-        ],
-        "use_photos_export (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.use_photos_export"]
-        ],
-        "uti (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.uti"]
-        ],
-        "uti (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.uti"]
-        ],
-        "uti_edited (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.uti_edited"]
-        ],
-        "uti_original (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.uti_original"]
-        ],
-        "uti_raw (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.uti_raw"]
-        ],
-        "utime() (osxphotos.fileutilnoop class method)": [
-            [4, "osxphotos.FileUtilNoOp.utime"]
-        ],
-        "uuid (osxphotos.folderinfo property)": [
-            [4, "osxphotos.FolderInfo.uuid"]
-        ],
-        "uuid (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.uuid"]
-        ],
-        "uuid (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.uuid"]
-        ],
-        "venue_types (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.venue_types"]
-        ],
-        "venues (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.venues"]
-        ],
-        "verbose (osxphotos.exportoptions attribute)": [
-            [4, "osxphotos.ExportOptions.verbose"]
-        ],
-        "version (osxphotos.exiftool property)": [
-            [4, "osxphotos.ExifTool.version"]
-        ],
-        "visible (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.visible"]
-        ],
-        "width (osxphotos.photoinfo property)": [
-            [4, "osxphotos.PhotoInfo.width"]
-        ],
-        "write_exiftool_metadata_to_file() (osxphotos.photoexporter method)": [
-            [4, "osxphotos.PhotoExporter.write_exiftool_metadata_to_file"]
-        ],
-        "year (osxphotos.queryoptions attribute)": [
-            [4, "osxphotos.QueryOptions.year"]
-        ],
-        "year (osxphotos.searchinfo property)": [
-            [4, "osxphotos.SearchInfo.year"]
-        ]
-    }
+    "indexentries": {}
 })
```

#### docs/template_help.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Package Overview" href="package_overview.html" /><link rel="prev" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Template System - osxphotos 0.60.3 documentation</title>
+        <title>OSXPhotos Template System - osxphotos 0.60.4 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -609,15 +609,15 @@
 <dt class="field-odd">A tab<span class="colon">:</span></dt>
 <dd class="field-odd"><p>‘t’</p>
 </dd>
 </dl>
 </td>
 </tr>
 <tr class="row-odd"><td><p>{osxphotos_version}</p></td>
-<td><p>The osxphotos version, e.g. ‘0.60.3’</p></td>
+<td><p>The osxphotos version, e.g. ‘0.60.4’</p></td>
 </tr>
 <tr class="row-even"><td><p>{osxphotos_cmd_line}</p></td>
 <td><p>The full command line used to run osxphotos</p></td>
 </tr>
 <tr class="row-odd"><td><p>{album}</p></td>
 <td><p>Album(s) photo is contained in</p></td>
 </tr>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -428,15 +428,15 @@
 {closebracket}                 A close bracket: â]â
 {newline}                      A newline: ânâ
 {lf}                           A line feed: ânâ, alias for {newline}
 {cr}                           A carriage return: ârâ
 {crlf}                         A carriage return + line feed: ârnâ
 {tab}                            A tab:
                                      âtâ
-{osxphotos_version}            The osxphotos version, e.g. â0.60.3â
+{osxphotos_version}            The osxphotos version, e.g. â0.60.4â
 {osxphotos_cmd_line}           The full command line used to run osxphotos
 {album}                        Album(s) photo is contained in
 {folder_album}                 Folder path + album photo is contained in. e.g. âFolder/Subfolder/Albumâ or just âAlbumâ if
                                no enclosing folder
 {project}                      Project(s) photo is contained in (such as greeting cards, calendars, slideshows)
 {album_project}                Album(s) and project(s) photo is contained in; treats projects as regular albums
 {folder_album_project}         Folder path + album (includes projects as albums) photo is contained in. e.g. âFolder/Subfolder/
```

#### docs/tutorial.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" /><link rel="prev" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Tutorial - osxphotos 0.60.3 documentation</title>
+        <title>OSXPhotos Tutorial - osxphotos 0.60.4 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.3 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.4 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.3 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.4 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.3_documentation
+osxphotos_0.60.4_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

### Comparing `osxphotos-0.60.3/osxphotos/exif_datetime_updater.py` & `osxphotos-0.60.4/osxphotos/exif_datetime_updater.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/exifinfo.py` & `osxphotos-0.60.4/osxphotos/exifinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/exiftool.py` & `osxphotos-0.60.4/osxphotos/exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/exiftool_filetypes.json` & `osxphotos-0.60.4/osxphotos/exiftool_filetypes.json`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/export_db.py` & `osxphotos-0.60.4/osxphotos/export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/export_db_utils.py` & `osxphotos-0.60.4/osxphotos/export_db_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/fileutil.py` & `osxphotos-0.60.4/osxphotos/fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/frozen_photoinfo.py` & `osxphotos-0.60.4/osxphotos/frozen_photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/imageconverter.py` & `osxphotos-0.60.4/osxphotos/imageconverter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/momentinfo.py` & `osxphotos-0.60.4/osxphotos/momentinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/path_utils.py` & `osxphotos-0.60.4/osxphotos/path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/personinfo.py` & `osxphotos-0.60.4/osxphotos/personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photodates.py` & `osxphotos-0.60.4/osxphotos/photodates.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photoexporter.py` & `osxphotos-0.60.4/osxphotos/photoexporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photoinfo.py` & `osxphotos-0.60.4/osxphotos/photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photokit.py` & `osxphotos-0.60.4/osxphotos/photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photosalbum.py` & `osxphotos-0.60.4/osxphotos/photosalbum.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photoscript_utils.py` & `osxphotos-0.60.4/osxphotos/photoscript_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_comments.py` & `osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_exif.py` & `osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_faceinfo.py` & `osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_scoreinfo.py` & `osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_searchinfo.py` & `osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photosdb/_photosdb_process_syndicationinfo.py` & `osxphotos-0.60.4/osxphotos/photosdb/_photosdb_process_syndicationinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photosdb/photosdb.py` & `osxphotos-0.60.4/osxphotos/photosdb/photosdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/photosdb/photosdb_utils.py` & `osxphotos-0.60.4/osxphotos/photosdb/photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/phototables.py` & `osxphotos-0.60.4/osxphotos/phototables.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/phototemplate.cog.md` & `osxphotos-0.60.4/osxphotos/phototemplate.cog.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/phototemplate.md` & `osxphotos-0.60.4/osxphotos/phototemplate.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/phototemplate.py` & `osxphotos-0.60.4/osxphotos/phototemplate.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/phototemplate.tx` & `osxphotos-0.60.4/osxphotos/phototemplate.tx`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/phototz.py` & `osxphotos-0.60.4/osxphotos/phototz.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/placeinfo.py` & `osxphotos-0.60.4/osxphotos/placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/pyrepl.py` & `osxphotos-0.60.4/osxphotos/pyrepl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/queries/shared_owner.sql.mako` & `osxphotos-0.60.4/osxphotos/queries/shared_owner.sql.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/query_builder.py` & `osxphotos-0.60.4/osxphotos/query_builder.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/queryoptions.py` & `osxphotos-0.60.4/osxphotos/queryoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/scoreinfo.py` & `osxphotos-0.60.4/osxphotos/scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/searchinfo.py` & `osxphotos-0.60.4/osxphotos/searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/sqlgrep.py` & `osxphotos-0.60.4/osxphotos/sqlgrep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/sqlite_utils.py` & `osxphotos-0.60.4/osxphotos/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/sqlitekvstore.py` & `osxphotos-0.60.4/osxphotos/sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/template_counter.py` & `osxphotos-0.60.4/osxphotos/template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/templates/xmp_sidecar.mako` & `osxphotos-0.60.4/osxphotos/templates/xmp_sidecar.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/templates/xmp_sidecar_beta.mako` & `osxphotos-0.60.4/osxphotos/templates/xmp_sidecar_beta.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/text_detection.py` & `osxphotos-0.60.4/osxphotos/text_detection.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/timeutils.py` & `osxphotos-0.60.4/osxphotos/timeutils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/timezones.py` & `osxphotos-0.60.4/osxphotos/timezones.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/tutorial.md` & `osxphotos-0.60.4/osxphotos/tutorial.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/uti.py` & `osxphotos-0.60.4/osxphotos/uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos/utils.py` & `osxphotos-0.60.4/osxphotos/utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos.egg-info/PKG-INFO` & `osxphotos-0.60.4/osxphotos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.3
+Version: 0.60.4
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.3/osxphotos.egg-info/SOURCES.txt` & `osxphotos-0.60.4/osxphotos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/osxphotos.egg-info/requires.txt` & `osxphotos-0.60.4/osxphotos.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/setup.py` & `osxphotos-0.60.4/setup.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_10_12_6.py` & `osxphotos-0.60.4/tests/test_10_12_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_albums_folders_catalina_10_15_7.py` & `osxphotos-0.60.4/tests/test_albums_folders_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_albums_folders_high_sierra_10_13_6.py` & `osxphotos-0.60.4/tests/test_albums_folders_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_albums_folders_mojave_10_14_6.py` & `osxphotos-0.60.4/tests/test_albums_folders_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_bigsur_10_16_0_1.py` & `osxphotos-0.60.4/tests/test_bigsur_10_16_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_catalina_10_15_7.py` & `osxphotos-0.60.4/tests/test_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli.py` & `osxphotos-0.60.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_add_locations.py` & `osxphotos-0.60.4/tests/test_cli_add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_add_to_album.py` & `osxphotos-0.60.4/tests/test_cli_add_to_album.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_all_commands.py` & `osxphotos-0.60.4/tests/test_cli_all_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_batch_edit.py` & `osxphotos-0.60.4/tests/test_cli_batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_dump.py` & `osxphotos-0.60.4/tests/test_cli_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_exiftool.py` & `osxphotos-0.60.4/tests/test_cli_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_export_cloud.py` & `osxphotos-0.60.4/tests/test_cli_export_cloud.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_export_projects.py` & `osxphotos-0.60.4/tests/test_cli_export_projects.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_exportdb.py` & `osxphotos-0.60.4/tests/test_cli_exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_import.py` & `osxphotos-0.60.4/tests/test_cli_import.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_orphans.py` & `osxphotos-0.60.4/tests/test_cli_orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_param_types.py` & `osxphotos-0.60.4/tests/test_cli_param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_sync.py` & `osxphotos-0.60.4/tests/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_timewarp.py` & `osxphotos-0.60.4/tests/test_cli_timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_utils.py` & `osxphotos-0.60.4/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cli_verbose.py` & `osxphotos-0.60.4/tests/test_cli_verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_cloud_owner_catalina.py` & `osxphotos-0.60.4/tests/test_cloud_owner_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_comments.py` & `osxphotos-0.60.4/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_concurrent_export.py` & `osxphotos-0.60.4/tests/test_concurrent_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_configoptions.py` & `osxphotos-0.60.4/tests/test_configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_datetime_formatter.py` & `osxphotos-0.60.4/tests/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_datetime_utils.py` & `osxphotos-0.60.4/tests/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_debug.py` & `osxphotos-0.60.4/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_empty_library_4_0.py` & `osxphotos-0.60.4/tests/test_empty_library_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_exif_info.py` & `osxphotos-0.60.4/tests/test_exif_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_exiftool.py` & `osxphotos-0.60.4/tests/test_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_exiftool_caching.py` & `osxphotos-0.60.4/tests/test_exiftool_caching.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_export_catalina_10_15_7.py` & `osxphotos-0.60.4/tests/test_export_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_export_catalina_10_15_7_use_photos_export.py` & `osxphotos-0.60.4/tests/test_export_catalina_10_15_7_use_photos_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_export_convert_to_jpeg.py` & `osxphotos-0.60.4/tests/test_export_convert_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_export_db.py` & `osxphotos-0.60.4/tests/test_export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_export_mojave_10_14_6.py` & `osxphotos-0.60.4/tests/test_export_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_export_raw_catalina_10_15_1.py` & `osxphotos-0.60.4/tests/test_export_raw_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_exportresults.py` & `osxphotos-0.60.4/tests/test_exportresults.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_faceinfo.py` & `osxphotos-0.60.4/tests/test_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_fileutil.py` & `osxphotos-0.60.4/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_highsierra.py` & `osxphotos-0.60.4/tests/test_highsierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_image_converter.py` & `osxphotos-0.60.4/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_incloud_big_sur_10_16_0.py` & `osxphotos-0.60.4/tests/test_incloud_big_sur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_incloud_catalina_10_15_1.py` & `osxphotos-0.60.4/tests/test_incloud_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_incloud_catalina_10_15_6.py` & `osxphotos-0.60.4/tests/test_incloud_catalina_10_15_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_incloud_mojave_10_14_6.py` & `osxphotos-0.60.4/tests/test_incloud_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_live_catalina_10_15_1.py` & `osxphotos-0.60.4/tests/test_live_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_modified_date_catalina_10_15_7.py` & `osxphotos-0.60.4/tests/test_modified_date_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_modified_date_mojave_10_14_6.py` & `osxphotos-0.60.4/tests/test_modified_date_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_mojave_10_14_6.py` & `osxphotos-0.60.4/tests/test_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_mojave_10_14_6_path_edited.py` & `osxphotos-0.60.4/tests/test_mojave_10_14_6_path_edited.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_monterey_12_0_1.py` & `osxphotos-0.60.4/tests/test_monterey_12_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_monterey_dev_beta_12_0_0.py` & `osxphotos-0.60.4/tests/test_monterey_dev_beta_12_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_movies_4_0.py` & `osxphotos-0.60.4/tests/test_movies_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_movies_5_0.py` & `osxphotos-0.60.4/tests/test_movies_5_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_path_utils.py` & `osxphotos-0.60.4/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_personinfo.py` & `osxphotos-0.60.4/tests/test_personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_photokit.py` & `osxphotos-0.60.4/tests/test_photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_photosdb_utils.py` & `osxphotos-0.60.4/tests/test_photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_placeinfo.py` & `osxphotos-0.60.4/tests/test_placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_places_catalina_10_15_1.py` & `osxphotos-0.60.4/tests/test_places_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_places_high_sierra_10_13_6.py` & `osxphotos-0.60.4/tests/test_places_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_places_mojave_10_14_6.py` & `osxphotos-0.60.4/tests/test_places_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_projects_catalina.py` & `osxphotos-0.60.4/tests/test_projects_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_projects_sierra.py` & `osxphotos-0.60.4/tests/test_projects_sierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_score_info.py` & `osxphotos-0.60.4/tests/test_score_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_search_info_10_14_6.py` & `osxphotos-0.60.4/tests/test_search_info_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_search_info_10_15_4.py` & `osxphotos-0.60.4/tests/test_search_info_10_15_4.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_search_info_10_15_5.py` & `osxphotos-0.60.4/tests/test_search_info_10_15_5.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_search_info_10_15_7.py` & `osxphotos-0.60.4/tests/test_search_info_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_shared_catalina_10_15_1.py` & `osxphotos-0.60.4/tests/test_shared_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_shared_mojave_10_14_6.py` & `osxphotos-0.60.4/tests/test_shared_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_sidecar_xmp.py` & `osxphotos-0.60.4/tests/test_sidecar_xmp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_specials_bigsur_10_16_0.py` & `osxphotos-0.60.4/tests/test_specials_bigsur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_specials_catalina_10_15_1.py` & `osxphotos-0.60.4/tests/test_specials_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_specials_mojave_10_14_6.py` & `osxphotos-0.60.4/tests/test_specials_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_specials_sierra_10_12.py` & `osxphotos-0.60.4/tests/test_specials_sierra_10_12.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_sqlitekvstore.py` & `osxphotos-0.60.4/tests/test_sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_template.py` & `osxphotos-0.60.4/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_template_counter.py` & `osxphotos-0.60.4/tests/test_template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_template_today.py` & `osxphotos-0.60.4/tests/test_template_today.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_uti.py` & `osxphotos-0.60.4/tests/test_uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_utils.py` & `osxphotos-0.60.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_ventura_13_0_0.py` & `osxphotos-0.60.4/tests/test_ventura_13_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.3/tests/test_ventura_dev_preview_13_0_0.py` & `osxphotos-0.60.4/tests/test_ventura_dev_preview_13_0_0.py`

 * *Files identical despite different names*

