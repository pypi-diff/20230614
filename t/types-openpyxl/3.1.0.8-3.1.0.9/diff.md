# Comparing `tmp/types-openpyxl-3.1.0.8.tar.gz` & `tmp/types-openpyxl-3.1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-openpyxl-3.1.0.8.tar", last modified: Mon May 15 12:30:39 2023, max compression
+gzip compressed data, was "types-openpyxl-3.1.0.9.tar", last modified: Mon Jun 12 15:15:14 2023, max compression
```

## Comparing `types-openpyxl-3.1.0.8.tar` & `types-openpyxl-3.1.0.9.tar`

### file list

```diff
@@ -1,221 +1,221 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.743408 types-openpyxl-3.1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-05-15 12:30:37.000000 types-openpyxl-3.1.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-15 12:30:37.000000 types-openpyxl-3.1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-15 12:30:39.743408 types-openpyxl-3.1.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.723408 types-openpyxl-3.1.0.8/openpyxl-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-15 12:30:37.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/_constants.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.723408 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/cell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/read_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/rich_text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/cell/text.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.727408 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/_3d.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/area_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/axis.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/bar_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/bubble_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/chartspace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/data_source.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/descriptors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/error_bar.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/label.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/layout.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/legend.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/line_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/marker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/pie_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/pivot.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/plotarea.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/print_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/radar_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/reader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/reference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/scatter_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/series.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/series_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/shapes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/stock_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/surface_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/title.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/trendline.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chart/updown_bars.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.727408 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/chartsheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/publish.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/relation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/views.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.727408 types-openpyxl-3.1.0.8/openpyxl-stubs/comments/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/comments/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/comments/author.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/comments/comment_sheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/comments/comments.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/comments/shape_writer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.727408 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/abc.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/product.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/singleton.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/compat/strings.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.727408 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14763 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/namespace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/nested.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/sequence.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/serialisable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/slots.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.731408 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/colors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/connector.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/effect.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/fill.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    16347 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/geometry.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/graphic.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/image.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/line.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/relation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/spreadsheet_drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18462 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/xdr.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.731408 types-openpyxl-3.1.0.8/openpyxl-stubs/formatting/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/formatting/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/formatting/formatting.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/formatting/rule.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.731408 types-openpyxl-3.1.0.8/openpyxl-stubs/formula/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/formula/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/formula/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/formula/translate.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.731408 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/extended.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/interface.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/manifest.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/relationship.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.735408 types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25251 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/cache.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/fields.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/record.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    34798 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/table.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.735408 types-openpyxl-3.1.0.8/openpyxl-stubs/reader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/reader/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/reader/drawings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/reader/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/reader/strings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/reader/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.735408 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/alignment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/borders.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/builtins.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/cell_style.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/colors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/differential.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/fills.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/fonts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/named_styles.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/numbers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/styleable.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/stylesheet.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/styles/table.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.735408 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/bound_dictionary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/cell.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/dataframe.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/datetime.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/escape.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/formulas.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/indexed_list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/inference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/utils/units.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.739408 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/child.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/defined_name.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.739408 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/external_link/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/external_link/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/external_link/external.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/external_reference.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/function_group.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/smart_tags.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/views.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/web.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/workbook.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.739408 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_read_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_reader.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_write_only.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/cell_range.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/cell_watch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/controls.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/copier.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/custom.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/datavalidation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/dimensions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/drawing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/filters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/formula.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/header_footer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/hyperlink.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/merge.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/ole.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/page.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/pagebreak.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/picture.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/print_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/properties.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/protection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/related.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/scenario.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/smart_tag.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/table.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/views.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/worksheet.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.739408 types-openpyxl-3.1.0.8/openpyxl-stubs/writer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/writer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/writer/excel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/writer/theme.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.739408 types-openpyxl-3.1.0.8/openpyxl-stubs/xml/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/xml/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/xml/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-15 12:30:22.000000 types-openpyxl-3.1.0.8/openpyxl-stubs/xml/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 12:30:39.743408 types-openpyxl-3.1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-15 12:30:37.000000 types-openpyxl-3.1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 12:30:39.739408 types-openpyxl-3.1.0.8/types_openpyxl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-15 12:30:39.000000 types-openpyxl-3.1.0.8/types_openpyxl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-05-15 12:30:39.000000 types-openpyxl-3.1.0.8/types_openpyxl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 12:30:39.000000 types-openpyxl-3.1.0.8/types_openpyxl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-15 12:30:39.000000 types-openpyxl-3.1.0.8/types_openpyxl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.717801 types-openpyxl-3.1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-12 15:15:12.000000 types-openpyxl-3.1.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 15:15:12.000000 types-openpyxl-3.1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-12 15:15:14.717801 types-openpyxl-3.1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.685801 types-openpyxl-3.1.0.9/openpyxl-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-12 15:15:12.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/_constants.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.689801 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/read_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/rich_text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/cell/text.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.693801 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/_3d.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/area_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/axis.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/bar_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/bubble_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/chartspace.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/data_source.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/descriptors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/error_bar.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/label.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/layout.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/legend.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/line_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/marker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/pie_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/pivot.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/plotarea.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/print_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/radar_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/reader.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/reference.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/scatter_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/series.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/series_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/shapes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/stock_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/surface_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/title.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/trendline.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chart/updown_bars.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.697801 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/chartsheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/publish.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/relation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/views.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.697801 types-openpyxl-3.1.0.9/openpyxl-stubs/comments/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/comments/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/comments/author.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/comments/comment_sheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/comments/comments.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/comments/shape_writer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.697801 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/abc.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/product.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/singleton.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/compat/strings.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.701801 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/namespace.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/nested.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/sequence.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/serialisable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/slots.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.701801 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17565 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/connector.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/effect.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/fill.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    16347 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/geometry.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/graphic.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/line.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4660 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/relation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/spreadsheet_drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/xdr.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.701801 types-openpyxl-3.1.0.9/openpyxl-stubs/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/formatting/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/formatting/formatting.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/formatting/rule.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.701801 types-openpyxl-3.1.0.9/openpyxl-stubs/formula/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/formula/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/formula/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/formula/translate.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.701801 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/extended.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/interface.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/manifest.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/relationship.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.705801 types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25468 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/cache.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/fields.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/record.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    34798 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/table.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.705801 types-openpyxl-3.1.0.9/openpyxl-stubs/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/reader/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/reader/drawings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/reader/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/reader/strings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/reader/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.705801 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/alignment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/borders.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/builtins.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/cell_style.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/differential.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/fills.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/fonts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/named_styles.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/numbers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/styleable.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/stylesheet.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/styles/table.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.709801 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/bound_dictionary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/cell.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/dataframe.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/escape.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/formulas.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/indexed_list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/inference.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/utils/units.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.709801 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/child.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/defined_name.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.709801 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/external_link/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/external_link/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/external_link/external.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/external_reference.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/function_group.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/smart_tags.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/views.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/web.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/workbook.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.713801 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/_read_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/_reader.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/_write_only.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/_writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/cell_range.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/cell_watch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/controls.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/copier.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/custom.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/datavalidation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/dimensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/drawing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/filters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/formula.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/header_footer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/hyperlink.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/merge.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/ole.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/page.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/pagebreak.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/picture.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/print_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/properties.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/protection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/related.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/scenario.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/smart_tag.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/table.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/views.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/worksheet.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.713801 types-openpyxl-3.1.0.9/openpyxl-stubs/writer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/writer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/writer/excel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/writer/theme.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.713801 types-openpyxl-3.1.0.9/openpyxl-stubs/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/xml/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/xml/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-12 15:14:58.000000 types-openpyxl-3.1.0.9/openpyxl-stubs/xml/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 15:15:14.717801 types-openpyxl-3.1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-12 15:15:11.000000 types-openpyxl-3.1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 15:15:14.717801 types-openpyxl-3.1.0.9/types_openpyxl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-12 15:15:14.000000 types-openpyxl-3.1.0.9/types_openpyxl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7031 2023-06-12 15:15:14.000000 types-openpyxl-3.1.0.9/types_openpyxl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 15:15:14.000000 types-openpyxl-3.1.0.9/types_openpyxl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-12 15:15:14.000000 types-openpyxl-3.1.0.9/types_openpyxl.egg-info/top_level.txt
```

### Comparing `types-openpyxl-3.1.0.8/CHANGELOG.md` & `types-openpyxl-3.1.0.9/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 3.1.0.9 (2023-06-12)
+
+Complete openpyxl's nested descriptors (#10298)
+
 ## 3.1.0.8 (2023-05-15)
 
 openpyxl: Type MetaSerialisable dunders (#10170)
 
 Typed `Serialisable.__attrs__`, `Serialisable.__nested__`, `Serialisable.__elements__`, and `Serialisable.__namespaced__` ClassVars.
 
 ## 3.1.0.7 (2023-05-10)
```

### Comparing `types-openpyxl-3.1.0.8/PKG-INFO` & `types-openpyxl-3.1.0.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-openpyxl
-Version: 3.1.0.8
+Version: 3.1.0.9
 Summary: Typing stubs for openpyxl
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/openpyxl.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,13 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `openpyxl`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/openpyxl. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2d5dafadb75f122e0c2aeced09a5b72232373f40`.
+This package was generated from typeshed commit `8c582c4459cc3e7c67531cd90bfd6cef5b71c7d3`.
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/cell/cell.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/cell/cell.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/cell/read_only.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/cell/read_only.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/cell/rich_text.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/cell/rich_text.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/cell/text.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/external_link/external.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,93 +1,79 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
 from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
-from openpyxl.descriptors.base import Alias, Integer, NoneSet, Typed, _ConvertibleToInt
+from openpyxl.descriptors.base import Bool, Integer, NoneSet, String, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.nested import NestedText
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.styles.fonts import Font
+from openpyxl.packaging.relationship import Relationship
 
-_PhoneticPropertiesType: TypeAlias = Literal["halfwidthKatakana", "fullwidthKatakana", "Hiragana", "noConversion"]
-_PhoneticPropertiesAlignment: TypeAlias = Literal["noControl", "left", "center", "distributed"]
+_ExternalCellType: TypeAlias = Literal["b", "d", "n", "e", "s", "str", "inlineStr"]
 
-class PhoneticProperties(Serialisable):
-    tagname: str
-    fontId: Integer[Literal[False]]
-    type: NoneSet[_PhoneticPropertiesType]
-    alignment: NoneSet[_PhoneticPropertiesAlignment]
+class ExternalCell(Serialisable):
+    r: String[Literal[False]]
+    t: NoneSet[_ExternalCellType]
+    vm: Integer[Literal[True]]
+    v: NestedText[str, Literal[True]]
     def __init__(
-        self,
-        fontId: _ConvertibleToInt,
-        type: _PhoneticPropertiesType | Literal["none"] | None = None,
-        alignment: _PhoneticPropertiesAlignment | Literal["none"] | None = None,
+        self, r: str, t: _ExternalCellType | Literal["none"] | None = None, vm: _ConvertibleToInt | None = None, v: object = None
     ) -> None: ...
 
-_PhoneticProperties: TypeAlias = PhoneticProperties
+class ExternalRow(Serialisable):
+    r: Integer[Literal[False]]
+    cell: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, r: _ConvertibleToInt, cell: Incomplete | None = None) -> None: ...
+
+class ExternalSheetData(Serialisable):
+    sheetId: Integer[Literal[False]]
+    refreshError: Bool[Literal[True]]
+    row: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, sheetId: _ConvertibleToInt, refreshError: _ConvertibleToBool | None = None, row=()) -> None: ...
+
+class ExternalSheetDataSet(Serialisable):
+    sheetData: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, sheetData: Incomplete | None = None) -> None: ...
 
-class PhoneticText(Serialisable):
+class ExternalSheetNames(Serialisable):
+    sheetName: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, sheetName=()) -> None: ...
+
+class ExternalDefinedName(Serialisable):
     tagname: str
-    sb: Integer[Literal[False]]
-    eb: Integer[Literal[False]]
-    t: Incomplete
-    text: Alias
-    def __init__(self, sb: _ConvertibleToInt, eb: _ConvertibleToInt, t: Incomplete | None = None) -> None: ...
+    name: String[Literal[False]]
+    refersTo: String[Literal[True]]
+    sheetId: Integer[Literal[True]]
+    def __init__(self, name: str, refersTo: str | None = None, sheetId: _ConvertibleToInt | None = None) -> None: ...
 
-class InlineFont(Font):
+class ExternalBook(Serialisable):
     tagname: str
-    rFont: Incomplete
-    charset: Incomplete
-    family: Incomplete
-    b: Incomplete
-    i: Incomplete
-    strike: Incomplete
-    outline: Incomplete
-    shadow: Incomplete
-    condense: Incomplete
-    extend: Incomplete
-    color: Incomplete
-    sz: Incomplete
-    u: Incomplete
-    vertAlign: Incomplete
-    scheme: Incomplete
+    sheetNames: Typed[ExternalSheetNames, Literal[True]]
+    definedNames: Incomplete
+    sheetDataSet: Typed[ExternalSheetDataSet, Literal[True]]
+    id: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        rFont: Incomplete | None = None,
-        charset: Incomplete | None = None,
-        family: Incomplete | None = None,
-        b: Incomplete | None = None,
-        i: Incomplete | None = None,
-        strike: Incomplete | None = None,
-        outline: Incomplete | None = None,
-        shadow: Incomplete | None = None,
-        condense: Incomplete | None = None,
-        extend: Incomplete | None = None,
-        color: Incomplete | None = None,
-        sz: Incomplete | None = None,
-        u: Incomplete | None = None,
-        vertAlign: Incomplete | None = None,
-        scheme: Incomplete | None = None,
+        sheetNames: ExternalSheetNames | None = None,
+        definedNames=(),
+        sheetDataSet: ExternalSheetDataSet | None = None,
+        id: Incomplete | None = None,
     ) -> None: ...
 
-class RichText(Serialisable):
-    tagname: str
-    rPr: Typed[InlineFont, Literal[True]]
-    font: Alias
-    t: Incomplete
-    text: Alias
-    __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, rPr: InlineFont | None = None, t: Incomplete | None = None) -> None: ...
-
-class Text(Serialisable):
+class ExternalLink(Serialisable):
     tagname: str
-    t: Incomplete
-    plain: Alias
-    r: Incomplete
-    formatted: Alias
-    rPh: Incomplete
-    phonetic: Alias
-    phoneticPr: Typed[_PhoneticProperties, Literal[True]]
-    PhoneticProperties: Alias
+    mime_type: str
+    externalBook: Typed[ExternalBook, Literal[True]]
+    file_link: Typed[Relationship, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, t: Incomplete | None = None, r=(), rPh=(), phoneticPr: _PhoneticProperties | None = None) -> None: ...
+    def __init__(
+        self, externalBook: ExternalBook | None = None, ddeLink: Unused = None, oleLink: Unused = None, extLst: Unused = None
+    ) -> None: ...
+    def to_tree(self): ...
     @property
-    def content(self): ...
+    def path(self): ...
+
+def read_external_link(archive, book_path): ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/_3d.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/_3d.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-from _typeshed import Incomplete, Unused
+from _typeshed import Unused
 from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.picture import PictureOptions
 from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool, _ConvertibleToFloat, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.nested import NestedBool, NestedInteger, NestedMinMax, _HasTagAndGet
 from openpyxl.descriptors.serialisable import Serialisable
 
 class View3D(Serialisable):
     tagname: str
-    rotX: Incomplete
+    rotX: NestedMinMax[float, Literal[True]]
     x_rotation: Alias
-    hPercent: Incomplete
+    hPercent: NestedMinMax[float, Literal[True]]
     height_percent: Alias
-    rotY: Incomplete
+    rotY: NestedInteger[Literal[True]]
     y_rotation: Alias
-    depthPercent: Incomplete
-    rAngAx: Incomplete
+    depthPercent: NestedInteger[Literal[True]]
+    rAngAx: NestedBool[Literal[True]]
     right_angle_axes: Alias
-    perspective: Incomplete
+    perspective: NestedInteger[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        rotX: int = 15,
-        hPercent: Incomplete | None = None,
-        rotY: int = 20,
-        depthPercent: Incomplete | None = None,
-        rAngAx: bool = True,
-        perspective: Incomplete | None = None,
+        rotX: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = 15,
+        hPercent: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        rotY: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = 20,
+        depthPercent: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        rAngAx: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = True,
+        perspective: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class Surface(Serialisable):
     tagname: str
-    thickness: Incomplete
+    thickness: NestedInteger[Literal[True]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     pictureOptions: Typed[PictureOptions, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        thickness: Incomplete | None = None,
+        thickness: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
         spPr: GraphicalProperties | None = None,
         pictureOptions: PictureOptions | None = None,
         extLst: Unused = None,
     ) -> None: ...
 
 class _3DBase(Serialisable):
     tagname: str
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/__init__.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/_chart.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/_chart.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/area_chart.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/area_chart.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from _typeshed import Incomplete, Unused
 from abc import abstractmethod
 from typing import ClassVar
-from typing_extensions import Literal
+from typing_extensions import Literal, TypeAlias
 
 from openpyxl.chart.axis import ChartLines, NumericAxis, SeriesAxis, TextAxis
 from openpyxl.chart.label import DataLabelList
-from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.nested import NestedBool, NestedSet, _HasTagAndGet
 
 from ._chart import ChartBase
 
+_AreaChartBaseGrouping: TypeAlias = Literal["percentStacked", "standard", "stacked"]
+
 class _AreaChartBase(ChartBase):
-    grouping: Incomplete
-    varyColors: Incomplete
+    grouping: NestedSet[_AreaChartBaseGrouping]
+    varyColors: NestedBool[Literal[True]]
     ser: Incomplete
     dLbls: Typed[DataLabelList, Literal[True]]
     dataLabels: Alias
     dropLines: Typed[ChartLines, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        grouping: str = "standard",
-        varyColors: Incomplete | None = None,
+        grouping: _HasTagAndGet[_AreaChartBaseGrouping] | _AreaChartBaseGrouping = "standard",
+        varyColors: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         ser=(),
         dLbls: DataLabelList | None = None,
         dropLines: ChartLines | None = None,
     ) -> None: ...
     @property
     @abstractmethod
     def tagname(self) -> str: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/bubble_chart.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/differential.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,43 @@
-from _typeshed import Incomplete, Unused
+from _typeshed import Incomplete
 from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.chart.axis import NumericAxis
-from openpyxl.chart.label import DataLabelList
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.styles import Alignment, Border, Fill, Font, Protection
+from openpyxl.styles.numbers import NumberFormat
 
-from ._chart import ChartBase
-
-class BubbleChart(ChartBase):
+class DifferentialStyle(Serialisable):
     tagname: str
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Typed[DataLabelList, Literal[True]]
-    dataLabels: Alias
-    bubble3D: Incomplete
-    bubbleScale: Incomplete
-    showNegBubbles: Incomplete
-    sizeRepresents: Incomplete
-    extLst: Typed[ExtensionList, Literal[True]]
-    x_axis: Typed[NumericAxis, Literal[False]]
-    y_axis: Typed[NumericAxis, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
+    font: Typed[Font, Literal[True]]
+    numFmt: Typed[NumberFormat, Literal[True]]
+    fill: Typed[Fill, Literal[True]]
+    alignment: Typed[Alignment, Literal[True]]
+    border: Typed[Border, Literal[True]]
+    protection: Typed[Protection, Literal[True]]
+    extLst: ExtensionList | None
     def __init__(
         self,
-        varyColors: Incomplete | None = None,
-        ser=(),
-        dLbls: DataLabelList | None = None,
-        bubble3D: Incomplete | None = None,
-        bubbleScale: Incomplete | None = None,
-        showNegBubbles: Incomplete | None = None,
-        sizeRepresents: Incomplete | None = None,
-        extLst: Unused = None,
-        **kw,
+        font: Font | None = None,
+        numFmt: NumberFormat | None = None,
+        fill: Fill | None = None,
+        alignment: Alignment | None = None,
+        border: Border | None = None,
+        protection: Protection | None = None,
+        extLst: ExtensionList | None = None,
     ) -> None: ...
+
+class DifferentialStyleList(Serialisable):
+    tagname: str
+    dxf: Incomplete
+    styles: Alias
+    __attrs__: ClassVar[tuple[str, ...]]
+    def __init__(self, dxf=(), count: Incomplete | None = None) -> None: ...
+    def append(self, dxf) -> None: ...
+    def add(self, dxf): ...
+    def __bool__(self) -> bool: ...
+    def __getitem__(self, idx): ...
+    @property
+    def count(self): ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/descriptors.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/descriptors.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from _typeshed import Incomplete
 from typing_extensions import Literal
 
 from openpyxl.chart.data_source import NumFmt
 from openpyxl.descriptors import Strict, Typed
 from openpyxl.descriptors.nested import NestedMinMax
 from openpyxl.descriptors.serialisable import Serialisable
 
-class NestedGapAmount(NestedMinMax):
+class NestedGapAmount(NestedMinMax[float, bool]):
     allow_none: bool
     min: float
     max: float
 
-class NestedOverlap(NestedMinMax):
+class NestedOverlap(NestedMinMax[float, bool]):
     allow_none: bool
     min: float
     max: float
 
-class NumberFormatDescriptor(Typed[NumFmt, Incomplete]):
+class NumberFormatDescriptor(Typed[NumFmt, Literal[True]]):
     expected_type: type[NumFmt]
     allow_none: Literal[True]
     def __set__(self, instance: Serialisable | Strict, value) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/error_bar.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/plotarea.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,74 @@
 from _typeshed import Incomplete, Unused
 from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.chart.data_source import NumDataSource
+from openpyxl.chart.layout import Layout
 from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.chart.text import RichText
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.nested import NestedBool, _HasTagAndGet
 from openpyxl.descriptors.serialisable import Serialisable
 
-class ErrorBars(Serialisable):
+class DataTable(Serialisable):
     tagname: str
-    errDir: Incomplete
-    direction: Alias
-    errBarType: Incomplete
-    style: Alias
-    errValType: Incomplete
-    size: Alias
-    noEndCap: Incomplete
-    plus: Typed[NumDataSource, Literal[True]]
-    minus: Typed[NumDataSource, Literal[True]]
-    val: Incomplete
+    showHorzBorder: NestedBool[Literal[True]]
+    showVertBorder: NestedBool[Literal[True]]
+    showOutline: NestedBool[Literal[True]]
+    showKeys: NestedBool[Literal[True]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
+    txPr: Typed[RichText, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        errDir: Incomplete | None = None,
-        errBarType: str = "both",
-        errValType: str = "fixedVal",
-        noEndCap: Incomplete | None = None,
-        plus: NumDataSource | None = None,
-        minus: NumDataSource | None = None,
-        val: Incomplete | None = None,
+        showHorzBorder: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        showVertBorder: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        showOutline: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        showKeys: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         spPr: GraphicalProperties | None = None,
+        txPr: RichText | None = None,
         extLst: Unused = None,
     ) -> None: ...
+
+class PlotArea(Serialisable):
+    tagname: str
+    layout: Typed[Layout, Literal[True]]
+    dTable: Typed[DataTable, Literal[True]]
+    spPr: Typed[GraphicalProperties, Literal[True]]
+    graphicalProperties: Alias
+    extLst: Typed[ExtensionList, Literal[True]]
+    areaChart: Incomplete
+    area3DChart: Incomplete
+    lineChart: Incomplete
+    line3DChart: Incomplete
+    stockChart: Incomplete
+    radarChart: Incomplete
+    scatterChart: Incomplete
+    pieChart: Incomplete
+    pie3DChart: Incomplete
+    doughnutChart: Incomplete
+    barChart: Incomplete
+    bar3DChart: Incomplete
+    ofPieChart: Incomplete
+    surfaceChart: Incomplete
+    surface3DChart: Incomplete
+    bubbleChart: Incomplete
+    valAx: Incomplete
+    catAx: Incomplete
+    dateAx: Incomplete
+    serAx: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(
+        self,
+        layout: Layout | None = None,
+        dTable: DataTable | None = None,
+        spPr: GraphicalProperties | None = None,
+        _charts=(),
+        _axes=(),
+        extLst: Unused = None,
+    ) -> None: ...
+    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None, namespace: Incomplete | None = None): ...
+    @classmethod
+    def from_tree(cls, node): ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/label.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/label.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,92 @@
 from _typeshed import Incomplete, Unused
 from abc import abstractmethod
 from typing import ClassVar
-from typing_extensions import Literal
+from typing_extensions import Literal, TypeAlias
 
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText
-from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.nested import NestedBool, NestedInteger, NestedNoneSet, NestedString, _HasTagAndGet, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable as Serialisable
 
+_DataLabelBaseDLblPos: TypeAlias = Literal["bestFit", "b", "ctr", "inBase", "inEnd", "l", "outEnd", "r", "t"]
+
 class _DataLabelBase(Serialisable):
-    numFmt: Incomplete
+    numFmt: NestedString[Literal[True]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     txPr: Typed[RichText, Literal[True]]
     textProperties: Alias
-    dLblPos: Incomplete
+    dLblPos: NestedNoneSet[_DataLabelBaseDLblPos]
     position: Alias
-    showLegendKey: Incomplete
-    showVal: Incomplete
-    showCatName: Incomplete
-    showSerName: Incomplete
-    showPercent: Incomplete
-    showBubbleSize: Incomplete
-    showLeaderLines: Incomplete
-    separator: Incomplete
+    showLegendKey: NestedBool[Literal[True]]
+    showVal: NestedBool[Literal[True]]
+    showCatName: NestedBool[Literal[True]]
+    showSerName: NestedBool[Literal[True]]
+    showPercent: NestedBool[Literal[True]]
+    showBubbleSize: NestedBool[Literal[True]]
+    showLeaderLines: NestedBool[Literal[True]]
+    separator: NestedString[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        numFmt: Incomplete | None = None,
+        numFmt: object = None,
         spPr: GraphicalProperties | None = None,
         txPr: RichText | None = None,
-        dLblPos: Incomplete | None = None,
-        showLegendKey: Incomplete | None = None,
-        showVal: Incomplete | None = None,
-        showCatName: Incomplete | None = None,
-        showSerName: Incomplete | None = None,
-        showPercent: Incomplete | None = None,
-        showBubbleSize: Incomplete | None = None,
-        showLeaderLines: Incomplete | None = None,
-        separator: Incomplete | None = None,
+        dLblPos: _NestedNoneSetParam[_DataLabelBaseDLblPos] = None,
+        showLegendKey: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        showVal: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        showCatName: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        showSerName: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        showPercent: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        showBubbleSize: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        showLeaderLines: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        separator: object = None,
         extLst: Unused = None,
     ) -> None: ...
     @property
     @abstractmethod
     def tagname(self) -> str: ...
 
 class DataLabel(_DataLabelBase):
     tagname: str
-    idx: Incomplete
+    idx: NestedInteger[Literal[False]]
     numFmt: Incomplete
     spPr: Incomplete
     txPr: Incomplete
     dLblPos: Incomplete
     showLegendKey: Incomplete
     showVal: Incomplete
     showCatName: Incomplete
     showSerName: Incomplete
     showPercent: Incomplete
     showBubbleSize: Incomplete
     showLeaderLines: Incomplete
     separator: Incomplete
     extLst: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, idx: int = 0, **kw) -> None: ...
+    def __init__(self, idx: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt = 0, **kw) -> None: ...
 
 class DataLabelList(_DataLabelBase):
     tagname: str
     dLbl: Incomplete
-    delete: Incomplete
+    delete: NestedBool[Literal[True]]
     numFmt: Incomplete
     spPr: Incomplete
     txPr: Incomplete
     dLblPos: Incomplete
     showLegendKey: Incomplete
     showVal: Incomplete
     showCatName: Incomplete
     showSerName: Incomplete
     showPercent: Incomplete
     showBubbleSize: Incomplete
     showLeaderLines: Incomplete
     separator: Incomplete
     extLst: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, dLbl=(), delete: Incomplete | None = None, **kw) -> None: ...
+    def __init__(
+        self, dLbl=(), delete: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None, **kw
+    ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/layout.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/stock_chart.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 from _typeshed import Incomplete, Unused
 from typing import ClassVar
 from typing_extensions import Literal
 
+from openpyxl.chart.axis import ChartLines, NumericAxis, TextAxis
+from openpyxl.chart.label import DataLabelList
+from openpyxl.chart.updown_bars import UpDownBars
 from openpyxl.descriptors.base import Alias, Typed
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.serialisable import Serialisable
 
-class ManualLayout(Serialisable):
+from ._chart import ChartBase
+
+class StockChart(ChartBase):
     tagname: str
-    layoutTarget: Incomplete
-    xMode: Incomplete
-    yMode: Incomplete
-    wMode: Incomplete
-    hMode: Incomplete
-    x: Incomplete
-    y: Incomplete
-    w: Incomplete
-    width: Alias
-    h: Incomplete
-    height: Alias
+    ser: Incomplete
+    dLbls: Typed[DataLabelList, Literal[True]]
+    dataLabels: Alias
+    dropLines: Typed[ChartLines, Literal[True]]
+    hiLowLines: Typed[ChartLines, Literal[True]]
+    upDownBars: Typed[UpDownBars, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
+    x_axis: Typed[TextAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        layoutTarget: Incomplete | None = None,
-        xMode: Incomplete | None = None,
-        yMode: Incomplete | None = None,
-        wMode: str = "factor",
-        hMode: str = "factor",
-        x: Incomplete | None = None,
-        y: Incomplete | None = None,
-        w: Incomplete | None = None,
-        h: Incomplete | None = None,
+        ser=(),
+        dLbls: DataLabelList | None = None,
+        dropLines: ChartLines | None = None,
+        hiLowLines: ChartLines | None = None,
+        upDownBars: UpDownBars | None = None,
         extLst: Unused = None,
+        **kw,
     ) -> None: ...
-
-class Layout(Serialisable):
-    tagname: str
-    manualLayout: Typed[ManualLayout, Literal[True]]
-    extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, manualLayout: ManualLayout | None = None, extLst: Unused = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/legend.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/cell/text.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,94 @@
-from _typeshed import Incomplete, Unused
+from _typeshed import Incomplete
 from typing import ClassVar
-from typing_extensions import Literal
+from typing_extensions import Literal, TypeAlias
 
-from openpyxl.chart.layout import Layout
-from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.chart.text import RichText
-from openpyxl.descriptors.base import Alias, Typed
-from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.base import Alias, Integer, NoneSet, Typed, _ConvertibleToInt
+from openpyxl.descriptors.nested import NestedString, NestedText
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.styles.fonts import Font
 
-class LegendEntry(Serialisable):
+_PhoneticPropertiesType: TypeAlias = Literal["halfwidthKatakana", "fullwidthKatakana", "Hiragana", "noConversion"]
+_PhoneticPropertiesAlignment: TypeAlias = Literal["noControl", "left", "center", "distributed"]
+
+class PhoneticProperties(Serialisable):
     tagname: str
-    idx: Incomplete
-    delete: Incomplete
-    txPr: Typed[RichText, Literal[True]]
-    extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, idx: int = 0, delete: bool = False, txPr: RichText | None = None, extLst: Unused = None) -> None: ...
+    fontId: Integer[Literal[False]]
+    type: NoneSet[_PhoneticPropertiesType]
+    alignment: NoneSet[_PhoneticPropertiesAlignment]
+    def __init__(
+        self,
+        fontId: _ConvertibleToInt,
+        type: _PhoneticPropertiesType | Literal["none"] | None = None,
+        alignment: _PhoneticPropertiesAlignment | Literal["none"] | None = None,
+    ) -> None: ...
+
+_PhoneticProperties: TypeAlias = PhoneticProperties
+
+class PhoneticText(Serialisable):
+    tagname: str
+    sb: Integer[Literal[False]]
+    eb: Integer[Literal[False]]
+    t: NestedText[str, Literal[False]]
+    text: Alias
+    def __init__(self, sb: _ConvertibleToInt, eb: _ConvertibleToInt, t: object = None) -> None: ...
 
-class Legend(Serialisable):
+class InlineFont(Font):
     tagname: str
-    legendPos: Incomplete
-    position: Alias
-    legendEntry: Incomplete
-    layout: Typed[Layout, Literal[True]]
-    overlay: Incomplete
-    spPr: Typed[GraphicalProperties, Literal[True]]
-    graphicalProperties: Alias
-    txPr: Typed[RichText, Literal[True]]
-    textProperties: Alias
-    extLst: Typed[ExtensionList, Literal[True]]
+    rFont: NestedString[Literal[True]]
+    charset: Incomplete
+    family: Incomplete
+    b: Incomplete
+    i: Incomplete
+    strike: Incomplete
+    outline: Incomplete
+    shadow: Incomplete
+    condense: Incomplete
+    extend: Incomplete
+    color: Incomplete
+    sz: Incomplete
+    u: Incomplete
+    vertAlign: Incomplete
+    scheme: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        legendPos: str = "r",
-        legendEntry=(),
-        layout: Layout | None = None,
-        overlay: Incomplete | None = None,
-        spPr: GraphicalProperties | None = None,
-        txPr: RichText | None = None,
-        extLst: Unused = None,
+        rFont: object = None,
+        charset: Incomplete | None = None,
+        family: Incomplete | None = None,
+        b: Incomplete | None = None,
+        i: Incomplete | None = None,
+        strike: Incomplete | None = None,
+        outline: Incomplete | None = None,
+        shadow: Incomplete | None = None,
+        condense: Incomplete | None = None,
+        extend: Incomplete | None = None,
+        color: Incomplete | None = None,
+        sz: Incomplete | None = None,
+        u: Incomplete | None = None,
+        vertAlign: Incomplete | None = None,
+        scheme: Incomplete | None = None,
     ) -> None: ...
+
+class RichText(Serialisable):
+    tagname: str
+    rPr: Typed[InlineFont, Literal[True]]
+    font: Alias
+    t: NestedText[str, Literal[True]]
+    text: Alias
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, rPr: InlineFont | None = None, t: object = None) -> None: ...
+
+class Text(Serialisable):
+    tagname: str
+    t: NestedText[str, Literal[True]]
+    plain: Alias
+    r: Incomplete
+    formatted: Alias
+    rPh: Incomplete
+    phonetic: Alias
+    phoneticPr: Typed[_PhoneticProperties, Literal[True]]
+    PhoneticProperties: Alias
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, t: object = None, r=(), rPh=(), phoneticPr: _PhoneticProperties | None = None) -> None: ...
+    @property
+    def content(self): ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/line_chart.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/bar_chart.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,85 +1,93 @@
 from _typeshed import Incomplete, Unused
 from abc import abstractmethod
 from typing import ClassVar
-from typing_extensions import Literal
+from typing_extensions import Literal, TypeAlias
 
-from openpyxl.chart.axis import ChartLines, NumericAxis, _BaseAxis
+from openpyxl.chart.axis import ChartLines, NumericAxis, SeriesAxis, TextAxis
 from openpyxl.chart.label import DataLabelList
-from openpyxl.chart.updown_bars import UpDownBars
-from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.nested import NestedBool, NestedNoneSet, NestedSet, _HasTagAndGet, _NestedNoneSetParam
 
+from ._3d import _3DBase
 from ._chart import ChartBase
 
-class _LineChartBase(ChartBase):
-    grouping: Incomplete
-    varyColors: Incomplete
+_BarChartBaseBarDir: TypeAlias = Literal["bar", "col"]
+_BarChartBaseGrouping: TypeAlias = Literal["percentStacked", "clustered", "standard", "stacked"]
+_BarChart3DShape: TypeAlias = Literal["cone", "coneToMax", "box", "cylinder", "pyramid", "pyramidToMax"]
+
+class _BarChartBase(ChartBase):
+    barDir: NestedSet[_BarChartBaseBarDir]
+    type: Alias
+    grouping: NestedSet[_BarChartBaseGrouping]
+    varyColors: NestedBool[Literal[True]]
     ser: Incomplete
     dLbls: Typed[DataLabelList, Literal[True]]
     dataLabels: Alias
-    dropLines: Typed[ChartLines, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        grouping: str = "standard",
-        varyColors: Incomplete | None = None,
+        barDir: _HasTagAndGet[_BarChartBaseBarDir] | _BarChartBaseBarDir = "col",
+        grouping: _HasTagAndGet[_BarChartBaseGrouping] | _BarChartBaseGrouping = "clustered",
+        varyColors: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         ser=(),
         dLbls: DataLabelList | None = None,
-        dropLines: ChartLines | None = None,
         **kw,
     ) -> None: ...
     @property
     @abstractmethod
     def tagname(self) -> str: ...
 
-class LineChart(_LineChartBase):
+class BarChart(_BarChartBase):
     tagname: str
+    barDir: Incomplete
     grouping: Incomplete
     varyColors: Incomplete
     ser: Incomplete
     dLbls: Incomplete
-    dropLines: Incomplete
-    hiLowLines: Typed[ChartLines, Literal[True]]
-    upDownBars: Typed[UpDownBars, Literal[True]]
-    marker: Incomplete
-    smooth: Incomplete
+    gapWidth: Incomplete
+    overlap: Incomplete
+    serLines: Typed[ChartLines, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    x_axis: Typed[_BaseAxis, Literal[False]]
+    x_axis: Typed[TextAxis, Literal[False]]
     y_axis: Typed[NumericAxis, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
+    legend: Incomplete
     def __init__(
         self,
-        hiLowLines: ChartLines | None = None,
-        upDownBars: UpDownBars | None = None,
-        marker: Incomplete | None = None,
-        smooth: Incomplete | None = None,
+        gapWidth: int = 150,
+        overlap: Incomplete | None = None,
+        serLines: ChartLines | None = None,
         extLst: Unused = None,
         **kw,
     ) -> None: ...
 
-class LineChart3D(_LineChartBase):
+class BarChart3D(_BarChartBase, _3DBase):
     tagname: str
+    barDir: Incomplete
     grouping: Incomplete
     varyColors: Incomplete
     ser: Incomplete
     dLbls: Incomplete
-    dropLines: Incomplete
+    view3D: Incomplete
+    floor: Incomplete
+    sideWall: Incomplete
+    backWall: Incomplete
+    gapWidth: Incomplete
     gapDepth: Incomplete
-    hiLowLines: Typed[ChartLines, Literal[True]]
-    upDownBars: Typed[UpDownBars, Literal[True]]
-    marker: Incomplete
-    smooth: Incomplete
+    shape: NestedNoneSet[_BarChart3DShape]
+    serLines: Typed[ChartLines, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    x_axis: Typed[ExtensionList, Literal[False]]
-    y_axis: Typed[ExtensionList, Literal[False]]
-    z_axis: Typed[ExtensionList, Literal[False]]
+    x_axis: Typed[TextAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
+    z_axis: Typed[SeriesAxis, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        gapDepth: Incomplete | None = None,
-        hiLowLines: ChartLines | None = None,
-        upDownBars: UpDownBars | None = None,
-        marker: Incomplete | None = None,
-        smooth: Incomplete | None = None,
+        gapWidth: int = 150,
+        gapDepth: int = 150,
+        shape: _NestedNoneSetParam[_BarChart3DShape] = None,
+        serLines: ChartLines | None = None,
+        extLst: Unused = None,
         **kw,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/marker.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/borders.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,86 @@
-from _typeshed import Incomplete, Unused
+from _typeshed import Incomplete
 from typing import ClassVar
-from typing_extensions import Literal
+from typing_extensions import Literal, TypeAlias
 
-from openpyxl.chart.picture import PictureOptions
-from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.descriptors.base import Alias, Typed
-from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.base import Alias, Bool, NoneSet, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
-class Marker(Serialisable):
-    tagname: str
-    symbol: Incomplete
-    size: Incomplete
-    spPr: Typed[GraphicalProperties, Literal[True]]
-    graphicalProperties: Alias
-    extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: ClassVar[tuple[str, ...]]
+_SideStyle: TypeAlias = Literal[
+    "dashDot",
+    "dashDotDot",
+    "dashed",
+    "dotted",
+    "double",
+    "hair",
+    "medium",
+    "mediumDashDot",
+    "mediumDashDotDot",
+    "mediumDashed",
+    "slantDashDot",
+    "thick",
+    "thin",
+]
+
+BORDER_NONE: Incomplete
+BORDER_DASHDOT: str
+BORDER_DASHDOTDOT: str
+BORDER_DASHED: str
+BORDER_DOTTED: str
+BORDER_DOUBLE: str
+BORDER_HAIR: str
+BORDER_MEDIUM: str
+BORDER_MEDIUMDASHDOT: str
+BORDER_MEDIUMDASHDOTDOT: str
+BORDER_MEDIUMDASHED: str
+BORDER_SLANTDASHDOT: str
+BORDER_THICK: str
+BORDER_THIN: str
+
+class Side(Serialisable):
+    __fields__: Incomplete
+    color: Incomplete
+    style: NoneSet[_SideStyle]
+    border_style: Alias
     def __init__(
         self,
-        symbol: Incomplete | None = None,
-        size: Incomplete | None = None,
-        spPr: GraphicalProperties | None = None,
-        extLst: Unused = None,
+        style: _SideStyle | Literal["none"] | None = None,
+        color: Incomplete | None = None,
+        border_style: Incomplete | None = None,
     ) -> None: ...
 
-class DataPoint(Serialisable):
+class Border(Serialisable):
     tagname: str
-    idx: Incomplete
-    invertIfNegative: Incomplete
-    marker: Typed[Marker, Literal[True]]
-    bubble3D: Incomplete
-    explosion: Incomplete
-    spPr: Typed[GraphicalProperties, Literal[True]]
-    graphicalProperties: Alias
-    pictureOptions: Typed[PictureOptions, Literal[True]]
-    extLst: Typed[ExtensionList, Literal[True]]
+    __fields__: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
+    start: Typed[Side, Literal[True]]
+    end: Typed[Side, Literal[True]]
+    left: Typed[Side, Literal[True]]
+    right: Typed[Side, Literal[True]]
+    top: Typed[Side, Literal[True]]
+    bottom: Typed[Side, Literal[True]]
+    diagonal: Typed[Side, Literal[True]]
+    vertical: Typed[Side, Literal[True]]
+    horizontal: Typed[Side, Literal[True]]
+    outline: Bool[Literal[False]]
+    diagonalUp: Bool[Literal[False]]
+    diagonalDown: Bool[Literal[False]]
+    diagonal_direction: Incomplete
     def __init__(
         self,
-        idx: Incomplete | None = None,
-        invertIfNegative: Incomplete | None = None,
-        marker: Marker | None = None,
-        bubble3D: Incomplete | None = None,
-        explosion: Incomplete | None = None,
-        spPr: GraphicalProperties | None = None,
-        pictureOptions: PictureOptions | None = None,
-        extLst: Unused = None,
+        left: Side | None = None,
+        right: Side | None = None,
+        top: Side | None = None,
+        bottom: Side | None = None,
+        diagonal: Side | None = None,
+        diagonal_direction: Incomplete | None = None,
+        vertical: Side | None = None,
+        horizontal: Side | None = None,
+        diagonalUp: _ConvertibleToBool = False,
+        diagonalDown: _ConvertibleToBool = False,
+        outline: _ConvertibleToBool = True,
+        start: Side | None = None,
+        end: Side | None = None,
     ) -> None: ...
+    def __iter__(self): ...
+
+DEFAULT_BORDER: Incomplete
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/pie_chart.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/line_chart.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,88 @@
 from _typeshed import Incomplete, Unused
 from abc import abstractmethod
 from typing import ClassVar
-from typing_extensions import Literal
+from typing_extensions import Literal, TypeAlias
 
-from openpyxl.chart.axis import ChartLines
+from openpyxl.chart.axis import ChartLines, NumericAxis, _BaseAxis
 from openpyxl.chart.label import DataLabelList
-from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.chart.updown_bars import UpDownBars
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
-from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.descriptors.nested import NestedBool, NestedSet, _HasTagAndGet
 
 from ._chart import ChartBase
 
-class _PieChartBase(ChartBase):
-    varyColors: Incomplete
+_LineChartBaseGrouping: TypeAlias = Literal["percentStacked", "standard", "stacked"]
+
+class _LineChartBase(ChartBase):
+    grouping: NestedSet[_LineChartBaseGrouping]
+    varyColors: NestedBool[Literal[True]]
     ser: Incomplete
     dLbls: Typed[DataLabelList, Literal[True]]
     dataLabels: Alias
+    dropLines: Typed[ChartLines, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, varyColors: bool = True, ser=(), dLbls: DataLabelList | None = None) -> None: ...
+    def __init__(
+        self,
+        grouping: _HasTagAndGet[_LineChartBaseGrouping] | _LineChartBaseGrouping = "standard",
+        varyColors: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        ser=(),
+        dLbls: DataLabelList | None = None,
+        dropLines: ChartLines | None = None,
+        **kw,
+    ) -> None: ...
     @property
     @abstractmethod
     def tagname(self) -> str: ...
 
-class PieChart(_PieChartBase):
+class LineChart(_LineChartBase):
     tagname: str
+    grouping: Incomplete
     varyColors: Incomplete
     ser: Incomplete
     dLbls: Incomplete
-    firstSliceAng: Incomplete
+    dropLines: Incomplete
+    hiLowLines: Typed[ChartLines, Literal[True]]
+    upDownBars: Typed[UpDownBars, Literal[True]]
+    marker: NestedBool[Literal[True]]
+    smooth: NestedBool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
+    x_axis: Typed[_BaseAxis, Literal[False]]
+    y_axis: Typed[NumericAxis, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, firstSliceAng: int = 0, extLst: Unused = None, **kw) -> None: ...
-
-class PieChart3D(_PieChartBase):
-    tagname: str
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: ClassVar[tuple[str, ...]]
-
-class DoughnutChart(_PieChartBase):
-    tagname: str
-    varyColors: Incomplete
-    ser: Incomplete
-    dLbls: Incomplete
-    firstSliceAng: Incomplete
-    holeSize: Incomplete
-    extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, firstSliceAng: int = 0, holeSize: int = 10, extLst: Unused = None, **kw) -> None: ...
-
-class CustomSplit(Serialisable):
-    tagname: str
-    secondPiePt: Incomplete
-    __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, secondPiePt=()) -> None: ...
+    def __init__(
+        self,
+        hiLowLines: ChartLines | None = None,
+        upDownBars: UpDownBars | None = None,
+        marker: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        smooth: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        extLst: Unused = None,
+        **kw,
+    ) -> None: ...
 
-class ProjectedPieChart(_PieChartBase):
+class LineChart3D(_LineChartBase):
     tagname: str
+    grouping: Incomplete
     varyColors: Incomplete
     ser: Incomplete
     dLbls: Incomplete
-    ofPieType: Incomplete
-    type: Alias
-    gapWidth: Incomplete
-    splitType: Incomplete
-    splitPos: Incomplete
-    custSplit: Typed[CustomSplit, Literal[True]]
-    secondPieSize: Incomplete
-    serLines: Typed[ChartLines, Literal[True]]
-    join_lines: Alias
+    dropLines: Incomplete
+    gapDepth: Incomplete
+    hiLowLines: Typed[ChartLines, Literal[True]]
+    upDownBars: Typed[UpDownBars, Literal[True]]
+    marker: NestedBool[Literal[True]]
+    smooth: NestedBool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
+    x_axis: Typed[ExtensionList, Literal[False]]
+    y_axis: Typed[ExtensionList, Literal[False]]
+    z_axis: Typed[ExtensionList, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        ofPieType: str = "pie",
-        gapWidth: Incomplete | None = None,
-        splitType: str = "auto",
-        splitPos: Incomplete | None = None,
-        custSplit: CustomSplit | None = None,
-        secondPieSize: int = 75,
-        serLines: ChartLines | None = None,
-        extLst: Unused = None,
+        gapDepth: Incomplete | None = None,
+        hiLowLines: ChartLines | None = None,
+        upDownBars: UpDownBars | None = None,
+        marker: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        smooth: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         **kw,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/pivot.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/legend.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 from _typeshed import Incomplete, Unused
 from typing import ClassVar
-from typing_extensions import Literal
+from typing_extensions import Literal, TypeAlias
 
-from openpyxl.chart.label import DataLabel as _DataLabel
-from openpyxl.chart.marker import Marker
+from openpyxl.chart.layout import Layout
 from openpyxl.chart.shapes import GraphicalProperties
 from openpyxl.chart.text import RichText
-from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.nested import NestedBool, NestedInteger, NestedSet, _HasTagAndGet
 from openpyxl.descriptors.serialisable import Serialisable
 
-class PivotSource(Serialisable):
+_LegendLegendPos: TypeAlias = Literal["b", "tr", "l", "r", "t"]
+
+class LegendEntry(Serialisable):
     tagname: str
-    name: Incomplete
-    fmtId: Incomplete
+    idx: NestedInteger[Literal[False]]
+    delete: NestedBool[Literal[False]]
+    txPr: Typed[RichText, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, name: str | None = None, fmtId: Incomplete | None = None, extLst: Unused = None) -> None: ...
+    def __init__(
+        self,
+        idx: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt = 0,
+        delete: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = False,
+        txPr: RichText | None = None,
+        extLst: Unused = None,
+    ) -> None: ...
 
-class PivotFormat(Serialisable):
+class Legend(Serialisable):
     tagname: str
-    idx: Incomplete
+    legendPos: NestedSet[_LegendLegendPos]
+    position: Alias
+    legendEntry: Incomplete
+    layout: Typed[Layout, Literal[True]]
+    overlay: NestedBool[Literal[True]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     txPr: Typed[RichText, Literal[True]]
-    TextBody: Alias
-    marker: Typed[Marker, Literal[True]]
-    dLbl: Typed[_DataLabel, Literal[True]]
-    DataLabel: Alias
+    textProperties: Alias
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        idx: int = 0,
+        legendPos: _HasTagAndGet[_LegendLegendPos] | _LegendLegendPos = "r",
+        legendEntry=(),
+        layout: Layout | None = None,
+        overlay: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         spPr: GraphicalProperties | None = None,
         txPr: RichText | None = None,
-        marker: Marker | None = None,
-        dLbl: _DataLabel | None = None,
         extLst: Unused = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/print_settings.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/print_settings.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/radar_chart.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/radar_chart.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from _typeshed import Incomplete, Unused
 from typing import ClassVar
-from typing_extensions import Literal
+from typing_extensions import Literal, TypeAlias
 
 from openpyxl.chart.axis import NumericAxis, TextAxis
 from openpyxl.chart.label import DataLabelList
-from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.nested import NestedBool, NestedSet, _HasTagAndGet
 
 from ._chart import ChartBase
 
+_RadarChartRadarStyle: TypeAlias = Literal["standard", "marker", "filled"]
+
 class RadarChart(ChartBase):
     tagname: str
-    radarStyle: Incomplete
+    radarStyle: NestedSet[_RadarChartRadarStyle]
     type: Alias
-    varyColors: Incomplete
+    varyColors: NestedBool[Literal[True]]
     ser: Incomplete
     dLbls: Typed[DataLabelList, Literal[True]]
     dataLabels: Alias
     extLst: Typed[ExtensionList, Literal[True]]
     x_axis: Typed[TextAxis, Literal[False]]
     y_axis: Typed[NumericAxis, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        radarStyle: str = "standard",
-        varyColors: Incomplete | None = None,
+        radarStyle: _HasTagAndGet[_RadarChartRadarStyle] | _RadarChartRadarStyle = "standard",
+        varyColors: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         ser=(),
         dLbls: DataLabelList | None = None,
         extLst: Unused = None,
         **kw,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/reference.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/reference.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/series.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/connector.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,97 +1,98 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar
+from typing import ClassVar, overload
 from typing_extensions import Literal
 
-from openpyxl.chart.data_source import AxDataSource, NumDataSource, StrRef
-from openpyxl.chart.error_bar import ErrorBars
-from openpyxl.chart.label import DataLabelList
-from openpyxl.chart.marker import Marker
-from openpyxl.chart.picture import PictureOptions
 from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.chart.trendline import Trendline
-from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.chart.text import RichText
+from openpyxl.descriptors import Typed
+from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
+from openpyxl.drawing.geometry import ShapeStyle
+from openpyxl.drawing.properties import NonVisualDrawingProps, NonVisualDrawingShapeProps
 
-attribute_mapping: Incomplete
+class Connection(Serialisable):
+    id: Integer[Literal[False]]
+    idx: Integer[Literal[False]]
+    def __init__(self, id: _ConvertibleToInt, idx: _ConvertibleToInt) -> None: ...
 
-class SeriesLabel(Serialisable):
-    tagname: str
-    strRef: Typed[StrRef, Literal[True]]
-    v: Incomplete
-    value: Alias
-    __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, strRef: StrRef | None = None, v: Incomplete | None = None) -> None: ...
+class ConnectorLocking(Serialisable):
+    extLst: Typed[ExtensionList, Literal[True]]
+    def __init__(self, extLst: ExtensionList | None = None) -> None: ...
 
-class Series(Serialisable):
-    tagname: str
-    idx: Incomplete
-    order: Incomplete
-    tx: Typed[SeriesLabel, Literal[True]]
-    title: Alias
-    spPr: Typed[GraphicalProperties, Literal[True]]
-    graphicalProperties: Incomplete
-    pictureOptions: Typed[PictureOptions, Literal[True]]
-    dPt: Incomplete
-    data_points: Alias
-    dLbls: Typed[DataLabelList, Literal[True]]
-    labels: Alias
-    trendline: Typed[Trendline, Literal[True]]
-    errBars: Typed[ErrorBars, Literal[True]]
-    cat: Typed[AxDataSource, Literal[True]]
-    identifiers: Alias
-    val: Typed[NumDataSource, Literal[True]]
+class NonVisualConnectorProperties(Serialisable):
+    cxnSpLocks: Typed[ConnectorLocking, Literal[True]]
+    stCxn: Typed[Connection, Literal[True]]
+    endCxn: Typed[Connection, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    invertIfNegative: Incomplete
-    shape: Incomplete
-    xVal: Typed[AxDataSource, Literal[True]]
-    yVal: Typed[NumDataSource, Literal[True]]
-    bubbleSize: Typed[NumDataSource, Literal[True]]
-    zVal: Alias
-    bubble3D: Incomplete
-    marker: Typed[Marker, Literal[True]]
-    smooth: Incomplete
-    explosion: Incomplete
+    def __init__(
+        self,
+        cxnSpLocks: ConnectorLocking | None = None,
+        stCxn: Connection | None = None,
+        endCxn: Connection | None = None,
+        extLst: ExtensionList | None = None,
+    ) -> None: ...
+
+class ConnectorNonVisual(Serialisable):
+    cNvPr: Typed[NonVisualDrawingProps, Literal[False]]
+    cNvCxnSpPr: Typed[NonVisualConnectorProperties, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, cNvPr: NonVisualDrawingProps, cNvCxnSpPr: NonVisualConnectorProperties) -> None: ...
+
+class ConnectorShape(Serialisable):
+    tagname: str
+    nvCxnSpPr: Typed[ConnectorNonVisual, Literal[False]]
+    spPr: Typed[GraphicalProperties, Literal[False]]
+    style: Typed[ShapeStyle, Literal[True]]
+    macro: String[Literal[True]]
+    fPublished: Bool[Literal[True]]
     def __init__(
         self,
-        idx: int = 0,
-        order: int = 0,
-        tx: SeriesLabel | None = None,
-        spPr: GraphicalProperties | None = None,
-        pictureOptions: PictureOptions | None = None,
-        dPt=(),
-        dLbls: DataLabelList | None = None,
-        trendline: Trendline | None = None,
-        errBars: ErrorBars | None = None,
-        cat: AxDataSource | None = None,
-        val: NumDataSource | None = None,
-        invertIfNegative: Incomplete | None = None,
-        shape: Incomplete | None = None,
-        xVal: AxDataSource | None = None,
-        yVal: NumDataSource | None = None,
-        bubbleSize: NumDataSource | None = None,
-        bubble3D: Incomplete | None = None,
-        marker: Marker | None = None,
-        smooth: Incomplete | None = None,
-        explosion: Incomplete | None = None,
-        extLst: Unused = None,
+        nvCxnSpPr: ConnectorNonVisual,
+        spPr: GraphicalProperties,
+        style: ShapeStyle | None = None,
+        macro: str | None = None,
+        fPublished: _ConvertibleToBool | None = None,
     ) -> None: ...
-    def to_tree(self, tagname: Incomplete | None = None, idx: Incomplete | None = None): ...  # type: ignore[override]
 
-class XYSeries(Series):
-    idx: Incomplete
-    order: Incomplete
-    tx: Incomplete
-    spPr: Incomplete
-    dPt: Incomplete
-    dLbls: Incomplete
-    trendline: Incomplete
-    errBars: Incomplete
-    xVal: Incomplete
-    yVal: Incomplete
-    invertIfNegative: Incomplete
-    bubbleSize: Incomplete
-    bubble3D: Incomplete
-    marker: Incomplete
-    smooth: Incomplete
+class ShapeMeta(Serialisable):
+    tagname: str
+    cNvPr: Typed[NonVisualDrawingProps, Literal[False]]
+    cNvSpPr: Typed[NonVisualDrawingShapeProps, Literal[False]]
+    def __init__(self, cNvPr: NonVisualDrawingProps, cNvSpPr: NonVisualDrawingShapeProps) -> None: ...
+
+class Shape(Serialisable):
+    macro: String[Literal[True]]
+    textlink: String[Literal[True]]
+    fPublished: Bool[Literal[True]]
+    fLocksText: Bool[Literal[True]]
+    nvSpPr: Typed[ShapeMeta, Literal[True]]
+    meta: Alias
+    spPr: Typed[GraphicalProperties, Literal[False]]
+    graphicalProperties: Alias
+    style: Typed[ShapeStyle, Literal[True]]
+    txBody: Typed[RichText, Literal[True]]
+    @overload
+    def __init__(
+        self,
+        macro: str | None = None,
+        textlink: str | None = None,
+        fPublished: _ConvertibleToBool | None = None,
+        fLocksText: _ConvertibleToBool | None = None,
+        nvSpPr: ShapeMeta | None = None,
+        *,
+        spPr: GraphicalProperties,
+        style: ShapeStyle | None = None,
+        txBody: RichText | None = None,
+    ) -> None: ...
+    @overload
+    def __init__(
+        self,
+        macro: str | None,
+        textlink: str | None,
+        fPublished: _ConvertibleToBool | None,
+        fLocksText: _ConvertibleToBool | None,
+        nvSpPr: ShapeMeta | None,
+        spPr: GraphicalProperties,
+        style: ShapeStyle | None = None,
+        txBody: RichText | None = None,
+    ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/shapes.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/shapes.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from _typeshed import Incomplete, Unused
 from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
-from openpyxl.descriptors.base import Alias, NoneSet, Typed
+from openpyxl.descriptors.base import Alias, NoneSet, Typed, _ConvertibleToBool
+from openpyxl.descriptors.nested import EmptyTag, _HasTagAndGet
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.fill import GradientFillProperties, PatternFillProperties
 from openpyxl.drawing.geometry import CustomGeometry2D, PresetGeometry2D, Scene3D, Shape3D, Transform2D
 from openpyxl.drawing.line import LineProperties
 
 _GraphicalPropertiesBwMode: TypeAlias = Literal[
     "clr", "auto", "gray", "ltGray", "invGray", "grayWhite", "blackGray", "blackWhite", "black", "white", "hidden"
@@ -15,30 +16,30 @@
 class GraphicalProperties(Serialisable):
     tagname: str
     bwMode: NoneSet[_GraphicalPropertiesBwMode]
     xfrm: Typed[Transform2D, Literal[True]]
     transform: Alias
     custGeom: Typed[CustomGeometry2D, Literal[True]]
     prstGeom: Typed[PresetGeometry2D, Literal[True]]
-    noFill: Incomplete
+    noFill: EmptyTag[Literal[False]]
     solidFill: Incomplete
     gradFill: Typed[GradientFillProperties, Literal[True]]
     pattFill: Typed[PatternFillProperties, Literal[True]]
     ln: Typed[LineProperties, Literal[True]]
     line: Alias
     scene3d: Typed[Scene3D, Literal[True]]
     sp3d: Typed[Shape3D, Literal[True]]
     shape3D: Alias
     extLst: Typed[Incomplete, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         bwMode: _GraphicalPropertiesBwMode | Literal["none"] | None = None,
         xfrm: Transform2D | None = None,
-        noFill: Incomplete | None = None,
+        noFill: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         solidFill: Incomplete | None = None,
         gradFill: GradientFillProperties | None = None,
         pattFill: PatternFillProperties | None = None,
         ln: Incomplete | None = None,
         scene3d: Scene3D | None = None,
         custGeom: CustomGeometry2D | None = None,
         prstGeom: PresetGeometry2D | None = None,
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/surface_chart.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/surface_chart.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 from _typeshed import Incomplete
 from abc import abstractmethod
 from typing import ClassVar
 from typing_extensions import Literal
 
 from openpyxl.chart.axis import NumericAxis, SeriesAxis, TextAxis
 from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.descriptors.base import Alias, Typed
+from openpyxl.descriptors.base import Alias, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.nested import NestedBool, NestedInteger, _HasTagAndGet
 from openpyxl.descriptors.serialisable import Serialisable
 
 from ._3d import _3DBase
 from ._chart import ChartBase
 
 class BandFormat(Serialisable):
     tagname: str
-    idx: Incomplete
+    idx: NestedInteger[Literal[False]]
     spPr: Typed[GraphicalProperties, Literal[True]]
     graphicalProperties: Alias
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, idx: int = 0, spPr: GraphicalProperties | None = None) -> None: ...
+    def __init__(
+        self, idx: _HasTagAndGet[_ConvertibleToInt] | _ConvertibleToInt = 0, spPr: GraphicalProperties | None = None
+    ) -> None: ...
 
 class BandFormatList(Serialisable):
     tagname: str
     bandFmt: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, bandFmt=()) -> None: ...
 
 class _SurfaceChartBase(ChartBase):
-    wireframe: Incomplete
+    wireframe: NestedBool[Literal[True]]
     ser: Incomplete
     bandFmts: Typed[BandFormatList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, wireframe: Incomplete | None = None, ser=(), bandFmts: BandFormatList | None = None, **kw) -> None: ...
+    def __init__(
+        self,
+        wireframe: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        ser=(),
+        bandFmts: BandFormatList | None = None,
+        **kw,
+    ) -> None: ...
     @property
     @abstractmethod
     def tagname(self) -> str: ...
 
 class SurfaceChart3D(_SurfaceChartBase, _3DBase):
     tagname: str
     wireframe: Incomplete
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/text.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/text.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/title.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/views.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 from _typeshed import Incomplete, Unused
 from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.chart.layout import Layout
-from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.chart.text import RichText, Text
-from openpyxl.descriptors import Strict, Typed
-from openpyxl.descriptors.base import Alias
+from openpyxl.descriptors.base import Bool, Integer, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
 
-class Title(Serialisable):
+class ChartsheetView(Serialisable):
     tagname: str
-    tx: Typed[Text, Literal[True]]
-    text: Alias
-    layout: Typed[Layout, Literal[True]]
-    overlay: Incomplete
-    spPr: Typed[GraphicalProperties, Literal[True]]
-    graphicalProperties: Alias
-    txPr: Typed[RichText, Literal[True]]
-    body: Alias
+    tabSelected: Bool[Literal[True]]
+    zoomScale: Integer[Literal[True]]
+    workbookViewId: Integer[Literal[False]]
+    zoomToFit: Bool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        tx: Text | None = None,
-        layout: Layout | None = None,
-        overlay: Incomplete | None = None,
-        spPr: GraphicalProperties | None = None,
-        txPr: RichText | None = None,
+        tabSelected: _ConvertibleToBool | None = None,
+        zoomScale: _ConvertibleToInt | None = None,
+        workbookViewId: _ConvertibleToInt = 0,
+        zoomToFit: _ConvertibleToBool | None = True,
         extLst: Unused = None,
     ) -> None: ...
 
-def title_maker(text): ...
-
-class TitleDescriptor(Typed[Title, Incomplete]):
-    expected_type: type[Title]
-    allow_none: Literal[True]
-    def __set__(self, instance: Serialisable | Strict, value) -> None: ...
+class ChartsheetViewList(Serialisable):
+    tagname: str
+    sheetView: Incomplete
+    extLst: Typed[ExtensionList, Literal[True]]
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, sheetView: Incomplete | None = None, extLst: Unused = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chart/updown_bars.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/updown_bars.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/chartsheet.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/chartsheet.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/custom.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/custom.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/properties.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/properties.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/protection.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/protection.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/publish.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/publish.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/relation.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chartsheet/relation.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/chartsheet/views.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/errors.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,50 @@
-from _typeshed import Incomplete, Unused
+from _typeshed import Incomplete
 from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.descriptors.base import Bool, Integer, Typed, _ConvertibleToBool, _ConvertibleToInt
-from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.base import Bool, String, Typed, _ConvertibleToBool
 from openpyxl.descriptors.serialisable import Serialisable
 
-class ChartsheetView(Serialisable):
+class Extension(Serialisable):
     tagname: str
-    tabSelected: Bool[Literal[True]]
-    zoomScale: Integer[Literal[True]]
-    workbookViewId: Integer[Literal[False]]
-    zoomToFit: Bool[Literal[True]]
-    extLst: Typed[ExtensionList, Literal[True]]
+    uri: String[Literal[True]]
+    def __init__(self, uri: str | None = None) -> None: ...
+
+class ExtensionList(Serialisable):
+    tagname: str
+    ext: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, ext=()) -> None: ...
+
+class IgnoredError(Serialisable):
+    tagname: str
+    sqref: Incomplete
+    evalError: Bool[Literal[True]]
+    twoDigitTextYear: Bool[Literal[True]]
+    numberStoredAsText: Bool[Literal[True]]
+    formula: Bool[Literal[True]]
+    formulaRange: Bool[Literal[True]]
+    unlockedFormula: Bool[Literal[True]]
+    emptyCellReference: Bool[Literal[True]]
+    listDataValidation: Bool[Literal[True]]
+    calculatedColumn: Bool[Literal[True]]
     def __init__(
         self,
-        tabSelected: _ConvertibleToBool | None = None,
-        zoomScale: _ConvertibleToInt | None = None,
-        workbookViewId: _ConvertibleToInt = 0,
-        zoomToFit: _ConvertibleToBool | None = True,
-        extLst: Unused = None,
+        sqref: Incomplete | None = None,
+        evalError: _ConvertibleToBool | None = False,
+        twoDigitTextYear: _ConvertibleToBool | None = False,
+        numberStoredAsText: _ConvertibleToBool | None = False,
+        formula: _ConvertibleToBool | None = False,
+        formulaRange: _ConvertibleToBool | None = False,
+        unlockedFormula: _ConvertibleToBool | None = False,
+        emptyCellReference: _ConvertibleToBool | None = False,
+        listDataValidation: _ConvertibleToBool | None = False,
+        calculatedColumn: _ConvertibleToBool | None = False,
     ) -> None: ...
 
-class ChartsheetViewList(Serialisable):
+class IgnoredErrors(Serialisable):
     tagname: str
-    sheetView: Incomplete
+    ignoredError: Incomplete
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, sheetView: Incomplete | None = None, extLst: Unused = None) -> None: ...
+    def __init__(self, ignoredError=(), extLst: ExtensionList | None = None) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/comments/comment_sheet.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/comments/comment_sheet.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/base.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/base.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
     expected_type: type[bool]
     allow_none: _N
     @overload
     def __init__(self: Bool[Literal[True]], name: str | None = None, *, allow_none: Literal[True]) -> None: ...
     @overload
     def __init__(self: Bool[Literal[False]], name: str | None = None, *, allow_none: Literal[False] = False) -> None: ...
     def __set__(  # type:ignore[override]  # Different restrictions
-        self: Bool[Literal[True]], instance: Serialisable | Strict, value: _ConvertibleToBool | None
+        self, instance: Serialisable | Strict, value: _ConvertibleToBool
     ) -> None: ...
 
 class String(Typed[str, _N]):
     allow_none: _N
     expected_type: type[str]
     @overload
     def __init__(self: String[Literal[True]], name: str | None = None, *, allow_none: Literal[True]) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/excel.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/excel.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/sequence.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/sequence.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/descriptors/serialisable.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/descriptors/serialisable.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/connector.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/cell_style.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,98 +1,95 @@
-from typing import ClassVar, overload
+from _typeshed import Incomplete, Unused
+from array import array
+from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.chart.shapes import GraphicalProperties
-from openpyxl.chart.text import RichText
-from openpyxl.descriptors import Typed
-from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors import Strict
+from openpyxl.descriptors.base import Bool, Integer, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.drawing.geometry import ShapeStyle
-from openpyxl.drawing.properties import NonVisualDrawingProps, NonVisualDrawingShapeProps
+from openpyxl.styles.alignment import Alignment
+from openpyxl.styles.protection import Protection
 
-class Connection(Serialisable):
-    id: Integer[Literal[False]]
-    idx: Integer[Literal[False]]
-    def __init__(self, id: _ConvertibleToInt, idx: _ConvertibleToInt) -> None: ...
+class ArrayDescriptor:
+    key: Incomplete
+    def __init__(self, key) -> None: ...
+    def __get__(self, instance: Serialisable | Strict, cls: Unused): ...
+    def __set__(self, instance: Serialisable | Strict, value) -> None: ...
 
-class ConnectorLocking(Serialisable):
-    extLst: Typed[ExtensionList, Literal[True]]
-    def __init__(self, extLst: ExtensionList | None = None) -> None: ...
+class StyleArray(array[Incomplete]):
+    tagname: str
+    fontId: Incomplete
+    fillId: Incomplete
+    borderId: Incomplete
+    numFmtId: Incomplete
+    protectionId: Incomplete
+    alignmentId: Incomplete
+    pivotButton: Incomplete
+    quotePrefix: Incomplete
+    xfId: Incomplete
+    def __new__(cls, args=[0, 0, 0, 0, 0, 0, 0, 0, 0]): ...
+    def __hash__(self) -> int: ...
+    def __copy__(self): ...
+    def __deepcopy__(self, memo): ...
 
-class NonVisualConnectorProperties(Serialisable):
-    cxnSpLocks: Typed[ConnectorLocking, Literal[True]]
-    stCxn: Typed[Connection, Literal[True]]
-    endCxn: Typed[Connection, Literal[True]]
+class CellStyle(Serialisable):
+    tagname: str
+    numFmtId: Integer[Literal[False]]
+    fontId: Integer[Literal[False]]
+    fillId: Integer[Literal[False]]
+    borderId: Integer[Literal[False]]
+    xfId: Integer[Literal[True]]
+    quotePrefix: Bool[Literal[True]]
+    pivotButton: Bool[Literal[True]]
+    applyNumberFormat: Bool[Literal[True]]
+    applyFont: Bool[Literal[True]]
+    applyFill: Bool[Literal[True]]
+    applyBorder: Bool[Literal[True]]
+    # Overwritten by properties below
+    # applyAlignment: Bool[Literal[True]]
+    # applyProtection: Bool[Literal[True]]
+    alignment: Typed[Alignment, Literal[True]]
+    protection: Typed[Protection, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    def __init__(
-        self,
-        cxnSpLocks: ConnectorLocking | None = None,
-        stCxn: Connection | None = None,
-        endCxn: Connection | None = None,
-        extLst: ExtensionList | None = None,
-    ) -> None: ...
-
-class ConnectorNonVisual(Serialisable):
-    cNvPr: Typed[NonVisualDrawingProps, Literal[False]]
-    cNvCxnSpPr: Typed[NonVisualConnectorProperties, Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, cNvPr: NonVisualDrawingProps, cNvCxnSpPr: NonVisualConnectorProperties) -> None: ...
-
-class ConnectorShape(Serialisable):
-    tagname: str
-    nvCxnSpPr: Typed[ConnectorNonVisual, Literal[False]]
-    spPr: Typed[GraphicalProperties, Literal[False]]
-    style: Typed[ShapeStyle, Literal[True]]
-    macro: String[Literal[True]]
-    fPublished: Bool[Literal[True]]
+    __attrs__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
-        nvCxnSpPr: ConnectorNonVisual,
-        spPr: GraphicalProperties,
-        style: ShapeStyle | None = None,
-        macro: str | None = None,
-        fPublished: _ConvertibleToBool | None = None,
+        numFmtId: _ConvertibleToInt = 0,
+        fontId: _ConvertibleToInt = 0,
+        fillId: _ConvertibleToInt = 0,
+        borderId: _ConvertibleToInt = 0,
+        xfId: _ConvertibleToInt | None = None,
+        quotePrefix: _ConvertibleToBool | None = None,
+        pivotButton: _ConvertibleToBool | None = None,
+        applyNumberFormat: _ConvertibleToBool | None = None,
+        applyFont: _ConvertibleToBool | None = None,
+        applyFill: _ConvertibleToBool | None = None,
+        applyBorder: _ConvertibleToBool | None = None,
+        applyAlignment: Unused = None,
+        applyProtection: Unused = None,
+        alignment: Alignment | None = None,
+        protection: Protection | None = None,
+        extLst: Unused = None,
     ) -> None: ...
+    def to_array(self): ...
+    @classmethod
+    def from_array(cls, style): ...
+    @property
+    def applyProtection(self): ...
+    @property
+    def applyAlignment(self): ...
 
-class ShapeMeta(Serialisable):
+class CellStyleList(Serialisable):
     tagname: str
-    cNvPr: Typed[NonVisualDrawingProps, Literal[False]]
-    cNvSpPr: Typed[NonVisualDrawingShapeProps, Literal[False]]
-    def __init__(self, cNvPr: NonVisualDrawingProps, cNvSpPr: NonVisualDrawingShapeProps) -> None: ...
-
-class Shape(Serialisable):
-    macro: String[Literal[True]]
-    textlink: String[Literal[True]]
-    fPublished: Bool[Literal[True]]
-    fLocksText: Bool[Literal[True]]
-    nvSpPr: Typed[ShapeMeta, Literal[True]]
-    meta: Alias
-    spPr: Typed[GraphicalProperties, Literal[False]]
-    graphicalProperties: Alias
-    style: Typed[ShapeStyle, Literal[True]]
-    txBody: Typed[RichText, Literal[True]]
-    @overload
-    def __init__(
-        self,
-        macro: str | None = None,
-        textlink: str | None = None,
-        fPublished: _ConvertibleToBool | None = None,
-        fLocksText: _ConvertibleToBool | None = None,
-        nvSpPr: ShapeMeta | None = None,
-        *,
-        spPr: GraphicalProperties,
-        style: ShapeStyle | None = None,
-        txBody: RichText | None = None,
-    ) -> None: ...
-    @overload
-    def __init__(
-        self,
-        macro: str | None,
-        textlink: str | None,
-        fPublished: _ConvertibleToBool | None,
-        fLocksText: _ConvertibleToBool | None,
-        nvSpPr: ShapeMeta | None,
-        spPr: GraphicalProperties,
-        style: ShapeStyle | None = None,
-        txBody: RichText | None = None,
-    ) -> None: ...
+    __attrs__: ClassVar[tuple[str, ...]]
+    # Overwritten by property below
+    # count: Integer
+    xf: Incomplete
+    alignment: Incomplete
+    protection: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, count: Unused = None, xf=()) -> None: ...
+    @property
+    def count(self): ...
+    def __getitem__(self, idx): ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/drawing.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/drawing.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/effect.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/effect.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/fill.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/fill.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,17 @@
     Set,
     Typed,
     _ConvertibleToBool,
     _ConvertibleToFloat,
     _ConvertibleToInt,
 )
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.nested import NestedNoneSet, NestedValue, _HasTagAndGet, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.drawing.colors import ColorChoice, HSLColor, RGBPercent as _RGBPercent, SchemeColor, SystemColor
+from openpyxl.drawing.colors import ColorChoice, HSLColor, RGBPercent as _RGBPercent, SchemeColor, SystemColor, _PresetColors
 from openpyxl.drawing.effect import (
     AlphaBiLevelEffect,
     AlphaCeilingEffect,
     AlphaFloorEffect,
     AlphaInverseEffect,
     AlphaModulateEffect,
     AlphaModulateFixedEffect,
@@ -138,30 +139,30 @@
 
 class GradientStop(Serialisable):
     tagname: str
     namespace: Incomplete
     pos: MinMax[float, Literal[True]]
     scrgbClr: Typed[_RGBPercent, Literal[True]]
     RGBPercent: Alias
-    srgbClr: Incomplete
+    srgbClr: NestedValue[_RGBPercent, Literal[True]]
     RGB: Alias
     hslClr: Typed[HSLColor, Literal[True]]
     sysClr: Typed[SystemColor, Literal[True]]
     schemeClr: Typed[SchemeColor, Literal[True]]
-    prstClr: Incomplete
+    prstClr: NestedNoneSet[_PresetColors]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         pos: _ConvertibleToFloat | None = None,
         scrgbClr: _RGBPercent | None = None,
-        srgbClr: Incomplete | None = None,
+        srgbClr: _HasTagAndGet[_RGBPercent | None] | _RGBPercent | None = None,
         hslClr: HSLColor | None = None,
         sysClr: SystemColor | None = None,
         schemeClr: SchemeColor | None = None,
-        prstClr: Incomplete | None = None,
+        prstClr: _NestedNoneSetParam[_PresetColors] = None,
     ) -> None: ...
 
 class LinearShadeProperties(Serialisable):
     tagname: str
     namespace: Incomplete
     ang: Integer[Literal[False]]
     scaled: Bool[Literal[True]]
@@ -196,29 +197,29 @@
         tileRect: RelativeRect | None = None,
     ) -> None: ...
 
 class SolidColorFillProperties(Serialisable):
     tagname: str
     scrgbClr: Typed[_RGBPercent, Literal[True]]
     RGBPercent: Alias
-    srgbClr: Incomplete
+    srgbClr: NestedValue[_RGBPercent, Literal[True]]
     RGB: Alias
     hslClr: Typed[HSLColor, Literal[True]]
     sysClr: Typed[SystemColor, Literal[True]]
     schemeClr: Typed[SchemeColor, Literal[True]]
-    prstClr: Incomplete
+    prstClr: NestedNoneSet[_PresetColors]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         scrgbClr: _RGBPercent | None = None,
-        srgbClr: Incomplete | None = None,
+        srgbClr: _HasTagAndGet[_RGBPercent | None] | _RGBPercent | None = None,
         hslClr: HSLColor | None = None,
         sysClr: SystemColor | None = None,
         schemeClr: SchemeColor | None = None,
-        prstClr: Incomplete | None = None,
+        prstClr: _NestedNoneSetParam[_PresetColors] = None,
     ) -> None: ...
 
 class Blip(Serialisable):
     tagname: str
     namespace: Incomplete
     cstate: NoneSet[_BlipCstate]
     embed: Incomplete
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/geometry.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/geometry.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/graphic.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/graphic.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/line.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/line.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 from _typeshed import Incomplete, Unused
 from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
-from openpyxl.descriptors.base import Alias, Integer, MinMax, NoneSet, Typed, _ConvertibleToFloat, _ConvertibleToInt
+from openpyxl.descriptors.base import (
+    Alias,
+    Integer,
+    MinMax,
+    NoneSet,
+    Typed,
+    _ConvertibleToBool,
+    _ConvertibleToFloat,
+    _ConvertibleToInt,
+)
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.nested import EmptyTag, NestedInteger, NestedNoneSet, _HasTagAndGet, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.fill import GradientFillProperties, PatternFillProperties
 
 _LineEndPropertiesType: TypeAlias = Literal["none", "triangle", "stealth", "diamond", "oval", "arrow"]
 _LineEndPropertiesWLen: TypeAlias = Literal["sm", "med", "lg"]
 _LinePropertiesCap: TypeAlias = Literal["rnd", "sq", "flat"]
 _LinePropertiesCmpd: TypeAlias = Literal["sng", "dbl", "thickThin", "thinThick", "tri"]
 _LinePropertiesAlgn: TypeAlias = Literal["ctr", "in"]
+_LinePropertiesPrstDash: TypeAlias = Literal[
+    "solid", "dot", "dash", "lgDash", "dashDot", "lgDashDot", "lgDashDotDot", "sysDash", "sysDot", "sysDashDot", "sysDashDotDot"
+]
 
 class LineEndProperties(Serialisable):
     tagname: str
     namespace: Incomplete
     type: NoneSet[_LineEndPropertiesType]
     w: NoneSet[_LineEndPropertiesWLen]
     len: NoneSet[_LineEndPropertiesWLen]
@@ -43,40 +56,40 @@
     tagname: str
     namespace: Incomplete
     w: MinMax[float, Literal[True]]
     width: Alias
     cap: NoneSet[_LinePropertiesCap]
     cmpd: NoneSet[_LinePropertiesCmpd]
     algn: NoneSet[_LinePropertiesAlgn]
-    noFill: Incomplete
+    noFill: EmptyTag[Literal[False]]
     solidFill: Incomplete
     gradFill: Typed[GradientFillProperties, Literal[True]]
     pattFill: Typed[PatternFillProperties, Literal[True]]
-    prstDash: Incomplete
+    prstDash: NestedNoneSet[_LinePropertiesPrstDash]
     dashStyle: Alias
     custDash: Typed[DashStop, Literal[True]]
-    round: Incomplete
-    bevel: Incomplete
-    miter: Incomplete
+    round: EmptyTag[Literal[False]]
+    bevel: EmptyTag[Literal[False]]
+    miter: NestedInteger[Literal[True]]
     headEnd: Typed[LineEndProperties, Literal[True]]
     tailEnd: Typed[LineEndProperties, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         w: _ConvertibleToFloat | None = None,
         cap: _LinePropertiesCap | Literal["none"] | None = None,
         cmpd: _LinePropertiesCmpd | Literal["none"] | None = None,
         algn: _LinePropertiesAlgn | Literal["none"] | None = None,
-        noFill: Incomplete | None = None,
+        noFill: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         solidFill: Incomplete | None = None,
         gradFill: GradientFillProperties | None = None,
         pattFill: PatternFillProperties | None = None,
-        prstDash: Incomplete | None = None,
+        prstDash: _NestedNoneSetParam[_LinePropertiesPrstDash] = None,
         custDash: DashStop | None = None,
-        round: Incomplete | None = None,
-        bevel: Incomplete | None = None,
-        miter: Incomplete | None = None,
+        round: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        bevel: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        miter: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
         headEnd: LineEndProperties | None = None,
         tailEnd: LineEndProperties | None = None,
         extLst: Unused = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/picture.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/picture.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/properties.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/properties.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/spreadsheet_drawing.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/spreadsheet_drawing.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from _typeshed import Incomplete
 from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
-from openpyxl.descriptors.base import Alias, Bool, NoneSet, Typed, _ConvertibleToBool
+from openpyxl.descriptors.base import Alias, Bool, NoneSet, Typed, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.nested import NestedText
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.connector import Shape
 from openpyxl.drawing.graphic import GraphicFrame, GroupShape
 from openpyxl.drawing.picture import PictureFrame
 from openpyxl.drawing.xdr import XDRPoint2D, XDRPositiveSize2D
 
 _TwoCellAnchorEditAs: TypeAlias = Literal["twoCell", "oneCell", "absolute"]
@@ -16,19 +17,21 @@
     fPrintsWithSheet: Bool[Literal[True]]
     def __init__(
         self, fLocksWithSheet: _ConvertibleToBool | None = None, fPrintsWithSheet: _ConvertibleToBool | None = None
     ) -> None: ...
 
 class AnchorMarker(Serialisable):
     tagname: str
-    col: Incomplete
-    colOff: Incomplete
-    row: Incomplete
-    rowOff: Incomplete
-    def __init__(self, col: int = 0, colOff: int = 0, row: int = 0, rowOff: int = 0) -> None: ...
+    col: NestedText[int, Literal[False]]
+    colOff: NestedText[int, Literal[False]]
+    row: NestedText[int, Literal[False]]
+    rowOff: NestedText[int, Literal[False]]
+    def __init__(
+        self, col: _ConvertibleToInt = 0, colOff: _ConvertibleToInt = 0, row: _ConvertibleToInt = 0, rowOff: _ConvertibleToInt = 0
+    ) -> None: ...
 
 class _AnchorBase(Serialisable):
     sp: Typed[Shape, Literal[True]]
     shape: Alias
     grpSp: Typed[GroupShape, Literal[True]]
     groupShape: Alias
     graphicFrame: Typed[GraphicFrame, Literal[True]]
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/drawing/text.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/drawing/text.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from _typeshed import Incomplete
+from _typeshed import Incomplete, Unused
 from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import (
     Alias,
     Bool,
     Integer,
@@ -12,17 +12,18 @@
     String,
     Typed,
     _ConvertibleToBool,
     _ConvertibleToFloat,
     _ConvertibleToInt,
 )
 from openpyxl.descriptors.excel import Coordinate, ExtensionList
+from openpyxl.descriptors.nested import EmptyTag, NestedBool, NestedInteger, NestedText, NestedValue, _HasTagAndGet
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.drawing.effect import Color, EffectContainer, EffectList
-from openpyxl.drawing.fill import BlipFillProperties, GradientFillProperties, PatternFillProperties
+from openpyxl.drawing.fill import Blip, BlipFillProperties, GradientFillProperties, PatternFillProperties
 from openpyxl.drawing.geometry import Scene3D
 from openpyxl.drawing.line import LineProperties
 
 _CharacterPropertiesU: TypeAlias = Literal[
     "words",
     "sng",
     "dbl",
@@ -213,28 +214,28 @@
     highlight: Typed[Color, Literal[True]]
     latin: Typed[Font, Literal[True]]
     ea: Typed[Font, Literal[True]]
     cs: Typed[Font, Literal[True]]
     sym: Typed[Font, Literal[True]]
     hlinkClick: Typed[Hyperlink, Literal[True]]
     hlinkMouseOver: Typed[Hyperlink, Literal[True]]
-    rtl: Incomplete
+    rtl: NestedBool[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    noFill: Incomplete
+    noFill: EmptyTag[Literal[False]]
     solidFill: Incomplete
     gradFill: Typed[GradientFillProperties, Literal[True]]
     blipFill: Typed[BlipFillProperties, Literal[True]]
     pattFill: Typed[PatternFillProperties, Literal[True]]
-    grpFill: Incomplete
+    grpFill: EmptyTag[Literal[False]]
     effectLst: Typed[EffectList, Literal[True]]
     effectDag: Typed[EffectContainer, Literal[True]]
-    uLnTx: Incomplete
+    uLnTx: EmptyTag[Literal[False]]
     uLn: Typed[LineProperties, Literal[True]]
-    uFillTx: Incomplete
-    uFill: Incomplete
+    uFillTx: EmptyTag[Literal[False]]
+    uFill: EmptyTag[Literal[False]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         kumimoji: _ConvertibleToBool | None = None,
         lang: str | None = None,
         altLang: str | None = None,
         sz: _ConvertibleToFloat | None = None,
@@ -257,44 +258,48 @@
         highlight: Color | None = None,
         latin: Font | None = None,
         ea: Font | None = None,
         cs: Font | None = None,
         sym: Font | None = None,
         hlinkClick: Hyperlink | None = None,
         hlinkMouseOver: Hyperlink | None = None,
-        rtl: Incomplete | None = None,
+        rtl: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
         extLst: ExtensionList | None = None,
-        noFill: Incomplete | None = None,
+        noFill: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         solidFill: Incomplete | None = None,
         gradFill: GradientFillProperties | None = None,
         blipFill: BlipFillProperties | None = None,
         pattFill: PatternFillProperties | None = None,
-        grpFill: Incomplete | None = None,
+        grpFill: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         effectLst: EffectList | None = None,
         effectDag: EffectContainer | None = None,
-        uLnTx: Incomplete | None = None,
+        uLnTx: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         uLn: LineProperties | None = None,
-        uFillTx: Incomplete | None = None,
-        uFill: Incomplete | None = None,
+        uFillTx: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        uFill: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
     ) -> None: ...
 
 class TabStop(Serialisable):
     pos: Typed[Coordinate[bool], Literal[True]]
     algn: Typed[Set[_TabStopAlgn], Literal[False]]
     def __init__(self, pos: Coordinate[bool] | None = None, algn: Set[_TabStopAlgn] | None = None) -> None: ...
 
 class TabStopList(Serialisable):
     tab: Typed[TabStop, Literal[True]]
     def __init__(self, tab: Incomplete | None = None) -> None: ...
 
 class Spacing(Serialisable):
-    spcPct: Incomplete
-    spcPts: Incomplete
+    spcPct: NestedInteger[Literal[True]]
+    spcPts: NestedInteger[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, spcPct: Incomplete | None = None, spcPts: Incomplete | None = None) -> None: ...
+    def __init__(
+        self,
+        spcPct: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        spcPts: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+    ) -> None: ...
 
 class AutonumberBullet(Serialisable):
     type: Set[_AutonumberBulletType]
     startAt: Integer[Literal[False]]
     def __init__(self, type: _AutonumberBulletType, startAt: _ConvertibleToInt) -> None: ...
 
 class ParagraphProperties(Serialisable):
@@ -313,25 +318,25 @@
     hangingPunct: Bool[Literal[True]]
     lnSpc: Typed[Spacing, Literal[True]]
     spcBef: Typed[Spacing, Literal[True]]
     spcAft: Typed[Spacing, Literal[True]]
     tabLst: Typed[TabStopList, Literal[True]]
     defRPr: Typed[CharacterProperties, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    buClrTx: Incomplete
+    buClrTx: EmptyTag[Literal[False]]
     buClr: Typed[Color, Literal[True]]
-    buSzTx: Incomplete
-    buSzPct: Incomplete
-    buSzPts: Incomplete
-    buFontTx: Incomplete
+    buSzTx: EmptyTag[Literal[False]]
+    buSzPct: NestedInteger[Literal[True]]
+    buSzPts: NestedInteger[Literal[True]]
+    buFontTx: EmptyTag[Literal[False]]
     buFont: Typed[Font, Literal[True]]
-    buNone: Incomplete
-    buAutoNum: Incomplete
-    buChar: Incomplete
-    buBlip: Incomplete
+    buNone: EmptyTag[Literal[False]]
+    buAutoNum: EmptyTag[Literal[False]]
+    buChar: NestedValue[str, Literal[True]]
+    buBlip: NestedValue[Blip, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         marL: _ConvertibleToInt | None = None,
         marR: _ConvertibleToInt | None = None,
         lvl: _ConvertibleToInt | None = None,
         indent: _ConvertibleToInt | None = None,
@@ -344,25 +349,25 @@
         hangingPunct: _ConvertibleToBool | None = None,
         lnSpc: Spacing | None = None,
         spcBef: Spacing | None = None,
         spcAft: Spacing | None = None,
         tabLst: TabStopList | None = None,
         defRPr: CharacterProperties | None = None,
         extLst: ExtensionList | None = None,
-        buClrTx: Incomplete | None = None,
+        buClrTx: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         buClr: Color | None = None,
-        buSzTx: Incomplete | None = None,
-        buSzPct: Incomplete | None = None,
-        buSzPts: Incomplete | None = None,
-        buFontTx: Incomplete | None = None,
+        buSzTx: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        buSzPct: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        buSzPts: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        buFontTx: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
         buFont: Font | None = None,
-        buNone: Incomplete | None = None,
-        buAutoNum: Incomplete | None = None,
-        buChar: Incomplete | None = None,
-        buBlip: Incomplete | None = None,
+        buNone: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        buAutoNum: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        buChar: object = None,
+        buBlip: object = None,
     ) -> None: ...
 
 class ListStyle(Serialisable):
     tagname: str
     namespace: Incomplete
     defPPr: Typed[ParagraphProperties, Literal[True]]
     lvl1pPr: Typed[ParagraphProperties, Literal[True]]
@@ -392,18 +397,18 @@
     ) -> None: ...
 
 class RegularTextRun(Serialisable):
     tagname: str
     namespace: Incomplete
     rPr: Typed[CharacterProperties, Literal[True]]
     properties: Alias
-    t: Incomplete
+    t: NestedText[str, Literal[False]]
     value: Alias
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, rPr: CharacterProperties | None = None, t: str = "") -> None: ...
+    def __init__(self, rPr: CharacterProperties | None = None, t: object = "") -> None: ...
 
 class LineBreak(Serialisable):
     tagname: str
     namespace: Incomplete
     rPr: Typed[CharacterProperties, Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(self, rPr: CharacterProperties | None = None) -> None: ...
@@ -484,18 +489,18 @@
     anchorCtr: Bool[Literal[True]]
     forceAA: Bool[Literal[True]]
     upright: Bool[Literal[True]]
     compatLnSpc: Bool[Literal[True]]
     prstTxWarp: Typed[PresetTextShape, Literal[True]]
     scene3d: Typed[Scene3D, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    noAutofit: Incomplete
-    normAutofit: Incomplete
-    spAutoFit: Incomplete
-    flatTx: Incomplete
+    noAutofit: EmptyTag[Literal[False]]
+    normAutofit: EmptyTag[Literal[False]]
+    spAutoFit: EmptyTag[Literal[False]]
+    flatTx: NestedInteger[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         rot: _ConvertibleToInt | None = None,
         spcFirstLastPara: _ConvertibleToBool | None = None,
         vertOverflow: _RichTextPropertiesVertOverflow | Literal["none"] | None = None,
         horzOverflow: _RichTextPropertiesHorzOverflow | Literal["none"] | None = None,
@@ -510,15 +515,15 @@
         rtlCol: _ConvertibleToBool | None = None,
         fromWordArt: _ConvertibleToBool | None = None,
         anchor: _RichTextPropertiesAnchor | Literal["none"] | None = None,
         anchorCtr: _ConvertibleToBool | None = None,
         forceAA: _ConvertibleToBool | None = None,
         upright: _ConvertibleToBool | None = None,
         compatLnSpc: _ConvertibleToBool | None = None,
-        prstTxWarp: Incomplete | None = None,
-        scene3d: Incomplete | None = None,
-        extLst: Incomplete | None = None,
-        noAutofit: Incomplete | None = None,
-        normAutofit: Incomplete | None = None,
-        spAutoFit: Incomplete | None = None,
-        flatTx: Incomplete | None = None,
+        prstTxWarp: PresetTextShape | None = None,
+        scene3d: Scene3D | None = None,
+        extLst: Unused = None,
+        noAutofit: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        normAutofit: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        spAutoFit: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        flatTx: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
     ) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/formatting/formatting.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/formatting/formatting.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/formatting/rule.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/formatting/rule.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/formula/tokenizer.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/formula/tokenizer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/formula/translate.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/formula/translate.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/custom.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/custom.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     _ConvertibleToInt,
 )
 from openpyxl.descriptors.nested import NestedText
 
 _T = TypeVar("_T")
 
 # Does not reimplement anything, so runtime also has incompatible supertypes
-class NestedBoolText(Bool[Incomplete], NestedText): ...  # type: ignore[misc]
+class NestedBoolText(Bool[Incomplete], NestedText[Incomplete, Incomplete]): ...  # type: ignore[misc]
 
 class _TypedProperty(Strict, Generic[_T]):
     name: String[Literal[False]]
     # Since this is internal, just list all possible values
     value: Integer[Literal[False]] | Float[Literal[False]] | String[Literal[True]] | DateTime[Literal[False]] | Bool[
         Literal[False]
     ] | String[Literal[False]]
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/manifest.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/manifest.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/relationship.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/relationship.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/packaging/workbook.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/packaging/workbook.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from _typeshed import Incomplete, Unused
 from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
 from openpyxl.descriptors.base import Alias, Bool, Integer, NoneSet, String, Typed, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.nested import NestedString
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.workbook.defined_name import DefinedNameList
 from openpyxl.workbook.function_group import FunctionGroupList
 from openpyxl.workbook.properties import CalcProperties, FileVersion, WorkbookProperties
 from openpyxl.workbook.protection import FileSharing, WorkbookProtection
 from openpyxl.workbook.smart_tags import SmartTagList, SmartTagProperties
 from openpyxl.workbook.web import WebPublishing, WebPublishObjectList
@@ -59,39 +60,39 @@
     workbookProtection: Typed[WorkbookProtection, Literal[True]]
     bookViews: Incomplete
     sheets: Incomplete
     functionGroups: Typed[FunctionGroupList, Literal[True]]
     externalReferences: Incomplete
     definedNames: Typed[DefinedNameList, Literal[True]]
     calcPr: Typed[CalcProperties, Literal[True]]
-    oleSize: Incomplete
+    oleSize: NestedString[Literal[True]]
     customWorkbookViews: Incomplete
     pivotCaches: Incomplete
     smartTagPr: Typed[SmartTagProperties, Literal[True]]
     smartTagTypes: Typed[SmartTagList, Literal[True]]
     webPublishing: Typed[WebPublishing, Literal[True]]
     fileRecoveryPr: Typed[FileRecoveryProperties, Literal[True]]
     webPublishObjects: Typed[WebPublishObjectList, Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
-    Ignorable: Incomplete
+    Ignorable: NestedString[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     def __init__(
         self,
         conformance: _WorkbookPackageConformance | Literal["none"] | None = None,
         fileVersion: FileVersion | None = None,
         fileSharing: FileSharing | None = None,
         workbookPr: WorkbookProperties | None = None,
         workbookProtection: WorkbookProtection | None = None,
         bookViews=(),
         sheets=(),
         functionGroups: FunctionGroupList | None = None,
         externalReferences=(),
         definedNames: DefinedNameList | None = None,
         calcPr: CalcProperties | None = None,
-        oleSize: Incomplete | None = None,
+        oleSize: object = None,
         customWorkbookViews=(),
         pivotCaches=(),
         smartTagPr: SmartTagProperties | None = None,
         smartTagTypes: SmartTagList | None = None,
         webPublishing: WebPublishing | None = None,
         fileRecoveryPr: FileRecoveryProperties | None = None,
         webPublishObjects: WebPublishObjectList | None = None,
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/cache.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/cache.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     String,
     Typed,
     _ConvertibleToBool,
     _ConvertibleToFloat,
     _ConvertibleToInt,
 )
 from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.nested import NestedInteger, _HasTagAndGet
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.pivot.fields import Error, Missing, Number, Text, TupleList
 from openpyxl.pivot.table import PivotArea
 
 _RangePrGroupBy: TypeAlias = Literal["range", "seconds", "minutes", "hours", "days", "months", "quarters", "years"]
 _CacheSourceType: TypeAlias = Literal["worksheet", "external", "consolidation", "scenario"]
 
@@ -382,17 +383,19 @@
     def __init__(self, count: Incomplete | None = None, m=(), n=(), b=(), e=(), s=(), d=()) -> None: ...
     @property
     def count(self): ...
 
 class DiscretePr(Serialisable):
     tagname: str
     count: Integer[Literal[False]]
-    x: Incomplete
+    x: NestedInteger[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: _ConvertibleToInt, x: Incomplete | None = None) -> None: ...
+    def __init__(
+        self, count: _ConvertibleToInt, x: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None
+    ) -> None: ...
 
 class RangePr(Serialisable):
     tagname: str
     autoStart: Bool[Literal[True]]
     autoEnd: Bool[Literal[True]]
     groupBy: Set[_RangePrGroupBy]
     startNum: Float[Literal[True]]
@@ -472,15 +475,15 @@
     @property
     def count(self): ...
 
 class CacheField(Serialisable):
     tagname: str
     sharedItems: Typed[SharedItems, Literal[True]]
     fieldGroup: Typed[FieldGroup, Literal[True]]
-    mpMap: Incomplete
+    mpMap: NestedInteger[Literal[True]]
     extLst: Typed[ExtensionList, Literal[True]]
     name: String[Literal[False]]
     caption: String[Literal[True]]
     propertyName: String[Literal[True]]
     serverField: Bool[Literal[True]]
     uniqueList: Bool[Literal[True]]
     numFmtId: Integer[Literal[True]]
@@ -493,15 +496,15 @@
     memberPropertyField: Bool[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
     @overload
     def __init__(
         self,
         sharedItems: SharedItems | None = None,
         fieldGroup: FieldGroup | None = None,
-        mpMap: Incomplete | None = None,
+        mpMap: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
         extLst: ExtensionList | None = None,
         *,
         name: str,
         caption: str | None = None,
         propertyName: str | None = None,
         serverField: _ConvertibleToBool | None = None,
         uniqueList: _ConvertibleToBool | None = True,
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/fields.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/fields.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/record.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/record.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/pivot/table.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/pivot/table.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/reader/excel.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/reader/excel.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/reader/workbook.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/reader/workbook.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/__init__.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/alignment.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/alignment.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/borders.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/web.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,86 +1,84 @@
-from _typeshed import Incomplete
-from typing import ClassVar
+from _typeshed import Incomplete, Unused
+from typing import ClassVar, overload
 from typing_extensions import Literal, TypeAlias
 
-from openpyxl.descriptors.base import Alias, Bool, NoneSet, Typed, _ConvertibleToBool
+from openpyxl.descriptors.base import Bool, Integer, NoneSet, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
 
-_SideStyle: TypeAlias = Literal[
-    "dashDot",
-    "dashDotDot",
-    "dashed",
-    "dotted",
-    "double",
-    "hair",
-    "medium",
-    "mediumDashDot",
-    "mediumDashDotDot",
-    "mediumDashed",
-    "slantDashDot",
-    "thick",
-    "thin",
+_WebPublishingTargetScreenSize: TypeAlias = Literal[
+    "544x376",
+    "640x480",
+    "720x512",
+    "800x600",
+    "1024x768",
+    "1152x882",
+    "1152x900",
+    "1280x1024",
+    "1600x1200",
+    "1800x1440",
+    "1920x1200",
 ]
 
-BORDER_NONE: Incomplete
-BORDER_DASHDOT: str
-BORDER_DASHDOTDOT: str
-BORDER_DASHED: str
-BORDER_DOTTED: str
-BORDER_DOUBLE: str
-BORDER_HAIR: str
-BORDER_MEDIUM: str
-BORDER_MEDIUMDASHDOT: str
-BORDER_MEDIUMDASHDOTDOT: str
-BORDER_MEDIUMDASHED: str
-BORDER_SLANTDASHDOT: str
-BORDER_THICK: str
-BORDER_THIN: str
-
-class Side(Serialisable):
-    __fields__: Incomplete
-    color: Incomplete
-    style: NoneSet[_SideStyle]
-    border_style: Alias
+class WebPublishObject(Serialisable):
+    tagname: str
+    id: Integer[Literal[False]]
+    divId: String[Literal[False]]
+    sourceObject: String[Literal[True]]
+    destinationFile: String[Literal[False]]
+    title: String[Literal[True]]
+    autoRepublish: Bool[Literal[True]]
+    @overload
+    def __init__(
+        self,
+        id: _ConvertibleToInt,
+        divId: str,
+        sourceObject: str | None = None,
+        *,
+        destinationFile: str,
+        title: str | None = None,
+        autoRepublish: _ConvertibleToBool | None = None,
+    ) -> None: ...
+    @overload
     def __init__(
         self,
-        style: _SideStyle | Literal["none"] | None = None,
-        color: Incomplete | None = None,
-        border_style: Incomplete | None = None,
+        id: _ConvertibleToInt,
+        divId: str,
+        sourceObject: str | None,
+        destinationFile: str,
+        title: str | None = None,
+        autoRepublish: _ConvertibleToBool | None = None,
     ) -> None: ...
 
-class Border(Serialisable):
+class WebPublishObjectList(Serialisable):
     tagname: str
-    __fields__: Incomplete
+    # Overwritten by property below
+    # count: Integer
+    webPublishObject: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    start: Typed[Side, Literal[True]]
-    end: Typed[Side, Literal[True]]
-    left: Typed[Side, Literal[True]]
-    right: Typed[Side, Literal[True]]
-    top: Typed[Side, Literal[True]]
-    bottom: Typed[Side, Literal[True]]
-    diagonal: Typed[Side, Literal[True]]
-    vertical: Typed[Side, Literal[True]]
-    horizontal: Typed[Side, Literal[True]]
-    outline: Bool[Literal[False]]
-    diagonalUp: Bool[Literal[False]]
-    diagonalDown: Bool[Literal[False]]
-    diagonal_direction: Incomplete
+    def __init__(self, count: Unused = None, webPublishObject=()) -> None: ...
+    @property
+    def count(self): ...
+
+class WebPublishing(Serialisable):
+    tagname: str
+    css: Bool[Literal[True]]
+    thicket: Bool[Literal[True]]
+    longFileNames: Bool[Literal[True]]
+    vml: Bool[Literal[True]]
+    allowPng: Bool[Literal[True]]
+    targetScreenSize: NoneSet[_WebPublishingTargetScreenSize]
+    dpi: Integer[Literal[True]]
+    codePage: Integer[Literal[True]]
+    characterSet: String[Literal[True]]
     def __init__(
         self,
-        left: Side | None = None,
-        right: Side | None = None,
-        top: Side | None = None,
-        bottom: Side | None = None,
-        diagonal: Side | None = None,
-        diagonal_direction: Incomplete | None = None,
-        vertical: Side | None = None,
-        horizontal: Side | None = None,
-        diagonalUp: _ConvertibleToBool = False,
-        diagonalDown: _ConvertibleToBool = False,
-        outline: _ConvertibleToBool = True,
-        start: Side | None = None,
-        end: Side | None = None,
+        css: _ConvertibleToBool | None = None,
+        thicket: _ConvertibleToBool | None = None,
+        longFileNames: _ConvertibleToBool | None = None,
+        vml: _ConvertibleToBool | None = None,
+        allowPng: _ConvertibleToBool | None = None,
+        targetScreenSize: _WebPublishingTargetScreenSize | Literal["none"] | None = "800x600",
+        dpi: _ConvertibleToInt | None = None,
+        codePage: _ConvertibleToInt | None = None,
+        characterSet: str | None = None,
     ) -> None: ...
-    def __iter__(self): ...
-
-DEFAULT_BORDER: Incomplete
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/builtins.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/builtins.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/cell_style.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/protection.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,95 +1,67 @@
-from _typeshed import Incomplete, Unused
-from array import array
+from _typeshed import Incomplete
 from typing import ClassVar
 from typing_extensions import Literal
 
-from openpyxl.descriptors import Strict
-from openpyxl.descriptors.base import Bool, Integer, Typed, _ConvertibleToBool, _ConvertibleToInt
-from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.base import Alias, Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.styles.alignment import Alignment
-from openpyxl.styles.protection import Protection
 
-class ArrayDescriptor:
-    key: Incomplete
-    def __init__(self, key) -> None: ...
-    def __get__(self, instance: Serialisable | Strict, cls: Unused): ...
-    def __set__(self, instance: Serialisable | Strict, value) -> None: ...
-
-class StyleArray(array[Incomplete]):
-    tagname: str
-    fontId: Incomplete
-    fillId: Incomplete
-    borderId: Incomplete
-    numFmtId: Incomplete
-    protectionId: Incomplete
-    alignmentId: Incomplete
-    pivotButton: Incomplete
-    quotePrefix: Incomplete
-    xfId: Incomplete
-    def __new__(cls, args=[0, 0, 0, 0, 0, 0, 0, 0, 0]): ...
-    def __hash__(self) -> int: ...
-    def __copy__(self): ...
-    def __deepcopy__(self, memo): ...
+class _Protected:
+    def set_password(self, value: str = "", already_hashed: bool = False) -> None: ...
+    @property
+    def password(self): ...
+    @password.setter
+    def password(self, value) -> None: ...
 
-class CellStyle(Serialisable):
+class SheetProtection(Serialisable, _Protected):
     tagname: str
-    numFmtId: Integer[Literal[False]]
-    fontId: Integer[Literal[False]]
-    fillId: Integer[Literal[False]]
-    borderId: Integer[Literal[False]]
-    xfId: Integer[Literal[True]]
-    quotePrefix: Bool[Literal[True]]
-    pivotButton: Bool[Literal[True]]
-    applyNumberFormat: Bool[Literal[True]]
-    applyFont: Bool[Literal[True]]
-    applyFill: Bool[Literal[True]]
-    applyBorder: Bool[Literal[True]]
-    # Overwritten by properties below
-    # applyAlignment: Bool[Literal[True]]
-    # applyProtection: Bool[Literal[True]]
-    alignment: Typed[Alignment, Literal[True]]
-    protection: Typed[Protection, Literal[True]]
-    extLst: Typed[ExtensionList, Literal[True]]
-    __elements__: ClassVar[tuple[str, ...]]
+    sheet: Bool[Literal[False]]
+    enabled: Alias
+    objects: Bool[Literal[False]]
+    scenarios: Bool[Literal[False]]
+    formatCells: Bool[Literal[False]]
+    formatColumns: Bool[Literal[False]]
+    formatRows: Bool[Literal[False]]
+    insertColumns: Bool[Literal[False]]
+    insertRows: Bool[Literal[False]]
+    insertHyperlinks: Bool[Literal[False]]
+    deleteColumns: Bool[Literal[False]]
+    deleteRows: Bool[Literal[False]]
+    selectLockedCells: Bool[Literal[False]]
+    selectUnlockedCells: Bool[Literal[False]]
+    sort: Bool[Literal[False]]
+    autoFilter: Bool[Literal[False]]
+    pivotTables: Bool[Literal[False]]
+    saltValue: Incomplete
+    spinCount: Integer[Literal[True]]
+    algorithmName: String[Literal[True]]
+    hashValue: Incomplete
     __attrs__: ClassVar[tuple[str, ...]]
+    password: Incomplete
     def __init__(
         self,
-        numFmtId: _ConvertibleToInt = 0,
-        fontId: _ConvertibleToInt = 0,
-        fillId: _ConvertibleToInt = 0,
-        borderId: _ConvertibleToInt = 0,
-        xfId: _ConvertibleToInt | None = None,
-        quotePrefix: _ConvertibleToBool | None = None,
-        pivotButton: _ConvertibleToBool | None = None,
-        applyNumberFormat: _ConvertibleToBool | None = None,
-        applyFont: _ConvertibleToBool | None = None,
-        applyFill: _ConvertibleToBool | None = None,
-        applyBorder: _ConvertibleToBool | None = None,
-        applyAlignment: Unused = None,
-        applyProtection: Unused = None,
-        alignment: Alignment | None = None,
-        protection: Protection | None = None,
-        extLst: Unused = None,
+        sheet: _ConvertibleToBool = False,
+        objects: _ConvertibleToBool = False,
+        scenarios: _ConvertibleToBool = False,
+        formatCells: _ConvertibleToBool = True,
+        formatRows: _ConvertibleToBool = True,
+        formatColumns: _ConvertibleToBool = True,
+        insertColumns: _ConvertibleToBool = True,
+        insertRows: _ConvertibleToBool = True,
+        insertHyperlinks: _ConvertibleToBool = True,
+        deleteColumns: _ConvertibleToBool = True,
+        deleteRows: _ConvertibleToBool = True,
+        selectLockedCells: _ConvertibleToBool = False,
+        selectUnlockedCells: _ConvertibleToBool = False,
+        sort: _ConvertibleToBool = True,
+        autoFilter: _ConvertibleToBool = True,
+        pivotTables: _ConvertibleToBool = True,
+        password: Incomplete | None = None,
+        algorithmName: str | None = None,
+        saltValue: Incomplete | None = None,
+        spinCount: _ConvertibleToInt | None = None,
+        hashValue: Incomplete | None = None,
     ) -> None: ...
-    def to_array(self): ...
-    @classmethod
-    def from_array(cls, style): ...
-    @property
-    def applyProtection(self): ...
-    @property
-    def applyAlignment(self): ...
-
-class CellStyleList(Serialisable):
-    tagname: str
-    __attrs__: ClassVar[tuple[str, ...]]
-    # Overwritten by property below
-    # count: Integer
-    xf: Incomplete
-    alignment: Incomplete
-    protection: Incomplete
-    __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: Unused = None, xf=()) -> None: ...
-    @property
-    def count(self): ...
-    def __getitem__(self, idx): ...
+    def set_password(self, value: str = "", already_hashed: bool = False) -> None: ...
+    def enable(self) -> None: ...
+    def disable(self) -> None: ...
+    def __bool__(self) -> bool: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/colors.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/colors.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/differential.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/smart_tag.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 from _typeshed import Incomplete
-from typing import ClassVar
+from typing import ClassVar, overload
 from typing_extensions import Literal
 
-from openpyxl.descriptors.base import Alias, Typed
-from openpyxl.descriptors.excel import ExtensionList
+from openpyxl.descriptors.base import Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
 from openpyxl.descriptors.serialisable import Serialisable
-from openpyxl.styles import Alignment, Border, Fill, Font, Protection
-from openpyxl.styles.numbers import NumberFormat
 
-class DifferentialStyle(Serialisable):
+class CellSmartTagPr(Serialisable):
     tagname: str
+    key: String[Literal[False]]
+    val: String[Literal[False]]
+    def __init__(self, key: str, val: str) -> None: ...
+
+class CellSmartTag(Serialisable):
+    tagname: str
+    cellSmartTagPr: Incomplete
+    type: Integer[Literal[False]]
+    deleted: Bool[Literal[True]]
+    xmlBased: Bool[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    font: Typed[Font, Literal[True]]
-    numFmt: Typed[NumberFormat, Literal[True]]
-    fill: Typed[Fill, Literal[True]]
-    alignment: Typed[Alignment, Literal[True]]
-    border: Typed[Border, Literal[True]]
-    protection: Typed[Protection, Literal[True]]
-    extLst: ExtensionList | None
+    @overload
+    def __init__(
+        self,
+        cellSmartTagPr=(),
+        *,
+        type: _ConvertibleToInt,
+        deleted: _ConvertibleToBool | None = False,
+        xmlBased: _ConvertibleToBool | None = False,
+    ) -> None: ...
+    @overload
     def __init__(
         self,
-        font: Font | None = None,
-        numFmt: NumberFormat | None = None,
-        fill: Fill | None = None,
-        alignment: Alignment | None = None,
-        border: Border | None = None,
-        protection: Protection | None = None,
-        extLst: ExtensionList | None = None,
+        cellSmartTagPr,
+        type: _ConvertibleToInt,
+        deleted: _ConvertibleToBool | None = False,
+        xmlBased: _ConvertibleToBool | None = False,
     ) -> None: ...
 
-class DifferentialStyleList(Serialisable):
+class CellSmartTags(Serialisable):
     tagname: str
-    dxf: Incomplete
-    styles: Alias
-    __attrs__: ClassVar[tuple[str, ...]]
-    def __init__(self, dxf=(), count: Incomplete | None = None) -> None: ...
-    def append(self, dxf) -> None: ...
-    def add(self, dxf): ...
-    def __bool__(self) -> bool: ...
-    def __getitem__(self, idx): ...
-    @property
-    def count(self): ...
+    cellSmartTag: Incomplete
+    r: String[Literal[False]]
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, cellSmartTag, r: str) -> None: ...
+
+class SmartTags(Serialisable):
+    tagname: str
+    cellSmartTags: Incomplete
+    __elements__: ClassVar[tuple[str, ...]]
+    def __init__(self, cellSmartTags=()) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/fills.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/fills.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/named_styles.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/named_styles.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/numbers.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/numbers.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/styleable.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/styleable.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/stylesheet.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/stylesheet.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/styles/table.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/table.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/utils/cell.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/utils/cell.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/utils/datetime.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/utils/datetime.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/utils/units.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/utils/units.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/_writer.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/_writer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/child.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/child.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/defined_name.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/defined_name.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/function_group.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/function_group.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/properties.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/properties.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/protection.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/protection.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/smart_tags.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/smart_tags.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/views.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/views.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/web.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/styles/fonts.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,75 @@
-from _typeshed import Incomplete, Unused
-from typing import ClassVar, overload
+from _typeshed import Incomplete
+from typing import ClassVar
 from typing_extensions import Literal, TypeAlias
 
-from openpyxl.descriptors.base import Bool, Integer, NoneSet, String, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import Alias, _ConvertibleToBool, _ConvertibleToFloat, _ConvertibleToInt
+from openpyxl.descriptors.nested import (
+    NestedBool,
+    NestedFloat,
+    NestedInteger,
+    NestedMinMax,
+    NestedNoneSet,
+    NestedString,
+    _HasTagAndGet,
+    _NestedNoneSetParam,
+)
 from openpyxl.descriptors.serialisable import Serialisable
 
-_WebPublishingTargetScreenSize: TypeAlias = Literal[
-    "544x376",
-    "640x480",
-    "720x512",
-    "800x600",
-    "1024x768",
-    "1152x882",
-    "1152x900",
-    "1280x1024",
-    "1600x1200",
-    "1800x1440",
-    "1920x1200",
-]
+_FontU: TypeAlias = Literal["single", "double", "singleAccounting", "doubleAccounting"]
+_FontVertAlign: TypeAlias = Literal["superscript", "subscript", "baseline"]
+_FontScheme: TypeAlias = Literal["major", "minor"]
 
-class WebPublishObject(Serialisable):
+class Font(Serialisable):
+    UNDERLINE_DOUBLE: str
+    UNDERLINE_DOUBLE_ACCOUNTING: str
+    UNDERLINE_SINGLE: str
+    UNDERLINE_SINGLE_ACCOUNTING: str
+    name: NestedString[Literal[True]]
+    charset: NestedInteger[Literal[True]]
+    family: NestedMinMax[float, Literal[True]]
+    sz: NestedFloat[Literal[True]]
+    size: Alias
+    b: NestedBool[Literal[False]]
+    bold: Alias
+    i: NestedBool[Literal[False]]
+    italic: Alias
+    strike: NestedBool[Literal[True]]
+    strikethrough: Alias
+    outline: NestedBool[Literal[True]]
+    shadow: NestedBool[Literal[True]]
+    condense: NestedBool[Literal[True]]
+    extend: NestedBool[Literal[True]]
+    u: NestedNoneSet[_FontU]
+    underline: Alias
+    vertAlign: NestedNoneSet[_FontVertAlign]
+    color: Incomplete
+    scheme: NestedNoneSet[_FontScheme]
     tagname: str
-    id: Integer[Literal[False]]
-    divId: String[Literal[False]]
-    sourceObject: String[Literal[True]]
-    destinationFile: String[Literal[False]]
-    title: String[Literal[True]]
-    autoRepublish: Bool[Literal[True]]
-    @overload
-    def __init__(
-        self,
-        id: _ConvertibleToInt,
-        divId: str,
-        sourceObject: str | None = None,
-        *,
-        destinationFile: str,
-        title: str | None = None,
-        autoRepublish: _ConvertibleToBool | None = None,
-    ) -> None: ...
-    @overload
-    def __init__(
-        self,
-        id: _ConvertibleToInt,
-        divId: str,
-        sourceObject: str | None,
-        destinationFile: str,
-        title: str | None = None,
-        autoRepublish: _ConvertibleToBool | None = None,
-    ) -> None: ...
-
-class WebPublishObjectList(Serialisable):
-    tagname: str
-    # Overwritten by property below
-    # count: Integer
-    webPublishObject: Incomplete
     __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, count: Unused = None, webPublishObject=()) -> None: ...
-    @property
-    def count(self): ...
-
-class WebPublishing(Serialisable):
-    tagname: str
-    css: Bool[Literal[True]]
-    thicket: Bool[Literal[True]]
-    longFileNames: Bool[Literal[True]]
-    vml: Bool[Literal[True]]
-    allowPng: Bool[Literal[True]]
-    targetScreenSize: NoneSet[_WebPublishingTargetScreenSize]
-    dpi: Integer[Literal[True]]
-    codePage: Integer[Literal[True]]
-    characterSet: String[Literal[True]]
     def __init__(
         self,
-        css: _ConvertibleToBool | None = None,
-        thicket: _ConvertibleToBool | None = None,
-        longFileNames: _ConvertibleToBool | None = None,
-        vml: _ConvertibleToBool | None = None,
-        allowPng: _ConvertibleToBool | None = None,
-        targetScreenSize: _WebPublishingTargetScreenSize | Literal["none"] | None = "800x600",
-        dpi: _ConvertibleToInt | None = None,
-        codePage: _ConvertibleToInt | None = None,
-        characterSet: str | None = None,
+        name: object = None,
+        sz: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        b: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        i: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool = None,
+        charset: _HasTagAndGet[_ConvertibleToInt | None] | _ConvertibleToInt | None = None,
+        u: _NestedNoneSetParam[_FontU] = None,
+        strike: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        color: Incomplete | None = None,
+        scheme: _NestedNoneSetParam[_FontScheme] = None,
+        family: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
+        size: _HasTagAndGet[_ConvertibleToFloat] | _ConvertibleToFloat | None = None,
+        bold: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool | None = None,
+        italic: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool | None = None,
+        strikethrough: _HasTagAndGet[_ConvertibleToBool] | _ConvertibleToBool | None = None,
+        underline: _NestedNoneSetParam[_FontU] = None,
+        vertAlign: _NestedNoneSetParam[_FontVertAlign] = None,
+        outline: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        shadow: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        condense: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        extend: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
     ) -> None: ...
+    @classmethod
+    def from_tree(cls, node): ...
+
+DEFAULT_FONT: Incomplete
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/workbook/workbook.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/workbook/workbook.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_read_only.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/_read_only.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_reader.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/_reader.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_write_only.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/_write_only.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/_writer.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/_writer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/cell_range.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/cell_range.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/controls.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/controls.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/custom.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/custom.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/datavalidation.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/datavalidation.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Integer,
     NoneSet,
     String,
     _ConvertibleToBool,
     _ConvertibleToInt,
     _ConvertibleToMultiCellRange,
 )
+from openpyxl.descriptors.nested import NestedText
 from openpyxl.descriptors.serialisable import Serialisable
 from openpyxl.worksheet.cell_range import MultiCellRange
 
 _DataValidationType: TypeAlias = Literal["whole", "decimal", "list", "date", "time", "textLength", "custom"]
 _DataValidationErrorStyle: TypeAlias = Literal["stop", "warning", "information"]
 _DataValidationImeMode: TypeAlias = Literal[
     "noControl",
@@ -49,26 +50,26 @@
     showErrorMessage: Bool[Literal[True]]
     allowBlank: Bool[Literal[True]]
     allow_blank: Alias
     errorTitle: String[Literal[True]]
     error: String[Literal[True]]
     promptTitle: String[Literal[True]]
     prompt: String[Literal[True]]
-    formula1: Incomplete
-    formula2: Incomplete
+    formula1: NestedText[str, Literal[True]]
+    formula2: NestedText[str, Literal[True]]
     type: NoneSet[_DataValidationType]
     errorStyle: NoneSet[_DataValidationErrorStyle]
     imeMode: NoneSet[_DataValidationImeMode]
     operator: NoneSet[_DataValidationOperator]
     validation_type: Alias
     def __init__(
         self,
         type: _DataValidationType | Literal["none"] | None = None,
-        formula1: Incomplete | None = None,
-        formula2: Incomplete | None = None,
+        formula1: object = None,
+        formula2: object = None,
         showErrorMessage: _ConvertibleToBool | None = False,
         showInputMessage: _ConvertibleToBool | None = False,
         showDropDown: _ConvertibleToBool | None = False,
         allowBlank: _ConvertibleToBool | None = False,
         sqref: _ConvertibleToMultiCellRange = (),
         promptTitle: str | None = None,
         errorStyle: _DataValidationErrorStyle | Literal["none"] | None = None,
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/dimensions.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/dimensions.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/filters.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/filters.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/formula.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/formula.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/header_footer.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/header_footer.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/hyperlink.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/hyperlink.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/merge.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/merge.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/ole.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/ole.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/page.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/page.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/pagebreak.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/pagebreak.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/print_settings.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/print_settings.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/properties.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/properties.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/scenario.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/scenario.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/smart_tag.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/chart/picture.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,25 @@
-from _typeshed import Incomplete
-from typing import ClassVar, overload
-from typing_extensions import Literal
+from typing import ClassVar
+from typing_extensions import Literal, TypeAlias
 
-from openpyxl.descriptors.base import Bool, Integer, String, _ConvertibleToBool, _ConvertibleToInt
+from openpyxl.descriptors.base import _ConvertibleToBool, _ConvertibleToFloat
+from openpyxl.descriptors.nested import NestedBool, NestedFloat, NestedNoneSet, _HasTagAndGet, _NestedNoneSetParam
 from openpyxl.descriptors.serialisable import Serialisable
 
-class CellSmartTagPr(Serialisable):
-    tagname: str
-    key: String[Literal[False]]
-    val: String[Literal[False]]
-    def __init__(self, key: str, val: str) -> None: ...
+_PictureOptionsPictureFormat: TypeAlias = Literal["stretch", "stack", "stackScale"]
 
-class CellSmartTag(Serialisable):
+class PictureOptions(Serialisable):
     tagname: str
-    cellSmartTagPr: Incomplete
-    type: Integer[Literal[False]]
-    deleted: Bool[Literal[True]]
-    xmlBased: Bool[Literal[True]]
+    applyToFront: NestedBool[Literal[True]]
+    applyToSides: NestedBool[Literal[True]]
+    applyToEnd: NestedBool[Literal[True]]
+    pictureFormat: NestedNoneSet[_PictureOptionsPictureFormat]
+    pictureStackUnit: NestedFloat[Literal[True]]
     __elements__: ClassVar[tuple[str, ...]]
-    @overload
     def __init__(
         self,
-        cellSmartTagPr=(),
-        *,
-        type: _ConvertibleToInt,
-        deleted: _ConvertibleToBool | None = False,
-        xmlBased: _ConvertibleToBool | None = False,
+        applyToFront: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        applyToSides: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        applyToEnd: _HasTagAndGet[_ConvertibleToBool | None] | _ConvertibleToBool | None = None,
+        pictureFormat: _NestedNoneSetParam[_PictureOptionsPictureFormat] = None,
+        pictureStackUnit: _HasTagAndGet[_ConvertibleToFloat | None] | _ConvertibleToFloat | None = None,
     ) -> None: ...
-    @overload
-    def __init__(
-        self,
-        cellSmartTagPr,
-        type: _ConvertibleToInt,
-        deleted: _ConvertibleToBool | None = False,
-        xmlBased: _ConvertibleToBool | None = False,
-    ) -> None: ...
-
-class CellSmartTags(Serialisable):
-    tagname: str
-    cellSmartTag: Incomplete
-    r: String[Literal[False]]
-    __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, cellSmartTag, r: str) -> None: ...
-
-class SmartTags(Serialisable):
-    tagname: str
-    cellSmartTags: Incomplete
-    __elements__: ClassVar[tuple[str, ...]]
-    def __init__(self, cellSmartTags=()) -> None: ...
```

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/table.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/table.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/views.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/views.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/worksheet/worksheet.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/worksheet/worksheet.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/openpyxl-stubs/xml/constants.pyi` & `types-openpyxl-3.1.0.9/openpyxl-stubs/xml/constants.pyi`

 * *Files identical despite different names*

### Comparing `types-openpyxl-3.1.0.8/setup.py` & `types-openpyxl-3.1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,33 +11,37 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `openpyxl`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/openpyxl. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2d5dafadb75f122e0c2aeced09a5b72232373f40`.
+This package was generated from typeshed commit `8c582c4459cc3e7c67531cd90bfd6cef5b71c7d3`.
 '''.lstrip()
 
 setup(name=name,
-      version="3.1.0.8",
+      version="3.1.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/openpyxl.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['openpyxl-stubs'],
-      package_data={'openpyxl-stubs': ['__init__.pyi', '_constants.pyi', 'cell/__init__.pyi', 'cell/_writer.pyi', 'cell/cell.pyi', 'cell/read_only.pyi', 'cell/rich_text.pyi', 'cell/text.pyi', 'chart/_3d.pyi', 'chart/__init__.pyi', 'chart/_chart.pyi', 'chart/area_chart.pyi', 'chart/axis.pyi', 'chart/bar_chart.pyi', 'chart/bubble_chart.pyi', 'chart/chartspace.pyi', 'chart/data_source.pyi', 'chart/descriptors.pyi', 'chart/error_bar.pyi', 'chart/label.pyi', 'chart/layout.pyi', 'chart/legend.pyi', 'chart/line_chart.pyi', 'chart/marker.pyi', 'chart/picture.pyi', 'chart/pie_chart.pyi', 'chart/pivot.pyi', 'chart/plotarea.pyi', 'chart/print_settings.pyi', 'chart/radar_chart.pyi', 'chart/reader.pyi', 'chart/reference.pyi', 'chart/scatter_chart.pyi', 'chart/series.pyi', 'chart/series_factory.pyi', 'chart/shapes.pyi', 'chart/stock_chart.pyi', 'chart/surface_chart.pyi', 'chart/text.pyi', 'chart/title.pyi', 'chart/trendline.pyi', 'chart/updown_bars.pyi', 'chartsheet/__init__.pyi', 'chartsheet/chartsheet.pyi', 'chartsheet/custom.pyi', 'chartsheet/properties.pyi', 'chartsheet/protection.pyi', 'chartsheet/publish.pyi', 'chartsheet/relation.pyi', 'chartsheet/views.pyi', 'comments/__init__.pyi', 'comments/author.pyi', 'comments/comment_sheet.pyi', 'comments/comments.pyi', 'comments/shape_writer.pyi', 'compat/__init__.pyi', 'compat/abc.pyi', 'compat/numbers.pyi', 'compat/product.pyi', 'compat/singleton.pyi', 'compat/strings.pyi', 'descriptors/__init__.pyi', 'descriptors/base.pyi', 'descriptors/excel.pyi', 'descriptors/namespace.pyi', 'descriptors/nested.pyi', 'descriptors/sequence.pyi', 'descriptors/serialisable.pyi', 'descriptors/slots.pyi', 'drawing/__init__.pyi', 'drawing/colors.pyi', 'drawing/connector.pyi', 'drawing/drawing.pyi', 'drawing/effect.pyi', 'drawing/fill.pyi', 'drawing/geometry.pyi', 'drawing/graphic.pyi', 'drawing/image.pyi', 'drawing/line.pyi', 'drawing/picture.pyi', 'drawing/properties.pyi', 'drawing/relation.pyi', 'drawing/spreadsheet_drawing.pyi', 'drawing/text.pyi', 'drawing/xdr.pyi', 'formatting/__init__.pyi', 'formatting/formatting.pyi', 'formatting/rule.pyi', 'formula/__init__.pyi', 'formula/tokenizer.pyi', 'formula/translate.pyi', 'packaging/__init__.pyi', 'packaging/core.pyi', 'packaging/custom.pyi', 'packaging/extended.pyi', 'packaging/interface.pyi', 'packaging/manifest.pyi', 'packaging/relationship.pyi', 'packaging/workbook.pyi', 'pivot/__init__.pyi', 'pivot/cache.pyi', 'pivot/fields.pyi', 'pivot/record.pyi', 'pivot/table.pyi', 'reader/__init__.pyi', 'reader/drawings.pyi', 'reader/excel.pyi', 'reader/strings.pyi', 'reader/workbook.pyi', 'styles/__init__.pyi', 'styles/alignment.pyi', 'styles/borders.pyi', 'styles/builtins.pyi', 'styles/cell_style.pyi', 'styles/colors.pyi', 'styles/differential.pyi', 'styles/fills.pyi', 'styles/fonts.pyi', 'styles/named_styles.pyi', 'styles/numbers.pyi', 'styles/protection.pyi', 'styles/proxy.pyi', 'styles/styleable.pyi', 'styles/stylesheet.pyi', 'styles/table.pyi', 'utils/__init__.pyi', 'utils/bound_dictionary.pyi', 'utils/cell.pyi', 'utils/dataframe.pyi', 'utils/datetime.pyi', 'utils/escape.pyi', 'utils/exceptions.pyi', 'utils/formulas.pyi', 'utils/indexed_list.pyi', 'utils/inference.pyi', 'utils/protection.pyi', 'utils/units.pyi', 'workbook/__init__.pyi', 'workbook/_writer.pyi', 'workbook/child.pyi', 'workbook/defined_name.pyi', 'workbook/external_link/__init__.pyi', 'workbook/external_link/external.pyi', 'workbook/external_reference.pyi', 'workbook/function_group.pyi', 'workbook/properties.pyi', 'workbook/protection.pyi', 'workbook/smart_tags.pyi', 'workbook/views.pyi', 'workbook/web.pyi', 'workbook/workbook.pyi', 'worksheet/__init__.pyi', 'worksheet/_read_only.pyi', 'worksheet/_reader.pyi', 'worksheet/_write_only.pyi', 'worksheet/_writer.pyi', 'worksheet/cell_range.pyi', 'worksheet/cell_watch.pyi', 'worksheet/controls.pyi', 'worksheet/copier.pyi', 'worksheet/custom.pyi', 'worksheet/datavalidation.pyi', 'worksheet/dimensions.pyi', 'worksheet/drawing.pyi', 'worksheet/errors.pyi', 'worksheet/filters.pyi', 'worksheet/formula.pyi', 'worksheet/header_footer.pyi', 'worksheet/hyperlink.pyi', 'worksheet/merge.pyi', 'worksheet/ole.pyi', 'worksheet/page.pyi', 'worksheet/pagebreak.pyi', 'worksheet/picture.pyi', 'worksheet/print_settings.pyi', 'worksheet/properties.pyi', 'worksheet/protection.pyi', 'worksheet/related.pyi', 'worksheet/scenario.pyi', 'worksheet/smart_tag.pyi', 'worksheet/table.pyi', 'worksheet/views.pyi', 'worksheet/worksheet.pyi', 'writer/__init__.pyi', 'writer/excel.pyi', 'writer/theme.pyi', 'xml/__init__.pyi', 'xml/constants.pyi', 'xml/functions.pyi', 'METADATA.toml']},
+      package_data={'openpyxl-stubs': ['__init__.pyi', '_constants.pyi', 'cell/__init__.pyi', 'cell/_writer.pyi', 'cell/cell.pyi', 'cell/read_only.pyi', 'cell/rich_text.pyi', 'cell/text.pyi', 'chart/_3d.pyi', 'chart/__init__.pyi', 'chart/_chart.pyi', 'chart/area_chart.pyi', 'chart/axis.pyi', 'chart/bar_chart.pyi', 'chart/bubble_chart.pyi', 'chart/chartspace.pyi', 'chart/data_source.pyi', 'chart/descriptors.pyi', 'chart/error_bar.pyi', 'chart/label.pyi', 'chart/layout.pyi', 'chart/legend.pyi', 'chart/line_chart.pyi', 'chart/marker.pyi', 'chart/picture.pyi', 'chart/pie_chart.pyi', 'chart/pivot.pyi', 'chart/plotarea.pyi', 'chart/print_settings.pyi', 'chart/radar_chart.pyi', 'chart/reader.pyi', 'chart/reference.pyi', 'chart/scatter_chart.pyi', 'chart/series.pyi', 'chart/series_factory.pyi', 'chart/shapes.pyi', 'chart/stock_chart.pyi', 'chart/surface_chart.pyi', 'chart/text.pyi', 'chart/title.pyi', 'chart/trendline.pyi', 'chart/updown_bars.pyi', 'chartsheet/__init__.pyi', 'chartsheet/chartsheet.pyi', 'chartsheet/custom.pyi', 'chartsheet/properties.pyi', 'chartsheet/protection.pyi', 'chartsheet/publish.pyi', 'chartsheet/relation.pyi', 'chartsheet/views.pyi', 'comments/__init__.pyi', 'comments/author.pyi', 'comments/comment_sheet.pyi', 'comments/comments.pyi', 'comments/shape_writer.pyi', 'compat/__init__.pyi', 'compat/abc.pyi', 'compat/numbers.pyi', 'compat/product.pyi', 'compat/singleton.pyi', 'compat/strings.pyi', 'descriptors/__init__.pyi', 'descriptors/base.pyi', 'descriptors/excel.pyi', 'descriptors/namespace.pyi', 'descriptors/nested.pyi', 'descriptors/sequence.pyi', 'descriptors/serialisable.pyi', 'descriptors/slots.pyi', 'drawing/__init__.pyi', 'drawing/colors.pyi', 'drawing/connector.pyi', 'drawing/drawing.pyi', 'drawing/effect.pyi', 'drawing/fill.pyi', 'drawing/geometry.pyi', 'drawing/graphic.pyi', 'drawing/image.pyi', 'drawing/line.pyi', 'drawing/picture.pyi', 'drawing/properties.pyi', 'drawing/relation.pyi', 'drawing/spreadsheet_drawing.pyi', 'drawing/text.pyi', 'drawing/xdr.pyi', 'formatting/__init__.pyi', 'formatting/formatting.pyi', 'formatting/rule.pyi', 'formula/__init__.pyi', 'formula/tokenizer.pyi', 'formula/translate.pyi', 'packaging/__init__.pyi', 'packaging/core.pyi', 'packaging/custom.pyi', 'packaging/extended.pyi', 'packaging/interface.pyi', 'packaging/manifest.pyi', 'packaging/relationship.pyi', 'packaging/workbook.pyi', 'pivot/__init__.pyi', 'pivot/cache.pyi', 'pivot/fields.pyi', 'pivot/record.pyi', 'pivot/table.pyi', 'reader/__init__.pyi', 'reader/drawings.pyi', 'reader/excel.pyi', 'reader/strings.pyi', 'reader/workbook.pyi', 'styles/__init__.pyi', 'styles/alignment.pyi', 'styles/borders.pyi', 'styles/builtins.pyi', 'styles/cell_style.pyi', 'styles/colors.pyi', 'styles/differential.pyi', 'styles/fills.pyi', 'styles/fonts.pyi', 'styles/named_styles.pyi', 'styles/numbers.pyi', 'styles/protection.pyi', 'styles/proxy.pyi', 'styles/styleable.pyi', 'styles/stylesheet.pyi', 'styles/table.pyi', 'utils/__init__.pyi', 'utils/bound_dictionary.pyi', 'utils/cell.pyi', 'utils/dataframe.pyi', 'utils/datetime.pyi', 'utils/escape.pyi', 'utils/exceptions.pyi', 'utils/formulas.pyi', 'utils/indexed_list.pyi', 'utils/inference.pyi', 'utils/protection.pyi', 'utils/units.pyi', 'workbook/__init__.pyi', 'workbook/_writer.pyi', 'workbook/child.pyi', 'workbook/defined_name.pyi', 'workbook/external_link/__init__.pyi', 'workbook/external_link/external.pyi', 'workbook/external_reference.pyi', 'workbook/function_group.pyi', 'workbook/properties.pyi', 'workbook/protection.pyi', 'workbook/smart_tags.pyi', 'workbook/views.pyi', 'workbook/web.pyi', 'workbook/workbook.pyi', 'worksheet/__init__.pyi', 'worksheet/_read_only.pyi', 'worksheet/_reader.pyi', 'worksheet/_write_only.pyi', 'worksheet/_writer.pyi', 'worksheet/cell_range.pyi', 'worksheet/cell_watch.pyi', 'worksheet/controls.pyi', 'worksheet/copier.pyi', 'worksheet/custom.pyi', 'worksheet/datavalidation.pyi', 'worksheet/dimensions.pyi', 'worksheet/drawing.pyi', 'worksheet/errors.pyi', 'worksheet/filters.pyi', 'worksheet/formula.pyi', 'worksheet/header_footer.pyi', 'worksheet/hyperlink.pyi', 'worksheet/merge.pyi', 'worksheet/ole.pyi', 'worksheet/page.pyi', 'worksheet/pagebreak.pyi', 'worksheet/picture.pyi', 'worksheet/print_settings.pyi', 'worksheet/properties.pyi', 'worksheet/protection.pyi', 'worksheet/related.pyi', 'worksheet/scenario.pyi', 'worksheet/smart_tag.pyi', 'worksheet/table.pyi', 'worksheet/views.pyi', 'worksheet/worksheet.pyi', 'writer/__init__.pyi', 'writer/excel.pyi', 'writer/theme.pyi', 'xml/__init__.pyi', 'xml/constants.pyi', 'xml/functions.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-openpyxl-3.1.0.8/types_openpyxl.egg-info/PKG-INFO` & `types-openpyxl-3.1.0.9/types_openpyxl.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-openpyxl
-Version: 3.1.0.8
+Version: 3.1.0.9
 Summary: Typing stubs for openpyxl
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/openpyxl.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,13 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `openpyxl`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/openpyxl. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2d5dafadb75f122e0c2aeced09a5b72232373f40`.
+This package was generated from typeshed commit `8c582c4459cc3e7c67531cd90bfd6cef5b71c7d3`.
```

### Comparing `types-openpyxl-3.1.0.8/types_openpyxl.egg-info/SOURCES.txt` & `types-openpyxl-3.1.0.9/types_openpyxl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

