# Comparing `tmp/songtradr-api-client-python-0.0.1.tar.gz` & `tmp/songtradr-api-client-python-1.12.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "songtradr-api-client-python-0.0.1.tar", last modified: Wed Jun 14 12:51:49 2023, max compression
+gzip compressed data, was "songtradr-api-client-python-1.12.21.tar", last modified: Wed Jun 14 15:38:31 2023, max compression
```

## Comparing `songtradr-api-client-python-0.0.1.tar` & `songtradr-api-client-python-1.12.21.tar`

### file list

```diff
@@ -1,416 +1,163 @@
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.896669 songtradr-api-client-python-0.0.1/
--rw-r--r--   0 darylfindlay   (501) staff       (20)     1950 2023-06-14 12:51:49.896746 songtradr-api-client-python-0.0.1/PKG-INFO
--rw-r--r--   0 darylfindlay   (501) staff       (20)    26123 2023-06-14 11:03:50.000000 songtradr-api-client-python-0.0.1/README.md
--rw-r--r--   0 darylfindlay   (501) staff       (20)       69 2023-06-14 12:51:49.897013 songtradr-api-client-python-0.0.1/setup.cfg
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4436 2023-06-14 11:03:50.000000 songtradr-api-client-python-0.0.1/setup.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.819710 songtradr-api-client-python-0.0.1/songtradr_api_client_python/
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2505 2023-06-14 11:03:50.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    60202 2023-06-14 11:03:50.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/api_client.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.821510 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      214 2023-06-14 11:03:50.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     8977 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/path_to_api.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.831981 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      254 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      148 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_allowed_values_genre.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      169 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_allowed_values_musical_features.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      144 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_allowed_values_tag.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      120 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_party.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      220 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_playlist.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      180 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_playlist_songtradr_playlist_guid.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      180 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_public_recording_ids_musical_features.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      173 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_public_recording_ids_similarities.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      165 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_public_recording_ids_taggrams.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      173 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_public_recording_ids_tagstrengths.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      151 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_public_recording_l_ids.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      151 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_public_recording_m_ids.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      151 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_public_recording_s_ids.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      154 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_public_recording_search.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      174 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_public_recording_search_granular.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      197 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_public_recording_search_granular_abstraction.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      161 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_file_name_init_upload.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      365 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_file_object_key.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      129 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_files.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      146 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_files_download.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      142 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_files_status.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      144 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_files_summary.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      170 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_folder_folder_name_taggrams.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      178 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_folder_folder_name_tagstrengths.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      133 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_folders.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      151 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_forgot_password.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      132 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_login.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      216 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_me.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      147 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_referrers_new.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      154 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_referrers_username.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      147 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_save_playlist.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      135 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_sign_up.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      132 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_token.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      151 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/paths/api_v1_user_update_password.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      975 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/tag_to_api.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.833396 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/tags/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      429 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/tags/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2394 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/tags/allowed_values_api.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2138 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/tags/party_api.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2404 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/tags/playlist_api.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     3529 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/tags/recording_api.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4398 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/tags/user_api.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    17447 2023-06-14 11:03:50.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/configuration.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     6164 2023-06-14 11:03:50.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/exceptions.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.849809 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      361 2023-06-14 11:03:50.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     6024 2023-06-14 11:03:21.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/category_medium_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4261 2023-06-14 11:03:22.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/category_minimal_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5852 2023-06-14 11:03:22.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/config_access_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4950 2023-06-14 11:03:22.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/config_identifier_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4251 2023-06-14 11:03:22.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/contributor_type_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     6238 2023-06-14 11:03:22.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/error_response.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5287 2023-06-14 11:03:22.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/field_summary_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    16576 2023-06-14 11:03:23.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/file_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     6944 2023-06-14 11:03:23.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/file_list_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5219 2023-06-14 11:03:23.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/file_minimal_with_url_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    15428 2023-06-14 11:03:23.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/file_small_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     8009 2023-06-14 11:03:23.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/file_upload_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4721 2023-06-14 11:03:23.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/file_w_ith_url_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    11669 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/files_summary_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5338 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/forgot_password_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4568 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/genre_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4194 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/genre_minimal_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5181 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/genres_summary_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5151 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/init_put_recording_audio_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5421 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/jwt_token_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5746 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/login_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)   140583 2023-06-14 11:03:25.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/musical_features_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4617 2023-06-14 11:03:25.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/p_line_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     8043 2023-06-14 11:03:25.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/party_large_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4653 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/party_small_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    12041 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/playlist_large_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    11422 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/product_medium_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5930 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/product_party_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4894 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/recording_for_similarity_search_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5458 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/recording_genre_prediction_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    16567 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/recording_large_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     7154 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/recording_list_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    14651 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/recording_medium_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5832 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/recording_minimal_with_musical_features_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     7081 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/recording_minimal_with_taggrams_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5755 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/recording_minimal_with_tagstrengths_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5926 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/recording_party_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     6128 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/recording_playlist_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     7694 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/recording_small_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4182 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/recording_tag_small_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)   273700 2023-06-14 11:03:28.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/save_file_recording_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    10983 2023-06-14 11:03:29.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/save_playlist_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5331 2023-06-14 11:03:29.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/save_recording_genre_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5634 2023-06-14 11:03:29.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/save_recording_party_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5532 2023-06-14 11:03:29.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/save_recording_playlist_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4771 2023-06-14 11:03:29.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/save_recording_tag_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4624 2023-06-14 11:03:29.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/save_referrer_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    93867 2023-06-14 11:03:30.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/save_taggrams_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     8038 2023-06-14 11:03:32.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/save_user_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    62113 2023-06-14 11:03:32.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/search_filter_values_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    13757 2023-06-14 11:03:33.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/search_recording_granular_abstraction_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4736 2023-06-14 11:03:33.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/search_recording_granular_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5910 2023-06-14 11:03:33.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/sign_up_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     6112 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/tag_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4589 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/tag_small_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     8061 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/taggram_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     6189 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/tags_summary_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     7204 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/tagstrength_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4189 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/title_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4204 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/token_request.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5368 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/track_to_medium_product_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4642 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/update_password_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     4094 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/usage_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    16400 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/user_dto.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.850023 songtradr-api-client-python-0.0.1/songtradr_api_client_python/models/
--rw-r--r--   0 darylfindlay   (501) staff       (20)     5772 2023-06-14 11:03:50.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/models/__init__.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.850340 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2636 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/__init__.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.850775 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_allowed_values_genre/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      367 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_allowed_values_genre/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    12397 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_allowed_values_genre/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.851218 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_allowed_values_musical_features/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      389 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_allowed_values_musical_features/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    12021 2023-06-14 11:03:35.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_allowed_values_musical_features/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.851859 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_allowed_values_tag/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      363 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_allowed_values_tag/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    14225 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_allowed_values_tag/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.852375 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_party/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      337 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_party/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    11513 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_party/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.853059 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_playlist/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      343 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_playlist/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    13606 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_playlist/get.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    14370 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_playlist/post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.853801 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_playlist_songtradr_playlist_guid/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      391 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_playlist_songtradr_playlist_guid/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    11482 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_playlist_songtradr_playlist_guid/delete.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.854484 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_ids_musical_features/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      401 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_ids_musical_features/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    12461 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_ids_musical_features/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.855221 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_ids_similarities/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      393 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_ids_similarities/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    12351 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_ids_similarities/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.855760 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_ids_taggrams/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      385 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_ids_taggrams/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    19615 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_ids_taggrams/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.856249 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_ids_tagstrengths/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      393 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_ids_tagstrengths/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    19028 2023-06-14 11:03:38.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_ids_tagstrengths/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.856716 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_l_ids/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      371 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_l_ids/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    12116 2023-06-14 11:03:38.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_l_ids/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.857260 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_m_ids/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      371 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_m_ids/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    15384 2023-06-14 11:03:38.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_m_ids/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.857796 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_s_ids/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      371 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_s_ids/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    12116 2023-06-14 11:03:38.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_s_ids/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.858254 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_search/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      373 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_search/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    48927 2023-06-14 11:03:38.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_search/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.858636 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_search_granular/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      391 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_search_granular/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    14867 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_search_granular/post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.859140 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_search_granular_abstraction/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      415 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_search_granular_abstraction/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    15148 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_public_recording_search_granular_abstraction/post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.859788 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_file_name_init_upload/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      379 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_file_name_init_upload/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    18843 2023-06-14 11:03:41.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_file_name_init_upload/post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.860873 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_file_object_key/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      367 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_file_object_key/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    11402 2023-06-14 11:03:40.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_file_object_key/delete.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    11895 2023-06-14 11:03:43.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_file_object_key/get.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    16624 2023-06-14 11:03:43.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_file_object_key/post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.861487 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_files/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      347 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_files/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    70443 2023-06-14 11:03:44.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_files/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.861939 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_files_download/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      365 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_files_download/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    65356 2023-06-14 11:03:45.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_files_download/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.862338 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_files_status/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      361 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_files_status/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    12772 2023-06-14 11:03:45.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_files_status/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.862878 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_files_summary/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      363 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_files_summary/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    69036 2023-06-14 11:03:46.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_files_summary/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.863371 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_folder_folder_name_taggrams/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      391 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_folder_folder_name_taggrams/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    21069 2023-06-14 11:03:41.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_folder_folder_name_taggrams/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.864051 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_folder_folder_name_tagstrengths/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      399 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_folder_folder_name_tagstrengths/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    20492 2023-06-14 11:03:41.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_folder_folder_name_tagstrengths/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.864549 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_folders/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      351 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_folders/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    13239 2023-06-14 11:03:46.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_folders/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.865028 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_forgot_password/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      366 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_forgot_password/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    13770 2023-06-14 11:03:41.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_forgot_password/post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.865560 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_login/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      347 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_login/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    13623 2023-06-14 11:03:41.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_login/post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.866268 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_me/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      341 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_me/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     9258 2023-06-14 11:03:41.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_me/get.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    13601 2023-06-14 11:03:40.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_me/post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.866757 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_referrers_new/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      363 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_referrers_new/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    13747 2023-06-14 11:03:40.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_referrers_new/post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.867226 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_referrers_username/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      373 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_referrers_username/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    11857 2023-06-14 11:03:46.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_referrers_username/get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.867612 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_save_playlist/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      363 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_save_playlist/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    71946 2023-06-14 11:03:42.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_save_playlist/post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.868398 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_sign_up/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      350 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_sign_up/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    14696 2023-06-14 11:03:43.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_sign_up/post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.868950 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_token/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      347 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_token/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    13663 2023-06-14 11:03:43.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_token/post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.869541 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_update_password/
--rw-r--r--   0 darylfindlay   (501) staff       (20)      366 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_update_password/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    13792 2023-06-14 11:03:43.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/paths/api_v1_user_update_password/post.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    12330 2023-06-14 11:03:50.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/rest.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)    99326 2023-06-14 11:03:50.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python/schemas.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.820715 songtradr-api-client-python-0.0.1/songtradr_api_client_python.egg-info/
--rw-r--r--   0 darylfindlay   (501) staff       (20)     1950 2023-06-14 12:51:49.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python.egg-info/PKG-INFO
--rw-r--r--   0 darylfindlay   (501) staff       (20)    19966 2023-06-14 12:51:49.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 darylfindlay   (501) staff       (20)        1 2023-06-14 12:51:49.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 darylfindlay   (501) staff       (20)      118 2023-06-14 12:51:49.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python.egg-info/requires.txt
--rw-r--r--   0 darylfindlay   (501) staff       (20)       33 2023-06-14 12:51:49.000000 songtradr-api-client-python-0.0.1/songtradr_api_client_python.egg-info/top_level.txt
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.813591 songtradr-api-client-python-0.0.1/test/
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.883477 songtradr-api-client-python-0.0.1/test/test_models/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:50.000000 songtradr-api-client-python-0.0.1/test/test_models/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2264 2023-06-14 11:03:22.000000 songtradr-api-client-python-0.0.1/test/test_models/test_category_medium_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2268 2023-06-14 11:03:22.000000 songtradr-api-client-python-0.0.1/test/test_models/test_category_minimal_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2256 2023-06-14 11:03:22.000000 songtradr-api-client-python-0.0.1/test/test_models/test_config_access_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2272 2023-06-14 11:03:22.000000 songtradr-api-client-python-0.0.1/test/test_models/test_config_identifier_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2268 2023-06-14 11:03:22.000000 songtradr-api-client-python-0.0.1/test/test_models/test_contributor_type_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2247 2023-06-14 11:03:22.000000 songtradr-api-client-python-0.0.1/test/test_models/test_error_response.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2256 2023-06-14 11:03:22.000000 songtradr-api-client-python-0.0.1/test/test_models/test_field_summary_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2223 2023-06-14 11:03:23.000000 songtradr-api-client-python-0.0.1/test/test_models/test_file_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2240 2023-06-14 11:03:23.000000 songtradr-api-client-python-0.0.1/test/test_models/test_file_list_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2282 2023-06-14 11:03:23.000000 songtradr-api-client-python-0.0.1/test/test_models/test_file_minimal_with_url_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2244 2023-06-14 11:03:23.000000 songtradr-api-client-python-0.0.1/test/test_models/test_file_small_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2248 2023-06-14 11:03:23.000000 songtradr-api-client-python-0.0.1/test/test_models/test_file_upload_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2254 2023-06-14 11:03:23.000000 songtradr-api-client-python-0.0.1/test/test_models/test_file_w_ith_url_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2256 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/test/test_models/test_files_summary_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2264 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/test/test_models/test_forgot_password_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2227 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/test/test_models/test_genre_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2256 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/test/test_models/test_genre_minimal_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2260 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/test/test_models/test_genres_summary_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2294 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/test/test_models/test_init_put_recording_audio_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2240 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/test/test_models/test_jwt_token_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2227 2023-06-14 11:03:24.000000 songtradr-api-client-python-0.0.1/test/test_models/test_login_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2268 2023-06-14 11:03:25.000000 songtradr-api-client-python-0.0.1/test/test_models/test_musical_features_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2228 2023-06-14 11:03:25.000000 songtradr-api-client-python-0.0.1/test/test_models/test_p_line_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2248 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/test/test_models/test_party_large_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2248 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/test/test_models/test_party_small_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2260 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/test/test_models/test_playlist_large_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2260 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/test/test_models/test_product_medium_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2256 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/test/test_models/test_product_party_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2322 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/test/test_models/test_recording_for_similarity_search_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2305 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/test/test_models/test_recording_genre_prediction_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2264 2023-06-14 11:03:26.000000 songtradr-api-client-python-0.0.1/test/test_models/test_recording_large_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2260 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/test/test_models/test_recording_list_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2268 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/test/test_models/test_recording_medium_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2351 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/test/test_models/test_recording_minimal_with_musical_features_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2322 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/test/test_models/test_recording_minimal_with_taggrams_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2338 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/test/test_models/test_recording_minimal_with_tagstrengths_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2264 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/test/test_models/test_recording_party_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2276 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/test/test_models/test_recording_playlist_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2264 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/test/test_models/test_recording_small_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2277 2023-06-14 11:03:27.000000 songtradr-api-client-python-0.0.1/test/test_models/test_recording_tag_small_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2277 2023-06-14 11:03:28.000000 songtradr-api-client-python-0.0.1/test/test_models/test_save_file_recording_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2256 2023-06-14 11:03:29.000000 songtradr-api-client-python-0.0.1/test/test_models/test_save_playlist_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2281 2023-06-14 11:03:29.000000 songtradr-api-client-python-0.0.1/test/test_models/test_save_recording_genre_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2281 2023-06-14 11:03:29.000000 songtradr-api-client-python-0.0.1/test/test_models/test_save_recording_party_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2293 2023-06-14 11:03:29.000000 songtradr-api-client-python-0.0.1/test/test_models/test_save_recording_playlist_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2273 2023-06-14 11:03:29.000000 songtradr-api-client-python-0.0.1/test/test_models/test_save_recording_tag_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2256 2023-06-14 11:03:29.000000 songtradr-api-client-python-0.0.1/test/test_models/test_save_referrer_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2256 2023-06-14 11:03:31.000000 songtradr-api-client-python-0.0.1/test/test_models/test_save_taggrams_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2240 2023-06-14 11:03:32.000000 songtradr-api-client-python-0.0.1/test/test_models/test_save_user_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2281 2023-06-14 11:03:33.000000 songtradr-api-client-python-0.0.1/test/test_models/test_search_filter_values_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2346 2023-06-14 11:03:33.000000 songtradr-api-client-python-0.0.1/test/test_models/test_search_recording_granular_abstraction_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2301 2023-06-14 11:03:33.000000 songtradr-api-client-python-0.0.1/test/test_models/test_search_recording_granular_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2232 2023-06-14 11:03:33.000000 songtradr-api-client-python-0.0.1/test/test_models/test_sign_up_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2219 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/test/test_models/test_tag_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2240 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/test/test_models/test_tag_small_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2235 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/test/test_models/test_taggram_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2252 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/test/test_models/test_tags_summary_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2251 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/test/test_models/test_tagstrength_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2227 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/test/test_models/test_title_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2243 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/test/test_models/test_token_request.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2290 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/test/test_models/test_track_to_medium_product_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2264 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/test/test_models/test_update_password_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2227 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/test/test_models/test_usage_dto.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     2223 2023-06-14 11:03:34.000000 songtradr-api-client-python-0.0.1/test/test_models/test_user_dto.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.883642 songtradr-api-client-python-0.0.1/test/test_paths/
--rw-r--r--   0 darylfindlay   (501) staff       (20)     1995 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/__init__.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.884072 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_allowed_values_genre/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_allowed_values_genre/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      898 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_allowed_values_genre/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.884367 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_allowed_values_musical_features/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_allowed_values_musical_features/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      988 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_allowed_values_musical_features/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.884725 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_allowed_values_tag/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_allowed_values_tag/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      912 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_allowed_values_tag/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.885101 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_party/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_party/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      873 2023-06-14 11:03:36.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_party/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.885663 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_playlist/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_playlist/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      854 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_playlist/test_get.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      870 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_playlist/test_post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.885971 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_playlist_songtradr_playlist_guid/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_playlist_songtradr_playlist_guid/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      931 2023-06-14 11:03:37.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_playlist_songtradr_playlist_guid/test_delete.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.886254 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_ids_musical_features/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_ids_musical_features/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      980 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_ids_musical_features/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.886723 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_ids_similarities/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_ids_similarities/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      953 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_ids_similarities/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.887213 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_ids_taggrams/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_ids_taggrams/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      982 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_ids_taggrams/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.887574 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_ids_tagstrengths/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_ids_tagstrengths/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     1013 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_ids_tagstrengths/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.887916 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_l_ids/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_l_ids/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      916 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_l_ids/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.888333 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_m_ids/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_m_ids/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      923 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_m_ids/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.888643 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_s_ids/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_s_ids/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      916 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_s_ids/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.888957 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_search/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_search/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      942 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_search/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.889269 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_search_granular/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_search_granular/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      949 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_search_granular/test_post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.889675 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_search_granular_abstraction/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_search_granular_abstraction/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     1007 2023-06-14 11:03:39.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_public_recording_search_granular_abstraction/test_post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.890015 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_file_name_init_upload/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_file_name_init_upload/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      967 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_file_name_init_upload/test_post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.891036 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_file_object_key/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_file_object_key/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      891 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_file_object_key/test_delete.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      909 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_file_object_key/test_get.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      914 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_file_object_key/test_post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.891359 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_files/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_files/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      875 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_files/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.891657 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_files_download/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_files_download/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      898 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_files_download/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.891990 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_files_status/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_files_status/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      888 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_files_status/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.892327 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_files_summary/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_files_summary/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      888 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_files_summary/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.892636 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_folder_folder_name_taggrams/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_folder_folder_name_taggrams/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      994 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_folder_folder_name_taggrams/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.892911 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_folder_folder_name_tagstrengths/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_folder_folder_name_tagstrengths/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)     1035 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_folder_folder_name_tagstrengths/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.893208 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_folders/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_folders/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      862 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_folders/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.893493 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_forgot_password/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_forgot_password/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      904 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_forgot_password/test_post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.893798 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_login/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_login/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      882 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_login/test_post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.894317 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_me/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_me/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      863 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_me/test_get.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      873 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_me/test_post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.894636 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_referrers_new/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_referrers_new/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      848 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_referrers_new/test_post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.894934 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_referrers_username/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_referrers_username/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      858 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_referrers_username/test_get.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.895287 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_save_playlist/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_save_playlist/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      920 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_save_playlist/test_post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.895666 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_sign_up/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_sign_up/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      872 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_sign_up/test_post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.896044 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_token/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_token/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      902 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_token/test_post.py
-drwxr-xr-x   0 darylfindlay   (501) staff       (20)        0 2023-06-14 12:51:49.896445 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_update_password/
--rw-r--r--   0 darylfindlay   (501) staff       (20)        0 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_update_password/__init__.py
--rw-r--r--   0 darylfindlay   (501) staff       (20)      926 2023-06-14 11:03:47.000000 songtradr-api-client-python-0.0.1/test/test_paths/test_api_v1_user_update_password/test_post.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:31.069454 songtradr-api-client-python-1.12.21/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-14 15:38:31.069454 songtradr-api-client-python-1.12.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13996 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 15:38:31.069454 songtradr-api-client-python-1.12.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:31.021454 songtradr-api-client-python-1.12.21/songtradr_api_client_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:31.025454 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21722 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/allowed_values_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/party_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24331 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/playlist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96081 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/recording_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   255960 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31745 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6964 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:31.045454 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     7422 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/category_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/category_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/config_access_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/config_identifier_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/contributor_type_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/field_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_minimal_with_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_upload_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_w_ith_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/files_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/forgot_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/genre_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/genres_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/init_put_recording_audio_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/jwt_token_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/login_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41920 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/p_line_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/party_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/party_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/playlist_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/product_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/product_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4150 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_for_similarity_search_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_genre_prediction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_minimal_with_musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_minimal_with_tagstrengths_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66338 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_file_recording_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_recording_genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_recording_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_recording_tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_referrer_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/search_filter_values_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/search_recording_granular_abstraction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/search_recording_granular_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/sign_up_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/taggram_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/tags_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/tagstrength_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/title_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/track_to_medium_product_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/update_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/usage_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14547 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:31.025454 songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-14 15:38:31.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-06-14 15:38:31.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:38:31.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 15:38:31.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 15:38:31.000000 songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:38:31.069454 songtradr-api-client-python-1.12.21/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_allowed_values_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_category_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_category_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_config_access_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_config_identifier_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_contributor_type_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_field_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11762 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_file_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22975 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_file_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_file_minimal_with_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_file_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_file_upload_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21599 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_file_w_ith_url_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_files_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_forgot_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_genre_minimal_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_genres_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_init_put_recording_audio_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_jwt_token_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_login_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_p_line_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/test/test_party_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_party_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_party_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/test/test_playlist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_playlist_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_product_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_product_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/test/test_recording_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_for_similarity_search_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_genre_prediction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_large_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19341 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_list_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_medium_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_minimal_with_musical_features_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_minimal_with_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_minimal_with_tagstrengths_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10757 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_recording_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14624 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_file_recording_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_recording_genre_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_recording_party_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_recording_playlist_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_recording_tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_referrer_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_taggrams_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_save_user_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_search_filter_values_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_search_recording_granular_abstraction_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_search_recording_granular_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_sign_up_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_tag_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_tag_small_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_taggram_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_tags_summary_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_tagstrength_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_title_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_track_to_medium_product_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_update_password_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_usage_dto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-06-14 15:38:18.000000 songtradr-api-client-python-1.12.21/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-14 15:38:17.000000 songtradr-api-client-python-1.12.21/test/test_user_dto.py
```

### Comparing `songtradr-api-client-python-0.0.1/PKG-INFO` & `songtradr-api-client-python-1.12.21/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: songtradr-api-client-python
-Version: 0.0.1
+Version: 1.12.21
 Summary: Songtradr API
-Home-page: 
+Home-page: https://pypi.org/project/songtradr-api-client-python/
 Author: Songtradr Inc.
 Author-email: info@songtradr.com
 Keywords: OpenAPI,OpenAPI-Generator,Songtradr API
-Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 
-    This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world&#x27;s released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
+    This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world&#39;s released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
```

### Comparing `songtradr-api-client-python-0.0.1/setup.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_minimal_with_taggrams_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,46 +3,81 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from setuptools import setup, find_packages  # noqa: H301
 
-NAME = "songtradr-api-client-python"
-VERSION = "0.0.1"
-# To install the library, run the following
-#
-# python setup.py install
-#
-# prerequisite: setuptools
-# http://pypi.python.org/pypi/setuptools
-
-REQUIRES = [
-    "certifi >= 14.5.14",
-    "frozendict ~= 2.3.4",
-    "python-dateutil ~= 2.7.0",
-    "setuptools >= 21.0.0",
-    "typing_extensions ~= 4.3.0",
-    "urllib3 ~= 1.26.7",
-]
-
-setup(
-    name=NAME,
-    version=VERSION,
-    description="Songtradr API",
-    author="Songtradr Inc.",
-    author_email="info@songtradr.com",
-    url="",
-    keywords=["OpenAPI", "OpenAPI-Generator", "Songtradr API"],
-    python_requires=">=3.7",
-    install_requires=REQUIRES,
-    packages=find_packages(exclude=["test", "tests"]),
-    include_package_data=True,
-    long_description="""\
-    This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world&#x27;s released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
+
+
+from typing import List, Optional, Union
+from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist
+from songtradr_api_client_python.models.taggram_dto import TaggramDTO
+
+class RecordingMinimalWithTaggramsDTO(BaseModel):
+    """
+    Recording in its minimal form, but with AI-predicted musical features.
     """
-)
+    isrc: StrictStr = Field(...)
+    timestamps: Optional[conlist(Union[StrictFloat, StrictInt])] = Field(None, description="Points in time in seconds. Each value refers to the taggrams values of the same index.")
+    taggrams: Optional[conlist(TaggramDTO)] = None
+    __properties = ["isrc", "timestamps", "taggrams"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> RecordingMinimalWithTaggramsDTO:
+        """Create an instance of RecordingMinimalWithTaggramsDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in taggrams (list)
+        _items = []
+        if self.taggrams:
+            for _item in self.taggrams:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['taggrams'] = _items
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> RecordingMinimalWithTaggramsDTO:
+        """Create an instance of RecordingMinimalWithTaggramsDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return RecordingMinimalWithTaggramsDTO.parse_obj(obj)
+
+        _obj = RecordingMinimalWithTaggramsDTO.parse_obj({
+            "isrc": obj.get("isrc"),
+            "timestamps": obj.get("timestamps"),
+            "taggrams": [TaggramDTO.from_dict(_item) for _item in obj.get("taggrams")] if obj.get("taggrams") is not None else None
+        })
+        return _obj
+
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/__init__.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-# coding: utf-8
+Metadata-Version: 2.1
+Name: songtradr-api-client-python
+Version: 1.12.21
+Summary: Songtradr API
+Home-page: https://pypi.org/project/songtradr-api-client-python/
+Author: Songtradr Inc.
+Author-email: info@songtradr.com
+Keywords: OpenAPI,OpenAPI-Generator,Songtradr API
+Description-Content-Type: text/markdown
 
-# flake8: noqa
-
-"""
-    Songtradr API
-
-    This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
-
-    The version of the OpenAPI document: 1.12.21
-    Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-__version__ = "0.0.1"
-
-# import ApiClient
-from songtradr_api_client_python.api_client import ApiClient
-
-# import Configuration
-from songtradr_api_client_python.configuration import Configuration
-
-# import exceptions
-from songtradr_api_client_python.exceptions import OpenApiException
-from songtradr_api_client_python.exceptions import ApiAttributeError
-from songtradr_api_client_python.exceptions import ApiTypeError
-from songtradr_api_client_python.exceptions import ApiValueError
-from songtradr_api_client_python.exceptions import ApiKeyError
-from songtradr_api_client_python.exceptions import ApiException
+    This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world&#39;s released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
+
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/tags/allowed_values_api.py` & `songtradr-api-client-python-1.12.21/test/test_usage_dto.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,26 +3,53 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from songtradr_api_client_python.paths.api_v1_allowed_values_musical_features.get import AllowedMusicalFeatures
-from songtradr_api_client_python.paths.api_v1_allowed_values_genre.get import Genres
-from songtradr_api_client_python.paths.api_v1_allowed_values_tag.get import Tags
 
+import unittest
+import datetime
 
-class AllowedValuesApi(
-    AllowedMusicalFeatures,
-    Genres,
-    Tags,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import songtradr_api_client_python
+from songtradr_api_client_python.models.usage_dto import UsageDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
+
+class TestUsageDTO(unittest.TestCase):
+    """UsageDTO unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test UsageDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `UsageDTO`
+        """
+        model = songtradr_api_client_python.models.usage_dto.UsageDTO()  # noqa: E501
+        if include_optional :
+            return UsageDTO(
+                name = ''
+            )
+        else :
+            return UsageDTO(
+        )
+        """
+
+    def testUsageDTO(self):
+        """Test UsageDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
-    Do not edit the class manually.
-    """
-    pass
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/tags/party_api.py` & `songtradr-api-client-python-1.12.21/test/test_party_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,22 +3,39 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from songtradr_api_client_python.paths.api_v1_party.get import Party
 
+import unittest
 
-class PartyApi(
-    Party,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import songtradr_api_client_python
+from songtradr_api_client_python.api.party_api import PartyApi  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
-    Do not edit the class manually.
-    """
-    pass
+
+class TestPartyApi(unittest.TestCase):
+    """PartyApi unit test stubs"""
+
+    def setUp(self):
+        self.api = songtradr_api_client_python.api.party_api.PartyApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_party(self):
+        """Test case for party
+
+        Information on a person, group or company.  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/tags/playlist_api.py` & `songtradr-api-client-python-1.12.21/test/test_playlist_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,53 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from songtradr_api_client_python.paths.api_v1_playlist.get import AllPlaylists
-from songtradr_api_client_python.paths.api_v1_playlist.post import CreateOrUpdatePlaylist
-from songtradr_api_client_python.paths.api_v1_playlist_songtradr_playlist_guid.delete import DeletePlaylist
 
+import unittest
 
-class PlaylistApi(
-    AllPlaylists,
-    CreateOrUpdatePlaylist,
-    DeletePlaylist,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
+import songtradr_api_client_python
+from songtradr_api_client_python.api.playlist_api import PlaylistApi  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
-    Do not edit the class manually.
-    """
-    pass
+
+class TestPlaylistApi(unittest.TestCase):
+    """PlaylistApi unit test stubs"""
+
+    def setUp(self):
+        self.api = songtradr_api_client_python.api.playlist_api.PlaylistApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_all_playlists(self):
+        """Test case for all_playlists
+
+        All playlists.  # noqa: E501
+        """
+        pass
+
+    def test_create_or_update_playlist(self):
+        """Test case for create_or_update_playlist
+
+        Create and edit playlist.  # noqa: E501
+        """
+        pass
+
+    def test_delete_playlist(self):
+        """Test case for delete_playlist
+
+        Delete playlist.  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/apis/tags/recording_api.py` & `songtradr-api-client-python-1.12.21/test/test_tagstrength_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,40 +3,61 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-from songtradr_api_client_python.paths.api_v1_public_recording_ids_musical_features.get import RecordingsByIdsWithMusicalFeatures
-from songtradr_api_client_python.paths.api_v1_public_recording_ids_similarities.get import RecordingsByIdsWithSimilarities
-from songtradr_api_client_python.paths.api_v1_public_recording_ids_taggrams.get import RecordingsByIdsWithTaggrams
-from songtradr_api_client_python.paths.api_v1_public_recording_ids_tagstrengths.get import RecordingsByIdsWithTagstrengths
-from songtradr_api_client_python.paths.api_v1_public_recording_l_ids.get import RecordingsLargeByIds
-from songtradr_api_client_python.paths.api_v1_public_recording_m_ids.get import RecordingsMediumByIds
-from songtradr_api_client_python.paths.api_v1_public_recording_s_ids.get import RecordingsSmallByIds
-from songtradr_api_client_python.paths.api_v1_public_recording_search.get import SearchRecordings
-from songtradr_api_client_python.paths.api_v1_public_recording_search_granular.post import SearchRecordingsGranular
-from songtradr_api_client_python.paths.api_v1_public_recording_search_granular_abstraction.post import SearchRecordingsGranularAbstraction
-
-
-class RecordingApi(
-    RecordingsByIdsWithMusicalFeatures,
-    RecordingsByIdsWithSimilarities,
-    RecordingsByIdsWithTaggrams,
-    RecordingsByIdsWithTagstrengths,
-    RecordingsLargeByIds,
-    RecordingsMediumByIds,
-    RecordingsSmallByIds,
-    SearchRecordings,
-    SearchRecordingsGranular,
-    SearchRecordingsGranularAbstraction,
-):
-    """NOTE: This class is auto generated by OpenAPI Generator
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
-    """
-    pass
+import unittest
+import datetime
+
+import songtradr_api_client_python
+from songtradr_api_client_python.models.tagstrength_dto import TagstrengthDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
+
+class TestTagstrengthDTO(unittest.TestCase):
+    """TagstrengthDTO unit test stubs"""
+
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test TagstrengthDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `TagstrengthDTO`
+        """
+        model = songtradr_api_client_python.models.tagstrength_dto.TagstrengthDTO()  # noqa: E501
+        if include_optional :
+            return TagstrengthDTO(
+                strength = 1.337, 
+                category_name = '', 
+                tag_name = '', 
+                genre_name = '', 
+                scale = [
+                    56
+                    ]
+            )
+        else :
+            return TagstrengthDTO(
+                strength = 1.337,
+                category_name = '',
+        )
+        """
+
+    def testTagstrengthDTO(self):
+        """Test TagstrengthDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/configuration.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,100 +3,74 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
-from http import client as http_client
+import http.client as httplib
 from songtradr_api_client_python.exceptions import ApiValueError
 
-
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
-    'minLength', 'pattern', 'maxItems', 'minItems',
-    'uniqueItems', 'maxProperties', 'minProperties',
+    'minLength', 'pattern', 'maxItems', 'minItems'
 }
 
 class Configuration(object):
-    """NOTE: This class is auto generated by OpenAPI Generator
-
-    Ref: https://openapi-generator.tech
-    Do not edit the class manually.
+    """This class contains various settings of the API client.
 
-    :param host: Base url
+    :param host: Base url.
     :param api_key: Dict to store API key(s).
       Each entry in the dict specifies an API key.
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is the API key secret.
-    :param api_key_prefix: Dict to store API prefix (e.g. Bearer)
+    :param api_key_prefix: Dict to store API prefix (e.g. Bearer).
       The dict key is the name of the security scheme in the OAS specification.
       The dict value is an API key prefix when generating the auth data.
-    :param username: Username for HTTP basic authentication
-    :param password: Password for HTTP basic authentication
-    :param discard_unknown_keys: Boolean value indicating whether to discard
-      unknown properties. A server may send a response that includes additional
-      properties that are not known by the client in the following scenarios:
-      1. The OpenAPI document is incomplete, i.e. it does not match the server
-         implementation.
-      2. The client was generated using an older version of the OpenAPI document
-         and the server has been upgraded since then.
-      If a schema in the OpenAPI document defines the additionalProperties attribute,
-      then all undeclared properties received by the server are injected into the
-      additional properties map. In that case, there are undeclared properties, and
-      nothing to discard.
-    :param disabled_client_side_validations (string): Comma-separated list of
-      JSON schema validation keywords to disable JSON schema structural validation
-      rules. The following keywords may be specified: multipleOf, maximum,
-      exclusiveMaximum, minimum, exclusiveMinimum, maxLength, minLength, pattern,
-      maxItems, minItems.
-      By default, the validation is performed for data generated locally by the client
-      and data received from the server, independent of any validation performed by
-      the server side. If the input data does not satisfy the JSON schema validation
-      rules specified in the OpenAPI document, an exception is raised.
-      If disabled_client_side_validations is set, structural validation is
-      disabled. This can be useful to troubleshoot data validation problem, such as
-      when the OpenAPI document validation rules do not match the actual API data
-      received by the server.
+    :param username: Username for HTTP basic authentication.
+    :param password: Password for HTTP basic authentication.
+    :param access_token: Access token.
     :param server_index: Index to servers configuration.
     :param server_variables: Mapping with string values to replace variables in
       templated server configuration. The validation of enums is performed for
       variables with defined enum values before.
     :param server_operation_index: Mapping from operation ID to an index to server
       configuration.
     :param server_operation_variables: Mapping from operation ID to a mapping with
       string values to replace variables in templated server configuration.
       The validation of enums is performed for variables with defined enum values before.
+    :param ssl_ca_cert: str - the path to a file of concatenated CA certificates
+      in PEM format.
 
     :Example:
     """
 
     _default = None
 
-    def __init__(
-        self,
-        host=None,
-        discard_unknown_keys=False,
-        disabled_client_side_validations="",
-        server_index=None,
-        server_variables=None,
-        server_operation_index=None,
-        server_operation_variables=None,
-        access_token=None,
-    ):
+    def __init__(self, host=None,
+                 api_key=None, api_key_prefix=None,
+                 username=None, password=None,
+                 access_token=None,
+                 server_index=None, server_variables=None,
+                 server_operation_index=None, server_operation_variables=None,
+                 ssl_ca_cert=None,
+                 ):
         """Constructor
         """
         self._base_path = "https://api.songtradr.com" if host is None else host
         """Default Base url
         """
         self.server_index = 0 if server_index is None and host is None else server_index
         self.server_operation_index = server_operation_index or {}
@@ -106,17 +80,35 @@
         self.server_operation_variables = server_operation_variables or {}
         """Default server variables
         """
         self.temp_folder_path = None
         """Temp file folder for downloading files
         """
         # Authentication Settings
-        self.disabled_client_side_validations = disabled_client_side_validations
-        self.access_token = None
-        """access token for OAuth/Bearer
+        self.api_key = {}
+        if api_key:
+            self.api_key = api_key
+        """dict to store API key(s)
+        """
+        self.api_key_prefix = {}
+        if api_key_prefix:
+            self.api_key_prefix = api_key_prefix
+        """dict to store API prefix (e.g. Bearer)
+        """
+        self.refresh_api_key_hook = None
+        """function hook to refresh API key if expired
+        """
+        self.username = username
+        """Username for HTTP basic authentication
+        """
+        self.password = password
+        """Password for HTTP basic authentication
+        """
+        self.access_token = access_token
+        """Access token
         """
         self.logger = {}
         """Logging Settings
         """
         self.logger["package_logger"] = logging.getLogger("songtradr_api_client_python")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
@@ -136,15 +128,15 @@
         """
 
         self.verify_ssl = True
         """SSL/TLS verification
            Set this to false to skip verifying SSL certificate when calling API
            from https server.
         """
-        self.ssl_ca_cert = None
+        self.ssl_ca_cert = ssl_ca_cert
         """Set this to customize the certificate file to verify the peer.
         """
         self.cert_file = None
         """client certificate file
         """
         self.key_file = None
         """client key file
@@ -176,16 +168,25 @@
         """
         self.retries = None
         """Adding retries to override urllib3 default value 3
         """
         # Enable client side validation
         self.client_side_validation = True
 
-        # Options to pass down to the underlying urllib3 socket
         self.socket_options = None
+        """Options to pass down to the underlying urllib3 socket
+        """
+
+        self.datetime_format = "%Y-%m-%dT%H:%M:%S.%f%z"
+        """datetime format
+        """
+
+        self.date_format = "%Y-%m-%d"
+        """date format
+        """
 
     def __deepcopy__(self, memo):
         cls = self.__class__
         result = cls.__new__(cls)
         memo[id(self)] = result
         for k, v in self.__dict__.items():
             if k not in ('logger', 'logger_file_handler'):
@@ -195,46 +196,49 @@
         # use setters to configure loggers
         result.logger_file = self.logger_file
         result.debug = self.debug
         return result
 
     def __setattr__(self, name, value):
         object.__setattr__(self, name, value)
-        if name == 'disabled_client_side_validations':
-            s = set(filter(None, value.split(',')))
-            for v in s:
-                if v not in JSON_SCHEMA_VALIDATION_KEYWORDS:
-                    raise ApiValueError(
-                        "Invalid keyword: '{0}''".format(v))
-            self._disabled_client_side_validations = s
 
     @classmethod
     def set_default(cls, default):
         """Set default instance of configuration.
 
         It stores default configuration, which can be
         returned by get_default_copy method.
 
         :param default: object of Configuration
         """
-        cls._default = copy.deepcopy(default)
+        cls._default = default
 
     @classmethod
     def get_default_copy(cls):
-        """Return new instance of configuration.
+        """Deprecated. Please use `get_default` instead.
+
+        Deprecated. Please use `get_default` instead.
+
+        :return: The configuration object.
+        """
+        return cls.get_default()
+
+    @classmethod
+    def get_default(cls):
+        """Return the default configuration.
 
         This method returns newly created, based on default constructor,
         object of Configuration class or returns a copy of default
-        configuration passed by the set_default method.
+        configuration.
 
         :return: The configuration object.
         """
-        if cls._default is not None:
-            return copy.deepcopy(cls._default)
-        return Configuration()
+        if cls._default is None:
+            cls._default = Configuration()
+        return cls._default
 
     @property
     def logger_file(self):
         """The logger file.
 
         If the logger_file is None, then add stream handler and remove file
         handler. Otherwise, add file handler and remove stream handler.
@@ -280,23 +284,23 @@
         :type: bool
         """
         self.__debug = value
         if self.__debug:
             # if debug status is True, turn on debug logging
             for _, logger in self.logger.items():
                 logger.setLevel(logging.DEBUG)
-            # turn on http_client debug
-            http_client.HTTPConnection.debuglevel = 1
+            # turn on httplib debug
+            httplib.HTTPConnection.debuglevel = 1
         else:
             # if debug status is False, turn off debug logging,
             # setting log level to default `logging.WARNING`
             for _, logger in self.logger.items():
                 logger.setLevel(logging.WARNING)
-            # turn off http_client debug
-            http_client.HTTPConnection.debuglevel = 0
+            # turn off httplib debug
+            httplib.HTTPConnection.debuglevel = 0
 
     @property
     def logger_format(self):
         """The logger format.
 
         The logger_formatter will be updated when sets logger_format.
 
@@ -370,15 +374,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.12.21\n"\
-               "SDK Package Version: 0.0.1".\
+               "SDK Package Version: 1.12.21".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/exceptions.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-import dataclasses
-import typing
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from urllib3._collections import HTTPHeaderDict
+    Do not edit the class manually.
+"""
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
 
 
 class ApiTypeError(OpenApiException, TypeError):
@@ -98,48 +96,69 @@
         self.path_to_item = path_to_item
         full_msg = msg
         if path_to_item:
             full_msg = "{0} at {1}".format(msg, render_path(path_to_item))
         super(ApiKeyError, self).__init__(full_msg)
 
 
-T = typing.TypeVar("T")
+class ApiException(OpenApiException):
 
-
-@dataclasses.dataclass
-class ApiException(OpenApiException, typing.Generic[T]):
-    status: int
-    reason: str
-    api_response: typing.Optional[T] = None
-
-    @property
-    def body(self) -> typing.Union[str, bytes, None]:
-        if not self.api_response:
-            return None
-        return self.api_response.response.data
-
-    @property
-    def headers(self) -> typing.Optional[HTTPHeaderDict]:
-        if not self.api_response:
-            return None
-        return self.api_response.response.getheaders()
+    def __init__(self, status=None, reason=None, http_resp=None):
+        if http_resp:
+            self.status = http_resp.status
+            self.reason = http_resp.reason
+            self.body = http_resp.data
+            self.headers = http_resp.getheaders()
+        else:
+            self.status = status
+            self.reason = reason
+            self.body = None
+            self.headers = None
 
     def __str__(self):
         """Custom error messages for exception"""
         error_message = "({0})\n"\
                         "Reason: {1}\n".format(self.status, self.reason)
         if self.headers:
             error_message += "HTTP response headers: {0}\n".format(
                 self.headers)
 
         if self.body:
             error_message += "HTTP response body: {0}\n".format(self.body)
 
         return error_message
 
+class BadRequestException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(BadRequestException, self).__init__(status, reason, http_resp)
+
+class NotFoundException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(NotFoundException, self).__init__(status, reason, http_resp)
+
+
+class UnauthorizedException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(UnauthorizedException, self).__init__(status, reason, http_resp)
+
+
+class ForbiddenException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ForbiddenException, self).__init__(status, reason, http_resp)
+
+
+class ServiceException(ApiException):
+
+    def __init__(self, status=None, reason=None, http_resp=None):
+        super(ServiceException, self).__init__(status, reason, http_resp)
+
 
 def render_path(path_to_item):
     """Returns a string representation of a path"""
     result = ""
     for pth in path_to_item:
         if isinstance(pth, int):
             result += "[{0}]".format(pth)
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/category_medium_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/playlist_large_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,133 +3,115 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
-
-from songtradr_api_client_python import schemas  # noqa: F401
+    Do not edit the class manually.
+"""
 
 
-class CategoryMediumDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-    Do not edit the class manually.
+from datetime import datetime
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictStr, conlist, validator
+from songtradr_api_client_python.models.recording_playlist_dto import RecordingPlaylistDTO
+from songtradr_api_client_python.models.usage_dto import UsageDTO
 
-    A category of tags with its underlying tags.
+class PlaylistLargeDTO(BaseModel):
     """
+    Details on a playlist
+    """
+    name: StrictStr = Field(...)
+    state: Optional[StrictStr] = None
+    created: Optional[datetime] = None
+    updated: Optional[datetime] = None
+    description: Optional[StrictStr] = None
+    asset_url: Optional[StrictStr] = Field(None, alias="assetURL")
+    pretzel_tier: Optional[StrictStr] = Field(None, alias="pretzelTier")
+    usage: Optional[StrictStr] = None
+    tracks: Optional[conlist(RecordingPlaylistDTO)] = None
+    songtradr_playlist_guid: Optional[StrictStr] = Field(None, alias="songtradrPlaylistGuid")
+    usages: Optional[conlist(UsageDTO)] = None
+    __properties = ["name", "state", "created", "updated", "description", "assetURL", "pretzelTier", "usage", "tracks", "songtradrPlaylistGuid", "usages"]
+
+    @validator('state')
+    def state_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('active', 'draft'):
+            raise ValueError("must be one of enum values ('active', 'draft')")
+        return value
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> PlaylistLargeDTO:
+        """Create an instance of PlaylistLargeDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in tracks (list)
+        _items = []
+        if self.tracks:
+            for _item in self.tracks:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['tracks'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in usages (list)
+        _items = []
+        if self.usages:
+            for _item in self.usages:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['usages'] = _items
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> PlaylistLargeDTO:
+        """Create an instance of PlaylistLargeDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return PlaylistLargeDTO.parse_obj(obj)
+
+        _obj = PlaylistLargeDTO.parse_obj({
+            "name": obj.get("name"),
+            "state": obj.get("state"),
+            "created": obj.get("created"),
+            "updated": obj.get("updated"),
+            "description": obj.get("description"),
+            "asset_url": obj.get("assetURL"),
+            "pretzel_tier": obj.get("pretzelTier"),
+            "usage": obj.get("usage"),
+            "tracks": [RecordingPlaylistDTO.from_dict(_item) for _item in obj.get("tracks")] if obj.get("tracks") is not None else None,
+            "songtradr_playlist_guid": obj.get("songtradrPlaylistGuid"),
+            "usages": [UsageDTO.from_dict(_item) for _item in obj.get("usages")] if obj.get("usages") is not None else None
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "name",
-            "id",
-        }
-        
-        class properties:
-            id = schemas.Int32Schema
-            name = schemas.StrSchema
-            
-            
-            class tags(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['TagSmallDTO']:
-                        return TagSmallDTO
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple['TagSmallDTO'], typing.List['TagSmallDTO']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'tags':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'TagSmallDTO':
-                    return super().__getitem__(i)
-            __annotations__ = {
-                "id": id,
-                "name": name,
-                "tags": tags,
-            }
-    
-    name: MetaOapg.properties.name
-    id: MetaOapg.properties.id
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["tags"]) -> MetaOapg.properties.tags: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "name", "tags", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["tags"]) -> typing.Union[MetaOapg.properties.tags, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "name", "tags", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        name: typing.Union[MetaOapg.properties.name, str, ],
-        id: typing.Union[MetaOapg.properties.id, decimal.Decimal, int, ],
-        tags: typing.Union[MetaOapg.properties.tags, list, tuple, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'CategoryMediumDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            name=name,
-            id=id,
-            tags=tags,
-            _configuration=_configuration,
-            **kwargs,
-        )
-
-from songtradr_api_client_python.model.tag_small_dto import TagSmallDTO
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/category_minimal_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/tagstrength_dto.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,84 +3,77 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from songtradr_api_client_python import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class CategoryMinimalDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import List, Optional, Union
+from pydantic import BaseModel, Field, StrictFloat, StrictInt, StrictStr, conlist
 
-    A category of tags in its minimal form.
+class TagstrengthDTO(BaseModel):
     """
+    A TaggramDTO for recordings.
+    """
+    strength: Union[StrictFloat, StrictInt] = Field(..., description="Strength of presence of the corresponding category, tag or genre.")
+    category_name: StrictStr = Field(..., alias="categoryName")
+    tag_name: Optional[StrictStr] = Field(None, alias="tagName")
+    genre_name: Optional[StrictStr] = Field(None, alias="genreName")
+    scale: Optional[conlist(StrictInt)] = None
+    __properties = ["strength", "categoryName", "tagName", "genreName", "scale"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> TagstrengthDTO:
+        """Create an instance of TagstrengthDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> TagstrengthDTO:
+        """Create an instance of TagstrengthDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return TagstrengthDTO.parse_obj(obj)
+
+        _obj = TagstrengthDTO.parse_obj({
+            "strength": obj.get("strength"),
+            "category_name": obj.get("categoryName"),
+            "tag_name": obj.get("tagName"),
+            "genre_name": obj.get("genreName"),
+            "scale": obj.get("scale")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "categoryName",
-        }
-        
-        class properties:
-            categoryName = schemas.StrSchema
-            __annotations__ = {
-                "categoryName": categoryName,
-            }
-    
-    categoryName: MetaOapg.properties.categoryName
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["categoryName"]) -> MetaOapg.properties.categoryName: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["categoryName", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["categoryName"]) -> MetaOapg.properties.categoryName: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["categoryName", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        categoryName: typing.Union[MetaOapg.properties.categoryName, str, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'CategoryMinimalDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            categoryName=categoryName,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/contributor_type_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_w_ith_url_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,84 +3,75 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Do not edit the class manually.
+"""
 
-import frozendict  # noqa: F401
 
-from songtradr_api_client_python import schemas  # noqa: F401
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
 
-class ContributorTypeDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from pydantic import BaseModel, Field, StrictStr
+from songtradr_api_client_python.models.file_dto import FileDTO
 
-    A type of contribution a party (person, group or organization) had on a recording or product.
+class FileWIthUrlDTO(BaseModel):
     """
+    Details on a file that has been uploaded for auto-tagging or audio-recognition purposes. including download path.
+    """
+    file: FileDTO = Field(...)
+    url: StrictStr = Field(...)
+    __properties = ["file", "url"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> FileWIthUrlDTO:
+        """Create an instance of FileWIthUrlDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of file
+        if self.file:
+            _dict['file'] = self.file.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> FileWIthUrlDTO:
+        """Create an instance of FileWIthUrlDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return FileWIthUrlDTO.parse_obj(obj)
+
+        _obj = FileWIthUrlDTO.parse_obj({
+            "file": FileDTO.from_dict(obj.get("file")) if obj.get("file") is not None else None,
+            "url": obj.get("url")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "typeName",
-        }
-        
-        class properties:
-            typeName = schemas.StrSchema
-            __annotations__ = {
-                "typeName": typeName,
-            }
-    
-    typeName: MetaOapg.properties.typeName
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["typeName"]) -> MetaOapg.properties.typeName: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["typeName", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["typeName"]) -> MetaOapg.properties.typeName: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["typeName", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        typeName: typing.Union[MetaOapg.properties.typeName, str, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'ContributorTypeDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            typeName=typeName,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/file_list_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/product_medium_dto.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,147 +3,113 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
-
-from songtradr_api_client_python import schemas  # noqa: F401
+    Do not edit the class manually.
+"""
 
 
-class FileListDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-    Do not edit the class manually.
+from datetime import datetime
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictStr, conlist
+from songtradr_api_client_python.models.genre_minimal_dto import GenreMinimalDTO
+from songtradr_api_client_python.models.p_line_dto import PLineDTO
+from songtradr_api_client_python.models.product_party_dto import ProductPartyDTO
+from songtradr_api_client_python.models.title_dto import TitleDTO
 
-    List of files.
+class ProductMediumDTO(BaseModel):
     """
+    Product details with a mid-sized field-set.
+    """
+    duration: Optional[datetime] = None
+    parties: Optional[conlist(ProductPartyDTO, unique_items=True)] = None
+    grid: Optional[StrictStr] = None
+    release_date: Optional[datetime] = Field(None, alias="releaseDate")
+    takedown_date: Optional[datetime] = Field(None, alias="takedownDate")
+    pline: Optional[PLineDTO] = None
+    titles: Optional[conlist(TitleDTO, unique_items=True)] = None
+    genres: Optional[conlist(GenreMinimalDTO, unique_items=True)] = None
+    gtin: Optional[StrictStr] = None
+    __properties = ["duration", "parties", "grid", "releaseDate", "takedownDate", "pline", "titles", "genres", "gtin"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> ProductMediumDTO:
+        """Create an instance of ProductMediumDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in parties (list)
+        _items = []
+        if self.parties:
+            for _item in self.parties:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['parties'] = _items
+        # override the default output from pydantic by calling `to_dict()` of pline
+        if self.pline:
+            _dict['pline'] = self.pline.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
+        _items = []
+        if self.titles:
+            for _item in self.titles:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['titles'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in genres (list)
+        _items = []
+        if self.genres:
+            for _item in self.genres:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['genres'] = _items
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> ProductMediumDTO:
+        """Create an instance of ProductMediumDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return ProductMediumDTO.parse_obj(obj)
+
+        _obj = ProductMediumDTO.parse_obj({
+            "duration": obj.get("duration"),
+            "parties": [ProductPartyDTO.from_dict(_item) for _item in obj.get("parties")] if obj.get("parties") is not None else None,
+            "grid": obj.get("grid"),
+            "release_date": obj.get("releaseDate"),
+            "takedown_date": obj.get("takedownDate"),
+            "pline": PLineDTO.from_dict(obj.get("pline")) if obj.get("pline") is not None else None,
+            "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None,
+            "genres": [GenreMinimalDTO.from_dict(_item) for _item in obj.get("genres")] if obj.get("genres") is not None else None,
+            "gtin": obj.get("gtin")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "totalResults",
-            "hasNextPage",
-            "currentPageNumber",
-            "files",
-        }
-        
-        class properties:
-            
-            
-            class files(
-                schemas.ListSchema
-            ):
-            
-            
-                class MetaOapg:
-                    
-                    @staticmethod
-                    def items() -> typing.Type['FileDTO']:
-                        return FileDTO
-            
-                def __new__(
-                    cls,
-                    _arg: typing.Union[typing.Tuple['FileDTO'], typing.List['FileDTO']],
-                    _configuration: typing.Optional[schemas.Configuration] = None,
-                ) -> 'files':
-                    return super().__new__(
-                        cls,
-                        _arg,
-                        _configuration=_configuration,
-                    )
-            
-                def __getitem__(self, i: int) -> 'FileDTO':
-                    return super().__getitem__(i)
-            hasNextPage = schemas.BoolSchema
-            currentPageNumber = schemas.Int32Schema
-            totalResults = schemas.Int32Schema
-            __annotations__ = {
-                "files": files,
-                "hasNextPage": hasNextPage,
-                "currentPageNumber": currentPageNumber,
-                "totalResults": totalResults,
-            }
-    
-    totalResults: MetaOapg.properties.totalResults
-    hasNextPage: MetaOapg.properties.hasNextPage
-    currentPageNumber: MetaOapg.properties.currentPageNumber
-    files: MetaOapg.properties.files
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["files"]) -> MetaOapg.properties.files: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["hasNextPage"]) -> MetaOapg.properties.hasNextPage: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["currentPageNumber"]) -> MetaOapg.properties.currentPageNumber: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["totalResults"]) -> MetaOapg.properties.totalResults: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["files", "hasNextPage", "currentPageNumber", "totalResults", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["files"]) -> MetaOapg.properties.files: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["hasNextPage"]) -> MetaOapg.properties.hasNextPage: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["currentPageNumber"]) -> MetaOapg.properties.currentPageNumber: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["totalResults"]) -> MetaOapg.properties.totalResults: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["files", "hasNextPage", "currentPageNumber", "totalResults", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        totalResults: typing.Union[MetaOapg.properties.totalResults, decimal.Decimal, int, ],
-        hasNextPage: typing.Union[MetaOapg.properties.hasNextPage, bool, ],
-        currentPageNumber: typing.Union[MetaOapg.properties.currentPageNumber, decimal.Decimal, int, ],
-        files: typing.Union[MetaOapg.properties.files, list, tuple, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'FileListDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            totalResults=totalResults,
-            hasNextPage=hasNextPage,
-            currentPageNumber=currentPageNumber,
-            files=files,
-            _configuration=_configuration,
-            **kwargs,
-        )
-
-from songtradr_api_client_python.model.file_dto import FileDTO
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/file_w_ith_url_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/file_upload_dto.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,101 +3,89 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from songtradr_api_client_python import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class FileWIthUrlDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import List, Optional
+from pydantic import BaseModel, StrictStr, conlist
+from songtradr_api_client_python.models.config_access_dto import ConfigAccessDTO
+from songtradr_api_client_python.models.config_identifier_dto import ConfigIdentifierDTO
 
-    Details on a file that has been uploaded for auto-tagging or audio-recognition purposes. including download path.
+class FileUploadDTO(BaseModel):
     """
+    Details on content, ownership, purpose and access rights of a file to be uploaded.
+    """
+    identifiers: Optional[conlist(ConfigIdentifierDTO)] = None
+    flags: Optional[conlist(StrictStr)] = None
+    access: Optional[conlist(ConfigAccessDTO)] = None
+    __properties = ["identifiers", "flags", "access"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> FileUploadDTO:
+        """Create an instance of FileUploadDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in identifiers (list)
+        _items = []
+        if self.identifiers:
+            for _item in self.identifiers:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['identifiers'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in access (list)
+        _items = []
+        if self.access:
+            for _item in self.access:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['access'] = _items
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> FileUploadDTO:
+        """Create an instance of FileUploadDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return FileUploadDTO.parse_obj(obj)
+
+        _obj = FileUploadDTO.parse_obj({
+            "identifiers": [ConfigIdentifierDTO.from_dict(_item) for _item in obj.get("identifiers")] if obj.get("identifiers") is not None else None,
+            "flags": obj.get("flags"),
+            "access": [ConfigAccessDTO.from_dict(_item) for _item in obj.get("access")] if obj.get("access") is not None else None
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "file",
-            "url",
-        }
-        
-        class properties:
-        
-            @staticmethod
-            def file() -> typing.Type['FileDTO']:
-                return FileDTO
-            url = schemas.StrSchema
-            __annotations__ = {
-                "file": file,
-                "url": url,
-            }
-    
-    file: 'FileDTO'
-    url: MetaOapg.properties.url
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["file"]) -> 'FileDTO': ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["url"]) -> MetaOapg.properties.url: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["file", "url", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["file"]) -> 'FileDTO': ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["url"]) -> MetaOapg.properties.url: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["file", "url", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        file: 'FileDTO',
-        url: typing.Union[MetaOapg.properties.url, str, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'FileWIthUrlDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            file=file,
-            url=url,
-            _configuration=_configuration,
-            **kwargs,
-        )
-
-from songtradr_api_client_python.model.file_dto import FileDTO
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/genre_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_playlist_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,96 +3,79 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from songtradr_api_client_python import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class GenreDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import Optional
+from pydantic import BaseModel, Field, StrictInt, StrictStr
+from songtradr_api_client_python.models.recording_medium_dto import RecordingMediumDTO
 
-    Genre including its sub-genres.
+class RecordingPlaylistDTO(BaseModel):
     """
+    Recording Playlist connection
+    """
+    recording: Optional[RecordingMediumDTO] = None
+    songtradr_track_guid: Optional[StrictStr] = Field(None, alias="songtradrTrackGuid")
+    assigned_by_id: Optional[StrictInt] = Field(None, alias="assignedById")
+    sequence: Optional[StrictInt] = None
+    __properties = ["recording", "songtradrTrackGuid", "assignedById", "sequence"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> RecordingPlaylistDTO:
+        """Create an instance of RecordingPlaylistDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of recording
+        if self.recording:
+            _dict['recording'] = self.recording.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> RecordingPlaylistDTO:
+        """Create an instance of RecordingPlaylistDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return RecordingPlaylistDTO.parse_obj(obj)
+
+        _obj = RecordingPlaylistDTO.parse_obj({
+            "recording": RecordingMediumDTO.from_dict(obj.get("recording")) if obj.get("recording") is not None else None,
+            "songtradr_track_guid": obj.get("songtradrTrackGuid"),
+            "assigned_by_id": obj.get("assignedById"),
+            "sequence": obj.get("sequence")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "name",
-            "id",
-        }
-        
-        class properties:
-            id = schemas.Int32Schema
-            name = schemas.StrSchema
-            __annotations__ = {
-                "id": id,
-                "name": name,
-            }
-    
-    name: MetaOapg.properties.name
-    id: MetaOapg.properties.id
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "name", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "name", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        name: typing.Union[MetaOapg.properties.name, str, ],
-        id: typing.Union[MetaOapg.properties.id, decimal.Decimal, int, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'GenreDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            name=name,
-            id=id,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/genre_minimal_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/field_summary_dto.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,84 +3,73 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Do not edit the class manually.
+"""
 
-import frozendict  # noqa: F401
 
-from songtradr_api_client_python import schemas  # noqa: F401
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
 
-class GenreMinimalDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-    Genre in its minimal form.
+class FieldSummaryDTO(BaseModel):
     """
+    Summary of genres occuring in files.
+    """
+    field_value: StrictStr = Field(..., alias="fieldValue")
+    total: StrictInt = Field(...)
+    field_name: StrictStr = Field(..., alias="fieldName")
+    __properties = ["fieldValue", "total", "fieldName"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> FieldSummaryDTO:
+        """Create an instance of FieldSummaryDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> FieldSummaryDTO:
+        """Create an instance of FieldSummaryDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return FieldSummaryDTO.parse_obj(obj)
+
+        _obj = FieldSummaryDTO.parse_obj({
+            "field_value": obj.get("fieldValue"),
+            "total": obj.get("total"),
+            "field_name": obj.get("fieldName")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "genreName",
-        }
-        
-        class properties:
-            genreName = schemas.StrSchema
-            __annotations__ = {
-                "genreName": genreName,
-            }
-    
-    genreName: MetaOapg.properties.genreName
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["genreName"]) -> MetaOapg.properties.genreName: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["genreName", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["genreName"]) -> MetaOapg.properties.genreName: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["genreName", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        genreName: typing.Union[MetaOapg.properties.genreName, str, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'GenreMinimalDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            genreName=genreName,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/jwt_token_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_small_dto.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,106 +3,91 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from songtradr_api_client_python import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class JwtTokenDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist
+from songtradr_api_client_python.models.recording_party_dto import RecordingPartyDTO
+from songtradr_api_client_python.models.title_dto import TitleDTO
 
-    Bearer token to be used for authentication.
+class RecordingSmallDTO(BaseModel):
     """
+    Recording with a small field set.
+    """
+    duration: Optional[StrictInt] = None
+    titles: Optional[conlist(TitleDTO, unique_items=True)] = None
+    parties: Optional[conlist(RecordingPartyDTO, unique_items=True)] = None
+    isrc: StrictStr = Field(...)
+    __properties = ["duration", "titles", "parties", "isrc"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> RecordingSmallDTO:
+        """Create an instance of RecordingSmallDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in titles (list)
+        _items = []
+        if self.titles:
+            for _item in self.titles:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['titles'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in parties (list)
+        _items = []
+        if self.parties:
+            for _item in self.parties:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['parties'] = _items
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> RecordingSmallDTO:
+        """Create an instance of RecordingSmallDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return RecordingSmallDTO.parse_obj(obj)
+
+        _obj = RecordingSmallDTO.parse_obj({
+            "duration": obj.get("duration"),
+            "titles": [TitleDTO.from_dict(_item) for _item in obj.get("titles")] if obj.get("titles") is not None else None,
+            "parties": [RecordingPartyDTO.from_dict(_item) for _item in obj.get("parties")] if obj.get("parties") is not None else None,
+            "isrc": obj.get("isrc")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "jwtToken",
-            "expirationDate",
-        }
-        
-        class properties:
-            jwtToken = schemas.StrSchema
-            expirationDate = schemas.DateTimeSchema
-            refreshToken = schemas.StrSchema
-            __annotations__ = {
-                "jwtToken": jwtToken,
-                "expirationDate": expirationDate,
-                "refreshToken": refreshToken,
-            }
-    
-    jwtToken: MetaOapg.properties.jwtToken
-    expirationDate: MetaOapg.properties.expirationDate
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["jwtToken"]) -> MetaOapg.properties.jwtToken: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["expirationDate"]) -> MetaOapg.properties.expirationDate: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["refreshToken"]) -> MetaOapg.properties.refreshToken: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["jwtToken", "expirationDate", "refreshToken", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["jwtToken"]) -> MetaOapg.properties.jwtToken: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["expirationDate"]) -> MetaOapg.properties.expirationDate: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["refreshToken"]) -> typing.Union[MetaOapg.properties.refreshToken, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["jwtToken", "expirationDate", "refreshToken", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        jwtToken: typing.Union[MetaOapg.properties.jwtToken, str, ],
-        expirationDate: typing.Union[MetaOapg.properties.expirationDate, str, datetime, ],
-        refreshToken: typing.Union[MetaOapg.properties.refreshToken, str, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'JwtTokenDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            jwtToken=jwtToken,
-            expirationDate=expirationDate,
-            refreshToken=refreshToken,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/p_line_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/forgot_password_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,94 +3,81 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from songtradr_api_client_python import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class PLineDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import Optional
+from pydantic import BaseModel, Field, StrictStr, validator
 
-    Details on a recording's or product's rights.
+class ForgotPasswordDTO(BaseModel):
     """
+    ForgotPasswordDTO
+    """
+    email_or_username: StrictStr = Field(..., alias="emailOrUsername")
+    system: Optional[StrictStr] = None
+    __properties = ["emailOrUsername", "system"]
+
+    @validator('system')
+    def system_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('musicube', 'cloud'):
+            raise ValueError("must be one of enum values ('musicube', 'cloud')")
+        return value
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> ForgotPasswordDTO:
+        """Create an instance of ForgotPasswordDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> ForgotPasswordDTO:
+        """Create an instance of ForgotPasswordDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return ForgotPasswordDTO.parse_obj(obj)
+
+        _obj = ForgotPasswordDTO.parse_obj({
+            "email_or_username": obj.get("emailOrUsername"),
+            "system": obj.get("system")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "text",
-        }
-        
-        class properties:
-            text = schemas.StrSchema
-            year = schemas.Int32Schema
-            __annotations__ = {
-                "text": text,
-                "year": year,
-            }
-    
-    text: MetaOapg.properties.text
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["text"]) -> MetaOapg.properties.text: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["year"]) -> MetaOapg.properties.year: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["text", "year", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["text"]) -> MetaOapg.properties.text: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["year"]) -> typing.Union[MetaOapg.properties.year, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["text", "year", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        text: typing.Union[MetaOapg.properties.text, str, ],
-        year: typing.Union[MetaOapg.properties.year, decimal.Decimal, int, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PLineDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            text=text,
-            year=year,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/party_small_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/party_large_dto.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,96 +3,83 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from songtradr_api_client_python import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class PartySmallDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import Optional
+from pydantic import BaseModel, Field, StrictStr
 
-    Party (person, group or organization) with a small field-set.
+class PartyLargeDTO(BaseModel):
     """
+    Party (person, group or organization) with a large field-set.
+    """
+    full_name: StrictStr = Field(..., alias="fullName")
+    birth_date: Optional[StrictStr] = Field(None, alias="birthDate")
+    death_date: Optional[StrictStr] = Field(None, alias="deathDate")
+    birth_year: Optional[StrictStr] = Field(None, alias="birthYear")
+    death_year: Optional[StrictStr] = Field(None, alias="deathYear")
+    birth_place: Optional[StrictStr] = Field(None, alias="birthPlace")
+    musicbrainz_type: Optional[StrictStr] = Field(None, alias="musicbrainzType")
+    area: Optional[StrictStr] = None
+    __properties = ["fullName", "birthDate", "deathDate", "birthYear", "deathYear", "birthPlace", "musicbrainzType", "area"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> PartyLargeDTO:
+        """Create an instance of PartyLargeDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> PartyLargeDTO:
+        """Create an instance of PartyLargeDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return PartyLargeDTO.parse_obj(obj)
+
+        _obj = PartyLargeDTO.parse_obj({
+            "full_name": obj.get("fullName"),
+            "birth_date": obj.get("birthDate"),
+            "death_date": obj.get("deathDate"),
+            "birth_year": obj.get("birthYear"),
+            "death_year": obj.get("deathYear"),
+            "birth_place": obj.get("birthPlace"),
+            "musicbrainz_type": obj.get("musicbrainzType"),
+            "area": obj.get("area")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "fullName",
-            "id",
-        }
-        
-        class properties:
-            id = schemas.StrSchema
-            fullName = schemas.StrSchema
-            __annotations__ = {
-                "id": id,
-                "fullName": fullName,
-            }
-    
-    fullName: MetaOapg.properties.fullName
-    id: MetaOapg.properties.id
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["fullName"]) -> MetaOapg.properties.fullName: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "fullName", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["fullName"]) -> MetaOapg.properties.fullName: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "fullName", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        fullName: typing.Union[MetaOapg.properties.fullName, str, ],
-        id: typing.Union[MetaOapg.properties.id, str, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'PartySmallDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            fullName=fullName,
-            id=id,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/recording_tag_small_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/recording_list_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,89 +3,83 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from songtradr_api_client_python import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class RecordingTagSmallDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import List
+from pydantic import BaseModel, Field, StrictBool, StrictInt, conlist
+from songtradr_api_client_python.models.recording_medium_dto import RecordingMediumDTO
 
-    Tag information in with a small field-set.
+class RecordingListDTO(BaseModel):
     """
+    List of recordings with with a mid-sized field set.
+    """
+    recordings: conlist(RecordingMediumDTO) = Field(...)
+    has_next_page: StrictBool = Field(..., alias="hasNextPage")
+    current_page_number: StrictInt = Field(..., alias="currentPageNumber")
+    total_results: StrictInt = Field(..., alias="totalResults")
+    __properties = ["recordings", "hasNextPage", "currentPageNumber", "totalResults"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> RecordingListDTO:
+        """Create an instance of RecordingListDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in recordings (list)
+        _items = []
+        if self.recordings:
+            for _item in self.recordings:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['recordings'] = _items
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> RecordingListDTO:
+        """Create an instance of RecordingListDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return RecordingListDTO.parse_obj(obj)
+
+        _obj = RecordingListDTO.parse_obj({
+            "recordings": [RecordingMediumDTO.from_dict(_item) for _item in obj.get("recordings")] if obj.get("recordings") is not None else None,
+            "has_next_page": obj.get("hasNextPage"),
+            "current_page_number": obj.get("currentPageNumber"),
+            "total_results": obj.get("totalResults")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "tag",
-        }
-        
-        class properties:
-        
-            @staticmethod
-            def tag() -> typing.Type['TagDTO']:
-                return TagDTO
-            __annotations__ = {
-                "tag": tag,
-            }
-    
-    tag: 'TagDTO'
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["tag"]) -> 'TagDTO': ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["tag", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["tag"]) -> 'TagDTO': ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["tag", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        tag: 'TagDTO',
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'RecordingTagSmallDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            tag=tag,
-            _configuration=_configuration,
-            **kwargs,
-        )
-
-from songtradr_api_client_python.model.tag_dto import TagDTO
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/save_recording_tag_dto.py` & `songtradr-api-client-python-1.12.21/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,94 +3,48 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
-
-import frozendict  # noqa: F401
-
-from songtradr_api_client_python import schemas  # noqa: F401
-
-
-class SaveRecordingTagDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
+"""
 
-    Recording-tag-connections the AI predicts and wants to save the API.
-    """
 
+from setuptools import setup, find_packages  # noqa: H301
 
-    class MetaOapg:
-        required = {
-            "tagName",
-        }
-        
-        class properties:
-            tagName = schemas.StrSchema
-            affinity = schemas.Float32Schema
-            __annotations__ = {
-                "tagName": tagName,
-                "affinity": affinity,
-            }
-    
-    tagName: MetaOapg.properties.tagName
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["tagName"]) -> MetaOapg.properties.tagName: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["affinity"]) -> MetaOapg.properties.affinity: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["tagName", "affinity", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["tagName"]) -> MetaOapg.properties.tagName: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["affinity"]) -> typing.Union[MetaOapg.properties.affinity, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["tagName", "affinity", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        tagName: typing.Union[MetaOapg.properties.tagName, str, ],
-        affinity: typing.Union[MetaOapg.properties.affinity, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SaveRecordingTagDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            tagName=tagName,
-            affinity=affinity,
-            _configuration=_configuration,
-            **kwargs,
-        )
+# To install the library, run the following
+#
+# python setup.py install
+#
+# prerequisite: setuptools
+# http://pypi.python.org/pypi/setuptools
+NAME = "songtradr-api-client-python"
+VERSION = "1.12.21"
+PYTHON_REQUIRES = ">=3.7"
+REQUIRES = [
+    "urllib3 >= 1.25.3, < 2.1.0",
+    "python-dateutil",
+    "pydantic >= 1.10.5, < 2",
+    "aenum"
+]
+
+setup(
+    name=NAME,
+    version=VERSION,
+    description="Songtradr API",
+    author="Songtradr Inc.",
+    author_email="info@songtradr.com",
+    url="https://pypi.org/project/songtradr-api-client-python/",
+    keywords=["OpenAPI", "OpenAPI-Generator", "Songtradr API"],
+    install_requires=REQUIRES,
+    packages=find_packages(exclude=["test", "tests"]),
+    include_package_data=True,
+    long_description_content_type='text/markdown',
+    long_description="""\
+    This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world&#39;s released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
+    """,
+    package_data={"songtradr_api_client_python": ["py.typed"]},
+)
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/search_recording_granular_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/category_medium_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,94 +3,81 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from songtradr_api_client_python import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class SearchRecordingGranularDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictInt, StrictStr, conlist
+from songtradr_api_client_python.models.tag_small_dto import TagSmallDTO
 
-    Timeseries of tags.
+class CategoryMediumDTO(BaseModel):
     """
+    A category of tags with its underlying tags.
+    """
+    id: StrictInt = Field(...)
+    tags: Optional[conlist(TagSmallDTO)] = None
+    name: StrictStr = Field(...)
+    __properties = ["id", "tags", "name"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> CategoryMediumDTO:
+        """Create an instance of CategoryMediumDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in tags (list)
+        _items = []
+        if self.tags:
+            for _item in self.tags:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['tags'] = _items
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> CategoryMediumDTO:
+        """Create an instance of CategoryMediumDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return CategoryMediumDTO.parse_obj(obj)
+
+        _obj = CategoryMediumDTO.parse_obj({
+            "id": obj.get("id"),
+            "tags": [TagSmallDTO.from_dict(_item) for _item in obj.get("tags")] if obj.get("tags") is not None else None,
+            "name": obj.get("name")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "tagName",
-        }
-        
-        class properties:
-            tagName = schemas.StrSchema
-            strength = schemas.Float32Schema
-            __annotations__ = {
-                "tagName": tagName,
-                "strength": strength,
-            }
-    
-    tagName: MetaOapg.properties.tagName
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["tagName"]) -> MetaOapg.properties.tagName: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["strength"]) -> MetaOapg.properties.strength: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["tagName", "strength", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["tagName"]) -> MetaOapg.properties.tagName: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["strength"]) -> typing.Union[MetaOapg.properties.strength, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["tagName", "strength", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        tagName: typing.Union[MetaOapg.properties.tagName, str, ],
-        strength: typing.Union[MetaOapg.properties.strength, decimal.Decimal, int, float, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'SearchRecordingGranularDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            tagName=tagName,
-            strength=strength,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/tag_small_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/product_party_dto.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,96 +3,83 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from songtradr_api_client_python import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class TagSmallDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import List, Optional
+from pydantic import BaseModel, Field, conlist
+from songtradr_api_client_python.models.contributor_type_dto import ContributorTypeDTO
+from songtradr_api_client_python.models.party_small_dto import PartySmallDTO
 
-    A tag for recordings with a reduced field-set.
+class ProductPartyDTO(BaseModel):
     """
+    Parties (persons, groups or organizations) that have contributed to a product.
+    """
+    contributor_types: Optional[conlist(ContributorTypeDTO)] = Field(None, alias="contributorTypes")
+    party: PartySmallDTO = Field(...)
+    __properties = ["contributorTypes", "party"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> ProductPartyDTO:
+        """Create an instance of ProductPartyDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of each item in contributor_types (list)
+        _items = []
+        if self.contributor_types:
+            for _item in self.contributor_types:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['contributorTypes'] = _items
+        # override the default output from pydantic by calling `to_dict()` of party
+        if self.party:
+            _dict['party'] = self.party.to_dict()
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> ProductPartyDTO:
+        """Create an instance of ProductPartyDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return ProductPartyDTO.parse_obj(obj)
+
+        _obj = ProductPartyDTO.parse_obj({
+            "contributor_types": [ContributorTypeDTO.from_dict(_item) for _item in obj.get("contributorTypes")] if obj.get("contributorTypes") is not None else None,
+            "party": PartySmallDTO.from_dict(obj.get("party")) if obj.get("party") is not None else None
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "name",
-            "id",
-        }
-        
-        class properties:
-            id = schemas.Int32Schema
-            name = schemas.StrSchema
-            __annotations__ = {
-                "id": id,
-                "name": name,
-            }
-    
-    name: MetaOapg.properties.name
-    id: MetaOapg.properties.id
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["id", "name", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["id"]) -> MetaOapg.properties.id: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["id", "name", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        name: typing.Union[MetaOapg.properties.name, str, ],
-        id: typing.Union[MetaOapg.properties.id, decimal.Decimal, int, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'TagSmallDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            name=name,
-            id=id,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/title_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/party_small_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,84 +3,71 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Do not edit the class manually.
+"""
 
-import frozendict  # noqa: F401
 
-from songtradr_api_client_python import schemas  # noqa: F401
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
 
-class TitleDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from pydantic import BaseModel, Field, StrictStr
 
-    A Title for recordings or products.
+class PartySmallDTO(BaseModel):
     """
+    Party (person, group or organization) with a small field-set.
+    """
+    id: StrictStr = Field(...)
+    full_name: StrictStr = Field(..., alias="fullName")
+    __properties = ["id", "fullName"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> PartySmallDTO:
+        """Create an instance of PartySmallDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> PartySmallDTO:
+        """Create an instance of PartySmallDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return PartySmallDTO.parse_obj(obj)
+
+        _obj = PartySmallDTO.parse_obj({
+            "id": obj.get("id"),
+            "full_name": obj.get("fullName")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "titleText",
-        }
-        
-        class properties:
-            titleText = schemas.StrSchema
-            __annotations__ = {
-                "titleText": titleText,
-            }
-    
-    titleText: MetaOapg.properties.titleText
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["titleText"]) -> MetaOapg.properties.titleText: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["titleText", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["titleText"]) -> MetaOapg.properties.titleText: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["titleText", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        titleText: typing.Union[MetaOapg.properties.titleText, str, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'TitleDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            titleText=titleText,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/token_request.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/genres_summary_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,82 +3,73 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Do not edit the class manually.
+"""
 
-import frozendict  # noqa: F401
 
-from songtradr_api_client_python import schemas  # noqa: F401
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
 
-class TokenRequest(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
+from typing import Optional
+from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-    Do not edit the class manually.
+class GenresSummaryDTO(BaseModel):
     """
+    Summary of genres occuring in files.
+    """
+    name: StrictStr = Field(...)
+    total: StrictInt = Field(...)
+    genre_type: Optional[StrictStr] = Field(None, alias="genreType")
+    __properties = ["name", "total", "genreType"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> GenresSummaryDTO:
+        """Create an instance of GenresSummaryDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> GenresSummaryDTO:
+        """Create an instance of GenresSummaryDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return GenresSummaryDTO.parse_obj(obj)
+
+        _obj = GenresSummaryDTO.parse_obj({
+            "name": obj.get("name"),
+            "total": obj.get("total"),
+            "genre_type": obj.get("genreType")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        required = {
-            "refreshToken",
-        }
-        
-        class properties:
-            refreshToken = schemas.StrSchema
-            __annotations__ = {
-                "refreshToken": refreshToken,
-            }
-    
-    refreshToken: MetaOapg.properties.refreshToken
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["refreshToken"]) -> MetaOapg.properties.refreshToken: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["refreshToken", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["refreshToken"]) -> MetaOapg.properties.refreshToken: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["refreshToken", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        refreshToken: typing.Union[MetaOapg.properties.refreshToken, str, ],
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'TokenRequest':
-        return super().__new__(
-            cls,
-            *_args,
-            refreshToken=refreshToken,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python/model/usage_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/save_referrer_dto.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,79 +3,71 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-from datetime import date, datetime  # noqa: F401
-import decimal  # noqa: F401
-import functools  # noqa: F401
-import io  # noqa: F401
-import re  # noqa: F401
-import typing  # noqa: F401
-import typing_extensions  # noqa: F401
-import uuid  # noqa: F401
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
-import frozendict  # noqa: F401
+    Do not edit the class manually.
+"""
 
-from songtradr_api_client_python import schemas  # noqa: F401
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
-class UsageDTO(
-    schemas.DictSchema
-):
-    """NOTE: This class is auto generated by OpenAPI Generator.
-    Ref: https://openapi-generator.tech
 
-    Do not edit the class manually.
+from typing import Optional
+from pydantic import BaseModel, StrictStr
 
-    Details on a track's or playlist's usage permissions.
+class SaveReferrerDTO(BaseModel):
     """
+    URLs that are allowed to reffer to musicube Widgets
+    """
+    username: Optional[StrictStr] = None
+    url: Optional[StrictStr] = None
+    __properties = ["username", "url"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> SaveReferrerDTO:
+        """Create an instance of SaveReferrerDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> SaveReferrerDTO:
+        """Create an instance of SaveReferrerDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return SaveReferrerDTO.parse_obj(obj)
+
+        _obj = SaveReferrerDTO.parse_obj({
+            "username": obj.get("username"),
+            "url": obj.get("url")
+        })
+        return _obj
 
-
-    class MetaOapg:
-        
-        class properties:
-            name = schemas.StrSchema
-            __annotations__ = {
-                "name": name,
-            }
-    
-    @typing.overload
-    def __getitem__(self, name: typing_extensions.Literal["name"]) -> MetaOapg.properties.name: ...
-    
-    @typing.overload
-    def __getitem__(self, name: str) -> schemas.UnsetAnyTypeSchema: ...
-    
-    def __getitem__(self, name: typing.Union[typing_extensions.Literal["name", ], str]):
-        # dict_instance[name] accessor
-        return super().__getitem__(name)
-    
-    
-    @typing.overload
-    def get_item_oapg(self, name: typing_extensions.Literal["name"]) -> typing.Union[MetaOapg.properties.name, schemas.Unset]: ...
-    
-    @typing.overload
-    def get_item_oapg(self, name: str) -> typing.Union[schemas.UnsetAnyTypeSchema, schemas.Unset]: ...
-    
-    def get_item_oapg(self, name: typing.Union[typing_extensions.Literal["name", ], str]):
-        return super().get_item_oapg(name)
-    
-
-    def __new__(
-        cls,
-        *_args: typing.Union[dict, frozendict.frozendict, ],
-        name: typing.Union[MetaOapg.properties.name, str, schemas.Unset] = schemas.unset,
-        _configuration: typing.Optional[schemas.Configuration] = None,
-        **kwargs: typing.Union[schemas.AnyTypeSchema, dict, frozendict.frozendict, str, date, datetime, uuid.UUID, int, float, decimal.Decimal, None, list, tuple, bytes],
-    ) -> 'UsageDTO':
-        return super().__new__(
-            cls,
-            *_args,
-            name=name,
-            _configuration=_configuration,
-            **kwargs,
-        )
```

### Comparing `songtradr-api-client-python-0.0.1/songtradr_api_client_python.egg-info/PKG-INFO` & `songtradr-api-client-python-1.12.21/test/test_allowed_values_api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,55 @@
-Metadata-Version: 2.1
-Name: songtradr-api-client-python
-Version: 0.0.1
-Summary: Songtradr API
-Home-page: 
-Author: Songtradr Inc.
-Author-email: info@songtradr.com
-Keywords: OpenAPI,OpenAPI-Generator,Songtradr API
-Requires-Python: >=3.7
+# coding: utf-8
 
-    This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world&#x27;s released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
-    
+"""
+    Songtradr API
+
+    This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
+
+    The version of the OpenAPI document: 1.12.21
+    Contact: info@songtradr.com
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
+"""
+
+
+import unittest
+
+import songtradr_api_client_python
+from songtradr_api_client_python.api.allowed_values_api import AllowedValuesApi  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
+
+
+class TestAllowedValuesApi(unittest.TestCase):
+    """AllowedValuesApi unit test stubs"""
+
+    def setUp(self):
+        self.api = songtradr_api_client_python.api.allowed_values_api.AllowedValuesApi()  # noqa: E501
+
+    def tearDown(self):
+        pass
+
+    def test_allowed_musical_features(self):
+        """Test case for allowed_musical_features
+
+        Allowed values for music descriptive parameters to be used in the searchAll endpoint.  # noqa: E501
+        """
+        pass
+
+    def test_genres(self):
+        """Test case for genres
+
+        Allowed values for genres.  # noqa: E501
+        """
+        pass
+
+    def test_tags(self):
+        """Test case for tags
+
+        All descriptive tags inside of tag-categories.  # noqa: E501
+        """
+        pass
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_category_medium_dto.py` & `songtradr-api-client-python-1.12.21/test/test_genre_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,24 +3,56 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.category_medium_dto import CategoryMediumDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.genre_dto import GenreDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestGenreDTO(unittest.TestCase):
+    """GenreDTO unit test stubs"""
 
-class TestCategoryMediumDTO(unittest.TestCase):
-    """CategoryMediumDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test GenreDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `GenreDTO`
+        """
+        model = songtradr_api_client_python.models.genre_dto.GenreDTO()  # noqa: E501
+        if include_optional :
+            return GenreDTO(
+                id = 56, 
+                name = ''
+            )
+        else :
+            return GenreDTO(
+                id = 56,
+                name = '',
+        )
+        """
+
+    def testGenreDTO(self):
+        """Test GenreDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_category_minimal_dto.py` & `songtradr-api-client-python-1.12.21/test/test_tag_small_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,24 +3,56 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.category_minimal_dto import CategoryMinimalDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.tag_small_dto import TagSmallDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestTagSmallDTO(unittest.TestCase):
+    """TagSmallDTO unit test stubs"""
 
-class TestCategoryMinimalDTO(unittest.TestCase):
-    """CategoryMinimalDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test TagSmallDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `TagSmallDTO`
+        """
+        model = songtradr_api_client_python.models.tag_small_dto.TagSmallDTO()  # noqa: E501
+        if include_optional :
+            return TagSmallDTO(
+                id = 56, 
+                name = ''
+            )
+        else :
+            return TagSmallDTO(
+                id = 56,
+                name = '',
+        )
+        """
+
+    def testTagSmallDTO(self):
+        """Test TagSmallDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_config_access_dto.py` & `songtradr-api-client-python-1.12.21/test/test_p_line_dto.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,24 +3,55 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.config_access_dto import ConfigAccessDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.p_line_dto import PLineDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestPLineDTO(unittest.TestCase):
+    """PLineDTO unit test stubs"""
 
-class TestConfigAccessDTO(unittest.TestCase):
-    """ConfigAccessDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test PLineDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `PLineDTO`
+        """
+        model = songtradr_api_client_python.models.p_line_dto.PLineDTO()  # noqa: E501
+        if include_optional :
+            return PLineDTO(
+                year = 56, 
+                text = ''
+            )
+        else :
+            return PLineDTO(
+                text = '',
+        )
+        """
+
+    def testPLineDTO(self):
+        """Test PLineDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_config_identifier_dto.py` & `songtradr-api-client-python-1.12.21/test/test_token_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,24 +3,54 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.config_identifier_dto import ConfigIdentifierDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.token_request import TokenRequest  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestTokenRequest(unittest.TestCase):
+    """TokenRequest unit test stubs"""
 
-class TestConfigIdentifierDTO(unittest.TestCase):
-    """ConfigIdentifierDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test TokenRequest
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `TokenRequest`
+        """
+        model = songtradr_api_client_python.models.token_request.TokenRequest()  # noqa: E501
+        if include_optional :
+            return TokenRequest(
+                refresh_token = ''
+            )
+        else :
+            return TokenRequest(
+                refresh_token = '',
+        )
+        """
+
+    def testTokenRequest(self):
+        """Test TokenRequest"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_contributor_type_dto.py` & `songtradr-api-client-python-1.12.21/test/test_sign_up_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,24 +3,59 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.contributor_type_dto import ContributorTypeDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.sign_up_dto import SignUpDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestSignUpDTO(unittest.TestCase):
+    """SignUpDTO unit test stubs"""
 
-class TestContributorTypeDTO(unittest.TestCase):
-    """ContributorTypeDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test SignUpDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `SignUpDTO`
+        """
+        model = songtradr_api_client_python.models.sign_up_dto.SignUpDTO()  # noqa: E501
+        if include_optional :
+            return SignUpDTO(
+                email_address = '', 
+                password = '', 
+                full_name = '', 
+                company_name = ''
+            )
+        else :
+            return SignUpDTO(
+                email_address = '',
+                password = '',
+                full_name = '',
+        )
+        """
+
+    def testSignUpDTO(self):
+        """Test SignUpDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_error_response.py` & `songtradr-api-client-python-1.12.21/test/test_party_large_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,24 +3,61 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.error_response import ErrorResponse
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.party_large_dto import PartyLargeDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestPartyLargeDTO(unittest.TestCase):
+    """PartyLargeDTO unit test stubs"""
 
-class TestErrorResponse(unittest.TestCase):
-    """ErrorResponse unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test PartyLargeDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `PartyLargeDTO`
+        """
+        model = songtradr_api_client_python.models.party_large_dto.PartyLargeDTO()  # noqa: E501
+        if include_optional :
+            return PartyLargeDTO(
+                full_name = '', 
+                birth_date = '', 
+                death_date = '', 
+                birth_year = '', 
+                death_year = '', 
+                birth_place = '', 
+                musicbrainz_type = '', 
+                area = ''
+            )
+        else :
+            return PartyLargeDTO(
+                full_name = '',
+        )
+        """
+
+    def testPartyLargeDTO(self):
+        """Test PartyLargeDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_field_summary_dto.py` & `songtradr-api-client-python-1.12.21/test/test_save_recording_genre_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,24 +3,56 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.field_summary_dto import FieldSummaryDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.save_recording_genre_dto import SaveRecordingGenreDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestSaveRecordingGenreDTO(unittest.TestCase):
+    """SaveRecordingGenreDTO unit test stubs"""
 
-class TestFieldSummaryDTO(unittest.TestCase):
-    """FieldSummaryDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test SaveRecordingGenreDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `SaveRecordingGenreDTO`
+        """
+        model = songtradr_api_client_python.models.save_recording_genre_dto.SaveRecordingGenreDTO()  # noqa: E501
+        if include_optional :
+            return SaveRecordingGenreDTO(
+                genre_name = '', 
+                genre_type = '', 
+                affinity = 1.337
+            )
+        else :
+            return SaveRecordingGenreDTO(
+                genre_name = '',
+        )
+        """
+
+    def testSaveRecordingGenreDTO(self):
+        """Test SaveRecordingGenreDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_file_dto.py` & `songtradr-api-client-python-1.12.21/test/test_config_access_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,24 +3,56 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.file_dto import FileDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.config_access_dto import ConfigAccessDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestConfigAccessDTO(unittest.TestCase):
+    """ConfigAccessDTO unit test stubs"""
 
-class TestFileDTO(unittest.TestCase):
-    """FileDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test ConfigAccessDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ConfigAccessDTO`
+        """
+        model = songtradr_api_client_python.models.config_access_dto.ConfigAccessDTO()  # noqa: E501
+        if include_optional :
+            return ConfigAccessDTO(
+                accessor_id = 'full', 
+                rights = 'full'
+            )
+        else :
+            return ConfigAccessDTO(
+                accessor_id = 'full',
+                rights = 'full',
+        )
+        """
+
+    def testConfigAccessDTO(self):
+        """Test ConfigAccessDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_file_list_dto.py` & `songtradr-api-client-python-1.12.21/test/test_search_recording_granular_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,24 +3,55 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.file_list_dto import FileListDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.search_recording_granular_dto import SearchRecordingGranularDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestSearchRecordingGranularDTO(unittest.TestCase):
+    """SearchRecordingGranularDTO unit test stubs"""
 
-class TestFileListDTO(unittest.TestCase):
-    """FileListDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test SearchRecordingGranularDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `SearchRecordingGranularDTO`
+        """
+        model = songtradr_api_client_python.models.search_recording_granular_dto.SearchRecordingGranularDTO()  # noqa: E501
+        if include_optional :
+            return SearchRecordingGranularDTO(
+                strength = 1.337, 
+                tag_name = ''
+            )
+        else :
+            return SearchRecordingGranularDTO(
+                tag_name = '',
+        )
+        """
+
+    def testSearchRecordingGranularDTO(self):
+        """Test SearchRecordingGranularDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_file_minimal_with_url_dto.py` & `songtradr-api-client-python-1.12.21/test/test_file_minimal_with_url_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,24 +3,58 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.file_minimal_with_url_dto import FileMinimalWithUrlDTO
-from songtradr_api_client_python import configuration
-
+from songtradr_api_client_python.models.file_minimal_with_url_dto import FileMinimalWithUrlDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
 class TestFileMinimalWithUrlDTO(unittest.TestCase):
     """FileMinimalWithUrlDTO unit test stubs"""
-    _configuration = configuration.Configuration()
 
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test FileMinimalWithUrlDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `FileMinimalWithUrlDTO`
+        """
+        model = songtradr_api_client_python.models.file_minimal_with_url_dto.FileMinimalWithUrlDTO()  # noqa: E501
+        if include_optional :
+            return FileMinimalWithUrlDTO(
+                file_name = '', 
+                url = '', 
+                isrc = ''
+            )
+        else :
+            return FileMinimalWithUrlDTO(
+                file_name = '',
+                url = '',
+                isrc = '',
+        )
+        """
+
+    def testFileMinimalWithUrlDTO(self):
+        """Test FileMinimalWithUrlDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_file_small_dto.py` & `songtradr-api-client-python-1.12.21/test/test_party_small_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,24 +3,56 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.file_small_dto import FileSmallDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.party_small_dto import PartySmallDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestPartySmallDTO(unittest.TestCase):
+    """PartySmallDTO unit test stubs"""
 
-class TestFileSmallDTO(unittest.TestCase):
-    """FileSmallDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test PartySmallDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `PartySmallDTO`
+        """
+        model = songtradr_api_client_python.models.party_small_dto.PartySmallDTO()  # noqa: E501
+        if include_optional :
+            return PartySmallDTO(
+                id = '', 
+                full_name = ''
+            )
+        else :
+            return PartySmallDTO(
+                id = '',
+                full_name = '',
+        )
+        """
+
+    def testPartySmallDTO(self):
+        """Test PartySmallDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_file_upload_dto.py` & `songtradr-api-client-python-1.12.21/test/test_save_recording_tag_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,24 +3,55 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.file_upload_dto import FileUploadDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.save_recording_tag_dto import SaveRecordingTagDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestSaveRecordingTagDTO(unittest.TestCase):
+    """SaveRecordingTagDTO unit test stubs"""
 
-class TestFileUploadDTO(unittest.TestCase):
-    """FileUploadDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test SaveRecordingTagDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `SaveRecordingTagDTO`
+        """
+        model = songtradr_api_client_python.models.save_recording_tag_dto.SaveRecordingTagDTO()  # noqa: E501
+        if include_optional :
+            return SaveRecordingTagDTO(
+                tag_name = '', 
+                affinity = 1.337
+            )
+        else :
+            return SaveRecordingTagDTO(
+                tag_name = '',
+        )
+        """
+
+    def testSaveRecordingTagDTO(self):
+        """Test SaveRecordingTagDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_file_w_ith_url_dto.py` & `songtradr-api-client-python-1.12.21/test/test_jwt_token_dto.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,24 +3,57 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.file_w_ith_url_dto import FileWIthUrlDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.jwt_token_dto import JwtTokenDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestJwtTokenDTO(unittest.TestCase):
+    """JwtTokenDTO unit test stubs"""
 
-class TestFileWIthUrlDTO(unittest.TestCase):
-    """FileWIthUrlDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test JwtTokenDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `JwtTokenDTO`
+        """
+        model = songtradr_api_client_python.models.jwt_token_dto.JwtTokenDTO()  # noqa: E501
+        if include_optional :
+            return JwtTokenDTO(
+                jwt_token = '', 
+                expiration_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                refresh_token = ''
+            )
+        else :
+            return JwtTokenDTO(
+                jwt_token = '',
+                expiration_date = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+        )
+        """
+
+    def testJwtTokenDTO(self):
+        """Test JwtTokenDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_files_summary_dto.py` & `songtradr-api-client-python-1.12.21/test/test_update_password_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,24 +3,56 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.files_summary_dto import FilesSummaryDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.update_password_dto import UpdatePasswordDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestUpdatePasswordDTO(unittest.TestCase):
+    """UpdatePasswordDTO unit test stubs"""
 
-class TestFilesSummaryDTO(unittest.TestCase):
-    """FilesSummaryDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test UpdatePasswordDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `UpdatePasswordDTO`
+        """
+        model = songtradr_api_client_python.models.update_password_dto.UpdatePasswordDTO()  # noqa: E501
+        if include_optional :
+            return UpdatePasswordDTO(
+                token = '', 
+                password = ''
+            )
+        else :
+            return UpdatePasswordDTO(
+                token = '',
+                password = '',
+        )
+        """
+
+    def testUpdatePasswordDTO(self):
+        """Test UpdatePasswordDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_forgot_password_dto.py` & `songtradr-api-client-python-1.12.21/test/test_save_recording_party_dto.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,24 +3,56 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.forgot_password_dto import ForgotPasswordDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.save_recording_party_dto import SaveRecordingPartyDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestSaveRecordingPartyDTO(unittest.TestCase):
+    """SaveRecordingPartyDTO unit test stubs"""
 
-class TestForgotPasswordDTO(unittest.TestCase):
-    """ForgotPasswordDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test SaveRecordingPartyDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `SaveRecordingPartyDTO`
+        """
+        model = songtradr_api_client_python.models.save_recording_party_dto.SaveRecordingPartyDTO()  # noqa: E501
+        if include_optional :
+            return SaveRecordingPartyDTO(
+                full_name = '', 
+                contributor_type = 'trackArtist'
+            )
+        else :
+            return SaveRecordingPartyDTO(
+                full_name = '',
+                contributor_type = 'trackArtist',
+        )
+        """
+
+    def testSaveRecordingPartyDTO(self):
+        """Test SaveRecordingPartyDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_genre_dto.py` & `songtradr-api-client-python-1.12.21/test/test_title_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,24 +3,54 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.genre_dto import GenreDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.title_dto import TitleDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestTitleDTO(unittest.TestCase):
+    """TitleDTO unit test stubs"""
 
-class TestGenreDTO(unittest.TestCase):
-    """GenreDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test TitleDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `TitleDTO`
+        """
+        model = songtradr_api_client_python.models.title_dto.TitleDTO()  # noqa: E501
+        if include_optional :
+            return TitleDTO(
+                title_text = ''
+            )
+        else :
+            return TitleDTO(
+                title_text = '',
+        )
+        """
+
+    def testTitleDTO(self):
+        """Test TitleDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_genre_minimal_dto.py` & `songtradr-api-client-python-1.12.21/test/test_genre_minimal_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,24 +3,54 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.genre_minimal_dto import GenreMinimalDTO
-from songtradr_api_client_python import configuration
-
+from songtradr_api_client_python.models.genre_minimal_dto import GenreMinimalDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
 class TestGenreMinimalDTO(unittest.TestCase):
     """GenreMinimalDTO unit test stubs"""
-    _configuration = configuration.Configuration()
 
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test GenreMinimalDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `GenreMinimalDTO`
+        """
+        model = songtradr_api_client_python.models.genre_minimal_dto.GenreMinimalDTO()  # noqa: E501
+        if include_optional :
+            return GenreMinimalDTO(
+                genre_name = ''
+            )
+        else :
+            return GenreMinimalDTO(
+                genre_name = '',
+        )
+        """
+
+    def testGenreMinimalDTO(self):
+        """Test GenreMinimalDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_genres_summary_dto.py` & `songtradr-api-client-python-1.12.21/test/test_contributor_type_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,54 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.genres_summary_dto import GenresSummaryDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.contributor_type_dto import ContributorTypeDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestContributorTypeDTO(unittest.TestCase):
+    """ContributorTypeDTO unit test stubs"""
 
-class TestGenresSummaryDTO(unittest.TestCase):
-    """GenresSummaryDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test ContributorTypeDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ContributorTypeDTO`
+        """
+        model = songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO()  # noqa: E501
+        if include_optional :
+            return ContributorTypeDTO(
+                type_name = ''
+            )
+        else :
+            return ContributorTypeDTO(
+                type_name = '',
+        )
+        """
+
+    def testContributorTypeDTO(self):
+        """Test ContributorTypeDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_init_put_recording_audio_dto.py` & `songtradr-api-client-python-1.12.21/test/test_save_recording_playlist_dto.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,24 +3,57 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.init_put_recording_audio_dto import InitPutRecordingAudioDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.save_recording_playlist_dto import SaveRecordingPlaylistDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestSaveRecordingPlaylistDTO(unittest.TestCase):
+    """SaveRecordingPlaylistDTO unit test stubs"""
 
-class TestInitPutRecordingAudioDTO(unittest.TestCase):
-    """InitPutRecordingAudioDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test SaveRecordingPlaylistDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `SaveRecordingPlaylistDTO`
+        """
+        model = songtradr_api_client_python.models.save_recording_playlist_dto.SaveRecordingPlaylistDTO()  # noqa: E501
+        if include_optional :
+            return SaveRecordingPlaylistDTO(
+                songtradr_track_guid = '', 
+                assigned_by_id = 56, 
+                sequence = 56
+            )
+        else :
+            return SaveRecordingPlaylistDTO(
+                songtradr_track_guid = '',
+                assigned_by_id = 56,
+        )
+        """
+
+    def testSaveRecordingPlaylistDTO(self):
+        """Test SaveRecordingPlaylistDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_jwt_token_dto.py` & `songtradr-api-client-python-1.12.21/test/test_login_dto.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,24 +3,58 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.jwt_token_dto import JwtTokenDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.login_dto import LoginDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestLoginDTO(unittest.TestCase):
+    """LoginDTO unit test stubs"""
 
-class TestJwtTokenDTO(unittest.TestCase):
-    """JwtTokenDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test LoginDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `LoginDTO`
+        """
+        model = songtradr_api_client_python.models.login_dto.LoginDTO()  # noqa: E501
+        if include_optional :
+            return LoginDTO(
+                username = '', 
+                version = '', 
+                email = '', 
+                password = ''
+            )
+        else :
+            return LoginDTO(
+                email = '',
+                password = '',
+        )
+        """
+
+    def testLoginDTO(self):
+        """Test LoginDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_login_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/usage_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,69 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
-"""
-
-import unittest
-
-import songtradr_api_client_python
-from songtradr_api_client_python.model.login_dto import LoginDTO
-from songtradr_api_client_python import configuration
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
 
+    Do not edit the class manually.
+"""
 
-class TestLoginDTO(unittest.TestCase):
-    """LoginDTO unit test stubs"""
-    _configuration = configuration.Configuration()
 
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
+
+
+from typing import Optional
+from pydantic import BaseModel, StrictStr
+
+class UsageDTO(BaseModel):
+    """
+    Details on a track's or playlist's usage permissions.
+    """
+    name: Optional[StrictStr] = None
+    __properties = ["name"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> UsageDTO:
+        """Create an instance of UsageDTO from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> UsageDTO:
+        """Create an instance of UsageDTO from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return UsageDTO.parse_obj(obj)
+
+        _obj = UsageDTO.parse_obj({
+            "name": obj.get("name")
+        })
+        return _obj
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_musical_features_dto.py` & `songtradr-api-client-python-1.12.21/test/test_save_referrer_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,54 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.musical_features_dto import MusicalFeaturesDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.save_referrer_dto import SaveReferrerDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestSaveReferrerDTO(unittest.TestCase):
+    """SaveReferrerDTO unit test stubs"""
 
-class TestMusicalFeaturesDTO(unittest.TestCase):
-    """MusicalFeaturesDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test SaveReferrerDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `SaveReferrerDTO`
+        """
+        model = songtradr_api_client_python.models.save_referrer_dto.SaveReferrerDTO()  # noqa: E501
+        if include_optional :
+            return SaveReferrerDTO(
+                username = '', 
+                url = ''
+            )
+        else :
+            return SaveReferrerDTO(
+        )
+        """
+
+    def testSaveReferrerDTO(self):
+        """Test SaveReferrerDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_p_line_dto.py` & `songtradr-api-client-python-1.12.21/test/test_recording_party_dto.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,24 +3,62 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.p_line_dto import PLineDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.recording_party_dto import RecordingPartyDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestRecordingPartyDTO(unittest.TestCase):
+    """RecordingPartyDTO unit test stubs"""
 
-class TestPLineDTO(unittest.TestCase):
-    """PLineDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test RecordingPartyDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `RecordingPartyDTO`
+        """
+        model = songtradr_api_client_python.models.recording_party_dto.RecordingPartyDTO()  # noqa: E501
+        if include_optional :
+            return RecordingPartyDTO(
+                contributor_types = [
+                    songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                        type_name = '', )
+                    ], 
+                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                    id = '', 
+                    full_name = '', )
+            )
+        else :
+            return RecordingPartyDTO(
+                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                    id = '', 
+                    full_name = '', ),
+        )
+        """
+
+    def testRecordingPartyDTO(self):
+        """Test RecordingPartyDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_party_small_dto.py` & `songtradr-api-client-python-1.12.21/test/test_config_identifier_dto.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,24 +3,56 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.party_small_dto import PartySmallDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.config_identifier_dto import ConfigIdentifierDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestConfigIdentifierDTO(unittest.TestCase):
+    """ConfigIdentifierDTO unit test stubs"""
 
-class TestPartySmallDTO(unittest.TestCase):
-    """PartySmallDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test ConfigIdentifierDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ConfigIdentifierDTO`
+        """
+        model = songtradr_api_client_python.models.config_identifier_dto.ConfigIdentifierDTO()  # noqa: E501
+        if include_optional :
+            return ConfigIdentifierDTO(
+                identifier_type = '', 
+                identifier_value = ''
+            )
+        else :
+            return ConfigIdentifierDTO(
+                identifier_type = '',
+                identifier_value = '',
+        )
+        """
+
+    def testConfigIdentifierDTO(self):
+        """Test ConfigIdentifierDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_product_medium_dto.py` & `songtradr-api-client-python-1.12.21/test/test_tags_summary_dto.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,24 +3,60 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.product_medium_dto import ProductMediumDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.tags_summary_dto import TagsSummaryDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestTagsSummaryDTO(unittest.TestCase):
+    """TagsSummaryDTO unit test stubs"""
 
-class TestProductMediumDTO(unittest.TestCase):
-    """ProductMediumDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test TagsSummaryDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `TagsSummaryDTO`
+        """
+        model = songtradr_api_client_python.models.tags_summary_dto.TagsSummaryDTO()  # noqa: E501
+        if include_optional :
+            return TagsSummaryDTO(
+                name = '', 
+                categories = [
+                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                        category_name = '', )
+                    ], 
+                total = 56
+            )
+        else :
+            return TagsSummaryDTO(
+                name = '',
+                total = 56,
+        )
+        """
+
+    def testTagsSummaryDTO(self):
+        """Test TagsSummaryDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_recording_for_similarity_search_dto.py` & `songtradr-api-client-python-1.12.21/test/test_genres_summary_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,57 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.recording_for_similarity_search_dto import RecordingForSimilaritySearchDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.genres_summary_dto import GenresSummaryDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestGenresSummaryDTO(unittest.TestCase):
+    """GenresSummaryDTO unit test stubs"""
 
-class TestRecordingForSimilaritySearchDTO(unittest.TestCase):
-    """RecordingForSimilaritySearchDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test GenresSummaryDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `GenresSummaryDTO`
+        """
+        model = songtradr_api_client_python.models.genres_summary_dto.GenresSummaryDTO()  # noqa: E501
+        if include_optional :
+            return GenresSummaryDTO(
+                name = '', 
+                total = 56, 
+                genre_type = ''
+            )
+        else :
+            return GenresSummaryDTO(
+                name = '',
+                total = 56,
+        )
+        """
+
+    def testGenresSummaryDTO(self):
+        """Test GenresSummaryDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_recording_genre_prediction_dto.py` & `songtradr-api-client-python-1.12.21/test/test_tag_dto.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,24 +3,60 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.recording_genre_prediction_dto import RecordingGenrePredictionDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.tag_dto import TagDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestTagDTO(unittest.TestCase):
+    """TagDTO unit test stubs"""
 
-class TestRecordingGenrePredictionDTO(unittest.TestCase):
-    """RecordingGenrePredictionDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test TagDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `TagDTO`
+        """
+        model = songtradr_api_client_python.models.tag_dto.TagDTO()  # noqa: E501
+        if include_optional :
+            return TagDTO(
+                id = 56, 
+                categories = [
+                    songtradr_api_client_python.models.category_minimal_dto.CategoryMinimalDTO(
+                        category_name = '', )
+                    ], 
+                name = ''
+            )
+        else :
+            return TagDTO(
+                id = 56,
+                name = '',
+        )
+        """
+
+    def testTagDTO(self):
+        """Test TagDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_recording_large_dto.py` & `songtradr-api-client-python-1.12.21/test/test_error_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,60 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.recording_large_dto import RecordingLargeDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.error_response import ErrorResponse  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestErrorResponse(unittest.TestCase):
+    """ErrorResponse unit test stubs"""
 
-class TestRecordingLargeDTO(unittest.TestCase):
-    """RecordingLargeDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test ErrorResponse
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ErrorResponse`
+        """
+        model = songtradr_api_client_python.models.error_response.ErrorResponse()  # noqa: E501
+        if include_optional :
+            return ErrorResponse(
+                timestamp = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                status = 56, 
+                error = '', 
+                message = '', 
+                path = ''
+            )
+        else :
+            return ErrorResponse(
+                timestamp = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                status = 56,
+                error = '',
+        )
+        """
+
+    def testErrorResponse(self):
+        """Test ErrorResponse"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_recording_medium_dto.py` & `songtradr-api-client-python-1.12.21/test/test_taggram_dto.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,24 +3,65 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.recording_medium_dto import RecordingMediumDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.taggram_dto import TaggramDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestTaggramDTO(unittest.TestCase):
+    """TaggramDTO unit test stubs"""
 
-class TestRecordingMediumDTO(unittest.TestCase):
-    """RecordingMediumDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test TaggramDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `TaggramDTO`
+        """
+        model = songtradr_api_client_python.models.taggram_dto.TaggramDTO()  # noqa: E501
+        if include_optional :
+            return TaggramDTO(
+                timeseries = [
+                    1.337
+                    ], 
+                category_name = '', 
+                tag_name = '', 
+                genre_name = '', 
+                scale = [
+                    56
+                    ]
+            )
+        else :
+            return TaggramDTO(
+                timeseries = [
+                    1.337
+                    ],
+                category_name = '',
+        )
+        """
+
+    def testTaggramDTO(self):
+        """Test TaggramDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_recording_minimal_with_taggrams_dto.py` & `songtradr-api-client-python-1.12.21/test/test_forgot_password_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,55 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.recording_minimal_with_taggrams_dto import RecordingMinimalWithTaggramsDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.forgot_password_dto import ForgotPasswordDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestForgotPasswordDTO(unittest.TestCase):
+    """ForgotPasswordDTO unit test stubs"""
 
-class TestRecordingMinimalWithTaggramsDTO(unittest.TestCase):
-    """RecordingMinimalWithTaggramsDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test ForgotPasswordDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ForgotPasswordDTO`
+        """
+        model = songtradr_api_client_python.models.forgot_password_dto.ForgotPasswordDTO()  # noqa: E501
+        if include_optional :
+            return ForgotPasswordDTO(
+                email_or_username = '', 
+                system = 'musicube'
+            )
+        else :
+            return ForgotPasswordDTO(
+                email_or_username = '',
+        )
+        """
+
+    def testForgotPasswordDTO(self):
+        """Test ForgotPasswordDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_save_recording_tag_dto.py` & `songtradr-api-client-python-1.12.21/test/test_category_medium_dto.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,24 +3,61 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.save_recording_tag_dto import SaveRecordingTagDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.category_medium_dto import CategoryMediumDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestCategoryMediumDTO(unittest.TestCase):
+    """CategoryMediumDTO unit test stubs"""
 
-class TestSaveRecordingTagDTO(unittest.TestCase):
-    """SaveRecordingTagDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test CategoryMediumDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `CategoryMediumDTO`
+        """
+        model = songtradr_api_client_python.models.category_medium_dto.CategoryMediumDTO()  # noqa: E501
+        if include_optional :
+            return CategoryMediumDTO(
+                id = 56, 
+                tags = [
+                    songtradr_api_client_python.models.tag_small_dto.TagSmallDTO(
+                        id = 56, 
+                        name = '', )
+                    ], 
+                name = ''
+            )
+        else :
+            return CategoryMediumDTO(
+                id = 56,
+                name = '',
+        )
+        """
+
+    def testCategoryMediumDTO(self):
+        """Test CategoryMediumDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_search_recording_granular_abstraction_dto.py` & `songtradr-api-client-python-1.12.21/test/test_search_recording_granular_abstraction_dto.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,24 +3,55 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.search_recording_granular_abstraction_dto import SearchRecordingGranularAbstractionDTO
-from songtradr_api_client_python import configuration
-
+from songtradr_api_client_python.models.search_recording_granular_abstraction_dto import SearchRecordingGranularAbstractionDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
 class TestSearchRecordingGranularAbstractionDTO(unittest.TestCase):
     """SearchRecordingGranularAbstractionDTO unit test stubs"""
-    _configuration = configuration.Configuration()
 
+    def setUp(self):
+        pass
+
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test SearchRecordingGranularAbstractionDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `SearchRecordingGranularAbstractionDTO`
+        """
+        model = songtradr_api_client_python.models.search_recording_granular_abstraction_dto.SearchRecordingGranularAbstractionDTO()  # noqa: E501
+        if include_optional :
+            return SearchRecordingGranularAbstractionDTO(
+                strength = 1.337, 
+                abstraction_name = 'brandarchetypeInnocent'
+            )
+        else :
+            return SearchRecordingGranularAbstractionDTO(
+                abstraction_name = 'brandarchetypeInnocent',
+        )
+        """
+
+    def testSearchRecordingGranularAbstractionDTO(self):
+        """Test SearchRecordingGranularAbstractionDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_search_recording_granular_dto.py` & `songtradr-api-client-python-1.12.21/songtradr_api_client_python/models/token_request.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,24 +3,69 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
-import unittest
 
-import songtradr_api_client_python
-from songtradr_api_client_python.model.search_recording_granular_dto import SearchRecordingGranularDTO
-from songtradr_api_client_python import configuration
+from __future__ import annotations
+import pprint
+import re  # noqa: F401
+import json
 
 
-class TestSearchRecordingGranularDTO(unittest.TestCase):
-    """SearchRecordingGranularDTO unit test stubs"""
-    _configuration = configuration.Configuration()
 
+from pydantic import BaseModel, Field, StrictStr
+
+class TokenRequest(BaseModel):
+    """
+    TokenRequest
+    """
+    refresh_token: StrictStr = Field(..., alias="refreshToken")
+    __properties = ["refreshToken"]
+
+    class Config:
+        """Pydantic configuration"""
+        allow_population_by_field_name = True
+        validate_assignment = True
+
+    def to_str(self) -> str:
+        """Returns the string representation of the model using alias"""
+        return pprint.pformat(self.dict(by_alias=True))
+
+    def to_json(self) -> str:
+        """Returns the JSON representation of the model using alias"""
+        return json.dumps(self.to_dict())
+
+    @classmethod
+    def from_json(cls, json_str: str) -> TokenRequest:
+        """Create an instance of TokenRequest from a JSON string"""
+        return cls.from_dict(json.loads(json_str))
+
+    def to_dict(self):
+        """Returns the dictionary representation of the model using alias"""
+        _dict = self.dict(by_alias=True,
+                          exclude={
+                          },
+                          exclude_none=True)
+        return _dict
+
+    @classmethod
+    def from_dict(cls, obj: dict) -> TokenRequest:
+        """Create an instance of TokenRequest from a dict"""
+        if obj is None:
+            return None
+
+        if not isinstance(obj, dict):
+            return TokenRequest.parse_obj(obj)
+
+        _obj = TokenRequest.parse_obj({
+            "refresh_token": obj.get("refreshToken")
+        })
+        return _obj
 
-if __name__ == '__main__':
-    unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_title_dto.py` & `songtradr-api-client-python-1.12.21/test/test_product_party_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,62 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.title_dto import TitleDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.product_party_dto import ProductPartyDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestProductPartyDTO(unittest.TestCase):
+    """ProductPartyDTO unit test stubs"""
 
-class TestTitleDTO(unittest.TestCase):
-    """TitleDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test ProductPartyDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `ProductPartyDTO`
+        """
+        model = songtradr_api_client_python.models.product_party_dto.ProductPartyDTO()  # noqa: E501
+        if include_optional :
+            return ProductPartyDTO(
+                contributor_types = [
+                    songtradr_api_client_python.models.contributor_type_dto.ContributorTypeDTO(
+                        type_name = '', )
+                    ], 
+                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                    id = '', 
+                    full_name = '', )
+            )
+        else :
+            return ProductPartyDTO(
+                party = songtradr_api_client_python.models.party_small_dto.PartySmallDTO(
+                    id = '', 
+                    full_name = '', ),
+        )
+        """
+
+    def testProductPartyDTO(self):
+        """Test ProductPartyDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_track_to_medium_product_dto.py` & `songtradr-api-client-python-1.12.21/test/test_field_summary_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,58 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.track_to_medium_product_dto import TrackToMediumProductDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.field_summary_dto import FieldSummaryDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestFieldSummaryDTO(unittest.TestCase):
+    """FieldSummaryDTO unit test stubs"""
 
-class TestTrackToMediumProductDTO(unittest.TestCase):
-    """TrackToMediumProductDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test FieldSummaryDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `FieldSummaryDTO`
+        """
+        model = songtradr_api_client_python.models.field_summary_dto.FieldSummaryDTO()  # noqa: E501
+        if include_optional :
+            return FieldSummaryDTO(
+                field_value = '', 
+                total = 56, 
+                field_name = ''
+            )
+        else :
+            return FieldSummaryDTO(
+                field_value = '',
+                total = 56,
+                field_name = '',
+        )
+        """
+
+    def testFieldSummaryDTO(self):
+        """Test FieldSummaryDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `songtradr-api-client-python-0.0.1/test/test_models/test_user_dto.py` & `songtradr-api-client-python-1.12.21/test/test_save_user_dto.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,59 @@
 """
     Songtradr API
 
     This is the Songtradr API. Use it to retrieve deep music metadata and trigger processes like auto-tagging.  You can also use the API to manage your account and musicube cloud data.  **Authentication**  1. Reach out to support@songtradr.com to receive a free account or use your login data if you are already signed up.  2. To authenticate, you need to login via the POST /api/v1/user/login endpoint.  3. The endpoint responds with a jwtToken which you can use in all following API requests as a bearer token.  **Rate Limiting**  The current limit is 120 Requests per minute. Reach out to us via support@songtradr.com if you need to request more.  **Getting Started with auto-tagging**  1. If you want to get your own files auto-tagged, use the POST /api/v1/user/file/{name}/initUpload endpoint. It responds with a presigned S3 link where you can upload your file. 2. You can check the processing status of your file via the GET /api/v1/user/file/{name}/filesStatus endpoint. 3. As soon as processing is done, you can request the generated data via the GET /api/v1/user/files endpoint.  **Getting Started with search**  You can either search the released music via the /public/recording endpoints or your own private uploaded music via the /user/file/ endpoints.  1. If you want to search the world's released music, a good starting point is the GET /api/v1/public/recording/search endpoint. Please find the extensive list of parameters that serve as semantic search filters. 2. If you want to search your own previously uploaded music, a good starting point is the GET GET /api/v1/user/files endpoint. It has the same extensive list of parameters that serve as semantic search filters.  # noqa: E501
 
     The version of the OpenAPI document: 1.12.21
     Contact: info@songtradr.com
-    Generated by: https://openapi-generator.tech
+    Generated by OpenAPI Generator (https://openapi-generator.tech)
+
+    Do not edit the class manually.
 """
 
+
 import unittest
+import datetime
 
 import songtradr_api_client_python
-from songtradr_api_client_python.model.user_dto import UserDTO
-from songtradr_api_client_python import configuration
+from songtradr_api_client_python.models.save_user_dto import SaveUserDTO  # noqa: E501
+from songtradr_api_client_python.rest import ApiException
 
+class TestSaveUserDTO(unittest.TestCase):
+    """SaveUserDTO unit test stubs"""
 
-class TestUserDTO(unittest.TestCase):
-    """UserDTO unit test stubs"""
-    _configuration = configuration.Configuration()
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
+
+    def make_instance(self, include_optional):
+        """Test SaveUserDTO
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # uncomment below to create an instance of `SaveUserDTO`
+        """
+        model = songtradr_api_client_python.models.save_user_dto.SaveUserDTO()  # noqa: E501
+        if include_optional :
+            return SaveUserDTO(
+                system = 'musicube', 
+                email_address = '', 
+                password = '', 
+                full_name = '', 
+                company_name = '', 
+                language = 'en'
+            )
+        else :
+            return SaveUserDTO(
+                email_address = '',
+        )
+        """
+
+    def testSaveUserDTO(self):
+        """Test SaveUserDTO"""
+        # inst_req_only = self.make_instance(include_optional=False)
+        # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

