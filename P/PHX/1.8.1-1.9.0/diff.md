# Comparing `tmp/PHX-1.8.1.tar.gz` & `tmp/PHX-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PHX-1.8.1.tar", last modified: Wed Mar 15 20:09:23 2023, max compression
+gzip compressed data, was "dist/PHX-1.9.0.tar", last modified: Thu Mar 16 08:56:36 2023, max compression
```

## Comparing `PHX-1.8.1.tar` & `PHX-1.9.0.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/.github/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/.github/workflows/
--rw-r--r--   0 runner     (501) staff       (20)     1865 2023-03-15 20:07:35.000000 PHX-1.8.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner     (501) staff       (20)    35129 2023-03-15 20:07:35.000000 PHX-1.8.1/LICENSE
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/PHPP/
--rw-r--r--   0 runner     (501) staff       (20)     1064 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/README.md
--rw-r--r--   0 runner     (501) staff       (20)       34 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    35984 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_app.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/PHPP/phpp_localization/
--rw-r--r--   0 runner     (501) staff       (20)    40141 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_localization/EN_10_3.json
--rw-r--r--   0 runner     (501) staff       (20)    40150 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_localization/EN_10_4A.json
--rw-r--r--   0 runner     (501) staff       (20)    39587 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_localization/EN_9_6A.json
--rw-r--r--   0 runner     (501) staff       (20)    39830 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_localization/EN_9_7IP.json
--rw-r--r--   0 runner     (501) staff       (20)       99 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_localization/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1682 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_localization/load.py
--rw-r--r--   0 runner     (501) staff       (20)    20844 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_localization/shape_model.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/PHPP/phpp_model/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1292 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/areas_data.py
--rw-r--r--   0 runner     (501) staff       (20)     3365 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/areas_surface.py
--rw-r--r--   0 runner     (501) staff       (20)     2304 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/areas_thermal_bridges.py
--rw-r--r--   0 runner     (501) staff       (20)     6008 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/climate_entry.py
--rw-r--r--   0 runner     (501) staff       (20)     5361 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/component_frame.py
--rw-r--r--   0 runner     (501) staff       (20)     2117 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/component_glazing.py
--rw-r--r--   0 runner     (501) staff       (20)     2522 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/component_vent.py
--rw-r--r--   0 runner     (501) staff       (20)     8328 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/electricity_item.py
--rw-r--r--   0 runner     (501) staff       (20)     4985 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/hot_water_piping.py
--rw-r--r--   0 runner     (501) staff       (20)     3167 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/hot_water_tank.py
--rw-r--r--   0 runner     (501) staff       (20)     3230 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/shading_rows.py
--rw-r--r--   0 runner     (501) staff       (20)     3937 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/uvalues_constructor.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/vent_ducts.py
--rw-r--r--   0 runner     (501) staff       (20)     6134 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/vent_space.py
--rw-r--r--   0 runner     (501) staff       (20)     2216 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/vent_units.py
--rw-r--r--   0 runner     (501) staff       (20)     2855 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/ventilation_data.py
--rw-r--r--   0 runner     (501) staff       (20)     2038 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/verification_data.py
--rw-r--r--   0 runner     (501) staff       (20)      758 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/version.py
--rw-r--r--   0 runner     (501) staff       (20)     3569 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/phpp_model/windows_rows.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/PHPP/sheet_io/
--rw-r--r--   0 runner     (501) staff       (20)      968 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12017 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_PER.py
--rw-r--r--   0 runner     (501) staff       (20)    13415 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_addnl_vent.py
--rw-r--r--   0 runner     (501) staff       (20)    11232 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_areas.py
--rw-r--r--   0 runner     (501) staff       (20)     1422 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_climate.py
--rw-r--r--   0 runner     (501) staff       (20)    10999 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_components.py
--rw-r--r--   0 runner     (501) staff       (20)     3682 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_cooling_demand.py
--rw-r--r--   0 runner     (501) staff       (20)     2622 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_cooling_peak_load.py
--rw-r--r--   0 runner     (501) staff       (20)      612 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_elec_non_res.py
--rw-r--r--   0 runner     (501) staff       (20)     1596 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_electricity.py
--rw-r--r--   0 runner     (501) staff       (20)     1247 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)     3033 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_heating_demand.py
--rw-r--r--   0 runner     (501) staff       (20)     2836 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_heating_peak_load.py
--rw-r--r--   0 runner     (501) staff       (20)     7542 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_hot_water.py
--rw-r--r--   0 runner     (501) staff       (20)      594 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_ihg_non_res.py
--rw-r--r--   0 runner     (501) staff       (20)     5279 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_overview.py
--rw-r--r--   0 runner     (501) staff       (20)     4191 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_shading.py
--rw-r--r--   0 runner     (501) staff       (20)     8585 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_u_values.py
--rw-r--r--   0 runner     (501) staff       (20)      594 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_use_non_res.py
--rw-r--r--   0 runner     (501) staff       (20)     9168 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_variants.py
--rw-r--r--   0 runner     (501) staff       (20)     5142 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_ventilation.py
--rw-r--r--   0 runner     (501) staff       (20)     2769 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_verification.py
--rw-r--r--   0 runner     (501) staff       (20)     5797 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/PHPP/sheet_io/io_windows.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/from_HBJSON/
--rw-r--r--   0 runner     (501) staff       (20)      331 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/README.md
--rw-r--r--   0 runner     (501) staff       (20)      129 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    18689 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/cleanup.py
--rw-r--r--   0 runner     (501) staff       (20)    12078 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/create_assemblies.py
--rw-r--r--   0 runner     (501) staff       (20)    14113 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/create_building.py
--rw-r--r--   0 runner     (501) staff       (20)     2594 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/create_elec_equip.py
--rw-r--r--   0 runner     (501) staff       (20)     4103 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/create_geometry.py
--rw-r--r--   0 runner     (501) staff       (20)    14515 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/create_hvac.py
--rw-r--r--   0 runner     (501) staff       (20)     3179 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/create_project.py
--rw-r--r--   0 runner     (501) staff       (20)     4730 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/create_rooms.py
--rw-r--r--   0 runner     (501) staff       (20)    13742 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/create_schedules.py
--rw-r--r--   0 runner     (501) staff       (20)     2729 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/create_shades.py
--rw-r--r--   0 runner     (501) staff       (20)     4814 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/create_shw.py
--rw-r--r--   0 runner     (501) staff       (20)    33349 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/create_variant.py
--rw-r--r--   0 runner     (501) staff       (20)     2121 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_HBJSON/read_HBJSON_file.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/from_WUFI_XML/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_WUFI_XML/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      574 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/from_WUFI_XML/read_WUFI_XML_file.py
--rw-r--r--   0 runner     (501) staff       (20)     3004 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/hbjson_to_phpp.py
--rw-r--r--   0 runner     (501) staff       (20)     2483 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/hbjson_to_wufi_xml.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/model/
--rw-r--r--   0 runner     (501) staff       (20)     2182 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/README.md
--rw-r--r--   0 runner     (501) staff       (20)      472 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     7351 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/building.py
--rw-r--r--   0 runner     (501) staff       (20)     3782 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/certification.py
--rw-r--r--   0 runner     (501) staff       (20)     9774 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/components.py
--rw-r--r--   0 runner     (501) staff       (20)     3782 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/constructions.py
--rw-r--r--   0 runner     (501) staff       (20)     6549 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/elec_equip.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/model/enums/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/enums/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      871 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/enums/building.py
--rw-r--r--   0 runner     (501) staff       (20)     1855 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/enums/hvac.py
--rw-r--r--   0 runner     (501) staff       (20)      824 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/enums/phi_certification_phpp_10.py
--rw-r--r--   0 runner     (501) staff       (20)      970 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/enums/phi_certification_phpp_9.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/enums/phius_certification.py
--rw-r--r--   0 runner     (501) staff       (20)      457 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/enums/phx_site.py
--rw-r--r--   0 runner     (501) staff       (20)    10576 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/geometry.py
--rw-r--r--   0 runner     (501) staff       (20)      304 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/ground.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/model/hvac/
--rw-r--r--   0 runner     (501) staff       (20)      404 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/hvac/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5008 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/hvac/_base.py
--rw-r--r--   0 runner     (501) staff       (20)    12333 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/hvac/collection.py
--rw-r--r--   0 runner     (501) staff       (20)     7319 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/hvac/cooling.py
--rw-r--r--   0 runner     (501) staff       (20)     3156 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/hvac/ducting.py
--rw-r--r--   0 runner     (501) staff       (20)     7219 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/hvac/heating.py
--rw-r--r--   0 runner     (501) staff       (20)     1174 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/hvac/piping.py
--rw-r--r--   0 runner     (501) staff       (20)     7998 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/hvac/ventilation.py
--rw-r--r--   0 runner     (501) staff       (20)     2783 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/hvac/water.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/model/loads/
--rw-r--r--   0 runner     (501) staff       (20)       98 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/loads/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      449 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/loads/occupancy.py
--rw-r--r--   0 runner     (501) staff       (20)      365 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/loads/ventilation.py
--rw-r--r--   0 runner     (501) staff       (20)     6131 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/phx_site.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/model/programs/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/programs/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      618 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/programs/occupancy.py
--rw-r--r--   0 runner     (501) staff       (20)      689 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/programs/ventilation.py
--rw-r--r--   0 runner     (501) staff       (20)     4890 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/project.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/model/schedules/
--rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/schedules/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2391 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/schedules/occupancy.py
--rw-r--r--   0 runner     (501) staff       (20)     2080 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/schedules/ventilation.py
--rw-r--r--   0 runner     (501) staff       (20)     1072 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/spaces.py
--rw-r--r--   0 runner     (501) staff       (20)     4475 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/model/utilization_patterns.py
--rw-r--r--   0 runner     (501) staff       (20)     5117 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/run.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/to_WUFI_XML/
--rw-r--r--   0 runner     (501) staff       (20)      236 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/to_WUFI_XML/README.md
--rw-r--r--   0 runner     (501) staff       (20)      286 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/to_WUFI_XML/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4998 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/to_WUFI_XML/xml_builder.py
--rw-r--r--   0 runner     (501) staff       (20)     2714 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/to_WUFI_XML/xml_converter.py
--rw-r--r--   0 runner     (501) staff       (20)    62361 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/to_WUFI_XML/xml_schemas.py
--rw-r--r--   0 runner     (501) staff       (20)     2262 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/to_WUFI_XML/xml_txt_to_file.py
--rw-r--r--   0 runner     (501) staff       (20)     2568 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/to_WUFI_XML/xml_writables.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX/xl/
--rw-r--r--   0 runner     (501) staff       (20)       45 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/xl/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    19644 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/xl/xl_app.py
--rw-r--r--   0 runner     (501) staff       (20)     8432 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/xl/xl_data.py
--rw-r--r--   0 runner     (501) staff       (20)     3756 2023-03-15 20:07:35.000000 PHX-1.8.1/PHX/xl/xl_typing.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2593 2023-03-15 20:09:22.000000 PHX-1.8.1/PHX.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     4268 2023-03-15 20:09:23.000000 PHX-1.8.1/PHX.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-03-15 20:09:22.000000 PHX-1.8.1/PHX.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       91 2023-03-15 20:09:22.000000 PHX-1.8.1/PHX.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        4 2023-03-15 20:09:22.000000 PHX-1.8.1/PHX.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     2593 2023-03-15 20:09:23.000000 PHX-1.8.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     1674 2023-03-15 20:07:35.000000 PHX-1.8.1/README.md
--rw-r--r--   0 runner     (501) staff       (20)     3175 2023-03-15 20:07:35.000000 PHX-1.8.1/_testing_to_PHPP.py
--rw-r--r--   0 runner     (501) staff       (20)     2422 2023-03-15 20:07:35.000000 PHX-1.8.1/_testing_to_WUFI.py
--rw-r--r--   0 runner     (501) staff       (20)       90 2023-03-15 20:07:35.000000 PHX-1.8.1/dev-requirements.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/docs/
--rw-r--r--   0 runner     (501) staff       (20)      765 2023-03-15 20:07:35.000000 PHX-1.8.1/docs/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/docs/sphinx/
--rw-r--r--   0 runner     (501) staff       (20)      638 2023-03-15 20:07:35.000000 PHX-1.8.1/docs/sphinx/Makefile
--rw-r--r--   0 runner     (501) staff       (20)      804 2023-03-15 20:07:35.000000 PHX-1.8.1/docs/sphinx/make.bat
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-15 20:09:23.000000 PHX-1.8.1/docs/sphinx/source/
--rw-r--r--   0 runner     (501) staff       (20)     1121 2023-03-15 20:07:35.000000 PHX-1.8.1/docs/sphinx/source/conf.py
--rw-r--r--   0 runner     (501) staff       (20)      201 2023-03-15 20:07:35.000000 PHX-1.8.1/docs/sphinx/source/index.rst
--rw-r--r--   0 runner     (501) staff       (20)       90 2023-03-15 20:07:35.000000 PHX-1.8.1/requirements.txt
--rw-r--r--   0 runner     (501) staff       (20)      819 2023-03-15 20:09:23.000000 PHX-1.8.1/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      376 2023-03-15 20:07:35.000000 PHX-1.8.1/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/.github/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/.github/workflows/
+-rw-r--r--   0 runner     (501) staff       (20)     1865 2023-03-16 08:55:02.000000 PHX-1.9.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner     (501) staff       (20)    35129 2023-03-16 08:55:02.000000 PHX-1.9.0/LICENSE
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/PHPP/
+-rw-r--r--   0 runner     (501) staff       (20)     1064 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       34 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    35984 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_app.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/PHPP/phpp_localization/
+-rw-r--r--   0 runner     (501) staff       (20)    40141 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_localization/EN_10_3.json
+-rw-r--r--   0 runner     (501) staff       (20)    40150 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_localization/EN_10_4A.json
+-rw-r--r--   0 runner     (501) staff       (20)    39587 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_localization/EN_9_6A.json
+-rw-r--r--   0 runner     (501) staff       (20)    39830 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_localization/EN_9_7IP.json
+-rw-r--r--   0 runner     (501) staff       (20)       99 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_localization/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1682 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_localization/load.py
+-rw-r--r--   0 runner     (501) staff       (20)    20844 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_localization/shape_model.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/PHPP/phpp_model/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1292 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/areas_data.py
+-rw-r--r--   0 runner     (501) staff       (20)     3365 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/areas_surface.py
+-rw-r--r--   0 runner     (501) staff       (20)     2304 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/areas_thermal_bridges.py
+-rw-r--r--   0 runner     (501) staff       (20)     6008 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/climate_entry.py
+-rw-r--r--   0 runner     (501) staff       (20)     5361 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/component_frame.py
+-rw-r--r--   0 runner     (501) staff       (20)     2117 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/component_glazing.py
+-rw-r--r--   0 runner     (501) staff       (20)     2522 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/component_vent.py
+-rw-r--r--   0 runner     (501) staff       (20)     8328 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/electricity_item.py
+-rw-r--r--   0 runner     (501) staff       (20)     4985 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/hot_water_piping.py
+-rw-r--r--   0 runner     (501) staff       (20)     3167 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/hot_water_tank.py
+-rw-r--r--   0 runner     (501) staff       (20)     3230 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/shading_rows.py
+-rw-r--r--   0 runner     (501) staff       (20)     3937 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/uvalues_constructor.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/vent_ducts.py
+-rw-r--r--   0 runner     (501) staff       (20)     6134 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/vent_space.py
+-rw-r--r--   0 runner     (501) staff       (20)     2216 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/vent_units.py
+-rw-r--r--   0 runner     (501) staff       (20)     2855 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/ventilation_data.py
+-rw-r--r--   0 runner     (501) staff       (20)     2038 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/verification_data.py
+-rw-r--r--   0 runner     (501) staff       (20)      758 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/version.py
+-rw-r--r--   0 runner     (501) staff       (20)     3569 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/phpp_model/windows_rows.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/PHPP/sheet_io/
+-rw-r--r--   0 runner     (501) staff       (20)      968 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12017 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_PER.py
+-rw-r--r--   0 runner     (501) staff       (20)    13415 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_addnl_vent.py
+-rw-r--r--   0 runner     (501) staff       (20)    11232 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_areas.py
+-rw-r--r--   0 runner     (501) staff       (20)     1422 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_climate.py
+-rw-r--r--   0 runner     (501) staff       (20)    10999 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_components.py
+-rw-r--r--   0 runner     (501) staff       (20)     3682 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_cooling_demand.py
+-rw-r--r--   0 runner     (501) staff       (20)     2622 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_cooling_peak_load.py
+-rw-r--r--   0 runner     (501) staff       (20)      612 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_elec_non_res.py
+-rw-r--r--   0 runner     (501) staff       (20)     1596 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_electricity.py
+-rw-r--r--   0 runner     (501) staff       (20)     1247 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)     3033 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_heating_demand.py
+-rw-r--r--   0 runner     (501) staff       (20)     2836 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_heating_peak_load.py
+-rw-r--r--   0 runner     (501) staff       (20)     7542 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_hot_water.py
+-rw-r--r--   0 runner     (501) staff       (20)      594 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_ihg_non_res.py
+-rw-r--r--   0 runner     (501) staff       (20)     5279 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_overview.py
+-rw-r--r--   0 runner     (501) staff       (20)     4191 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_shading.py
+-rw-r--r--   0 runner     (501) staff       (20)     8585 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_u_values.py
+-rw-r--r--   0 runner     (501) staff       (20)      594 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_use_non_res.py
+-rw-r--r--   0 runner     (501) staff       (20)     9168 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_variants.py
+-rw-r--r--   0 runner     (501) staff       (20)     5142 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_ventilation.py
+-rw-r--r--   0 runner     (501) staff       (20)     2769 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_verification.py
+-rw-r--r--   0 runner     (501) staff       (20)     5797 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/PHPP/sheet_io/io_windows.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/from_HBJSON/
+-rw-r--r--   0 runner     (501) staff       (20)      331 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/README.md
+-rw-r--r--   0 runner     (501) staff       (20)      129 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    18689 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/cleanup.py
+-rw-r--r--   0 runner     (501) staff       (20)    12078 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/create_assemblies.py
+-rw-r--r--   0 runner     (501) staff       (20)    14113 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/create_building.py
+-rw-r--r--   0 runner     (501) staff       (20)     2594 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/create_elec_equip.py
+-rw-r--r--   0 runner     (501) staff       (20)     4103 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/create_geometry.py
+-rw-r--r--   0 runner     (501) staff       (20)    14515 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/create_hvac.py
+-rw-r--r--   0 runner     (501) staff       (20)     3179 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/create_project.py
+-rw-r--r--   0 runner     (501) staff       (20)     4730 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/create_rooms.py
+-rw-r--r--   0 runner     (501) staff       (20)    13742 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/create_schedules.py
+-rw-r--r--   0 runner     (501) staff       (20)     2729 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/create_shades.py
+-rw-r--r--   0 runner     (501) staff       (20)     4814 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/create_shw.py
+-rw-r--r--   0 runner     (501) staff       (20)    33409 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/create_variant.py
+-rw-r--r--   0 runner     (501) staff       (20)     2121 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_HBJSON/read_HBJSON_file.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/from_WUFI_XML/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_WUFI_XML/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      574 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/from_WUFI_XML/read_WUFI_XML_file.py
+-rw-r--r--   0 runner     (501) staff       (20)     3004 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/hbjson_to_phpp.py
+-rw-r--r--   0 runner     (501) staff       (20)     2483 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/hbjson_to_wufi_xml.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/model/
+-rw-r--r--   0 runner     (501) staff       (20)     2182 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/README.md
+-rw-r--r--   0 runner     (501) staff       (20)      472 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     7351 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/building.py
+-rw-r--r--   0 runner     (501) staff       (20)     3819 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/certification.py
+-rw-r--r--   0 runner     (501) staff       (20)     9774 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/components.py
+-rw-r--r--   0 runner     (501) staff       (20)     3782 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/constructions.py
+-rw-r--r--   0 runner     (501) staff       (20)     6549 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/elec_equip.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/model/enums/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/enums/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      871 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/enums/building.py
+-rw-r--r--   0 runner     (501) staff       (20)     1855 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/enums/hvac.py
+-rw-r--r--   0 runner     (501) staff       (20)      824 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/enums/phi_certification_phpp_10.py
+-rw-r--r--   0 runner     (501) staff       (20)      970 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/enums/phi_certification_phpp_9.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/enums/phius_certification.py
+-rw-r--r--   0 runner     (501) staff       (20)      457 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/enums/phx_site.py
+-rw-r--r--   0 runner     (501) staff       (20)    10576 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/geometry.py
+-rw-r--r--   0 runner     (501) staff       (20)      304 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/ground.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/model/hvac/
+-rw-r--r--   0 runner     (501) staff       (20)      404 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/hvac/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5008 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/hvac/_base.py
+-rw-r--r--   0 runner     (501) staff       (20)    12333 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/hvac/collection.py
+-rw-r--r--   0 runner     (501) staff       (20)     7319 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/hvac/cooling.py
+-rw-r--r--   0 runner     (501) staff       (20)     3156 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/hvac/ducting.py
+-rw-r--r--   0 runner     (501) staff       (20)     7219 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/hvac/heating.py
+-rw-r--r--   0 runner     (501) staff       (20)     1174 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/hvac/piping.py
+-rw-r--r--   0 runner     (501) staff       (20)     7998 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/hvac/ventilation.py
+-rw-r--r--   0 runner     (501) staff       (20)     2783 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/hvac/water.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/model/loads/
+-rw-r--r--   0 runner     (501) staff       (20)       98 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/loads/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      449 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/loads/occupancy.py
+-rw-r--r--   0 runner     (501) staff       (20)      365 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/loads/ventilation.py
+-rw-r--r--   0 runner     (501) staff       (20)     6131 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/phx_site.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/model/programs/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/programs/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      618 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/programs/occupancy.py
+-rw-r--r--   0 runner     (501) staff       (20)      689 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/programs/ventilation.py
+-rw-r--r--   0 runner     (501) staff       (20)     4890 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/project.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/model/schedules/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/schedules/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2391 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/schedules/occupancy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2080 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/schedules/ventilation.py
+-rw-r--r--   0 runner     (501) staff       (20)     1072 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/spaces.py
+-rw-r--r--   0 runner     (501) staff       (20)     4475 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/model/utilization_patterns.py
+-rw-r--r--   0 runner     (501) staff       (20)     5117 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/run.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/to_WUFI_XML/
+-rw-r--r--   0 runner     (501) staff       (20)      236 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/to_WUFI_XML/README.md
+-rw-r--r--   0 runner     (501) staff       (20)      286 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/to_WUFI_XML/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4998 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/to_WUFI_XML/xml_builder.py
+-rw-r--r--   0 runner     (501) staff       (20)     2714 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/to_WUFI_XML/xml_converter.py
+-rw-r--r--   0 runner     (501) staff       (20)    62639 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/to_WUFI_XML/xml_schemas.py
+-rw-r--r--   0 runner     (501) staff       (20)     2262 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/to_WUFI_XML/xml_txt_to_file.py
+-rw-r--r--   0 runner     (501) staff       (20)     2568 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/to_WUFI_XML/xml_writables.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX/xl/
+-rw-r--r--   0 runner     (501) staff       (20)       45 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/xl/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    19644 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/xl/xl_app.py
+-rw-r--r--   0 runner     (501) staff       (20)     8432 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/xl/xl_data.py
+-rw-r--r--   0 runner     (501) staff       (20)     3756 2023-03-16 08:55:02.000000 PHX-1.9.0/PHX/xl/xl_typing.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     2593 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     4268 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       91 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        4 2023-03-16 08:56:36.000000 PHX-1.9.0/PHX.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     2593 2023-03-16 08:56:36.000000 PHX-1.9.0/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     1674 2023-03-16 08:55:02.000000 PHX-1.9.0/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     3175 2023-03-16 08:55:02.000000 PHX-1.9.0/_testing_to_PHPP.py
+-rw-r--r--   0 runner     (501) staff       (20)     2416 2023-03-16 08:55:02.000000 PHX-1.9.0/_testing_to_WUFI.py
+-rw-r--r--   0 runner     (501) staff       (20)       90 2023-03-16 08:55:02.000000 PHX-1.9.0/dev-requirements.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/docs/
+-rw-r--r--   0 runner     (501) staff       (20)      765 2023-03-16 08:55:02.000000 PHX-1.9.0/docs/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/docs/sphinx/
+-rw-r--r--   0 runner     (501) staff       (20)      638 2023-03-16 08:55:02.000000 PHX-1.9.0/docs/sphinx/Makefile
+-rw-r--r--   0 runner     (501) staff       (20)      804 2023-03-16 08:55:02.000000 PHX-1.9.0/docs/sphinx/make.bat
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-03-16 08:56:36.000000 PHX-1.9.0/docs/sphinx/source/
+-rw-r--r--   0 runner     (501) staff       (20)     1121 2023-03-16 08:55:02.000000 PHX-1.9.0/docs/sphinx/source/conf.py
+-rw-r--r--   0 runner     (501) staff       (20)      201 2023-03-16 08:55:02.000000 PHX-1.9.0/docs/sphinx/source/index.rst
+-rw-r--r--   0 runner     (501) staff       (20)       90 2023-03-16 08:55:02.000000 PHX-1.9.0/requirements.txt
+-rw-r--r--   0 runner     (501) staff       (20)      819 2023-03-16 08:56:36.000000 PHX-1.9.0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      376 2023-03-16 08:55:02.000000 PHX-1.9.0/setup.py
```

### Comparing `PHX-1.8.1/.github/workflows/ci.yaml` & `PHX-1.9.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/LICENSE` & `PHX-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/README.md` & `PHX-1.9.0/PHX/PHPP/README.md`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_app.py` & `PHX-1.9.0/PHX/PHPP/phpp_app.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_localization/EN_10_3.json` & `PHX-1.9.0/PHX/PHPP/phpp_localization/EN_10_3.json`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_localization/EN_10_4A.json` & `PHX-1.9.0/PHX/PHPP/phpp_localization/EN_10_4A.json`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_localization/EN_9_6A.json` & `PHX-1.9.0/PHX/PHPP/phpp_localization/EN_9_6A.json`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_localization/EN_9_7IP.json` & `PHX-1.9.0/PHX/PHPP/phpp_localization/EN_9_7IP.json`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_localization/load.py` & `PHX-1.9.0/PHX/PHPP/phpp_localization/load.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_localization/shape_model.py` & `PHX-1.9.0/PHX/PHPP/phpp_localization/shape_model.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/areas_data.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/areas_data.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/areas_surface.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/areas_surface.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/areas_thermal_bridges.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/areas_thermal_bridges.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/climate_entry.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/climate_entry.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/component_frame.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/component_frame.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/component_glazing.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/component_glazing.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/component_vent.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/component_vent.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/electricity_item.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/electricity_item.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/hot_water_piping.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/hot_water_piping.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/hot_water_tank.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/hot_water_tank.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/shading_rows.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/shading_rows.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/uvalues_constructor.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/uvalues_constructor.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/vent_space.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/vent_space.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/vent_units.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/vent_units.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/ventilation_data.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/ventilation_data.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/verification_data.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/verification_data.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/version.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/version.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/phpp_model/windows_rows.py` & `PHX-1.9.0/PHX/PHPP/phpp_model/windows_rows.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/__init__.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/__init__.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_PER.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_PER.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_addnl_vent.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_addnl_vent.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_areas.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_areas.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_climate.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_climate.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_components.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_components.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_cooling_demand.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_cooling_demand.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_cooling_peak_load.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_cooling_peak_load.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_elec_non_res.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_elec_non_res.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_electricity.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_electricity.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_exceptions.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_exceptions.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_heating_demand.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_heating_demand.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_heating_peak_load.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_heating_peak_load.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_hot_water.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_hot_water.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_ihg_non_res.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_ihg_non_res.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_overview.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_overview.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_shading.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_shading.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_u_values.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_u_values.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_use_non_res.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_use_non_res.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_variants.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_variants.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_ventilation.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_ventilation.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_verification.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_verification.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/PHPP/sheet_io/io_windows.py` & `PHX-1.9.0/PHX/PHPP/sheet_io/io_windows.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/from_HBJSON/cleanup.py` & `PHX-1.9.0/PHX/from_HBJSON/cleanup.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/from_HBJSON/create_assemblies.py` & `PHX-1.9.0/PHX/from_HBJSON/create_assemblies.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/from_HBJSON/create_building.py` & `PHX-1.9.0/PHX/from_HBJSON/create_building.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/from_HBJSON/create_elec_equip.py` & `PHX-1.9.0/PHX/from_HBJSON/create_elec_equip.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/from_HBJSON/create_geometry.py` & `PHX-1.9.0/PHX/from_HBJSON/create_geometry.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/from_HBJSON/create_hvac.py` & `PHX-1.9.0/PHX/from_HBJSON/create_hvac.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/from_HBJSON/create_project.py` & `PHX-1.9.0/PHX/from_HBJSON/create_project.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/from_HBJSON/create_rooms.py` & `PHX-1.9.0/PHX/from_HBJSON/create_rooms.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/from_HBJSON/create_schedules.py` & `PHX-1.9.0/PHX/from_HBJSON/create_schedules.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/from_HBJSON/create_shades.py` & `PHX-1.9.0/PHX/from_HBJSON/create_shades.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/from_HBJSON/create_shw.py` & `PHX-1.9.0/PHX/from_HBJSON/create_shw.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/from_HBJSON/create_variant.py` & `PHX-1.9.0/PHX/from_HBJSON/create_variant.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,30 +280,32 @@
     --------
         * None
     """
 
     # -- Type Aliases
     ph_bldg = _variant.phius_cert.ph_building_data  # alias
     hb_prop_energy: RoomEnergyProperties = _hb_room.properties.energy  # type: ignore
+    hb_prop_ph: RoomPhProperties = _hb_room.properties.ph # type: ignore
 
     # -- Set the occupancy
     if hb_prop_energy.people:
         hb_ppl_prop_ph: people.PeoplePhProperties = hb_prop_energy.people.properties.ph  # type: ignore
         ph_bldg.num_of_units = hb_ppl_prop_ph.number_dwelling_units
     ph_bldg.num_of_floors = _hb_room.properties.ph.ph_bldg_segment.num_floor_levels  # type: ignore
 
     # TODO: Foundations. For now: set to None
     ph_bldg.add_foundation(ground.PhxFoundation())
 
     # -- Set the airtightness for Building
-    ph_bldg.airtightness_q50 = _hb_room.properties.energy.infiltration.flow_per_exterior_area * 3600  # type: ignore
+    ph_bldg.airtightness_q50 = hb_prop_energy.infiltration.flow_per_exterior_area * 3600
 
     # -- Set the air temp setpoints
-    ph_bldg.setpoints.winter = _hb_room.properties.ph.ph_bldg_segment.set_points.winter  # type: ignore
-    ph_bldg.setpoints.summer = _hb_room.properties.ph.ph_bldg_segment.set_points.summer  # type: ignore
+    ph_bldg.setpoints.winter = hb_prop_ph.ph_bldg_segment.set_points.winter
+    ph_bldg.setpoints.summer = hb_prop_ph.ph_bldg_segment.set_points.summer
+    ph_bldg.mech_room_temp = hb_prop_ph.ph_bldg_segment.mech_room_temp
 
     return None
 
 
 def add_climate_from_hb_room(_variant: project.PhxVariant, _hb_room: room.Room) -> None:
     """Copy PHX-Climate info from a Honeybee-Room over to a PHX-Variant.
```

### Comparing `PHX-1.8.1/PHX/from_HBJSON/read_HBJSON_file.py` & `PHX-1.9.0/PHX/from_HBJSON/read_HBJSON_file.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/from_WUFI_XML/read_WUFI_XML_file.py` & `PHX-1.9.0/PHX/from_WUFI_XML/read_WUFI_XML_file.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/hbjson_to_phpp.py` & `PHX-1.9.0/PHX/hbjson_to_phpp.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/hbjson_to_wufi_xml.py` & `PHX-1.9.0/PHX/hbjson_to_wufi_xml.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/README.md` & `PHX-1.9.0/PHX/model/README.md`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/building.py` & `PHX-1.9.0/PHX/model/building.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/certification.py` & `PHX-1.9.0/PHX/model/certification.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 from PHX.model import ground
 from PHX.model.enums import phi_certification_phpp_9, phius_certification
 
 
 @dataclass
 class PhxSetpoints:
-    winter: float = 20  # deg. C
-    summer: float = 25  # deg. C
+    winter: float = 20.0  # deg. C
+    summer: float = 25.0  # deg. C
 
 
 @dataclass
 class PhxPhBuildingData:
     _count: ClassVar[int] = 0
 
     id_num: int = field(init=False, default=0)
@@ -30,14 +30,15 @@
 
     airtightness_q50: float = 1.0  # m3/hr-m2-envelope
     airtightness_n50: float = 1.0  # ach
     wind_coefficient_e: float = 0.07
     wind_coefficient_f: float = 15
 
     setpoints: PhxSetpoints = field(default_factory=PhxSetpoints)
+    mech_room_temp: float = 20.0
 
     foundations: list[ground.PhxFoundation] = field(default_factory=list)
 
     def __post_init__(self) -> None:
         self.__class__._count += 1
         self.id_num = self.__class__._count
```

### Comparing `PHX-1.8.1/PHX/model/components.py` & `PHX-1.9.0/PHX/model/components.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/constructions.py` & `PHX-1.9.0/PHX/model/constructions.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/elec_equip.py` & `PHX-1.9.0/PHX/model/elec_equip.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/enums/building.py` & `PHX-1.9.0/PHX/model/enums/building.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/enums/hvac.py` & `PHX-1.9.0/PHX/model/enums/hvac.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/enums/phi_certification_phpp_10.py` & `PHX-1.9.0/PHX/model/enums/phi_certification_phpp_10.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/enums/phi_certification_phpp_9.py` & `PHX-1.9.0/PHX/model/enums/phi_certification_phpp_9.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/enums/phius_certification.py` & `PHX-1.9.0/PHX/model/enums/phius_certification.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/geometry.py` & `PHX-1.9.0/PHX/model/geometry.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/hvac/_base.py` & `PHX-1.9.0/PHX/model/hvac/_base.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/hvac/collection.py` & `PHX-1.9.0/PHX/model/hvac/collection.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/hvac/cooling.py` & `PHX-1.9.0/PHX/model/hvac/cooling.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/hvac/ducting.py` & `PHX-1.9.0/PHX/model/hvac/ducting.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/hvac/heating.py` & `PHX-1.9.0/PHX/model/hvac/heating.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/hvac/piping.py` & `PHX-1.9.0/PHX/model/hvac/piping.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/hvac/ventilation.py` & `PHX-1.9.0/PHX/model/hvac/ventilation.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/hvac/water.py` & `PHX-1.9.0/PHX/model/hvac/water.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/phx_site.py` & `PHX-1.9.0/PHX/model/phx_site.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/programs/occupancy.py` & `PHX-1.9.0/PHX/model/programs/occupancy.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/programs/ventilation.py` & `PHX-1.9.0/PHX/model/programs/ventilation.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/project.py` & `PHX-1.9.0/PHX/model/project.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/schedules/occupancy.py` & `PHX-1.9.0/PHX/model/schedules/occupancy.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/schedules/ventilation.py` & `PHX-1.9.0/PHX/model/schedules/ventilation.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/spaces.py` & `PHX-1.9.0/PHX/model/spaces.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/model/utilization_patterns.py` & `PHX-1.9.0/PHX/model/utilization_patterns.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/run.py` & `PHX-1.9.0/PHX/run.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/to_WUFI_XML/xml_builder.py` & `PHX-1.9.0/PHX/to_WUFI_XML/xml_builder.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/to_WUFI_XML/xml_converter.py` & `PHX-1.9.0/PHX/to_WUFI_XML/xml_converter.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/to_WUFI_XML/xml_schemas.py` & `PHX-1.9.0/PHX/to_WUFI_XML/xml_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,14 +310,17 @@
             ],
         ),
         XML_Object(
             "InternalGainsAdditionalData",
             None,
             _schema_name="_InternalGainsAdditionalData",
         ),
+        XML_Node("MechanicalRoomTemperature", _phius_cert.ph_building_data.mech_room_temp),
+        XML_Node("IndoorTemperature", _phius_cert.ph_building_data.setpoints.winter),
+        XML_Node("OverheatingTemperatureThreshold", _phius_cert.ph_building_data.setpoints.summer),
     ]
 
 
 def _InternalGainsAdditionalData(*args, **kwargs) -> List[xml_writable]:
     return [
         XML_Node("EvaporationHeatPerPerson", 15, "unit", "W"),
         XML_Node("HeatLossFluschingWC", True),
```

### Comparing `PHX-1.8.1/PHX/to_WUFI_XML/xml_txt_to_file.py` & `PHX-1.9.0/PHX/to_WUFI_XML/xml_txt_to_file.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/to_WUFI_XML/xml_writables.py` & `PHX-1.9.0/PHX/to_WUFI_XML/xml_writables.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/xl/xl_app.py` & `PHX-1.9.0/PHX/xl/xl_app.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/xl/xl_data.py` & `PHX-1.9.0/PHX/xl/xl_data.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX/xl/xl_typing.py` & `PHX-1.9.0/PHX/xl/xl_typing.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PHX.egg-info/PKG-INFO` & `PHX-1.9.0/PHX.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PHX
-Version: 1.8.1
+Version: 1.9.0
 Summary: Input / Output Passive House building energy model data.
 Home-page: https://github.com/PH-Tools/PHX
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PHX (Passive House Exchange):
         The Passive House Exchange (PHX) model standard and libraries enable users to move their building model data in and out of energy modeling software platforms such as the Passive House Planning Package (PHPP) and WUFI-Passive.
```

### Comparing `PHX-1.8.1/PHX.egg-info/SOURCES.txt` & `PHX-1.9.0/PHX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/PKG-INFO` & `PHX-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PHX
-Version: 1.8.1
+Version: 1.9.0
 Summary: Input / Output Passive House building energy model data.
 Home-page: https://github.com/PH-Tools/PHX
 Author: PH-Tools
 Author-email: phtools@bldgtyp.com
 License: GPLv3+
 Description: # PHX (Passive House Exchange):
         The Passive House Exchange (PHX) model standard and libraries enable users to move their building model data in and out of energy modeling software platforms such as the Passive House Planning Package (PHPP) and WUFI-Passive.
```

### Comparing `PHX-1.8.1/README.md` & `PHX-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/_testing_to_PHPP.py` & `PHX-1.9.0/_testing_to_PHPP.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/_testing_to_WUFI.py` & `PHX-1.9.0/_testing_to_WUFI.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ]
 SOURCE_FILES = [SOURCE_DIR / file for file in SOURCE_FILE_NAMES]
 TARGET_DIR = pathlib.Path("tests", "_reference_xml")
 
 # -- Temp
 SOURCE_FILES = [
     pathlib.Path(
-        "/Users/em/Dropbox/bldgtyp-00/00_PH_Tools/PHX/sample/hbjson/Ridgeway_VI_230315.hbjson"
+        "/Users/em/Dropbox/bldgtyp-00/00_PH_Tools/PHX/sample/hbjson/ducting_test.hbjson"
     )
 ]
 TARGET_DIR = pathlib.Path("sample")
 
 
 def generate_xml_file(_source: pathlib.Path, _target_dir: pathlib.Path):
     # -- Re-set all the PHX modules (counters)
```

### Comparing `PHX-1.8.1/docs/README.md` & `PHX-1.9.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/docs/sphinx/Makefile` & `PHX-1.9.0/docs/sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/docs/sphinx/make.bat` & `PHX-1.9.0/docs/sphinx/make.bat`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/docs/sphinx/source/conf.py` & `PHX-1.9.0/docs/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `PHX-1.8.1/setup.cfg` & `PHX-1.9.0/setup.cfg`

 * *Files identical despite different names*

