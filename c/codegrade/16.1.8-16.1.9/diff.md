# Comparing `tmp/codegrade-16.1.8.tar.gz` & `tmp/codegrade-16.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codegrade-16.1.8.tar", max compression
+gzip compressed data, was "codegrade-16.1.9.tar", max compression
```

## Comparing `codegrade-16.1.8.tar` & `codegrade-16.1.9.tar`

### file list

```diff
@@ -1,532 +1,538 @@
--rw-r--r--   0        0        0     2019 2023-03-10 09:50:00.309274 codegrade-16.1.8/README.md
--rw-r--r--   0        0        0     5813 2023-03-10 09:53:19.577625 codegrade-16.1.8/cg_dt_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 09:53:19.589625 codegrade-16.1.8/cg_dt_utils/py.typed
--rw-r--r--   0        0        0      260 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_maybe/__init__.py
--rw-r--r--   0        0        0    13379 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_maybe/_just.py
--rw-r--r--   0        0        0      342 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_maybe/_maybe.py
--rw-r--r--   0        0        0     5400 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_maybe/_nothing.py
--rw-r--r--   0        0        0      705 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_maybe/_type_helpers.py
--rw-r--r--   0        0        0     2580 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_maybe/cg_maybe_plugin.py
--rw-r--r--   0        0        0        0 2023-03-10 09:53:19.589625 codegrade-16.1.8/cg_maybe/py.typed
--rw-r--r--   0        0        0     3929 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_maybe/utils.py
--rw-r--r--   0        0        0      994 2023-03-10 09:53:19.577625 codegrade-16.1.8/cg_request_args/__init__.py
--rw-r--r--   0        0        0      724 2023-03-10 09:53:19.577625 codegrade-16.1.8/cg_request_args/_any_value.py
--rw-r--r--   0        0        0    15429 2023-03-10 09:53:19.577625 codegrade-16.1.8/cg_request_args/_base.py
--rw-r--r--   0        0        0    12024 2023-03-10 09:53:19.577625 codegrade-16.1.8/cg_request_args/_convert.py
--rw-r--r--   0        0        0     2360 2023-03-10 09:53:19.577625 codegrade-16.1.8/cg_request_args/_enum.py
--rw-r--r--   0        0        0     1437 2023-03-10 09:53:19.577625 codegrade-16.1.8/cg_request_args/_lazy.py
--rw-r--r--   0        0        0     2565 2023-03-10 09:53:19.577625 codegrade-16.1.8/cg_request_args/_list.py
--rw-r--r--   0        0        0     1080 2023-03-10 09:53:19.577625 codegrade-16.1.8/cg_request_args/_literal.py
--rw-r--r--   0        0        0    22148 2023-03-10 09:53:19.577625 codegrade-16.1.8/cg_request_args/_mapping.py
--rw-r--r--   0        0        0     6789 2023-03-10 09:53:19.577625 codegrade-16.1.8/cg_request_args/_multipart.py
--rw-r--r--   0        0        0     1211 2023-03-10 09:53:19.577625 codegrade-16.1.8/cg_request_args/_nullable.py
--rw-r--r--   0        0        0     2094 2023-03-10 09:53:19.577625 codegrade-16.1.8/cg_request_args/_parse_utils.py
--rw-r--r--   0        0        0     1900 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_request_args/_query.py
--rw-r--r--   0        0        0    10772 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_request_args/_rich_value.py
--rw-r--r--   0        0        0     1402 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_request_args/_swagger_utils.py
--rw-r--r--   0        0        0     3960 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_request_args/_swaggerize.py
--rw-r--r--   0        0        0     1519 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_request_args/_utils.py
--rw-r--r--   0        0        0     4340 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_request_args/exceptions.py
--rw-r--r--   0        0        0        0 2023-03-10 09:53:19.589625 codegrade-16.1.8/cg_request_args/py.typed
--rw-r--r--   0        0        0    15309 2023-03-10 09:53:19.581625 codegrade-16.1.8/cg_request_args/request_args_plugin.py
--rw-r--r--   0        0        0     2475 2023-03-10 09:50:04.321281 codegrade-16.1.8/codegrade/__init__.py
--rw-r--r--   0        0        0      490 2023-03-10 09:50:03.009279 codegrade-16.1.8/codegrade/_api/__init__.py
--rw-r--r--   0        0        0     2354 2023-03-10 09:50:04.349281 codegrade-16.1.8/codegrade/_api/about.py
--rw-r--r--   0        0        0    59235 2023-03-10 09:50:05.133283 codegrade-16.1.8/codegrade/_api/assignment.py
--rw-r--r--   0        0        0    42296 2023-03-10 09:50:04.897282 codegrade-16.1.8/codegrade/_api/auto_test.py
--rw-r--r--   0        0        0    15003 2023-03-10 09:50:05.053283 codegrade-16.1.8/codegrade/_api/comment.py
--rw-r--r--   0        0        0    65745 2023-03-10 09:50:06.033284 codegrade-16.1.8/codegrade/_api/course.py
--rw-r--r--   0        0        0    11234 2023-03-10 09:50:05.257283 codegrade-16.1.8/codegrade/_api/course_price.py
--rw-r--r--   0        0        0     2657 2023-03-10 09:50:05.325283 codegrade-16.1.8/codegrade/_api/file.py
--rw-r--r--   0        0        0     7924 2023-03-10 09:50:05.417283 codegrade-16.1.8/codegrade/_api/git_provider.py
--rw-r--r--   0        0        0     8551 2023-03-10 09:50:05.517283 codegrade-16.1.8/codegrade/_api/group.py
--rw-r--r--   0        0        0     6844 2023-03-10 09:50:05.597283 codegrade-16.1.8/codegrade/_api/group_set.py
--rw-r--r--   0        0        0     4134 2023-03-10 09:50:05.641283 codegrade-16.1.8/codegrade/_api/login_link.py
--rw-r--r--   0        0        0    14594 2023-03-10 09:50:05.865284 codegrade-16.1.8/codegrade/_api/lti.py
--rw-r--r--   0        0        0     6562 2023-03-10 09:50:05.937284 codegrade-16.1.8/codegrade/_api/notification.py
--rw-r--r--   0        0        0     5104 2023-03-10 09:50:06.001284 codegrade-16.1.8/codegrade/_api/oauth_provider.py
--rw-r--r--   0        0        0     6472 2023-03-10 09:50:06.157284 codegrade-16.1.8/codegrade/_api/oauth_token.py
--rw-r--r--   0        0        0     3019 2023-03-10 09:50:06.065284 codegrade-16.1.8/codegrade/_api/permission.py
--rw-r--r--   0        0        0     1909 2023-03-10 09:50:06.093284 codegrade-16.1.8/codegrade/_api/plagiarism.py
--rw-r--r--   0        0        0     3566 2023-03-10 09:50:06.201284 codegrade-16.1.8/codegrade/_api/role.py
--rw-r--r--   0        0        0    11091 2023-03-10 09:50:06.285285 codegrade-16.1.8/codegrade/_api/section.py
--rw-r--r--   0        0        0     4110 2023-03-10 09:50:06.253285 codegrade-16.1.8/codegrade/_api/site_settings.py
--rw-r--r--   0        0        0     6583 2023-03-10 09:50:06.329285 codegrade-16.1.8/codegrade/_api/snippet.py
--rw-r--r--   0        0        0     2600 2023-03-10 09:50:06.313284 codegrade-16.1.8/codegrade/_api/sso_provider.py
--rw-r--r--   0        0        0    20958 2023-03-10 09:50:06.665285 codegrade-16.1.8/codegrade/_api/submission.py
--rw-r--r--   0        0        0     6862 2023-03-10 09:50:06.405285 codegrade-16.1.8/codegrade/_api/task_result.py
--rw-r--r--   0        0        0    25894 2023-03-10 09:50:06.825285 codegrade-16.1.8/codegrade/_api/tenant.py
--rw-r--r--   0        0        0     3455 2023-03-10 09:50:06.709285 codegrade-16.1.8/codegrade/_api/transaction.py
--rw-r--r--   0        0        0    13833 2023-03-10 09:50:06.873285 codegrade-16.1.8/codegrade/_api/user.py
--rw-r--r--   0        0        0     8745 2023-03-10 09:50:06.929286 codegrade-16.1.8/codegrade/_api/user_setting.py
--rw-r--r--   0        0        0    23115 2023-03-10 09:50:07.257286 codegrade-16.1.8/codegrade/client.py
--rw-r--r--   0        0        0      597 2023-03-10 09:50:06.937286 codegrade-16.1.8/codegrade/errors.py
--rw-r--r--   0        0        0    28707 2023-03-10 09:50:07.229286 codegrade-16.1.8/codegrade/models/__init__.py
--rw-r--r--   0        0        0     2635 2023-03-10 09:50:07.269286 codegrade-16.1.8/codegrade/models/_base_price.py
--rw-r--r--   0        0        0     1715 2023-03-10 09:50:07.285286 codegrade-16.1.8/codegrade/models/_saml_ui_logo_info.py
--rw-r--r--   0        0        0     2285 2023-03-10 09:50:07.305286 codegrade-16.1.8/codegrade/models/_submission_rubric_item_data_parser.py
--rw-r--r--   0        0        0     2670 2023-03-10 09:50:07.329286 codegrade-16.1.8/codegrade/models/about.py
--rw-r--r--   0        0        0     1390 2023-03-10 09:50:07.329286 codegrade-16.1.8/codegrade/models/abstract_role.py
--rw-r--r--   0        0        0     1298 2023-03-10 09:50:07.349286 codegrade-16.1.8/codegrade/models/add_users_section_data.py
--rw-r--r--   0        0        0     1914 2023-03-10 09:50:07.357286 codegrade-16.1.8/codegrade/models/all_auto_test_results.py
--rw-r--r--   0        0        0    36010 2023-03-10 09:50:08.121287 codegrade-16.1.8/codegrade/models/all_site_settings.py
--rw-r--r--   0        0        0     2202 2023-03-10 09:50:07.393286 codegrade-16.1.8/codegrade/models/any_auto_test_step_as_json.py
--rw-r--r--   0        0        0     2530 2023-03-10 09:50:07.417286 codegrade-16.1.8/codegrade/models/any_error.py
--rw-r--r--   0        0        0     2083 2023-03-10 09:50:07.449286 codegrade-16.1.8/codegrade/models/any_non_redacted_auto_test_step_as_json.py
--rw-r--r--   0        0        0     2914 2023-03-10 09:50:07.489287 codegrade-16.1.8/codegrade/models/any_redacted_auto_test_step_as_json.py
--rw-r--r--   0        0        0     2459 2023-03-10 09:50:01.965277 codegrade-16.1.8/codegrade/models/api_codes.py
--rw-r--r--   0        0        0    21454 2023-03-10 09:50:08.185288 codegrade-16.1.8/codegrade/models/assignment.py
--rw-r--r--   0        0        0      225 2023-03-10 09:50:02.397278 codegrade-16.1.8/codegrade/models/assignment_anonymization_algo.py
--rw-r--r--   0        0        0     1597 2023-03-10 09:50:08.153288 codegrade-16.1.8/codegrade/models/assignment_default_grading_scale_points_setting.py
--rw-r--r--   0        0        0     1536 2023-03-10 09:50:08.177288 codegrade-16.1.8/codegrade/models/assignment_default_grading_scale_setting.py
--rw-r--r--   0        0        0     1481 2023-03-10 09:50:08.205288 codegrade-16.1.8/codegrade/models/assignment_description_enabled_setting.py
--rw-r--r--   0        0        0      247 2023-03-10 09:50:00.929275 codegrade-16.1.8/codegrade/models/assignment_done_type.py
--rw-r--r--   0        0        0      405 2023-03-10 09:50:02.541278 codegrade-16.1.8/codegrade/models/assignment_export_column.py
--rw-r--r--   0        0        0     1990 2023-03-10 09:50:08.221288 codegrade-16.1.8/codegrade/models/assignment_feedback.py
--rw-r--r--   0        0        0     2426 2023-03-10 09:50:08.245288 codegrade-16.1.8/codegrade/models/assignment_grader.py
--rw-r--r--   0        0        0     1527 2023-03-10 09:50:08.249288 codegrade-16.1.8/codegrade/models/assignment_grading_scale_points_enabled_setting.py
--rw-r--r--   0        0        0      211 2023-03-10 09:50:01.785277 codegrade-16.1.8/codegrade/models/assignment_kind.py
--rw-r--r--   0        0        0     2326 2023-03-10 09:50:08.285288 codegrade-16.1.8/codegrade/models/assignment_login_link.py
--rw-r--r--   0        0        0     1462 2023-03-10 09:50:08.273288 codegrade-16.1.8/codegrade/models/assignment_max_points_enabled_setting.py
--rw-r--r--   0        0        0     1658 2023-03-10 09:50:08.301288 codegrade-16.1.8/codegrade/models/assignment_peer_feedback_connection.py
--rw-r--r--   0        0        0     3342 2023-03-10 09:50:08.329288 codegrade-16.1.8/codegrade/models/assignment_peer_feedback_settings.py
--rw-r--r--   0        0        0     1479 2023-03-10 09:50:08.325288 codegrade-16.1.8/codegrade/models/assignment_percentage_decimals_setting.py
--rw-r--r--   0        0        0     1535 2023-03-10 09:50:08.349288 codegrade-16.1.8/codegrade/models/assignment_percentage_grading_settings.py
--rw-r--r--   0        0        0     1440 2023-03-10 09:50:08.357288 codegrade-16.1.8/codegrade/models/assignment_point_decimals_setting.py
--rw-r--r--   0        0        0     1985 2023-03-10 09:50:08.377288 codegrade-16.1.8/codegrade/models/assignment_points_grading_settings.py
--rw-r--r--   0        0        0      239 2023-03-10 09:50:02.249278 codegrade-16.1.8/codegrade/models/assignment_state_enum.py
--rw-r--r--   0        0        0     1661 2023-03-10 09:50:08.385288 codegrade-16.1.8/codegrade/models/assignment_template.py
--rw-r--r--   0        0        0     1432 2023-03-10 09:50:08.405288 codegrade-16.1.8/codegrade/models/at_image_caching_enabled_setting.py
--rw-r--r--   0        0        0     8263 2023-03-10 09:50:08.677288 codegrade-16.1.8/codegrade/models/auto_test.py
--rw-r--r--   0        0        0     1483 2023-03-10 09:50:08.429288 codegrade-16.1.8/codegrade/models/auto_test_capture_points_message_setting.py
--rw-r--r--   0        0        0     1454 2023-03-10 09:50:08.621288 codegrade-16.1.8/codegrade/models/auto_test_checkpoint_message_setting.py
--rw-r--r--   0        0        0     1462 2023-03-10 09:50:08.645288 codegrade-16.1.8/codegrade/models/auto_test_code_quality_message_setting.py
--rw-r--r--   0        0        0     1394 2023-03-10 09:50:08.673288 codegrade-16.1.8/codegrade/models/auto_test_enabled_setting.py
--rw-r--r--   0        0        0     1743 2023-03-10 09:50:08.705289 codegrade-16.1.8/codegrade/models/auto_test_fixture.py
--rw-r--r--   0        0        0     3532 2023-03-10 09:50:08.729288 codegrade-16.1.8/codegrade/models/auto_test_global_setup_output.py
--rw-r--r--   0        0        0     1765 2023-03-10 09:50:08.733289 codegrade-16.1.8/codegrade/models/auto_test_global_setup_script.py
--rw-r--r--   0        0        0     1489 2023-03-10 09:50:08.757289 codegrade-16.1.8/codegrade/models/auto_test_heartbeat_interval_setting.py
--rw-r--r--   0        0        0     1462 2023-03-10 09:50:08.757289 codegrade-16.1.8/codegrade/models/auto_test_heartbeat_max_missed_setting.py
--rw-r--r--   0        0        0     1432 2023-03-10 09:50:08.785289 codegrade-16.1.8/codegrade/models/auto_test_io_test_message_setting.py
--rw-r--r--   0        0        0     1452 2023-03-10 09:50:08.785289 codegrade-16.1.8/codegrade/models/auto_test_io_test_sub_message_setting.py
--rw-r--r--   0        0        0     1497 2023-03-10 09:50:08.809289 codegrade-16.1.8/codegrade/models/auto_test_max_concurrent_batch_runs_setting.py
--rw-r--r--   0        0        0     1499 2023-03-10 09:50:08.813289 codegrade-16.1.8/codegrade/models/auto_test_max_global_setup_time_setting.py
--rw-r--r--   0        0        0     1452 2023-03-10 09:50:08.833289 codegrade-16.1.8/codegrade/models/auto_test_max_jobs_per_runner_setting.py
--rw-r--r--   0        0        0     1534 2023-03-10 09:50:08.841289 codegrade-16.1.8/codegrade/models/auto_test_max_per_student_setup_time_setting.py
--rw-r--r--   0        0        0     1514 2023-03-10 09:50:08.861289 codegrade-16.1.8/codegrade/models/auto_test_max_result_not_started_setting.py
--rw-r--r--   0        0        0     1473 2023-03-10 09:50:08.869289 codegrade-16.1.8/codegrade/models/auto_test_max_time_command_setting.py
--rw-r--r--   0        0        0     1679 2023-03-10 09:50:08.889289 codegrade-16.1.8/codegrade/models/auto_test_max_unit_test_metadata_length_setting.py
--rw-r--r--   0        0        0     3144 2023-03-10 09:50:08.917289 codegrade-16.1.8/codegrade/models/auto_test_quality_comment.py
--rw-r--r--   0        0        0     3711 2023-03-10 09:50:08.941289 codegrade-16.1.8/codegrade/models/auto_test_result.py
--rw-r--r--   0        0        0      399 2023-03-10 09:50:01.381276 codegrade-16.1.8/codegrade/models/auto_test_result_state.py
--rw-r--r--   0        0        0     2591 2023-03-10 09:50:08.957289 codegrade-16.1.8/codegrade/models/auto_test_result_with_extra_data.py
--rw-r--r--   0        0        0     2387 2023-03-10 09:50:08.981289 codegrade-16.1.8/codegrade/models/auto_test_run.py
--rw-r--r--   0        0        0     1456 2023-03-10 09:50:08.981289 codegrade-16.1.8/codegrade/models/auto_test_run_program_message_setting.py
--rw-r--r--   0        0        0     1267 2023-03-10 09:50:09.005289 codegrade-16.1.8/codegrade/models/auto_test_runner.py
--rw-r--r--   0        0        0      417 2023-03-10 09:50:02.537279 codegrade-16.1.8/codegrade/models/auto_test_runner_state.py
--rw-r--r--   0        0        0     2424 2023-03-10 09:50:09.021289 codegrade-16.1.8/codegrade/models/auto_test_set.py
--rw-r--r--   0        0        0     1390 2023-03-10 09:50:09.025289 codegrade-16.1.8/codegrade/models/auto_test_step_base.py
--rw-r--r--   0        0        0     2055 2023-03-10 09:50:09.049289 codegrade-16.1.8/codegrade/models/auto_test_step_base_as_json.py
--rw-r--r--   0        0        0     2922 2023-03-10 09:50:09.073289 codegrade-16.1.8/codegrade/models/auto_test_step_base_input_as_json.py
--rw-r--r--   0        0        0      964 2023-03-10 09:50:09.065289 codegrade-16.1.8/codegrade/models/auto_test_step_log_base.py
--rw-r--r--   0        0        0     4809 2023-03-10 09:50:09.133289 codegrade-16.1.8/codegrade/models/auto_test_step_result.py
--rw-r--r--   0        0        0      341 2023-03-10 09:50:01.785277 codegrade-16.1.8/codegrade/models/auto_test_step_result_state.py
--rw-r--r--   0        0        0     2005 2023-03-10 09:50:09.109289 codegrade-16.1.8/codegrade/models/auto_test_step_validation_exception.py
--rw-r--r--   0        0        0     3556 2023-03-10 09:50:09.161289 codegrade-16.1.8/codegrade/models/auto_test_suite.py
--rw-r--r--   0        0        0     1444 2023-03-10 09:50:09.161289 codegrade-16.1.8/codegrade/models/auto_test_unit_test_message_setting.py
--rw-r--r--   0        0        0     1503 2023-03-10 09:50:09.185289 codegrade-16.1.8/codegrade/models/automatic_lti1p3_assignment_import_setting.py
--rw-r--r--   0        0        0     1444 2023-03-10 09:50:09.189289 codegrade-16.1.8/codegrade/models/automatic_lti_role_enabled_setting.py
--rw-r--r--   0        0        0     3714 2023-03-10 09:50:09.377290 codegrade-16.1.8/codegrade/models/base_about.py
--rw-r--r--   0        0        0     3205 2023-03-10 09:50:09.233289 codegrade-16.1.8/codegrade/models/base_auto_test_quality_comment.py
--rw-r--r--   0        0        0     1690 2023-03-10 09:50:09.265289 codegrade-16.1.8/codegrade/models/base_comment_base.py
--rw-r--r--   0        0        0     2274 2023-03-10 09:50:09.297289 codegrade-16.1.8/codegrade/models/base_comment_base_with_extended_replies.py
--rw-r--r--   0        0        0     1857 2023-03-10 09:50:09.325290 codegrade-16.1.8/codegrade/models/base_comment_base_with_normal_replies.py
--rw-r--r--   0        0        0     4564 2023-03-10 09:50:09.389289 codegrade-16.1.8/codegrade/models/base_comment_reply.py
--rw-r--r--   0        0        0     2861 2023-03-10 09:50:09.417290 codegrade-16.1.8/codegrade/models/base_coupon.py
--rw-r--r--   0        0        0     2032 2023-03-10 09:50:09.425290 codegrade-16.1.8/codegrade/models/base_directory.py
--rw-r--r--   0        0        0     2752 2023-03-10 09:50:09.457290 codegrade-16.1.8/codegrade/models/base_error.py
--rw-r--r--   0        0        0     2831 2023-03-10 09:50:09.469290 codegrade-16.1.8/codegrade/models/base_file.py
--rw-r--r--   0        0        0    11095 2023-03-10 09:50:09.561290 codegrade-16.1.8/codegrade/models/base_lms_capabilities.py
--rw-r--r--   0        0        0     3246 2023-03-10 09:50:09.693290 codegrade-16.1.8/codegrade/models/base_lti1p1_provider.py
--rw-r--r--   0        0        0     3712 2023-03-10 09:50:09.613290 codegrade-16.1.8/codegrade/models/base_lti1p3_provider.py
--rw-r--r--   0        0        0     2648 2023-03-10 09:50:09.649290 codegrade-16.1.8/codegrade/models/base_lti_provider.py
--rw-r--r--   0        0        0     5105 2023-03-10 09:50:09.717290 codegrade-16.1.8/codegrade/models/base_notification.py
--rw-r--r--   0        0        0     1231 2023-03-10 09:50:09.713290 codegrade-16.1.8/codegrade/models/base_release_info.py
--rw-r--r--   0        0        0     1923 2023-03-10 09:50:09.745290 codegrade-16.1.8/codegrade/models/base_rubric_item.py
--rw-r--r--   0        0        0     1462 2023-03-10 09:50:09.745290 codegrade-16.1.8/codegrade/models/blackboard_zip_upload_enabled_setting.py
--rw-r--r--   0        0        0     1372 2023-03-10 09:50:09.765290 codegrade-16.1.8/codegrade/models/bulk_enroll_course_data.py
--rw-r--r--   0        0        0     1485 2023-03-10 09:50:09.773290 codegrade-16.1.8/codegrade/models/canvas_course_id_copying_enabled_setting.py
--rw-r--r--   0        0        0      321 2023-03-10 09:50:01.709277 codegrade-16.1.8/codegrade/models/cg_ignore_version.py
--rw-r--r--   0        0        0     4080 2023-03-10 09:50:09.833290 codegrade-16.1.8/codegrade/models/change_user_role_course_data.py
--rw-r--r--   0        0        0     2098 2023-03-10 09:50:09.805290 codegrade-16.1.8/codegrade/models/check_points_as_json.py
--rw-r--r--   0        0        0     1257 2023-03-10 09:50:09.829290 codegrade-16.1.8/codegrade/models/check_points_data.py
--rw-r--r--   0        0        0     1603 2023-03-10 09:50:09.853290 codegrade-16.1.8/codegrade/models/check_points_extra.py
--rw-r--r--   0        0        0     2115 2023-03-10 09:50:09.869290 codegrade-16.1.8/codegrade/models/check_points_input_as_json.py
--rw-r--r--   0        0        0     1211 2023-03-10 09:50:09.873290 codegrade-16.1.8/codegrade/models/clone_result.py
--rw-r--r--   0        0        0     2098 2023-03-10 09:50:10.077291 codegrade-16.1.8/codegrade/models/code_quality_as_json.py
--rw-r--r--   0        0        0     2908 2023-03-10 09:50:09.913290 codegrade-16.1.8/codegrade/models/code_quality_base_data.py
--rw-r--r--   0        0        0     2624 2023-03-10 09:50:09.957291 codegrade-16.1.8/codegrade/models/code_quality_data.py
--rw-r--r--   0        0        0     1603 2023-03-10 09:50:09.981290 codegrade-16.1.8/codegrade/models/code_quality_extra.py
--rw-r--r--   0        0        0     2115 2023-03-10 09:50:10.017291 codegrade-16.1.8/codegrade/models/code_quality_input_as_json.py
--rw-r--r--   0        0        0     2106 2023-03-10 09:50:10.049291 codegrade-16.1.8/codegrade/models/code_quality_penalties.py
--rw-r--r--   0        0        0     1760 2023-03-10 09:50:10.077291 codegrade-16.1.8/codegrade/models/column_range.py
--rw-r--r--   0        0        0      678 2023-03-10 09:50:10.085291 codegrade-16.1.8/codegrade/models/comment_base.py
--rw-r--r--   0        0        0      640 2023-03-10 09:50:10.089291 codegrade-16.1.8/codegrade/models/comment_reply.py
--rw-r--r--   0        0        0     2730 2023-03-10 09:50:10.125291 codegrade-16.1.8/codegrade/models/comment_reply_edit.py
--rw-r--r--   0        0        0      231 2023-03-10 09:50:02.033277 codegrade-16.1.8/codegrade/models/comment_reply_type.py
--rw-r--r--   0        0        0      223 2023-03-10 09:50:02.509278 codegrade-16.1.8/codegrade/models/comment_type.py
--rw-r--r--   0        0        0     1449 2023-03-10 09:50:10.117291 codegrade-16.1.8/codegrade/models/connect_repository_git_provider_data.py
--rw-r--r--   0        0        0     1386 2023-03-10 09:50:10.141291 codegrade-16.1.8/codegrade/models/copy_auto_test_data.py
--rw-r--r--   0        0        0     1444 2023-03-10 09:50:10.149291 codegrade-16.1.8/codegrade/models/copy_rubric_assignment_data.py
--rw-r--r--   0        0        0      572 2023-03-10 09:50:10.153291 codegrade-16.1.8/codegrade/models/coupon.py
--rw-r--r--   0        0        0     1676 2023-03-10 09:50:10.177291 codegrade-16.1.8/codegrade/models/coupon_data_parser.py
--rw-r--r--   0        0        0     2112 2023-03-10 09:50:10.189291 codegrade-16.1.8/codegrade/models/coupon_usage.py
--rw-r--r--   0        0        0     2257 2023-03-10 09:50:10.213291 codegrade-16.1.8/codegrade/models/coupon_with_code.py
--rw-r--r--   0        0        0     1994 2023-03-10 09:50:10.221291 codegrade-16.1.8/codegrade/models/coupon_without_code.py
--rw-r--r--   0        0        0     4395 2023-03-10 09:50:10.273291 codegrade-16.1.8/codegrade/models/course.py
--rw-r--r--   0        0        0     2016 2023-03-10 09:50:10.253291 codegrade-16.1.8/codegrade/models/course_bulk_enroll_result.py
--rw-r--r--   0        0        0     1456 2023-03-10 09:50:10.281291 codegrade-16.1.8/codegrade/models/course_bulk_register_enabled_setting.py
--rw-r--r--   0        0        0     1436 2023-03-10 09:50:10.301291 codegrade-16.1.8/codegrade/models/course_gradebook_enabled_setting.py
--rw-r--r--   0        0        0     1507 2023-03-10 09:50:10.309291 codegrade-16.1.8/codegrade/models/course_gradebook_render_warning_size_setting.py
--rw-r--r--   0        0        0     2046 2023-03-10 09:50:10.333291 codegrade-16.1.8/codegrade/models/course_of_course_price.py
--rw-r--r--   0        0        0    56729 2023-03-10 09:50:14.753300 codegrade-16.1.8/codegrade/models/course_perm_map.py
--rw-r--r--   0        0        0     5291 2023-03-10 09:50:10.377291 codegrade-16.1.8/codegrade/models/course_permission.py
--rw-r--r--   0        0        0     2415 2023-03-10 09:50:10.417291 codegrade-16.1.8/codegrade/models/course_price.py
--rw-r--r--   0        0        0     1430 2023-03-10 09:50:10.441291 codegrade-16.1.8/codegrade/models/course_register_enabled_setting.py
--rw-r--r--   0        0        0     1374 2023-03-10 09:50:10.461291 codegrade-16.1.8/codegrade/models/course_register_response.py
--rw-r--r--   0        0        0     2611 2023-03-10 09:50:10.501291 codegrade-16.1.8/codegrade/models/course_registration_link.py
--rw-r--r--   0        0        0     1938 2023-03-10 09:50:10.533291 codegrade-16.1.8/codegrade/models/course_role.py
--rw-r--r--   0        0        0     2743 2023-03-10 09:50:10.577292 codegrade-16.1.8/codegrade/models/course_role_as_json_with_perms.py
--rw-r--r--   0        0        0     2156 2023-03-10 09:50:10.609292 codegrade-16.1.8/codegrade/models/course_section.py
--rw-r--r--   0        0        0     1756 2023-03-10 09:50:10.633292 codegrade-16.1.8/codegrade/models/course_section_division.py
--rw-r--r--   0        0        0     1862 2023-03-10 09:50:10.665292 codegrade-16.1.8/codegrade/models/course_section_division_connection.py
--rw-r--r--   0        0        0     1530 2023-03-10 09:50:10.689292 codegrade-16.1.8/codegrade/models/course_section_division_user.py
--rw-r--r--   0        0        0     1847 2023-03-10 09:50:10.721292 codegrade-16.1.8/codegrade/models/course_snippet.py
--rw-r--r--   0        0        0      239 2023-03-10 09:50:01.409276 codegrade-16.1.8/codegrade/models/course_state.py
--rw-r--r--   0        0        0     1632 2023-03-10 09:50:10.745292 codegrade-16.1.8/codegrade/models/course_statistics_as_json.py
--rw-r--r--   0        0        0     1247 2023-03-10 09:50:10.765292 codegrade-16.1.8/codegrade/models/create_assignment_course_data.py
--rw-r--r--   0        0        0     1827 2023-03-10 09:50:10.797292 codegrade-16.1.8/codegrade/models/create_auto_test_data.py
--rw-r--r--   0        0        0     2744 2023-03-10 09:50:10.845292 codegrade-16.1.8/codegrade/models/create_comment_data.py
--rw-r--r--   0        0        0     2299 2023-03-10 09:50:10.881292 codegrade-16.1.8/codegrade/models/create_comment_reply_data.py
--rw-r--r--   0        0        0     2018 2023-03-10 09:50:10.913292 codegrade-16.1.8/codegrade/models/create_course_data.py
--rw-r--r--   0        0        0     1431 2023-03-10 09:50:10.937292 codegrade-16.1.8/codegrade/models/create_division_section_data.py
--rw-r--r--   0        0        0     2296 2023-03-10 09:50:10.969292 codegrade-16.1.8/codegrade/models/create_group_group_set_data.py
--rw-r--r--   0        0        0     2365 2023-03-10 09:50:11.009292 codegrade-16.1.8/codegrade/models/create_group_set_course_data.py
--rw-r--r--   0        0        0      613 2023-03-10 09:50:11.017292 codegrade-16.1.8/codegrade/models/create_lti_data.py
--rw-r--r--   0        0        0     1740 2023-03-10 09:50:11.041292 codegrade-16.1.8/codegrade/models/create_output_html_proxy_auto_test_data.py
--rw-r--r--   0        0        0     2074 2023-03-10 09:50:11.069292 codegrade-16.1.8/codegrade/models/create_proxy_submission_data.py
--rw-r--r--   0        0        0     1732 2023-03-10 09:50:11.097292 codegrade-16.1.8/codegrade/models/create_repository_git_provider_data.py
--rw-r--r--   0        0        0     1219 2023-03-10 09:50:11.117293 codegrade-16.1.8/codegrade/models/create_role_course_data.py
--rw-r--r--   0        0        0     1681 2023-03-10 09:50:11.145292 codegrade-16.1.8/codegrade/models/create_section_course_data.py
--rw-r--r--   0        0        0     1506 2023-03-10 09:50:11.169293 codegrade-16.1.8/codegrade/models/create_snippet_course_data.py
--rw-r--r--   0        0        0     1504 2023-03-10 09:50:11.193292 codegrade-16.1.8/codegrade/models/create_snippet_data.py
--rw-r--r--   0        0        0     2066 2023-03-10 09:50:11.225293 codegrade-16.1.8/codegrade/models/create_sso_provider_data.py
--rw-r--r--   0        0        0     2223 2023-03-10 09:50:11.429293 codegrade-16.1.8/codegrade/models/create_tenant_data.py
--rw-r--r--   0        0        0     1568 2023-03-10 09:50:11.457293 codegrade-16.1.8/codegrade/models/csv_large_file_limit_setting.py
--rw-r--r--   0        0        0     1432 2023-03-10 09:50:11.481293 codegrade-16.1.8/codegrade/models/csv_too_many_errors_limit_setting.py
--rw-r--r--   0        0        0      207 2023-03-10 09:50:02.481278 codegrade-16.1.8/codegrade/models/currency.py
--rw-r--r--   0        0        0     2135 2023-03-10 09:50:11.517293 codegrade-16.1.8/codegrade/models/custom_output_as_json.py
--rw-r--r--   0        0        0     1554 2023-03-10 09:50:11.541293 codegrade-16.1.8/codegrade/models/custom_output_data.py
--rw-r--r--   0        0        0     1616 2023-03-10 09:50:11.569293 codegrade-16.1.8/codegrade/models/custom_output_extra.py
--rw-r--r--   0        0        0     2125 2023-03-10 09:50:11.601293 codegrade-16.1.8/codegrade/models/custom_output_input_as_json.py
--rw-r--r--   0        0        0     2838 2023-03-10 09:50:11.649293 codegrade-16.1.8/codegrade/models/custom_output_log.py
--rw-r--r--   0        0        0     2536 2023-03-10 09:50:11.685293 codegrade-16.1.8/codegrade/models/custom_output_log_base.py
--rw-r--r--   0        0        0     2361 2023-03-10 09:50:11.721293 codegrade-16.1.8/codegrade/models/deleted_comment_reply.py
--rw-r--r--   0        0        0      283 2023-03-10 09:50:02.505278 codegrade-16.1.8/codegrade/models/deletion_type.py
--rw-r--r--   0        0        0     2419 2023-03-10 09:50:11.757293 codegrade-16.1.8/codegrade/models/directory_with_children.py
--rw-r--r--   0        0        0     2493 2023-03-10 09:50:11.793294 codegrade-16.1.8/codegrade/models/disabled_setting_exception.py
--rw-r--r--   0        0        0     1450 2023-03-10 09:50:11.817294 codegrade-16.1.8/codegrade/models/editor_enabled_for_teachers_setting.py
--rw-r--r--   0        0        0     1380 2023-03-10 09:50:11.845294 codegrade-16.1.8/codegrade/models/editor_enabled_setting.py
--rw-r--r--   0        0        0      267 2023-03-10 09:50:02.369278 codegrade-16.1.8/codegrade/models/email_notification_types.py
--rw-r--r--   0        0        0     1424 2023-03-10 09:50:11.873294 codegrade-16.1.8/codegrade/models/email_students_enabled_setting.py
--rw-r--r--   0        0        0     5504 2023-03-10 09:50:11.949294 codegrade-16.1.8/codegrade/models/email_users_course_data.py
--rw-r--r--   0        0        0     1447 2023-03-10 09:50:11.973294 codegrade-16.1.8/codegrade/models/exam_login_max_length_setting.py
--rw-r--r--   0        0        0     2235 2023-03-10 09:50:12.009294 codegrade-16.1.8/codegrade/models/export_assignment_csv_data.py
--rw-r--r--   0        0        0      693 2023-03-10 09:50:12.017294 codegrade-16.1.8/codegrade/models/export_assignment_data.py
--rw-r--r--   0        0        0     1685 2023-03-10 09:50:12.045294 codegrade-16.1.8/codegrade/models/export_assignment_files_data.py
--rw-r--r--   0        0        0    10220 2023-03-10 09:50:12.365295 codegrade-16.1.8/codegrade/models/extended_auto_test_result.py
--rw-r--r--   0        0        0     3231 2023-03-10 09:50:12.413295 codegrade-16.1.8/codegrade/models/extended_auto_test_run.py
--rw-r--r--   0        0        0     3342 2023-03-10 09:50:12.461295 codegrade-16.1.8/codegrade/models/extended_course.py
--rw-r--r--   0        0        0     2126 2023-03-10 09:50:12.497295 codegrade-16.1.8/codegrade/models/extended_course_registration_link.py
--rw-r--r--   0        0        0     1930 2023-03-10 09:50:12.529295 codegrade-16.1.8/codegrade/models/extended_course_section.py
--rw-r--r--   0        0        0     2258 2023-03-10 09:50:12.565295 codegrade-16.1.8/codegrade/models/extended_group.py
--rw-r--r--   0        0        0     3144 2023-03-10 09:50:12.613295 codegrade-16.1.8/codegrade/models/extended_job.py
--rw-r--r--   0        0        0     3042 2023-03-10 09:50:12.657295 codegrade-16.1.8/codegrade/models/extended_non_deleted_comment_reply.py
--rw-r--r--   0        0        0     4255 2023-03-10 09:50:12.717295 codegrade-16.1.8/codegrade/models/extended_tenant.py
--rw-r--r--   0        0        0     2456 2023-03-10 09:50:12.753295 codegrade-16.1.8/codegrade/models/extended_transaction.py
--rw-r--r--   0        0        0     4999 2023-03-10 09:50:12.825296 codegrade-16.1.8/codegrade/models/extended_user.py
--rw-r--r--   0        0        0     3868 2023-03-10 09:50:12.881296 codegrade-16.1.8/codegrade/models/extended_work.py
--rw-r--r--   0        0        0     1901 2023-03-10 09:50:12.913296 codegrade-16.1.8/codegrade/models/extract_file_tree_directory.py
--rw-r--r--   0        0        0     1168 2023-03-10 09:50:12.933296 codegrade-16.1.8/codegrade/models/extract_file_tree_file.py
--rw-r--r--   0        0        0     2477 2023-03-10 09:50:12.973296 codegrade-16.1.8/codegrade/models/failed_to_send_email_exception.py
--rw-r--r--   0        0        0     2628 2023-03-10 09:50:13.009296 codegrade-16.1.8/codegrade/models/feedback_base.py
--rw-r--r--   0        0        0     1511 2023-03-10 09:50:13.037296 codegrade-16.1.8/codegrade/models/feedback_threads_initially_collapsed_setting.py
--rw-r--r--   0        0        0     3676 2023-03-10 09:50:13.305297 codegrade-16.1.8/codegrade/models/feedback_with_replies.py
--rw-r--r--   0        0        0     3630 2023-03-10 09:50:13.357297 codegrade-16.1.8/codegrade/models/feedback_without_replies.py
--rw-r--r--   0        0        0     2485 2023-03-10 09:50:13.393297 codegrade-16.1.8/codegrade/models/file_deletion.py
--rw-r--r--   0        0        0     1850 2023-03-10 09:50:13.425297 codegrade-16.1.8/codegrade/models/file_rule.py
--rw-r--r--   0        0        0     2130 2023-03-10 09:50:13.457297 codegrade-16.1.8/codegrade/models/file_rule_input_data.py
--rw-r--r--   0        0        0      569 2023-03-10 09:50:13.465297 codegrade-16.1.8/codegrade/models/file_tree.py
--rw-r--r--   0        0        0      205 2023-03-10 09:50:02.185278 codegrade-16.1.8/codegrade/models/file_type.py
--rw-r--r--   0        0        0     2462 2023-03-10 09:50:13.509297 codegrade-16.1.8/codegrade/models/finalized_lti1p1_provider.py
--rw-r--r--   0        0        0     2594 2023-03-10 09:50:13.549297 codegrade-16.1.8/codegrade/models/finalized_lti1p3_provider.py
--rw-r--r--   0        0        0     1416 2023-03-10 09:50:13.573297 codegrade-16.1.8/codegrade/models/find_element_interval_setting.py
--rw-r--r--   0        0        0     1418 2023-03-10 09:50:13.601297 codegrade-16.1.8/codegrade/models/find_element_max_tries_setting.py
--rw-r--r--   0        0        0     2233 2023-03-10 09:50:13.637297 codegrade-16.1.8/codegrade/models/first_phase_lti_launch_exception.py
--rw-r--r--   0        0        0     1139 2023-03-10 09:50:13.657297 codegrade-16.1.8/codegrade/models/fixture_like.py
--rw-r--r--   0        0        0     1402 2023-03-10 09:50:13.685297 codegrade-16.1.8/codegrade/models/fraction.py
--rw-r--r--   0        0        0    50981 2023-03-10 09:50:16.541303 codegrade-16.1.8/codegrade/models/frontend_site_settings.py
--rw-r--r--   0        0        0     1784 2023-03-10 09:50:14.781300 codegrade-16.1.8/codegrade/models/general_feedback_comment_base.py
--rw-r--r--   0        0        0     1994 2023-03-10 09:50:14.809300 codegrade-16.1.8/codegrade/models/general_feedback_comment_base_with_extended_replies.py
--rw-r--r--   0        0        0     1212 2023-03-10 09:50:14.829300 codegrade-16.1.8/codegrade/models/general_feedback_extra.py
--rw-r--r--   0        0        0     1848 2023-03-10 09:50:14.861300 codegrade-16.1.8/codegrade/models/git_repositories_page.py
--rw-r--r--   0        0        0     1720 2023-03-10 09:50:14.889300 codegrade-16.1.8/codegrade/models/git_repository_like.py
--rw-r--r--   0        0        0     1491 2023-03-10 09:50:14.913300 codegrade-16.1.8/codegrade/models/git_user_info.py
--rw-r--r--   0        0        0    14535 2023-03-10 09:50:15.173300 codegrade-16.1.8/codegrade/models/global_perm_map.py
--rw-r--r--   0        0        0     1477 2023-03-10 09:50:15.189300 codegrade-16.1.8/codegrade/models/global_permission.py
--rw-r--r--   0        0        0     3176 2023-03-10 09:50:15.237301 codegrade-16.1.8/codegrade/models/grade_history.py
--rw-r--r--   0        0        0      287 2023-03-10 09:50:02.489278 codegrade-16.1.8/codegrade/models/grade_origin.py
--rw-r--r--   0        0        0     1475 2023-03-10 09:50:15.265301 codegrade-16.1.8/codegrade/models/grading_notifications_enabled_setting.py
--rw-r--r--   0        0        0     2527 2023-03-10 09:50:15.301301 codegrade-16.1.8/codegrade/models/group.py
--rw-r--r--   0        0        0     2470 2023-03-10 09:50:15.341301 codegrade-16.1.8/codegrade/models/group_not_ready_for_submission_exception.py
--rw-r--r--   0        0        0     2354 2023-03-10 09:50:15.373301 codegrade-16.1.8/codegrade/models/group_set.py
--rw-r--r--   0        0        0     1380 2023-03-10 09:50:15.401301 codegrade-16.1.8/codegrade/models/groups_enabled_setting.py
--rw-r--r--   0        0        0     1290 2023-03-10 09:50:15.421301 codegrade-16.1.8/codegrade/models/has_unread_notifcation_json.py
--rw-r--r--   0        0        0     3388 2023-03-10 09:50:15.469301 codegrade-16.1.8/codegrade/models/health_information.py
--rw-r--r--   0        0        0      231 2023-03-10 09:50:00.865275 codegrade-16.1.8/codegrade/models/ignore_handling.py
--rw-r--r--   0        0        0     5316 2023-03-10 09:50:15.537301 codegrade-16.1.8/codegrade/models/ignored_files_exception.py
--rw-r--r--   0        0        0     1462 2023-03-10 09:50:15.561301 codegrade-16.1.8/codegrade/models/import_into_assignment_data.py
--rw-r--r--   0        0        0     1317 2023-03-10 09:50:15.581301 codegrade-16.1.8/codegrade/models/import_into_course_data.py
--rw-r--r--   0        0        0     1519 2023-03-10 09:50:15.609301 codegrade-16.1.8/codegrade/models/incremental_rubric_submission_enabled_setting.py
--rw-r--r--   0        0        0     1927 2023-03-10 09:50:15.641301 codegrade-16.1.8/codegrade/models/inline_feedback_comment_base.py
--rw-r--r--   0        0        0     2137 2023-03-10 09:50:15.673302 codegrade-16.1.8/codegrade/models/inline_feedback_comment_base_with_extended_replies.py
--rw-r--r--   0        0        0     1863 2023-03-10 09:50:15.705302 codegrade-16.1.8/codegrade/models/inline_feedback_extra.py
--rw-r--r--   0        0        0     2040 2023-03-10 09:50:15.741302 codegrade-16.1.8/codegrade/models/invalid_group_exception.py
--rw-r--r--   0        0        0     3002 2023-03-10 09:50:15.781302 codegrade-16.1.8/codegrade/models/invalid_io_cases_exception.py
--rw-r--r--   0        0        0     2052 2023-03-10 09:50:15.813302 codegrade-16.1.8/codegrade/models/invalid_options_exception.py
--rw-r--r--   0        0        0     2048 2023-03-10 09:50:15.849302 codegrade-16.1.8/codegrade/models/io_test_as_json.py
--rw-r--r--   0        0        0     1606 2023-03-10 09:50:15.877302 codegrade-16.1.8/codegrade/models/io_test_base_data.py
--rw-r--r--   0        0        0     2008 2023-03-10 09:50:15.909302 codegrade-16.1.8/codegrade/models/io_test_data.py
--rw-r--r--   0        0        0     1512 2023-03-10 09:50:15.937302 codegrade-16.1.8/codegrade/models/io_test_extra.py
--rw-r--r--   0        0        0     2065 2023-03-10 09:50:15.973302 codegrade-16.1.8/codegrade/models/io_test_input_as_json.py
--rw-r--r--   0        0        0     2770 2023-03-10 09:50:16.413303 codegrade-16.1.8/codegrade/models/io_test_input_case.py
--rw-r--r--   0        0        0     1568 2023-03-10 09:50:16.437303 codegrade-16.1.8/codegrade/models/io_test_log.py
--rw-r--r--   0        0        0      319 2023-03-10 09:50:02.437278 codegrade-16.1.8/codegrade/models/io_test_option.py
--rw-r--r--   0        0        0     4604 2023-03-10 09:50:16.509303 codegrade-16.1.8/codegrade/models/io_test_step_log.py
--rw-r--r--   0        0        0     1678 2023-03-10 09:50:16.537303 codegrade-16.1.8/codegrade/models/io_test_step_log_base.py
--rw-r--r--   0        0        0     1450 2023-03-10 09:50:16.561303 codegrade-16.1.8/codegrade/models/is_admin_permission_enabled_setting.py
--rw-r--r--   0        0        0     1889 2023-03-10 09:50:16.577304 codegrade-16.1.8/codegrade/models/job.py
--rw-r--r--   0        0        0     7412 2023-03-10 09:50:16.665304 codegrade-16.1.8/codegrade/models/json_create_auto_test.py
--rw-r--r--   0        0        0     1612 2023-03-10 09:50:16.601303 codegrade-16.1.8/codegrade/models/json_create_tenant.py
--rw-r--r--   0        0        0     6846 2023-03-10 09:50:16.697304 codegrade-16.1.8/codegrade/models/json_patch_auto_test.py
--rw-r--r--   0        0        0     3286 2023-03-10 09:50:16.713304 codegrade-16.1.8/codegrade/models/json_patch_submit_types_assignment.py
--rw-r--r--   0        0        0     2078 2023-03-10 09:50:16.733304 codegrade-16.1.8/codegrade/models/junit_test_as_json.py
--rw-r--r--   0        0        0     1177 2023-03-10 09:50:16.737304 codegrade-16.1.8/codegrade/models/junit_test_base_data.py
--rw-r--r--   0        0        0     2965 2023-03-10 09:50:16.777304 codegrade-16.1.8/codegrade/models/junit_test_data.py
--rw-r--r--   0        0        0     1577 2023-03-10 09:50:16.761304 codegrade-16.1.8/codegrade/models/junit_test_extra.py
--rw-r--r--   0        0        0     2095 2023-03-10 09:50:16.797304 codegrade-16.1.8/codegrade/models/junit_test_input_as_json.py
--rw-r--r--   0        0        0     2345 2023-03-10 09:50:16.813304 codegrade-16.1.8/codegrade/models/junit_test_log.py
--rw-r--r--   0        0        0     2517 2023-03-10 09:50:16.833304 codegrade-16.1.8/codegrade/models/junit_test_log_base.py
--rw-r--r--   0        0        0     1465 2023-03-10 09:50:16.841304 codegrade-16.1.8/codegrade/models/jwt_access_token_expires_setting.py
--rw-r--r--   0        0        0     4695 2023-03-10 09:50:16.893304 codegrade-16.1.8/codegrade/models/legacy_features.py
--rw-r--r--   0        0        0     1501 2023-03-10 09:50:16.865304 codegrade-16.1.8/codegrade/models/line_range.py
--rw-r--r--   0        0        0     1902 2023-03-10 09:50:16.897304 codegrade-16.1.8/codegrade/models/linter_comment.py
--rw-r--r--   0        0        0     1386 2023-03-10 09:50:16.921304 codegrade-16.1.8/codegrade/models/linters_enabled_setting.py
--rw-r--r--   0        0        0     3208 2023-03-10 09:50:16.941304 codegrade-16.1.8/codegrade/models/lms_capabilities.py
--rw-r--r--   0        0        0     1481 2023-03-10 09:50:16.945304 codegrade-16.1.8/codegrade/models/login_token_before_time_setting.py
--rw-r--r--   0        0        0     4556 2023-03-10 09:50:17.357305 codegrade-16.1.8/codegrade/models/login_user_data.py
--rw-r--r--   0        0        0      678 2023-03-10 09:50:16.953304 codegrade-16.1.8/codegrade/models/lti1p1_provider.py
--rw-r--r--   0        0        0     2791 2023-03-10 09:50:16.993304 codegrade-16.1.8/codegrade/models/lti1p1_provider_data.py
--rw-r--r--   0        0        0      678 2023-03-10 09:50:17.001304 codegrade-16.1.8/codegrade/models/lti1p3_provider.py
--rw-r--r--   0        0        0     2820 2023-03-10 09:50:17.061304 codegrade-16.1.8/codegrade/models/lti1p3_provider_data.py
--rw-r--r--   0        0        0     1558 2023-03-10 09:50:17.089305 codegrade-16.1.8/codegrade/models/lti1p3_provider_presentation_as_json.py
--rw-r--r--   0        0        0     1362 2023-03-10 09:50:17.113305 codegrade-16.1.8/codegrade/models/lti_enabled_setting.py
--rw-r--r--   0        0        0     1458 2023-03-10 09:50:17.141305 codegrade-16.1.8/codegrade/models/lti_lock_date_copying_enabled_setting.py
--rw-r--r--   0        0        0      976 2023-03-10 09:50:17.149305 codegrade-16.1.8/codegrade/models/lti_provider_base.py
--rw-r--r--   0        0        0     1592 2023-03-10 09:50:17.177305 codegrade-16.1.8/codegrade/models/max_document_update_size_setting.py
--rw-r--r--   0        0        0     1568 2023-03-10 09:50:17.205305 codegrade-16.1.8/codegrade/models/max_dynamo_file_size_setting.py
--rw-r--r--   0        0        0     1604 2023-03-10 09:50:17.233305 codegrade-16.1.8/codegrade/models/max_dynamo_submission_size_setting.py
--rw-r--r--   0        0        0     1530 2023-03-10 09:50:17.261305 codegrade-16.1.8/codegrade/models/max_file_size_setting.py
--rw-r--r--   0        0        0     1574 2023-03-10 09:50:17.289305 codegrade-16.1.8/codegrade/models/max_large_upload_size_setting.py
--rw-r--r--   0        0        0     1348 2023-03-10 09:50:17.313305 codegrade-16.1.8/codegrade/models/max_lines_setting.py
--rw-r--r--   0        0        0     1435 2023-03-10 09:50:17.341305 codegrade-16.1.8/codegrade/models/max_mirror_file_age_setting.py
--rw-r--r--   0        0        0     1580 2023-03-10 09:50:17.373305 codegrade-16.1.8/codegrade/models/max_normal_upload_size_setting.py
--rw-r--r--   0        0        0     1400 2023-03-10 09:50:17.385305 codegrade-16.1.8/codegrade/models/max_number_of_files_setting.py
--rw-r--r--   0        0        0     1422 2023-03-10 09:50:17.397305 codegrade-16.1.8/codegrade/models/max_plagiarism_matches_setting.py
--rw-r--r--   0        0        0     1424 2023-03-10 09:50:17.409305 codegrade-16.1.8/codegrade/models/max_user_setting_amount_setting.py
--rw-r--r--   0        0        0     1524 2023-03-10 09:50:17.425305 codegrade-16.1.8/codegrade/models/metric_evaluation_time_chunk_size_setting.py
--rw-r--r--   0        0        0     1489 2023-03-10 09:50:17.437305 codegrade-16.1.8/codegrade/models/metric_evaluation_time_limit_setting.py
--rw-r--r--   0        0        0     1430 2023-03-10 09:50:17.449305 codegrade-16.1.8/codegrade/models/metric_event_buffer_size_setting.py
--rw-r--r--   0        0        0     1436 2023-03-10 09:50:17.465305 codegrade-16.1.8/codegrade/models/metric_gathering_enabled_setting.py
--rw-r--r--   0        0        0     1481 2023-03-10 09:50:17.477306 codegrade-16.1.8/codegrade/models/metric_gathering_event_interval_setting.py
--rw-r--r--   0        0        0     1493 2023-03-10 09:50:17.489305 codegrade-16.1.8/codegrade/models/metric_gathering_expressions_setting.py
--rw-r--r--   0        0        0     1510 2023-03-10 09:50:17.505305 codegrade-16.1.8/codegrade/models/metric_gathering_time_interval_setting.py
--rw-r--r--   0        0        0     1398 2023-03-10 09:50:17.517305 codegrade-16.1.8/codegrade/models/min_password_score_setting.py
--rw-r--r--   0        0        0     2523 2023-03-10 09:50:17.541306 codegrade-16.1.8/codegrade/models/mirror_file_result.py
--rw-r--r--   0        0        0     2164 2023-03-10 09:50:17.549306 codegrade-16.1.8/codegrade/models/missing_cookie_error.py
--rw-r--r--   0        0        0     1863 2023-03-10 09:50:17.569306 codegrade-16.1.8/codegrade/models/missing_file.py
--rw-r--r--   0        0        0     1539 2023-03-10 09:50:17.577306 codegrade-16.1.8/codegrade/models/new_auto_test_allowed_initial_build_ids_setting.py
--rw-r--r--   0        0        0     1534 2023-03-10 09:50:17.597306 codegrade-16.1.8/codegrade/models/new_auto_test_build_max_command_time_setting.py
--rw-r--r--   0        0        0     1641 2023-03-10 09:50:17.605306 codegrade-16.1.8/codegrade/models/new_auto_test_build_output_limit_setting.py
--rw-r--r--   0        0        0     1458 2023-03-10 09:50:17.621306 codegrade-16.1.8/codegrade/models/new_auto_test_copying_enabled_setting.py
--rw-r--r--   0        0        0     1539 2023-03-10 09:50:17.633306 codegrade-16.1.8/codegrade/models/new_auto_test_current_initial_build_ids_setting.py
--rw-r--r--   0        0        0     1414 2023-03-10 09:50:17.649306 codegrade-16.1.8/codegrade/models/new_auto_test_enabled_setting.py
--rw-r--r--   0        0        0     1458 2023-03-10 09:50:17.657306 codegrade-16.1.8/codegrade/models/new_auto_test_initial_build_id_setting.py
--rw-r--r--   0        0        0     1626 2023-03-10 09:50:17.677306 codegrade-16.1.8/codegrade/models/new_auto_test_max_dynamodb_size_setting.py
--rw-r--r--   0        0        0     1602 2023-03-10 09:50:17.689306 codegrade-16.1.8/codegrade/models/new_auto_test_max_file_size_setting.py
--rw-r--r--   0        0        0     1620 2023-03-10 09:50:17.705306 codegrade-16.1.8/codegrade/models/new_auto_test_max_storage_size_setting.py
--rw-r--r--   0        0        0     1514 2023-03-10 09:50:17.713306 codegrade-16.1.8/codegrade/models/new_auto_test_old_submission_age_setting.py
--rw-r--r--   0        0        0     1528 2023-03-10 09:50:17.729306 codegrade-16.1.8/codegrade/models/new_auto_test_test_max_command_time_setting.py
--rw-r--r--   0        0        0     1626 2023-03-10 09:50:17.741306 codegrade-16.1.8/codegrade/models/new_auto_test_test_output_limit_setting.py
--rw-r--r--   0        0        0     1285 2023-03-10 09:50:17.749306 codegrade-16.1.8/codegrade/models/no_permissions.py
--rw-r--r--   0        0        0     3658 2023-03-10 09:50:17.793306 codegrade-16.1.8/codegrade/models/non_deleted_comment_reply.py
--rw-r--r--   0        0        0     4472 2023-03-10 09:50:18.045306 codegrade-16.1.8/codegrade/models/non_finalized_lti1p1_provider.py
--rw-r--r--   0        0        0     7279 2023-03-10 09:50:17.893306 codegrade-16.1.8/codegrade/models/non_finalized_lti1p3_provider.py
--rw-r--r--   0        0        0     1385 2023-03-10 09:50:17.917306 codegrade-16.1.8/codegrade/models/non_present_preference.py
--rw-r--r--   0        0        0      868 2023-03-10 09:50:17.929306 codegrade-16.1.8/codegrade/models/notification.py
--rw-r--r--   0        0        0     3037 2023-03-10 09:50:17.969306 codegrade-16.1.8/codegrade/models/notification_comment_reply_notification_as_json.py
--rw-r--r--   0        0        0     2729 2023-03-10 09:50:18.005306 codegrade-16.1.8/codegrade/models/notification_general_feedback_reply_notification_as_json.py
--rw-r--r--   0        0        0     1457 2023-03-10 09:50:18.033306 codegrade-16.1.8/codegrade/models/notification_poll_time_setting.py
--rw-r--r--   0        0        0      253 2023-03-10 09:50:01.025276 codegrade-16.1.8/codegrade/models/notification_reasons.py
--rw-r--r--   0        0        0     1855 2023-03-10 09:50:18.065306 codegrade-16.1.8/codegrade/models/notification_setting.py
--rw-r--r--   0        0        0     2163 2023-03-10 09:50:18.073306 codegrade-16.1.8/codegrade/models/notification_setting_option.py
--rw-r--r--   0        0        0     1327 2023-03-10 09:50:18.085306 codegrade-16.1.8/codegrade/models/notifications_json.py
--rw-r--r--   0        0        0     2150 2023-03-10 09:50:18.109306 codegrade-16.1.8/codegrade/models/oauth_provider.py
--rw-r--r--   0        0        0     2231 2023-03-10 09:50:18.121307 codegrade-16.1.8/codegrade/models/oauth_token.py
--rw-r--r--   0        0        0     1698 2023-03-10 09:50:18.137307 codegrade-16.1.8/codegrade/models/option.py
--rw-r--r--   0        0        0     1691 2023-03-10 09:50:18.149306 codegrade-16.1.8/codegrade/models/options_input_data.py
--rw-r--r--   0        0        0     1993 2023-03-10 09:50:18.169306 codegrade-16.1.8/codegrade/models/parse_api_exception.py
--rw-r--r--   0        0        0    92507 2023-03-10 09:50:24.449316 codegrade-16.1.8/codegrade/models/partial_all_site_settings.py
--rw-r--r--   0        0        0     1555 2023-03-10 09:50:18.197306 codegrade-16.1.8/codegrade/models/patch1_p1_provider_lti_data.py
--rw-r--r--   0        0        0     4217 2023-03-10 09:50:18.257307 codegrade-16.1.8/codegrade/models/patch1_p3_provider_lti_data.py
--rw-r--r--   0        0        0     1355 2023-03-10 09:50:18.277307 codegrade-16.1.8/codegrade/models/patch_all_notification_data.py
--rw-r--r--   0        0        0    15935 2023-03-10 09:50:18.781307 codegrade-16.1.8/codegrade/models/patch_assignment_data.py
--rw-r--r--   0        0        0     1818 2023-03-10 09:50:18.813307 codegrade-16.1.8/codegrade/models/patch_auto_test_data.py
--rw-r--r--   0        0        0     1228 2023-03-10 09:50:18.837308 codegrade-16.1.8/codegrade/models/patch_comment_reply_data.py
--rw-r--r--   0        0        0     2129 2023-03-10 09:50:18.869308 codegrade-16.1.8/codegrade/models/patch_course_data.py
--rw-r--r--   0        0        0     1240 2023-03-10 09:50:18.893308 codegrade-16.1.8/codegrade/models/patch_grader_submission_data.py
--rw-r--r--   0        0        0     1248 2023-03-10 09:50:18.913308 codegrade-16.1.8/codegrade/models/patch_notification_data.py
--rw-r--r--   0        0        0     1992 2023-03-10 09:50:18.941308 codegrade-16.1.8/codegrade/models/patch_notification_setting_user_setting_data.py
--rw-r--r--   0        0        0     1497 2023-03-10 09:50:18.965308 codegrade-16.1.8/codegrade/models/patch_provider_lti_data.py
--rw-r--r--   0        0        0     1858 2023-03-10 09:50:18.993308 codegrade-16.1.8/codegrade/models/patch_role_course_data.py
--rw-r--r--   0        0        0     1828 2023-03-10 09:50:19.021308 codegrade-16.1.8/codegrade/models/patch_role_data.py
--rw-r--r--   0        0        0     1858 2023-03-10 09:50:19.053308 codegrade-16.1.8/codegrade/models/patch_role_tenant_data.py
--rw-r--r--   0        0        0     1966 2023-03-10 09:50:19.081308 codegrade-16.1.8/codegrade/models/patch_rubric_category_type_assignment_data.py
--rw-r--r--   0        0        0     2946 2023-03-10 09:50:19.129308 codegrade-16.1.8/codegrade/models/patch_rubric_result_submission_data.py
--rw-r--r--   0        0        0     1478 2023-03-10 09:50:19.157308 codegrade-16.1.8/codegrade/models/patch_section_data.py
--rw-r--r--   0        0        0     1378 2023-03-10 09:50:19.177308 codegrade-16.1.8/codegrade/models/patch_settings_tenant_data.py
--rw-r--r--   0        0        0     1369 2023-03-10 09:50:19.197308 codegrade-16.1.8/codegrade/models/patch_site_settings_data.py
--rw-r--r--   0        0        0     1501 2023-03-10 09:50:19.225308 codegrade-16.1.8/codegrade/models/patch_snippet_course_data.py
--rw-r--r--   0        0        0     1499 2023-03-10 09:50:19.249308 codegrade-16.1.8/codegrade/models/patch_snippet_data.py
--rw-r--r--   0        0        0     2019 2023-03-10 09:50:19.281308 codegrade-16.1.8/codegrade/models/patch_submission_data.py
--rw-r--r--   0        0        0     1945 2023-03-10 09:50:19.313308 codegrade-16.1.8/codegrade/models/patch_submit_types_assignment_data.py
--rw-r--r--   0        0        0     2987 2023-03-10 09:50:19.357308 codegrade-16.1.8/codegrade/models/patch_tenant_data.py
--rw-r--r--   0        0        0     1583 2023-03-10 09:50:19.381308 codegrade-16.1.8/codegrade/models/patch_ui_preference_user_setting_data.py
--rw-r--r--   0        0        0     3228 2023-03-10 09:50:19.433308 codegrade-16.1.8/codegrade/models/patch_user_data.py
--rw-r--r--   0        0        0     1240 2023-03-10 09:50:19.453308 codegrade-16.1.8/codegrade/models/pay_with_coupon_course_price_data.py
--rw-r--r--   0        0        0     1418 2023-03-10 09:50:19.481308 codegrade-16.1.8/codegrade/models/peer_feedback_enabled_setting.py
--rw-r--r--   0        0        0     3297 2023-03-10 09:50:19.525308 codegrade-16.1.8/codegrade/models/permission_exception.py
--rw-r--r--   0        0        0     6831 2023-03-10 09:50:19.613309 codegrade-16.1.8/codegrade/models/plagiarism_run.py
--rw-r--r--   0        0        0     1933 2023-03-10 09:50:19.641309 codegrade-16.1.8/codegrade/models/plagiarism_run_plagiarism_assignment_as_json.py
--rw-r--r--   0        0        0     1859 2023-03-10 09:50:19.673309 codegrade-16.1.8/codegrade/models/plagiarism_run_plagiarism_course_as_json.py
--rw-r--r--   0        0        0      371 2023-03-10 09:50:02.345278 codegrade-16.1.8/codegrade/models/plagiarism_state.py
--rw-r--r--   0        0        0     1752 2023-03-10 09:50:19.701309 codegrade-16.1.8/codegrade/models/post_oauth_token_data.py
--rw-r--r--   0        0        0     1668 2023-03-10 09:50:19.729309 codegrade-16.1.8/codegrade/models/present_preference.py
--rw-r--r--   0        0        0     1087 2023-03-10 09:50:19.753309 codegrade-16.1.8/codegrade/models/proxy.py
--rw-r--r--   0        0        0     1506 2023-03-10 09:50:19.777309 codegrade-16.1.8/codegrade/models/put_description_assignment_data.py
--rw-r--r--   0        0        0     3196 2023-03-10 09:50:19.825309 codegrade-16.1.8/codegrade/models/put_enroll_link_course_data.py
--rw-r--r--   0        0        0     2542 2023-03-10 09:50:19.861309 codegrade-16.1.8/codegrade/models/put_price_course_data.py
--rw-r--r--   0        0        0     2542 2023-03-10 09:50:19.893309 codegrade-16.1.8/codegrade/models/put_price_tenant_data.py
--rw-r--r--   0        0        0     2839 2023-03-10 09:50:19.933309 codegrade-16.1.8/codegrade/models/put_rubric_assignment_data.py
--rw-r--r--   0        0        0      269 2023-03-10 09:50:01.977277 codegrade-16.1.8/codegrade/models/quality_comment_severity.py
--rw-r--r--   0        0        0     2164 2023-03-10 09:50:19.969309 codegrade-16.1.8/codegrade/models/quality_test_log.py
--rw-r--r--   0        0        0     2531 2023-03-10 09:50:20.009309 codegrade-16.1.8/codegrade/models/quality_test_log_base.py
--rw-r--r--   0        0        0     1392 2023-03-10 09:50:20.033309 codegrade-16.1.8/codegrade/models/register_enabled_setting.py
--rw-r--r--   0        0        0     2429 2023-03-10 09:50:20.069309 codegrade-16.1.8/codegrade/models/register_user_data.py
--rw-r--r--   0        0        0     2153 2023-03-10 09:50:20.101309 codegrade-16.1.8/codegrade/models/register_user_with_link_course_data.py
--rw-r--r--   0        0        0     3661 2023-03-10 09:50:20.157309 codegrade-16.1.8/codegrade/models/release_info.py
--rw-r--r--   0        0        0     1465 2023-03-10 09:50:20.185310 codegrade-16.1.8/codegrade/models/release_message_max_time_setting.py
--rw-r--r--   0        0        0     1205 2023-03-10 09:50:20.205309 codegrade-16.1.8/codegrade/models/rename_group_group_data.py
--rw-r--r--   0        0        0     1406 2023-03-10 09:50:20.229310 codegrade-16.1.8/codegrade/models/render_html_enabled_setting.py
--rw-r--r--   0        0        0     1421 2023-03-10 09:50:20.257310 codegrade-16.1.8/codegrade/models/reset_token_time_setting.py
--rw-r--r--   0        0        0     8360 2023-03-10 09:50:20.665310 codegrade-16.1.8/codegrade/models/result_data_get_auto_test_get.py
--rw-r--r--   0        0        0     2477 2023-03-10 09:50:20.701310 codegrade-16.1.8/codegrade/models/result_data_get_task_result_get_all.py
--rw-r--r--   0        0        0     1770 2023-03-10 09:50:20.729310 codegrade-16.1.8/codegrade/models/result_data_post_login_link_login.py
--rw-r--r--   0        0        0     1880 2023-03-10 09:50:20.757310 codegrade-16.1.8/codegrade/models/result_data_post_section_create_division.py
--rw-r--r--   0        0        0     1750 2023-03-10 09:50:20.785310 codegrade-16.1.8/codegrade/models/result_data_post_user_login.py
--rw-r--r--   0        0        0     1762 2023-03-10 09:50:20.817310 codegrade-16.1.8/codegrade/models/result_data_post_user_register.py
--rw-r--r--   0        0        0     2391 2023-03-10 09:50:20.853310 codegrade-16.1.8/codegrade/models/role_as_json_with_perms.py
--rw-r--r--   0        0        0     1940 2023-03-10 09:50:20.881311 codegrade-16.1.8/codegrade/models/root_file_trees_json.py
--rw-r--r--   0        0        0      241 2023-03-10 09:50:02.001277 codegrade-16.1.8/codegrade/models/rubric_description_type.py
--rw-r--r--   0        0        0     1599 2023-03-10 09:50:20.909311 codegrade-16.1.8/codegrade/models/rubric_enabled_for_teacher_on_submissions_page_setting.py
--rw-r--r--   0        0        0     1663 2023-03-10 09:50:20.941311 codegrade-16.1.8/codegrade/models/rubric_item.py
--rw-r--r--   0        0        0     2265 2023-03-10 09:50:20.977311 codegrade-16.1.8/codegrade/models/rubric_item_input_as_json.py
--rw-r--r--   0        0        0      235 2023-03-10 09:50:02.213278 codegrade-16.1.8/codegrade/models/rubric_lock_reason.py
--rw-r--r--   0        0        0     3803 2023-03-10 09:50:21.033311 codegrade-16.1.8/codegrade/models/rubric_row_base.py
--rw-r--r--   0        0        0     2844 2023-03-10 09:50:21.081311 codegrade-16.1.8/codegrade/models/rubric_row_base_input_as_json.py
--rw-r--r--   0        0        0     1993 2023-03-10 09:50:21.109311 codegrade-16.1.8/codegrade/models/rubric_row_base_input_base_as_json.py
--rw-r--r--   0        0        0     1386 2023-03-10 09:50:21.137311 codegrade-16.1.8/codegrade/models/rubrics_enabled_setting.py
--rw-r--r--   0        0        0      221 2023-03-10 09:50:02.429278 codegrade-16.1.8/codegrade/models/rule_type.py
--rw-r--r--   0        0        0     2113 2023-03-10 09:50:21.169311 codegrade-16.1.8/codegrade/models/run_program_as_json.py
--rw-r--r--   0        0        0     1156 2023-03-10 09:50:21.193311 codegrade-16.1.8/codegrade/models/run_program_data.py
--rw-r--r--   0        0        0     1590 2023-03-10 09:50:21.217311 codegrade-16.1.8/codegrade/models/run_program_extra.py
--rw-r--r--   0        0        0     2105 2023-03-10 09:50:21.253311 codegrade-16.1.8/codegrade/models/run_program_input_as_json.py
--rw-r--r--   0        0        0     2505 2023-03-10 09:50:21.289311 codegrade-16.1.8/codegrade/models/run_program_log.py
--rw-r--r--   0        0        0     2164 2023-03-10 09:50:21.321311 codegrade-16.1.8/codegrade/models/saml2_provider_json.py
--rw-r--r--   0        0        0     1929 2023-03-10 09:50:21.353311 codegrade-16.1.8/codegrade/models/saml_ui_info.py
--rw-r--r--   0        0        0     1430 2023-03-10 09:50:21.377311 codegrade-16.1.8/codegrade/models/send_registration_email_setting.py
--rw-r--r--   0        0        0     1477 2023-03-10 09:50:21.405311 codegrade-16.1.8/codegrade/models/server_time_correction_enabled_setting.py
--rw-r--r--   0        0        0     1477 2023-03-10 09:50:21.429311 codegrade-16.1.8/codegrade/models/server_time_diff_tolerance_setting.py
--rw-r--r--   0        0        0     1471 2023-03-10 09:50:21.457311 codegrade-16.1.8/codegrade/models/server_time_sync_interval_setting.py
--rw-r--r--   0        0        0     1433 2023-03-10 09:50:21.481311 codegrade-16.1.8/codegrade/models/setting_token_time_setting.py
--rw-r--r--   0        0        0     1265 2023-03-10 09:50:21.501311 codegrade-16.1.8/codegrade/models/setup_oauth_result.py
--rw-r--r--   0        0        0     1354 2023-03-10 09:50:21.525312 codegrade-16.1.8/codegrade/models/site_email_setting.py
--rw-r--r--   0        0        0    18379 2023-03-10 09:50:21.657312 codegrade-16.1.8/codegrade/models/site_setting_input.py
--rw-r--r--   0        0        0     1690 2023-03-10 09:50:21.949312 codegrade-16.1.8/codegrade/models/snippet.py
--rw-r--r--   0        0        0     1489 2023-03-10 09:50:21.977312 codegrade-16.1.8/codegrade/models/sso_username_decollision_enabled_setting.py
--rw-r--r--   0        0        0     1303 2023-03-10 09:50:21.997312 codegrade-16.1.8/codegrade/models/start_payment_course_price_close_tab_data.py
--rw-r--r--   0        0        0      825 2023-03-10 09:50:22.005312 codegrade-16.1.8/codegrade/models/start_payment_course_price_data.py
--rw-r--r--   0        0        0     2068 2023-03-10 09:50:22.037312 codegrade-16.1.8/codegrade/models/start_payment_course_price_redirect_data.py
--rw-r--r--   0        0        0     1803 2023-03-10 09:50:22.065312 codegrade-16.1.8/codegrade/models/started_transaction.py
--rw-r--r--   0        0        0     1430 2023-03-10 09:50:22.093312 codegrade-16.1.8/codegrade/models/student_payment_enabled_setting.py
--rw-r--r--   0        0        0     2376 2023-03-10 09:50:22.129312 codegrade-16.1.8/codegrade/models/submission_validator_input_data.py
--rw-r--r--   0        0        0      349 2023-03-10 09:50:02.369278 codegrade-16.1.8/codegrade/models/task_result_state.py
--rw-r--r--   0        0        0      247 2023-03-10 09:50:01.961277 codegrade-16.1.8/codegrade/models/tax_behavior.py
--rw-r--r--   0        0        0     4104 2023-03-10 09:50:22.189313 codegrade-16.1.8/codegrade/models/tenant.py
--rw-r--r--   0        0        0     1879 2023-03-10 09:50:22.217312 codegrade-16.1.8/codegrade/models/tenant_course_statistics.py
--rw-r--r--   0        0        0     1243 2023-03-10 09:50:22.241313 codegrade-16.1.8/codegrade/models/tenant_of_tenant_price.py
--rw-r--r--   0        0        0     1699 2023-03-10 09:50:22.269313 codegrade-16.1.8/codegrade/models/tenant_permissions.py
--rw-r--r--   0        0        0     2077 2023-03-10 09:50:22.301313 codegrade-16.1.8/codegrade/models/tenant_price.py
--rw-r--r--   0        0        0     2415 2023-03-10 09:50:22.337313 codegrade-16.1.8/codegrade/models/tenant_role_as_json_with_perms.py
--rw-r--r--   0        0        0     2944 2023-03-10 09:50:22.377313 codegrade-16.1.8/codegrade/models/tenant_statistics.py
--rw-r--r--   0        0        0     1535 2023-03-10 09:50:22.405313 codegrade-16.1.8/codegrade/models/test_submission_copying_on_import_enabled_setting.py
--rw-r--r--   0        0        0     1425 2023-03-10 09:50:22.429313 codegrade-16.1.8/codegrade/models/tour_configurations_setting.py
--rw-r--r--   0        0        0     1416 2023-03-10 09:50:22.453313 codegrade-16.1.8/codegrade/models/tour_polling_interval_setting.py
--rw-r--r--   0        0        0     2943 2023-03-10 09:50:22.497313 codegrade-16.1.8/codegrade/models/transaction.py
--rw-r--r--   0        0        0      299 2023-03-10 09:50:01.349276 codegrade-16.1.8/codegrade/models/transaction_state.py
--rw-r--r--   0        0        0     1036 2023-03-10 09:50:22.517313 codegrade-16.1.8/codegrade/models/types.py
--rw-r--r--   0        0        0     3418 2023-03-10 09:50:22.561313 codegrade-16.1.8/codegrade/models/update_peer_feedback_settings_assignment_data.py
--rw-r--r--   0        0        0     1752 2023-03-10 09:50:22.589313 codegrade-16.1.8/codegrade/models/update_set_auto_test_data.py
--rw-r--r--   0        0        0     3439 2023-03-10 09:50:22.633313 codegrade-16.1.8/codegrade/models/update_suite_auto_test_base_data.py
--rw-r--r--   0        0        0     4543 2023-03-10 09:50:22.693313 codegrade-16.1.8/codegrade/models/update_suite_auto_test_data.py
--rw-r--r--   0        0        0     2231 2023-03-10 09:50:22.725313 codegrade-16.1.8/codegrade/models/upgraded_lti_provider_exception.py
--rw-r--r--   0        0        0     1516 2023-03-10 09:50:22.753313 codegrade-16.1.8/codegrade/models/upload_submission_assignment_data.py
--rw-r--r--   0        0        0     2128 2023-03-10 09:50:22.785313 codegrade-16.1.8/codegrade/models/user.py
--rw-r--r--   0        0        0     1555 2023-03-10 09:50:22.813313 codegrade-16.1.8/codegrade/models/user_course.py
--rw-r--r--   0        0        0     2118 2023-03-10 09:50:22.845313 codegrade-16.1.8/codegrade/models/user_info_with_role.py
--rw-r--r--   0        0        0     1993 2023-03-10 09:50:22.877313 codegrade-16.1.8/codegrade/models/user_input.py
--rw-r--r--   0        0        0     2663 2023-03-10 09:50:22.917314 codegrade-16.1.8/codegrade/models/user_without_group.py
--rw-r--r--   0        0        0     2125 2023-03-10 09:50:22.949314 codegrade-16.1.8/codegrade/models/weak_password_exception.py
--rw-r--r--   0        0        0     1651 2023-03-10 09:50:22.977314 codegrade-16.1.8/codegrade/models/weak_password_feedback.py
--rw-r--r--   0        0        0     3456 2023-03-10 09:50:23.029314 codegrade-16.1.8/codegrade/models/webhook_base.py
--rw-r--r--   0        0        0     4476 2023-03-10 09:50:23.093314 codegrade-16.1.8/codegrade/models/work.py
--rw-r--r--   0        0        0      245 2023-03-10 09:50:02.129278 codegrade-16.1.8/codegrade/models/work_origin.py
--rw-r--r--   0        0        0     2898 2023-03-10 09:50:23.137314 codegrade-16.1.8/codegrade/models/work_rubric_item.py
--rw-r--r--   0        0        0     2757 2023-03-10 09:50:23.173314 codegrade-16.1.8/codegrade/models/work_rubric_result_as_json.py
--rw-r--r--   0        0        0     2155 2023-03-10 09:50:23.205314 codegrade-16.1.8/codegrade/models/work_rubric_result_points_as_json.py
--rw-r--r--   0        0        0     3932 2023-03-10 09:50:23.581315 codegrade-16.1.8/codegrade/parsers.py
--rw-r--r--   0        0        0        0 2023-03-10 09:50:00.285274 codegrade-16.1.8/codegrade/py.typed
--rw-r--r--   0        0        0     7278 2023-03-10 09:50:23.701315 codegrade-16.1.8/codegrade/utils.py
--rw-r--r--   0        0        0     1364 2023-03-10 09:50:00.309274 codegrade-16.1.8/pyproject.toml
--rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 codegrade-16.1.8/setup.py
--rw-r--r--   0        0        0     2971 1970-01-01 00:00:00.000000 codegrade-16.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2019 2023-03-13 14:14:10.451287 codegrade-16.1.9/README.md
+-rw-r--r--   0        0        0     5813 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_dt_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-13 14:18:58.875312 codegrade-16.1.9/cg_dt_utils/py.typed
+-rw-r--r--   0        0        0      260 2023-03-13 14:18:58.863311 codegrade-16.1.9/cg_maybe/__init__.py
+-rw-r--r--   0        0        0    13379 2023-03-13 14:18:58.863311 codegrade-16.1.9/cg_maybe/_just.py
+-rw-r--r--   0        0        0      342 2023-03-13 14:18:58.863311 codegrade-16.1.9/cg_maybe/_maybe.py
+-rw-r--r--   0        0        0     5400 2023-03-13 14:18:58.863311 codegrade-16.1.9/cg_maybe/_nothing.py
+-rw-r--r--   0        0        0      705 2023-03-13 14:18:58.863311 codegrade-16.1.9/cg_maybe/_type_helpers.py
+-rw-r--r--   0        0        0     2580 2023-03-13 14:18:58.863311 codegrade-16.1.9/cg_maybe/cg_maybe_plugin.py
+-rw-r--r--   0        0        0        0 2023-03-13 14:18:58.875312 codegrade-16.1.9/cg_maybe/py.typed
+-rw-r--r--   0        0        0     3929 2023-03-13 14:18:58.863311 codegrade-16.1.9/cg_maybe/utils.py
+-rw-r--r--   0        0        0      994 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/__init__.py
+-rw-r--r--   0        0        0      724 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_any_value.py
+-rw-r--r--   0        0        0    15429 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_base.py
+-rw-r--r--   0        0        0    12024 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_convert.py
+-rw-r--r--   0        0        0     2360 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_enum.py
+-rw-r--r--   0        0        0     1437 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_lazy.py
+-rw-r--r--   0        0        0     2565 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_list.py
+-rw-r--r--   0        0        0     1080 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_literal.py
+-rw-r--r--   0        0        0    22148 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_mapping.py
+-rw-r--r--   0        0        0     6789 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_multipart.py
+-rw-r--r--   0        0        0     1211 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_nullable.py
+-rw-r--r--   0        0        0     2094 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_parse_utils.py
+-rw-r--r--   0        0        0     1900 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_query.py
+-rw-r--r--   0        0        0    10772 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_rich_value.py
+-rw-r--r--   0        0        0     1402 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_swagger_utils.py
+-rw-r--r--   0        0        0     3960 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_swaggerize.py
+-rw-r--r--   0        0        0     1519 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/_utils.py
+-rw-r--r--   0        0        0     4340 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-13 14:18:58.875312 codegrade-16.1.9/cg_request_args/py.typed
+-rw-r--r--   0        0        0    15309 2023-03-13 14:18:58.859311 codegrade-16.1.9/cg_request_args/request_args_plugin.py
+-rw-r--r--   0        0        0     2475 2023-03-13 14:14:15.967445 codegrade-16.1.9/codegrade/__init__.py
+-rw-r--r--   0        0        0      503 2023-03-13 14:14:14.187394 codegrade-16.1.9/codegrade/_api/__init__.py
+-rw-r--r--   0        0        0     2354 2023-03-13 14:14:16.023447 codegrade-16.1.9/codegrade/_api/about.py
+-rw-r--r--   0        0        0    59235 2023-03-13 14:14:17.095479 codegrade-16.1.9/codegrade/_api/assignment.py
+-rw-r--r--   0        0        0    42296 2023-03-13 14:14:16.771469 codegrade-16.1.9/codegrade/_api/auto_test.py
+-rw-r--r--   0        0        0    15003 2023-03-13 14:14:16.999476 codegrade-16.1.9/codegrade/_api/comment.py
+-rw-r--r--   0        0        0    65745 2023-03-13 14:14:18.427518 codegrade-16.1.9/codegrade/_api/course.py
+-rw-r--r--   0        0        0    11234 2023-03-13 14:14:17.267484 codegrade-16.1.9/codegrade/_api/course_price.py
+-rw-r--r--   0        0        0     2657 2023-03-13 14:14:17.399488 codegrade-16.1.9/codegrade/_api/file.py
+-rw-r--r--   0        0        0     7924 2023-03-13 14:14:17.527492 codegrade-16.1.9/codegrade/_api/git_provider.py
+-rw-r--r--   0        0        0     8551 2023-03-13 14:14:17.663496 codegrade-16.1.9/codegrade/_api/group.py
+-rw-r--r--   0        0        0     6844 2023-03-13 14:14:17.775499 codegrade-16.1.9/codegrade/_api/group_set.py
+-rw-r--r--   0        0        0     4134 2023-03-13 14:14:17.835501 codegrade-16.1.9/codegrade/_api/login_link.py
+-rw-r--r--   0        0        0    14594 2023-03-13 14:14:18.179511 codegrade-16.1.9/codegrade/_api/lti.py
+-rw-r--r--   0        0        0     6562 2023-03-13 14:14:18.271514 codegrade-16.1.9/codegrade/_api/notification.py
+-rw-r--r--   0        0        0     5104 2023-03-13 14:14:18.359516 codegrade-16.1.9/codegrade/_api/oauth_provider.py
+-rw-r--r--   0        0        0     6472 2023-03-13 14:14:18.607524 codegrade-16.1.9/codegrade/_api/oauth_token.py
+-rw-r--r--   0        0        0     3019 2023-03-13 14:14:18.471520 codegrade-16.1.9/codegrade/_api/permission.py
+-rw-r--r--   0        0        0     1909 2023-03-13 14:14:18.507521 codegrade-16.1.9/codegrade/_api/plagiarism.py
+-rw-r--r--   0        0        0     3566 2023-03-13 14:14:18.703527 codegrade-16.1.9/codegrade/_api/role.py
+-rw-r--r--   0        0        0    11091 2023-03-13 14:14:18.771529 codegrade-16.1.9/codegrade/_api/section.py
+-rw-r--r--   0        0        0     4110 2023-03-13 14:14:18.775529 codegrade-16.1.9/codegrade/_api/site_settings.py
+-rw-r--r--   0        0        0     6583 2023-03-13 14:14:18.879532 codegrade-16.1.9/codegrade/_api/snippet.py
+-rw-r--r--   0        0        0     2600 2023-03-13 14:14:18.815530 codegrade-16.1.9/codegrade/_api/sso_provider.py
+-rw-r--r--   0        0        0    20958 2023-03-13 14:14:19.151540 codegrade-16.1.9/codegrade/_api/submission.py
+-rw-r--r--   0        0        0     6862 2023-03-13 14:14:18.987535 codegrade-16.1.9/codegrade/_api/task_result.py
+-rw-r--r--   0        0        0    25894 2023-03-13 14:14:19.627554 codegrade-16.1.9/codegrade/_api/tenant.py
+-rw-r--r--   0        0        0     3455 2023-03-13 14:14:19.371547 codegrade-16.1.9/codegrade/_api/transaction.py
+-rw-r--r--   0        0        0    13833 2023-03-13 14:14:19.591553 codegrade-16.1.9/codegrade/_api/user.py
+-rw-r--r--   0        0        0     8745 2023-03-13 14:14:19.735557 codegrade-16.1.9/codegrade/_api/user_setting.py
+-rw-r--r--   0        0        0     1795 2023-03-13 14:14:19.659555 codegrade-16.1.9/codegrade/_api/webhook.py
+-rw-r--r--   0        0        0    23616 2023-03-13 14:14:20.239573 codegrade-16.1.9/codegrade/client.py
+-rw-r--r--   0        0        0      597 2023-03-13 14:14:19.747558 codegrade-16.1.9/codegrade/errors.py
+-rw-r--r--   0        0        0    29037 2023-03-13 14:14:20.215572 codegrade-16.1.9/codegrade/models/__init__.py
+-rw-r--r--   0        0        0     2635 2023-03-13 14:14:20.267573 codegrade-16.1.9/codegrade/models/_base_price.py
+-rw-r--r--   0        0        0     1715 2023-03-13 14:14:20.275574 codegrade-16.1.9/codegrade/models/_saml_ui_logo_info.py
+-rw-r--r--   0        0        0     2285 2023-03-13 14:14:20.315575 codegrade-16.1.9/codegrade/models/_submission_rubric_item_data_parser.py
+-rw-r--r--   0        0        0     2670 2023-03-13 14:14:20.331575 codegrade-16.1.9/codegrade/models/about.py
+-rw-r--r--   0        0        0     1390 2023-03-13 14:14:20.351576 codegrade-16.1.9/codegrade/models/abstract_role.py
+-rw-r--r--   0        0        0     1298 2023-03-13 14:14:20.359576 codegrade-16.1.9/codegrade/models/add_users_section_data.py
+-rw-r--r--   0        0        0     1914 2023-03-13 14:14:20.391577 codegrade-16.1.9/codegrade/models/all_auto_test_results.py
+-rw-r--r--   0        0        0    36010 2023-03-13 14:14:21.475609 codegrade-16.1.9/codegrade/models/all_site_settings.py
+-rw-r--r--   0        0        0     2202 2023-03-13 14:14:20.443579 codegrade-16.1.9/codegrade/models/any_auto_test_step_as_json.py
+-rw-r--r--   0        0        0     2887 2023-03-13 14:14:20.479580 codegrade-16.1.9/codegrade/models/any_error.py
+-rw-r--r--   0        0        0     2083 2023-03-13 14:14:20.523581 codegrade-16.1.9/codegrade/models/any_non_redacted_auto_test_step_as_json.py
+-rw-r--r--   0        0        0     2914 2023-03-13 14:14:20.579583 codegrade-16.1.9/codegrade/models/any_redacted_auto_test_step_as_json.py
+-rw-r--r--   0        0        0     2617 2023-03-13 14:14:12.695351 codegrade-16.1.9/codegrade/models/api_codes.py
+-rw-r--r--   0        0        0    23212 2023-03-13 14:14:21.887621 codegrade-16.1.9/codegrade/models/assignment.py
+-rw-r--r--   0        0        0      225 2023-03-13 14:14:13.359370 codegrade-16.1.9/codegrade/models/assignment_anonymization_algo.py
+-rw-r--r--   0        0        0     1597 2023-03-13 14:14:21.511610 codegrade-16.1.9/codegrade/models/assignment_default_grading_scale_points_setting.py
+-rw-r--r--   0        0        0     1536 2023-03-13 14:14:21.547611 codegrade-16.1.9/codegrade/models/assignment_default_grading_scale_setting.py
+-rw-r--r--   0        0        0     1481 2023-03-13 14:14:21.579612 codegrade-16.1.9/codegrade/models/assignment_description_enabled_setting.py
+-rw-r--r--   0        0        0      247 2023-03-13 14:14:11.327312 codegrade-16.1.9/codegrade/models/assignment_done_type.py
+-rw-r--r--   0        0        0      405 2023-03-13 14:14:13.551376 codegrade-16.1.9/codegrade/models/assignment_export_column.py
+-rw-r--r--   0        0        0     1990 2023-03-13 14:14:21.627614 codegrade-16.1.9/codegrade/models/assignment_feedback.py
+-rw-r--r--   0        0        0     2426 2023-03-13 14:14:21.679615 codegrade-16.1.9/codegrade/models/assignment_grader.py
+-rw-r--r--   0        0        0     1527 2023-03-13 14:14:21.719617 codegrade-16.1.9/codegrade/models/assignment_grading_scale_points_enabled_setting.py
+-rw-r--r--   0        0        0      211 2023-03-13 14:14:12.507346 codegrade-16.1.9/codegrade/models/assignment_kind.py
+-rw-r--r--   0        0        0     2326 2023-03-13 14:14:21.771618 codegrade-16.1.9/codegrade/models/assignment_login_link.py
+-rw-r--r--   0        0        0     1462 2023-03-13 14:14:21.807619 codegrade-16.1.9/codegrade/models/assignment_max_points_enabled_setting.py
+-rw-r--r--   0        0        0     1658 2023-03-13 14:14:21.843620 codegrade-16.1.9/codegrade/models/assignment_peer_feedback_connection.py
+-rw-r--r--   0        0        0     3342 2023-03-13 14:14:21.907622 codegrade-16.1.9/codegrade/models/assignment_peer_feedback_settings.py
+-rw-r--r--   0        0        0     1479 2023-03-13 14:14:21.919623 codegrade-16.1.9/codegrade/models/assignment_percentage_decimals_setting.py
+-rw-r--r--   0        0        0     1535 2023-03-13 14:14:21.939623 codegrade-16.1.9/codegrade/models/assignment_percentage_grading_settings.py
+-rw-r--r--   0        0        0     1440 2023-03-13 14:14:21.959624 codegrade-16.1.9/codegrade/models/assignment_point_decimals_setting.py
+-rw-r--r--   0        0        0     1985 2023-03-13 14:14:21.979624 codegrade-16.1.9/codegrade/models/assignment_points_grading_settings.py
+-rw-r--r--   0        0        0      239 2023-03-13 14:14:13.167365 codegrade-16.1.9/codegrade/models/assignment_state_enum.py
+-rw-r--r--   0        0        0     1661 2023-03-13 14:14:21.999625 codegrade-16.1.9/codegrade/models/assignment_template.py
+-rw-r--r--   0        0        0     1432 2023-03-13 14:14:22.011625 codegrade-16.1.9/codegrade/models/at_image_caching_enabled_setting.py
+-rw-r--r--   0        0        0     8263 2023-03-13 14:14:22.163630 codegrade-16.1.9/codegrade/models/auto_test.py
+-rw-r--r--   0        0        0     1483 2023-03-13 14:14:22.299634 codegrade-16.1.9/codegrade/models/auto_test_capture_points_message_setting.py
+-rw-r--r--   0        0        0     1454 2023-03-13 14:14:22.203631 codegrade-16.1.9/codegrade/models/auto_test_checkpoint_message_setting.py
+-rw-r--r--   0        0        0     1462 2023-03-13 14:14:22.247632 codegrade-16.1.9/codegrade/models/auto_test_code_quality_message_setting.py
+-rw-r--r--   0        0        0     1394 2023-03-13 14:14:22.279633 codegrade-16.1.9/codegrade/models/auto_test_enabled_setting.py
+-rw-r--r--   0        0        0     1743 2023-03-13 14:14:22.327635 codegrade-16.1.9/codegrade/models/auto_test_fixture.py
+-rw-r--r--   0        0        0     3532 2023-03-13 14:14:22.379636 codegrade-16.1.9/codegrade/models/auto_test_global_setup_output.py
+-rw-r--r--   0        0        0     1765 2023-03-13 14:14:22.363636 codegrade-16.1.9/codegrade/models/auto_test_global_setup_script.py
+-rw-r--r--   0        0        0     1489 2023-03-13 14:14:22.403637 codegrade-16.1.9/codegrade/models/auto_test_heartbeat_interval_setting.py
+-rw-r--r--   0        0        0     1462 2023-03-13 14:14:22.415637 codegrade-16.1.9/codegrade/models/auto_test_heartbeat_max_missed_setting.py
+-rw-r--r--   0        0        0     1432 2023-03-13 14:14:22.439638 codegrade-16.1.9/codegrade/models/auto_test_io_test_message_setting.py
+-rw-r--r--   0        0        0     1452 2023-03-13 14:14:22.447638 codegrade-16.1.9/codegrade/models/auto_test_io_test_sub_message_setting.py
+-rw-r--r--   0        0        0     1497 2023-03-13 14:14:22.475639 codegrade-16.1.9/codegrade/models/auto_test_max_concurrent_batch_runs_setting.py
+-rw-r--r--   0        0        0     1499 2023-03-13 14:14:22.483639 codegrade-16.1.9/codegrade/models/auto_test_max_global_setup_time_setting.py
+-rw-r--r--   0        0        0     1452 2023-03-13 14:14:22.511640 codegrade-16.1.9/codegrade/models/auto_test_max_jobs_per_runner_setting.py
+-rw-r--r--   0        0        0     1534 2023-03-13 14:14:22.519640 codegrade-16.1.9/codegrade/models/auto_test_max_per_student_setup_time_setting.py
+-rw-r--r--   0        0        0     1514 2023-03-13 14:14:22.547641 codegrade-16.1.9/codegrade/models/auto_test_max_result_not_started_setting.py
+-rw-r--r--   0        0        0     1473 2023-03-13 14:14:22.551641 codegrade-16.1.9/codegrade/models/auto_test_max_time_command_setting.py
+-rw-r--r--   0        0        0     1679 2023-03-13 14:14:22.583642 codegrade-16.1.9/codegrade/models/auto_test_max_unit_test_metadata_length_setting.py
+-rw-r--r--   0        0        0     3144 2023-03-13 14:14:22.627644 codegrade-16.1.9/codegrade/models/auto_test_quality_comment.py
+-rw-r--r--   0        0        0     3711 2023-03-13 14:14:22.659644 codegrade-16.1.9/codegrade/models/auto_test_result.py
+-rw-r--r--   0        0        0      399 2023-03-13 14:14:11.943330 codegrade-16.1.9/codegrade/models/auto_test_result_state.py
+-rw-r--r--   0        0        0     2591 2023-03-13 14:14:22.679645 codegrade-16.1.9/codegrade/models/auto_test_result_with_extra_data.py
+-rw-r--r--   0        0        0     2387 2023-03-13 14:14:22.707646 codegrade-16.1.9/codegrade/models/auto_test_run.py
+-rw-r--r--   0        0        0     1456 2023-03-13 14:14:22.715646 codegrade-16.1.9/codegrade/models/auto_test_run_program_message_setting.py
+-rw-r--r--   0        0        0     1267 2023-03-13 14:14:22.735647 codegrade-16.1.9/codegrade/models/auto_test_runner.py
+-rw-r--r--   0        0        0      417 2023-03-13 14:14:13.543376 codegrade-16.1.9/codegrade/models/auto_test_runner_state.py
+-rw-r--r--   0        0        0     2424 2023-03-13 14:14:22.771648 codegrade-16.1.9/codegrade/models/auto_test_set.py
+-rw-r--r--   0        0        0     1390 2023-03-13 14:14:22.759647 codegrade-16.1.9/codegrade/models/auto_test_step_base.py
+-rw-r--r--   0        0        0     2055 2023-03-13 14:14:22.803649 codegrade-16.1.9/codegrade/models/auto_test_step_base_as_json.py
+-rw-r--r--   0        0        0     2922 2023-03-13 14:14:22.839650 codegrade-16.1.9/codegrade/models/auto_test_step_base_input_as_json.py
+-rw-r--r--   0        0        0      964 2023-03-13 14:14:22.823650 codegrade-16.1.9/codegrade/models/auto_test_step_log_base.py
+-rw-r--r--   0        0        0     4809 2023-03-13 14:14:22.915652 codegrade-16.1.9/codegrade/models/auto_test_step_result.py
+-rw-r--r--   0        0        0      341 2023-03-13 14:14:12.535347 codegrade-16.1.9/codegrade/models/auto_test_step_result_state.py
+-rw-r--r--   0        0        0     2005 2023-03-13 14:14:22.883651 codegrade-16.1.9/codegrade/models/auto_test_step_validation_exception.py
+-rw-r--r--   0        0        0     3556 2023-03-13 14:14:22.951653 codegrade-16.1.9/codegrade/models/auto_test_suite.py
+-rw-r--r--   0        0        0     1444 2023-03-13 14:14:22.947653 codegrade-16.1.9/codegrade/models/auto_test_unit_test_message_setting.py
+-rw-r--r--   0        0        0     1503 2023-03-13 14:14:23.267663 codegrade-16.1.9/codegrade/models/automatic_lti1p3_assignment_import_setting.py
+-rw-r--r--   0        0        0     1444 2023-03-13 14:14:22.987654 codegrade-16.1.9/codegrade/models/automatic_lti_role_enabled_setting.py
+-rw-r--r--   0        0        0     3714 2023-03-13 14:14:23.063657 codegrade-16.1.9/codegrade/models/base_about.py
+-rw-r--r--   0        0        0     3205 2023-03-13 14:14:23.123658 codegrade-16.1.9/codegrade/models/base_auto_test_quality_comment.py
+-rw-r--r--   0        0        0     1690 2023-03-13 14:14:23.163659 codegrade-16.1.9/codegrade/models/base_comment_base.py
+-rw-r--r--   0        0        0     2274 2023-03-13 14:14:23.207661 codegrade-16.1.9/codegrade/models/base_comment_base_with_extended_replies.py
+-rw-r--r--   0        0        0     1857 2023-03-13 14:14:23.247662 codegrade-16.1.9/codegrade/models/base_comment_base_with_normal_replies.py
+-rw-r--r--   0        0        0     4564 2023-03-13 14:14:23.335665 codegrade-16.1.9/codegrade/models/base_comment_reply.py
+-rw-r--r--   0        0        0     2861 2023-03-13 14:14:23.323664 codegrade-16.1.9/codegrade/models/base_coupon.py
+-rw-r--r--   0        0        0     2032 2023-03-13 14:14:23.367666 codegrade-16.1.9/codegrade/models/base_directory.py
+-rw-r--r--   0        0        0     2752 2023-03-13 14:14:23.391666 codegrade-16.1.9/codegrade/models/base_error.py
+-rw-r--r--   0        0        0     2831 2023-03-13 14:14:23.427667 codegrade-16.1.9/codegrade/models/base_file.py
+-rw-r--r--   0        0        0    11095 2023-03-13 14:14:23.787678 codegrade-16.1.9/codegrade/models/base_lms_capabilities.py
+-rw-r--r--   0        0        0     3246 2023-03-13 14:14:23.483669 codegrade-16.1.9/codegrade/models/base_lti1p1_provider.py
+-rw-r--r--   0        0        0     3712 2023-03-13 14:14:23.551671 codegrade-16.1.9/codegrade/models/base_lti1p3_provider.py
+-rw-r--r--   0        0        0     2648 2023-03-13 14:14:23.603673 codegrade-16.1.9/codegrade/models/base_lti_provider.py
+-rw-r--r--   0        0        0     5105 2023-03-13 14:14:23.703676 codegrade-16.1.9/codegrade/models/base_notification.py
+-rw-r--r--   0        0        0     1231 2023-03-13 14:14:23.731676 codegrade-16.1.9/codegrade/models/base_release_info.py
+-rw-r--r--   0        0        0     1923 2023-03-13 14:14:23.775678 codegrade-16.1.9/codegrade/models/base_rubric_item.py
+-rw-r--r--   0        0        0     1462 2023-03-13 14:14:23.815679 codegrade-16.1.9/codegrade/models/blackboard_zip_upload_enabled_setting.py
+-rw-r--r--   0        0        0     1372 2023-03-13 14:14:23.819679 codegrade-16.1.9/codegrade/models/bulk_enroll_course_data.py
+-rw-r--r--   0        0        0     1485 2023-03-13 14:14:23.855680 codegrade-16.1.9/codegrade/models/canvas_course_id_copying_enabled_setting.py
+-rw-r--r--   0        0        0      321 2023-03-13 14:14:12.391342 codegrade-16.1.9/codegrade/models/cg_ignore_version.py
+-rw-r--r--   0        0        0     4080 2023-03-13 14:14:23.907682 codegrade-16.1.9/codegrade/models/change_user_role_course_data.py
+-rw-r--r--   0        0        0     2098 2023-03-13 14:14:23.899681 codegrade-16.1.9/codegrade/models/check_points_as_json.py
+-rw-r--r--   0        0        0     1257 2023-03-13 14:14:23.927682 codegrade-16.1.9/codegrade/models/check_points_data.py
+-rw-r--r--   0        0        0     1603 2023-03-13 14:14:23.943683 codegrade-16.1.9/codegrade/models/check_points_extra.py
+-rw-r--r--   0        0        0     2115 2023-03-13 14:14:23.971683 codegrade-16.1.9/codegrade/models/check_points_input_as_json.py
+-rw-r--r--   0        0        0     1211 2023-03-13 14:14:23.971683 codegrade-16.1.9/codegrade/models/clone_result.py
+-rw-r--r--   0        0        0     2098 2023-03-13 14:14:24.019685 codegrade-16.1.9/codegrade/models/code_quality_as_json.py
+-rw-r--r--   0        0        0     2908 2023-03-13 14:14:24.031685 codegrade-16.1.9/codegrade/models/code_quality_base_data.py
+-rw-r--r--   0        0        0     2624 2023-03-13 14:14:24.079686 codegrade-16.1.9/codegrade/models/code_quality_data.py
+-rw-r--r--   0        0        0     1603 2023-03-13 14:14:24.071686 codegrade-16.1.9/codegrade/models/code_quality_extra.py
+-rw-r--r--   0        0        0     2115 2023-03-13 14:14:24.119688 codegrade-16.1.9/codegrade/models/code_quality_input_as_json.py
+-rw-r--r--   0        0        0     2106 2023-03-13 14:14:24.123688 codegrade-16.1.9/codegrade/models/code_quality_penalties.py
+-rw-r--r--   0        0        0     1760 2023-03-13 14:14:24.163689 codegrade-16.1.9/codegrade/models/column_range.py
+-rw-r--r--   0        0        0      678 2023-03-13 14:14:24.135688 codegrade-16.1.9/codegrade/models/comment_base.py
+-rw-r--r--   0        0        0      640 2023-03-13 14:14:24.147688 codegrade-16.1.9/codegrade/models/comment_reply.py
+-rw-r--r--   0        0        0     2730 2023-03-13 14:14:24.203690 codegrade-16.1.9/codegrade/models/comment_reply_edit.py
+-rw-r--r--   0        0        0      231 2023-03-13 14:14:12.855356 codegrade-16.1.9/codegrade/models/comment_reply_type.py
+-rw-r--r--   0        0        0      223 2023-03-13 14:14:13.511375 codegrade-16.1.9/codegrade/models/comment_type.py
+-rw-r--r--   0        0        0     1449 2023-03-13 14:14:24.199690 codegrade-16.1.9/codegrade/models/connect_repository_git_provider_data.py
+-rw-r--r--   0        0        0     1386 2023-03-13 14:14:24.231691 codegrade-16.1.9/codegrade/models/copy_auto_test_data.py
+-rw-r--r--   0        0        0     1444 2023-03-13 14:14:24.235691 codegrade-16.1.9/codegrade/models/copy_rubric_assignment_data.py
+-rw-r--r--   0        0        0      572 2023-03-13 14:14:24.247691 codegrade-16.1.9/codegrade/models/coupon.py
+-rw-r--r--   0        0        0     1676 2023-03-13 14:14:24.503699 codegrade-16.1.9/codegrade/models/coupon_data_parser.py
+-rw-r--r--   0        0        0     2112 2023-03-13 14:14:24.291693 codegrade-16.1.9/codegrade/models/coupon_usage.py
+-rw-r--r--   0        0        0     2257 2023-03-13 14:14:24.343694 codegrade-16.1.9/codegrade/models/coupon_with_code.py
+-rw-r--r--   0        0        0     1994 2023-03-13 14:14:24.387696 codegrade-16.1.9/codegrade/models/coupon_without_code.py
+-rw-r--r--   0        0        0     4395 2023-03-13 14:14:24.471698 codegrade-16.1.9/codegrade/models/course.py
+-rw-r--r--   0        0        0     2016 2023-03-13 14:14:24.515699 codegrade-16.1.9/codegrade/models/course_bulk_enroll_result.py
+-rw-r--r--   0        0        0     1456 2023-03-13 14:14:24.539700 codegrade-16.1.9/codegrade/models/course_bulk_register_enabled_setting.py
+-rw-r--r--   0        0        0     1436 2023-03-13 14:14:24.551700 codegrade-16.1.9/codegrade/models/course_gradebook_enabled_setting.py
+-rw-r--r--   0        0        0     1507 2023-03-13 14:14:24.571701 codegrade-16.1.9/codegrade/models/course_gradebook_render_warning_size_setting.py
+-rw-r--r--   0        0        0     2046 2023-03-13 14:14:24.595702 codegrade-16.1.9/codegrade/models/course_of_course_price.py
+-rw-r--r--   0        0        0    56861 2023-03-13 14:14:30.539875 codegrade-16.1.9/codegrade/models/course_perm_map.py
+-rw-r--r--   0        0        0     5291 2023-03-13 14:14:24.671704 codegrade-16.1.9/codegrade/models/course_permission.py
+-rw-r--r--   0        0        0     2415 2023-03-13 14:14:24.727705 codegrade-16.1.9/codegrade/models/course_price.py
+-rw-r--r--   0        0        0     1430 2023-03-13 14:14:24.763707 codegrade-16.1.9/codegrade/models/course_register_enabled_setting.py
+-rw-r--r--   0        0        0     1374 2023-03-13 14:14:24.791707 codegrade-16.1.9/codegrade/models/course_register_response.py
+-rw-r--r--   0        0        0     2611 2023-03-13 14:14:24.843709 codegrade-16.1.9/codegrade/models/course_registration_link.py
+-rw-r--r--   0        0        0     1938 2023-03-13 14:14:24.887710 codegrade-16.1.9/codegrade/models/course_role.py
+-rw-r--r--   0        0        0     2743 2023-03-13 14:14:24.943712 codegrade-16.1.9/codegrade/models/course_role_as_json_with_perms.py
+-rw-r--r--   0        0        0     2156 2023-03-13 14:14:24.995713 codegrade-16.1.9/codegrade/models/course_section.py
+-rw-r--r--   0        0        0     1756 2023-03-13 14:14:25.031714 codegrade-16.1.9/codegrade/models/course_section_division.py
+-rw-r--r--   0        0        0     1862 2023-03-13 14:14:25.075716 codegrade-16.1.9/codegrade/models/course_section_division_connection.py
+-rw-r--r--   0        0        0     1530 2023-03-13 14:14:25.107716 codegrade-16.1.9/codegrade/models/course_section_division_user.py
+-rw-r--r--   0        0        0     1847 2023-03-13 14:14:25.159718 codegrade-16.1.9/codegrade/models/course_snippet.py
+-rw-r--r--   0        0        0      239 2023-03-13 14:14:11.983331 codegrade-16.1.9/codegrade/models/course_state.py
+-rw-r--r--   0        0        0     1632 2023-03-13 14:14:25.195719 codegrade-16.1.9/codegrade/models/course_statistics_as_json.py
+-rw-r--r--   0        0        0     1247 2023-03-13 14:14:25.235720 codegrade-16.1.9/codegrade/models/create_assignment_course_data.py
+-rw-r--r--   0        0        0     1827 2023-03-13 14:14:25.283722 codegrade-16.1.9/codegrade/models/create_auto_test_data.py
+-rw-r--r--   0        0        0     2744 2023-03-13 14:14:25.347724 codegrade-16.1.9/codegrade/models/create_comment_data.py
+-rw-r--r--   0        0        0     2299 2023-03-13 14:14:25.399725 codegrade-16.1.9/codegrade/models/create_comment_reply_data.py
+-rw-r--r--   0        0        0     2018 2023-03-13 14:14:25.447726 codegrade-16.1.9/codegrade/models/create_course_data.py
+-rw-r--r--   0        0        0     1431 2023-03-13 14:14:25.763736 codegrade-16.1.9/codegrade/models/create_division_section_data.py
+-rw-r--r--   0        0        0     2296 2023-03-13 14:14:25.815737 codegrade-16.1.9/codegrade/models/create_group_group_set_data.py
+-rw-r--r--   0        0        0     2365 2023-03-13 14:14:25.867739 codegrade-16.1.9/codegrade/models/create_group_set_course_data.py
+-rw-r--r--   0        0        0      613 2023-03-13 14:14:25.879739 codegrade-16.1.9/codegrade/models/create_lti_data.py
+-rw-r--r--   0        0        0     1740 2023-03-13 14:14:25.915740 codegrade-16.1.9/codegrade/models/create_output_html_proxy_auto_test_data.py
+-rw-r--r--   0        0        0     2074 2023-03-13 14:14:25.955741 codegrade-16.1.9/codegrade/models/create_proxy_submission_data.py
+-rw-r--r--   0        0        0     1732 2023-03-13 14:14:25.999743 codegrade-16.1.9/codegrade/models/create_repository_git_provider_data.py
+-rw-r--r--   0        0        0     1219 2023-03-13 14:14:26.027743 codegrade-16.1.9/codegrade/models/create_role_course_data.py
+-rw-r--r--   0        0        0     1681 2023-03-13 14:14:26.067745 codegrade-16.1.9/codegrade/models/create_section_course_data.py
+-rw-r--r--   0        0        0     1506 2023-03-13 14:14:26.099745 codegrade-16.1.9/codegrade/models/create_snippet_course_data.py
+-rw-r--r--   0        0        0     1504 2023-03-13 14:14:26.135747 codegrade-16.1.9/codegrade/models/create_snippet_data.py
+-rw-r--r--   0        0        0     2066 2023-03-13 14:14:26.175748 codegrade-16.1.9/codegrade/models/create_sso_provider_data.py
+-rw-r--r--   0        0        0     2223 2023-03-13 14:14:26.227749 codegrade-16.1.9/codegrade/models/create_tenant_data.py
+-rw-r--r--   0        0        0     1568 2023-03-13 14:14:26.263750 codegrade-16.1.9/codegrade/models/csv_large_file_limit_setting.py
+-rw-r--r--   0        0        0     1432 2023-03-13 14:14:26.295751 codegrade-16.1.9/codegrade/models/csv_too_many_errors_limit_setting.py
+-rw-r--r--   0        0        0      207 2023-03-13 14:14:13.423372 codegrade-16.1.9/codegrade/models/currency.py
+-rw-r--r--   0        0        0     2135 2023-03-13 14:14:26.339753 codegrade-16.1.9/codegrade/models/custom_output_as_json.py
+-rw-r--r--   0        0        0     1554 2023-03-13 14:14:26.375753 codegrade-16.1.9/codegrade/models/custom_output_data.py
+-rw-r--r--   0        0        0     1616 2023-03-13 14:14:26.415755 codegrade-16.1.9/codegrade/models/custom_output_extra.py
+-rw-r--r--   0        0        0     2125 2023-03-13 14:14:26.467756 codegrade-16.1.9/codegrade/models/custom_output_input_as_json.py
+-rw-r--r--   0        0        0     2838 2023-03-13 14:14:26.531758 codegrade-16.1.9/codegrade/models/custom_output_log.py
+-rw-r--r--   0        0        0     2536 2023-03-13 14:14:26.583760 codegrade-16.1.9/codegrade/models/custom_output_log_base.py
+-rw-r--r--   0        0        0     2361 2023-03-13 14:14:26.631761 codegrade-16.1.9/codegrade/models/deleted_comment_reply.py
+-rw-r--r--   0        0        0      283 2023-03-13 14:14:13.503374 codegrade-16.1.9/codegrade/models/deletion_type.py
+-rw-r--r--   0        0        0     2419 2023-03-13 14:14:26.683762 codegrade-16.1.9/codegrade/models/directory_with_children.py
+-rw-r--r--   0        0        0     2493 2023-03-13 14:14:26.735764 codegrade-16.1.9/codegrade/models/disabled_setting_exception.py
+-rw-r--r--   0        0        0     1450 2023-03-13 14:14:26.775765 codegrade-16.1.9/codegrade/models/editor_enabled_for_teachers_setting.py
+-rw-r--r--   0        0        0     1380 2023-03-13 14:14:26.815766 codegrade-16.1.9/codegrade/models/editor_enabled_setting.py
+-rw-r--r--   0        0        0      267 2023-03-13 14:14:13.263368 codegrade-16.1.9/codegrade/models/email_notification_types.py
+-rw-r--r--   0        0        0     1424 2023-03-13 14:14:26.855768 codegrade-16.1.9/codegrade/models/email_students_enabled_setting.py
+-rw-r--r--   0        0        0     5504 2023-03-13 14:14:26.963771 codegrade-16.1.9/codegrade/models/email_users_course_data.py
+-rw-r--r--   0        0        0     1447 2023-03-13 14:14:26.999772 codegrade-16.1.9/codegrade/models/exam_login_max_length_setting.py
+-rw-r--r--   0        0        0     2235 2023-03-13 14:14:27.047773 codegrade-16.1.9/codegrade/models/export_assignment_csv_data.py
+-rw-r--r--   0        0        0      693 2023-03-13 14:14:27.063773 codegrade-16.1.9/codegrade/models/export_assignment_data.py
+-rw-r--r--   0        0        0     1685 2023-03-13 14:14:27.103775 codegrade-16.1.9/codegrade/models/export_assignment_files_data.py
+-rw-r--r--   0        0        0    10220 2023-03-13 14:14:27.587789 codegrade-16.1.9/codegrade/models/extended_auto_test_result.py
+-rw-r--r--   0        0        0     3231 2023-03-13 14:14:27.655791 codegrade-16.1.9/codegrade/models/extended_auto_test_run.py
+-rw-r--r--   0        0        0     3342 2023-03-13 14:14:27.723793 codegrade-16.1.9/codegrade/models/extended_course.py
+-rw-r--r--   0        0        0     2126 2023-03-13 14:14:27.767794 codegrade-16.1.9/codegrade/models/extended_course_registration_link.py
+-rw-r--r--   0        0        0     1930 2023-03-13 14:14:27.815796 codegrade-16.1.9/codegrade/models/extended_course_section.py
+-rw-r--r--   0        0        0     2258 2023-03-13 14:14:27.863797 codegrade-16.1.9/codegrade/models/extended_group.py
+-rw-r--r--   0        0        0     3144 2023-03-13 14:14:27.931799 codegrade-16.1.9/codegrade/models/extended_job.py
+-rw-r--r--   0        0        0     3042 2023-03-13 14:14:27.991801 codegrade-16.1.9/codegrade/models/extended_non_deleted_comment_reply.py
+-rw-r--r--   0        0        0     4255 2023-03-13 14:14:28.079803 codegrade-16.1.9/codegrade/models/extended_tenant.py
+-rw-r--r--   0        0        0     2456 2023-03-13 14:14:28.135805 codegrade-16.1.9/codegrade/models/extended_transaction.py
+-rw-r--r--   0        0        0     4999 2023-03-13 14:14:28.235808 codegrade-16.1.9/codegrade/models/extended_user.py
+-rw-r--r--   0        0        0     3868 2023-03-13 14:14:28.315810 codegrade-16.1.9/codegrade/models/extended_work.py
+-rw-r--r--   0        0        0     1901 2023-03-13 14:14:28.355811 codegrade-16.1.9/codegrade/models/extract_file_tree_directory.py
+-rw-r--r--   0        0        0     1168 2023-03-13 14:14:28.387812 codegrade-16.1.9/codegrade/models/extract_file_tree_file.py
+-rw-r--r--   0        0        0     2477 2023-03-13 14:14:28.439814 codegrade-16.1.9/codegrade/models/failed_to_send_email_exception.py
+-rw-r--r--   0        0        0     2628 2023-03-13 14:14:28.487815 codegrade-16.1.9/codegrade/models/feedback_base.py
+-rw-r--r--   0        0        0     1511 2023-03-13 14:14:28.531816 codegrade-16.1.9/codegrade/models/feedback_threads_initially_collapsed_setting.py
+-rw-r--r--   0        0        0     3676 2023-03-13 14:14:28.939828 codegrade-16.1.9/codegrade/models/feedback_with_replies.py
+-rw-r--r--   0        0        0     3630 2023-03-13 14:14:29.007830 codegrade-16.1.9/codegrade/models/feedback_without_replies.py
+-rw-r--r--   0        0        0     2485 2023-03-13 14:14:29.063832 codegrade-16.1.9/codegrade/models/file_deletion.py
+-rw-r--r--   0        0        0     1850 2023-03-13 14:14:29.107833 codegrade-16.1.9/codegrade/models/file_rule.py
+-rw-r--r--   0        0        0     2130 2023-03-13 14:14:29.151834 codegrade-16.1.9/codegrade/models/file_rule_input_data.py
+-rw-r--r--   0        0        0      569 2023-03-13 14:14:29.163835 codegrade-16.1.9/codegrade/models/file_tree.py
+-rw-r--r--   0        0        0      205 2023-03-13 14:14:13.075362 codegrade-16.1.9/codegrade/models/file_type.py
+-rw-r--r--   0        0        0     2462 2023-03-13 14:14:29.211836 codegrade-16.1.9/codegrade/models/finalized_lti1p1_provider.py
+-rw-r--r--   0        0        0     2594 2023-03-13 14:14:29.263838 codegrade-16.1.9/codegrade/models/finalized_lti1p3_provider.py
+-rw-r--r--   0        0        0     1416 2023-03-13 14:14:29.303839 codegrade-16.1.9/codegrade/models/find_element_interval_setting.py
+-rw-r--r--   0        0        0     1418 2023-03-13 14:14:29.347840 codegrade-16.1.9/codegrade/models/find_element_max_tries_setting.py
+-rw-r--r--   0        0        0     2233 2023-03-13 14:14:29.395841 codegrade-16.1.9/codegrade/models/first_phase_lti_launch_exception.py
+-rw-r--r--   0        0        0     1494 2023-03-13 14:14:29.431843 codegrade-16.1.9/codegrade/models/fixed_availability.py
+-rw-r--r--   0        0        0     1545 2023-03-13 14:14:29.471844 codegrade-16.1.9/codegrade/models/fixed_grade_availability.py
+-rw-r--r--   0        0        0     1139 2023-03-13 14:14:29.499845 codegrade-16.1.9/codegrade/models/fixture_like.py
+-rw-r--r--   0        0        0     1402 2023-03-13 14:14:29.535846 codegrade-16.1.9/codegrade/models/fraction.py
+-rw-r--r--   0        0        0    50981 2023-03-13 14:14:33.855971 codegrade-16.1.9/codegrade/models/frontend_site_settings.py
+-rw-r--r--   0        0        0     1784 2023-03-13 14:14:30.579876 codegrade-16.1.9/codegrade/models/general_feedback_comment_base.py
+-rw-r--r--   0        0        0     1994 2023-03-13 14:14:30.619877 codegrade-16.1.9/codegrade/models/general_feedback_comment_base_with_extended_replies.py
+-rw-r--r--   0        0        0     1212 2023-03-13 14:14:30.647878 codegrade-16.1.9/codegrade/models/general_feedback_extra.py
+-rw-r--r--   0        0        0     1848 2023-03-13 14:14:30.687879 codegrade-16.1.9/codegrade/models/git_repositories_page.py
+-rw-r--r--   0        0        0     1720 2023-03-13 14:14:30.727880 codegrade-16.1.9/codegrade/models/git_repository_like.py
+-rw-r--r--   0        0        0     1491 2023-03-13 14:14:30.771882 codegrade-16.1.9/codegrade/models/git_user_info.py
+-rw-r--r--   0        0        0    14535 2023-03-13 14:14:31.919915 codegrade-16.1.9/codegrade/models/global_perm_map.py
+-rw-r--r--   0        0        0     1477 2023-03-13 14:14:31.943916 codegrade-16.1.9/codegrade/models/global_permission.py
+-rw-r--r--   0        0        0     3176 2023-03-13 14:14:32.011918 codegrade-16.1.9/codegrade/models/grade_history.py
+-rw-r--r--   0        0        0      287 2023-03-13 14:14:13.431372 codegrade-16.1.9/codegrade/models/grade_origin.py
+-rw-r--r--   0        0        0     1475 2023-03-13 14:14:32.051919 codegrade-16.1.9/codegrade/models/grading_notifications_enabled_setting.py
+-rw-r--r--   0        0        0     2527 2023-03-13 14:14:32.111921 codegrade-16.1.9/codegrade/models/group.py
+-rw-r--r--   0        0        0     2470 2023-03-13 14:14:32.167922 codegrade-16.1.9/codegrade/models/group_not_ready_for_submission_exception.py
+-rw-r--r--   0        0        0     2354 2023-03-13 14:14:32.211923 codegrade-16.1.9/codegrade/models/group_set.py
+-rw-r--r--   0        0        0     1380 2023-03-13 14:14:32.247924 codegrade-16.1.9/codegrade/models/groups_enabled_setting.py
+-rw-r--r--   0        0        0     1290 2023-03-13 14:14:32.279925 codegrade-16.1.9/codegrade/models/has_unread_notifcation_json.py
+-rw-r--r--   0        0        0     3388 2023-03-13 14:14:32.347927 codegrade-16.1.9/codegrade/models/health_information.py
+-rw-r--r--   0        0        0      231 2023-03-13 14:14:11.243310 codegrade-16.1.9/codegrade/models/ignore_handling.py
+-rw-r--r--   0        0        0     5316 2023-03-13 14:14:32.439930 codegrade-16.1.9/codegrade/models/ignored_files_exception.py
+-rw-r--r--   0        0        0     1462 2023-03-13 14:14:32.471931 codegrade-16.1.9/codegrade/models/import_into_assignment_data.py
+-rw-r--r--   0        0        0     1317 2023-03-13 14:14:32.499932 codegrade-16.1.9/codegrade/models/import_into_course_data.py
+-rw-r--r--   0        0        0     1519 2023-03-13 14:14:32.539933 codegrade-16.1.9/codegrade/models/incremental_rubric_submission_enabled_setting.py
+-rw-r--r--   0        0        0     1927 2023-03-13 14:14:32.579934 codegrade-16.1.9/codegrade/models/inline_feedback_comment_base.py
+-rw-r--r--   0        0        0     2137 2023-03-13 14:14:32.623935 codegrade-16.1.9/codegrade/models/inline_feedback_comment_base_with_extended_replies.py
+-rw-r--r--   0        0        0     1863 2023-03-13 14:14:32.663936 codegrade-16.1.9/codegrade/models/inline_feedback_extra.py
+-rw-r--r--   0        0        0     2040 2023-03-13 14:14:32.711938 codegrade-16.1.9/codegrade/models/invalid_group_exception.py
+-rw-r--r--   0        0        0     3002 2023-03-13 14:14:32.767939 codegrade-16.1.9/codegrade/models/invalid_io_cases_exception.py
+-rw-r--r--   0        0        0     2052 2023-03-13 14:14:32.811941 codegrade-16.1.9/codegrade/models/invalid_options_exception.py
+-rw-r--r--   0        0        0     2048 2023-03-13 14:14:32.855942 codegrade-16.1.9/codegrade/models/io_test_as_json.py
+-rw-r--r--   0        0        0     1606 2023-03-13 14:14:32.895943 codegrade-16.1.9/codegrade/models/io_test_base_data.py
+-rw-r--r--   0        0        0     2008 2023-03-13 14:14:32.939944 codegrade-16.1.9/codegrade/models/io_test_data.py
+-rw-r--r--   0        0        0     1512 2023-03-13 14:14:32.991946 codegrade-16.1.9/codegrade/models/io_test_extra.py
+-rw-r--r--   0        0        0     2065 2023-03-13 14:14:33.035947 codegrade-16.1.9/codegrade/models/io_test_input_as_json.py
+-rw-r--r--   0        0        0     2770 2023-03-13 14:14:33.091949 codegrade-16.1.9/codegrade/models/io_test_input_case.py
+-rw-r--r--   0        0        0     1568 2023-03-13 14:14:33.127950 codegrade-16.1.9/codegrade/models/io_test_log.py
+-rw-r--r--   0        0        0      319 2023-03-13 14:14:13.411372 codegrade-16.1.9/codegrade/models/io_test_option.py
+-rw-r--r--   0        0        0     4604 2023-03-13 14:14:33.523961 codegrade-16.1.9/codegrade/models/io_test_step_log.py
+-rw-r--r--   0        0        0     1678 2023-03-13 14:14:33.559962 codegrade-16.1.9/codegrade/models/io_test_step_log_base.py
+-rw-r--r--   0        0        0     1450 2023-03-13 14:14:33.595963 codegrade-16.1.9/codegrade/models/is_admin_permission_enabled_setting.py
+-rw-r--r--   0        0        0     1889 2023-03-13 14:14:33.639965 codegrade-16.1.9/codegrade/models/job.py
+-rw-r--r--   0        0        0     7412 2023-03-13 14:14:33.783969 codegrade-16.1.9/codegrade/models/json_create_auto_test.py
+-rw-r--r--   0        0        0     1612 2023-03-13 14:14:33.819970 codegrade-16.1.9/codegrade/models/json_create_tenant.py
+-rw-r--r--   0        0        0     6846 2023-03-13 14:14:33.947974 codegrade-16.1.9/codegrade/models/json_patch_auto_test.py
+-rw-r--r--   0        0        0     3286 2023-03-13 14:14:33.919973 codegrade-16.1.9/codegrade/models/json_patch_submit_types_assignment.py
+-rw-r--r--   0        0        0     2078 2023-03-13 14:14:33.963974 codegrade-16.1.9/codegrade/models/junit_test_as_json.py
+-rw-r--r--   0        0        0     1177 2023-03-13 14:14:33.975974 codegrade-16.1.9/codegrade/models/junit_test_base_data.py
+-rw-r--r--   0        0        0     2965 2023-03-13 14:14:34.023976 codegrade-16.1.9/codegrade/models/junit_test_data.py
+-rw-r--r--   0        0        0     1577 2023-03-13 14:14:34.011975 codegrade-16.1.9/codegrade/models/junit_test_extra.py
+-rw-r--r--   0        0        0     2095 2023-03-13 14:14:34.059977 codegrade-16.1.9/codegrade/models/junit_test_input_as_json.py
+-rw-r--r--   0        0        0     2345 2023-03-13 14:14:34.075977 codegrade-16.1.9/codegrade/models/junit_test_log.py
+-rw-r--r--   0        0        0     2517 2023-03-13 14:14:34.107978 codegrade-16.1.9/codegrade/models/junit_test_log_base.py
+-rw-r--r--   0        0        0     1465 2023-03-13 14:14:34.107978 codegrade-16.1.9/codegrade/models/jwt_access_token_expires_setting.py
+-rw-r--r--   0        0        0     4695 2023-03-13 14:14:34.191980 codegrade-16.1.9/codegrade/models/legacy_features.py
+-rw-r--r--   0        0        0     1501 2023-03-13 14:14:34.143979 codegrade-16.1.9/codegrade/models/line_range.py
+-rw-r--r--   0        0        0     1902 2023-03-13 14:14:34.191980 codegrade-16.1.9/codegrade/models/linter_comment.py
+-rw-r--r--   0        0        0     1386 2023-03-13 14:14:34.227981 codegrade-16.1.9/codegrade/models/linters_enabled_setting.py
+-rw-r--r--   0        0        0     3208 2023-03-13 14:14:34.247982 codegrade-16.1.9/codegrade/models/lms_capabilities.py
+-rw-r--r--   0        0        0     1481 2023-03-13 14:14:34.267983 codegrade-16.1.9/codegrade/models/login_token_before_time_setting.py
+-rw-r--r--   0        0        0     4556 2023-03-13 14:14:34.359985 codegrade-16.1.9/codegrade/models/login_user_data.py
+-rw-r--r--   0        0        0      678 2023-03-13 14:14:34.279983 codegrade-16.1.9/codegrade/models/lti1p1_provider.py
+-rw-r--r--   0        0        0     2791 2023-03-13 14:14:34.335985 codegrade-16.1.9/codegrade/models/lti1p1_provider_data.py
+-rw-r--r--   0        0        0      678 2023-03-13 14:14:34.347985 codegrade-16.1.9/codegrade/models/lti1p3_provider.py
+-rw-r--r--   0        0        0     2820 2023-03-13 14:14:34.407987 codegrade-16.1.9/codegrade/models/lti1p3_provider_data.py
+-rw-r--r--   0        0        0     1558 2023-03-13 14:14:34.715996 codegrade-16.1.9/codegrade/models/lti1p3_provider_presentation_as_json.py
+-rw-r--r--   0        0        0     1362 2023-03-13 14:14:34.443988 codegrade-16.1.9/codegrade/models/lti_enabled_setting.py
+-rw-r--r--   0        0        0     1458 2023-03-13 14:14:34.479989 codegrade-16.1.9/codegrade/models/lti_lock_date_copying_enabled_setting.py
+-rw-r--r--   0        0        0      976 2023-03-13 14:14:34.499989 codegrade-16.1.9/codegrade/models/lti_provider_base.py
+-rw-r--r--   0        0        0     1592 2023-03-13 14:14:34.535990 codegrade-16.1.9/codegrade/models/max_document_update_size_setting.py
+-rw-r--r--   0        0        0     1568 2023-03-13 14:14:34.571992 codegrade-16.1.9/codegrade/models/max_dynamo_file_size_setting.py
+-rw-r--r--   0        0        0     1604 2023-03-13 14:14:34.611993 codegrade-16.1.9/codegrade/models/max_dynamo_submission_size_setting.py
+-rw-r--r--   0        0        0     1530 2023-03-13 14:14:34.651994 codegrade-16.1.9/codegrade/models/max_file_size_setting.py
+-rw-r--r--   0        0        0     1574 2023-03-13 14:14:34.691995 codegrade-16.1.9/codegrade/models/max_large_upload_size_setting.py
+-rw-r--r--   0        0        0     1348 2023-03-13 14:14:34.727996 codegrade-16.1.9/codegrade/models/max_lines_setting.py
+-rw-r--r--   0        0        0     1435 2023-03-13 14:14:34.747996 codegrade-16.1.9/codegrade/models/max_mirror_file_age_setting.py
+-rw-r--r--   0        0        0     1580 2023-03-13 14:14:34.763997 codegrade-16.1.9/codegrade/models/max_normal_upload_size_setting.py
+-rw-r--r--   0        0        0     1400 2023-03-13 14:14:34.783998 codegrade-16.1.9/codegrade/models/max_number_of_files_setting.py
+-rw-r--r--   0        0        0     1422 2023-03-13 14:14:34.799998 codegrade-16.1.9/codegrade/models/max_plagiarism_matches_setting.py
+-rw-r--r--   0        0        0     1424 2023-03-13 14:14:34.815998 codegrade-16.1.9/codegrade/models/max_user_setting_amount_setting.py
+-rw-r--r--   0        0        0     1524 2023-03-13 14:14:34.852000 codegrade-16.1.9/codegrade/models/metric_evaluation_time_chunk_size_setting.py
+-rw-r--r--   0        0        0     1489 2023-03-13 14:14:34.852000 codegrade-16.1.9/codegrade/models/metric_evaluation_time_limit_setting.py
+-rw-r--r--   0        0        0     1430 2023-03-13 14:14:34.888001 codegrade-16.1.9/codegrade/models/metric_event_buffer_size_setting.py
+-rw-r--r--   0        0        0     1436 2023-03-13 14:14:34.888001 codegrade-16.1.9/codegrade/models/metric_gathering_enabled_setting.py
+-rw-r--r--   0        0        0     1481 2023-03-13 14:14:34.924002 codegrade-16.1.9/codegrade/models/metric_gathering_event_interval_setting.py
+-rw-r--r--   0        0        0     1493 2023-03-13 14:14:34.924002 codegrade-16.1.9/codegrade/models/metric_gathering_expressions_setting.py
+-rw-r--r--   0        0        0     1510 2023-03-13 14:14:34.956003 codegrade-16.1.9/codegrade/models/metric_gathering_time_interval_setting.py
+-rw-r--r--   0        0        0     1398 2023-03-13 14:14:34.960003 codegrade-16.1.9/codegrade/models/min_password_score_setting.py
+-rw-r--r--   0        0        0     2523 2023-03-13 14:14:35.008004 codegrade-16.1.9/codegrade/models/mirror_file_result.py
+-rw-r--r--   0        0        0     2164 2023-03-13 14:14:35.008004 codegrade-16.1.9/codegrade/models/missing_cookie_error.py
+-rw-r--r--   0        0        0     1863 2023-03-13 14:14:35.052005 codegrade-16.1.9/codegrade/models/missing_file.py
+-rw-r--r--   0        0        0     1539 2023-03-13 14:14:35.044005 codegrade-16.1.9/codegrade/models/new_auto_test_allowed_initial_build_ids_setting.py
+-rw-r--r--   0        0        0     1534 2023-03-13 14:14:35.084006 codegrade-16.1.9/codegrade/models/new_auto_test_build_max_command_time_setting.py
+-rw-r--r--   0        0        0     1641 2023-03-13 14:14:35.092007 codegrade-16.1.9/codegrade/models/new_auto_test_build_output_limit_setting.py
+-rw-r--r--   0        0        0     1458 2023-03-13 14:14:35.128008 codegrade-16.1.9/codegrade/models/new_auto_test_copying_enabled_setting.py
+-rw-r--r--   0        0        0     1539 2023-03-13 14:14:35.132008 codegrade-16.1.9/codegrade/models/new_auto_test_current_initial_build_ids_setting.py
+-rw-r--r--   0        0        0     1414 2023-03-13 14:14:35.164008 codegrade-16.1.9/codegrade/models/new_auto_test_enabled_setting.py
+-rw-r--r--   0        0        0     1458 2023-03-13 14:14:35.172009 codegrade-16.1.9/codegrade/models/new_auto_test_initial_build_id_setting.py
+-rw-r--r--   0        0        0     1626 2023-03-13 14:14:35.200009 codegrade-16.1.9/codegrade/models/new_auto_test_max_dynamodb_size_setting.py
+-rw-r--r--   0        0        0     1602 2023-03-13 14:14:35.212010 codegrade-16.1.9/codegrade/models/new_auto_test_max_file_size_setting.py
+-rw-r--r--   0        0        0     1620 2023-03-13 14:14:35.240011 codegrade-16.1.9/codegrade/models/new_auto_test_max_storage_size_setting.py
+-rw-r--r--   0        0        0     1514 2023-03-13 14:14:35.244011 codegrade-16.1.9/codegrade/models/new_auto_test_old_submission_age_setting.py
+-rw-r--r--   0        0        0     1528 2023-03-13 14:14:35.276012 codegrade-16.1.9/codegrade/models/new_auto_test_test_max_command_time_setting.py
+-rw-r--r--   0        0        0     1626 2023-03-13 14:14:35.284012 codegrade-16.1.9/codegrade/models/new_auto_test_test_output_limit_setting.py
+-rw-r--r--   0        0        0     1285 2023-03-13 14:14:35.304013 codegrade-16.1.9/codegrade/models/no_permissions.py
+-rw-r--r--   0        0        0     3658 2023-03-13 14:14:35.352014 codegrade-16.1.9/codegrade/models/non_deleted_comment_reply.py
+-rw-r--r--   0        0        0     4472 2023-03-13 14:14:35.392015 codegrade-16.1.9/codegrade/models/non_finalized_lti1p1_provider.py
+-rw-r--r--   0        0        0     7279 2023-03-13 14:14:35.492018 codegrade-16.1.9/codegrade/models/non_finalized_lti1p3_provider.py
+-rw-r--r--   0        0        0     1385 2023-03-13 14:14:35.424016 codegrade-16.1.9/codegrade/models/non_present_preference.py
+-rw-r--r--   0        0        0      868 2023-03-13 14:14:35.436016 codegrade-16.1.9/codegrade/models/notification.py
+-rw-r--r--   0        0        0     3037 2023-03-13 14:14:35.492018 codegrade-16.1.9/codegrade/models/notification_comment_reply_notification_as_json.py
+-rw-r--r--   0        0        0     2729 2023-03-13 14:14:35.544020 codegrade-16.1.9/codegrade/models/notification_general_feedback_reply_notification_as_json.py
+-rw-r--r--   0        0        0     1457 2023-03-13 14:14:35.532019 codegrade-16.1.9/codegrade/models/notification_poll_time_setting.py
+-rw-r--r--   0        0        0      253 2023-03-13 14:14:11.503317 codegrade-16.1.9/codegrade/models/notification_reasons.py
+-rw-r--r--   0        0        0     1855 2023-03-13 14:14:35.572020 codegrade-16.1.9/codegrade/models/notification_setting.py
+-rw-r--r--   0        0        0     2163 2023-03-13 14:14:35.584021 codegrade-16.1.9/codegrade/models/notification_setting_option.py
+-rw-r--r--   0        0        0     1327 2023-03-13 14:14:35.604021 codegrade-16.1.9/codegrade/models/notifications_json.py
+-rw-r--r--   0        0        0     2150 2023-03-13 14:14:35.628022 codegrade-16.1.9/codegrade/models/oauth_provider.py
+-rw-r--r--   0        0        0     2231 2023-03-13 14:14:35.652022 codegrade-16.1.9/codegrade/models/oauth_token.py
+-rw-r--r--   0        0        0     1698 2023-03-13 14:14:35.668023 codegrade-16.1.9/codegrade/models/option.py
+-rw-r--r--   0        0        0     1691 2023-03-13 14:14:35.692024 codegrade-16.1.9/codegrade/models/options_input_data.py
+-rw-r--r--   0        0        0     1993 2023-03-13 14:14:35.712024 codegrade-16.1.9/codegrade/models/parse_api_exception.py
+-rw-r--r--   0        0        0    92507 2023-03-13 14:14:45.388305 codegrade-16.1.9/codegrade/models/partial_all_site_settings.py
+-rw-r--r--   0        0        0     1555 2023-03-13 14:14:35.748025 codegrade-16.1.9/codegrade/models/patch1_p1_provider_lti_data.py
+-rw-r--r--   0        0        0     4217 2023-03-13 14:14:35.840028 codegrade-16.1.9/codegrade/models/patch1_p3_provider_lti_data.py
+-rw-r--r--   0        0        0     1355 2023-03-13 14:14:35.872029 codegrade-16.1.9/codegrade/models/patch_all_notification_data.py
+-rw-r--r--   0        0        0    17901 2023-03-13 14:14:36.652051 codegrade-16.1.9/codegrade/models/patch_assignment_data.py
+-rw-r--r--   0        0        0     1818 2023-03-13 14:14:36.696053 codegrade-16.1.9/codegrade/models/patch_auto_test_data.py
+-rw-r--r--   0        0        0     1228 2023-03-13 14:14:36.724053 codegrade-16.1.9/codegrade/models/patch_comment_reply_data.py
+-rw-r--r--   0        0        0     2129 2023-03-13 14:14:36.776055 codegrade-16.1.9/codegrade/models/patch_course_data.py
+-rw-r--r--   0        0        0     1240 2023-03-13 14:14:36.804056 codegrade-16.1.9/codegrade/models/patch_grader_submission_data.py
+-rw-r--r--   0        0        0     1248 2023-03-13 14:14:36.836057 codegrade-16.1.9/codegrade/models/patch_notification_data.py
+-rw-r--r--   0        0        0     1992 2023-03-13 14:14:36.880058 codegrade-16.1.9/codegrade/models/patch_notification_setting_user_setting_data.py
+-rw-r--r--   0        0        0     1497 2023-03-13 14:14:36.920059 codegrade-16.1.9/codegrade/models/patch_provider_lti_data.py
+-rw-r--r--   0        0        0     1858 2023-03-13 14:14:36.964060 codegrade-16.1.9/codegrade/models/patch_role_course_data.py
+-rw-r--r--   0        0        0     1828 2023-03-13 14:14:37.008062 codegrade-16.1.9/codegrade/models/patch_role_data.py
+-rw-r--r--   0        0        0     1858 2023-03-13 14:14:37.048063 codegrade-16.1.9/codegrade/models/patch_role_tenant_data.py
+-rw-r--r--   0        0        0     1966 2023-03-13 14:14:37.092064 codegrade-16.1.9/codegrade/models/patch_rubric_category_type_assignment_data.py
+-rw-r--r--   0        0        0     2946 2023-03-13 14:14:37.156066 codegrade-16.1.9/codegrade/models/patch_rubric_result_submission_data.py
+-rw-r--r--   0        0        0     1478 2023-03-13 14:14:37.196067 codegrade-16.1.9/codegrade/models/patch_section_data.py
+-rw-r--r--   0        0        0     1378 2023-03-13 14:14:37.224068 codegrade-16.1.9/codegrade/models/patch_settings_tenant_data.py
+-rw-r--r--   0        0        0     1369 2023-03-13 14:14:37.256069 codegrade-16.1.9/codegrade/models/patch_site_settings_data.py
+-rw-r--r--   0        0        0     1501 2023-03-13 14:14:37.292070 codegrade-16.1.9/codegrade/models/patch_snippet_course_data.py
+-rw-r--r--   0        0        0     1499 2023-03-13 14:14:37.328071 codegrade-16.1.9/codegrade/models/patch_snippet_data.py
+-rw-r--r--   0        0        0     2019 2023-03-13 14:14:37.392073 codegrade-16.1.9/codegrade/models/patch_submission_data.py
+-rw-r--r--   0        0        0     1945 2023-03-13 14:14:37.440074 codegrade-16.1.9/codegrade/models/patch_submit_types_assignment_data.py
+-rw-r--r--   0        0        0     2987 2023-03-13 14:14:37.500076 codegrade-16.1.9/codegrade/models/patch_tenant_data.py
+-rw-r--r--   0        0        0     1583 2023-03-13 14:14:37.540077 codegrade-16.1.9/codegrade/models/patch_ui_preference_user_setting_data.py
+-rw-r--r--   0        0        0     3228 2023-03-13 14:14:37.976090 codegrade-16.1.9/codegrade/models/patch_user_data.py
+-rw-r--r--   0        0        0     1240 2023-03-13 14:14:38.008090 codegrade-16.1.9/codegrade/models/pay_with_coupon_course_price_data.py
+-rw-r--r--   0        0        0     1418 2023-03-13 14:14:38.044092 codegrade-16.1.9/codegrade/models/peer_feedback_enabled_setting.py
+-rw-r--r--   0        0        0     3297 2023-03-13 14:14:38.112093 codegrade-16.1.9/codegrade/models/permission_exception.py
+-rw-r--r--   0        0        0     6831 2023-03-13 14:14:38.232097 codegrade-16.1.9/codegrade/models/plagiarism_run.py
+-rw-r--r--   0        0        0     1933 2023-03-13 14:14:38.272098 codegrade-16.1.9/codegrade/models/plagiarism_run_plagiarism_assignment_as_json.py
+-rw-r--r--   0        0        0     1859 2023-03-13 14:14:38.316099 codegrade-16.1.9/codegrade/models/plagiarism_run_plagiarism_course_as_json.py
+-rw-r--r--   0        0        0      371 2023-03-13 14:14:13.231366 codegrade-16.1.9/codegrade/models/plagiarism_state.py
+-rw-r--r--   0        0        0     1752 2023-03-13 14:14:38.356100 codegrade-16.1.9/codegrade/models/post_oauth_token_data.py
+-rw-r--r--   0        0        0     1668 2023-03-13 14:14:38.396102 codegrade-16.1.9/codegrade/models/present_preference.py
+-rw-r--r--   0        0        0     1087 2023-03-13 14:14:38.420102 codegrade-16.1.9/codegrade/models/proxy.py
+-rw-r--r--   0        0        0     1506 2023-03-13 14:14:38.460103 codegrade-16.1.9/codegrade/models/put_description_assignment_data.py
+-rw-r--r--   0        0        0     3196 2023-03-13 14:14:38.524105 codegrade-16.1.9/codegrade/models/put_enroll_link_course_data.py
+-rw-r--r--   0        0        0     2542 2023-03-13 14:14:38.580107 codegrade-16.1.9/codegrade/models/put_price_course_data.py
+-rw-r--r--   0        0        0     2542 2023-03-13 14:14:38.628108 codegrade-16.1.9/codegrade/models/put_price_tenant_data.py
+-rw-r--r--   0        0        0     2839 2023-03-13 14:14:38.684110 codegrade-16.1.9/codegrade/models/put_rubric_assignment_data.py
+-rw-r--r--   0        0        0      269 2023-03-13 14:14:12.467345 codegrade-16.1.9/codegrade/models/quality_comment_severity.py
+-rw-r--r--   0        0        0     2164 2023-03-13 14:14:38.736111 codegrade-16.1.9/codegrade/models/quality_test_log.py
+-rw-r--r--   0        0        0     2531 2023-03-13 14:14:38.784113 codegrade-16.1.9/codegrade/models/quality_test_log_base.py
+-rw-r--r--   0        0        0     1392 2023-03-13 14:14:38.824114 codegrade-16.1.9/codegrade/models/register_enabled_setting.py
+-rw-r--r--   0        0        0     2429 2023-03-13 14:14:38.880116 codegrade-16.1.9/codegrade/models/register_user_data.py
+-rw-r--r--   0        0        0     2153 2023-03-13 14:14:38.928117 codegrade-16.1.9/codegrade/models/register_user_with_link_course_data.py
+-rw-r--r--   0        0        0     3661 2023-03-13 14:14:39.032120 codegrade-16.1.9/codegrade/models/release_info.py
+-rw-r--r--   0        0        0     1465 2023-03-13 14:14:39.076121 codegrade-16.1.9/codegrade/models/release_message_max_time_setting.py
+-rw-r--r--   0        0        0     1205 2023-03-13 14:14:39.108122 codegrade-16.1.9/codegrade/models/rename_group_group_data.py
+-rw-r--r--   0        0        0     1406 2023-03-13 14:14:39.144123 codegrade-16.1.9/codegrade/models/render_html_enabled_setting.py
+-rw-r--r--   0        0        0     2128 2023-03-13 14:14:39.188125 codegrade-16.1.9/codegrade/models/repository_connection_limit_reached_exception.py
+-rw-r--r--   0        0        0     1421 2023-03-13 14:14:39.220125 codegrade-16.1.9/codegrade/models/reset_token_time_setting.py
+-rw-r--r--   0        0        0     8360 2023-03-13 14:14:39.744140 codegrade-16.1.9/codegrade/models/result_data_get_auto_test_get.py
+-rw-r--r--   0        0        0     2477 2023-03-13 14:14:39.796142 codegrade-16.1.9/codegrade/models/result_data_get_task_result_get_all.py
+-rw-r--r--   0        0        0     1770 2023-03-13 14:14:39.836143 codegrade-16.1.9/codegrade/models/result_data_post_login_link_login.py
+-rw-r--r--   0        0        0     1880 2023-03-13 14:14:39.876144 codegrade-16.1.9/codegrade/models/result_data_post_section_create_division.py
+-rw-r--r--   0        0        0     1750 2023-03-13 14:14:39.916145 codegrade-16.1.9/codegrade/models/result_data_post_user_login.py
+-rw-r--r--   0        0        0     1762 2023-03-13 14:14:39.960147 codegrade-16.1.9/codegrade/models/result_data_post_user_register.py
+-rw-r--r--   0        0        0     2391 2023-03-13 14:14:40.012148 codegrade-16.1.9/codegrade/models/role_as_json_with_perms.py
+-rw-r--r--   0        0        0     1940 2023-03-13 14:14:40.056150 codegrade-16.1.9/codegrade/models/root_file_trees_json.py
+-rw-r--r--   0        0        0      241 2023-03-13 14:14:12.811354 codegrade-16.1.9/codegrade/models/rubric_description_type.py
+-rw-r--r--   0        0        0     1599 2023-03-13 14:14:40.096151 codegrade-16.1.9/codegrade/models/rubric_enabled_for_teacher_on_submissions_page_setting.py
+-rw-r--r--   0        0        0     1663 2023-03-13 14:14:40.136152 codegrade-16.1.9/codegrade/models/rubric_item.py
+-rw-r--r--   0        0        0     2265 2023-03-13 14:14:40.192154 codegrade-16.1.9/codegrade/models/rubric_item_input_as_json.py
+-rw-r--r--   0        0        0      235 2023-03-13 14:14:13.055362 codegrade-16.1.9/codegrade/models/rubric_lock_reason.py
+-rw-r--r--   0        0        0     3803 2023-03-13 14:14:40.272156 codegrade-16.1.9/codegrade/models/rubric_row_base.py
+-rw-r--r--   0        0        0     2844 2023-03-13 14:14:40.336158 codegrade-16.1.9/codegrade/models/rubric_row_base_input_as_json.py
+-rw-r--r--   0        0        0     1993 2023-03-13 14:14:40.380159 codegrade-16.1.9/codegrade/models/rubric_row_base_input_base_as_json.py
+-rw-r--r--   0        0        0     1386 2023-03-13 14:14:40.416160 codegrade-16.1.9/codegrade/models/rubrics_enabled_setting.py
+-rw-r--r--   0        0        0      221 2023-03-13 14:14:13.403371 codegrade-16.1.9/codegrade/models/rule_type.py
+-rw-r--r--   0        0        0     2113 2023-03-13 14:14:40.460161 codegrade-16.1.9/codegrade/models/run_program_as_json.py
+-rw-r--r--   0        0        0     1156 2023-03-13 14:14:40.496162 codegrade-16.1.9/codegrade/models/run_program_data.py
+-rw-r--r--   0        0        0     1590 2023-03-13 14:14:40.532163 codegrade-16.1.9/codegrade/models/run_program_extra.py
+-rw-r--r--   0        0        0     2105 2023-03-13 14:14:40.576165 codegrade-16.1.9/codegrade/models/run_program_input_as_json.py
+-rw-r--r--   0        0        0     2505 2023-03-13 14:14:40.628166 codegrade-16.1.9/codegrade/models/run_program_log.py
+-rw-r--r--   0        0        0     2164 2023-03-13 14:14:40.676168 codegrade-16.1.9/codegrade/models/saml2_provider_json.py
+-rw-r--r--   0        0        0     1929 2023-03-13 14:14:40.720169 codegrade-16.1.9/codegrade/models/saml_ui_info.py
+-rw-r--r--   0        0        0     1430 2023-03-13 14:14:40.756170 codegrade-16.1.9/codegrade/models/send_registration_email_setting.py
+-rw-r--r--   0        0        0     1477 2023-03-13 14:14:40.792171 codegrade-16.1.9/codegrade/models/server_time_correction_enabled_setting.py
+-rw-r--r--   0        0        0     1477 2023-03-13 14:14:40.828172 codegrade-16.1.9/codegrade/models/server_time_diff_tolerance_setting.py
+-rw-r--r--   0        0        0     1471 2023-03-13 14:14:40.860173 codegrade-16.1.9/codegrade/models/server_time_sync_interval_setting.py
+-rw-r--r--   0        0        0     1433 2023-03-13 14:14:40.908174 codegrade-16.1.9/codegrade/models/setting_token_time_setting.py
+-rw-r--r--   0        0        0     1265 2023-03-13 14:14:40.940175 codegrade-16.1.9/codegrade/models/setup_oauth_result.py
+-rw-r--r--   0        0        0     1354 2023-03-13 14:14:40.972176 codegrade-16.1.9/codegrade/models/site_email_setting.py
+-rw-r--r--   0        0        0    18379 2023-03-13 14:14:41.144181 codegrade-16.1.9/codegrade/models/site_setting_input.py
+-rw-r--r--   0        0        0     1690 2023-03-13 14:14:41.184183 codegrade-16.1.9/codegrade/models/snippet.py
+-rw-r--r--   0        0        0     1489 2023-03-13 14:14:41.220183 codegrade-16.1.9/codegrade/models/sso_username_decollision_enabled_setting.py
+-rw-r--r--   0        0        0     1303 2023-03-13 14:14:41.248184 codegrade-16.1.9/codegrade/models/start_payment_course_price_close_tab_data.py
+-rw-r--r--   0        0        0      825 2023-03-13 14:14:41.264185 codegrade-16.1.9/codegrade/models/start_payment_course_price_data.py
+-rw-r--r--   0        0        0     2068 2023-03-13 14:14:41.304186 codegrade-16.1.9/codegrade/models/start_payment_course_price_redirect_data.py
+-rw-r--r--   0        0        0     1803 2023-03-13 14:14:41.344187 codegrade-16.1.9/codegrade/models/started_transaction.py
+-rw-r--r--   0        0        0     1430 2023-03-13 14:14:41.384188 codegrade-16.1.9/codegrade/models/student_payment_enabled_setting.py
+-rw-r--r--   0        0        0     2376 2023-03-13 14:14:41.436190 codegrade-16.1.9/codegrade/models/submission_validator_input_data.py
+-rw-r--r--   0        0        0      349 2023-03-13 14:14:13.267368 codegrade-16.1.9/codegrade/models/task_result_state.py
+-rw-r--r--   0        0        0      247 2023-03-13 14:14:12.687351 codegrade-16.1.9/codegrade/models/tax_behavior.py
+-rw-r--r--   0        0        0     4104 2023-03-13 14:14:41.952205 codegrade-16.1.9/codegrade/models/tenant.py
+-rw-r--r--   0        0        0     1879 2023-03-13 14:14:41.992206 codegrade-16.1.9/codegrade/models/tenant_course_statistics.py
+-rw-r--r--   0        0        0     1243 2023-03-13 14:14:42.020207 codegrade-16.1.9/codegrade/models/tenant_of_tenant_price.py
+-rw-r--r--   0        0        0     1699 2023-03-13 14:14:42.068208 codegrade-16.1.9/codegrade/models/tenant_permissions.py
+-rw-r--r--   0        0        0     2077 2023-03-13 14:14:42.120210 codegrade-16.1.9/codegrade/models/tenant_price.py
+-rw-r--r--   0        0        0     2415 2023-03-13 14:14:42.172211 codegrade-16.1.9/codegrade/models/tenant_role_as_json_with_perms.py
+-rw-r--r--   0        0        0     2944 2023-03-13 14:14:42.224213 codegrade-16.1.9/codegrade/models/tenant_statistics.py
+-rw-r--r--   0        0        0     1535 2023-03-13 14:14:42.256214 codegrade-16.1.9/codegrade/models/test_submission_copying_on_import_enabled_setting.py
+-rw-r--r--   0        0        0     1588 2023-03-13 14:14:42.296215 codegrade-16.1.9/codegrade/models/timed_availability.py
+-rw-r--r--   0        0        0     1969 2023-03-13 14:14:42.344216 codegrade-16.1.9/codegrade/models/token_revoked_exception.py
+-rw-r--r--   0        0        0     1425 2023-03-13 14:14:42.380217 codegrade-16.1.9/codegrade/models/tour_configurations_setting.py
+-rw-r--r--   0        0        0     1416 2023-03-13 14:14:42.416218 codegrade-16.1.9/codegrade/models/tour_polling_interval_setting.py
+-rw-r--r--   0        0        0     2943 2023-03-13 14:14:42.480220 codegrade-16.1.9/codegrade/models/transaction.py
+-rw-r--r--   0        0        0      299 2023-03-13 14:14:11.895328 codegrade-16.1.9/codegrade/models/transaction_state.py
+-rw-r--r--   0        0        0     1036 2023-03-13 14:14:42.504221 codegrade-16.1.9/codegrade/models/types.py
+-rw-r--r--   0        0        0     3418 2023-03-13 14:14:42.568223 codegrade-16.1.9/codegrade/models/update_peer_feedback_settings_assignment_data.py
+-rw-r--r--   0        0        0     1752 2023-03-13 14:14:42.604224 codegrade-16.1.9/codegrade/models/update_set_auto_test_data.py
+-rw-r--r--   0        0        0     3439 2023-03-13 14:14:42.668226 codegrade-16.1.9/codegrade/models/update_suite_auto_test_base_data.py
+-rw-r--r--   0        0        0     4543 2023-03-13 14:14:42.748228 codegrade-16.1.9/codegrade/models/update_suite_auto_test_data.py
+-rw-r--r--   0        0        0     2231 2023-03-13 14:14:42.796229 codegrade-16.1.9/codegrade/models/upgraded_lti_provider_exception.py
+-rw-r--r--   0        0        0     1516 2023-03-13 14:14:42.832230 codegrade-16.1.9/codegrade/models/upload_submission_assignment_data.py
+-rw-r--r--   0        0        0     2128 2023-03-13 14:14:42.880232 codegrade-16.1.9/codegrade/models/user.py
+-rw-r--r--   0        0        0     1555 2023-03-13 14:14:42.916233 codegrade-16.1.9/codegrade/models/user_course.py
+-rw-r--r--   0        0        0     2118 2023-03-13 14:14:42.964234 codegrade-16.1.9/codegrade/models/user_info_with_role.py
+-rw-r--r--   0        0        0     1993 2023-03-13 14:14:43.008236 codegrade-16.1.9/codegrade/models/user_input.py
+-rw-r--r--   0        0        0     2663 2023-03-13 14:14:43.064237 codegrade-16.1.9/codegrade/models/user_without_group.py
+-rw-r--r--   0        0        0     2125 2023-03-13 14:14:43.112239 codegrade-16.1.9/codegrade/models/weak_password_exception.py
+-rw-r--r--   0        0        0     1651 2023-03-13 14:14:43.156240 codegrade-16.1.9/codegrade/models/weak_password_feedback.py
+-rw-r--r--   0        0        0     3456 2023-03-13 14:14:43.232242 codegrade-16.1.9/codegrade/models/webhook_base.py
+-rw-r--r--   0        0        0     4476 2023-03-13 14:14:43.320245 codegrade-16.1.9/codegrade/models/work.py
+-rw-r--r--   0        0        0      245 2023-03-13 14:14:12.987360 codegrade-16.1.9/codegrade/models/work_origin.py
+-rw-r--r--   0        0        0     2898 2023-03-13 14:14:43.376246 codegrade-16.1.9/codegrade/models/work_rubric_item.py
+-rw-r--r--   0        0        0     2757 2023-03-13 14:14:43.432248 codegrade-16.1.9/codegrade/models/work_rubric_result_as_json.py
+-rw-r--r--   0        0        0     2155 2023-03-13 14:14:43.476249 codegrade-16.1.9/codegrade/models/work_rubric_result_points_as_json.py
+-rw-r--r--   0        0        0     3932 2023-03-13 14:14:43.576252 codegrade-16.1.9/codegrade/parsers.py
+-rw-r--r--   0        0        0        0 2023-03-13 14:14:10.415286 codegrade-16.1.9/codegrade/py.typed
+-rw-r--r--   0        0        0     7278 2023-03-13 14:14:44.176270 codegrade-16.1.9/codegrade/utils.py
+-rw-r--r--   0        0        0     1364 2023-03-13 14:14:10.447287 codegrade-16.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3068 1970-01-01 00:00:00.000000 codegrade-16.1.9/setup.py
+-rw-r--r--   0        0        0     2971 1970-01-01 00:00:00.000000 codegrade-16.1.9/PKG-INFO
```

### Comparing `codegrade-16.1.8/README.md` & `codegrade-16.1.9/README.md`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_dt_utils/__init__.py` & `codegrade-16.1.9/cg_dt_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_maybe/_just.py` & `codegrade-16.1.9/cg_maybe/_just.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_maybe/_nothing.py` & `codegrade-16.1.9/cg_maybe/_nothing.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_maybe/_type_helpers.py` & `codegrade-16.1.9/cg_maybe/_type_helpers.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_maybe/cg_maybe_plugin.py` & `codegrade-16.1.9/cg_maybe/cg_maybe_plugin.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_maybe/utils.py` & `codegrade-16.1.9/cg_maybe/utils.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/__init__.py` & `codegrade-16.1.9/cg_request_args/__init__.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_any_value.py` & `codegrade-16.1.9/cg_request_args/_any_value.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_base.py` & `codegrade-16.1.9/cg_request_args/_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_convert.py` & `codegrade-16.1.9/cg_request_args/_convert.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_enum.py` & `codegrade-16.1.9/cg_request_args/_enum.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_lazy.py` & `codegrade-16.1.9/cg_request_args/_lazy.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_list.py` & `codegrade-16.1.9/cg_request_args/_list.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_literal.py` & `codegrade-16.1.9/cg_request_args/_literal.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_mapping.py` & `codegrade-16.1.9/cg_request_args/_mapping.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_multipart.py` & `codegrade-16.1.9/cg_request_args/_multipart.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_nullable.py` & `codegrade-16.1.9/cg_request_args/_nullable.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_parse_utils.py` & `codegrade-16.1.9/cg_request_args/_parse_utils.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_query.py` & `codegrade-16.1.9/cg_request_args/_query.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_rich_value.py` & `codegrade-16.1.9/cg_request_args/_rich_value.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_swagger_utils.py` & `codegrade-16.1.9/cg_request_args/_swagger_utils.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_swaggerize.py` & `codegrade-16.1.9/cg_request_args/_swaggerize.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/_utils.py` & `codegrade-16.1.9/cg_request_args/_utils.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/exceptions.py` & `codegrade-16.1.9/cg_request_args/exceptions.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/cg_request_args/request_args_plugin.py` & `codegrade-16.1.9/cg_request_args/request_args_plugin.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/__init__.py` & `codegrade-16.1.9/codegrade/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 SPDX-License-Identifier: AGPL-3.0-only OR BSD-3-Clause-Clear
 """
 from functools import wraps
 
 from .client import AuthenticatedClient, Client
 
 __all__ = ("login", "AuthenticatedClient", "Client", "login_from_cli")
-__version__ = "16.1.8"
+__version__ = "16.1.9"
 
 
 @wraps(AuthenticatedClient.get)
 def login(*args, **kwargs):
     return AuthenticatedClient.get(*args, **kwargs)
```

### Comparing `codegrade-16.1.8/codegrade/_api/about.py` & `codegrade-16.1.9/codegrade/_api/about.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/assignment.py` & `codegrade-16.1.9/codegrade/_api/assignment.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/auto_test.py` & `codegrade-16.1.9/codegrade/_api/auto_test.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/comment.py` & `codegrade-16.1.9/codegrade/_api/comment.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/course.py` & `codegrade-16.1.9/codegrade/_api/course.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/course_price.py` & `codegrade-16.1.9/codegrade/_api/course_price.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/file.py` & `codegrade-16.1.9/codegrade/_api/file.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/git_provider.py` & `codegrade-16.1.9/codegrade/_api/git_provider.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/group.py` & `codegrade-16.1.9/codegrade/_api/group.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/group_set.py` & `codegrade-16.1.9/codegrade/_api/group_set.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/login_link.py` & `codegrade-16.1.9/codegrade/_api/login_link.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/lti.py` & `codegrade-16.1.9/codegrade/_api/lti.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/notification.py` & `codegrade-16.1.9/codegrade/_api/notification.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/oauth_provider.py` & `codegrade-16.1.9/codegrade/_api/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/oauth_token.py` & `codegrade-16.1.9/codegrade/_api/oauth_token.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/permission.py` & `codegrade-16.1.9/codegrade/_api/permission.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/plagiarism.py` & `codegrade-16.1.9/codegrade/_api/plagiarism.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/role.py` & `codegrade-16.1.9/codegrade/_api/role.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/section.py` & `codegrade-16.1.9/codegrade/_api/section.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/site_settings.py` & `codegrade-16.1.9/codegrade/_api/site_settings.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/snippet.py` & `codegrade-16.1.9/codegrade/_api/snippet.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/sso_provider.py` & `codegrade-16.1.9/codegrade/_api/sso_provider.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/submission.py` & `codegrade-16.1.9/codegrade/_api/submission.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/task_result.py` & `codegrade-16.1.9/codegrade/_api/task_result.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/tenant.py` & `codegrade-16.1.9/codegrade/_api/tenant.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/transaction.py` & `codegrade-16.1.9/codegrade/_api/transaction.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/user.py` & `codegrade-16.1.9/codegrade/_api/user.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/_api/user_setting.py` & `codegrade-16.1.9/codegrade/_api/user_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/client.py` & `codegrade-16.1.9/codegrade/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     from codegrade._api.transaction import (
         TransactionService as _TransactionService,
     )
     from codegrade._api.user import UserService as _UserService
     from codegrade._api.user_setting import (
         UserSettingService as _UserSettingService,
     )
+    from codegrade._api.webhook import WebhookService as _WebhookService
 
 
 class _BaseClient:
     """A base class for keeping track of data related to the API."""
 
     __slots__ = (
         "__about",
@@ -105,14 +106,15 @@
         "__sso_provider",
         "__submission",
         "__task_result",
         "__tenant",
         "__transaction",
         "__user",
         "__user_setting",
+        "__webhook",
         "__open_level",
         "__http",
         "base_url",
     )
 
     def __init__(self: "_BaseClientT", base_url: str) -> None:
         # Open level makes it possible to efficiently nest the context manager.
@@ -171,14 +173,15 @@
         self.__transaction: t.Optional[
             "_TransactionService[_BaseClientT]"
         ] = None
         self.__user: t.Optional["_UserService[_BaseClientT]"] = None
         self.__user_setting: t.Optional[
             "_UserSettingService[_BaseClientT]"
         ] = None
+        self.__webhook: t.Optional["_WebhookService[_BaseClientT]"] = None
         self.__http: t.Optional[httpx.Client] = None
 
     def _get_headers(self) -> t.Mapping[str, str]:
         """Get headers to be used in all endpoints"""
         return {}
 
     @abc.abstractmethod
@@ -500,14 +503,23 @@
         """
         if self.__user_setting is None:
             import codegrade._api.user_setting as m
 
             self.__user_setting = m.UserSettingService(self)
         return self.__user_setting
 
+    @property
+    def webhook(self: _BaseClientT) -> "_WebhookService[_BaseClientT]":
+        """Get a :class:`.WebhookService` to do requests concerning Webhook."""
+        if self.__webhook is None:
+            import codegrade._api.webhook as m
+
+            self.__webhook = m.WebhookService(self)
+        return self.__webhook
+
 
 class Client(_BaseClient):
     """A class used to do unauthenticated requests to CodeGrade"""
 
     __slots__ = ()
 
     def _make_http(self) -> httpx.Client:
```

### Comparing `codegrade-16.1.8/codegrade/errors.py` & `codegrade-16.1.9/codegrade/errors.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/__init__.py` & `codegrade-16.1.9/codegrade/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -282,14 +282,16 @@
 from .file_tree import FileTree
 from .file_type import FileType
 from .finalized_lti1p1_provider import FinalizedLTI1p1Provider
 from .finalized_lti1p3_provider import FinalizedLTI1p3Provider
 from .find_element_interval_setting import FindElementIntervalSetting
 from .find_element_max_tries_setting import FindElementMaxTriesSetting
 from .first_phase_lti_launch_exception import FirstPhaseLTILaunchException
+from .fixed_availability import FixedAvailability
+from .fixed_grade_availability import FixedGradeAvailability
 from .fixture_like import FixtureLike
 from .fraction import Fraction
 from .frontend_site_settings import FrontendSiteSettings
 from .general_feedback_comment_base import GeneralFeedbackCommentBase
 from .general_feedback_comment_base_with_extended_replies import (
     GeneralFeedbackCommentBaseWithExtendedReplies,
 )
@@ -521,14 +523,17 @@
 from .register_enabled_setting import RegisterEnabledSetting
 from .register_user_data import RegisterUserData
 from .register_user_with_link_course_data import RegisterUserWithLinkCourseData
 from .release_info import ReleaseInfo
 from .release_message_max_time_setting import ReleaseMessageMaxTimeSetting
 from .rename_group_group_data import RenameGroupGroupData
 from .render_html_enabled_setting import RenderHtmlEnabledSetting
+from .repository_connection_limit_reached_exception import (
+    RepositoryConnectionLimitReachedException,
+)
 from .reset_token_time_setting import ResetTokenTimeSetting
 from .result_data_get_auto_test_get import ResultDataGetAutoTestGet
 from .result_data_get_task_result_get_all import ResultDataGetTaskResultGetAll
 from .result_data_post_login_link_login import ResultDataPostLoginLinkLogin
 from .result_data_post_section_create_division import (
     ResultDataPostSectionCreateDivision,
 )
@@ -587,14 +592,16 @@
 from .tenant_permissions import TenantPermissions
 from .tenant_price import TenantPrice
 from .tenant_role_as_json_with_perms import TenantRoleAsJSONWithPerms
 from .tenant_statistics import TenantStatistics
 from .test_submission_copying_on_import_enabled_setting import (
     TestSubmissionCopyingOnImportEnabledSetting,
 )
+from .timed_availability import TimedAvailability
+from .token_revoked_exception import TokenRevokedException
 from .tour_configurations_setting import TourConfigurationsSetting
 from .tour_polling_interval_setting import TourPollingIntervalSetting
 from .transaction import Transaction
 from .transaction_state import TransactionState
 from .types import *
 from .update_peer_feedback_settings_assignment_data import (
     UpdatePeerFeedbackSettingsAssignmentData,
```

### Comparing `codegrade-16.1.8/codegrade/models/_base_price.py` & `codegrade-16.1.9/codegrade/models/_base_price.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/_saml_ui_logo_info.py` & `codegrade-16.1.9/codegrade/models/_saml_ui_logo_info.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/_submission_rubric_item_data_parser.py` & `codegrade-16.1.9/codegrade/models/_submission_rubric_item_data_parser.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/about.py` & `codegrade-16.1.9/codegrade/models/about.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/abstract_role.py` & `codegrade-16.1.9/codegrade/models/abstract_role.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/add_users_section_data.py` & `codegrade-16.1.9/codegrade/models/add_users_section_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/all_auto_test_results.py` & `codegrade-16.1.9/codegrade/models/all_auto_test_results.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/all_site_settings.py` & `codegrade-16.1.9/codegrade/models/all_site_settings.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/any_auto_test_step_as_json.py` & `codegrade-16.1.9/codegrade/models/any_auto_test_step_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/any_error.py` & `codegrade-16.1.9/codegrade/models/any_error.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,27 +24,33 @@
 from .ignored_files_exception import IgnoredFilesException
 from .invalid_group_exception import InvalidGroupException
 from .invalid_io_cases_exception import InvalidIOCasesException
 from .invalid_options_exception import InvalidOptionsException
 from .missing_cookie_error import MissingCookieError
 from .parse_api_exception import ParseAPIException
 from .permission_exception import PermissionException
+from .repository_connection_limit_reached_exception import (
+    RepositoryConnectionLimitReachedException,
+)
+from .token_revoked_exception import TokenRevokedException
 from .upgraded_lti_provider_exception import UpgradedLTIProviderException
 from .weak_password_exception import WeakPasswordException
 
 AnyError = t.Union[
     DisabledSettingException,
     WeakPasswordException,
     ParseAPIException,
     InvalidIOCasesException,
     PermissionException,
     FailedToSendEmailException,
     GroupNotReadyForSubmissionException,
     InvalidGroupException,
     AutoTestStepValidationException,
+    RepositoryConnectionLimitReachedException,
+    TokenRevokedException,
     MissingCookieError,
     IgnoredFilesException,
     InvalidOptionsException,
     UpgradedLTIProviderException,
     FirstPhaseLTILaunchException,
     BaseError,
 ]
@@ -55,14 +61,16 @@
         ParserFor.make(ParseAPIException),
         ParserFor.make(InvalidIOCasesException),
         ParserFor.make(PermissionException),
         ParserFor.make(FailedToSendEmailException),
         ParserFor.make(GroupNotReadyForSubmissionException),
         ParserFor.make(InvalidGroupException),
         ParserFor.make(AutoTestStepValidationException),
+        ParserFor.make(RepositoryConnectionLimitReachedException),
+        ParserFor.make(TokenRevokedException),
         ParserFor.make(MissingCookieError),
         ParserFor.make(IgnoredFilesException),
         ParserFor.make(InvalidOptionsException),
         ParserFor.make(UpgradedLTIProviderException),
         ParserFor.make(FirstPhaseLTILaunchException),
         ParserFor.make(BaseError),
     ),
```

### Comparing `codegrade-16.1.8/codegrade/models/any_non_redacted_auto_test_step_as_json.py` & `codegrade-16.1.9/codegrade/models/any_non_redacted_auto_test_step_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/any_redacted_auto_test_step_as_json.py` & `codegrade-16.1.9/codegrade/models/any_redacted_auto_test_step_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/api_codes.py` & `codegrade-16.1.9/codegrade/models/api_codes.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,7 +53,10 @@
     LTI1_3_ERROR = "LTI1_3_ERROR"
     LTI1_3_COOKIE_ERROR = "LTI1_3_COOKIE_ERROR"
     LTI1_1_ERROR = "LTI1_1_ERROR"
     IMAGE_BEING_CREATED = "IMAGE_BEING_CREATED"
     OBJECT_TOO_NEW = "OBJECT_TOO_NEW"
     SKIPPED_RESULT = "SKIPPED_RESULT"
     LIMIT_REACHED = "LIMIT_REACHED"
+    TOKEN_REVOKED = "TOKEN_REVOKED"
+    REPO_ALREADY_CONNECTED = "REPO_ALREADY_CONNECTED"
+    REPO_CONNECTION_LIMIT_REACHED = "REPO_CONNECTION_LIMIT_REACHED"
```

### Comparing `codegrade-16.1.8/codegrade/models/assignment.py` & `codegrade-16.1.9/codegrade/models/assignment.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,31 +15,36 @@
 from .assignment_kind import AssignmentKind
 from .assignment_peer_feedback_settings import AssignmentPeerFeedbackSettings
 from .assignment_percentage_grading_settings import (
     AssignmentPercentageGradingSettings,
 )
 from .assignment_points_grading_settings import AssignmentPointsGradingSettings
 from .cg_ignore_version import CGIgnoreVersion
+from .fixed_availability import FixedAvailability
+from .fixed_grade_availability import FixedGradeAvailability
 from .group_set import GroupSet
 from .submission_validator_input_data import SubmissionValidatorInputData
+from .timed_availability import TimedAvailability
 
 
 @dataclass
 class Assignment:
     """The serialization of an assignment.
 
     See the comments in the source code for the meaning of each field.
     """
 
     #: The id of the assignment.
     id: "int"
-    #: Current state of the assignment.
+    #: Current state of the assignment. Deprecated: use availability and
+    #: grade\_availability fields, it will be removed in Q3 2023.
     state: "t.Literal['done', 'grading', 'hidden', 'submitting']"
     #: Description of the assignment. Deprecated, use available routes to
-    #: upload and retrieve a description file instead.
+    #: upload and retrieve a description file instead. It will be removed in Q3
+    #: 2023.
     description: "t.Optional[str]"
     #: Whether the assignment has liked description file.
     has_description: "bool"
     #: When this assignment was created.
     created_at: "datetime.datetime"
     #: The deadline of the assignment. It is possible the assignment has no
     #: deadline yet, in which case it will be `None`.
@@ -56,15 +61,16 @@
     #: The cginore.
     cgignore: "t.Optional[t.Union[SubmissionValidatorInputData, str]]"
     #: The version of the cignore file.
     cgignore_version: "t.Optional[CGIgnoreVersion]"
     #: The time the assignment will become available (i.e. the state will
     #: switch from 'hidden' to 'open'). If the state is not 'hidden' this value
     #: has no meaning. If this value is not `None` you cannot change to state
-    #: to 'hidden' or 'open'.
+    #: to 'hidden' or 'open'. Deprecated: use availability and
+    #: grade\_availability fields, it will be removed in Q3 2023.
     available_at: "t.Optional[datetime.datetime]"
     #: Should we send login links to all users before the `available_at` time.
     send_login_links: "bool"
     #: The fixed value for the maximum that can be achieved in a rubric. This
     #: can be higher and lower than the actual max. Will be `None` if unset.
     fixed_max_rubric_points: "t.Optional[float]"
     #: The maximum grade you can get for this assignment. This is based around
@@ -125,36 +131,44 @@
     #: What kind of assignment is this.
     kind: "AssignmentKind"
     #: The anonymization algorithm used for this assignment.
     anonymized_grading: "t.Optional[AssignmentAnonymizationAlgo]"
     #: Optionally a glob for a file that should be loaded first in the file
     #: viewer. There is no guarantee that any file actually matches this glob.
     file_to_load_first: "t.Optional[str]"
+    #: What is the availability state of this assignment.
+    availability: "t.Union[FixedAvailability, TimedAvailability]"
+    #: What is grade availability of this assignment.
+    grade_availability: "FixedGradeAvailability"
 
     raw_data: t.Optional[t.Dict[str, t.Any]] = field(init=False, repr=False)
 
     data_parser: t.ClassVar = rqa.Lazy(
         lambda: rqa.FixedMapping(
             rqa.RequiredArgument(
                 "id",
                 rqa.SimpleValue.int,
                 doc="The id of the assignment.",
             ),
             rqa.RequiredArgument(
                 "state",
                 rqa.StringEnum("done", "grading", "hidden", "submitting"),
-                doc="Current state of the assignment.",
+                doc=(
+                    "Current state of the assignment. Deprecated: use"
+                    " availability and grade\\_availability fields, it will be"
+                    " removed in Q3 2023."
+                ),
             ),
             rqa.RequiredArgument(
                 "description",
                 rqa.Nullable(rqa.SimpleValue.str),
                 doc=(
                     "Description of the assignment. Deprecated, use available"
                     " routes to upload and retrieve a description file"
-                    " instead."
+                    " instead. It will be removed in Q3 2023."
                 ),
             ),
             rqa.RequiredArgument(
                 "has_description",
                 rqa.SimpleValue.bool,
                 doc="Whether the assignment has liked description file.",
             ),
@@ -214,15 +228,17 @@
                 "available_at",
                 rqa.Nullable(rqa.RichValue.DateTime),
                 doc=(
                     "The time the assignment will become available (i.e. the"
                     " state will switch from 'hidden' to 'open'). If the state"
                     " is not 'hidden' this value has no meaning. If this value"
                     " is not `None` you cannot change to state to 'hidden' or"
-                    " 'open'."
+                    " 'open'. Deprecated: use availability and"
+                    " grade\\_availability fields, it will be removed in Q3"
+                    " 2023."
                 ),
             ),
             rqa.RequiredArgument(
                 "send_login_links",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Should we send login links to all users before the"
@@ -400,14 +416,27 @@
                 rqa.Nullable(rqa.SimpleValue.str),
                 doc=(
                     "Optionally a glob for a file that should be loaded first"
                     " in the file viewer. There is no guarantee that any file"
                     " actually matches this glob."
                 ),
             ),
+            rqa.RequiredArgument(
+                "availability",
+                parsers.make_union(
+                    parsers.ParserFor.make(FixedAvailability),
+                    parsers.ParserFor.make(TimedAvailability),
+                ),
+                doc="What is the availability state of this assignment.",
+            ),
+            rqa.RequiredArgument(
+                "grade_availability",
+                parsers.ParserFor.make(FixedGradeAvailability),
+                doc="What is grade availability of this assignment.",
+            ),
         ).use_readable_describe(True)
     )
 
     def to_dict(self) -> t.Dict[str, t.Any]:
         res: t.Dict[str, t.Any] = {
             "id": to_dict(self.id),
             "state": to_dict(self.state),
@@ -442,14 +471,16 @@
             "done_type": to_dict(self.done_type),
             "done_email": to_dict(self.done_email),
             "division_parent_id": to_dict(self.division_parent_id),
             "analytics_workspace_ids": to_dict(self.analytics_workspace_ids),
             "kind": to_dict(self.kind),
             "anonymized_grading": to_dict(self.anonymized_grading),
             "file_to_load_first": to_dict(self.file_to_load_first),
+            "availability": to_dict(self.availability),
+            "grade_availability": to_dict(self.grade_availability),
         }
         return res
 
     @classmethod
     def from_dict(
         cls: t.Type["Assignment"], d: t.Dict[str, t.Any]
     ) -> "Assignment":
@@ -487,10 +518,12 @@
             done_type=parsed.done_type,
             done_email=parsed.done_email,
             division_parent_id=parsed.division_parent_id,
             analytics_workspace_ids=parsed.analytics_workspace_ids,
             kind=parsed.kind,
             anonymized_grading=parsed.anonymized_grading,
             file_to_load_first=parsed.file_to_load_first,
+            availability=parsed.availability,
+            grade_availability=parsed.grade_availability,
         )
         res.raw_data = d
         return res
```

### Comparing `codegrade-16.1.8/codegrade/models/assignment_default_grading_scale_points_setting.py` & `codegrade-16.1.9/codegrade/models/assignment_default_grading_scale_points_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_default_grading_scale_setting.py` & `codegrade-16.1.9/codegrade/models/assignment_default_grading_scale_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_description_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/assignment_description_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_feedback.py` & `codegrade-16.1.9/codegrade/models/assignment_feedback.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_grader.py` & `codegrade-16.1.9/codegrade/models/assignment_grader.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_grading_scale_points_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/assignment_grading_scale_points_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_login_link.py` & `codegrade-16.1.9/codegrade/models/assignment_login_link.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_max_points_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/assignment_max_points_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_peer_feedback_connection.py` & `codegrade-16.1.9/codegrade/models/assignment_peer_feedback_connection.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_peer_feedback_settings.py` & `codegrade-16.1.9/codegrade/models/assignment_peer_feedback_settings.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_percentage_decimals_setting.py` & `codegrade-16.1.9/codegrade/models/assignment_percentage_decimals_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_percentage_grading_settings.py` & `codegrade-16.1.9/codegrade/models/assignment_percentage_grading_settings.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_point_decimals_setting.py` & `codegrade-16.1.9/codegrade/models/assignment_point_decimals_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_points_grading_settings.py` & `codegrade-16.1.9/codegrade/models/assignment_points_grading_settings.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/assignment_template.py` & `codegrade-16.1.9/codegrade/models/assignment_template.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/at_image_caching_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/at_image_caching_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test.py` & `codegrade-16.1.9/codegrade/models/auto_test.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_capture_points_message_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_capture_points_message_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_checkpoint_message_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_checkpoint_message_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_code_quality_message_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_code_quality_message_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_fixture.py` & `codegrade-16.1.9/codegrade/models/auto_test_fixture.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_global_setup_output.py` & `codegrade-16.1.9/codegrade/models/auto_test_global_setup_output.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_global_setup_script.py` & `codegrade-16.1.9/codegrade/models/auto_test_global_setup_script.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_heartbeat_interval_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_heartbeat_interval_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_heartbeat_max_missed_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_heartbeat_max_missed_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_io_test_message_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_io_test_message_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_io_test_sub_message_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_io_test_sub_message_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_max_concurrent_batch_runs_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_max_concurrent_batch_runs_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_max_global_setup_time_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_max_global_setup_time_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_max_jobs_per_runner_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_max_jobs_per_runner_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_max_per_student_setup_time_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_max_per_student_setup_time_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_max_result_not_started_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_max_result_not_started_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_max_time_command_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_max_time_command_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_max_unit_test_metadata_length_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_max_unit_test_metadata_length_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_quality_comment.py` & `codegrade-16.1.9/codegrade/models/auto_test_quality_comment.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_result.py` & `codegrade-16.1.9/codegrade/models/auto_test_result.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_result_with_extra_data.py` & `codegrade-16.1.9/codegrade/models/auto_test_result_with_extra_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_run.py` & `codegrade-16.1.9/codegrade/models/auto_test_run.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_run_program_message_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_run_program_message_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_runner.py` & `codegrade-16.1.9/codegrade/models/auto_test_runner.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_set.py` & `codegrade-16.1.9/codegrade/models/auto_test_set.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_step_base.py` & `codegrade-16.1.9/codegrade/models/auto_test_step_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_step_base_as_json.py` & `codegrade-16.1.9/codegrade/models/auto_test_step_base_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_step_base_input_as_json.py` & `codegrade-16.1.9/codegrade/models/auto_test_step_base_input_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_step_log_base.py` & `codegrade-16.1.9/codegrade/models/auto_test_step_log_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_step_result.py` & `codegrade-16.1.9/codegrade/models/auto_test_step_result.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_step_validation_exception.py` & `codegrade-16.1.9/codegrade/models/auto_test_step_validation_exception.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_suite.py` & `codegrade-16.1.9/codegrade/models/auto_test_suite.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/auto_test_unit_test_message_setting.py` & `codegrade-16.1.9/codegrade/models/auto_test_unit_test_message_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/automatic_lti1p3_assignment_import_setting.py` & `codegrade-16.1.9/codegrade/models/automatic_lti1p3_assignment_import_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/automatic_lti_role_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/automatic_lti_role_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_about.py` & `codegrade-16.1.9/codegrade/models/base_about.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_auto_test_quality_comment.py` & `codegrade-16.1.9/codegrade/models/base_auto_test_quality_comment.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_comment_base.py` & `codegrade-16.1.9/codegrade/models/base_comment_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_comment_base_with_extended_replies.py` & `codegrade-16.1.9/codegrade/models/base_comment_base_with_extended_replies.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_comment_base_with_normal_replies.py` & `codegrade-16.1.9/codegrade/models/base_comment_base_with_normal_replies.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_comment_reply.py` & `codegrade-16.1.9/codegrade/models/base_comment_reply.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_coupon.py` & `codegrade-16.1.9/codegrade/models/base_coupon.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_directory.py` & `codegrade-16.1.9/codegrade/models/base_directory.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_error.py` & `codegrade-16.1.9/codegrade/models/base_error.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_file.py` & `codegrade-16.1.9/codegrade/models/base_file.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_lms_capabilities.py` & `codegrade-16.1.9/codegrade/models/base_lms_capabilities.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_lti1p1_provider.py` & `codegrade-16.1.9/codegrade/models/base_lti1p1_provider.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_lti1p3_provider.py` & `codegrade-16.1.9/codegrade/models/base_lti1p3_provider.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_lti_provider.py` & `codegrade-16.1.9/codegrade/models/base_lti_provider.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_notification.py` & `codegrade-16.1.9/codegrade/models/base_notification.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_release_info.py` & `codegrade-16.1.9/codegrade/models/base_release_info.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/base_rubric_item.py` & `codegrade-16.1.9/codegrade/models/base_rubric_item.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/blackboard_zip_upload_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/blackboard_zip_upload_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/bulk_enroll_course_data.py` & `codegrade-16.1.9/codegrade/models/bulk_enroll_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/canvas_course_id_copying_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/canvas_course_id_copying_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/change_user_role_course_data.py` & `codegrade-16.1.9/codegrade/models/change_user_role_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/check_points_as_json.py` & `codegrade-16.1.9/codegrade/models/check_points_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/check_points_data.py` & `codegrade-16.1.9/codegrade/models/check_points_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/check_points_extra.py` & `codegrade-16.1.9/codegrade/models/check_points_extra.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/check_points_input_as_json.py` & `codegrade-16.1.9/codegrade/models/check_points_input_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/clone_result.py` & `codegrade-16.1.9/codegrade/models/clone_result.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/code_quality_as_json.py` & `codegrade-16.1.9/codegrade/models/code_quality_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/code_quality_base_data.py` & `codegrade-16.1.9/codegrade/models/code_quality_base_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/code_quality_data.py` & `codegrade-16.1.9/codegrade/models/code_quality_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/code_quality_extra.py` & `codegrade-16.1.9/codegrade/models/code_quality_extra.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/code_quality_input_as_json.py` & `codegrade-16.1.9/codegrade/models/code_quality_input_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/code_quality_penalties.py` & `codegrade-16.1.9/codegrade/models/code_quality_penalties.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/column_range.py` & `codegrade-16.1.9/codegrade/models/column_range.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/comment_base.py` & `codegrade-16.1.9/codegrade/models/comment_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/comment_reply.py` & `codegrade-16.1.9/codegrade/models/comment_reply.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/comment_reply_edit.py` & `codegrade-16.1.9/codegrade/models/comment_reply_edit.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/connect_repository_git_provider_data.py` & `codegrade-16.1.9/codegrade/models/connect_repository_git_provider_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/copy_auto_test_data.py` & `codegrade-16.1.9/codegrade/models/copy_auto_test_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/copy_rubric_assignment_data.py` & `codegrade-16.1.9/codegrade/models/copy_rubric_assignment_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/coupon.py` & `codegrade-16.1.9/codegrade/models/coupon.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/coupon_data_parser.py` & `codegrade-16.1.9/codegrade/models/coupon_data_parser.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/coupon_usage.py` & `codegrade-16.1.9/codegrade/models/coupon_usage.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/coupon_with_code.py` & `codegrade-16.1.9/codegrade/models/coupon_with_code.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/coupon_without_code.py` & `codegrade-16.1.9/codegrade/models/coupon_without_code.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course.py` & `codegrade-16.1.9/codegrade/models/course.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_bulk_enroll_result.py` & `codegrade-16.1.9/codegrade/models/course_bulk_enroll_result.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_bulk_register_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/course_bulk_register_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_gradebook_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/course_gradebook_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_gradebook_render_warning_size_setting.py` & `codegrade-16.1.9/codegrade/models/course_gradebook_render_warning_size_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_of_course_price.py` & `codegrade-16.1.9/codegrade/models/course_of_course_price.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_perm_map.py` & `codegrade-16.1.9/codegrade/models/course_perm_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     #: course. Usually TAs and teachers have this permission, so they can
     #: change files in the CodeGra.de filesystem if code doesn't compile, for
     #: example.
     can_edit_others_work: "bool"
     #: Users with this permission can grade submissions.
     can_grade_work: "bool"
     #: Users with this permission can see the grade for a submission before an
-    #: assignment is set to "Done".
+    #: assignment's grades are published.
     can_see_grade_before_open: "bool"
     #: Users with this permission can see submissions of other users of this
     #: course.
     can_see_others_work: "bool"
     #: Users with this permission can view the assignments of this course.
     can_see_assignments: "bool"
     #: Users with this permission can view assignments of this course that are
-    #: set to "Hidden".
+    #: set to "Unavailable".
     can_see_hidden_assignments: "bool"
     #: Users with this permission can update the assignment info such as name,
     #: deadline and status.
     can_edit_assignment_info: "bool"
     #: Users with this permission can assign a grader to submissions of
     #: assignments.
     can_assign_graders: "bool"
@@ -135,36 +135,36 @@
     #: Users with this permission can create, delete, edit the fixtures of,
     #: setup scripts of, and test sets of an AutoTest
     can_edit_autotest: "bool"
     #: Users with this permission can view hidden AutoTest steps if they have
     #: the permission to view the summary of this step
     can_view_hidden_autotest_steps: "bool"
     #: Users with this permission can view AutoTest, such as sets, before the
-    #: state of the assignment is "Done"
+    #: state of the assignment's grades are published
     can_view_autotest_before_done: "bool"
     #: Users with this permission are allowed to see the details of non hidden
     #: AutoTest steps
     can_view_autotest_step_details: "bool"
     #: Users with this permission are allowed to see non hidden AutoTest
     #: fixtures
     can_view_autotest_fixture: "bool"
     #: Users with this permission can view output files created during an
-    #: AutoTest before the assignment state is "Done"
+    #: AutoTest before the assignment's grades are published
     can_view_autotest_output_files_before_done: "bool"
     #: Users with this permission can delete assignments within this course.
     can_delete_assignments: "bool"
     #: Users with this permission can create new submissions, even if the
     #: maximum number of submissions has been reached, or if a cool-off period
     #: is in effect.
     can_override_submission_limiting: "bool"
     #: Users with this permission can see the output of linters before an
-    #: assignment is set to "Done"
+    #: assignment's grades are published
     can_see_linter_feedback_before_done: "bool"
     #: Users with this permission can see all inline and general feedback,
-    #: except for peer feedback, before an assignment is set to "Done"
+    #: except for peer feedback, before an assignment's grades are published
     can_see_user_feedback_before_done: "bool"
     #: Users with this permission can view the analytics dashboard of an
     #: assignment.
     can_view_analytics: "bool"
     #: Users with this permission can edit inline and general comments authored
     #: by other users
     can_edit_others_comments: "bool"
@@ -206,15 +206,15 @@
     #: Users with this permission can edit general information of a course, for
     #: example the name.
     can_edit_course_info: "bool"
     #: Users with this permission can still create submissions after the lock
     #: date of an assignment.
     can_upload_after_lock_date: "bool"
     #: Users with this permission are allowed to see inline and general peer
-    #: feedback before the state of an assignment has been set to "Done".
+    #: feedback before the state of an assignment's grades are published.
     can_see_peer_feedback_before_done: "bool"
     #: Users with this permission can see the real name of students even when
     #: anonymized grading is enabled.
     can_see_anonymized_names: "bool"
     #: Users with this permission can view AutoTest results of other users they
     #: are peer reviewing.
     can_view_peer_review_autotest_results: "bool"
@@ -311,15 +311,15 @@
                 doc="Users with this permission can grade submissions.",
             ),
             rqa.RequiredArgument(
                 "can_see_grade_before_open",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Users with this permission can see the grade for a"
-                    ' submission before an assignment is set to "Done".'
+                    " submission before an assignment's grades are published."
                 ),
             ),
             rqa.RequiredArgument(
                 "can_see_others_work",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Users with this permission can see submissions of other"
@@ -335,15 +335,15 @@
                 ),
             ),
             rqa.RequiredArgument(
                 "can_see_hidden_assignments",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Users with this permission can view assignments of this"
-                    ' course that are set to "Hidden".'
+                    ' course that are set to "Unavailable".'
                 ),
             ),
             rqa.RequiredArgument(
                 "can_edit_assignment_info",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Users with this permission can update the assignment info"
@@ -615,15 +615,16 @@
                 ),
             ),
             rqa.RequiredArgument(
                 "can_view_autotest_before_done",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Users with this permission can view AutoTest, such as"
-                    ' sets, before the state of the assignment is "Done"'
+                    " sets, before the state of the assignment's grades are"
+                    " published"
                 ),
             ),
             rqa.RequiredArgument(
                 "can_view_autotest_step_details",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Users with this permission are allowed to see the details"
@@ -639,15 +640,16 @@
                 ),
             ),
             rqa.RequiredArgument(
                 "can_view_autotest_output_files_before_done",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Users with this permission can view output files created"
-                    ' during an AutoTest before the assignment state is "Done"'
+                    " during an AutoTest before the assignment's grades are"
+                    " published"
                 ),
             ),
             rqa.RequiredArgument(
                 "can_delete_assignments",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Users with this permission can delete assignments within"
@@ -664,24 +666,24 @@
                 ),
             ),
             rqa.RequiredArgument(
                 "can_see_linter_feedback_before_done",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Users with this permission can see the output of linters"
-                    ' before an assignment is set to "Done"'
+                    " before an assignment's grades are published"
                 ),
             ),
             rqa.RequiredArgument(
                 "can_see_user_feedback_before_done",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Users with this permission can see all inline and general"
-                    " feedback, except for peer feedback, before an assignment"
-                    ' is set to "Done"'
+                    " feedback, except for peer feedback, before an"
+                    " assignment's grades are published"
                 ),
             ),
             rqa.RequiredArgument(
                 "can_view_analytics",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Users with this permission can view the analytics"
@@ -804,16 +806,16 @@
                 ),
             ),
             rqa.RequiredArgument(
                 "can_see_peer_feedback_before_done",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Users with this permission are allowed to see inline and"
-                    " general peer feedback before the state of an assignment"
-                    ' has been set to "Done".'
+                    " general peer feedback before the state of an"
+                    " assignment's grades are published."
                 ),
             ),
             rqa.RequiredArgument(
                 "can_see_anonymized_names",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Users with this permission can see the real name of"
```

### Comparing `codegrade-16.1.8/codegrade/models/course_permission.py` & `codegrade-16.1.9/codegrade/models/course_permission.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_price.py` & `codegrade-16.1.9/codegrade/models/course_price.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_register_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/course_register_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_register_response.py` & `codegrade-16.1.9/codegrade/models/course_register_response.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_registration_link.py` & `codegrade-16.1.9/codegrade/models/course_registration_link.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_role.py` & `codegrade-16.1.9/codegrade/models/course_role.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_role_as_json_with_perms.py` & `codegrade-16.1.9/codegrade/models/course_role_as_json_with_perms.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_section.py` & `codegrade-16.1.9/codegrade/models/course_section.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_section_division.py` & `codegrade-16.1.9/codegrade/models/course_section_division.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_section_division_connection.py` & `codegrade-16.1.9/codegrade/models/course_section_division_connection.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_section_division_user.py` & `codegrade-16.1.9/codegrade/models/course_section_division_user.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_snippet.py` & `codegrade-16.1.9/codegrade/models/course_snippet.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/course_statistics_as_json.py` & `codegrade-16.1.9/codegrade/models/course_statistics_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_assignment_course_data.py` & `codegrade-16.1.9/codegrade/models/create_assignment_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_auto_test_data.py` & `codegrade-16.1.9/codegrade/models/create_auto_test_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_comment_data.py` & `codegrade-16.1.9/codegrade/models/create_comment_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_comment_reply_data.py` & `codegrade-16.1.9/codegrade/models/create_comment_reply_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_course_data.py` & `codegrade-16.1.9/codegrade/models/create_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_division_section_data.py` & `codegrade-16.1.9/codegrade/models/create_division_section_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_group_group_set_data.py` & `codegrade-16.1.9/codegrade/models/create_group_group_set_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_group_set_course_data.py` & `codegrade-16.1.9/codegrade/models/create_group_set_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_lti_data.py` & `codegrade-16.1.9/codegrade/models/create_lti_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_output_html_proxy_auto_test_data.py` & `codegrade-16.1.9/codegrade/models/create_output_html_proxy_auto_test_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_proxy_submission_data.py` & `codegrade-16.1.9/codegrade/models/create_proxy_submission_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_repository_git_provider_data.py` & `codegrade-16.1.9/codegrade/models/create_repository_git_provider_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_role_course_data.py` & `codegrade-16.1.9/codegrade/models/create_role_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_section_course_data.py` & `codegrade-16.1.9/codegrade/models/create_section_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_snippet_course_data.py` & `codegrade-16.1.9/codegrade/models/create_snippet_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_snippet_data.py` & `codegrade-16.1.9/codegrade/models/create_snippet_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_sso_provider_data.py` & `codegrade-16.1.9/codegrade/models/create_sso_provider_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/create_tenant_data.py` & `codegrade-16.1.9/codegrade/models/create_tenant_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/csv_large_file_limit_setting.py` & `codegrade-16.1.9/codegrade/models/csv_large_file_limit_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/csv_too_many_errors_limit_setting.py` & `codegrade-16.1.9/codegrade/models/csv_too_many_errors_limit_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/custom_output_as_json.py` & `codegrade-16.1.9/codegrade/models/custom_output_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/custom_output_data.py` & `codegrade-16.1.9/codegrade/models/custom_output_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/custom_output_extra.py` & `codegrade-16.1.9/codegrade/models/custom_output_extra.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/custom_output_input_as_json.py` & `codegrade-16.1.9/codegrade/models/custom_output_input_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/custom_output_log.py` & `codegrade-16.1.9/codegrade/models/custom_output_log.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/custom_output_log_base.py` & `codegrade-16.1.9/codegrade/models/custom_output_log_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/deleted_comment_reply.py` & `codegrade-16.1.9/codegrade/models/deleted_comment_reply.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/directory_with_children.py` & `codegrade-16.1.9/codegrade/models/directory_with_children.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/disabled_setting_exception.py` & `codegrade-16.1.9/codegrade/models/disabled_setting_exception.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/editor_enabled_for_teachers_setting.py` & `codegrade-16.1.9/codegrade/models/editor_enabled_for_teachers_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/editor_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/editor_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/email_students_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/email_students_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/email_users_course_data.py` & `codegrade-16.1.9/codegrade/models/email_users_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/exam_login_max_length_setting.py` & `codegrade-16.1.9/codegrade/models/exam_login_max_length_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/export_assignment_csv_data.py` & `codegrade-16.1.9/codegrade/models/export_assignment_csv_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/export_assignment_data.py` & `codegrade-16.1.9/codegrade/models/export_assignment_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/export_assignment_files_data.py` & `codegrade-16.1.9/codegrade/models/export_assignment_files_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extended_auto_test_result.py` & `codegrade-16.1.9/codegrade/models/extended_auto_test_result.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extended_auto_test_run.py` & `codegrade-16.1.9/codegrade/models/extended_auto_test_run.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extended_course.py` & `codegrade-16.1.9/codegrade/models/extended_course.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extended_course_registration_link.py` & `codegrade-16.1.9/codegrade/models/extended_course_registration_link.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extended_course_section.py` & `codegrade-16.1.9/codegrade/models/extended_course_section.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extended_group.py` & `codegrade-16.1.9/codegrade/models/extended_group.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extended_job.py` & `codegrade-16.1.9/codegrade/models/extended_job.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extended_non_deleted_comment_reply.py` & `codegrade-16.1.9/codegrade/models/extended_non_deleted_comment_reply.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extended_tenant.py` & `codegrade-16.1.9/codegrade/models/extended_tenant.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extended_transaction.py` & `codegrade-16.1.9/codegrade/models/extended_transaction.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extended_user.py` & `codegrade-16.1.9/codegrade/models/extended_user.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extended_work.py` & `codegrade-16.1.9/codegrade/models/extended_work.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extract_file_tree_directory.py` & `codegrade-16.1.9/codegrade/models/extract_file_tree_directory.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/extract_file_tree_file.py` & `codegrade-16.1.9/codegrade/models/extract_file_tree_file.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/failed_to_send_email_exception.py` & `codegrade-16.1.9/codegrade/models/failed_to_send_email_exception.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/feedback_base.py` & `codegrade-16.1.9/codegrade/models/feedback_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/feedback_threads_initially_collapsed_setting.py` & `codegrade-16.1.9/codegrade/models/feedback_threads_initially_collapsed_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/feedback_with_replies.py` & `codegrade-16.1.9/codegrade/models/feedback_with_replies.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/feedback_without_replies.py` & `codegrade-16.1.9/codegrade/models/feedback_without_replies.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/file_deletion.py` & `codegrade-16.1.9/codegrade/models/file_deletion.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/file_rule.py` & `codegrade-16.1.9/codegrade/models/file_rule.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/file_rule_input_data.py` & `codegrade-16.1.9/codegrade/models/file_rule_input_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/file_tree.py` & `codegrade-16.1.9/codegrade/models/file_tree.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/finalized_lti1p1_provider.py` & `codegrade-16.1.9/codegrade/models/finalized_lti1p1_provider.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/finalized_lti1p3_provider.py` & `codegrade-16.1.9/codegrade/models/finalized_lti1p3_provider.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/find_element_interval_setting.py` & `codegrade-16.1.9/codegrade/models/find_element_interval_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/find_element_max_tries_setting.py` & `codegrade-16.1.9/codegrade/models/find_element_max_tries_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/first_phase_lti_launch_exception.py` & `codegrade-16.1.9/codegrade/models/first_phase_lti_launch_exception.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/fixture_like.py` & `codegrade-16.1.9/codegrade/models/fixture_like.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/fraction.py` & `codegrade-16.1.9/codegrade/models/fraction.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/frontend_site_settings.py` & `codegrade-16.1.9/codegrade/models/frontend_site_settings.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/general_feedback_comment_base.py` & `codegrade-16.1.9/codegrade/models/general_feedback_comment_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/general_feedback_comment_base_with_extended_replies.py` & `codegrade-16.1.9/codegrade/models/general_feedback_comment_base_with_extended_replies.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/general_feedback_extra.py` & `codegrade-16.1.9/codegrade/models/general_feedback_extra.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/git_repositories_page.py` & `codegrade-16.1.9/codegrade/models/git_repositories_page.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/git_repository_like.py` & `codegrade-16.1.9/codegrade/models/git_repository_like.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/git_user_info.py` & `codegrade-16.1.9/codegrade/models/git_user_info.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/global_perm_map.py` & `codegrade-16.1.9/codegrade/models/global_perm_map.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/global_permission.py` & `codegrade-16.1.9/codegrade/models/global_permission.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/grade_history.py` & `codegrade-16.1.9/codegrade/models/grade_history.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/grading_notifications_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/grading_notifications_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/group.py` & `codegrade-16.1.9/codegrade/models/group.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/group_not_ready_for_submission_exception.py` & `codegrade-16.1.9/codegrade/models/group_not_ready_for_submission_exception.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/group_set.py` & `codegrade-16.1.9/codegrade/models/group_set.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/groups_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/groups_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/has_unread_notifcation_json.py` & `codegrade-16.1.9/codegrade/models/has_unread_notifcation_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/health_information.py` & `codegrade-16.1.9/codegrade/models/health_information.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/ignored_files_exception.py` & `codegrade-16.1.9/codegrade/models/ignored_files_exception.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/import_into_assignment_data.py` & `codegrade-16.1.9/codegrade/models/import_into_assignment_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/import_into_course_data.py` & `codegrade-16.1.9/codegrade/models/import_into_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/incremental_rubric_submission_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/incremental_rubric_submission_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/inline_feedback_comment_base.py` & `codegrade-16.1.9/codegrade/models/inline_feedback_comment_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/inline_feedback_comment_base_with_extended_replies.py` & `codegrade-16.1.9/codegrade/models/inline_feedback_comment_base_with_extended_replies.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/inline_feedback_extra.py` & `codegrade-16.1.9/codegrade/models/inline_feedback_extra.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/invalid_group_exception.py` & `codegrade-16.1.9/codegrade/models/invalid_group_exception.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/invalid_io_cases_exception.py` & `codegrade-16.1.9/codegrade/models/invalid_io_cases_exception.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/invalid_options_exception.py` & `codegrade-16.1.9/codegrade/models/invalid_options_exception.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/io_test_as_json.py` & `codegrade-16.1.9/codegrade/models/io_test_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/io_test_base_data.py` & `codegrade-16.1.9/codegrade/models/io_test_base_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/io_test_data.py` & `codegrade-16.1.9/codegrade/models/io_test_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/io_test_extra.py` & `codegrade-16.1.9/codegrade/models/io_test_extra.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/io_test_input_as_json.py` & `codegrade-16.1.9/codegrade/models/io_test_input_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/io_test_input_case.py` & `codegrade-16.1.9/codegrade/models/io_test_input_case.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/io_test_log.py` & `codegrade-16.1.9/codegrade/models/io_test_log.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/io_test_step_log.py` & `codegrade-16.1.9/codegrade/models/io_test_step_log.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/io_test_step_log_base.py` & `codegrade-16.1.9/codegrade/models/io_test_step_log_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/is_admin_permission_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/is_admin_permission_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/job.py` & `codegrade-16.1.9/codegrade/models/job.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/json_create_auto_test.py` & `codegrade-16.1.9/codegrade/models/json_create_auto_test.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/json_create_tenant.py` & `codegrade-16.1.9/codegrade/models/json_create_tenant.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/json_patch_auto_test.py` & `codegrade-16.1.9/codegrade/models/json_patch_auto_test.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/json_patch_submit_types_assignment.py` & `codegrade-16.1.9/codegrade/models/json_patch_submit_types_assignment.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/junit_test_as_json.py` & `codegrade-16.1.9/codegrade/models/junit_test_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/junit_test_base_data.py` & `codegrade-16.1.9/codegrade/models/junit_test_base_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/junit_test_data.py` & `codegrade-16.1.9/codegrade/models/junit_test_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/junit_test_extra.py` & `codegrade-16.1.9/codegrade/models/junit_test_extra.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/junit_test_input_as_json.py` & `codegrade-16.1.9/codegrade/models/junit_test_input_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/junit_test_log.py` & `codegrade-16.1.9/codegrade/models/junit_test_log.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/junit_test_log_base.py` & `codegrade-16.1.9/codegrade/models/junit_test_log_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/jwt_access_token_expires_setting.py` & `codegrade-16.1.9/codegrade/models/jwt_access_token_expires_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/legacy_features.py` & `codegrade-16.1.9/codegrade/models/legacy_features.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/line_range.py` & `codegrade-16.1.9/codegrade/models/line_range.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/linter_comment.py` & `codegrade-16.1.9/codegrade/models/linter_comment.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/linters_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/linters_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/lms_capabilities.py` & `codegrade-16.1.9/codegrade/models/lms_capabilities.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/login_token_before_time_setting.py` & `codegrade-16.1.9/codegrade/models/login_token_before_time_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/login_user_data.py` & `codegrade-16.1.9/codegrade/models/login_user_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/lti1p1_provider.py` & `codegrade-16.1.9/codegrade/models/lti1p1_provider.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/lti1p1_provider_data.py` & `codegrade-16.1.9/codegrade/models/lti1p1_provider_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/lti1p3_provider.py` & `codegrade-16.1.9/codegrade/models/lti1p3_provider.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/lti1p3_provider_data.py` & `codegrade-16.1.9/codegrade/models/lti1p3_provider_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/lti1p3_provider_presentation_as_json.py` & `codegrade-16.1.9/codegrade/models/lti1p3_provider_presentation_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/lti_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/lti_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/lti_lock_date_copying_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/lti_lock_date_copying_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/lti_provider_base.py` & `codegrade-16.1.9/codegrade/models/lti_provider_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/max_document_update_size_setting.py` & `codegrade-16.1.9/codegrade/models/max_document_update_size_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/max_dynamo_file_size_setting.py` & `codegrade-16.1.9/codegrade/models/max_dynamo_file_size_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/max_dynamo_submission_size_setting.py` & `codegrade-16.1.9/codegrade/models/max_dynamo_submission_size_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/max_file_size_setting.py` & `codegrade-16.1.9/codegrade/models/max_file_size_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/max_large_upload_size_setting.py` & `codegrade-16.1.9/codegrade/models/max_large_upload_size_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/max_lines_setting.py` & `codegrade-16.1.9/codegrade/models/max_lines_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/max_mirror_file_age_setting.py` & `codegrade-16.1.9/codegrade/models/max_mirror_file_age_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/max_normal_upload_size_setting.py` & `codegrade-16.1.9/codegrade/models/max_normal_upload_size_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/max_number_of_files_setting.py` & `codegrade-16.1.9/codegrade/models/max_number_of_files_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/max_plagiarism_matches_setting.py` & `codegrade-16.1.9/codegrade/models/max_plagiarism_matches_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/max_user_setting_amount_setting.py` & `codegrade-16.1.9/codegrade/models/max_user_setting_amount_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/metric_evaluation_time_chunk_size_setting.py` & `codegrade-16.1.9/codegrade/models/metric_evaluation_time_chunk_size_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/metric_evaluation_time_limit_setting.py` & `codegrade-16.1.9/codegrade/models/metric_evaluation_time_limit_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/metric_event_buffer_size_setting.py` & `codegrade-16.1.9/codegrade/models/metric_event_buffer_size_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/metric_gathering_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/metric_gathering_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/metric_gathering_event_interval_setting.py` & `codegrade-16.1.9/codegrade/models/metric_gathering_event_interval_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/metric_gathering_expressions_setting.py` & `codegrade-16.1.9/codegrade/models/metric_gathering_expressions_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/metric_gathering_time_interval_setting.py` & `codegrade-16.1.9/codegrade/models/metric_gathering_time_interval_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/min_password_score_setting.py` & `codegrade-16.1.9/codegrade/models/min_password_score_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/mirror_file_result.py` & `codegrade-16.1.9/codegrade/models/mirror_file_result.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/missing_cookie_error.py` & `codegrade-16.1.9/codegrade/models/missing_cookie_error.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/missing_file.py` & `codegrade-16.1.9/codegrade/models/missing_file.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/new_auto_test_allowed_initial_build_ids_setting.py` & `codegrade-16.1.9/codegrade/models/new_auto_test_allowed_initial_build_ids_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/new_auto_test_build_max_command_time_setting.py` & `codegrade-16.1.9/codegrade/models/new_auto_test_build_max_command_time_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/new_auto_test_build_output_limit_setting.py` & `codegrade-16.1.9/codegrade/models/new_auto_test_build_output_limit_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/new_auto_test_copying_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/new_auto_test_copying_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/new_auto_test_current_initial_build_ids_setting.py` & `codegrade-16.1.9/codegrade/models/new_auto_test_current_initial_build_ids_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/new_auto_test_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/new_auto_test_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/new_auto_test_initial_build_id_setting.py` & `codegrade-16.1.9/codegrade/models/new_auto_test_initial_build_id_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/new_auto_test_max_dynamodb_size_setting.py` & `codegrade-16.1.9/codegrade/models/new_auto_test_max_dynamodb_size_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/new_auto_test_max_file_size_setting.py` & `codegrade-16.1.9/codegrade/models/new_auto_test_max_file_size_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/new_auto_test_max_storage_size_setting.py` & `codegrade-16.1.9/codegrade/models/new_auto_test_max_storage_size_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/new_auto_test_old_submission_age_setting.py` & `codegrade-16.1.9/codegrade/models/new_auto_test_old_submission_age_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/new_auto_test_test_max_command_time_setting.py` & `codegrade-16.1.9/codegrade/models/new_auto_test_test_max_command_time_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/new_auto_test_test_output_limit_setting.py` & `codegrade-16.1.9/codegrade/models/new_auto_test_test_output_limit_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/no_permissions.py` & `codegrade-16.1.9/codegrade/models/no_permissions.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/non_deleted_comment_reply.py` & `codegrade-16.1.9/codegrade/models/non_deleted_comment_reply.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/non_finalized_lti1p1_provider.py` & `codegrade-16.1.9/codegrade/models/non_finalized_lti1p1_provider.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/non_finalized_lti1p3_provider.py` & `codegrade-16.1.9/codegrade/models/non_finalized_lti1p3_provider.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/non_present_preference.py` & `codegrade-16.1.9/codegrade/models/non_present_preference.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/notification.py` & `codegrade-16.1.9/codegrade/models/notification.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/notification_comment_reply_notification_as_json.py` & `codegrade-16.1.9/codegrade/models/notification_comment_reply_notification_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/notification_general_feedback_reply_notification_as_json.py` & `codegrade-16.1.9/codegrade/models/notification_general_feedback_reply_notification_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/notification_poll_time_setting.py` & `codegrade-16.1.9/codegrade/models/notification_poll_time_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/notification_setting.py` & `codegrade-16.1.9/codegrade/models/notification_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/notification_setting_option.py` & `codegrade-16.1.9/codegrade/models/notification_setting_option.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/notifications_json.py` & `codegrade-16.1.9/codegrade/models/notifications_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/oauth_provider.py` & `codegrade-16.1.9/codegrade/models/oauth_provider.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/oauth_token.py` & `codegrade-16.1.9/codegrade/models/oauth_token.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/option.py` & `codegrade-16.1.9/codegrade/models/option.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/options_input_data.py` & `codegrade-16.1.9/codegrade/models/options_input_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/parse_api_exception.py` & `codegrade-16.1.9/codegrade/models/parse_api_exception.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/partial_all_site_settings.py` & `codegrade-16.1.9/codegrade/models/partial_all_site_settings.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch1_p1_provider_lti_data.py` & `codegrade-16.1.9/codegrade/models/patch1_p1_provider_lti_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch1_p3_provider_lti_data.py` & `codegrade-16.1.9/codegrade/models/patch1_p3_provider_lti_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_all_notification_data.py` & `codegrade-16.1.9/codegrade/models/patch_all_notification_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_assignment_data.py` & `codegrade-16.1.9/codegrade/models/patch_assignment_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,39 +17,44 @@
 from .assignment_done_type import AssignmentDoneType
 from .assignment_kind import AssignmentKind
 from .assignment_percentage_grading_settings import (
     AssignmentPercentageGradingSettings,
 )
 from .assignment_points_grading_settings import AssignmentPointsGradingSettings
 from .assignment_state_enum import AssignmentStateEnum
+from .fixed_availability import FixedAvailability
+from .fixed_grade_availability import FixedGradeAvailability
 from .submission_validator_input_data import SubmissionValidatorInputData
+from .timed_availability import TimedAvailability
 
 
 @dataclass
 class PatchAssignmentData:
     """Input data required for the `Assignment::Patch` operation."""
 
-    #: The new state of the assignment
+    #: The new state of the assignment. Deprecated, use the "availability" and
+    #: "grade\_availability" options, will be removed in Q3 2023.
     state: Maybe["AssignmentStateEnum"] = Nothing
     #: The new name of the assignment
     name: Maybe["str"] = Nothing
     #: The new deadline of the assignment
     deadline: Maybe["datetime.datetime"] = Nothing
     #: The new lock date of the assignment
     lock_date: Maybe["t.Optional[datetime.datetime]"] = Nothing
     #: The maximum possible grade for this assignment. You can reset this by
     #: passing `null` as value
     max_grade: Maybe["t.Optional[float]"] = Nothing
     #: The group set id for this assignment. Set to `null` to make this
     #: assignment not a group assignment
     group_set_id: Maybe["t.Optional[int]"] = Nothing
-    #: The time the assignment should become available
+    #: The time the assignment should become available. Deprecated, use the
+    #: "availability" option, will be removed in Q3 2023.
     available_at: Maybe["t.Optional[datetime.datetime]"] = Nothing
     #: Should we send login links to students before the assignment opens. This
-    #: is only available for assignments with 'kind' equal to 'exam'
+    #: is only available for assignments with 'kind' equal to 'exam'.
     send_login_links: Maybe["bool"] = Nothing
     #: The new kind of assignment
     kind: Maybe["AssignmentKind"] = Nothing
     #: Should students be allowed to make submissions by uploading files
     files_upload_enabled: Maybe["bool"] = Nothing
     #: Should students be allowed to make submissions using git webhooks
     webhook_upload_enabled: Maybe["bool"] = Nothing
@@ -84,23 +89,33 @@
     #: The file we should load first in an asignment
     file_to_load_first: Maybe["t.Optional[str]"] = Nothing
     #: Grading settings of this assignment.
     grading: Maybe[
         "t.Union[AssignmentPointsGradingSettings,"
         " AssignmentPercentageGradingSettings]"
     ] = Nothing
+    #: The availability of this assignment.
+    availability: Maybe[
+        "t.Union[FixedAvailability, TimedAvailability]"
+    ] = Nothing
+    #: The grade availability of this assignment.
+    grade_availability: Maybe["FixedGradeAvailability"] = Nothing
 
     raw_data: t.Optional[t.Dict[str, t.Any]] = field(init=False, repr=False)
 
     data_parser: t.ClassVar = rqa.Lazy(
         lambda: rqa.FixedMapping(
             rqa.OptionalArgument(
                 "state",
                 rqa.EnumValue(AssignmentStateEnum),
-                doc="The new state of the assignment",
+                doc=(
+                    "The new state of the assignment. Deprecated, use the"
+                    ' "availability" and "grade\\_availability" options, will'
+                    " be removed in Q3 2023."
+                ),
             ),
             rqa.OptionalArgument(
                 "name",
                 rqa.SimpleValue.str,
                 doc="The new name of the assignment",
             ),
             rqa.OptionalArgument(
@@ -128,23 +143,27 @@
                     "The group set id for this assignment. Set to `null` to"
                     " make this assignment not a group assignment"
                 ),
             ),
             rqa.OptionalArgument(
                 "available_at",
                 rqa.Nullable(rqa.RichValue.DateTime),
-                doc="The time the assignment should become available",
+                doc=(
+                    "The time the assignment should become available."
+                    ' Deprecated, use the "availability" option, will be'
+                    " removed in Q3 2023."
+                ),
             ),
             rqa.OptionalArgument(
                 "send_login_links",
                 rqa.SimpleValue.bool,
                 doc=(
                     "Should we send login links to students before the"
                     " assignment opens. This is only available for assignments"
-                    " with 'kind' equal to 'exam'"
+                    " with 'kind' equal to 'exam'."
                 ),
             ),
             rqa.OptionalArgument(
                 "kind",
                 rqa.EnumValue(AssignmentKind),
                 doc="The new kind of assignment",
             ),
@@ -250,14 +269,27 @@
                     parsers.ParserFor.make(AssignmentPointsGradingSettings),
                     parsers.ParserFor.make(
                         AssignmentPercentageGradingSettings
                     ),
                 ),
                 doc="Grading settings of this assignment.",
             ),
+            rqa.OptionalArgument(
+                "availability",
+                parsers.make_union(
+                    parsers.ParserFor.make(FixedAvailability),
+                    parsers.ParserFor.make(TimedAvailability),
+                ),
+                doc="The availability of this assignment.",
+            ),
+            rqa.OptionalArgument(
+                "grade_availability",
+                parsers.ParserFor.make(FixedGradeAvailability),
+                doc="The grade availability of this assignment.",
+            ),
         ).use_readable_describe(True)
     )
 
     def __post_init__(self) -> None:
         getattr(super(), "__post_init__", lambda: None)()
         self.state = maybe_from_nullable(self.state)
         self.name = maybe_from_nullable(self.name)
@@ -283,14 +315,16 @@
         self.ignore_version = maybe_from_nullable(self.ignore_version)
         self.done_type = maybe_from_nullable(self.done_type)
         self.reminder_time = maybe_from_nullable(self.reminder_time)
         self.done_email = maybe_from_nullable(self.done_email)
         self.anonymized_grading = maybe_from_nullable(self.anonymized_grading)
         self.file_to_load_first = maybe_from_nullable(self.file_to_load_first)
         self.grading = maybe_from_nullable(self.grading)
+        self.availability = maybe_from_nullable(self.availability)
+        self.grade_availability = maybe_from_nullable(self.grade_availability)
 
     def to_dict(self) -> t.Dict[str, t.Any]:
         res: t.Dict[str, t.Any] = {}
         if self.state.is_just:
             res["state"] = to_dict(self.state.value)
         if self.name.is_just:
             res["name"] = to_dict(self.name.value)
@@ -336,14 +370,18 @@
             res["done_email"] = to_dict(self.done_email.value)
         if self.anonymized_grading.is_just:
             res["anonymized_grading"] = to_dict(self.anonymized_grading.value)
         if self.file_to_load_first.is_just:
             res["file_to_load_first"] = to_dict(self.file_to_load_first.value)
         if self.grading.is_just:
             res["grading"] = to_dict(self.grading.value)
+        if self.availability.is_just:
+            res["availability"] = to_dict(self.availability.value)
+        if self.grade_availability.is_just:
+            res["grade_availability"] = to_dict(self.grade_availability.value)
         return res
 
     @classmethod
     def from_dict(
         cls: t.Type["PatchAssignmentData"], d: t.Dict[str, t.Any]
     ) -> "PatchAssignmentData":
         parsed = cls.data_parser.try_parse(d)
@@ -367,10 +405,12 @@
             ignore_version=parsed.ignore_version,
             done_type=parsed.done_type,
             reminder_time=parsed.reminder_time,
             done_email=parsed.done_email,
             anonymized_grading=parsed.anonymized_grading,
             file_to_load_first=parsed.file_to_load_first,
             grading=parsed.grading,
+            availability=parsed.availability,
+            grade_availability=parsed.grade_availability,
         )
         res.raw_data = d
         return res
```

### Comparing `codegrade-16.1.8/codegrade/models/patch_auto_test_data.py` & `codegrade-16.1.9/codegrade/models/patch_auto_test_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_comment_reply_data.py` & `codegrade-16.1.9/codegrade/models/patch_comment_reply_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_course_data.py` & `codegrade-16.1.9/codegrade/models/patch_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_grader_submission_data.py` & `codegrade-16.1.9/codegrade/models/patch_grader_submission_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_notification_data.py` & `codegrade-16.1.9/codegrade/models/patch_notification_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_notification_setting_user_setting_data.py` & `codegrade-16.1.9/codegrade/models/patch_notification_setting_user_setting_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_provider_lti_data.py` & `codegrade-16.1.9/codegrade/models/patch_provider_lti_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_role_course_data.py` & `codegrade-16.1.9/codegrade/models/patch_role_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_role_data.py` & `codegrade-16.1.9/codegrade/models/patch_role_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_role_tenant_data.py` & `codegrade-16.1.9/codegrade/models/patch_role_tenant_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_rubric_category_type_assignment_data.py` & `codegrade-16.1.9/codegrade/models/patch_rubric_category_type_assignment_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_rubric_result_submission_data.py` & `codegrade-16.1.9/codegrade/models/patch_rubric_result_submission_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_section_data.py` & `codegrade-16.1.9/codegrade/models/patch_section_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_settings_tenant_data.py` & `codegrade-16.1.9/codegrade/models/patch_settings_tenant_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_site_settings_data.py` & `codegrade-16.1.9/codegrade/models/patch_site_settings_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_snippet_course_data.py` & `codegrade-16.1.9/codegrade/models/patch_snippet_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_snippet_data.py` & `codegrade-16.1.9/codegrade/models/patch_snippet_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_submission_data.py` & `codegrade-16.1.9/codegrade/models/patch_submission_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_submit_types_assignment_data.py` & `codegrade-16.1.9/codegrade/models/patch_submit_types_assignment_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_tenant_data.py` & `codegrade-16.1.9/codegrade/models/patch_tenant_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_ui_preference_user_setting_data.py` & `codegrade-16.1.9/codegrade/models/patch_ui_preference_user_setting_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/patch_user_data.py` & `codegrade-16.1.9/codegrade/models/patch_user_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/pay_with_coupon_course_price_data.py` & `codegrade-16.1.9/codegrade/models/pay_with_coupon_course_price_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/peer_feedback_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/peer_feedback_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/permission_exception.py` & `codegrade-16.1.9/codegrade/models/permission_exception.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/plagiarism_run.py` & `codegrade-16.1.9/codegrade/models/plagiarism_run.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/plagiarism_run_plagiarism_assignment_as_json.py` & `codegrade-16.1.9/codegrade/models/plagiarism_run_plagiarism_assignment_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/plagiarism_run_plagiarism_course_as_json.py` & `codegrade-16.1.9/codegrade/models/plagiarism_run_plagiarism_course_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/post_oauth_token_data.py` & `codegrade-16.1.9/codegrade/models/post_oauth_token_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/present_preference.py` & `codegrade-16.1.9/codegrade/models/present_preference.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/proxy.py` & `codegrade-16.1.9/codegrade/models/proxy.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/put_description_assignment_data.py` & `codegrade-16.1.9/codegrade/models/put_description_assignment_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/put_enroll_link_course_data.py` & `codegrade-16.1.9/codegrade/models/put_enroll_link_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/put_price_course_data.py` & `codegrade-16.1.9/codegrade/models/put_price_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/put_price_tenant_data.py` & `codegrade-16.1.9/codegrade/models/put_price_tenant_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/put_rubric_assignment_data.py` & `codegrade-16.1.9/codegrade/models/put_rubric_assignment_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/quality_test_log.py` & `codegrade-16.1.9/codegrade/models/quality_test_log.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/quality_test_log_base.py` & `codegrade-16.1.9/codegrade/models/quality_test_log_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/register_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/register_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/register_user_data.py` & `codegrade-16.1.9/codegrade/models/register_user_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/register_user_with_link_course_data.py` & `codegrade-16.1.9/codegrade/models/register_user_with_link_course_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/release_info.py` & `codegrade-16.1.9/codegrade/models/release_info.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/release_message_max_time_setting.py` & `codegrade-16.1.9/codegrade/models/release_message_max_time_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/rename_group_group_data.py` & `codegrade-16.1.9/codegrade/models/rename_group_group_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/render_html_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/render_html_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/reset_token_time_setting.py` & `codegrade-16.1.9/codegrade/models/reset_token_time_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/result_data_get_auto_test_get.py` & `codegrade-16.1.9/codegrade/models/result_data_get_auto_test_get.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/result_data_get_task_result_get_all.py` & `codegrade-16.1.9/codegrade/models/result_data_get_task_result_get_all.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/result_data_post_login_link_login.py` & `codegrade-16.1.9/codegrade/models/result_data_post_login_link_login.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/result_data_post_section_create_division.py` & `codegrade-16.1.9/codegrade/models/result_data_post_section_create_division.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/result_data_post_user_login.py` & `codegrade-16.1.9/codegrade/models/result_data_post_user_login.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/result_data_post_user_register.py` & `codegrade-16.1.9/codegrade/models/result_data_post_user_register.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/role_as_json_with_perms.py` & `codegrade-16.1.9/codegrade/models/role_as_json_with_perms.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/root_file_trees_json.py` & `codegrade-16.1.9/codegrade/models/root_file_trees_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/rubric_enabled_for_teacher_on_submissions_page_setting.py` & `codegrade-16.1.9/codegrade/models/rubric_enabled_for_teacher_on_submissions_page_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/rubric_item.py` & `codegrade-16.1.9/codegrade/models/rubric_item.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/rubric_item_input_as_json.py` & `codegrade-16.1.9/codegrade/models/rubric_item_input_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/rubric_row_base.py` & `codegrade-16.1.9/codegrade/models/rubric_row_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/rubric_row_base_input_as_json.py` & `codegrade-16.1.9/codegrade/models/rubric_row_base_input_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/rubric_row_base_input_base_as_json.py` & `codegrade-16.1.9/codegrade/models/rubric_row_base_input_base_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/rubrics_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/rubrics_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/run_program_as_json.py` & `codegrade-16.1.9/codegrade/models/run_program_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/run_program_data.py` & `codegrade-16.1.9/codegrade/models/run_program_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/run_program_extra.py` & `codegrade-16.1.9/codegrade/models/run_program_extra.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/run_program_input_as_json.py` & `codegrade-16.1.9/codegrade/models/run_program_input_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/run_program_log.py` & `codegrade-16.1.9/codegrade/models/run_program_log.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/saml2_provider_json.py` & `codegrade-16.1.9/codegrade/models/saml2_provider_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/saml_ui_info.py` & `codegrade-16.1.9/codegrade/models/saml_ui_info.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/send_registration_email_setting.py` & `codegrade-16.1.9/codegrade/models/send_registration_email_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/server_time_correction_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/server_time_correction_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/server_time_diff_tolerance_setting.py` & `codegrade-16.1.9/codegrade/models/server_time_diff_tolerance_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/server_time_sync_interval_setting.py` & `codegrade-16.1.9/codegrade/models/server_time_sync_interval_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/setting_token_time_setting.py` & `codegrade-16.1.9/codegrade/models/setting_token_time_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/setup_oauth_result.py` & `codegrade-16.1.9/codegrade/models/setup_oauth_result.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/site_email_setting.py` & `codegrade-16.1.9/codegrade/models/site_email_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/site_setting_input.py` & `codegrade-16.1.9/codegrade/models/site_setting_input.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/snippet.py` & `codegrade-16.1.9/codegrade/models/snippet.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/sso_username_decollision_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/sso_username_decollision_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/start_payment_course_price_close_tab_data.py` & `codegrade-16.1.9/codegrade/models/start_payment_course_price_close_tab_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/start_payment_course_price_data.py` & `codegrade-16.1.9/codegrade/models/start_payment_course_price_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/start_payment_course_price_redirect_data.py` & `codegrade-16.1.9/codegrade/models/start_payment_course_price_redirect_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/started_transaction.py` & `codegrade-16.1.9/codegrade/models/started_transaction.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/student_payment_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/student_payment_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/submission_validator_input_data.py` & `codegrade-16.1.9/codegrade/models/submission_validator_input_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/tenant.py` & `codegrade-16.1.9/codegrade/models/tenant.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/tenant_course_statistics.py` & `codegrade-16.1.9/codegrade/models/tenant_course_statistics.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/tenant_of_tenant_price.py` & `codegrade-16.1.9/codegrade/models/tenant_of_tenant_price.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/tenant_permissions.py` & `codegrade-16.1.9/codegrade/models/tenant_permissions.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/tenant_price.py` & `codegrade-16.1.9/codegrade/models/tenant_price.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/tenant_role_as_json_with_perms.py` & `codegrade-16.1.9/codegrade/models/tenant_role_as_json_with_perms.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/tenant_statistics.py` & `codegrade-16.1.9/codegrade/models/tenant_statistics.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/test_submission_copying_on_import_enabled_setting.py` & `codegrade-16.1.9/codegrade/models/test_submission_copying_on_import_enabled_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/tour_configurations_setting.py` & `codegrade-16.1.9/codegrade/models/tour_configurations_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/tour_polling_interval_setting.py` & `codegrade-16.1.9/codegrade/models/tour_polling_interval_setting.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/transaction.py` & `codegrade-16.1.9/codegrade/models/transaction.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/types.py` & `codegrade-16.1.9/codegrade/models/types.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/update_peer_feedback_settings_assignment_data.py` & `codegrade-16.1.9/codegrade/models/update_peer_feedback_settings_assignment_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/update_set_auto_test_data.py` & `codegrade-16.1.9/codegrade/models/update_set_auto_test_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/update_suite_auto_test_base_data.py` & `codegrade-16.1.9/codegrade/models/update_suite_auto_test_base_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/update_suite_auto_test_data.py` & `codegrade-16.1.9/codegrade/models/update_suite_auto_test_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/upgraded_lti_provider_exception.py` & `codegrade-16.1.9/codegrade/models/upgraded_lti_provider_exception.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/upload_submission_assignment_data.py` & `codegrade-16.1.9/codegrade/models/upload_submission_assignment_data.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/user.py` & `codegrade-16.1.9/codegrade/models/user.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/user_course.py` & `codegrade-16.1.9/codegrade/models/user_course.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/user_info_with_role.py` & `codegrade-16.1.9/codegrade/models/user_info_with_role.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/user_input.py` & `codegrade-16.1.9/codegrade/models/user_input.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/user_without_group.py` & `codegrade-16.1.9/codegrade/models/user_without_group.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/weak_password_exception.py` & `codegrade-16.1.9/codegrade/models/weak_password_exception.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/weak_password_feedback.py` & `codegrade-16.1.9/codegrade/models/weak_password_feedback.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/webhook_base.py` & `codegrade-16.1.9/codegrade/models/webhook_base.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/work.py` & `codegrade-16.1.9/codegrade/models/work.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/work_rubric_item.py` & `codegrade-16.1.9/codegrade/models/work_rubric_item.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/work_rubric_result_as_json.py` & `codegrade-16.1.9/codegrade/models/work_rubric_result_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/models/work_rubric_result_points_as_json.py` & `codegrade-16.1.9/codegrade/models/work_rubric_result_points_as_json.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/parsers.py` & `codegrade-16.1.9/codegrade/parsers.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/codegrade/utils.py` & `codegrade-16.1.9/codegrade/utils.py`

 * *Files identical despite different names*

### Comparing `codegrade-16.1.8/pyproject.toml` & `codegrade-16.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "codegrade"
-version = "16.1.8"
+version = "16.1.9"
 description = "A client library for accessing CodeGrade"
 license = "AGPL-3.0-only OR BSD-3-Clause-Clear"
 
 authors = []
 
 readme = "README.md"
 packages = [
```

### Comparing `codegrade-16.1.8/setup.py` & `codegrade-16.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'validate-email>=1.3,<2.0']
 
 extras_require = \
 {':python_version >= "3.6" and python_version < "3.7"': ['dataclasses>=0.8,<0.9']}
 
 setup_kwargs = {
     'name': 'codegrade',
-    'version': '16.1.8',
+    'version': '16.1.9',
     'description': 'A client library for accessing CodeGrade',
     'long_description': '# CodeGrade API\n\nThis library makes it easier to use the CodeGrade API. Its API allows you to\nautomate your usage of CodeGrade. We are currently still busy documenting the\nentire API, but everything that is possible in the UI of CodeGrade is also\npossible through the API.\n## Installation\nYou can install the library through [pypi](https://pypi.org/), simply run\n`python3 -m pip install codegrade`. If you want to get a dev version with support\nfor the latest features, simply email [support@codegrade.com](mailto:support@codegrade.com)\nand we\'ll provide you with a dev version.\n## Usage\nFirst, create a client:\n\n```python\nimport codegrade\n\n# Don\'t store your password in your code!\nwith codegrade.login(\n    username=\'my-username\',\n    password=os.getenv(\'CG_PASSWORD\'),\n    tenant=\'My University\',\n) as client:\n    pass\n\n# Or supply information interactively.\nwith codegrade.login_from_cli() as client:\n    pass\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom codegrade.models import PatchCourseData\n\ncourses = client.course.get_all()\nfor course in courses:\n    client.course.patch(\n        PatchCourseData(name=course.name + \' (NEW)\'),\n        course_id=course.id,\n    )\n\n# Or, simply use dictionaries.\nfor course in courses:\n    client.course.patch(\n        {"name": course.name + \' (NEW)\'},\n        course_id=course.id,\n    )\n```\n\nFor the complete documentation go to\nhttps://python.api.codegrade.com.\n## Backwards compatibility\nCodeGrade is constantly upgrading its API, but we try to minimize backwards\nincompatible changes. We\'ll announce every backwards incompatible change in the\n[changelog](http://codegrade.com/changelog). A new version of the API\nclient is released with every release of CodeGrade, which is approximately every\nmonth. To upgrade simply run `pip install --upgrade codegrade`.\n## Supported python versions\nWe support python 3.6 and above, `pypy` is currently not tested but should work\njust fine.\n## License\nThe library is licensed under AGPL-3.0-only or BSD-3-Clause-Clear.',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `codegrade-16.1.8/PKG-INFO` & `codegrade-16.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codegrade
-Version: 16.1.8
+Version: 16.1.9
 Summary: A client library for accessing CodeGrade
 License: AGPL-3.0-only OR BSD-3-Clause-Clear
 Requires-Python: >=3.6.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

