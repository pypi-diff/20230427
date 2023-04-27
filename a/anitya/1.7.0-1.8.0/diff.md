# Comparing `tmp/anitya-1.7.0.tar.gz` & `tmp/anitya-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anitya-1.7.0.tar", max compression
+gzip compressed data, was "anitya-1.8.0.tar", max compression
```

## Comparing `anitya-1.7.0.tar` & `anitya-1.8.0.tar`

### file list

```diff
@@ -1,2085 +1,2085 @@
--rw-r--r--   0        0        0    18002 2020-12-02 09:02:04.975902 anitya-1.7.0/LICENSE
--rw-r--r--   0        0        0     1904 2022-06-22 14:20:39.926825 anitya-1.7.0/README.rst
--rw-r--r--   0        0        0     1184 2020-12-02 09:02:04.975902 anitya-1.7.0/alembic.ini
--rw-r--r--   0        0        0      124 2022-12-14 14:15:40.056732 anitya-1.7.0/anitya/__init__.py
--rw-r--r--   0        0        0    18452 2022-12-14 14:15:40.059732 anitya-1.7.0/anitya/admin.py
--rw-r--r--   0        0        0    15354 2020-12-16 13:18:27.985536 anitya-1.7.0/anitya/api.py
--rw-r--r--   0        0        0    31823 2022-12-14 14:15:40.062732 anitya-1.7.0/anitya/api_v2.py
--rw-r--r--   0        0        0     7621 2022-10-03 14:15:14.613326 anitya-1.7.0/anitya/app.py
--rw-r--r--   0        0        0     4450 2020-12-02 09:02:04.976902 anitya-1.7.0/anitya/authentication.py
--rw-r--r--   0        0        0    11976 2022-12-14 14:15:40.070732 anitya-1.7.0/anitya/check_service.py
--rw-r--r--   0        0        0     1113 2020-12-02 09:02:04.976902 anitya-1.7.0/anitya/compat.py
--rw-r--r--   0        0        0     5894 2022-12-14 14:15:40.074732 anitya-1.7.0/anitya/config.py
--rw-r--r--   0        0        0     1368 2020-12-02 09:02:04.976902 anitya-1.7.0/anitya/db/__init__.py
--rw-r--r--   0        0        0     3132 2020-12-02 09:02:04.976902 anitya-1.7.0/anitya/db/events.py
--rw-r--r--   0        0        0     5777 2020-12-02 09:02:04.976902 anitya-1.7.0/anitya/db/meta.py
--rw-r--r--   0        0        0      464 2020-12-02 09:02:04.976902 anitya-1.7.0/anitya/db/migrations/README.md
--rw-r--r--   0        0        0        0 2020-12-02 09:02:04.976902 anitya-1.7.0/anitya/db/migrations/__init__.py
--rw-r--r--   0        0        0     2106 2022-06-22 14:20:39.932825 anitya-1.7.0/anitya/db/migrations/env.py
--rw-r--r--   0        0        0      413 2020-12-02 09:02:04.976902 anitya-1.7.0/anitya/db/migrations/script.py.mako
--rw-r--r--   0        0        0      658 2020-12-02 09:02:04.976902 anitya-1.7.0/anitya/db/migrations/versions/136d119ab015_rename_project_latest_known_cursor_to_.py
--rw-r--r--   0        0        0      542 2020-12-02 09:02:04.976902 anitya-1.7.0/anitya/db/migrations/versions/16aa7da2764c_add_projectversion_commit_url.py
--rw-r--r--   0        0        0      592 2022-06-22 14:20:39.932825 anitya-1.7.0/anitya/db/migrations/versions/1ab95561edae_convert_date_to_rpm.py
--rw-r--r--   0        0        0     1391 2022-06-22 14:20:39.932825 anitya-1.7.0/anitya/db/migrations/versions/1bf8aead6179_add_check_times.py
--rw-r--r--   0        0        0      663 2022-06-22 14:20:39.932825 anitya-1.7.0/anitya/db/migrations/versions/1f839c54e428_add_archive_flag.py
--rw-r--r--   0        0        0      635 2022-06-22 14:20:39.932825 anitya-1.7.0/anitya/db/migrations/versions/24b6734e8565_creation_date_on_version.py
--rw-r--r--   0        0        0      747 2022-06-22 14:20:39.932825 anitya-1.7.0/anitya/db/migrations/versions/27342bce1d0f_populate_project_version_scheme.py
--rw-r--r--   0        0        0      591 2022-06-22 14:20:39.933825 anitya-1.7.0/anitya/db/migrations/versions/2925648d8cc3_add_a_version_prefix_field.py
--rw-r--r--   0        0        0      557 2021-03-18 13:23:05.984865 anitya-1.7.0/anitya/db/migrations/versions/2d1aa7ff82a5_remove_code_google_backend.py
--rw-r--r--   0        0        0      803 2022-06-22 14:20:39.933825 anitya-1.7.0/anitya/db/migrations/versions/314651690dc7_add_error_counter_to_project.py
--rw-r--r--   0        0        0     1810 2020-12-02 09:02:04.976902 anitya-1.7.0/anitya/db/migrations/versions/34b9bb5fa388_make_ecosystem_non_nullable.py
--rw-r--r--   0        0        0     3722 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/3fae8239eeec_add_an_api_token_table.py
--rw-r--r--   0        0        0      882 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/540bdcf7edbc_convert_github_url_to_owner_project.py
--rw-r--r--   0        0        0      676 2022-06-22 14:20:39.933825 anitya-1.7.0/anitya/db/migrations/versions/571bd07533a9_add_insecure_column_to_projects_table.py
--rw-r--r--   0        0        0      590 2022-06-22 14:20:39.933825 anitya-1.7.0/anitya/db/migrations/versions/5b8b587d7dbe_add_version_filter_column.py
--rw-r--r--   0        0        0      695 2022-06-22 14:20:39.934825 anitya-1.7.0/anitya/db/migrations/versions/5e209766aead_add_release_check_to_project.py
--rw-r--r--   0        0        0     1738 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/6ac0e42df937_drop_logs_table.py
--rw-r--r--   0        0        0      557 2022-06-22 14:20:39.934825 anitya-1.7.0/anitya/db/migrations/versions/708f6f26b4b6_add_version_pattern.py
--rw-r--r--   0        0        0     1023 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/7a8c4aa92678_add_missing_github_owner_project_pairs.py
--rw-r--r--   0        0        0      610 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/8040ef9a9dda_add_a_version_scheme_column_to_projects.py
--rw-r--r--   0        0        0      684 2021-02-12 16:21:32.439942 anitya-1.7.0/anitya/db/migrations/versions/8be6e153962c_remove_cursor.py
--rw-r--r--   0        0        0      970 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/921c612ba0da_model_upstream_ecosystems.py
--rw-r--r--   0        0        0      544 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/92a2e9eba0a7_add_project_latest_known_cursor.py
--rw-r--r--   0        0        0      928 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/9c29da0af3af_populate_ecosystem_data.py
--rw-r--r--   0        0        0        0 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/__init__.py
--rw-r--r--   0        0        0     3126 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/a52d2fe99d4f_users.py
--rw-r--r--   0        0        0      301 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/ac10bf3f974c_.py
--rw-r--r--   0        0        0      495 2022-06-22 14:20:39.934825 anitya-1.7.0/anitya/db/migrations/versions/b13662e5d288_add_admin_flag.py
--rw-r--r--   0        0        0     2881 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/b9201d816075_remove_the_backends_and_ecosystems_.py
--rw-r--r--   0        0        0      409 2022-06-22 14:20:39.934825 anitya-1.7.0/anitya/db/migrations/versions/c8735fa14a0a_add_cascade_delete.py
--rw-r--r--   0        0        0      596 2020-12-02 09:04:10.562083 anitya-1.7.0/anitya/db/migrations/versions/d6170cfc2814_add_pre_release_flag.py
--rw-r--r--   0        0        0     1148 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/e34988f3e2f4_add_statistics_to_run.py
--rw-r--r--   0        0        0     6582 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/db/migrations/versions/feeaa70ead67_social_authentication_table.py
--rw-r--r--   0        0        0    34852 2022-06-22 14:20:39.935825 anitya-1.7.0/anitya/db/models.py
--rw-r--r--   0        0        0     3507 2022-06-22 14:20:39.935825 anitya-1.7.0/anitya/forms.py
--rw-r--r--   0        0        0      152 2020-12-02 09:02:04.977902 anitya-1.7.0/anitya/lib/__init__.py
--rw-r--r--   0        0        0    15821 2022-12-14 14:15:40.080732 anitya-1.7.0/anitya/lib/backends/__init__.py
--rw-r--r--   0        0        0     2495 2022-12-14 14:15:40.080732 anitya-1.7.0/anitya/lib/backends/bitbucket.py
--rw-r--r--   0        0        0     2492 2022-12-14 14:15:40.081732 anitya-1.7.0/anitya/lib/backends/cgit.py
--rw-r--r--   0        0        0     3059 2022-12-14 14:15:40.082732 anitya-1.7.0/anitya/lib/backends/cpan.py
--rw-r--r--   0        0        0     7766 2020-12-16 13:18:27.989536 anitya-1.7.0/anitya/lib/backends/cran.py
--rw-r--r--   0        0        0     8182 2022-06-22 14:20:39.936825 anitya-1.7.0/anitya/lib/backends/crates.py
--rw-r--r--   0        0        0     2346 2022-12-14 14:15:40.082732 anitya-1.7.0/anitya/lib/backends/custom.py
--rw-r--r--   0        0        0     2460 2022-12-14 14:15:40.083732 anitya-1.7.0/anitya/lib/backends/debian.py
--rw-r--r--   0        0        0     2700 2022-12-14 14:15:40.083732 anitya-1.7.0/anitya/lib/backends/drupal6.py
--rw-r--r--   0        0        0     2700 2022-12-14 14:15:40.084732 anitya-1.7.0/anitya/lib/backends/drupal7.py
--rw-r--r--   0        0        0     2737 2022-12-14 14:15:40.084732 anitya-1.7.0/anitya/lib/backends/folder.py
--rw-r--r--   0        0        0     1947 2022-12-14 14:15:40.084732 anitya-1.7.0/anitya/lib/backends/freshmeat.py
--rw-r--r--   0        0        0     9388 2022-12-14 14:15:40.085732 anitya-1.7.0/anitya/lib/backends/github.py
--rw-r--r--   0        0        0     4313 2022-12-14 14:15:40.087732 anitya-1.7.0/anitya/lib/backends/gitlab.py
--rw-r--r--   0        0        0     3089 2022-12-14 14:15:40.087732 anitya-1.7.0/anitya/lib/backends/gnome.py
--rw-r--r--   0        0        0     2647 2022-12-14 14:15:40.088732 anitya-1.7.0/anitya/lib/backends/gnu.py
--rw-r--r--   0        0        0     2993 2022-12-14 14:15:40.088732 anitya-1.7.0/anitya/lib/backends/gogs.py
--rw-r--r--   0        0        0     2237 2022-12-14 14:15:40.089732 anitya-1.7.0/anitya/lib/backends/hackage.py
--rw-r--r--   0        0        0     1869 2022-12-14 14:15:40.089732 anitya-1.7.0/anitya/lib/backends/launchpad.py
--rw-r--r--   0        0        0     2631 2022-12-14 14:15:40.090732 anitya-1.7.0/anitya/lib/backends/maven.py
--rw-r--r--   0        0        0     5116 2020-12-16 13:18:27.990536 anitya-1.7.0/anitya/lib/backends/npmjs.py
--rw-r--r--   0        0        0     3263 2022-12-14 14:15:40.090732 anitya-1.7.0/anitya/lib/backends/packagist.py
--rw-r--r--   0        0        0     3121 2022-06-22 14:20:39.938825 anitya-1.7.0/anitya/lib/backends/pagure.py
--rw-r--r--   0        0        0     4418 2022-06-22 14:20:39.938825 anitya-1.7.0/anitya/lib/backends/pear.py
--rw-r--r--   0        0        0     4407 2022-06-22 14:20:39.938825 anitya-1.7.0/anitya/lib/backends/pecl.py
--rw-r--r--   0        0        0     5059 2022-12-14 14:15:40.091732 anitya-1.7.0/anitya/lib/backends/pypi.py
--rw-r--r--   0        0        0     3465 2022-12-14 14:15:40.091732 anitya-1.7.0/anitya/lib/backends/rubygems.py
--rw-r--r--   0        0        0     2066 2022-12-14 14:15:40.092732 anitya-1.7.0/anitya/lib/backends/sourceforge.py
--rw-r--r--   0        0        0     4289 2022-12-14 14:15:40.092732 anitya-1.7.0/anitya/lib/backends/sourceforge_git.py
--rw-r--r--   0        0        0     3524 2022-12-14 14:15:40.092732 anitya-1.7.0/anitya/lib/backends/sourcehut.py
--rw-r--r--   0        0        0     2030 2022-12-14 14:15:40.093732 anitya-1.7.0/anitya/lib/backends/stackage.py
--rw-r--r--   0        0        0     1086 2022-06-22 14:20:39.939825 anitya-1.7.0/anitya/lib/ecosystems/__init__.py
--rw-r--r--   0        0        0     1072 2022-06-22 14:20:39.939825 anitya-1.7.0/anitya/lib/ecosystems/crates.py
--rw-r--r--   0        0        0      278 2022-06-22 14:20:39.939825 anitya-1.7.0/anitya/lib/ecosystems/maven.py
--rw-r--r--   0        0        0      264 2022-06-22 14:20:39.939825 anitya-1.7.0/anitya/lib/ecosystems/npm.py
--rw-r--r--   0        0        0      266 2022-06-22 14:20:39.939825 anitya-1.7.0/anitya/lib/ecosystems/pypi.py
--rw-r--r--   0        0        0      282 2022-06-22 14:20:39.939825 anitya-1.7.0/anitya/lib/ecosystems/rubygems.py
--rw-r--r--   0        0        0     4084 2022-06-22 14:20:39.940825 anitya-1.7.0/anitya/lib/exceptions.py
--rw-r--r--   0        0        0     3430 2022-06-22 14:20:39.940825 anitya-1.7.0/anitya/lib/plugins.py
--rw-r--r--   0        0        0    18381 2022-12-14 14:15:40.100732 anitya-1.7.0/anitya/lib/utilities.py
--rw-r--r--   0        0        0     2186 2020-12-02 09:02:04.979902 anitya-1.7.0/anitya/lib/versions/__init__.py
--rw-r--r--   0        0        0     7346 2022-06-22 14:20:39.941825 anitya-1.7.0/anitya/lib/versions/base.py
--rw-r--r--   0        0        0    15319 2022-06-22 14:20:39.941825 anitya-1.7.0/anitya/lib/versions/calver.py
--rw-r--r--   0        0        0     3084 2022-12-14 14:15:40.101732 anitya-1.7.0/anitya/lib/versions/python.py
--rw-r--r--   0        0        0     7547 2022-12-14 14:15:40.103732 anitya-1.7.0/anitya/lib/versions/rpm.py
--rw-r--r--   0        0        0     3766 2020-12-02 09:04:10.567083 anitya-1.7.0/anitya/lib/versions/semver.py
--rw-r--r--   0        0        0     2824 2020-12-02 09:04:10.567083 anitya-1.7.0/anitya/lib/xml2dict.py
--rw-r--r--   0        0        0     7366 2022-12-14 14:15:40.104732 anitya-1.7.0/anitya/librariesio_consumer.py
--rw-r--r--   0        0        0     6251 2022-06-22 14:20:39.943825 anitya-1.7.0/anitya/mail_logging.py
--rw-r--r--   0        0        0     2946 2022-12-14 14:15:40.105732 anitya-1.7.0/anitya/sar.py
--rw-r--r--   0        0        0       54 2022-11-14 14:56:56.902921 anitya-1.7.0/anitya/static/css/avatars.css
--rw-r--r--   0        0        0      888 2022-11-14 14:57:00.636935 anitya-1.7.0/anitya/static/css/cnucnu.css
--rw-r--r--   0        0        0    24734 2022-11-14 14:57:06.871959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-Bold-webfont.eot
--rw-r--r--   0        0        0    28113 2022-11-14 14:57:06.871959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-Bold-webfont.svg
--rw-r--r--   0        0        0    49276 2022-11-14 14:57:06.872959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-Bold-webfont.ttf
--rw-r--r--   0        0        0    16708 2022-11-14 14:57:06.872959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-Bold-webfont.woff
--rw-r--r--   0        0        0    27450 2022-11-14 14:57:06.872959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.eot
--rw-r--r--   0        0        0    29130 2022-11-14 14:57:06.873959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.svg
--rw-r--r--   0        0        0    52200 2022-11-14 14:57:06.873959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.ttf
--rw-r--r--   0        0        0    17988 2022-11-14 14:57:06.873959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.woff
--rw-r--r--   0        0        0    27610 2022-11-14 14:57:06.873959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.eot
--rw-r--r--   0        0        0    29402 2022-11-14 14:57:06.874959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.svg
--rw-r--r--   0        0        0    50068 2022-11-14 14:57:06.874959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.ttf
--rw-r--r--   0        0        0    17980 2022-11-14 14:57:06.874959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.woff
--rw-r--r--   0        0        0    24350 2022-11-14 14:57:06.874959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-Regular-webfont.eot
--rw-r--r--   0        0        0    28095 2022-11-14 14:57:06.874959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-Regular-webfont.svg
--rw-r--r--   0        0        0    47504 2022-11-14 14:57:06.875959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-Regular-webfont.ttf
--rw-r--r--   0        0        0    16400 2022-11-14 14:57:06.875959 anitya-1.7.0/anitya/static/css/fonts/Cantarell-Regular-webfont.woff
--rw-r--r--   0        0        0    94588 2022-11-14 14:57:06.876959 anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.eot
--rw-r--r--   0        0        0   171329 2022-11-14 14:57:06.876959 anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.svg
--rw-r--r--   0        0        0   170608 2022-11-14 14:57:06.878960 anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.ttf
--rw-r--r--   0        0        0    56608 2022-11-14 14:57:06.878960 anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.woff
--rw-r--r--   0        0        0    91164 2022-11-14 14:57:06.878960 anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.eot
--rw-r--r--   0        0        0   169419 2022-11-14 14:57:06.879959 anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.svg
--rw-r--r--   0        0        0   170388 2022-11-14 14:57:06.880959 anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.ttf
--rw-r--r--   0        0        0    54684 2022-11-14 14:57:06.880959 anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.woff
--rw-r--r--   0        0        0    95020 2022-11-14 14:57:06.881960 anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.eot
--rw-r--r--   0        0        0   167898 2022-11-14 14:57:06.882959 anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.svg
--rw-r--r--   0        0        0   170308 2022-11-14 14:57:06.883959 anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.ttf
--rw-r--r--   0        0        0    56100 2022-11-14 14:57:06.883959 anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.woff
--rw-r--r--   0        0        0      279 2022-11-14 14:57:22.414019 anitya-1.7.0/anitya/static/css/footer.css
--rw-r--r--   0        0        0      212 2022-11-14 14:57:16.686997 anitya-1.7.0/anitya/static/css/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-r--r--   0        0        0      220 2022-11-14 14:57:16.686997 anitya-1.7.0/anitya/static/css/images/ui-bg_flat_0_eeeeee_40x100.png
--rw-r--r--   0        0        0      208 2022-11-14 14:57:16.686997 anitya-1.7.0/anitya/static/css/images/ui-bg_flat_55_ffffff_40x100.png
--rw-r--r--   0        0        0      208 2022-11-14 14:57:16.686997 anitya-1.7.0/anitya/static/css/images/ui-bg_flat_75_ffffff_40x100.png
--rw-r--r--   0        0        0      207 2022-11-14 14:57:16.686997 anitya-1.7.0/anitya/static/css/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0        0        0      277 2022-11-14 14:57:16.686997 anitya-1.7.0/anitya/static/css/images/ui-bg_highlight-soft_100_f6f6f6_1x100.png
--rw-r--r--   0        0        0      338 2022-11-14 14:57:16.687997 anitya-1.7.0/anitya/static/css/images/ui-bg_highlight-soft_25_0073ea_1x100.png
--rw-r--r--   0        0        0      280 2022-11-14 14:57:16.687997 anitya-1.7.0/anitya/static/css/images/ui-bg_highlight-soft_50_dddddd_1x100.png
--rw-r--r--   0        0        0     4549 2022-11-14 14:57:16.687997 anitya-1.7.0/anitya/static/css/images/ui-icons_0073ea_256x240.png
--rw-r--r--   0        0        0     6992 2022-11-14 14:57:16.687997 anitya-1.7.0/anitya/static/css/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     6988 2022-11-14 14:57:16.688997 anitya-1.7.0/anitya/static/css/images/ui-icons_666666_256x240.png
--rw-r--r--   0        0        0     4549 2022-11-14 14:57:16.688997 anitya-1.7.0/anitya/static/css/images/ui-icons_ff0084_256x240.png
--rw-r--r--   0        0        0     6299 2022-11-14 14:57:16.688997 anitya-1.7.0/anitya/static/css/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0      125 2022-11-14 14:57:29.052045 anitya-1.7.0/anitya/static/css/navbar.css
--rw-r--r--   0        0        0     2519 2022-11-14 14:57:32.802060 anitya-1.7.0/anitya/static/css/text.css
--rw-r--r--   0        0        0    33392 2021-01-15 12:47:19.805568 anitya-1.7.0/anitya/static/docs/_images/database.png
--rw-r--r--   0        0        0    13224 2021-01-15 12:47:19.813568 anitya-1.7.0/anitya/static/docs/_modules/anitya/db/events.html
--rw-r--r--   0        0        0    20589 2021-01-15 12:47:19.814568 anitya-1.7.0/anitya/static/docs/_modules/anitya/db/meta.html
--rw-r--r--   0        0        0   150267 2021-01-15 12:47:19.816568 anitya-1.7.0/anitya/static/docs/_modules/anitya/db/models.html
--rw-r--r--   0        0        0    52067 2021-01-15 12:47:19.818568 anitya-1.7.0/anitya/static/docs/_modules/anitya/lib/backends.html
--rw-r--r--   0        0        0     6469 2021-01-15 12:47:19.819568 anitya-1.7.0/anitya/static/docs/_modules/anitya/lib/ecosystems.html
--rw-r--r--   0        0        0    18072 2021-01-15 12:47:19.821568 anitya-1.7.0/anitya/static/docs/_modules/anitya/lib/exceptions.html
--rw-r--r--   0        0        0    15350 2021-01-15 12:47:19.822568 anitya-1.7.0/anitya/static/docs/_modules/anitya/lib/plugins.html
--rw-r--r--   0        0        0    26768 2021-01-15 12:47:19.824568 anitya-1.7.0/anitya/static/docs/_modules/anitya/lib/versions/base.html
--rw-r--r--   0        0        0     5081 2021-01-15 12:47:19.841568 anitya-1.7.0/anitya/static/docs/_modules/index.html
--rw-r--r--   0        0        0    76032 2021-01-15 12:47:19.827568 anitya-1.7.0/anitya/static/docs/_modules/sqlalchemy/ext/declarative/api.html
--rw-r--r--   0        0        0   245360 2021-01-15 12:47:19.830568 anitya-1.7.0/anitya/static/docs/_modules/sqlalchemy/orm/attributes.html
--rw-r--r--   0        0        0    23324 2021-01-15 12:47:19.832568 anitya-1.7.0/anitya/static/docs/_modules/sqlalchemy/orm/scoping.html
--rw-r--r--   0        0        0   500489 2021-01-15 12:47:19.837568 anitya-1.7.0/anitya/static/docs/_modules/sqlalchemy/sql/schema.html
--rw-r--r--   0        0        0   296008 2021-01-15 12:47:19.840568 anitya-1.7.0/anitya/static/docs/_modules/sqlalchemy/sql/sqltypes.html
--rw-r--r--   0        0        0     5095 2021-01-15 12:47:19.850568 anitya-1.7.0/anitya/static/docs/_sources/admin-guide.rst.txt
--rw-r--r--   0        0        0     8467 2021-01-15 12:47:19.851568 anitya-1.7.0/anitya/static/docs/_sources/admin-user-guide.rst.txt
--rw-r--r--   0        0        0     1756 2021-01-15 12:47:19.852568 anitya-1.7.0/anitya/static/docs/_sources/api.rst.txt
--rw-r--r--   0        0        0     9534 2021-01-15 12:47:19.853568 anitya-1.7.0/anitya/static/docs/_sources/contributing.rst.txt
--rw-r--r--   0        0        0      314 2021-01-15 12:47:19.854568 anitya-1.7.0/anitya/static/docs/_sources/database.rst.txt
--rw-r--r--   0        0        0      306 2021-01-15 12:47:19.856568 anitya-1.7.0/anitya/static/docs/_sources/docblocks/anitya.db.models.rst.txt
--rw-r--r--   0        0        0      510 2021-01-15 12:47:19.857568 anitya-1.7.0/anitya/static/docs/_sources/glossary.rst.txt
--rw-r--r--   0        0        0     1279 2021-01-15 12:47:19.858568 anitya-1.7.0/anitya/static/docs/_sources/index.rst.txt
--rw-r--r--   0        0        0     2624 2021-01-15 12:47:19.859568 anitya-1.7.0/anitya/static/docs/_sources/integrating-with-anitya.rst.txt
--rw-r--r--   0        0        0     2229 2020-12-02 12:47:56.984892 anitya-1.7.0/anitya/static/docs/_sources/release-monitoring-admin-guide.rst.txt
--rw-r--r--   0        0        0    23367 2021-01-15 12:47:19.860568 anitya-1.7.0/anitya/static/docs/_sources/release-notes.rst.txt
--rw-r--r--   0        0        0    19248 2021-01-15 12:47:19.861568 anitya-1.7.0/anitya/static/docs/_sources/user-guide.rst.txt
--rw-r--r--   0        0        0    11187 2021-01-15 12:47:19.881568 anitya-1.7.0/anitya/static/docs/_static/alabaster.css
--rw-r--r--   0        0        0    12171 2021-01-15 12:47:19.864568 anitya-1.7.0/anitya/static/docs/_static/basic.css
--rw-r--r--   0        0        0       42 2021-01-15 12:47:19.880568 anitya-1.7.0/anitya/static/docs/_static/custom.css
--rw-r--r--   0        0        0     9270 2021-01-15 12:47:19.874568 anitya-1.7.0/anitya/static/docs/_static/doctools.js
--rw-r--r--   0        0        0      307 2021-01-15 12:47:19.873568 anitya-1.7.0/anitya/static/docs/_static/documentation_options.js
--rw-r--r--   0        0        0      286 2021-01-15 12:47:19.866568 anitya-1.7.0/anitya/static/docs/_static/file.png
--rw-r--r--   0        0        0   280364 2021-01-15 12:47:19.884568 anitya-1.7.0/anitya/static/docs/_static/jquery-3.4.1.js
--rw-r--r--   0        0        0   287630 2021-01-15 12:47:19.871568 anitya-1.7.0/anitya/static/docs/_static/jquery-3.5.1.js
--rw-r--r--   0        0        0    88145 2021-01-15 12:47:19.868568 anitya-1.7.0/anitya/static/docs/_static/jquery.js
--rw-r--r--   0        0        0    10847 2021-01-15 12:47:19.879568 anitya-1.7.0/anitya/static/docs/_static/language_data.js
--rw-r--r--   0        0        0       90 2021-01-15 12:47:19.878568 anitya-1.7.0/anitya/static/docs/_static/minus.png
--rw-r--r--   0        0        0       90 2021-01-15 12:47:19.877568 anitya-1.7.0/anitya/static/docs/_static/plus.png
--rw-r--r--   0        0        0     4395 2021-01-15 12:47:19.863568 anitya-1.7.0/anitya/static/docs/_static/pygments.css
--rw-r--r--   0        0        0    15987 2021-01-15 12:47:19.875568 anitya-1.7.0/anitya/static/docs/_static/searchtools.js
--rw-r--r--   0        0        0    35168 2021-01-15 12:47:19.876568 anitya-1.7.0/anitya/static/docs/_static/underscore-1.3.1.js
--rw-r--r--   0        0        0    12140 2021-01-15 12:47:19.865568 anitya-1.7.0/anitya/static/docs/_static/underscore.js
--rw-r--r--   0        0        0    17984 2021-01-15 12:47:19.782568 anitya-1.7.0/anitya/static/docs/admin-guide.html
--rw-r--r--   0        0        0    19172 2021-01-15 12:47:19.785568 anitya-1.7.0/anitya/static/docs/admin-user-guide.html
--rw-r--r--   0        0        0   186318 2021-01-15 12:47:19.790568 anitya-1.7.0/anitya/static/docs/api.html
--rw-r--r--   0        0        0    24463 2021-01-15 12:47:19.792568 anitya-1.7.0/anitya/static/docs/contributing.html
--rw-r--r--   0        0        0     5793 2021-01-15 12:47:19.794568 anitya-1.7.0/anitya/static/docs/database.html
--rw-r--r--   0        0        0     6755 2021-01-15 12:47:19.797568 anitya-1.7.0/anitya/static/docs/docblocks/anitya.db.models.html
--rw-r--r--   0        0        0    21157 2021-01-15 12:47:19.799568 anitya-1.7.0/anitya/static/docs/genindex.html
--rw-r--r--   0        0        0     5045 2021-01-15 12:47:19.801568 anitya-1.7.0/anitya/static/docs/glossary.html
--rw-r--r--   0        0        0     9045 2021-01-15 12:47:19.803568 anitya-1.7.0/anitya/static/docs/http-routingtable.html
--rw-r--r--   0        0        0    13545 2021-01-15 12:47:19.807568 anitya-1.7.0/anitya/static/docs/index.html
--rw-r--r--   0        0        0     8658 2021-01-15 12:47:19.809568 anitya-1.7.0/anitya/static/docs/integrating-with-anitya.html
--rw-r--r--   0        0        0     1672 2021-01-15 12:47:19.842568 anitya-1.7.0/anitya/static/docs/objects.inv
--rw-r--r--   0        0        0     6028 2021-01-15 12:47:19.844568 anitya-1.7.0/anitya/static/docs/py-modindex.html
--rw-r--r--   0        0        0     8309 2020-12-02 12:47:56.964892 anitya-1.7.0/anitya/static/docs/release-monitoring-admin-guide.html
--rw-r--r--   0        0        0    48756 2021-01-15 12:47:19.846568 anitya-1.7.0/anitya/static/docs/release-notes.html
--rw-r--r--   0        0        0     4548 2021-01-15 12:47:19.847568 anitya-1.7.0/anitya/static/docs/search.html
--rw-r--r--   0        0        0    24161 2021-01-15 12:47:19.848568 anitya-1.7.0/anitya/static/docs/searchindex.js
--rw-r--r--   0        0        0    38361 2021-01-15 12:47:19.885568 anitya-1.7.0/anitya/static/docs/user-guide.html
--rw-r--r--   0        0        0     4683 2020-12-02 09:02:04.991902 anitya-1.7.0/anitya/static/google_logo.png
--rw-r--r--   0        0        0     5430 2022-11-14 16:27:56.526971 anitya-1.7.0/anitya/static/ico/favicon.ico
--rw-r--r--   0        0        0     4077 2022-11-14 14:58:19.913241 anitya-1.7.0/anitya/static/img/spinner.gif
--rw-r--r--   0        0        0     1957 2022-12-05 10:22:04.064212 anitya-1.7.0/anitya/static/node_modules/.package-lock.json
--rw-r--r--   0        0        0     1082 2022-11-14 15:08:03.408809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/LICENSE.md
--rw-r--r--   0        0        0    13561 2022-11-14 15:08:03.409809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/README.md
--rw-r--r--   0        0        0     2037 2022-11-14 15:08:03.426809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/enums.js
--rw-r--r--   0        0        0       45 2022-11-14 15:08:03.426809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/enums.js.flow
--rw-r--r--   0        0        0     4234 2022-11-14 15:08:03.427809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/enums.js.map
--rw-r--r--   0        0        0    36698 2022-11-14 15:08:03.428809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-base.js
--rw-r--r--   0        0        0       51 2022-11-14 15:08:03.429809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-base.js.flow
--rw-r--r--   0        0        0    87394 2022-11-14 15:08:03.433809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-base.js.map
--rw-r--r--   0        0        0    47193 2022-11-14 15:08:03.436809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js
--rw-r--r--   0        0        0       51 2022-11-14 15:08:03.437809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js.flow
--rw-r--r--   0        0        0   110974 2022-11-14 15:08:03.441809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js.map
--rw-r--r--   0        0        0    67554 2022-11-14 15:08:03.449809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper.js
--rw-r--r--   0        0        0       46 2022-11-14 15:08:03.450809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper.js.flow
--rw-r--r--   0        0        0   158154 2022-11-14 15:08:03.455809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper.js.map
--rw-r--r--   0        0        0    10007 2022-11-14 15:08:03.457809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/createPopper.js
--rw-r--r--   0        0        0      677 2022-11-14 15:08:03.578809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/contains.js
--rw-r--r--   0        0        0     1371 2022-11-14 15:08:03.579810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getBoundingClientRect.js
--rw-r--r--   0        0        0     3400 2022-11-14 15:08:03.579810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getClippingRect.js
--rw-r--r--   0        0        0     2072 2022-11-14 15:08:03.579810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getCompositeRect.js
--rw-r--r--   0        0        0      148 2022-11-14 15:08:03.579810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getComputedStyle.js
--rw-r--r--   0        0        0      311 2022-11-14 15:08:03.580809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getDocumentElement.js
--rw-r--r--   0        0        0     1227 2022-11-14 15:08:03.580809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getDocumentRect.js
--rw-r--r--   0        0        0      142 2022-11-14 15:08:03.580809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getHTMLElementScroll.js
--rw-r--r--   0        0        0      767 2022-11-14 15:08:03.581809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getLayoutRect.js
--rw-r--r--   0        0        0      114 2022-11-14 15:08:03.581809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getNodeName.js
--rw-r--r--   0        0        0      396 2022-11-14 15:08:03.581809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getNodeScroll.js
--rw-r--r--   0        0        0     2613 2022-11-14 15:08:03.582810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getOffsetParent.js
--rw-r--r--   0        0        0      759 2022-11-14 15:08:03.582810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getParentNode.js
--rw-r--r--   0        0        0      546 2022-11-14 15:08:03.582810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getScrollParent.js
--rw-r--r--   0        0        0      881 2022-11-14 15:08:03.583809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getViewportRect.js
--rw-r--r--   0        0        0      273 2022-11-14 15:08:03.583809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindow.js
--rw-r--r--   0        0        0      258 2022-11-14 15:08:03.583809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindowScroll.js
--rw-r--r--   0        0        0      721 2022-11-14 15:08:03.583809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindowScrollBarX.js
--rw-r--r--   0        0        0      621 2022-11-14 15:08:03.584809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/instanceOf.js
--rw-r--r--   0        0        0      159 2022-11-14 15:08:03.584809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/isLayoutViewport.js
--rw-r--r--   0        0        0      440 2022-11-14 15:08:03.584809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/isScrollParent.js
--rw-r--r--   0        0        0      162 2022-11-14 15:08:03.585809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/isTableElement.js
--rw-r--r--   0        0        0     1177 2022-11-14 15:08:03.585809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/listScrollParents.js
--rw-r--r--   0        0        0     1335 2022-11-14 15:08:03.457809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/enums.js
--rw-r--r--   0        0        0      443 2022-11-14 15:08:03.458809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/index.js
--rw-r--r--   0        0        0     2527 2022-11-14 15:08:03.586809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/applyStyles.js
--rw-r--r--   0        0        0     3878 2022-11-14 15:08:03.586809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/arrow.js
--rw-r--r--   0        0        0     6566 2022-11-14 15:08:03.587809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/computeStyles.js
--rw-r--r--   0        0        0     1330 2022-11-14 15:08:03.587809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/eventListeners.js
--rw-r--r--   0        0        0     4910 2022-11-14 15:08:03.587809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/flip.js
--rw-r--r--   0        0        0     1954 2022-11-14 15:08:03.588809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/hide.js
--rw-r--r--   0        0        0      502 2022-11-14 15:08:03.588809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/index.js
--rw-r--r--   0        0        0     1613 2022-11-14 15:08:03.589810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/offset.js
--rw-r--r--   0        0        0      706 2022-11-14 15:08:03.589810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/popperOffsets.js
--rw-r--r--   0        0        0     6585 2022-11-14 15:08:03.589810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/preventOverflow.js
--rw-r--r--   0        0        0      193 2022-11-14 15:08:03.458809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/popper-base.js
--rw-r--r--   0        0        0      603 2022-11-14 15:08:03.459809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/popper-lite.js
--rw-r--r--   0        0        0     1090 2022-11-14 15:08:03.459809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/popper.js
--rw-r--r--   0        0        0        0 2022-11-14 15:08:03.459809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/types.js
--rw-r--r--   0        0        0     1991 2022-11-14 15:08:03.590809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/computeAutoPlacement.js
--rw-r--r--   0        0        0     1738 2022-11-14 15:08:03.591809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/computeOffsets.js
--rw-r--r--   0        0        0      302 2022-11-14 15:08:03.591809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/debounce.js
--rw-r--r--   0        0        0     3528 2022-11-14 15:08:03.591809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/detectOverflow.js
--rw-r--r--   0        0        0      159 2022-11-14 15:08:03.592810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/expandToHashMap.js
--rw-r--r--   0        0        0      286 2022-11-14 15:08:03.592810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/format.js
--rw-r--r--   0        0        0       79 2022-11-14 15:08:03.592810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getAltAxis.js
--rw-r--r--   0        0        0       89 2022-11-14 15:08:03.592810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getAltLen.js
--rw-r--r--   0        0        0      125 2022-11-14 15:08:03.593809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getBasePlacement.js
--rw-r--r--   0        0        0      117 2022-11-14 15:08:03.593809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getFreshSideObject.js
--rw-r--r--   0        0        0      127 2022-11-14 15:08:03.593809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getMainAxisFromPlacement.js
--rw-r--r--   0        0        0      248 2022-11-14 15:08:03.594809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getOppositePlacement.js
--rw-r--r--   0        0        0      209 2022-11-14 15:08:03.594809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getOppositeVariationPlacement.js
--rw-r--r--   0        0        0       85 2022-11-14 15:08:03.594809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getVariation.js
--rw-r--r--   0        0        0       84 2022-11-14 15:08:03.595810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/math.js
--rw-r--r--   0        0        0      524 2022-11-14 15:08:03.595810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/mergeByName.js
--rw-r--r--   0        0        0      184 2022-11-14 15:08:03.595810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/mergePaddingObject.js
--rw-r--r--   0        0        0     1240 2022-11-14 15:08:03.596809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/orderModifiers.js
--rw-r--r--   0        0        0      191 2022-11-14 15:08:03.596809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/rectToClientRect.js
--rw-r--r--   0        0        0      252 2022-11-14 15:08:03.597809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/uniqueBy.js
--rw-r--r--   0        0        0      269 2022-11-14 15:08:03.597809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/userAgent.js
--rw-r--r--   0        0        0     3261 2022-11-14 15:08:03.597809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/validateModifiers.js
--rw-r--r--   0        0        0      262 2022-11-14 15:08:03.597809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/within.js
--rw-r--r--   0        0        0     2479 2022-11-14 15:08:03.461809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.js
--rw-r--r--   0        0        0     4240 2022-11-14 15:08:03.461809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.js.map
--rw-r--r--   0        0        0     1108 2022-11-14 15:08:03.462809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.min.js
--rw-r--r--   0        0        0       45 2022-11-14 15:08:03.463809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.min.js.flow
--rw-r--r--   0        0        0     3736 2022-11-14 15:08:03.464809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.min.js.map
--rw-r--r--   0        0        0    38668 2022-11-14 15:08:03.465809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.js
--rw-r--r--   0        0        0    87396 2022-11-14 15:08:03.467809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.js.map
--rw-r--r--   0        0        0     9755 2022-11-14 15:08:03.467809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js
--rw-r--r--   0        0        0       51 2022-11-14 15:08:03.467809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js.flow
--rw-r--r--   0        0        0    60851 2022-11-14 15:08:03.468809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js.map
--rw-r--r--   0        0        0    49678 2022-11-14 15:08:03.471809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.js
--rw-r--r--   0        0        0   110975 2022-11-14 15:08:03.474809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.js.map
--rw-r--r--   0        0        0    13539 2022-11-14 15:08:03.475809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js
--rw-r--r--   0        0        0       51 2022-11-14 15:08:03.476809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js.flow
--rw-r--r--   0        0        0    78475 2022-11-14 15:08:03.477809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js.map
--rw-r--r--   0        0        0    70878 2022-11-14 15:08:03.479809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.js
--rw-r--r--   0        0        0   158154 2022-11-14 15:08:03.482809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.js.map
--rw-r--r--   0        0        0    20095 2022-11-14 15:08:03.484809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.min.js
--rw-r--r--   0        0        0       46 2022-11-14 15:08:03.485809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.min.js.flow
--rw-r--r--   0        0        0   114779 2022-11-14 15:08:03.487809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.min.js.map
--rw-r--r--   0        0        0       23 2022-11-14 15:08:03.411809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/index.d.ts
--rw-r--r--   0        0        0      750 2022-11-14 15:08:03.412809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/createPopper.d.ts
--rw-r--r--   0        0        0    10135 2022-11-14 15:08:03.413809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/createPopper.js
--rw-r--r--   0        0        0     9415 2022-11-14 15:08:03.414809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/createPopper.js.flow
--rw-r--r--   0        0        0       76 2022-11-14 15:08:03.488809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/contains.d.ts
--rw-r--r--   0        0        0      677 2022-11-14 15:08:03.489809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/contains.js
--rw-r--r--   0        0        0      697 2022-11-14 15:08:03.490809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/contains.js.flow
--rw-r--r--   0        0        0      217 2022-11-14 15:08:03.490809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.d.ts
--rw-r--r--   0        0        0     1371 2022-11-14 15:08:03.491809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.js
--rw-r--r--   0        0        0     1485 2022-11-14 15:08:03.491809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.js.flow
--rw-r--r--   0        0        0      283 2022-11-14 15:08:03.492809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.d.ts
--rw-r--r--   0        0        0     3400 2022-11-14 15:08:03.492809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.js
--rw-r--r--   0        0        0     3782 2022-11-14 15:08:03.493809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.js.flow
--rw-r--r--   0        0        0      212 2022-11-14 15:08:03.493809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.d.ts
--rw-r--r--   0        0        0     2072 2022-11-14 15:08:03.494809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.js
--rw-r--r--   0        0        0     2192 2022-11-14 15:08:03.494809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.js.flow
--rw-r--r--   0        0        0       81 2022-11-14 15:08:03.496809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getComputedStyle.d.ts
--rw-r--r--   0        0        0      148 2022-11-14 15:08:03.496809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getComputedStyle.js
--rw-r--r--   0        0        0      190 2022-11-14 15:08:03.497809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getComputedStyle.js.flow
--rw-r--r--   0        0        0      124 2022-11-14 15:08:03.497809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentElement.d.ts
--rw-r--r--   0        0        0      311 2022-11-14 15:08:03.498809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentElement.js
--rw-r--r--   0        0        0      420 2022-11-14 15:08:03.498809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentElement.js.flow
--rw-r--r--   0        0        0      107 2022-11-14 15:08:03.499809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.d.ts
--rw-r--r--   0        0        0     1227 2022-11-14 15:08:03.501809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.js
--rw-r--r--   0        0        0     1198 2022-11-14 15:08:03.502809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.js.flow
--rw-r--r--   0        0        0      120 2022-11-14 15:08:03.502809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getHTMLElementScroll.d.ts
--rw-r--r--   0        0        0      142 2022-11-14 15:08:03.503809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getHTMLElementScroll.js
--rw-r--r--   0        0        0      167 2022-11-14 15:08:03.504809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getHTMLElementScroll.js.flow
--rw-r--r--   0        0        0      105 2022-11-14 15:08:03.505809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.d.ts
--rw-r--r--   0        0        0      767 2022-11-14 15:08:03.509809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.js
--rw-r--r--   0        0        0      821 2022-11-14 15:08:03.509809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.js.flow
--rw-r--r--   0        0        0      149 2022-11-14 15:08:03.510809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeName.d.ts
--rw-r--r--   0        0        0      114 2022-11-14 15:08:03.511809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeName.js
--rw-r--r--   0        0        0      190 2022-11-14 15:08:03.511809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeName.js.flow
--rw-r--r--   0        0        0      146 2022-11-14 15:08:03.512809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeScroll.d.ts
--rw-r--r--   0        0        0      396 2022-11-14 15:08:03.512809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeScroll.js
--rw-r--r--   0        0        0      450 2022-11-14 15:08:03.513809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeScroll.js.flow
--rw-r--r--   0        0        0       64 2022-11-14 15:08:03.513809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.d.ts
--rw-r--r--   0        0        0     2613 2022-11-14 15:08:03.514809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.js
--rw-r--r--   0        0        0     2767 2022-11-14 15:08:03.514809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.js.flow
--rw-r--r--   0        0        0       73 2022-11-14 15:08:03.515809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.d.ts
--rw-r--r--   0        0        0      759 2022-11-14 15:08:03.515809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.js
--rw-r--r--   0        0        0      789 2022-11-14 15:08:03.515809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.js.flow
--rw-r--r--   0        0        0       66 2022-11-14 15:08:03.516809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.d.ts
--rw-r--r--   0        0        0      546 2022-11-14 15:08:03.516809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.js
--rw-r--r--   0        0        0      564 2022-11-14 15:08:03.517809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.js.flow
--rw-r--r--   0        0        0      217 2022-11-14 15:08:03.517809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.d.ts
--rw-r--r--   0        0        0      881 2022-11-14 15:08:03.518809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.js
--rw-r--r--   0        0        0      964 2022-11-14 15:08:03.518809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.js.flow
--rw-r--r--   0        0        0       51 2022-11-14 15:08:03.519809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindow.d.ts
--rw-r--r--   0        0        0      273 2022-11-14 15:08:03.519809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindow.js
--rw-r--r--   0        0        0      383 2022-11-14 15:08:03.520809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindow.js.flow
--rw-r--r--   0        0        0      148 2022-11-14 15:08:03.520809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScroll.d.ts
--rw-r--r--   0        0        0      258 2022-11-14 15:08:03.521809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScroll.js
--rw-r--r--   0        0        0      306 2022-11-14 15:08:03.521809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScroll.js.flow
--rw-r--r--   0        0        0       71 2022-11-14 15:08:03.521809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.d.ts
--rw-r--r--   0        0        0      721 2022-11-14 15:08:03.522809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.js
--rw-r--r--   0        0        0      754 2022-11-14 15:08:03.522809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.js.flow
--rw-r--r--   0        0        0      214 2022-11-14 15:08:03.523809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.d.ts
--rw-r--r--   0        0        0      621 2022-11-14 15:08:03.523809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.js
--rw-r--r--   0        0        0      902 2022-11-14 15:08:03.524809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.js.flow
--rw-r--r--   0        0        0       53 2022-11-14 15:08:03.525809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isLayoutViewport.d.ts
--rw-r--r--   0        0        0      159 2022-11-14 15:08:03.525809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isLayoutViewport.js
--rw-r--r--   0        0        0      167 2022-11-14 15:08:03.525809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isLayoutViewport.js.flow
--rw-r--r--   0        0        0       71 2022-11-14 15:08:03.526809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isScrollParent.d.ts
--rw-r--r--   0        0        0      440 2022-11-14 15:08:03.526809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isScrollParent.js
--rw-r--r--   0        0        0      349 2022-11-14 15:08:03.527809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isScrollParent.js.flow
--rw-r--r--   0        0        0       67 2022-11-14 15:08:03.527809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isTableElement.d.ts
--rw-r--r--   0        0        0      162 2022-11-14 15:08:03.527809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isTableElement.js
--rw-r--r--   0        0        0      188 2022-11-14 15:08:03.528809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isTableElement.js.flow
--rw-r--r--   0        0        0      188 2022-11-14 15:08:03.528809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.d.ts
--rw-r--r--   0        0        0     1177 2022-11-14 15:08:03.529809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.js
--rw-r--r--   0        0        0     1227 2022-11-14 15:08:03.529809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.js.flow
--rw-r--r--   0        0        0     2008 2022-11-14 15:08:03.414809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/enums.d.ts
--rw-r--r--   0        0        0     1335 2022-11-14 15:08:03.415809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/enums.js
--rw-r--r--   0        0        0     2763 2022-11-14 15:08:03.416809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/enums.js.flow
--rw-r--r--   0        0        0      286 2022-11-14 15:08:03.417809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/index.d.ts
--rw-r--r--   0        0        0      443 2022-11-14 15:08:03.417809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/index.js
--rw-r--r--   0        0        0      462 2022-11-14 15:08:03.418809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/index.js.flow
--rw-r--r--   0        0        0      183 2022-11-14 15:08:03.530809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.d.ts
--rw-r--r--   0        0        0     2527 2022-11-14 15:08:03.530809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.js
--rw-r--r--   0        0        0     2723 2022-11-14 15:08:03.531809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.js.flow
--rw-r--r--   0        0        0      435 2022-11-14 15:08:03.532809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/arrow.d.ts
--rw-r--r--   0        0        0     3942 2022-11-14 15:08:03.534809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/arrow.js
--rw-r--r--   0        0        0     4208 2022-11-14 15:08:03.536809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/arrow.js.flow
--rw-r--r--   0        0        0     1208 2022-11-14 15:08:03.537809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.d.ts
--rw-r--r--   0        0        0     6598 2022-11-14 15:08:03.537809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.js
--rw-r--r--   0        0        0     6945 2022-11-14 15:08:03.538809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.js.flow
--rw-r--r--   0        0        0      274 2022-11-14 15:08:03.539809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.d.ts
--rw-r--r--   0        0        0     1330 2022-11-14 15:08:03.540809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.js
--rw-r--r--   0        0        0     1341 2022-11-14 15:08:03.540809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.js.flow
--rw-r--r--   0        0        0      543 2022-11-14 15:08:03.540809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.d.ts
--rw-r--r--   0        0        0     4910 2022-11-14 15:08:03.541809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.js
--rw-r--r--   0        0        0     4893 2022-11-14 15:08:03.542809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.js.flow
--rw-r--r--   0        0        0      162 2022-11-14 15:08:03.542809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/hide.d.ts
--rw-r--r--   0        0        0     1954 2022-11-14 15:08:03.543809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/hide.js
--rw-r--r--   0        0        0     2034 2022-11-14 15:08:03.543809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/hide.js.flow
--rw-r--r--   0        0        0      476 2022-11-14 15:08:03.544809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/index.d.ts
--rw-r--r--   0        0        0      502 2022-11-14 15:08:03.544809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/index.js
--rw-r--r--   0        0        0      485 2022-11-14 15:08:03.544809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/index.js.flow
--rw-r--r--   0        0        0      703 2022-11-14 15:08:03.545809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.d.ts
--rw-r--r--   0        0        0     1613 2022-11-14 15:08:03.545809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.js
--rw-r--r--   0        0        0     1933 2022-11-14 15:08:03.546809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.js.flow
--rw-r--r--   0        0        0      189 2022-11-14 15:08:03.547809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.d.ts
--rw-r--r--   0        0        0      706 2022-11-14 15:08:03.547809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.js
--rw-r--r--   0        0        0      855 2022-11-14 15:08:03.547809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.js.flow
--rw-r--r--   0        0        0      862 2022-11-14 15:08:03.548809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.d.ts
--rw-r--r--   0        0        0     6585 2022-11-14 15:08:03.548809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.js
--rw-r--r--   0        0        0     7439 2022-11-14 15:08:03.548809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.js.flow
--rw-r--r--   0        0        0      163 2022-11-14 15:08:03.419809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper-base.d.ts
--rw-r--r--   0        0        0      193 2022-11-14 15:08:03.419809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper-base.js
--rw-r--r--   0        0        0      232 2022-11-14 15:08:03.420809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper-base.js.flow
--rw-r--r--   0        0        0      705 2022-11-14 15:08:03.420809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper-lite.d.ts
--rw-r--r--   0        0        0      603 2022-11-14 15:08:03.420809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper-lite.js
--rw-r--r--   0        0        0      614 2022-11-14 15:08:03.421809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper-lite.js.flow
--rw-r--r--   0        0        0     1038 2022-11-14 15:08:03.421809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper.d.ts
--rw-r--r--   0        0        0     1090 2022-11-14 15:08:03.422809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper.js
--rw-r--r--   0        0        0     1082 2022-11-14 15:08:03.422809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper.js.flow
--rw-r--r--   0        0        0     5224 2022-11-14 15:08:03.422809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/types.d.ts
--rw-r--r--   0        0        0        0 2022-11-14 15:08:03.422809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/types.js
--rw-r--r--   0        0        0     4933 2022-11-14 15:08:03.424809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/types.js.flow
--rw-r--r--   0        0        0      466 2022-11-14 15:08:03.549809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.d.ts
--rw-r--r--   0        0        0     2023 2022-11-14 15:08:03.549809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.js
--rw-r--r--   0        0        0     2178 2022-11-14 15:08:03.550809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.js.flow
--rw-r--r--   0        0        0      353 2022-11-14 15:08:03.550809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeOffsets.d.ts
--rw-r--r--   0        0        0     1738 2022-11-14 15:08:03.550809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeOffsets.js
--rw-r--r--   0        0        0     1971 2022-11-14 15:08:03.550809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeOffsets.js.flow
--rw-r--r--   0        0        0       89 2022-11-14 15:08:03.551809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/debounce.d.ts
--rw-r--r--   0        0        0      302 2022-11-14 15:08:03.551809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/debounce.js
--rw-r--r--   0        0        0      327 2022-11-14 15:08:03.551809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/debounce.js.flow
--rw-r--r--   0        0        0      480 2022-11-14 15:08:03.551809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/detectOverflow.d.ts
--rw-r--r--   0        0        0     3528 2022-11-14 15:08:03.552809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/detectOverflow.js
--rw-r--r--   0        0        0     3265 2022-11-14 15:08:03.552809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/detectOverflow.js.flow
--rw-r--r--   0        0        0      149 2022-11-14 15:08:03.555809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/expandToHashMap.d.ts
--rw-r--r--   0        0        0      159 2022-11-14 15:08:03.555809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/expandToHashMap.js
--rw-r--r--   0        0        0      246 2022-11-14 15:08:03.555809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/expandToHashMap.js.flow
--rw-r--r--   0        0        0       77 2022-11-14 15:08:03.556809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/format.d.ts
--rw-r--r--   0        0        0      286 2022-11-14 15:08:03.556809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/format.js
--rw-r--r--   0        0        0      144 2022-11-14 15:08:03.556809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/format.js.flow
--rw-r--r--   0        0        0       64 2022-11-14 15:08:03.557809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getAltAxis.d.ts
--rw-r--r--   0        0        0       79 2022-11-14 15:08:03.557809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getAltAxis.js
--rw-r--r--   0        0        0      112 2022-11-14 15:08:03.558809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getAltAxis.js.flow
--rw-r--r--   0        0        0       80 2022-11-14 15:08:03.558809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getAltLen.d.ts
--rw-r--r--   0        0        0       89 2022-11-14 15:08:03.558809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getAltLen.js
--rw-r--r--   0        0        0      140 2022-11-14 15:08:03.559809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getAltLen.js.flow
--rw-r--r--   0        0        0      152 2022-11-14 15:08:03.559809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getBasePlacement.d.ts
--rw-r--r--   0        0        0      125 2022-11-14 15:08:03.559809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getBasePlacement.js
--rw-r--r--   0        0        0      220 2022-11-14 15:08:03.559809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getBasePlacement.js.flow
--rw-r--r--   0        0        0      102 2022-11-14 15:08:03.560809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getFreshSideObject.d.ts
--rw-r--r--   0        0        0      117 2022-11-14 15:08:03.560809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getFreshSideObject.js
--rw-r--r--   0        0        0      185 2022-11-14 15:08:03.560809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getFreshSideObject.js.flow
--rw-r--r--   0        0        0      126 2022-11-14 15:08:03.561809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getMainAxisFromPlacement.d.ts
--rw-r--r--   0        0        0      127 2022-11-14 15:08:03.561809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getMainAxisFromPlacement.js
--rw-r--r--   0        0        0      207 2022-11-14 15:08:03.562809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getMainAxisFromPlacement.js.flow
--rw-r--r--   0        0        0      122 2022-11-14 15:08:03.562809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositePlacement.d.ts
--rw-r--r--   0        0        0      248 2022-11-14 15:08:03.563809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositePlacement.js
--rw-r--r--   0        0        0      312 2022-11-14 15:08:03.564809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositePlacement.js.flow
--rw-r--r--   0        0        0      131 2022-11-14 15:08:03.564809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositeVariationPlacement.d.ts
--rw-r--r--   0        0        0      209 2022-11-14 15:08:03.564809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositeVariationPlacement.js
--rw-r--r--   0        0        0      269 2022-11-14 15:08:03.565809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositeVariationPlacement.js.flow
--rw-r--r--   0        0        0      139 2022-11-14 15:08:03.565809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getVariation.d.ts
--rw-r--r--   0        0        0       85 2022-11-14 15:08:03.565809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getVariation.js
--rw-r--r--   0        0        0      185 2022-11-14 15:08:03.566809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/getVariation.js.flow
--rw-r--r--   0        0        0      169 2022-11-14 15:08:03.566809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/math.d.ts
--rw-r--r--   0        0        0       84 2022-11-14 15:08:03.567809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/math.js
--rw-r--r--   0        0        0      100 2022-11-14 15:08:03.567809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/math.js.flow
--rw-r--r--   0        0        0      162 2022-11-14 15:08:03.568809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergeByName.d.ts
--rw-r--r--   0        0        0      524 2022-11-14 15:08:03.568809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergeByName.js
--rw-r--r--   0        0        0      639 2022-11-14 15:08:03.569809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergeByName.js.flow
--rw-r--r--   0        0        0      136 2022-11-14 15:08:03.569809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergePaddingObject.d.ts
--rw-r--r--   0        0        0      184 2022-11-14 15:08:03.570809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergePaddingObject.js
--rw-r--r--   0        0        0      274 2022-11-14 15:08:03.571809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergePaddingObject.js.flow
--rw-r--r--   0        0        0      147 2022-11-14 15:08:03.571809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/orderModifiers.d.ts
--rw-r--r--   0        0        0     1240 2022-11-14 15:08:03.571809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/orderModifiers.js
--rw-r--r--   0        0        0     1360 2022-11-14 15:08:03.572809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/orderModifiers.js.flow
--rw-r--r--   0        0        0      128 2022-11-14 15:08:03.572809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/rectToClientRect.d.ts
--rw-r--r--   0        0        0      191 2022-11-14 15:08:03.572809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/rectToClientRect.js
--rw-r--r--   0        0        0      271 2022-11-14 15:08:03.573809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/rectToClientRect.js.flow
--rw-r--r--   0        0        0       84 2022-11-14 15:08:03.573809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/uniqueBy.d.ts
--rw-r--r--   0        0        0      252 2022-11-14 15:08:03.573809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/uniqueBy.js
--rw-r--r--   0        0        0      293 2022-11-14 15:08:03.574809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/uniqueBy.js.flow
--rw-r--r--   0        0        0       47 2022-11-14 15:08:03.574809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/userAgent.d.ts
--rw-r--r--   0        0        0      269 2022-11-14 15:08:03.575809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/userAgent.js
--rw-r--r--   0        0        0      461 2022-11-14 15:08:03.575809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/userAgent.js.flow
--rw-r--r--   0        0        0       72 2022-11-14 15:08:03.575809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/validateModifiers.d.ts
--rw-r--r--   0        0        0     3261 2022-11-14 15:08:03.576810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/validateModifiers.js
--rw-r--r--   0        0        0     4504 2022-11-14 15:08:03.576810 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/validateModifiers.js.flow
--rw-r--r--   0        0        0      170 2022-11-14 15:08:03.577809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/within.d.ts
--rw-r--r--   0        0        0      262 2022-11-14 15:08:03.577809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/within.js
--rw-r--r--   0        0        0      329 2022-11-14 15:08:03.577809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/within.js.flow
--rw-r--r--   0        0        0     4230 2022-11-14 15:08:03.411809 anitya-1.7.0/anitya/static/node_modules/@popperjs/core/package.json
--rw-r--r--   0        0        0     1131 2022-11-16 11:34:15.722286 anitya-1.7.0/anitya/static/node_modules/bootstrap/LICENSE
--rw-r--r--   0        0        0    13659 2022-11-16 11:34:15.764286 anitya-1.7.0/anitya/static/node_modules/bootstrap/README.md
--rw-r--r--   0        0        0    71861 2022-11-16 11:34:15.723286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.css
--rw-r--r--   0        0        0   210357 2022-11-16 11:34:15.745286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    53265 2022-11-16 11:34:15.724286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   131395 2022-11-16 11:34:15.746286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    71935 2022-11-16 11:34:15.725286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   210361 2022-11-16 11:34:15.746286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    53340 2022-11-16 11:34:15.725286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   131472 2022-11-16 11:34:15.747286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0     7965 2022-11-16 11:34:15.725286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   110875 2022-11-16 11:34:15.747286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0     6490 2022-11-16 11:34:15.726286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    40331 2022-11-16 11:34:15.747286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0     7958 2022-11-16 11:34:15.726286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   110888 2022-11-16 11:34:15.748286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0     6562 2022-11-16 11:34:15.727286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    48693 2022-11-16 11:34:15.748286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0    74135 2022-11-16 11:34:15.727286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   196435 2022-11-16 11:34:15.748286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    56365 2022-11-16 11:34:15.728286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   115588 2022-11-16 11:34:15.749286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0    74002 2022-11-16 11:34:15.728286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   196378 2022-11-16 11:34:15.749286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    56293 2022-11-16 11:34:15.729286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   115423 2022-11-16 11:34:15.750286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   237994 2022-11-16 11:34:15.729286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.css
--rw-r--r--   0        0        0   608416 2022-11-16 11:34:15.753286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.css.map
--rw-r--r--   0        0        0   194901 2022-11-16 11:34:15.730286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.min.css
--rw-r--r--   0        0        0   522733 2022-11-16 11:34:15.756286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   237526 2022-11-16 11:34:15.731286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   608236 2022-11-16 11:34:15.758286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   195007 2022-11-16 11:34:15.731286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   767573 2022-11-16 11:34:15.760286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0   208123 2022-11-16 11:34:15.734286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   452089 2022-11-16 11:34:15.751286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80496 2022-11-16 11:34:15.734286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   333304 2022-11-16 11:34:15.752286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   136335 2022-11-16 11:34:15.735286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.js
--rw-r--r--   0        0        0   308526 2022-11-16 11:34:15.754286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    74054 2022-11-16 11:34:15.735286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   221402 2022-11-16 11:34:15.755286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145677 2022-11-16 11:34:15.736286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.js
--rw-r--r--   0        0        0   309667 2022-11-16 11:34:15.755286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.js.map
--rw-r--r--   0        0        0    60480 2022-11-16 11:34:15.736286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.min.js
--rw-r--r--   0        0        0   217134 2022-11-16 11:34:15.757286 anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.min.js.map
--rw-r--r--   0        0        0     3140 2022-11-16 11:34:15.732286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/alert.js
--rw-r--r--   0        0        0     4294 2022-11-16 11:34:15.744286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/alert.js.map
--rw-r--r--   0        0        0     3224 2022-11-16 11:34:15.733286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/base-component.js
--rw-r--r--   0        0        0     4602 2022-11-16 11:34:15.745286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/base-component.js.map
--rw-r--r--   0        0        0     2756 2022-11-16 11:34:15.736286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/button.js
--rw-r--r--   0        0        0     3466 2022-11-16 11:34:15.761286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/button.js.map
--rw-r--r--   0        0        0    14281 2022-11-16 11:34:15.737286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/carousel.js
--rw-r--r--   0        0        0    27442 2022-11-16 11:34:15.761286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/carousel.js.map
--rw-r--r--   0        0        0     9455 2022-11-16 11:34:15.737286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/collapse.js
--rw-r--r--   0        0        0    18212 2022-11-16 11:34:15.761286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/collapse.js.map
--rw-r--r--   0        0        0     2119 2022-11-16 11:34:15.738286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/data.js
--rw-r--r--   0        0        0     3047 2022-11-16 11:34:15.761286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/data.js.map
--rw-r--r--   0        0        0     9578 2022-11-16 11:34:15.739286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/event-handler.js
--rw-r--r--   0        0        0    19800 2022-11-16 11:34:15.762286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/event-handler.js.map
--rw-r--r--   0        0        0     2438 2022-11-16 11:34:15.740286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/manipulator.js
--rw-r--r--   0        0        0     4319 2022-11-16 11:34:15.762286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/manipulator.js.map
--rw-r--r--   0        0        0     2700 2022-11-16 11:34:15.742286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/selector-engine.js
--rw-r--r--   0        0        0     4619 2022-11-16 11:34:15.763286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/selector-engine.js.map
--rw-r--r--   0        0        0    16199 2022-11-16 11:34:15.739286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dropdown.js
--rw-r--r--   0        0        0    29448 2022-11-16 11:34:15.762286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dropdown.js.map
--rw-r--r--   0        0        0    12194 2022-11-16 11:34:15.741286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/modal.js
--rw-r--r--   0        0        0    22634 2022-11-16 11:34:15.762286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/modal.js.map
--rw-r--r--   0        0        0     9166 2022-11-16 11:34:15.741286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/offcanvas.js
--rw-r--r--   0        0        0    16142 2022-11-16 11:34:15.763286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/offcanvas.js.map
--rw-r--r--   0        0        0     2883 2022-11-16 11:34:15.741286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/popover.js
--rw-r--r--   0        0        0     4053 2022-11-16 11:34:15.763286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/popover.js.map
--rw-r--r--   0        0        0    10303 2022-11-16 11:34:15.742286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/scrollspy.js
--rw-r--r--   0        0        0    18973 2022-11-16 11:34:15.763286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/scrollspy.js.map
--rw-r--r--   0        0        0    10647 2022-11-16 11:34:15.743286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/tab.js
--rw-r--r--   0        0        0    19947 2022-11-16 11:34:15.764286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/tab.js.map
--rw-r--r--   0        0        0     6632 2022-11-16 11:34:15.744286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/toast.js
--rw-r--r--   0        0        0    12018 2022-11-16 11:34:15.764286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/toast.js.map
--rw-r--r--   0        0        0    19359 2022-11-16 11:34:15.744286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/tooltip.js
--rw-r--r--   0        0        0    37922 2022-11-16 11:34:15.764286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/tooltip.js.map
--rw-r--r--   0        0        0     4413 2022-11-16 11:34:15.732286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/backdrop.js
--rw-r--r--   0        0        0     7172 2022-11-16 11:34:15.745286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/backdrop.js.map
--rw-r--r--   0        0        0     2174 2022-11-16 11:34:15.738286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/component-functions.js
--rw-r--r--   0        0        0     2310 2022-11-16 11:34:15.761286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/component-functions.js.map
--rw-r--r--   0        0        0     2808 2022-11-16 11:34:15.738286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/config.js
--rw-r--r--   0        0        0     4073 2022-11-16 11:34:15.761286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/config.js.map
--rw-r--r--   0        0        0     3913 2022-11-16 11:34:15.740286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/focustrap.js
--rw-r--r--   0        0        0     5891 2022-11-16 11:34:15.762286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/focustrap.js.map
--rw-r--r--   0        0        0    10248 2022-11-16 11:34:15.740286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/index.js
--rw-r--r--   0        0        0    18675 2022-11-16 11:34:15.762286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/index.js.map
--rw-r--r--   0        0        0     4253 2022-11-16 11:34:15.742286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/sanitizer.js
--rw-r--r--   0        0        0     7572 2022-11-16 11:34:15.763286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/sanitizer.js.map
--rw-r--r--   0        0        0     5031 2022-11-16 11:34:15.742286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/scrollbar.js
--rw-r--r--   0        0        0     8041 2022-11-16 11:34:15.763286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/scrollbar.js.map
--rw-r--r--   0        0        0     4733 2022-11-16 11:34:15.743286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/swipe.js
--rw-r--r--   0        0        0     8335 2022-11-16 11:34:15.763286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/swipe.js.map
--rw-r--r--   0        0        0     4980 2022-11-16 11:34:15.743286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/template-factory.js
--rw-r--r--   0        0        0     8655 2022-11-16 11:34:15.764286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/template-factory.js.map
--rw-r--r--   0        0        0     1901 2022-11-16 11:34:15.732286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/alert.js
--rw-r--r--   0        0        0     1930 2022-11-16 11:34:15.733286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/base-component.js
--rw-r--r--   0        0        0     1626 2022-11-16 11:34:15.737286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/button.js
--rw-r--r--   0        0        0    11820 2022-11-16 11:34:15.737286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/carousel.js
--rw-r--r--   0        0        0     7669 2022-11-16 11:34:15.737286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/collapse.js
--rw-r--r--   0        0        0     1405 2022-11-16 11:34:15.739286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/dom/data.js
--rw-r--r--   0        0        0     8450 2022-11-16 11:34:15.739286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/dom/event-handler.js
--rw-r--r--   0        0        0     1668 2022-11-16 11:34:15.740286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/dom/manipulator.js
--rw-r--r--   0        0        0     1968 2022-11-16 11:34:15.743286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/dom/selector-engine.js
--rw-r--r--   0        0        0    13257 2022-11-16 11:34:15.739286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/dropdown.js
--rw-r--r--   0        0        0     9629 2022-11-16 11:34:15.741286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/modal.js
--rw-r--r--   0        0        0     6804 2022-11-16 11:34:15.741286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/offcanvas.js
--rw-r--r--   0        0        0     1874 2022-11-16 11:34:15.741286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/popover.js
--rw-r--r--   0        0        0     8448 2022-11-16 11:34:15.742286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/scrollspy.js
--rw-r--r--   0        0        0     8756 2022-11-16 11:34:15.743286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/tab.js
--rw-r--r--   0        0        0     5037 2022-11-16 11:34:15.744286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/toast.js
--rw-r--r--   0        0        0    16305 2022-11-16 11:34:15.744286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/tooltip.js
--rw-r--r--   0        0        0     3126 2022-11-16 11:34:15.733286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/backdrop.js
--rw-r--r--   0        0        0     1072 2022-11-16 11:34:15.738286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/component-functions.js
--rw-r--r--   0        0        0     1818 2022-11-16 11:34:15.738286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/config.js
--rw-r--r--   0        0        0     2519 2022-11-16 11:34:15.740286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/focustrap.js
--rw-r--r--   0        0        0     8436 2022-11-16 11:34:15.740286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/index.js
--rw-r--r--   0        0        0     3253 2022-11-16 11:34:15.742286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/sanitizer.js
--rw-r--r--   0        0        0     3755 2022-11-16 11:34:15.742286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/scrollbar.js
--rw-r--r--   0        0        0     3410 2022-11-16 11:34:15.743286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/swipe.js
--rw-r--r--   0        0        0     3630 2022-11-16 11:34:15.743286 anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/template-factory.js
--rw-r--r--   0        0        0     9330 2022-11-16 11:34:15.744286 anitya-1.7.0/anitya/static/node_modules/bootstrap/package.json
--rw-r--r--   0        0        0     4790 2022-11-16 11:34:15.765286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_accordion.scss
--rw-r--r--   0        0        0     2126 2022-11-16 11:34:15.765286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_alert.scss
--rw-r--r--   0        0        0     1118 2022-11-16 11:34:15.765286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_badge.scss
--rw-r--r--   0        0        0     1751 2022-11-16 11:34:15.766286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_breadcrumb.scss
--rw-r--r--   0        0        0     3073 2022-11-16 11:34:15.766286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_button-group.scss
--rw-r--r--   0        0        0     6685 2022-11-16 11:34:15.766286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_buttons.scss
--rw-r--r--   0        0        0     6736 2022-11-16 11:34:15.766286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_card.scss
--rw-r--r--   0        0        0     5625 2022-11-16 11:34:15.767286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_carousel.scss
--rw-r--r--   0        0        0     1127 2022-11-16 11:34:15.767286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_close.scss
--rw-r--r--   0        0        0     1201 2022-11-16 11:34:15.769286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_containers.scss
--rw-r--r--   0        0        0     8018 2022-11-16 11:34:15.770286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_dropdown.scss
--rw-r--r--   0        0        0      256 2022-11-16 11:34:15.773286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_forms.scss
--rw-r--r--   0        0        0    10553 2022-11-16 11:34:15.773286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_functions.scss
--rw-r--r--   0        0        0      575 2022-11-16 11:34:15.774286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_grid.scss
--rw-r--r--   0        0        0      294 2022-11-16 11:34:15.774286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_helpers.scss
--rw-r--r--   0        0        0     1158 2022-11-16 11:34:15.774286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_images.scss
--rw-r--r--   0        0        0     6475 2022-11-16 11:34:15.775287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_list-group.scss
--rw-r--r--   0        0        0     1648 2022-11-16 11:34:15.776286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_maps.scss
--rw-r--r--   0        0        0      899 2022-11-16 11:34:15.776286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_mixins.scss
--rw-r--r--   0        0        0     7762 2022-11-16 11:34:15.776286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_modal.scss
--rw-r--r--   0        0        0     4665 2022-11-16 11:34:15.777286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_nav.scss
--rw-r--r--   0        0        0     8936 2022-11-16 11:34:15.777286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_navbar.scss
--rw-r--r--   0        0        0     4555 2022-11-16 11:34:15.777286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_offcanvas.scss
--rw-r--r--   0        0        0     3940 2022-11-16 11:34:15.777286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_pagination.scss
--rw-r--r--   0        0        0      859 2022-11-16 11:34:15.778287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_placeholders.scss
--rw-r--r--   0        0        0     6907 2022-11-16 11:34:15.778287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_popover.scss
--rw-r--r--   0        0        0     1875 2022-11-16 11:34:15.778287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_progress.scss
--rw-r--r--   0        0        0    12311 2022-11-16 11:34:15.779286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_reboot.scss
--rw-r--r--   0        0        0     2395 2022-11-16 11:34:15.780286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_root.scss
--rw-r--r--   0        0        0     2429 2022-11-16 11:34:15.780286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_spinners.scss
--rw-r--r--   0        0        0     4358 2022-11-16 11:34:15.780286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_tables.scss
--rw-r--r--   0        0        0     2490 2022-11-16 11:34:15.781287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_toasts.scss
--rw-r--r--   0        0        0     3939 2022-11-16 11:34:15.781287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_tooltip.scss
--rw-r--r--   0        0        0      425 2022-11-16 11:34:15.782287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_transitions.scss
--rw-r--r--   0        0        0     1420 2022-11-16 11:34:15.782287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_type.scss
--rw-r--r--   0        0        0    14817 2022-11-16 11:34:15.782287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_utilities.scss
--rw-r--r--   0        0        0    68610 2022-11-16 11:34:15.783286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_variables.scss
--rw-r--r--   0        0        0     1198 2022-11-16 11:34:15.783286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/bootstrap-grid.scss
--rw-r--r--   0        0        0      163 2022-11-16 11:34:15.784287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/bootstrap-reboot.scss
--rw-r--r--   0        0        0      240 2022-11-16 11:34:15.784287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/bootstrap-utilities.scss
--rw-r--r--   0        0        0      912 2022-11-16 11:34:15.784287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/bootstrap.scss
--rw-r--r--   0        0        0     2030 2022-11-16 11:34:15.771286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_floating-labels.scss
--rw-r--r--   0        0        0     4287 2022-11-16 11:34:15.771286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_form-check.scss
--rw-r--r--   0        0        0     5695 2022-11-16 11:34:15.771286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_form-control.scss
--rw-r--r--   0        0        0     2796 2022-11-16 11:34:15.771286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_form-range.scss
--rw-r--r--   0        0        0     2316 2022-11-16 11:34:15.771286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_form-select.scss
--rw-r--r--   0        0        0      219 2022-11-16 11:34:15.771286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_form-text.scss
--rw-r--r--   0        0        0     3835 2022-11-16 11:34:15.775287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_input-group.scss
--rw-r--r--   0        0        0     1142 2022-11-16 11:34:15.775287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_labels.scss
--rw-r--r--   0        0        0      478 2022-11-16 11:34:15.782287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_validation.scss
--rw-r--r--   0        0        0       37 2022-11-16 11:34:15.767286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/helpers/_clearfix.scss
--rw-r--r--   0        0        0      454 2022-11-16 11:34:15.767286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/helpers/_color-bg.scss
--rw-r--r--   0        0        0      450 2022-11-16 11:34:15.769286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/helpers/_colored-links.scss
--rw-r--r--   0        0        0      621 2022-11-16 11:34:15.778287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/helpers/_position.scss
--rw-r--r--   0        0        0      399 2022-11-16 11:34:15.779286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/helpers/_ratio.scss
--rw-r--r--   0        0        0      245 2022-11-16 11:34:15.780286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/helpers/_stacks.scss
--rw-r--r--   0        0        0      223 2022-11-16 11:34:15.780286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/helpers/_stretched-link.scss
--rw-r--r--   0        0        0       73 2022-11-16 11:34:15.781287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/helpers/_text-truncation.scss
--rw-r--r--   0        0        0      136 2022-11-16 11:34:15.783286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/helpers/_visually-hidden.scss
--rw-r--r--   0        0        0      147 2022-11-16 11:34:15.783286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/helpers/_vr.scss
--rw-r--r--   0        0        0      393 2022-11-16 11:34:15.765286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_alert.scss
--rw-r--r--   0        0        0      328 2022-11-16 11:34:15.765286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_backdrop.scss
--rw-r--r--   0        0        0      263 2022-11-16 11:34:15.765286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_banner.scss
--rw-r--r--   0        0        0     2031 2022-11-16 11:34:15.766286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_border-radius.scss
--rw-r--r--   0        0        0      398 2022-11-16 11:34:15.766286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_box-shadow.scss
--rw-r--r--   0        0        0     4580 2022-11-16 11:34:15.766286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_breakpoints.scss
--rw-r--r--   0        0        0     3220 2022-11-16 11:34:15.766286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_buttons.scss
--rw-r--r--   0        0        0     1473 2022-11-16 11:34:15.767286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_caret.scss
--rw-r--r--   0        0        0      147 2022-11-16 11:34:15.767286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_clearfix.scss
--rw-r--r--   0        0        0      167 2022-11-16 11:34:15.769286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_color-scheme.scss
--rw-r--r--   0        0        0      410 2022-11-16 11:34:15.769286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_container.scss
--rw-r--r--   0        0        0      613 2022-11-16 11:34:15.770286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_deprecate.scss
--rw-r--r--   0        0        0     4122 2022-11-16 11:34:15.773286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_forms.scss
--rw-r--r--   0        0        0     1956 2022-11-16 11:34:15.773286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_gradients.scss
--rw-r--r--   0        0        0     4726 2022-11-16 11:34:15.774286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_grid.scss
--rw-r--r--   0        0        0      395 2022-11-16 11:34:15.774286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_image.scss
--rw-r--r--   0        0        0      509 2022-11-16 11:34:15.776286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_list-group.scss
--rw-r--r--   0        0        0      168 2022-11-16 11:34:15.776286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_lists.scss
--rw-r--r--   0        0        0      387 2022-11-16 11:34:15.778287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_pagination.scss
--rw-r--r--   0        0        0      495 2022-11-16 11:34:15.779286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_reset-text.scss
--rw-r--r--   0        0        0      202 2022-11-16 11:34:15.779286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_resize.scss
--rw-r--r--   0        0        0     1101 2022-11-16 11:34:15.780286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_table-variants.scss
--rw-r--r--   0        0        0      168 2022-11-16 11:34:15.781287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_text-truncate.scss
--rw-r--r--   0        0        0      661 2022-11-16 11:34:15.781287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_transition.scss
--rw-r--r--   0        0        0     3380 2022-11-16 11:34:15.782287 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_utilities.scss
--rw-r--r--   0        0        0     1012 2022-11-16 11:34:15.783286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_visually-hidden.scss
--rw-r--r--   0        0        0     1737 2022-11-16 11:34:15.765286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/utilities/_api.scss
--rw-r--r--   0        0        0    10029 2022-11-16 11:34:15.779286 anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/vendor/_rfs.scss
--rw-r--r--   0        0        0    12631 2022-11-14 15:08:03.532809 anitya-1.7.0/anitya/static/node_modules/jquery/AUTHORS.txt
--rw-r--r--   0        0        0     1097 2022-11-14 15:08:03.538809 anitya-1.7.0/anitya/static/node_modules/jquery/LICENSE.txt
--rw-r--r--   0        0        0     2004 2022-11-14 15:08:03.531809 anitya-1.7.0/anitya/static/node_modules/jquery/README.md
--rw-r--r--   0        0        0      190 2022-11-14 15:08:03.522809 anitya-1.7.0/anitya/static/node_modules/jquery/bower.json
--rw-r--r--   0        0        0   289812 2022-11-14 15:08:03.468809 anitya-1.7.0/anitya/static/node_modules/jquery/dist/jquery.js
--rw-r--r--   0        0        0    89664 2022-11-14 15:08:03.472809 anitya-1.7.0/anitya/static/node_modules/jquery/dist/jquery.min.js
--rw-r--r--   0        0        0   138161 2022-11-14 15:08:03.526809 anitya-1.7.0/anitya/static/node_modules/jquery/dist/jquery.min.map
--rw-r--r--   0        0        0   236513 2022-11-14 15:08:03.477809 anitya-1.7.0/anitya/static/node_modules/jquery/dist/jquery.slim.js
--rw-r--r--   0        0        0    72535 2022-11-14 15:08:03.479809 anitya-1.7.0/anitya/static/node_modules/jquery/dist/jquery.slim.min.js
--rw-r--r--   0        0        0   110515 2022-11-14 15:08:03.529809 anitya-1.7.0/anitya/static/node_modules/jquery/dist/jquery.slim.min.map
--rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.537809 anitya-1.7.0/anitya/static/node_modules/jquery/external/sizzle/LICENSE.txt
--rw-r--r--   0        0        0    70555 2022-11-14 15:08:03.509809 anitya-1.7.0/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.js
--rw-r--r--   0        0        0    20245 2022-11-14 15:08:03.510809 anitya-1.7.0/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.min.js
--rw-r--r--   0        0        0    31112 2022-11-14 15:08:03.530809 anitya-1.7.0/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.min.map
--rw-r--r--   0        0        0     3284 2022-11-14 15:08:03.523809 anitya-1.7.0/anitya/static/node_modules/jquery/package.json
--rw-r--r--   0        0        0     2753 2022-11-14 15:08:03.480809 anitya-1.7.0/anitya/static/node_modules/jquery/src/ajax/jsonp.js
--rw-r--r--   0        0        0     1904 2022-11-14 15:08:03.480809 anitya-1.7.0/anitya/static/node_modules/jquery/src/ajax/load.js
--rw-r--r--   0        0        0     1637 2022-11-14 15:08:03.496809 anitya-1.7.0/anitya/static/node_modules/jquery/src/ajax/script.js
--rw-r--r--   0        0        0       67 2022-11-14 15:08:03.481809 anitya-1.7.0/anitya/static/node_modules/jquery/src/ajax/var/location.js
--rw-r--r--   0        0        0       72 2022-11-14 15:08:03.482809 anitya-1.7.0/anitya/static/node_modules/jquery/src/ajax/var/nonce.js
--rw-r--r--   0        0        0       60 2022-11-14 15:08:03.492809 anitya-1.7.0/anitya/static/node_modules/jquery/src/ajax/var/rquery.js
--rw-r--r--   0        0        0     4355 2022-11-14 15:08:03.521809 anitya-1.7.0/anitya/static/node_modules/jquery/src/ajax/xhr.js
--rw-r--r--   0        0        0    22924 2022-11-14 15:08:03.421809 anitya-1.7.0/anitya/static/node_modules/jquery/src/ajax.js
--rw-r--r--   0        0        0     3272 2022-11-14 15:08:03.425809 anitya-1.7.0/anitya/static/node_modules/jquery/src/attributes/attr.js
--rw-r--r--   0        0        0     4527 2022-11-14 15:08:03.428809 anitya-1.7.0/anitya/static/node_modules/jquery/src/attributes/classes.js
--rw-r--r--   0        0        0     2857 2022-11-14 15:08:03.486809 anitya-1.7.0/anitya/static/node_modules/jquery/src/attributes/prop.js
--rw-r--r--   0        0        0      786 2022-11-14 15:08:03.513809 anitya-1.7.0/anitya/static/node_modules/jquery/src/attributes/support.js
--rw-r--r--   0        0        0     4261 2022-11-14 15:08:03.519809 anitya-1.7.0/anitya/static/node_modules/jquery/src/attributes/val.js
--rw-r--r--   0        0        0      217 2022-11-14 15:08:03.425809 anitya-1.7.0/anitya/static/node_modules/jquery/src/attributes.js
--rw-r--r--   0        0        0     5552 2022-11-14 15:08:03.427809 anitya-1.7.0/anitya/static/node_modules/jquery/src/callbacks.js
--rw-r--r--   0        0        0     1160 2022-11-14 15:08:03.449809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/DOMEval.js
--rw-r--r--   0        0        0     1314 2022-11-14 15:08:03.414809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/access.js
--rw-r--r--   0        0        0      550 2022-11-14 15:08:03.427809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/camelCase.js
--rw-r--r--   0        0        0     3345 2022-11-14 15:08:03.460809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/init.js
--rw-r--r--   0        0        0      789 2022-11-14 15:08:03.461809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/isAttached.js
--rw-r--r--   0        0        0      176 2022-11-14 15:08:03.482809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/nodeName.js
--rw-r--r--   0        0        0     1604 2022-11-14 15:08:03.485809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/parseHTML.js
--rw-r--r--   0        0        0      739 2022-11-14 15:08:03.486809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/parseXML.js
--rw-r--r--   0        0        0     2268 2022-11-14 15:08:03.489809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/ready-no-deferred.js
--rw-r--r--   0        0        0     2101 2022-11-14 15:08:03.490809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/ready.js
--rw-r--r--   0        0        0      168 2022-11-14 15:08:03.490809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/readyException.js
--rw-r--r--   0        0        0      362 2022-11-14 15:08:03.512809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/stripAndCollapse.js
--rw-r--r--   0        0        0      631 2022-11-14 15:08:03.513809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/support.js
--rw-r--r--   0        0        0      379 2022-11-14 15:08:03.516809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/toType.js
--rw-r--r--   0        0        0      244 2022-11-14 15:08:03.494809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core/var/rsingleTag.js
--rw-r--r--   0        0        0     9183 2022-11-14 15:08:03.429809 anitya-1.7.0/anitya/static/node_modules/jquery/src/core.js
--rw-r--r--   0        0        0      530 2022-11-14 15:08:03.416809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/addGetHookIf.js
--rw-r--r--   0        0        0     2002 2022-11-14 15:08:03.417809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/adjustCSS.js
--rw-r--r--   0        0        0     2191 2022-11-14 15:08:03.434809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/curCSS.js
--rw-r--r--   0        0        0      870 2022-11-14 15:08:03.454809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/finalPropName.js
--rw-r--r--   0        0        0      317 2022-11-14 15:08:03.460809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/hiddenVisibleSelectors.js
--rw-r--r--   0        0        0     2304 2022-11-14 15:08:03.499809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/showHide.js
--rw-r--r--   0        0        0     4829 2022-11-14 15:08:03.514809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/support.js
--rw-r--r--   0        0        0       88 2022-11-14 15:08:03.433809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/var/cssExpand.js
--rw-r--r--   0        0        0      409 2022-11-14 15:08:03.458809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/var/getStyles.js
--rw-r--r--   0        0        0     1284 2022-11-14 15:08:03.461809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/var/isHiddenWithinTree.js
--rw-r--r--   0        0        0      123 2022-11-14 15:08:03.487809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/var/rboxStyle.js
--rw-r--r--   0        0        0       57 2022-11-14 15:08:03.489809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/var/rcustomProp.js
--rw-r--r--   0        0        0      131 2022-11-14 15:08:03.492809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/var/rnumnonpx.js
--rw-r--r--   0        0        0      501 2022-11-14 15:08:03.515809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css/var/swap.js
--rw-r--r--   0        0        0    14195 2022-11-14 15:08:03.430809 anitya-1.7.0/anitya/static/node_modules/jquery/src/css.js
--rw-r--r--   0        0        0     3956 2022-11-14 15:08:03.436809 anitya-1.7.0/anitya/static/node_modules/jquery/src/data/Data.js
--rw-r--r--   0        0        0      318 2022-11-14 15:08:03.412809 anitya-1.7.0/anitya/static/node_modules/jquery/src/data/var/acceptData.js
--rw-r--r--   0        0        0       84 2022-11-14 15:08:03.437809 anitya-1.7.0/anitya/static/node_modules/jquery/src/data/var/dataPriv.js
--rw-r--r--   0        0        0       84 2022-11-14 15:08:03.437809 anitya-1.7.0/anitya/static/node_modules/jquery/src/data/var/dataUser.js
--rw-r--r--   0        0        0     4325 2022-11-14 15:08:03.435809 anitya-1.7.0/anitya/static/node_modules/jquery/src/data.js
--rw-r--r--   0        0        0      640 2022-11-14 15:08:03.452809 anitya-1.7.0/anitya/static/node_modules/jquery/src/deferred/exceptionHook.js
--rw-r--r--   0        0        0    11007 2022-11-14 15:08:03.438809 anitya-1.7.0/anitya/static/node_modules/jquery/src/deferred.js
--rw-r--r--   0        0        0      296 2022-11-14 15:08:03.419809 anitya-1.7.0/anitya/static/node_modules/jquery/src/deprecated/ajax-event-alias.js
--rw-r--r--   0        0        0     1140 2022-11-14 15:08:03.451809 anitya-1.7.0/anitya/static/node_modules/jquery/src/deprecated/event.js
--rw-r--r--   0        0        0     2406 2022-11-14 15:08:03.440809 anitya-1.7.0/anitya/static/node_modules/jquery/src/deprecated.js
--rw-r--r--   0        0        0     1756 2022-11-14 15:08:03.441809 anitya-1.7.0/anitya/static/node_modules/jquery/src/dimensions.js
--rw-r--r--   0        0        0     3291 2022-11-14 15:08:03.518809 anitya-1.7.0/anitya/static/node_modules/jquery/src/effects/Tween.js
--rw-r--r--   0        0        0      244 2022-11-14 15:08:03.423809 anitya-1.7.0/anitya/static/node_modules/jquery/src/effects/animatedSelector.js
--rw-r--r--   0        0        0    17417 2022-11-14 15:08:03.450809 anitya-1.7.0/anitya/static/node_modules/jquery/src/effects.js
--rw-r--r--   0        0        0     1665 2022-11-14 15:08:03.457809 anitya-1.7.0/anitya/static/node_modules/jquery/src/event/focusin.js
--rw-r--r--   0        0        0      133 2022-11-14 15:08:03.514809 anitya-1.7.0/anitya/static/node_modules/jquery/src/event/support.js
--rw-r--r--   0        0        0     5438 2022-11-14 15:08:03.518809 anitya-1.7.0/anitya/static/node_modules/jquery/src/event/trigger.js
--rw-r--r--   0        0        0    24505 2022-11-14 15:08:03.452809 anitya-1.7.0/anitya/static/node_modules/jquery/src/event.js
--rw-r--r--   0        0        0     1024 2022-11-14 15:08:03.422809 anitya-1.7.0/anitya/static/node_modules/jquery/src/exports/amd.js
--rw-r--r--   0        0        0      628 2022-11-14 15:08:03.459809 anitya-1.7.0/anitya/static/node_modules/jquery/src/exports/global.js
--rw-r--r--   0        0        0      646 2022-11-14 15:08:03.470809 anitya-1.7.0/anitya/static/node_modules/jquery/src/jquery.js
--rw-r--r--   0        0        0      690 2022-11-14 15:08:03.409809 anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation/_evalUrl.js
--rw-r--r--   0        0        0     2490 2022-11-14 15:08:03.426809 anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation/buildFragment.js
--rw-r--r--   0        0        0      654 2022-11-14 15:08:03.457809 anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation/getAll.js
--rw-r--r--   0        0        0      381 2022-11-14 15:08:03.499809 anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation/setGlobalEval.js
--rw-r--r--   0        0        0     1244 2022-11-14 15:08:03.514809 anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation/support.js
--rw-r--r--   0        0        0       92 2022-11-14 15:08:03.493809 anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation/var/rscriptType.js
--rw-r--r--   0        0        0      304 2022-11-14 15:08:03.494809 anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation/var/rtagName.js
--rw-r--r--   0        0        0      823 2022-11-14 15:08:03.520809 anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation/wrapMap.js
--rw-r--r--   0        0        0    12674 2022-11-14 15:08:03.481809 anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation.js
--rw-r--r--   0        0        0     6828 2022-11-14 15:08:03.484809 anitya-1.7.0/anitya/static/node_modules/jquery/src/offset.js
--rw-r--r--   0        0        0      534 2022-11-14 15:08:03.439809 anitya-1.7.0/anitya/static/node_modules/jquery/src/queue/delay.js
--rw-r--r--   0        0        0     3091 2022-11-14 15:08:03.487809 anitya-1.7.0/anitya/static/node_modules/jquery/src/queue.js
--rw-r--r--   0        0        0     6463 2022-11-14 15:08:03.497809 anitya-1.7.0/anitya/static/node_modules/jquery/src/selector-native.js
--rw-r--r--   0        0        0      411 2022-11-14 15:08:03.497809 anitya-1.7.0/anitya/static/node_modules/jquery/src/selector-sizzle.js
--rw-r--r--   0        0        0       66 2022-11-14 15:08:03.498809 anitya-1.7.0/anitya/static/node_modules/jquery/src/selector.js
--rw-r--r--   0        0        0     3236 2022-11-14 15:08:03.498809 anitya-1.7.0/anitya/static/node_modules/jquery/src/serialize.js
--rw-r--r--   0        0        0     2352 2022-11-14 15:08:03.455809 anitya-1.7.0/anitya/static/node_modules/jquery/src/traversing/findFilter.js
--rw-r--r--   0        0        0      371 2022-11-14 15:08:03.447809 anitya-1.7.0/anitya/static/node_modules/jquery/src/traversing/var/dir.js
--rw-r--r--   0        0        0      128 2022-11-14 15:08:03.491809 anitya-1.7.0/anitya/static/node_modules/jquery/src/traversing/var/rneedsContext.js
--rw-r--r--   0        0        0      218 2022-11-14 15:08:03.500809 anitya-1.7.0/anitya/static/node_modules/jquery/src/traversing/var/siblings.js
--rw-r--r--   0        0        0     4692 2022-11-14 15:08:03.517809 anitya-1.7.0/anitya/static/node_modules/jquery/src/traversing.js
--rw-r--r--   0        0        0      110 2022-11-14 15:08:03.483809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/ObjectFunctionString.js
--rw-r--r--   0        0        0       54 2022-11-14 15:08:03.424809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/arr.js
--rw-r--r--   0        0        0       82 2022-11-14 15:08:03.428809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/class2type.js
--rw-r--r--   0        0        0       67 2022-11-14 15:08:03.448809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/document.js
--rw-r--r--   0        0        0      105 2022-11-14 15:08:03.448809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/documentElement.js
--rw-r--r--   0        0        0      372 2022-11-14 15:08:03.455809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/flat.js
--rw-r--r--   0        0        0       92 2022-11-14 15:08:03.456809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/fnToString.js
--rw-r--r--   0        0        0       73 2022-11-14 15:08:03.458809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/getProto.js
--rw-r--r--   0        0        0      110 2022-11-14 15:08:03.459809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/hasOwn.js
--rw-r--r--   0        0        0       82 2022-11-14 15:08:03.460809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/indexOf.js
--rw-r--r--   0        0        0      674 2022-11-14 15:08:03.461809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/isFunction.js
--rw-r--r--   0        0        0      126 2022-11-14 15:08:03.462809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/isWindow.js
--rw-r--r--   0        0        0      100 2022-11-14 15:08:03.486809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/pnum.js
--rw-r--r--   0        0        0       79 2022-11-14 15:08:03.486809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/push.js
--rw-r--r--   0        0        0       79 2022-11-14 15:08:03.488809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/rcheckableType.js
--rw-r--r--   0        0        0      136 2022-11-14 15:08:03.488809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/rcssNum.js
--rw-r--r--   0        0        0      202 2022-11-14 15:08:03.491809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/rnothtmlwhite.js
--rw-r--r--   0        0        0      174 2022-11-14 15:08:03.494809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/rtrimCSS.js
--rw-r--r--   0        0        0       80 2022-11-14 15:08:03.512809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/slice.js
--rw-r--r--   0        0        0      117 2022-11-14 15:08:03.515809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/support.js
--rw-r--r--   0        0        0      104 2022-11-14 15:08:03.516809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/toString.js
--rw-r--r--   0        0        0      125 2022-11-14 15:08:03.519809 anitya-1.7.0/anitya/static/node_modules/jquery/src/var/whitespace.js
--rw-r--r--   0        0        0     1477 2022-11-14 15:08:03.520809 anitya-1.7.0/anitya/static/node_modules/jquery/src/wrap.js
--rw-r--r--   0        0        0      115 2022-11-14 15:08:03.829810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/.github/dependabot.yml
--rw-r--r--   0        0        0     1484 2022-11-14 15:08:03.829810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/.github/workflows/test.yml
--rw-r--r--   0        0        0    14243 2022-11-14 15:08:03.819810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/AUTHORS.txt
--rw-r--r--   0        0        0     4545 2022-11-14 15:08:03.751810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/CONTRIBUTING.md
--rw-r--r--   0        0        0     1817 2022-11-14 15:08:03.824810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/LICENSE.txt
--rw-r--r--   0        0        0     2470 2022-11-14 15:08:03.751810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/README.md
--rw-r--r--   0        0        0     2262 2022-11-14 15:08:03.751810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/bower.json
--rw-r--r--   0        0        0     1241 2022-11-14 15:08:03.746810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/build/release-test.js
--rw-r--r--   0        0        0     4749 2022-11-14 15:08:03.746810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/build/release.js
--rw-r--r--   0        0        0     1108 2022-11-14 15:08:03.593809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/build/tasks/build.js
--rw-r--r--   0        0        0     3110 2022-11-14 15:08:03.750810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/build/tasks/testswarm.js
--rw-r--r--   0        0        0    60060 2022-11-14 15:08:03.413809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/build/themes
--rw-r--r--   0        0        0   529159 2022-11-14 15:08:03.637810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/jquery-ui.js
--rw-r--r--   0        0        0   255084 2022-11-14 15:08:03.640810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/jquery-ui.min.js
--rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.792810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     7126 2022-11-14 15:08:03.795810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.797810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.797810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.806810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.814810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36099 2022-11-14 15:08:03.424809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/jquery-ui.css
--rw-r--r--   0        0        0    30778 2022-11-14 15:08:03.525809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/jquery-ui.min.css
--rw-r--r--   0        0        0    17432 2022-11-14 15:08:03.565809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/theme.css
--rw-r--r--   0        0        0      435 2022-11-14 15:08:03.756810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_diagonals-thick_8_333333_40x40.png
--rw-r--r--   0        0        0      375 2022-11-14 15:08:03.768810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_glass_40_111111_1x400.png
--rw-r--r--   0        0        0      375 2022-11-14 15:08:03.769810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_glass_55_1c1c1c_1x400.png
--rw-r--r--   0        0        0      367 2022-11-14 15:08:03.778810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_highlight-hard_100_f9f9f9_1x100.png
--rw-r--r--   0        0        0      368 2022-11-14 15:08:03.779810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_highlight-hard_40_aaaaaa_1x100.png
--rw-r--r--   0        0        0      379 2022-11-14 15:08:03.783810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_highlight-soft_50_aaaaaa_1x100.png
--rw-r--r--   0        0        0      434 2022-11-14 15:08:03.785810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_inset-hard_45_cd0a0a_1x100.png
--rw-r--r--   0        0        0      419 2022-11-14 15:08:03.785810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_inset-hard_55_ffeb80_1x100.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_4ca300_256x240.png
--rw-r--r--   0        0        0     7144 2022-11-14 15:08:03.802810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_bbbbbb_256x240.png
--rw-r--r--   0        0        0     7063 2022-11-14 15:08:03.810810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ededed_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ffcf29_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.814810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36800 2022-11-14 15:08:03.427809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/jquery-ui.css
--rw-r--r--   0        0        0    31457 2022-11-14 15:08:03.526809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/jquery-ui.min.css
--rw-r--r--   0        0        0    18133 2022-11-14 15:08:03.566809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/theme.css
--rw-r--r--   0        0        0      523 2022-11-14 15:08:03.756810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_diagonals-thick_75_f3d8d8_40x40.png
--rw-r--r--   0        0        0      318 2022-11-14 15:08:03.760810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_dots-small_65_a6a6a6_2x2.png
--rw-r--r--   0        0        0      450 2022-11-14 15:08:03.770810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_glass_55_fbf8ee_1x400.png
--rw-r--r--   0        0        0      368 2022-11-14 15:08:03.778810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_highlight-hard_100_eeeeee_1x100.png
--rw-r--r--   0        0        0      368 2022-11-14 15:08:03.778810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_highlight-hard_100_f6f6f6_1x100.png
--rw-r--r--   0        0        0      437 2022-11-14 15:08:03.781810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_highlight-soft_15_cc0000_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.787810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_004276_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.806810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.814810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36693 2022-11-14 15:08:03.430809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/jquery-ui.css
--rw-r--r--   0        0        0    31359 2022-11-14 15:08:03.527809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/jquery-ui.min.css
--rw-r--r--   0        0        0    18026 2022-11-14 15:08:03.568809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/theme.css
--rw-r--r--   0        0        0      432 2022-11-14 15:08:03.757810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_diagonals-thick_90_eeeeee_40x40.png
--rw-r--r--   0        0        0      460 2022-11-14 15:08:03.765810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_glass_100_e4f1fb_1x400.png
--rw-r--r--   0        0        0      446 2022-11-14 15:08:03.769810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_glass_50_3baae3_1x400.png
--rw-r--r--   0        0        0      456 2022-11-14 15:08:03.772810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_glass_80_d7ebf9_1x400.png
--rw-r--r--   0        0        0      442 2022-11-14 15:08:03.778810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_highlight-hard_100_f2f5f7_1x100.png
--rw-r--r--   0        0        0      362 2022-11-14 15:08:03.780810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_highlight-hard_70_000000_1x100.png
--rw-r--r--   0        0        0      497 2022-11-14 15:08:03.780810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_highlight-soft_100_deedf7_1x100.png
--rw-r--r--   0        0        0      419 2022-11-14 15:08:03.782810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_highlight-soft_25_ffef8f_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.790810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_2694e8_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_3d80b3_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_72a7cf_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.814810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36850 2022-11-14 15:08:03.437809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/jquery-ui.css
--rw-r--r--   0        0        0    31543 2022-11-14 15:08:03.528809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/jquery-ui.min.css
--rw-r--r--   0        0        0    18183 2022-11-14 15:08:03.570809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/theme.css
--rw-r--r--   0        0        0      426 2022-11-14 15:08:03.768810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_glass_40_ffc73d_1x400.png
--rw-r--r--   0        0        0      433 2022-11-14 15:08:03.779810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-hard_20_0972a5_1x100.png
--rw-r--r--   0        0        0      453 2022-11-14 15:08:03.782810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-soft_33_003147_1x100.png
--rw-r--r--   0        0        0      394 2022-11-14 15:08:03.783810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-soft_35_222222_1x100.png
--rw-r--r--   0        0        0      380 2022-11-14 15:08:03.783810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-soft_44_444444_1x100.png
--rw-r--r--   0        0        0      387 2022-11-14 15:08:03.784810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-soft_80_eeeeee_1x100.png
--rw-r--r--   0        0        0      430 2022-11-14 15:08:03.787810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_loop_25_000000_21x21.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_4b8e0b_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_a83300_256x240.png
--rw-r--r--   0        0        0     7086 2022-11-14 15:08:03.806810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_cccccc_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.815810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36796 2022-11-14 15:08:03.441809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/jquery-ui.css
--rw-r--r--   0        0        0    31444 2022-11-14 15:08:03.530809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/jquery-ui.min.css
--rw-r--r--   0        0        0    18129 2022-11-14 15:08:03.571809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/theme.css
--rw-r--r--   0        0        0      534 2022-11-14 15:08:03.755810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_diagonals-thick_15_0b3e6f_40x40.png
--rw-r--r--   0        0        0      347 2022-11-14 15:08:03.759810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_dots-medium_30_0b58a2_4x4.png
--rw-r--r--   0        0        0      318 2022-11-14 15:08:03.759810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_dots-small_20_333333_2x2.png
--rw-r--r--   0        0        0      328 2022-11-14 15:08:03.759810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_dots-small_30_a32d00_2x2.png
--rw-r--r--   0        0        0      334 2022-11-14 15:08:03.760810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_dots-small_40_00498f_2x2.png
--rw-r--r--   0        0        0     4042 2022-11-14 15:08:03.774810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_gloss-wave_20_111111_500x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.787810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_00498f_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_98d2fb_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_9ccdfc_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.815810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36666 2022-11-14 15:08:03.451809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/jquery-ui.css
--rw-r--r--   0        0        0    31341 2022-11-14 15:08:03.531809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/jquery-ui.min.css
--rw-r--r--   0        0        0    17999 2022-11-14 15:08:03.572809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/theme.css
--rw-r--r--   0        0        0     6051 2022-11-14 15:08:03.774810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_gloss-wave_30_3d3644_500x100.png
--rw-r--r--   0        0        0      452 2022-11-14 15:08:03.780810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_highlight-soft_100_dcd9de_1x100.png
--rw-r--r--   0        0        0      483 2022-11-14 15:08:03.781810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_highlight-soft_100_eae6ea_1x100.png
--rw-r--r--   0        0        0      472 2022-11-14 15:08:03.782810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_highlight-soft_25_30273a_1x100.png
--rw-r--r--   0        0        0      457 2022-11-14 15:08:03.783810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_highlight-soft_45_5f5964_1x100.png
--rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.792810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_734d99_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_8d78a5_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_a8a3ae_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_ebccce_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.815810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36720 2022-11-14 15:08:03.455809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/jquery-ui.css
--rw-r--r--   0        0        0    31404 2022-11-14 15:08:03.534809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/jquery-ui.min.css
--rw-r--r--   0        0        0    18053 2022-11-14 15:08:03.573809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/theme.css
--rw-r--r--   0        0        0      452 2022-11-14 15:08:03.753810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-small_25_c5ddfc_40x40.png
--rw-r--r--   0        0        0      527 2022-11-14 15:08:03.755810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_20_e69700_40x40.png
--rw-r--r--   0        0        0      519 2022-11-14 15:08:03.756810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_22_1484e6_40x40.png
--rw-r--r--   0        0        0      516 2022-11-14 15:08:03.756810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_26_2293f7_40x40.png
--rw-r--r--   0        0        0      377 2022-11-14 15:08:03.781810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_highlight-soft_100_f9f9f9_1x100.png
--rw-r--r--   0        0        0      366 2022-11-14 15:08:03.785810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_inset-hard_100_eeeeee_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_0a82eb_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_0b54d5_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.795810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_5fa5e3_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_fcdd4a_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.815810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36824 2022-11-14 15:08:03.459809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/jquery-ui.css
--rw-r--r--   0        0        0    31486 2022-11-14 15:08:03.536809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/jquery-ui.min.css
--rw-r--r--   0        0        0    18157 2022-11-14 15:08:03.575809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/theme.css
--rw-r--r--   0        0        0      317 2022-11-14 15:08:03.771810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0        0        0      382 2022-11-14 15:08:03.781810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-bg_highlight-soft_100_f6f6f6_1x100.png
--rw-r--r--   0        0        0      445 2022-11-14 15:08:03.782810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-bg_highlight-soft_25_0073ea_1x100.png
--rw-r--r--   0        0        0      391 2022-11-14 15:08:03.783810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-bg_highlight-soft_50_dddddd_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_0073ea_256x240.png
--rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.792810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.795810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_666666_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_ff0084_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.816810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36570 2022-11-14 15:08:03.462809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/jquery-ui.css
--rw-r--r--   0        0        0    31215 2022-11-14 15:08:03.538809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/jquery-ui.min.css
--rw-r--r--   0        0        0    17903 2022-11-14 15:08:03.575809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/theme.css
--rw-r--r--   0        0        0      442 2022-11-14 15:08:03.754810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_diagonals-small_40_db4865_40x40.png
--rw-r--r--   0        0        0      443 2022-11-14 15:08:03.754810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_diagonals-small_50_93c3cd_40x40.png
--rw-r--r--   0        0        0      440 2022-11-14 15:08:03.754810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_diagonals-small_50_ff3853_40x40.png
--rw-r--r--   0        0        0      443 2022-11-14 15:08:03.754810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_diagonals-small_75_ccd232_40x40.png
--rw-r--r--   0        0        0      335 2022-11-14 15:08:03.759810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_dots-medium_80_ffff38_4x4.png
--rw-r--r--   0        0        0      333 2022-11-14 15:08:03.760810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_dots-small_35_35414f_2x2.png
--rw-r--r--   0        0        0      474 2022-11-14 15:08:03.787810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_white-lines_85_f7f7ba_40x100.png
--rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.793810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.798810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_88a206_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.804810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_c02669_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_e1e463_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.814810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_ffeb33_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36804 2022-11-14 15:08:03.466809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/jquery-ui.css
--rw-r--r--   0        0        0    31500 2022-11-14 15:08:03.540809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/jquery-ui.min.css
--rw-r--r--   0        0        0    18137 2022-11-14 15:08:03.576810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/theme.css
--rw-r--r--   0        0        0      464 2022-11-14 15:08:03.766810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_glass_100_f5f0e5_1x400.png
--rw-r--r--   0        0        0      445 2022-11-14 15:08:03.767810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_glass_25_cb842e_1x400.png
--rw-r--r--   0        0        0      464 2022-11-14 15:08:03.772810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_glass_70_ede4d4_1x400.png
--rw-r--r--   0        0        0      437 2022-11-14 15:08:03.778810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_highlight-hard_100_f4f0ec_1x100.png
--rw-r--r--   0        0        0      424 2022-11-14 15:08:03.780810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_highlight-hard_65_fee4bd_1x100.png
--rw-r--r--   0        0        0      433 2022-11-14 15:08:03.780810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_highlight-hard_75_f5f5b5_1x100.png
--rw-r--r--   0        0        0      513 2022-11-14 15:08:03.786810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_inset-soft_100_f4f0ec_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.805810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_c47a23_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.805810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_cb672b_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.810810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_f08000_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_f35f07_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_ff7519_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36789 2022-11-14 15:08:03.468809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/jquery-ui.css
--rw-r--r--   0        0        0    31503 2022-11-14 15:08:03.541809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/jquery-ui.min.css
--rw-r--r--   0        0        0    18122 2022-11-14 15:08:03.577809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/theme.css
--rw-r--r--   0        0        0      317 2022-11-14 15:08:03.752810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_diagonals-small_0_aaaaaa_40x40.png
--rw-r--r--   0        0        0      435 2022-11-14 15:08:03.755810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_diagonals-thick_15_444444_40x40.png
--rw-r--r--   0        0        0      521 2022-11-14 15:08:03.757810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_diagonals-thick_95_ffdc2e_40x40.png
--rw-r--r--   0        0        0      446 2022-11-14 15:08:03.770810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_glass_55_fbf5d0_1x400.png
--rw-r--r--   0        0        0      434 2022-11-14 15:08:03.779810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_highlight-hard_30_285c00_1x100.png
--rw-r--r--   0        0        0      455 2022-11-14 15:08:03.782810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_highlight-soft_33_3a8104_1x100.png
--rw-r--r--   0        0        0      461 2022-11-14 15:08:03.783810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_highlight-soft_50_4eb305_1x100.png
--rw-r--r--   0        0        0      469 2022-11-14 15:08:03.783810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_highlight-soft_60_4ca20b_1x100.png
--rw-r--r--   0        0        0      476 2022-11-14 15:08:03.786810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_inset-soft_10_285c00_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_4eb305_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_72b42d_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36964 2022-11-14 15:08:03.471809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/jquery-ui.css
--rw-r--r--   0        0        0    31647 2022-11-14 15:08:03.542809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/jquery-ui.min.css
--rw-r--r--   0        0        0    18297 2022-11-14 15:08:03.578809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/theme.css
--rw-r--r--   0        0        0      445 2022-11-14 15:08:03.767810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_glass_15_5f391b_1x400.png
--rw-r--r--   0        0        0     5903 2022-11-14 15:08:03.774810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_20_1c160d_500x100.png
--rw-r--r--   0        0        0     5962 2022-11-14 15:08:03.774810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_25_453326_500x100.png
--rw-r--r--   0        0        0     6024 2022-11-14 15:08:03.775810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_30_44372c_500x100.png
--rw-r--r--   0        0        0      485 2022-11-14 15:08:03.781810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_highlight-soft_20_201913_1x100.png
--rw-r--r--   0        0        0      453 2022-11-14 15:08:03.782810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_highlight-soft_20_619226_1x100.png
--rw-r--r--   0        0        0      490 2022-11-14 15:08:03.786810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_inset-soft_10_201913_1x100.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_9bcc60_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_add978_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_e3ddc9_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_f1fd86_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36822 2022-11-14 15:08:03.474809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/jquery-ui.css
--rw-r--r--   0        0        0    31521 2022-11-14 15:08:03.543809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/jquery-ui.min.css
--rw-r--r--   0        0        0    18155 2022-11-14 15:08:03.579810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/theme.css
--rw-r--r--   0        0        0      376 2022-11-14 15:08:03.766810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_glass_100_f8f8f8_1x400.png
--rw-r--r--   0        0        0      375 2022-11-14 15:08:03.767810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_glass_35_dddddd_1x400.png
--rw-r--r--   0        0        0      375 2022-11-14 15:08:03.771810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_glass_60_eeeeee_1x400.png
--rw-r--r--   0        0        0      362 2022-11-14 15:08:03.785810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_inset-hard_75_999999_1x100.png
--rw-r--r--   0        0        0      381 2022-11-14 15:08:03.787810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_inset-soft_50_c9c9c9_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_3383bb_256x240.png
--rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.793810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_70b2e1_256x240.png
--rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.799810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_999999_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_fbc856_256x240.png
--rw-r--r--   0        0        0    36646 2022-11-14 15:08:03.477809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/jquery-ui.css
--rw-r--r--   0        0        0    31288 2022-11-14 15:08:03.544809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/jquery-ui.min.css
--rw-r--r--   0        0        0    17979 2022-11-14 15:08:03.579810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/theme.css
--rw-r--r--   0        0        0      406 2022-11-14 15:08:03.752810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_diagonal-maze_20_6e4f1c_10x10.png
--rw-r--r--   0        0        0      353 2022-11-14 15:08:03.752810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_diagonal-maze_40_000000_10x10.png
--rw-r--r--   0        0        0    10869 2022-11-14 15:08:03.760810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_10_eceadf_60x60.png
--rw-r--r--   0        0        0    10014 2022-11-14 15:08:03.762810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_10_f8f7f6_60x60.png
--rw-r--r--   0        0        0    10639 2022-11-14 15:08:03.763810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_eceadf_60x60.png
--rw-r--r--   0        0        0    11001 2022-11-14 15:08:03.764810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_f7f3de_60x60.png
--rw-r--r--   0        0        0     4314 2022-11-14 15:08:03.764810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_ffffff_60x60.png
--rw-r--r--   0        0        0    14555 2022-11-14 15:08:03.764810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_65_654b24_60x60.png
--rw-r--r--   0        0        0    11987 2022-11-14 15:08:03.764810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_68_b83400_60x60.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_3572ac_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.798810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_8c291d_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.802810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_b83400_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_fbdb93_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36906 2022-11-14 15:08:03.480809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/jquery-ui.css
--rw-r--r--   0        0        0    31611 2022-11-14 15:08:03.545809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/jquery-ui.min.css
--rw-r--r--   0        0        0    18239 2022-11-14 15:08:03.580809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/theme.css
--rw-r--r--   0        0        0      446 2022-11-14 15:08:03.772810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_glass_75_d0e5f5_1x400.png
--rw-r--r--   0        0        0      451 2022-11-14 15:08:03.773810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_glass_85_dfeffc_1x400.png
--rw-r--r--   0        0        0      442 2022-11-14 15:08:03.773810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0        0        0     5934 2022-11-14 15:08:03.776810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_gloss-wave_55_5c9ccc_500x100.png
--rw-r--r--   0        0        0      443 2022-11-14 15:08:03.785810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_inset-hard_100_f5f8f9_1x100.png
--rw-r--r--   0        0        0      402 2022-11-14 15:08:03.785810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_inset-hard_100_fcfdfd_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.789810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_217bc0_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_469bdd_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_6da8d5_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_d8e7f3_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_f9bd01_256x240.png
--rw-r--r--   0        0        0    36735 2022-11-14 15:08:03.482809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/jquery-ui.css
--rw-r--r--   0        0        0    31443 2022-11-14 15:08:03.547809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/jquery-ui.min.css
--rw-r--r--   0        0        0    18068 2022-11-14 15:08:03.581809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/theme.css
--rw-r--r--   0        0        0      445 2022-11-14 15:08:03.770810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0        0        0      317 2022-11-14 15:08:03.771810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0        0        0      375 2022-11-14 15:08:03.772810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0        0        0      376 2022-11-14 15:08:03.772810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0        0        0      442 2022-11-14 15:08:03.773810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0        0        0      377 2022-11-14 15:08:03.784810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.790810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.794810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.798810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0    36662 2022-11-14 15:08:03.486809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/jquery-ui.css
--rw-r--r--   0        0        0    31340 2022-11-14 15:08:03.548809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/jquery-ui.min.css
--rw-r--r--   0        0        0    17995 2022-11-14 15:08:03.582810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/theme.css
--rw-r--r--   0        0        0      443 2022-11-14 15:08:03.771810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_glass_55_fcf0ba_1x400.png
--rw-r--r--   0        0        0     5869 2022-11-14 15:08:03.773810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_gloss-wave_100_ece8da_500x100.png
--rw-r--r--   0        0        0      446 2022-11-14 15:08:03.778810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-hard_100_f5f3e5_1x100.png
--rw-r--r--   0        0        0      431 2022-11-14 15:08:03.779810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-hard_100_fafaf4_1x100.png
--rw-r--r--   0        0        0      432 2022-11-14 15:08:03.779810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-hard_15_459e00_1x100.png
--rw-r--r--   0        0        0      369 2022-11-14 15:08:03.780810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-hard_95_cccccc_1x100.png
--rw-r--r--   0        0        0      463 2022-11-14 15:08:03.782810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-soft_25_67b021_1x100.png
--rw-r--r--   0        0        0      461 2022-11-14 15:08:03.784810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-soft_95_ffedad_1x100.png
--rw-r--r--   0        0        0      432 2022-11-14 15:08:03.786810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_inset-soft_15_2b2922_1x100.png
--rw-r--r--   0        0        0     7169 2022-11-14 15:08:03.798810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_808080_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.798810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_847e71_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_8DC262_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0     7062 2022-11-14 15:08:03.810810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_eeeeee_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.818810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36912 2022-11-14 15:08:03.489809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/jquery-ui.css
--rw-r--r--   0        0        0    31623 2022-11-14 15:08:03.549809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/jquery-ui.min.css
--rw-r--r--   0        0        0    18245 2022-11-14 15:08:03.583809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/theme.css
--rw-r--r--   0        0        0      455 2022-11-14 15:08:03.769810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_glass_45_0078ae_1x400.png
--rw-r--r--   0        0        0      455 2022-11-14 15:08:03.770810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_glass_55_f8da4e_1x400.png
--rw-r--r--   0        0        0      458 2022-11-14 15:08:03.772810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_glass_75_79c9ec_1x400.png
--rw-r--r--   0        0        0     5974 2022-11-14 15:08:03.775810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_45_e14f1c_500x100.png
--rw-r--r--   0        0        0     6016 2022-11-14 15:08:03.776810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_50_6eac2c_500x100.png
--rw-r--r--   0        0        0     6087 2022-11-14 15:08:03.777810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_75_2191c0_500x100.png
--rw-r--r--   0        0        0      402 2022-11-14 15:08:03.785810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_inset-hard_100_fcfdfd_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_0078ae_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_056b93_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_d8e7f3_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_e0fdff_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_f5e175_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_f7a50d_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_fcd113_256x240.png
--rw-r--r--   0        0        0    36755 2022-11-14 15:08:03.493809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/jquery-ui.css
--rw-r--r--   0        0        0    31441 2022-11-14 15:08:03.550809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/jquery-ui.min.css
--rw-r--r--   0        0        0    18088 2022-11-14 15:08:03.584809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/theme.css
--rw-r--r--   0        0        0      492 2022-11-14 15:08:03.752810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_diagonals-medium_20_d34d17_40x40.png
--rw-r--r--   0        0        0     6000 2022-11-14 15:08:03.775810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_45_817865_500x100.png
--rw-r--r--   0        0        0     5960 2022-11-14 15:08:03.777810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_60_fece2f_500x100.png
--rw-r--r--   0        0        0     5653 2022-11-14 15:08:03.777810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_70_ffdd57_500x100.png
--rw-r--r--   0        0        0     5499 2022-11-14 15:08:03.777810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_90_fff9e5_500x100.png
--rw-r--r--   0        0        0      453 2022-11-14 15:08:03.781810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_highlight-soft_100_feeebd_1x100.png
--rw-r--r--   0        0        0      313 2022-11-14 15:08:03.787810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_inset-soft_30_ffffff_1x100.png
--rw-r--r--   0        0        0     7126 2022-11-14 15:08:03.791810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_3d3d3d_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.804810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_bd7b00_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_d19405_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_eb990f_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.810810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_ed9f26_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_fadc7a_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.814810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_ffe180_256x240.png
--rw-r--r--   0        0        0    36805 2022-11-14 15:08:03.498809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/jquery-ui.css
--rw-r--r--   0        0        0    31510 2022-11-14 15:08:03.550809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/jquery-ui.min.css
--rw-r--r--   0        0        0    18138 2022-11-14 15:08:03.585809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/theme.css
--rw-r--r--   0        0        0      417 2022-11-14 15:08:03.757810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_10_4f4221_10x8.png
--rw-r--r--   0        0        0      420 2022-11-14 15:08:03.758810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_20_372806_10x8.png
--rw-r--r--   0        0        0      422 2022-11-14 15:08:03.758810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_25_675423_10x8.png
--rw-r--r--   0        0        0      423 2022-11-14 15:08:03.758810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_25_d5ac5d_10x8.png
--rw-r--r--   0        0        0      420 2022-11-14 15:08:03.758810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_8_261803_10x8.png
--rw-r--r--   0        0        0      420 2022-11-14 15:08:03.758810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_8_443113_10x8.png
--rw-r--r--   0        0        0      424 2022-11-14 15:08:03.780810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_highlight-hard_65_fee4bd_1x100.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_070603_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_e8e2b5_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_e9cd86_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.810810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_efec9f_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_f2ec64_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_f9f2bd_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_ff7519_256x240.png
--rw-r--r--   0        0        0    36812 2022-11-14 15:08:03.504809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/jquery-ui.css
--rw-r--r--   0        0        0    31541 2022-11-14 15:08:03.551809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/jquery-ui.min.css
--rw-r--r--   0        0        0    18145 2022-11-14 15:08:03.586809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/theme.css
--rw-r--r--   0        0        0      373 2022-11-14 15:08:03.754810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_diagonals-small_50_262626_40x40.png
--rw-r--r--   0        0        0      374 2022-11-14 15:08:03.768810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_glass_40_0a0a0a_1x400.png
--rw-r--r--   0        0        0      458 2022-11-14 15:08:03.770810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_glass_55_f1fbe5_1x400.png
--rw-r--r--   0        0        0      375 2022-11-14 15:08:03.771810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_glass_60_000000_1x400.png
--rw-r--r--   0        0        0     4412 2022-11-14 15:08:03.776810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_55_000000_500x100.png
--rw-r--r--   0        0        0     6050 2022-11-14 15:08:03.777810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_85_9fda58_500x100.png
--rw-r--r--   0        0        0     5908 2022-11-14 15:08:03.778810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_95_f6ecd5_500x100.png
--rw-r--r--   0        0        0     5634 2022-11-14 15:08:03.787810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_000000_256x240.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_1f1f1f_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_9fda58_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.802810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_b8ec79_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.818810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36792 2022-11-14 15:08:03.513809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/jquery-ui.css
--rw-r--r--   0        0        0    31488 2022-11-14 15:08:03.552809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/jquery-ui.min.css
--rw-r--r--   0        0        0    18125 2022-11-14 15:08:03.587809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/theme.css
--rw-r--r--   0        0        0      370 2022-11-14 15:08:03.767810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_glass_20_555555_1x400.png
--rw-r--r--   0        0        0      452 2022-11-14 15:08:03.767810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_glass_40_0078a3_1x400.png
--rw-r--r--   0        0        0      426 2022-11-14 15:08:03.768810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_glass_40_ffc73d_1x400.png
--rw-r--r--   0        0        0     4028 2022-11-14 15:08:03.774810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_gloss-wave_25_333333_500x100.png
--rw-r--r--   0        0        0      387 2022-11-14 15:08:03.784810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_highlight-soft_80_eeeeee_1x100.png
--rw-r--r--   0        0        0      364 2022-11-14 15:08:03.786810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_inset-soft_25_000000_1x100.png
--rw-r--r--   0        0        0      450 2022-11-14 15:08:03.786810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_inset-soft_30_f58400_1x100.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.790810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_4b8e0b_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_a83300_256x240.png
--rw-r--r--   0        0        0     7086 2022-11-14 15:08:03.806810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_cccccc_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.818810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36760 2022-11-14 15:08:03.517809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/jquery-ui.css
--rw-r--r--   0        0        0    31408 2022-11-14 15:08:03.555809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/jquery-ui.min.css
--rw-r--r--   0        0        0    18093 2022-11-14 15:08:03.588809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/theme.css
--rw-r--r--   0        0        0      528 2022-11-14 15:08:03.755810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_diagonals-thick_18_b81900_40x40.png
--rw-r--r--   0        0        0      436 2022-11-14 15:08:03.755810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_diagonals-thick_20_666666_40x40.png
--rw-r--r--   0        0        0      376 2022-11-14 15:08:03.766810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_glass_100_f6f6f6_1x400.png
--rw-r--r--   0        0        0      458 2022-11-14 15:08:03.766810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_glass_100_fdf5ce_1x400.png
--rw-r--r--   0        0        0      317 2022-11-14 15:08:03.771810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0        0        0     5925 2022-11-14 15:08:03.775810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_gloss-wave_35_f6a828_500x100.png
--rw-r--r--   0        0        0      394 2022-11-14 15:08:03.781810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_highlight-soft_100_eeeeee_1x100.png
--rw-r--r--   0        0        0      438 2022-11-14 15:08:03.784810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_highlight-soft_75_ffe45c_1x100.png
--rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.790810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_222222_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.790810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_228ef1_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.810810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ef8c08_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ffd27a_256x240.png
--rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.819810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    36922 2022-11-14 15:08:03.520809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/jquery-ui.css
--rw-r--r--   0        0        0    31606 2022-11-14 15:08:03.556809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/jquery-ui.min.css
--rw-r--r--   0        0        0    18255 2022-11-14 15:08:03.588809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/theme.css
--rw-r--r--   0        0        0      442 2022-11-14 15:08:03.773810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0        0        0     4083 2022-11-14 15:08:03.774810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_gloss-wave_16_121212_500x100.png
--rw-r--r--   0        0        0      363 2022-11-14 15:08:03.779810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_highlight-hard_15_888888_1x100.png
--rw-r--r--   0        0        0      363 2022-11-14 15:08:03.779810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_highlight-hard_55_555555_1x100.png
--rw-r--r--   0        0        0      378 2022-11-14 15:08:03.783810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_highlight-soft_35_adadad_1x100.png
--rw-r--r--   0        0        0      394 2022-11-14 15:08:03.784810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_highlight-soft_60_dddddd_1x100.png
--rw-r--r--   0        0        0      374 2022-11-14 15:08:03.786810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_inset-soft_15_121212_1x100.png
--rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.795810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_666666_256x240.png
--rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.797810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     7127 2022-11-14 15:08:03.800810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_aaaaaa_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.805810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_c98000_256x240.png
--rw-r--r--   0        0        0     7086 2022-11-14 15:08:03.806810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_cccccc_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_f29a00_256x240.png
--rw-r--r--   0        0        0    36802 2022-11-14 15:08:03.524809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/jquery-ui.css
--rw-r--r--   0        0        0    31448 2022-11-14 15:08:03.557809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/jquery-ui.min.css
--rw-r--r--   0        0        0    18135 2022-11-14 15:08:03.589810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/theme.css
--rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.410809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/globalize/LICENSE
--rw-r--r--   0        0        0     1898 2022-11-14 15:08:03.633810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/globalize/globalize.culture.de-DE.js
--rw-r--r--   0        0        0     2859 2022-11-14 15:08:03.633810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/globalize/globalize.culture.ja-JP.js
--rw-r--r--   0        0        0    45705 2022-11-14 15:08:03.633810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/globalize/globalize.js
--rw-r--r--   0        0        0     1097 2022-11-14 15:08:03.823810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery/LICENSE.txt
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery/MIT-LICENSE.txt
--rw-r--r--   0        0        0   288580 2022-11-14 15:08:03.741810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.824810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.0/MIT-LICENSE.txt
--rw-r--r--   0        0        0   273809 2022-11-14 15:08:03.644810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.824810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.1/MIT-LICENSE.txt
--rw-r--r--   0        0        0   274080 2022-11-14 15:08:03.650810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.1/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.824810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.2/MIT-LICENSE.txt
--rw-r--r--   0        0        0   273199 2022-11-14 15:08:03.655810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.2/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.0/MIT-LICENSE.txt
--rw-r--r--   0        0        0   282944 2022-11-14 15:08:03.658810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.1/MIT-LICENSE.txt
--rw-r--r--   0        0        0   282766 2022-11-14 15:08:03.662810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.1/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.2/MIT-LICENSE.txt
--rw-r--r--   0        0        0   284184 2022-11-14 15:08:03.666810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.2/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.3/MIT-LICENSE.txt
--rw-r--r--   0        0        0   284394 2022-11-14 15:08:03.671810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.3/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.819810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.0/LICENSE.txt
--rw-r--r--   0        0        0   294161 2022-11-14 15:08:03.688810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.0/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.819810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.1/LICENSE.txt
--rw-r--r--   0        0        0   294199 2022-11-14 15:08:03.693810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.1/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.2/LICENSE.txt
--rw-r--r--   0        0        0   293840 2022-11-14 15:08:03.700810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.2/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.3/LICENSE.txt
--rw-r--r--   0        0        0   293650 2022-11-14 15:08:03.702810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.3/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.4/LICENSE.txt
--rw-r--r--   0        0        0   293430 2022-11-14 15:08:03.705810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.4/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.0/MIT-LICENSE.txt
--rw-r--r--   0        0        0   258377 2022-11-14 15:08:03.706810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.1/MIT-LICENSE.txt
--rw-r--r--   0        0        0   259996 2022-11-14 15:08:03.707810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.1/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.2/MIT-LICENSE.txt
--rw-r--r--   0        0        0   265217 2022-11-14 15:08:03.707810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.2/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.3/MIT-LICENSE.txt
--rw-r--r--   0        0        0   418275 2022-11-14 15:08:03.709810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.3/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.0/MIT-LICENSE.txt
--rw-r--r--   0        0        0   267320 2022-11-14 15:08:03.710810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.1/MIT-LICENSE.txt
--rw-r--r--   0        0        0   268380 2022-11-14 15:08:03.711810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.1/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.0/MIT-LICENSE.txt
--rw-r--r--   0        0        0   240196 2022-11-14 15:08:03.711810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.1/MIT-LICENSE.txt
--rw-r--r--   0        0        0   242727 2022-11-14 15:08:03.712810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.1/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.2/MIT-LICENSE.txt
--rw-r--r--   0        0        0   242915 2022-11-14 15:08:03.713810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.2/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.3/MIT-LICENSE.txt
--rw-r--r--   0        0        0   242142 2022-11-14 15:08:03.714810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.3/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.0/MIT-LICENSE.txt
--rw-r--r--   0        0        0   244963 2022-11-14 15:08:03.715810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.1/MIT-LICENSE.txt
--rw-r--r--   0        0        0   247351 2022-11-14 15:08:03.715810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.1/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.2/MIT-LICENSE.txt
--rw-r--r--   0        0        0   247380 2022-11-14 15:08:03.716810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.2/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.3/MIT-LICENSE.txt
--rw-r--r--   0        0        0   247387 2022-11-14 15:08:03.717810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.3/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.4/MIT-LICENSE.txt
--rw-r--r--   0        0        0   247597 2022-11-14 15:08:03.718810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.4/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.0/LICENSE.txt
--rw-r--r--   0        0        0   258388 2022-11-14 15:08:03.719810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.0/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.1/LICENSE.txt
--rw-r--r--   0        0        0   258549 2022-11-14 15:08:03.720810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.1/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.2/LICENSE.txt
--rw-r--r--   0        0        0   258648 2022-11-14 15:08:03.721810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.2/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.3/LICENSE.txt
--rw-r--r--   0        0        0   258648 2022-11-14 15:08:03.722810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.3/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.4/LICENSE.txt
--rw-r--r--   0        0        0   257551 2022-11-14 15:08:03.723810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.4/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.0.0/LICENSE.txt
--rw-r--r--   0        0        0   263268 2022-11-14 15:08:03.723810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.0.0/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.0/LICENSE.txt
--rw-r--r--   0        0        0   263767 2022-11-14 15:08:03.724810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.0/jquery.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.1/LICENSE.txt
--rw-r--r--   0        0        0   267194 2022-11-14 15:08:03.725810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.1/jquery.js
--rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.821810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.0/LICENSE.txt
--rw-r--r--   0        0        0   267686 2022-11-14 15:08:03.726810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.0/jquery.js
--rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.821810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.1/LICENSE.txt
--rw-r--r--   0        0        0   268039 2022-11-14 15:08:03.727810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.1/jquery.js
--rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.822810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.0/LICENSE.txt
--rw-r--r--   0        0        0   271751 2022-11-14 15:08:03.728810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.0/jquery.js
--rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.822810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.1/LICENSE.txt
--rw-r--r--   0        0        0   271751 2022-11-14 15:08:03.728810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.1/jquery.js
--rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.822810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.0/LICENSE.txt
--rw-r--r--   0        0        0   279860 2022-11-14 15:08:03.729810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.0/jquery.js
--rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.822810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.1/LICENSE.txt
--rw-r--r--   0        0        0   280364 2022-11-14 15:08:03.730810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.1/jquery.js
--rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.822810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.0/LICENSE.txt
--rw-r--r--   0        0        0   287649 2022-11-14 15:08:03.734810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.0/jquery.js
--rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.822810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.1/LICENSE.txt
--rw-r--r--   0        0        0   287630 2022-11-14 15:08:03.735810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.1/jquery.js
--rw-r--r--   0        0        0     1097 2022-11-14 15:08:03.822810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.6.0/LICENSE.txt
--rw-r--r--   0        0        0   288580 2022-11-14 15:08:03.737810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.6.0/jquery.js
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-custom/MIT-LICENSE.txt
--rw-r--r--   0        0        0   283248 2022-11-14 15:08:03.739810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-custom/jquery.js
--rw-r--r--   0        0        0     1614 2022-11-14 15:08:03.822810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-1.4.1/LICENSE.txt
--rw-r--r--   0        0        0    23497 2022-11-14 15:08:03.634810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-1.4.1/jquery-migrate.js
--rw-r--r--   0        0        0     1615 2022-11-14 15:08:03.823810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-3.3.2/LICENSE.txt
--rw-r--r--   0        0        0    25300 2022-11-14 15:08:03.635810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-3.3.2/jquery-migrate.js
--rw-r--r--   0        0        0     1084 2022-11-14 15:08:03.823810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-mousewheel/LICENSE.txt
--rw-r--r--   0        0        0     8279 2022-11-14 15:08:03.741810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-mousewheel/jquery.mousewheel.js
--rw-r--r--   0        0        0     1615 2022-11-14 15:08:03.823810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-simulate/LICENSE.txt
--rw-r--r--   0        0        0     8710 2022-11-14 15:08:03.742810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-simulate/jquery.simulate.js
--rw-r--r--   0        0        0     1590 2022-11-14 15:08:03.824810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit/LICENSE.txt
--rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.828810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit/MIT-LICENSE.txt
--rw-r--r--   0        0        0     5146 2022-11-14 15:08:03.560809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit/qunit.css
--rw-r--r--   0        0        0   115758 2022-11-14 15:08:03.746810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit/qunit.js
--rw-r--r--   0        0        0     1085 2022-11-14 15:08:03.823810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-classes/LICENSE.txt
--rw-r--r--   0        0        0     5295 2022-11-14 15:08:03.744810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-classes/qunit-assert-classes.js
--rw-r--r--   0        0        0     1094 2022-11-14 15:08:03.828810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-close/MIT-LICENSE.txt
--rw-r--r--   0        0        0     4181 2022-11-14 15:08:03.745810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-close/qunit-assert-close.js
--rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.823810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit-composite/LICENSE.txt
--rw-r--r--   0        0        0      196 2022-11-14 15:08:03.559809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit-composite/qunit-composite.css
--rw-r--r--   0        0        0     4768 2022-11-14 15:08:03.745810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit-composite/qunit-composite.js
--rw-r--r--   0        0        0    83083 2022-11-14 15:08:03.746810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/requirejs/require.js
--rw-r--r--   0        0        0     1812 2022-11-14 15:08:03.751810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/package.json
--rw-r--r--   0        0        0      489 2022-11-14 15:08:03.414809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/accordion.css
--rw-r--r--   0        0        0      275 2022-11-14 15:08:03.415809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/all.css
--rw-r--r--   0        0        0      316 2022-11-14 15:08:03.415809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/autocomplete.css
--rw-r--r--   0        0        0      791 2022-11-14 15:08:03.417809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/base.css
--rw-r--r--   0        0        0     1497 2022-11-14 15:08:03.417809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/button.css
--rw-r--r--   0        0        0      789 2022-11-14 15:08:03.418809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/checkboxradio.css
--rw-r--r--   0        0        0     1526 2022-11-14 15:08:03.419809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/controlgroup.css
--rw-r--r--   0        0        0     1581 2022-11-14 15:08:03.419809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/core.css
--rw-r--r--   0        0        0     3788 2022-11-14 15:08:03.420809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/datepicker.css
--rw-r--r--   0        0        0     1753 2022-11-14 15:08:03.420809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/dialog.css
--rw-r--r--   0        0        0      253 2022-11-14 15:08:03.421809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/draggable.css
--rw-r--r--   0        0        0       86 2022-11-14 15:08:03.765810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-r--r--   0        0        0     3266 2022-11-14 15:08:03.792810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     3274 2022-11-14 15:08:03.795810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     3262 2022-11-14 15:08:03.797810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     3266 2022-11-14 15:08:03.797810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     3262 2022-11-14 15:08:03.806810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     3264 2022-11-14 15:08:03.819810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0     1124 2022-11-14 15:08:03.557809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/menu.css
--rw-r--r--   0        0        0     2952 2022-11-14 15:08:03.558809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/progressbar.css
--rw-r--r--   0        0        0     1198 2022-11-14 15:08:03.561809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/resizable.css
--rw-r--r--   0        0        0      337 2022-11-14 15:08:03.562809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/selectable.css
--rw-r--r--   0        0        0      916 2022-11-14 15:08:03.563809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/selectmenu.css
--rw-r--r--   0        0        0     1359 2022-11-14 15:08:03.563809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/slider.css
--rw-r--r--   0        0        0      251 2022-11-14 15:08:03.564809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/sortable.css
--rw-r--r--   0        0        0      964 2022-11-14 15:08:03.564809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/spinner.css
--rw-r--r--   0        0        0     1217 2022-11-14 15:08:03.565809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/tabs.css
--rw-r--r--   0        0        0    18128 2022-11-14 15:08:03.590809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/theme.css
--rw-r--r--   0        0        0      355 2022-11-14 15:08:03.591809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/tooltip.css
--rw-r--r--   0        0        0      361 2022-11-14 15:08:03.596809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/core.js
--rw-r--r--   0        0        0      934 2022-11-14 15:08:03.597809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/data.js
--rw-r--r--   0        0        0     1079 2022-11-14 15:08:03.623810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/disable-selection.js
--rw-r--r--   0        0        0    24612 2022-11-14 15:08:03.629810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effect.js
--rw-r--r--   0        0        0     1640 2022-11-14 15:08:03.624810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-blind.js
--rw-r--r--   0        0        0     2656 2022-11-14 15:08:03.624810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-bounce.js
--rw-r--r--   0        0        0     1573 2022-11-14 15:08:03.625810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-clip.js
--rw-r--r--   0        0        0     1591 2022-11-14 15:08:03.625810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-drop.js
--rw-r--r--   0        0        0     2920 2022-11-14 15:08:03.625810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-explode.js
--rw-r--r--   0        0        0      964 2022-11-14 15:08:03.625810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-fade.js
--rw-r--r--   0        0        0     2181 2022-11-14 15:08:03.625810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-fold.js
--rw-r--r--   0        0        0     1239 2022-11-14 15:08:03.626810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-highlight.js
--rw-r--r--   0        0        0      991 2022-11-14 15:08:03.626810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-puff.js
--rw-r--r--   0        0        0     1563 2022-11-14 15:08:03.626810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-pulsate.js
--rw-r--r--   0        0        0     1369 2022-11-14 15:08:03.626810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-scale.js
--rw-r--r--   0        0        0     1880 2022-11-14 15:08:03.628810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-shake.js
--rw-r--r--   0        0        0     5414 2022-11-14 15:08:03.628810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-size.js
--rw-r--r--   0        0        0     1963 2022-11-14 15:08:03.628810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-slide.js
--rw-r--r--   0        0        0      884 2022-11-14 15:08:03.628810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-transfer.js
--rw-r--r--   0        0        0     2295 2022-11-14 15:08:03.629810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/focusable.js
--rw-r--r--   0        0        0     1827 2022-11-14 15:08:03.629810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/form-reset-mixin.js
--rw-r--r--   0        0        0      581 2022-11-14 15:08:03.629810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/form.js
--rw-r--r--   0        0        0     1207 2022-11-14 15:08:03.597809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-af.js
--rw-r--r--   0        0        0     1532 2022-11-14 15:08:03.597809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ar-DZ.js
--rw-r--r--   0        0        0     1499 2022-11-14 15:08:03.598810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ar.js
--rw-r--r--   0        0        0     1241 2022-11-14 15:08:03.598810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-az.js
--rw-r--r--   0        0        0     1467 2022-11-14 15:08:03.598810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-be.js
--rw-r--r--   0        0        0     1444 2022-11-14 15:08:03.599810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-bg.js
--rw-r--r--   0        0        0     1183 2022-11-14 15:08:03.599810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-bs.js
--rw-r--r--   0        0        0     1207 2022-11-14 15:08:03.599810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ca.js
--rw-r--r--   0        0        0     1232 2022-11-14 15:08:03.599810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-cs.js
--rw-r--r--   0        0        0     1248 2022-11-14 15:08:03.599810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-cy-GB.js
--rw-r--r--   0        0        0     1212 2022-11-14 15:08:03.600809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-da.js
--rw-r--r--   0        0        0     1227 2022-11-14 15:08:03.600809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-de-AT.js
--rw-r--r--   0        0        0     1202 2022-11-14 15:08:03.600809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-de.js
--rw-r--r--   0        0        0     1521 2022-11-14 15:08:03.600809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-el.js
--rw-r--r--   0        0        0     1226 2022-11-14 15:08:03.600809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-AU.js
--rw-r--r--   0        0        0     1203 2022-11-14 15:08:03.601810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-GB.js
--rw-r--r--   0        0        0     1228 2022-11-14 15:08:03.601810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-NZ.js
--rw-r--r--   0        0        0     1214 2022-11-14 15:08:03.601810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-eo.js
--rw-r--r--   0        0        0     1209 2022-11-14 15:08:03.601810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-es.js
--rw-r--r--   0        0        0     1277 2022-11-14 15:08:03.601810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-et.js
--rw-r--r--   0        0        0     1164 2022-11-14 15:08:03.601810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-eu.js
--rw-r--r--   0        0        0     1420 2022-11-14 15:08:03.602810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fa.js
--rw-r--r--   0        0        0     1266 2022-11-14 15:08:03.602810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fi.js
--rw-r--r--   0        0        0     1254 2022-11-14 15:08:03.602810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fo.js
--rw-r--r--   0        0        0     1221 2022-11-14 15:08:03.602810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr-CA.js
--rw-r--r--   0        0        0     1258 2022-11-14 15:08:03.603809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr-CH.js
--rw-r--r--   0        0        0     1341 2022-11-14 15:08:03.604810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr.js
--rw-r--r--   0        0        0     1211 2022-11-14 15:08:03.604810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-gl.js
--rw-r--r--   0        0        0     1325 2022-11-14 15:08:03.604810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-he.js
--rw-r--r--   0        0        0     1618 2022-11-14 15:08:03.604810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hi.js
--rw-r--r--   0        0        0     1208 2022-11-14 15:08:03.604810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hr.js
--rw-r--r--   0        0        0     1187 2022-11-14 15:08:03.605810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hu.js
--rw-r--r--   0        0        0     1495 2022-11-14 15:08:03.605810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hy.js
--rw-r--r--   0        0        0     1266 2022-11-14 15:08:03.605810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-id.js
--rw-r--r--   0        0        0     1281 2022-11-14 15:08:03.605810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-is.js
--rw-r--r--   0        0        0     1257 2022-11-14 15:08:03.605810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-it-CH.js
--rw-r--r--   0        0        0     1233 2022-11-14 15:08:03.606809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-it.js
--rw-r--r--   0        0        0     1223 2022-11-14 15:08:03.606809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ja.js
--rw-r--r--   0        0        0     1761 2022-11-14 15:08:03.606809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ka.js
--rw-r--r--   0        0        0     1438 2022-11-14 15:08:03.606809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-kk.js
--rw-r--r--   0        0        0     1645 2022-11-14 15:08:03.608810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-km.js
--rw-r--r--   0        0        0     1264 2022-11-14 15:08:03.609809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ko.js
--rw-r--r--   0        0        0     1416 2022-11-14 15:08:03.609809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ky.js
--rw-r--r--   0        0        0     1260 2022-11-14 15:08:03.609809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lb.js
--rw-r--r--   0        0        0     1297 2022-11-14 15:08:03.609809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lt.js
--rw-r--r--   0        0        0     1290 2022-11-14 15:08:03.610809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lv.js
--rw-r--r--   0        0        0     1408 2022-11-14 15:08:03.610809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-mk.js
--rw-r--r--   0        0        0     1747 2022-11-14 15:08:03.610809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ml.js
--rw-r--r--   0        0        0     1212 2022-11-14 15:08:03.611810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ms.js
--rw-r--r--   0        0        0     1244 2022-11-14 15:08:03.612810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nb.js
--rw-r--r--   0        0        0     1238 2022-11-14 15:08:03.612810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nl-BE.js
--rw-r--r--   0        0        0     1230 2022-11-14 15:08:03.612810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nl.js
--rw-r--r--   0        0        0     1241 2022-11-14 15:08:03.613809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nn.js
--rw-r--r--   0        0        0     1236 2022-11-14 15:08:03.613809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-no.js
--rw-r--r--   0        0        0     1238 2022-11-14 15:08:03.614810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pl.js
--rw-r--r--   0        0        0     1299 2022-11-14 15:08:03.614810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pt-BR.js
--rw-r--r--   0        0        0     1216 2022-11-14 15:08:03.615810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pt.js
--rw-r--r--   0        0        0     1278 2022-11-14 15:08:03.615810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-rm.js
--rw-r--r--   0        0        0     1287 2022-11-14 15:08:03.615810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ro.js
--rw-r--r--   0        0        0     1438 2022-11-14 15:08:03.615810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ru.js
--rw-r--r--   0        0        0     1226 2022-11-14 15:08:03.616809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sk.js
--rw-r--r--   0        0        0     1264 2022-11-14 15:08:03.617810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sl.js
--rw-r--r--   0        0        0     1208 2022-11-14 15:08:03.617810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sq.js
--rw-r--r--   0        0        0     1205 2022-11-14 15:08:03.617810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sr-SR.js
--rw-r--r--   0        0        0     1390 2022-11-14 15:08:03.618810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sr.js
--rw-r--r--   0        0        0     1222 2022-11-14 15:08:03.618810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sv.js
--rw-r--r--   0        0        0     1859 2022-11-14 15:08:03.618810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ta.js
--rw-r--r--   0        0        0     1583 2022-11-14 15:08:03.619809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-th.js
--rw-r--r--   0        0        0     1395 2022-11-14 15:08:03.619809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-tj.js
--rw-r--r--   0        0        0     1205 2022-11-14 15:08:03.619809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-tr.js
--rw-r--r--   0        0        0     1544 2022-11-14 15:08:03.620810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-uk.js
--rw-r--r--   0        0        0     1377 2022-11-14 15:08:03.620810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-vi.js
--rw-r--r--   0        0        0     1322 2022-11-14 15:08:03.621810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-CN.js
--rw-r--r--   0        0        0     1320 2022-11-14 15:08:03.621810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-HK.js
--rw-r--r--   0        0        0     1322 2022-11-14 15:08:03.621810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-TW.js
--rw-r--r--   0        0        0      385 2022-11-14 15:08:03.633810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/ie.js
--rw-r--r--   0        0        0     2168 2022-11-14 15:08:03.635810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/jquery-patch.js
--rw-r--r--   0        0        0      530 2022-11-14 15:08:03.640810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/jquery-var-for-color.js
--rw-r--r--   0        0        0      820 2022-11-14 15:08:03.742810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/keycode.js
--rw-r--r--   0        0        0     1775 2022-11-14 15:08:03.742810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/labels.js
--rw-r--r--   0        0        0     1020 2022-11-14 15:08:03.743810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/plugin.js
--rw-r--r--   0        0        0    15125 2022-11-14 15:08:03.743810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/position.js
--rw-r--r--   0        0        0     1014 2022-11-14 15:08:03.747810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/safe-active-element.js
--rw-r--r--   0        0        0      523 2022-11-14 15:08:03.747810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/safe-blur.js
--rw-r--r--   0        0        0     1280 2022-11-14 15:08:03.747810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/scroll-parent.js
--rw-r--r--   0        0        0      883 2022-11-14 15:08:03.749810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/tabbable.js
--rw-r--r--   0        0        0      976 2022-11-14 15:08:03.750810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/unique-id.js
--rw-r--r--   0        0        0     1811 2022-11-14 15:08:03.824810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/vendor/jquery-color/LICENSE.txt
--rw-r--r--   0        0        0    17418 2022-11-14 15:08:03.641810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/vendor/jquery-color/jquery.color.js
--rw-r--r--   0        0        0      322 2022-11-14 15:08:03.750810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/version.js
--rw-r--r--   0        0        0    20283 2022-11-14 15:08:03.751810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widget.js
--rw-r--r--   0        0        0    16134 2022-11-14 15:08:03.592810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/accordion.js
--rw-r--r--   0        0        0    17526 2022-11-14 15:08:03.593809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/autocomplete.js
--rw-r--r--   0        0        0    11702 2022-11-14 15:08:03.594809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/button.js
--rw-r--r--   0        0        0     7585 2022-11-14 15:08:03.594809 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/checkboxradio.js
--rw-r--r--   0        0        0     8622 2022-11-14 15:08:03.595810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/controlgroup.js
--rw-r--r--   0        0        0    82518 2022-11-14 15:08:03.622810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/datepicker.js
--rw-r--r--   0        0        0    23738 2022-11-14 15:08:03.622810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/dialog.js
--rw-r--r--   0        0        0    35541 2022-11-14 15:08:03.623810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/draggable.js
--rw-r--r--   0        0        0    12895 2022-11-14 15:08:03.624810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/droppable.js
--rw-r--r--   0        0        0    18956 2022-11-14 15:08:03.743810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/menu.js
--rw-r--r--   0        0        0     6224 2022-11-14 15:08:03.743810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/mouse.js
--rw-r--r--   0        0        0     4235 2022-11-14 15:08:03.744810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/progressbar.js
--rw-r--r--   0        0        0    30395 2022-11-14 15:08:03.747810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/resizable.js
--rw-r--r--   0        0        0     8125 2022-11-14 15:08:03.748810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/selectable.js
--rw-r--r--   0        0        0    16249 2022-11-14 15:08:03.748810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/selectmenu.js
--rw-r--r--   0        0        0    19595 2022-11-14 15:08:03.748810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/slider.js
--rw-r--r--   0        0        0    47637 2022-11-14 15:08:03.749810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/sortable.js
--rw-r--r--   0        0        0    14430 2022-11-14 15:08:03.749810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/spinner.js
--rw-r--r--   0        0        0    23658 2022-11-14 15:08:03.750810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/tabs.js
--rw-r--r--   0        0        0    14472 2022-11-14 15:08:03.750810 anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/tooltip.js
--rw-r--r--   0        0        0    45726 2022-11-14 15:08:03.705810 anitya-1.7.0/anitya/static/node_modules/moment/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2022-11-14 15:08:03.408809 anitya-1.7.0/anitya/static/node_modules/moment/LICENSE
--rw-r--r--   0        0        0     2468 2022-11-14 15:08:03.705810 anitya-1.7.0/anitya/static/node_modules/moment/README.md
--rw-r--r--   0        0        0     2149 2022-11-14 15:08:03.420809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/af.js
--rw-r--r--   0        0        0     4449 2022-11-14 15:08:03.427809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar-dz.js
--rw-r--r--   0        0        0     1934 2022-11-14 15:08:03.428809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar-kw.js
--rw-r--r--   0        0        0     4648 2022-11-14 15:08:03.429809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar-ly.js
--rw-r--r--   0        0        0     1989 2022-11-14 15:08:03.433809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar-ma.js
--rw-r--r--   0        0        0     3042 2022-11-14 15:08:03.436809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar-sa.js
--rw-r--r--   0        0        0     1936 2022-11-14 15:08:03.439809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar-tn.js
--rw-r--r--   0        0        0     5072 2022-11-14 15:08:03.440809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar.js
--rw-r--r--   0        0        0     2846 2022-11-14 15:08:03.448809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/az.js
--rw-r--r--   0        0        0     5154 2022-11-14 15:08:03.452809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/be.js
--rw-r--r--   0        0        0     2955 2022-11-14 15:08:03.455809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/bg.js
--rw-r--r--   0        0        0     1784 2022-11-14 15:08:03.457809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/bm.js
--rw-r--r--   0        0        0     4349 2022-11-14 15:08:03.459809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/bn-bd.js
--rw-r--r--   0        0        0     3898 2022-11-14 15:08:03.461809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/bn.js
--rw-r--r--   0        0        0     4399 2022-11-14 15:08:03.462809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/bo.js
--rw-r--r--   0        0        0     4544 2022-11-14 15:08:03.464809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/br.js
--rw-r--r--   0        0        0     4475 2022-11-14 15:08:03.466809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/bs.js
--rw-r--r--   0        0        0     3031 2022-11-14 15:08:03.466809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ca.js
--rw-r--r--   0        0        0     6718 2022-11-14 15:08:03.475809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/cs.js
--rw-r--r--   0        0        0     2341 2022-11-14 15:08:03.476809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/cv.js
--rw-r--r--   0        0        0     2834 2022-11-14 15:08:03.477809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/cy.js
--rw-r--r--   0        0        0     1629 2022-11-14 15:08:03.478809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/da.js
--rw-r--r--   0        0        0     2635 2022-11-14 15:08:03.480809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/de-at.js
--rw-r--r--   0        0        0     2563 2022-11-14 15:08:03.482809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/de-ch.js
--rw-r--r--   0        0        0     2562 2022-11-14 15:08:03.484809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/de.js
--rw-r--r--   0        0        0     2464 2022-11-14 15:08:03.487809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/dv.js
--rw-r--r--   0        0        0     3877 2022-11-14 15:08:03.488809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/el.js
--rw-r--r--   0        0        0     2029 2022-11-14 15:08:03.490809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-au.js
--rw-r--r--   0        0        0     1878 2022-11-14 15:08:03.491809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-ca.js
--rw-r--r--   0        0        0     2035 2022-11-14 15:08:03.493809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-gb.js
--rw-r--r--   0        0        0     2033 2022-11-14 15:08:03.496809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-ie.js
--rw-r--r--   0        0        0     1871 2022-11-14 15:08:03.498809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-il.js
--rw-r--r--   0        0        0     2029 2022-11-14 15:08:03.500809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-in.js
--rw-r--r--   0        0        0     2038 2022-11-14 15:08:03.502809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-nz.js
--rw-r--r--   0        0        0     2047 2022-11-14 15:08:03.505809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-sg.js
--rw-r--r--   0        0        0     2338 2022-11-14 15:08:03.512809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/eo.js
--rw-r--r--   0        0        0     3441 2022-11-14 15:08:03.515809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/es-do.js
--rw-r--r--   0        0        0     3510 2022-11-14 15:08:03.517809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/es-mx.js
--rw-r--r--   0        0        0     3538 2022-11-14 15:08:03.519809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/es-us.js
--rw-r--r--   0        0        0     3498 2022-11-14 15:08:03.521809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/es.js
--rw-r--r--   0        0        0     2631 2022-11-14 15:08:03.523809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/et.js
--rw-r--r--   0        0        0     1964 2022-11-14 15:08:03.525809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/eu.js
--rw-r--r--   0        0        0     3230 2022-11-14 15:08:03.526809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fa.js
--rw-r--r--   0        0        0     3632 2022-11-14 15:08:03.528809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fi.js
--rw-r--r--   0        0        0     1776 2022-11-14 15:08:03.530809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fil.js
--rw-r--r--   0        0        0     1772 2022-11-14 15:08:03.531809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fo.js
--rw-r--r--   0        0        0     2104 2022-11-14 15:08:03.540809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fr-ca.js
--rw-r--r--   0        0        0     2263 2022-11-14 15:08:03.542809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fr-ch.js
--rw-r--r--   0        0        0     3471 2022-11-14 15:08:03.543809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fr.js
--rw-r--r--   0        0        0     2275 2022-11-14 15:08:03.548809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fy.js
--rw-r--r--   0        0        0     2360 2022-11-14 15:08:03.549809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ga.js
--rw-r--r--   0        0        0     2380 2022-11-14 15:08:03.551809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/gd.js
--rw-r--r--   0        0        0     2347 2022-11-14 15:08:03.552809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/gl.js
--rw-r--r--   0        0        0     5506 2022-11-14 15:08:03.555809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/gom-deva.js
--rw-r--r--   0        0        0     4130 2022-11-14 15:08:03.557809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/gom-latn.js
--rw-r--r--   0        0        0     4132 2022-11-14 15:08:03.559809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/gu.js
--rw-r--r--   0        0        0     3211 2022-11-14 15:08:03.560809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/he.js
--rw-r--r--   0        0        0     6421 2022-11-14 15:08:03.562809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/hi.js
--rw-r--r--   0        0        0     4718 2022-11-14 15:08:03.564809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/hr.js
--rw-r--r--   0        0        0     3815 2022-11-14 15:08:03.566809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/hu.js
--rw-r--r--   0        0        0     3236 2022-11-14 15:08:03.568809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/hy-am.js
--rw-r--r--   0        0        0     2375 2022-11-14 15:08:03.571809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/id.js
--rw-r--r--   0        0        0     4458 2022-11-14 15:08:03.577809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/is.js
--rw-r--r--   0        0        0     1941 2022-11-14 15:08:03.578809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/it-ch.js
--rw-r--r--   0        0        0     3251 2022-11-14 15:08:03.579810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/it.js
--rw-r--r--   0        0        0     3955 2022-11-14 15:08:03.580809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ja.js
--rw-r--r--   0        0        0     2384 2022-11-14 15:08:03.582810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/jv.js
--rw-r--r--   0        0        0     3504 2022-11-14 15:08:03.583809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ka.js
--rw-r--r--   0        0        0     2495 2022-11-14 15:08:03.584809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/kk.js
--rw-r--r--   0        0        0     3362 2022-11-14 15:08:03.586809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/km.js
--rw-r--r--   0        0        0     4252 2022-11-14 15:08:03.587809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/kn.js
--rw-r--r--   0        0        0     2223 2022-11-14 15:08:03.589810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ko.js
--rw-r--r--   0        0        0     3330 2022-11-14 15:08:03.590809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ku.js
--rw-r--r--   0        0        0     2521 2022-11-14 15:08:03.591809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ky.js
--rw-r--r--   0        0        0     4269 2022-11-14 15:08:03.593809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/lb.js
--rw-r--r--   0        0        0     2585 2022-11-14 15:08:03.595810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/lo.js
--rw-r--r--   0        0        0     4005 2022-11-14 15:08:03.610809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/lt.js
--rw-r--r--   0        0        0     3449 2022-11-14 15:08:03.612810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/lv.js
--rw-r--r--   0        0        0     3661 2022-11-14 15:08:03.613809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/me.js
--rw-r--r--   0        0        0     2023 2022-11-14 15:08:03.615810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/mi.js
--rw-r--r--   0        0        0     3021 2022-11-14 15:08:03.617810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/mk.js
--rw-r--r--   0        0        0     3287 2022-11-14 15:08:03.619809 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ml.js
--rw-r--r--   0        0        0     3414 2022-11-14 15:08:03.620810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/mn.js
--rw-r--r--   0        0        0     6574 2022-11-14 15:08:03.637810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/mr.js
--rw-r--r--   0        0        0     2330 2022-11-14 15:08:03.637810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ms-my.js
--rw-r--r--   0        0        0     2277 2022-11-14 15:08:03.638810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ms.js
--rw-r--r--   0        0        0     1684 2022-11-14 15:08:03.639810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/mt.js
--rw-r--r--   0        0        0     3094 2022-11-14 15:08:03.639810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/my.js
--rw-r--r--   0        0        0     1899 2022-11-14 15:08:03.640810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/nb.js
--rw-r--r--   0        0        0     4031 2022-11-14 15:08:03.640810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ne.js
--rw-r--r--   0        0        0     3169 2022-11-14 15:08:03.641810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/nl-be.js
--rw-r--r--   0        0        0     3202 2022-11-14 15:08:03.642810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/nl.js
--rw-r--r--   0        0        0     1828 2022-11-14 15:08:03.642810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/nn.js
--rw-r--r--   0        0        0     2472 2022-11-14 15:08:03.643810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/oc-lnc.js
--rw-r--r--   0        0        0     4198 2022-11-14 15:08:03.644810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/pa-in.js
--rw-r--r--   0        0        0     4166 2022-11-14 15:08:03.647810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/pl.js
--rw-r--r--   0        0        0     1854 2022-11-14 15:08:03.649810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/pt-br.js
--rw-r--r--   0        0        0     1968 2022-11-14 15:08:03.650810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/pt.js
--rw-r--r--   0        0        0     2319 2022-11-14 15:08:03.652810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ro.js
--rw-r--r--   0        0        0     8418 2022-11-14 15:08:03.654810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ru.js
--rw-r--r--   0        0        0     2153 2022-11-14 15:08:03.655810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sd.js
--rw-r--r--   0        0        0     1849 2022-11-14 15:08:03.655810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/se.js
--rw-r--r--   0        0        0     2681 2022-11-14 15:08:03.656810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/si.js
--rw-r--r--   0        0        0     5173 2022-11-14 15:08:03.657810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sk.js
--rw-r--r--   0        0        0     6115 2022-11-14 15:08:03.657810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sl.js
--rw-r--r--   0        0        0     1987 2022-11-14 15:08:03.658810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sq.js
--rw-r--r--   0        0        0     4762 2022-11-14 15:08:03.659810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sr-cyrl.js
--rw-r--r--   0        0        0     4209 2022-11-14 15:08:03.659810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sr.js
--rw-r--r--   0        0        0     2572 2022-11-14 15:08:03.660810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ss.js
--rw-r--r--   0        0        0     2066 2022-11-14 15:08:03.662810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sv.js
--rw-r--r--   0        0        0     1651 2022-11-14 15:08:03.663810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sw.js
--rw-r--r--   0        0        0     4800 2022-11-14 15:08:03.663810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ta.js
--rw-r--r--   0        0        0     3392 2022-11-14 15:08:03.664810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/te.js
--rw-r--r--   0        0        0     2155 2022-11-14 15:08:03.665810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tet.js
--rw-r--r--   0        0        0     3604 2022-11-14 15:08:03.666810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tg.js
--rw-r--r--   0        0        0     2736 2022-11-14 15:08:03.667810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/th.js
--rw-r--r--   0        0        0     2488 2022-11-14 15:08:03.668810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tk.js
--rw-r--r--   0        0        0     1735 2022-11-14 15:08:03.669810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tl-ph.js
--rw-r--r--   0        0        0     3755 2022-11-14 15:08:03.670810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tlh.js
--rw-r--r--   0        0        0     2927 2022-11-14 15:08:03.672810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tr.js
--rw-r--r--   0        0        0     3109 2022-11-14 15:08:03.674810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tzl.js
--rw-r--r--   0        0        0     1691 2022-11-14 15:08:03.674810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tzm-latn.js
--rw-r--r--   0        0        0     2322 2022-11-14 15:08:03.675810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tzm.js
--rw-r--r--   0        0        0     3880 2022-11-14 15:08:03.687810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ug-cn.js
--rw-r--r--   0        0        0     5955 2022-11-14 15:08:03.688810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/uk.js
--rw-r--r--   0        0        0     2200 2022-11-14 15:08:03.689810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ur.js
--rw-r--r--   0        0        0     1639 2022-11-14 15:08:03.691810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/uz-latn.js
--rw-r--r--   0        0        0     1885 2022-11-14 15:08:03.692810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/uz.js
--rw-r--r--   0        0        0     2430 2022-11-14 15:08:03.693810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/vi.js
--rw-r--r--   0        0        0     2348 2022-11-14 15:08:03.695810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/x-pseudo.js
--rw-r--r--   0        0        0     1887 2022-11-14 15:08:03.696810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/yo.js
--rw-r--r--   0        0        0     3711 2022-11-14 15:08:03.698810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/zh-cn.js
--rw-r--r--   0        0        0     3116 2022-11-14 15:08:03.700810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/zh-hk.js
--rw-r--r--   0        0        0     3066 2022-11-14 15:08:03.701810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/zh-mo.js
--rw-r--r--   0        0        0     3013 2022-11-14 15:08:03.701810 anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/zh-tw.js
--rw-r--r--   0        0        0   154671 2022-11-14 15:08:03.635810 anitya-1.7.0/anitya/static/node_modules/moment/dist/moment.js
--rw-r--r--   0        0        0       39 2022-11-14 15:08:03.512809 anitya-1.7.0/anitya/static/node_modules/moment/ender.js
--rw-r--r--   0        0        0     2753 2022-11-14 15:08:03.421809 anitya-1.7.0/anitya/static/node_modules/moment/locale/af.js
--rw-r--r--   0        0        0     5377 2022-11-14 15:08:03.427809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ar-dz.js
--rw-r--r--   0        0        0     2478 2022-11-14 15:08:03.428809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ar-kw.js
--rw-r--r--   0        0        0     5652 2022-11-14 15:08:03.430809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ar-ly.js
--rw-r--r--   0        0        0     2533 2022-11-14 15:08:03.435809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ar-ma.js
--rw-r--r--   0        0        0     3782 2022-11-14 15:08:03.437809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ar-sa.js
--rw-r--r--   0        0        0     2480 2022-11-14 15:08:03.439809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ar-tn.js
--rw-r--r--   0        0        0     6136 2022-11-14 15:08:03.440809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ar.js
--rw-r--r--   0        0        0     3570 2022-11-14 15:08:03.449809 anitya-1.7.0/anitya/static/node_modules/moment/locale/az.js
--rw-r--r--   0        0        0     6030 2022-11-14 15:08:03.454809 anitya-1.7.0/anitya/static/node_modules/moment/locale/be.js
--rw-r--r--   0        0        0     3623 2022-11-14 15:08:03.456809 anitya-1.7.0/anitya/static/node_modules/moment/locale/bg.js
--rw-r--r--   0        0        0     2233 2022-11-14 15:08:03.457809 anitya-1.7.0/anitya/static/node_modules/moment/locale/bm.js
--rw-r--r--   0        0        0     5177 2022-11-14 15:08:03.460809 anitya-1.7.0/anitya/static/node_modules/moment/locale/bn-bd.js
--rw-r--r--   0        0        0     4690 2022-11-14 15:08:03.461809 anitya-1.7.0/anitya/static/node_modules/moment/locale/bn.js
--rw-r--r--   0        0        0     5211 2022-11-14 15:08:03.463809 anitya-1.7.0/anitya/static/node_modules/moment/locale/bo.js
--rw-r--r--   0        0        0     5520 2022-11-14 15:08:03.465809 anitya-1.7.0/anitya/static/node_modules/moment/locale/br.js
--rw-r--r--   0        0        0     5387 2022-11-14 15:08:03.466809 anitya-1.7.0/anitya/static/node_modules/moment/locale/bs.js
--rw-r--r--   0        0        0     3751 2022-11-14 15:08:03.467809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ca.js
--rw-r--r--   0        0        0     7750 2022-11-14 15:08:03.475809 anitya-1.7.0/anitya/static/node_modules/moment/locale/cs.js
--rw-r--r--   0        0        0     2913 2022-11-14 15:08:03.476809 anitya-1.7.0/anitya/static/node_modules/moment/locale/cv.js
--rw-r--r--   0        0        0     3542 2022-11-14 15:08:03.477809 anitya-1.7.0/anitya/static/node_modules/moment/locale/cy.js
--rw-r--r--   0        0        0     2161 2022-11-14 15:08:03.478809 anitya-1.7.0/anitya/static/node_modules/moment/locale/da.js
--rw-r--r--   0        0        0     3259 2022-11-14 15:08:03.481809 anitya-1.7.0/anitya/static/node_modules/moment/locale/de-at.js
--rw-r--r--   0        0        0     3094 2022-11-14 15:08:03.482809 anitya-1.7.0/anitya/static/node_modules/moment/locale/de-ch.js
--rw-r--r--   0        0        0     3182 2022-11-14 15:08:03.485809 anitya-1.7.0/anitya/static/node_modules/moment/locale/de.js
--rw-r--r--   0        0        0     3140 2022-11-14 15:08:03.487809 anitya-1.7.0/anitya/static/node_modules/moment/locale/dv.js
--rw-r--r--   0        0        0     4617 2022-11-14 15:08:03.489809 anitya-1.7.0/anitya/static/node_modules/moment/locale/el.js
--rw-r--r--   0        0        0     2625 2022-11-14 15:08:03.490809 anitya-1.7.0/anitya/static/node_modules/moment/locale/en-au.js
--rw-r--r--   0        0        0     2458 2022-11-14 15:08:03.492809 anitya-1.7.0/anitya/static/node_modules/moment/locale/en-ca.js
--rw-r--r--   0        0        0     2631 2022-11-14 15:08:03.494809 anitya-1.7.0/anitya/static/node_modules/moment/locale/en-gb.js
--rw-r--r--   0        0        0     2629 2022-11-14 15:08:03.496809 anitya-1.7.0/anitya/static/node_modules/moment/locale/en-ie.js
--rw-r--r--   0        0        0     2451 2022-11-14 15:08:03.499809 anitya-1.7.0/anitya/static/node_modules/moment/locale/en-il.js
--rw-r--r--   0        0        0     2625 2022-11-14 15:08:03.501809 anitya-1.7.0/anitya/static/node_modules/moment/locale/en-in.js
--rw-r--r--   0        0        0     2634 2022-11-14 15:08:03.503809 anitya-1.7.0/anitya/static/node_modules/moment/locale/en-nz.js
--rw-r--r--   0        0        0     2643 2022-11-14 15:08:03.509809 anitya-1.7.0/anitya/static/node_modules/moment/locale/en-sg.js
--rw-r--r--   0        0        0     2918 2022-11-14 15:08:03.513809 anitya-1.7.0/anitya/static/node_modules/moment/locale/eo.js
--rw-r--r--   0        0        0     4197 2022-11-14 15:08:03.516809 anitya-1.7.0/anitya/static/node_modules/moment/locale/es-do.js
--rw-r--r--   0        0        0     4270 2022-11-14 15:08:03.518809 anitya-1.7.0/anitya/static/node_modules/moment/locale/es-mx.js
--rw-r--r--   0        0        0     4294 2022-11-14 15:08:03.520809 anitya-1.7.0/anitya/static/node_modules/moment/locale/es-us.js
--rw-r--r--   0        0        0     4254 2022-11-14 15:08:03.522809 anitya-1.7.0/anitya/static/node_modules/moment/locale/es.js
--rw-r--r--   0        0        0     3255 2022-11-14 15:08:03.524809 anitya-1.7.0/anitya/static/node_modules/moment/locale/et.js
--rw-r--r--   0        0        0     2544 2022-11-14 15:08:03.525809 anitya-1.7.0/anitya/static/node_modules/moment/locale/eu.js
--rw-r--r--   0        0        0     3998 2022-11-14 15:08:03.527809 anitya-1.7.0/anitya/static/node_modules/moment/locale/fa.js
--rw-r--r--   0        0        0     4444 2022-11-14 15:08:03.529809 anitya-1.7.0/anitya/static/node_modules/moment/locale/fi.js
--rw-r--r--   0        0        0     2326 2022-11-14 15:08:03.530809 anitya-1.7.0/anitya/static/node_modules/moment/locale/fil.js
--rw-r--r--   0        0        0     2316 2022-11-14 15:08:03.534809 anitya-1.7.0/anitya/static/node_modules/moment/locale/fo.js
--rw-r--r--   0        0        0     2704 2022-11-14 15:08:03.541809 anitya-1.7.0/anitya/static/node_modules/moment/locale/fr-ca.js
--rw-r--r--   0        0        0     2879 2022-11-14 15:08:03.542809 anitya-1.7.0/anitya/static/node_modules/moment/locale/fr-ch.js
--rw-r--r--   0        0        0     4211 2022-11-14 15:08:03.544809 anitya-1.7.0/anitya/static/node_modules/moment/locale/fr.js
--rw-r--r--   0        0        0     2891 2022-11-14 15:08:03.549809 anitya-1.7.0/anitya/static/node_modules/moment/locale/fy.js
--rw-r--r--   0        0        0     3056 2022-11-14 15:08:03.550809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ga.js
--rw-r--r--   0        0        0     3076 2022-11-14 15:08:03.551809 anitya-1.7.0/anitya/static/node_modules/moment/locale/gd.js
--rw-r--r--   0        0        0     2967 2022-11-14 15:08:03.552809 anitya-1.7.0/anitya/static/node_modules/moment/locale/gl.js
--rw-r--r--   0        0        0     6336 2022-11-14 15:08:03.556809 anitya-1.7.0/anitya/static/node_modules/moment/locale/gom-deva.js
--rw-r--r--   0        0        0     4952 2022-11-14 15:08:03.558809 anitya-1.7.0/anitya/static/node_modules/moment/locale/gom-latn.js
--rw-r--r--   0        0        0     4936 2022-11-14 15:08:03.559809 anitya-1.7.0/anitya/static/node_modules/moment/locale/gu.js
--rw-r--r--   0        0        0     3899 2022-11-14 15:08:03.560809 anitya-1.7.0/anitya/static/node_modules/moment/locale/he.js
--rw-r--r--   0        0        0     7385 2022-11-14 15:08:03.562809 anitya-1.7.0/anitya/static/node_modules/moment/locale/hi.js
--rw-r--r--   0        0        0     5658 2022-11-14 15:08:03.565809 anitya-1.7.0/anitya/static/node_modules/moment/locale/hr.js
--rw-r--r--   0        0        0     4599 2022-11-14 15:08:03.566809 anitya-1.7.0/anitya/static/node_modules/moment/locale/hu.js
--rw-r--r--   0        0        0     3936 2022-11-14 15:08:03.569809 anitya-1.7.0/anitya/static/node_modules/moment/locale/hy-am.js
--rw-r--r--   0        0        0     2995 2022-11-14 15:08:03.571809 anitya-1.7.0/anitya/static/node_modules/moment/locale/id.js
--rw-r--r--   0        0        0     5334 2022-11-14 15:08:03.577809 anitya-1.7.0/anitya/static/node_modules/moment/locale/is.js
--rw-r--r--   0        0        0     2521 2022-11-14 15:08:03.578809 anitya-1.7.0/anitya/static/node_modules/moment/locale/it-ch.js
--rw-r--r--   0        0        0     3987 2022-11-14 15:08:03.579810 anitya-1.7.0/anitya/static/node_modules/moment/locale/it.js
--rw-r--r--   0        0        0     4867 2022-11-14 15:08:03.581809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ja.js
--rw-r--r--   0        0        0     3004 2022-11-14 15:08:03.582810 anitya-1.7.0/anitya/static/node_modules/moment/locale/jv.js
--rw-r--r--   0        0        0     4192 2022-11-14 15:08:03.583809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ka.js
--rw-r--r--   0        0        0     3139 2022-11-14 15:08:03.585809 anitya-1.7.0/anitya/static/node_modules/moment/locale/kk.js
--rw-r--r--   0        0        0     4090 2022-11-14 15:08:03.586809 anitya-1.7.0/anitya/static/node_modules/moment/locale/km.js
--rw-r--r--   0        0        0     5064 2022-11-14 15:08:03.588809 anitya-1.7.0/anitya/static/node_modules/moment/locale/kn.js
--rw-r--r--   0        0        0     2839 2022-11-14 15:08:03.589810 anitya-1.7.0/anitya/static/node_modules/moment/locale/ko.js
--rw-r--r--   0        0        0     4118 2022-11-14 15:08:03.590809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ku.js
--rw-r--r--   0        0        0     3173 2022-11-14 15:08:03.591809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ky.js
--rw-r--r--   0        0        0     5129 2022-11-14 15:08:03.593809 anitya-1.7.0/anitya/static/node_modules/moment/locale/lb.js
--rw-r--r--   0        0        0     3169 2022-11-14 15:08:03.595810 anitya-1.7.0/anitya/static/node_modules/moment/locale/lo.js
--rw-r--r--   0        0        0     4825 2022-11-14 15:08:03.610809 anitya-1.7.0/anitya/static/node_modules/moment/locale/lt.js
--rw-r--r--   0        0        0     4137 2022-11-14 15:08:03.612810 anitya-1.7.0/anitya/static/node_modules/moment/locale/lv.js
--rw-r--r--   0        0        0     4441 2022-11-14 15:08:03.614810 anitya-1.7.0/anitya/static/node_modules/moment/locale/me.js
--rw-r--r--   0        0        0     2583 2022-11-14 15:08:03.615810 anitya-1.7.0/anitya/static/node_modules/moment/locale/mi.js
--rw-r--r--   0        0        0     3682 2022-11-14 15:08:03.618810 anitya-1.7.0/anitya/static/node_modules/moment/locale/mk.js
--rw-r--r--   0        0        0     3935 2022-11-14 15:08:03.619809 anitya-1.7.0/anitya/static/node_modules/moment/locale/ml.js
--rw-r--r--   0        0        0     4130 2022-11-14 15:08:03.621810 anitya-1.7.0/anitya/static/node_modules/moment/locale/mn.js
--rw-r--r--   0        0        0     7694 2022-11-14 15:08:03.637810 anitya-1.7.0/anitya/static/node_modules/moment/locale/mr.js
--rw-r--r--   0        0        0     2954 2022-11-14 15:08:03.638810 anitya-1.7.0/anitya/static/node_modules/moment/locale/ms-my.js
--rw-r--r--   0        0        0     2897 2022-11-14 15:08:03.638810 anitya-1.7.0/anitya/static/node_modules/moment/locale/ms.js
--rw-r--r--   0        0        0     2228 2022-11-14 15:08:03.639810 anitya-1.7.0/anitya/static/node_modules/moment/locale/mt.js
--rw-r--r--   0        0        0     3762 2022-11-14 15:08:03.639810 anitya-1.7.0/anitya/static/node_modules/moment/locale/my.js
--rw-r--r--   0        0        0     2451 2022-11-14 15:08:03.640810 anitya-1.7.0/anitya/static/node_modules/moment/locale/nb.js
--rw-r--r--   0        0        0     4831 2022-11-14 15:08:03.641810 anitya-1.7.0/anitya/static/node_modules/moment/locale/ne.js
--rw-r--r--   0        0        0     3881 2022-11-14 15:08:03.641810 anitya-1.7.0/anitya/static/node_modules/moment/locale/nl-be.js
--rw-r--r--   0        0        0     3918 2022-11-14 15:08:03.642810 anitya-1.7.0/anitya/static/node_modules/moment/locale/nl.js
--rw-r--r--   0        0        0     2380 2022-11-14 15:08:03.642810 anitya-1.7.0/anitya/static/node_modules/moment/locale/nn.js
--rw-r--r--   0        0        0     3138 2022-11-14 15:08:03.643810 anitya-1.7.0/anitya/static/node_modules/moment/locale/oc-lnc.js
--rw-r--r--   0        0        0     5006 2022-11-14 15:08:03.646810 anitya-1.7.0/anitya/static/node_modules/moment/locale/pa-in.js
--rw-r--r--   0        0        0     5026 2022-11-14 15:08:03.647810 anitya-1.7.0/anitya/static/node_modules/moment/locale/pl.js
--rw-r--r--   0        0        0     2410 2022-11-14 15:08:03.649810 anitya-1.7.0/anitya/static/node_modules/moment/locale/pt-br.js
--rw-r--r--   0        0        0     2540 2022-11-14 15:08:03.650810 anitya-1.7.0/anitya/static/node_modules/moment/locale/pt.js
--rw-r--r--   0        0        0     2931 2022-11-14 15:08:03.652810 anitya-1.7.0/anitya/static/node_modules/moment/locale/ro.js
--rw-r--r--   0        0        0     9562 2022-11-14 15:08:03.654810 anitya-1.7.0/anitya/static/node_modules/moment/locale/ru.js
--rw-r--r--   0        0        0     2793 2022-11-14 15:08:03.655810 anitya-1.7.0/anitya/static/node_modules/moment/locale/sd.js
--rw-r--r--   0        0        0     2397 2022-11-14 15:08:03.655810 anitya-1.7.0/anitya/static/node_modules/moment/locale/se.js
--rw-r--r--   0        0        0     3277 2022-11-14 15:08:03.656810 anitya-1.7.0/anitya/static/node_modules/moment/locale/si.js
--rw-r--r--   0        0        0     6065 2022-11-14 15:08:03.657810 anitya-1.7.0/anitya/static/node_modules/moment/locale/sk.js
--rw-r--r--   0        0        0     7111 2022-11-14 15:08:03.657810 anitya-1.7.0/anitya/static/node_modules/moment/locale/sl.js
--rw-r--r--   0        0        0     2559 2022-11-14 15:08:03.658810 anitya-1.7.0/anitya/static/node_modules/moment/locale/sq.js
--rw-r--r--   0        0        0     5578 2022-11-14 15:08:03.659810 anitya-1.7.0/anitya/static/node_modules/moment/locale/sr-cyrl.js
--rw-r--r--   0        0        0     5025 2022-11-14 15:08:03.660810 anitya-1.7.0/anitya/static/node_modules/moment/locale/sr.js
--rw-r--r--   0        0        0     3228 2022-11-14 15:08:03.661810 anitya-1.7.0/anitya/static/node_modules/moment/locale/ss.js
--rw-r--r--   0        0        0     2658 2022-11-14 15:08:03.662810 anitya-1.7.0/anitya/static/node_modules/moment/locale/sv.js
--rw-r--r--   0        0        0     2191 2022-11-14 15:08:03.663810 anitya-1.7.0/anitya/static/node_modules/moment/locale/sw.js
--rw-r--r--   0        0        0     5640 2022-11-14 15:08:03.664810 anitya-1.7.0/anitya/static/node_modules/moment/locale/ta.js
--rw-r--r--   0        0        0     4064 2022-11-14 15:08:03.665810 anitya-1.7.0/anitya/static/node_modules/moment/locale/te.js
--rw-r--r--   0        0        0     2741 2022-11-14 15:08:03.666810 anitya-1.7.0/anitya/static/node_modules/moment/locale/tet.js
--rw-r--r--   0        0        0     4388 2022-11-14 15:08:03.667810 anitya-1.7.0/anitya/static/node_modules/moment/locale/tg.js
--rw-r--r--   0        0        0     3316 2022-11-14 15:08:03.667810 anitya-1.7.0/anitya/static/node_modules/moment/locale/th.js
--rw-r--r--   0        0        0     3168 2022-11-14 15:08:03.669810 anitya-1.7.0/anitya/static/node_modules/moment/locale/tk.js
--rw-r--r--   0        0        0     2287 2022-11-14 15:08:03.670810 anitya-1.7.0/anitya/static/node_modules/moment/locale/tl-ph.js
--rw-r--r--   0        0        0     4553 2022-11-14 15:08:03.670810 anitya-1.7.0/anitya/static/node_modules/moment/locale/tlh.js
--rw-r--r--   0        0        0     3663 2022-11-14 15:08:03.673810 anitya-1.7.0/anitya/static/node_modules/moment/locale/tr.js
--rw-r--r--   0        0        0     3779 2022-11-14 15:08:03.674810 anitya-1.7.0/anitya/static/node_modules/moment/locale/tzl.js
--rw-r--r--   0        0        0     2237 2022-11-14 15:08:03.675810 anitya-1.7.0/anitya/static/node_modules/moment/locale/tzm-latn.js
--rw-r--r--   0        0        0     2860 2022-11-14 15:08:03.676810 anitya-1.7.0/anitya/static/node_modules/moment/locale/tzm.js
--rw-r--r--   0        0        0     4644 2022-11-14 15:08:03.688810 anitya-1.7.0/anitya/static/node_modules/moment/locale/ug-cn.js
--rw-r--r--   0        0        0     6927 2022-11-14 15:08:03.689810 anitya-1.7.0/anitya/static/node_modules/moment/locale/uk.js
--rw-r--r--   0        0        0     2840 2022-11-14 15:08:03.690810 anitya-1.7.0/anitya/static/node_modules/moment/locale/ur.js
--rw-r--r--   0        0        0     2183 2022-11-14 15:08:03.691810 anitya-1.7.0/anitya/static/node_modules/moment/locale/uz-latn.js
--rw-r--r--   0        0        0     2409 2022-11-14 15:08:03.692810 anitya-1.7.0/anitya/static/node_modules/moment/locale/uz.js
--rw-r--r--   0        0        0     3066 2022-11-14 15:08:03.694810 anitya-1.7.0/anitya/static/node_modules/moment/locale/vi.js
--rw-r--r--   0        0        0     2970 2022-11-14 15:08:03.695810 anitya-1.7.0/anitya/static/node_modules/moment/locale/x-pseudo.js
--rw-r--r--   0        0        0     2419 2022-11-14 15:08:03.696810 anitya-1.7.0/anitya/static/node_modules/moment/locale/yo.js
--rw-r--r--   0        0        0     4507 2022-11-14 15:08:03.699810 anitya-1.7.0/anitya/static/node_modules/moment/locale/zh-cn.js
--rw-r--r--   0        0        0     3832 2022-11-14 15:08:03.700810 anitya-1.7.0/anitya/static/node_modules/moment/locale/zh-hk.js
--rw-r--r--   0        0        0     3782 2022-11-14 15:08:03.701810 anitya-1.7.0/anitya/static/node_modules/moment/locale/zh-mo.js
--rw-r--r--   0        0        0     3729 2022-11-14 15:08:03.701810 anitya-1.7.0/anitya/static/node_modules/moment/locale/zh-tw.js
--rw-r--r--   0        0        0   448027 2022-11-14 15:08:03.602810 anitya-1.7.0/anitya/static/node_modules/moment/min/locales.js
--rw-r--r--   0        0        0   310773 2022-11-14 15:08:03.609809 anitya-1.7.0/anitya/static/node_modules/moment/min/locales.min.js
--rw-r--r--   0        0        0   140130 2022-11-14 15:08:03.702810 anitya-1.7.0/anitya/static/node_modules/moment/min/locales.min.js.map
--rw-r--r--   0        0        0   622045 2022-11-14 15:08:03.629810 anitya-1.7.0/anitya/static/node_modules/moment/min/moment-with-locales.js
--rw-r--r--   0        0        0   369019 2022-11-14 15:08:03.634810 anitya-1.7.0/anitya/static/node_modules/moment/min/moment-with-locales.min.js
--rw-r--r--   0        0        0   230173 2022-11-14 15:08:03.704810 anitya-1.7.0/anitya/static/node_modules/moment/min/moment-with-locales.min.js.map
--rw-r--r--   0        0        0    58103 2022-11-14 15:08:03.636810 anitya-1.7.0/anitya/static/node_modules/moment/min/moment.min.js
--rw-r--r--   0        0        0    86041 2022-11-14 15:08:03.705810 anitya-1.7.0/anitya/static/node_modules/moment/min/moment.min.js.map
--rw-r--r--   0        0        0    23820 2022-11-14 15:08:03.705810 anitya-1.7.0/anitya/static/node_modules/moment/moment.d.ts
--rw-r--r--   0        0        0   174604 2022-11-14 15:08:03.636810 anitya-1.7.0/anitya/static/node_modules/moment/moment.js
--rw-r--r--   0        0        0      273 2022-11-14 15:08:03.646810 anitya-1.7.0/anitya/static/node_modules/moment/package.js
--rw-r--r--   0        0        0     3418 2022-11-14 15:08:03.702810 anitya-1.7.0/anitya/static/node_modules/moment/package.json
--rw-r--r--   0        0        0     1542 2022-11-14 15:08:03.470809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/check-overflow.js
--rw-r--r--   0        0        0     1076 2022-11-14 15:08:03.479809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/date-from-array.js
--rw-r--r--   0        0        0     3351 2022-11-14 15:08:03.545809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/from-anything.js
--rw-r--r--   0        0        0     5585 2022-11-14 15:08:03.546809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/from-array.js
--rw-r--r--   0        0        0      549 2022-11-14 15:08:03.546809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/from-object.js
--rw-r--r--   0        0        0     2011 2022-11-14 15:08:03.546809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/from-string-and-array.js
--rw-r--r--   0        0        0     4092 2022-11-14 15:08:03.547809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/from-string-and-format.js
--rw-r--r--   0        0        0     8007 2022-11-14 15:08:03.547809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/from-string.js
--rw-r--r--   0        0        0      183 2022-11-14 15:08:03.596809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/local.js
--rw-r--r--   0        0        0      644 2022-11-14 15:08:03.646810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/parsing-flags.js
--rw-r--r--   0        0        0      186 2022-11-14 15:08:03.690810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/utc.js
--rw-r--r--   0        0        0     1514 2022-11-14 15:08:03.692810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/valid.js
--rw-r--r--   0        0        0      484 2022-11-14 15:08:03.414809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/abs.js
--rw-r--r--   0        0        0      644 2022-11-14 15:08:03.415809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/add-subtract.js
--rw-r--r--   0        0        0     2360 2022-11-14 15:08:03.441809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/as.js
--rw-r--r--   0        0        0     1774 2022-11-14 15:08:03.466809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/bubble.js
--rw-r--r--   0        0        0      105 2022-11-14 15:08:03.470809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/clone.js
--rw-r--r--   0        0        0     1593 2022-11-14 15:08:03.472809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/constructor.js
--rw-r--r--   0        0        0     4335 2022-11-14 15:08:03.474809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/create.js
--rw-r--r--   0        0        0      342 2022-11-14 15:08:03.487809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/duration.js
--rw-r--r--   0        0        0      728 2022-11-14 15:08:03.552809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/get.js
--rw-r--r--   0        0        0     3493 2022-11-14 15:08:03.567809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/humanize.js
--rw-r--r--   0        0        0     2078 2022-11-14 15:08:03.578809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/iso-string.js
--rw-r--r--   0        0        0     1739 2022-11-14 15:08:03.647810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/prototype.js
--rw-r--r--   0        0        0     1184 2022-11-14 15:08:03.693810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/valid.js
--rw-r--r--   0        0        0     2911 2022-11-14 15:08:03.538809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/format/format.js
--rw-r--r--   0        0        0     1187 2022-11-14 15:08:03.452809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/base-config.js
--rw-r--r--   0        0        0      442 2022-11-14 15:08:03.467809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/calendar.js
--rw-r--r--   0        0        0       93 2022-11-14 15:08:03.472809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/constructor.js
--rw-r--r--   0        0        0      989 2022-11-14 15:08:03.511809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/en.js
--rw-r--r--   0        0        0      876 2022-11-14 15:08:03.540809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/formats.js
--rw-r--r--   0        0        0      113 2022-11-14 15:08:03.572809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/invalid.js
--rw-r--r--   0        0        0     2188 2022-11-14 15:08:03.594809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/lists.js
--rw-r--r--   0        0        0      829 2022-11-14 15:08:03.596809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/locale.js
--rw-r--r--   0        0        0     7728 2022-11-14 15:08:03.602810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/locales.js
--rw-r--r--   0        0        0      218 2022-11-14 15:08:03.643810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/ordinal.js
--rw-r--r--   0        0        0       66 2022-11-14 15:08:03.647810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/pre-post-format.js
--rw-r--r--   0        0        0     2229 2022-11-14 15:08:03.648810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/prototype.js
--rw-r--r--   0        0        0      842 2022-11-14 15:08:03.652810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/relative.js
--rw-r--r--   0        0        0     1831 2022-11-14 15:08:03.656810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/set.js
--rw-r--r--   0        0        0     1869 2022-11-14 15:08:03.419809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/add-subtract.js
--rw-r--r--   0        0        0     1737 2022-11-14 15:08:03.467809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/calendar.js
--rw-r--r--   0        0        0       98 2022-11-14 15:08:03.471809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/clone.js
--rw-r--r--   0        0        0     2379 2022-11-14 15:08:03.471809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/compare.js
--rw-r--r--   0        0        0     2106 2022-11-14 15:08:03.473809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/constructor.js
--rw-r--r--   0        0        0      192 2022-11-14 15:08:03.475809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/creation-data.js
--rw-r--r--   0        0        0     2345 2022-11-14 15:08:03.486809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/diff.js
--rw-r--r--   0        0        0     2340 2022-11-14 15:08:03.539809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/format.js
--rw-r--r--   0        0        0      609 2022-11-14 15:08:03.547809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/from.js
--rw-r--r--   0        0        0     2041 2022-11-14 15:08:03.552809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/get-set.js
--rw-r--r--   0        0        0      946 2022-11-14 15:08:03.596809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/locale.js
--rw-r--r--   0        0        0     1922 2022-11-14 15:08:03.617810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/min-max.js
--rw-r--r--   0        0        0      609 2022-11-14 15:08:03.636810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/moment.js
--rw-r--r--   0        0        0       82 2022-11-14 15:08:03.643810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/now.js
--rw-r--r--   0        0        0     5511 2022-11-14 15:08:03.648810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/prototype.js
--rw-r--r--   0        0        0     4819 2022-11-14 15:08:03.661810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/start-end-of.js
--rw-r--r--   0        0        0      834 2022-11-14 15:08:03.672810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/to-type.js
--rw-r--r--   0        0        0      603 2022-11-14 15:08:03.672810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/to.js
--rw-r--r--   0        0        0      364 2022-11-14 15:08:03.693810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/valid.js
--rw-r--r--   0        0        0     2500 2022-11-14 15:08:03.652810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/parse/regex.js
--rw-r--r--   0        0        0      958 2022-11-14 15:08:03.672810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/parse/token.js
--rw-r--r--   0        0        0      809 2022-11-14 15:08:03.426809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/aliases.js
--rw-r--r--   0        0        0      148 2022-11-14 15:08:03.471809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/constants.js
--rw-r--r--   0        0        0     1065 2022-11-14 15:08:03.479809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/day-of-month.js
--rw-r--r--   0        0        0    12904 2022-11-14 15:08:03.480809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/day-of-week.js
--rw-r--r--   0        0        0      920 2022-11-14 15:08:03.480809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/day-of-year.js
--rw-r--r--   0        0        0     7984 2022-11-14 15:08:03.514809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/era.js
--rw-r--r--   0        0        0     4475 2022-11-14 15:08:03.564809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/hour.js
--rw-r--r--   0        0        0     1870 2022-11-14 15:08:03.616809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/millisecond.js
--rw-r--r--   0        0        0      679 2022-11-14 15:08:03.617810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/minute.js
--rw-r--r--   0        0        0    10021 2022-11-14 15:08:03.637810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/month.js
--rw-r--r--   0        0        0     7070 2022-11-14 15:08:03.643810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/offset.js
--rw-r--r--   0        0        0      480 2022-11-14 15:08:03.647810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/priorities.js
--rw-r--r--   0        0        0      780 2022-11-14 15:08:03.651810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/quarter.js
--rw-r--r--   0        0        0      679 2022-11-14 15:08:03.656810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/second.js
--rw-r--r--   0        0        0      590 2022-11-14 15:08:03.668810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/timestamp.js
--rw-r--r--   0        0        0      325 2022-11-14 15:08:03.668810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/timezone.js
--rw-r--r--   0        0        0      404 2022-11-14 15:08:03.689810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/units.js
--rw-r--r--   0        0        0     2107 2022-11-14 15:08:03.694810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/week-calendar-utils.js
--rw-r--r--   0        0        0     3483 2022-11-14 15:08:03.694810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/week-year.js
--rw-r--r--   0        0        0     1664 2022-11-14 15:08:03.694810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/week.js
--rw-r--r--   0        0        0     2001 2022-11-14 15:08:03.695810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/year.js
--rw-r--r--   0        0        0      154 2022-11-14 15:08:03.411809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/abs-ceil.js
--rw-r--r--   0        0        0      179 2022-11-14 15:08:03.411809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/abs-floor.js
--rw-r--r--   0        0        0      166 2022-11-14 15:08:03.412809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/abs-round.js
--rw-r--r--   0        0        0      553 2022-11-14 15:08:03.471809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/compare-arrays.js
--rw-r--r--   0        0        0      203 2022-11-14 15:08:03.486809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/defaults.js
--rw-r--r--   0        0        0     1946 2022-11-14 15:08:03.486809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/deprecate.js
--rw-r--r--   0        0        0      345 2022-11-14 15:08:03.526809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/extend.js
--rw-r--r--   0        0        0      100 2022-11-14 15:08:03.560809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/has-own-prop.js
--rw-r--r--   0        0        0      296 2022-11-14 15:08:03.563809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/hooks.js
--rw-r--r--   0        0        0      342 2022-11-14 15:08:03.572809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/index-of.js
--rw-r--r--   0        0        0      164 2022-11-14 15:08:03.573809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/is-array.js
--rw-r--r--   0        0        0      670 2022-11-14 15:08:03.573809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/is-calendar-spec.js
--rw-r--r--   0        0        0      161 2022-11-14 15:08:03.573809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/is-date.js
--rw-r--r--   0        0        0      210 2022-11-14 15:08:03.574809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/is-function.js
--rw-r--r--   0        0        0      106 2022-11-14 15:08:03.574809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/is-leap-year.js
--rw-r--r--   0        0        0     1988 2022-11-14 15:08:03.574809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/is-moment-input.js
--rw-r--r--   0        0        0      169 2022-11-14 15:08:03.575809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/is-number.js
--rw-r--r--   0        0        0      360 2022-11-14 15:08:03.575809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/is-object-empty.js
--rw-r--r--   0        0        0      246 2022-11-14 15:08:03.576810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/is-object.js
--rw-r--r--   0        0        0      109 2022-11-14 15:08:03.576810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/is-string.js
--rw-r--r--   0        0        0       76 2022-11-14 15:08:03.576810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/is-undefined.js
--rw-r--r--   0        0        0      344 2022-11-14 15:08:03.584809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/keys.js
--rw-r--r--   0        0        0      189 2022-11-14 15:08:03.613809 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/map.js
--rw-r--r--   0        0        0       68 2022-11-14 15:08:03.622810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/mod.js
--rw-r--r--   0        0        0      394 2022-11-14 15:08:03.658810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/some.js
--rw-r--r--   0        0        0      282 2022-11-14 15:08:03.671810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/to-int.js
--rw-r--r--   0        0        0      352 2022-11-14 15:08:03.697810 anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/zero-fill.js
--rw-r--r--   0        0        0     2149 2022-11-14 15:08:03.424809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/af.js
--rw-r--r--   0        0        0     4449 2022-11-14 15:08:03.428809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar-dz.js
--rw-r--r--   0        0        0     1934 2022-11-14 15:08:03.429809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar-kw.js
--rw-r--r--   0        0        0     4648 2022-11-14 15:08:03.432809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar-ly.js
--rw-r--r--   0        0        0     1989 2022-11-14 15:08:03.436809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar-ma.js
--rw-r--r--   0        0        0     3042 2022-11-14 15:08:03.438809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar-sa.js
--rw-r--r--   0        0        0     1936 2022-11-14 15:08:03.439809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar-tn.js
--rw-r--r--   0        0        0     5072 2022-11-14 15:08:03.441809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar.js
--rw-r--r--   0        0        0     2846 2022-11-14 15:08:03.449809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/az.js
--rw-r--r--   0        0        0     5154 2022-11-14 15:08:03.454809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/be.js
--rw-r--r--   0        0        0     2955 2022-11-14 15:08:03.456809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/bg.js
--rw-r--r--   0        0        0     1784 2022-11-14 15:08:03.459809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/bm.js
--rw-r--r--   0        0        0     4349 2022-11-14 15:08:03.460809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/bn-bd.js
--rw-r--r--   0        0        0     3898 2022-11-14 15:08:03.462809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/bn.js
--rw-r--r--   0        0        0     4399 2022-11-14 15:08:03.464809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/bo.js
--rw-r--r--   0        0        0     4544 2022-11-14 15:08:03.465809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/br.js
--rw-r--r--   0        0        0     4475 2022-11-14 15:08:03.466809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/bs.js
--rw-r--r--   0        0        0     3031 2022-11-14 15:08:03.467809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ca.js
--rw-r--r--   0        0        0     6718 2022-11-14 15:08:03.476809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/cs.js
--rw-r--r--   0        0        0     2341 2022-11-14 15:08:03.476809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/cv.js
--rw-r--r--   0        0        0     2834 2022-11-14 15:08:03.478809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/cy.js
--rw-r--r--   0        0        0     1629 2022-11-14 15:08:03.478809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/da.js
--rw-r--r--   0        0        0     2635 2022-11-14 15:08:03.481809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/de-at.js
--rw-r--r--   0        0        0     2563 2022-11-14 15:08:03.483809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/de-ch.js
--rw-r--r--   0        0        0     2562 2022-11-14 15:08:03.485809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/de.js
--rw-r--r--   0        0        0     2464 2022-11-14 15:08:03.488809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/dv.js
--rw-r--r--   0        0        0     3877 2022-11-14 15:08:03.489809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/el.js
--rw-r--r--   0        0        0     2029 2022-11-14 15:08:03.491809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-au.js
--rw-r--r--   0        0        0     1878 2022-11-14 15:08:03.492809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-ca.js
--rw-r--r--   0        0        0     2035 2022-11-14 15:08:03.494809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-gb.js
--rw-r--r--   0        0        0     2033 2022-11-14 15:08:03.497809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-ie.js
--rw-r--r--   0        0        0     1871 2022-11-14 15:08:03.500809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-il.js
--rw-r--r--   0        0        0     2029 2022-11-14 15:08:03.502809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-in.js
--rw-r--r--   0        0        0     2038 2022-11-14 15:08:03.504809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-nz.js
--rw-r--r--   0        0        0     2047 2022-11-14 15:08:03.510809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-sg.js
--rw-r--r--   0        0        0     2338 2022-11-14 15:08:03.513809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/eo.js
--rw-r--r--   0        0        0     3441 2022-11-14 15:08:03.517809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/es-do.js
--rw-r--r--   0        0        0     3510 2022-11-14 15:08:03.518809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/es-mx.js
--rw-r--r--   0        0        0     3538 2022-11-14 15:08:03.521809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/es-us.js
--rw-r--r--   0        0        0     3498 2022-11-14 15:08:03.523809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/es.js
--rw-r--r--   0        0        0     2631 2022-11-14 15:08:03.524809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/et.js
--rw-r--r--   0        0        0     1964 2022-11-14 15:08:03.526809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/eu.js
--rw-r--r--   0        0        0     3230 2022-11-14 15:08:03.527809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fa.js
--rw-r--r--   0        0        0     3632 2022-11-14 15:08:03.529809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fi.js
--rw-r--r--   0        0        0     1776 2022-11-14 15:08:03.531809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fil.js
--rw-r--r--   0        0        0     1772 2022-11-14 15:08:03.534809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fo.js
--rw-r--r--   0        0        0     2104 2022-11-14 15:08:03.541809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fr-ca.js
--rw-r--r--   0        0        0     2263 2022-11-14 15:08:03.543809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fr-ch.js
--rw-r--r--   0        0        0     3471 2022-11-14 15:08:03.544809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fr.js
--rw-r--r--   0        0        0     2275 2022-11-14 15:08:03.549809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fy.js
--rw-r--r--   0        0        0     2360 2022-11-14 15:08:03.550809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ga.js
--rw-r--r--   0        0        0     2380 2022-11-14 15:08:03.551809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/gd.js
--rw-r--r--   0        0        0     2347 2022-11-14 15:08:03.555809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/gl.js
--rw-r--r--   0        0        0     5506 2022-11-14 15:08:03.556809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/gom-deva.js
--rw-r--r--   0        0        0     4130 2022-11-14 15:08:03.558809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/gom-latn.js
--rw-r--r--   0        0        0     4132 2022-11-14 15:08:03.559809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/gu.js
--rw-r--r--   0        0        0     3211 2022-11-14 15:08:03.561809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/he.js
--rw-r--r--   0        0        0     6421 2022-11-14 15:08:03.563809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/hi.js
--rw-r--r--   0        0        0     4718 2022-11-14 15:08:03.566809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/hr.js
--rw-r--r--   0        0        0     3815 2022-11-14 15:08:03.567809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/hu.js
--rw-r--r--   0        0        0     3236 2022-11-14 15:08:03.570809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/hy-am.js
--rw-r--r--   0        0        0     2375 2022-11-14 15:08:03.571809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/id.js
--rw-r--r--   0        0        0     4458 2022-11-14 15:08:03.577809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/is.js
--rw-r--r--   0        0        0     1941 2022-11-14 15:08:03.579810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/it-ch.js
--rw-r--r--   0        0        0     3251 2022-11-14 15:08:03.580809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/it.js
--rw-r--r--   0        0        0     3955 2022-11-14 15:08:03.581809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ja.js
--rw-r--r--   0        0        0     2384 2022-11-14 15:08:03.583809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/jv.js
--rw-r--r--   0        0        0     3504 2022-11-14 15:08:03.584809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ka.js
--rw-r--r--   0        0        0     2495 2022-11-14 15:08:03.585809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/kk.js
--rw-r--r--   0        0        0     3362 2022-11-14 15:08:03.587809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/km.js
--rw-r--r--   0        0        0     4252 2022-11-14 15:08:03.588809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/kn.js
--rw-r--r--   0        0        0     2223 2022-11-14 15:08:03.590809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ko.js
--rw-r--r--   0        0        0     3330 2022-11-14 15:08:03.591809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ku.js
--rw-r--r--   0        0        0     2521 2022-11-14 15:08:03.592810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ky.js
--rw-r--r--   0        0        0     4269 2022-11-14 15:08:03.594809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/lb.js
--rw-r--r--   0        0        0     2585 2022-11-14 15:08:03.595810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/lo.js
--rw-r--r--   0        0        0     4005 2022-11-14 15:08:03.610809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/lt.js
--rw-r--r--   0        0        0     3449 2022-11-14 15:08:03.613809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/lv.js
--rw-r--r--   0        0        0     3661 2022-11-14 15:08:03.614810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/me.js
--rw-r--r--   0        0        0     2023 2022-11-14 15:08:03.616809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/mi.js
--rw-r--r--   0        0        0     3021 2022-11-14 15:08:03.619809 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/mk.js
--rw-r--r--   0        0        0     3287 2022-11-14 15:08:03.620810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ml.js
--rw-r--r--   0        0        0     3414 2022-11-14 15:08:03.621810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/mn.js
--rw-r--r--   0        0        0     6574 2022-11-14 15:08:03.637810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/mr.js
--rw-r--r--   0        0        0     2330 2022-11-14 15:08:03.638810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ms-my.js
--rw-r--r--   0        0        0     2277 2022-11-14 15:08:03.638810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ms.js
--rw-r--r--   0        0        0     1684 2022-11-14 15:08:03.639810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/mt.js
--rw-r--r--   0        0        0     3094 2022-11-14 15:08:03.640810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/my.js
--rw-r--r--   0        0        0     1899 2022-11-14 15:08:03.640810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/nb.js
--rw-r--r--   0        0        0     4031 2022-11-14 15:08:03.641810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ne.js
--rw-r--r--   0        0        0     3169 2022-11-14 15:08:03.641810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/nl-be.js
--rw-r--r--   0        0        0     3202 2022-11-14 15:08:03.642810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/nl.js
--rw-r--r--   0        0        0     1828 2022-11-14 15:08:03.642810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/nn.js
--rw-r--r--   0        0        0     2472 2022-11-14 15:08:03.643810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/oc-lnc.js
--rw-r--r--   0        0        0     4198 2022-11-14 15:08:03.646810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/pa-in.js
--rw-r--r--   0        0        0     4166 2022-11-14 15:08:03.647810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/pl.js
--rw-r--r--   0        0        0     1854 2022-11-14 15:08:03.650810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/pt-br.js
--rw-r--r--   0        0        0     1968 2022-11-14 15:08:03.650810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/pt.js
--rw-r--r--   0        0        0     2319 2022-11-14 15:08:03.652810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ro.js
--rw-r--r--   0        0        0     8418 2022-11-14 15:08:03.654810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ru.js
--rw-r--r--   0        0        0     2153 2022-11-14 15:08:03.655810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sd.js
--rw-r--r--   0        0        0     1849 2022-11-14 15:08:03.656810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/se.js
--rw-r--r--   0        0        0     2681 2022-11-14 15:08:03.656810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/si.js
--rw-r--r--   0        0        0     5173 2022-11-14 15:08:03.657810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sk.js
--rw-r--r--   0        0        0     6115 2022-11-14 15:08:03.658810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sl.js
--rw-r--r--   0        0        0     1987 2022-11-14 15:08:03.658810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sq.js
--rw-r--r--   0        0        0     4762 2022-11-14 15:08:03.659810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sr-cyrl.js
--rw-r--r--   0        0        0     4209 2022-11-14 15:08:03.660810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sr.js
--rw-r--r--   0        0        0     2572 2022-11-14 15:08:03.661810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ss.js
--rw-r--r--   0        0        0     2066 2022-11-14 15:08:03.663810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sv.js
--rw-r--r--   0        0        0     1651 2022-11-14 15:08:03.663810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sw.js
--rw-r--r--   0        0        0     4800 2022-11-14 15:08:03.664810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ta.js
--rw-r--r--   0        0        0     3392 2022-11-14 15:08:03.665810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/te.js
--rw-r--r--   0        0        0     2155 2022-11-14 15:08:03.666810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tet.js
--rw-r--r--   0        0        0     3604 2022-11-14 15:08:03.667810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tg.js
--rw-r--r--   0        0        0     2736 2022-11-14 15:08:03.668810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/th.js
--rw-r--r--   0        0        0     2488 2022-11-14 15:08:03.669810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tk.js
--rw-r--r--   0        0        0     1735 2022-11-14 15:08:03.670810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tl-ph.js
--rw-r--r--   0        0        0     3755 2022-11-14 15:08:03.671810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tlh.js
--rw-r--r--   0        0        0     2927 2022-11-14 15:08:03.673810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tr.js
--rw-r--r--   0        0        0     3109 2022-11-14 15:08:03.674810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tzl.js
--rw-r--r--   0        0        0     1691 2022-11-14 15:08:03.675810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tzm-latn.js
--rw-r--r--   0        0        0     2322 2022-11-14 15:08:03.681810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tzm.js
--rw-r--r--   0        0        0     3880 2022-11-14 15:08:03.688810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ug-cn.js
--rw-r--r--   0        0        0     5955 2022-11-14 15:08:03.689810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/uk.js
--rw-r--r--   0        0        0     2200 2022-11-14 15:08:03.690810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ur.js
--rw-r--r--   0        0        0     1639 2022-11-14 15:08:03.691810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/uz-latn.js
--rw-r--r--   0        0        0     1885 2022-11-14 15:08:03.692810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/uz.js
--rw-r--r--   0        0        0     2430 2022-11-14 15:08:03.694810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/vi.js
--rw-r--r--   0        0        0     2348 2022-11-14 15:08:03.695810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/x-pseudo.js
--rw-r--r--   0        0        0     1887 2022-11-14 15:08:03.696810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/yo.js
--rw-r--r--   0        0        0     3711 2022-11-14 15:08:03.700810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/zh-cn.js
--rw-r--r--   0        0        0     3116 2022-11-14 15:08:03.701810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/zh-hk.js
--rw-r--r--   0        0        0     3066 2022-11-14 15:08:03.701810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/zh-mo.js
--rw-r--r--   0        0        0     3013 2022-11-14 15:08:03.702810 anitya-1.7.0/anitya/static/node_modules/moment/src/locale/zh-tw.js
--rw-r--r--   0        0        0     2694 2022-11-14 15:08:03.636810 anitya-1.7.0/anitya/static/node_modules/moment/src/moment.js
--rw-r--r--   0        0        0    23327 2022-11-14 15:08:03.705810 anitya-1.7.0/anitya/static/node_modules/moment/ts3.1-typings/moment.d.ts
--rw-r--r--   0        0        0     3584 2022-12-14 14:15:40.107732 anitya-1.7.0/anitya/static/package-lock.json
--rw-r--r--   0        0        0      765 2022-12-14 14:15:40.108732 anitya-1.7.0/anitya/static/package.json
--rw-r--r--   0        0        0     2970 2020-12-02 09:02:04.993902 anitya-1.7.0/anitya/static/yahoo_logo.png
--rw-r--r--   0        0        0        0 2020-12-02 09:02:04.993902 anitya-1.7.0/anitya/templates/__init__.py
--rw-r--r--   0        0        0     3236 2022-12-14 14:15:40.108732 anitya-1.7.0/anitya/templates/distro_add_edit.html
--rw-r--r--   0        0        0      596 2022-12-14 14:15:40.113732 anitya-1.7.0/anitya/templates/distro_delete.html
--rw-r--r--   0        0        0     2293 2022-12-14 14:15:40.113732 anitya-1.7.0/anitya/templates/distros.html
--rw-r--r--   0        0        0     4148 2022-12-14 14:15:40.114732 anitya-1.7.0/anitya/templates/flags.html
--rw-r--r--   0        0        0      438 2020-12-02 09:02:04.994902 anitya-1.7.0/anitya/templates/functions.html
--rw-r--r--   0        0        0     1626 2022-12-14 14:15:40.114732 anitya-1.7.0/anitya/templates/index.html
--rw-r--r--   0        0        0     1019 2022-12-14 14:15:40.116732 anitya-1.7.0/anitya/templates/login.html
--rw-r--r--   0        0        0     2388 2022-12-14 14:15:40.116732 anitya-1.7.0/anitya/templates/logs.html
--rw-r--r--   0        0        0     1762 2022-12-14 14:15:40.116732 anitya-1.7.0/anitya/templates/mapping.html
--rw-r--r--   0        0        0     9973 2022-12-14 14:15:40.117732 anitya-1.7.0/anitya/templates/master.html
--rw-r--r--   0        0        0    14965 2022-12-14 14:15:40.123732 anitya-1.7.0/anitya/templates/project.html
--rw-r--r--   0        0        0     3734 2022-12-14 14:15:40.123732 anitya-1.7.0/anitya/templates/project_archive.html
--rw-r--r--   0        0        0     3053 2022-12-14 14:15:40.124732 anitya-1.7.0/anitya/templates/project_delete.html
--rw-r--r--   0        0        0     1134 2022-12-14 14:15:40.124732 anitya-1.7.0/anitya/templates/project_flag.html
--rw-r--r--   0        0        0    17245 2022-12-14 14:15:40.129732 anitya-1.7.0/anitya/templates/project_new.html
--rw-r--r--   0        0        0      999 2022-12-14 14:15:40.130732 anitya-1.7.0/anitya/templates/project_versions_delete.html
--rw-r--r--   0        0        0     3751 2022-12-14 14:15:40.130732 anitya-1.7.0/anitya/templates/projects.html
--rw-r--r--   0        0        0     1354 2022-12-14 14:15:40.130732 anitya-1.7.0/anitya/templates/regex_delete.html
--rw-r--r--   0        0        0     3543 2022-12-14 14:15:40.131732 anitya-1.7.0/anitya/templates/search.html
--rw-r--r--   0        0        0     2101 2022-12-14 14:15:40.132732 anitya-1.7.0/anitya/templates/settings.html
--rw-r--r--   0        0        0     4848 2022-12-14 14:15:40.137732 anitya-1.7.0/anitya/templates/updates.html
--rw-r--r--   0        0        0     4393 2022-12-14 14:15:40.137732 anitya-1.7.0/anitya/templates/users.html
--rw-r--r--   0        0        0     1250 2022-12-14 14:15:40.138732 anitya-1.7.0/anitya/templates/version_delete.html
--rw-r--r--   0        0        0    23996 2022-12-14 14:15:41.885738 anitya-1.7.0/anitya/ui.py
--rw-r--r--   0        0        0      835 2020-12-02 09:02:05.009902 anitya-1.7.0/anitya/wsgi.py
--rw-r--r--   0        0        0     1866 2020-12-02 09:02:05.011902 anitya-1.7.0/createdb.py
--rw-r--r--   0        0        0     3954 2022-12-14 14:15:41.913739 anitya-1.7.0/files/anitya.toml.sample
--rw-r--r--   0        0        0      364 2020-12-02 09:02:05.012902 anitya-1.7.0/files/config.toml.sample
--rw-r--r--   0        0        0     3491 2023-01-26 12:00:09.384181 anitya-1.7.0/pyproject.toml
--rw-r--r--   0        0        0    16615 2023-01-26 12:07:38.422862 anitya-1.7.0/setup.py
--rw-r--r--   0        0        0     3692 2023-01-26 12:07:38.423556 anitya-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0    18002 2020-12-02 09:02:04.975902 anitya-1.8.0/LICENSE
+-rw-r--r--   0        0        0     1904 2022-06-22 14:20:39.926825 anitya-1.8.0/README.rst
+-rw-r--r--   0        0        0     1184 2020-12-02 09:02:04.975902 anitya-1.8.0/alembic.ini
+-rw-r--r--   0        0        0      124 2022-12-14 14:15:40.056732 anitya-1.8.0/anitya/__init__.py
+-rw-r--r--   0        0        0    18442 2023-04-24 16:04:41.035772 anitya-1.8.0/anitya/admin.py
+-rw-r--r--   0        0        0    15353 2023-04-24 16:04:41.036772 anitya-1.8.0/anitya/api.py
+-rw-r--r--   0        0        0    31952 2023-04-24 16:04:41.037772 anitya-1.8.0/anitya/api_v2.py
+-rw-r--r--   0        0        0     7621 2022-10-03 14:15:14.613326 anitya-1.8.0/anitya/app.py
+-rw-r--r--   0        0        0     4450 2020-12-02 09:02:04.976902 anitya-1.8.0/anitya/authentication.py
+-rw-r--r--   0        0        0    11974 2023-04-24 16:04:41.037772 anitya-1.8.0/anitya/check_service.py
+-rw-r--r--   0        0        0     1113 2020-12-02 09:02:04.976902 anitya-1.8.0/anitya/compat.py
+-rw-r--r--   0        0        0     5894 2022-12-14 14:15:40.074732 anitya-1.8.0/anitya/config.py
+-rw-r--r--   0        0        0     1368 2020-12-02 09:02:04.976902 anitya-1.8.0/anitya/db/__init__.py
+-rw-r--r--   0        0        0     3132 2020-12-02 09:02:04.976902 anitya-1.8.0/anitya/db/events.py
+-rw-r--r--   0        0        0     5777 2020-12-02 09:02:04.976902 anitya-1.8.0/anitya/db/meta.py
+-rw-r--r--   0        0        0      464 2020-12-02 09:02:04.976902 anitya-1.8.0/anitya/db/migrations/README.md
+-rw-r--r--   0        0        0        0 2020-12-02 09:02:04.976902 anitya-1.8.0/anitya/db/migrations/__init__.py
+-rw-r--r--   0        0        0     2106 2022-06-22 14:20:39.932825 anitya-1.8.0/anitya/db/migrations/env.py
+-rw-r--r--   0        0        0      413 2020-12-02 09:02:04.976902 anitya-1.8.0/anitya/db/migrations/script.py.mako
+-rw-r--r--   0        0        0      658 2020-12-02 09:02:04.976902 anitya-1.8.0/anitya/db/migrations/versions/136d119ab015_rename_project_latest_known_cursor_to_.py
+-rw-r--r--   0        0        0      542 2020-12-02 09:02:04.976902 anitya-1.8.0/anitya/db/migrations/versions/16aa7da2764c_add_projectversion_commit_url.py
+-rw-r--r--   0        0        0      592 2022-06-22 14:20:39.932825 anitya-1.8.0/anitya/db/migrations/versions/1ab95561edae_convert_date_to_rpm.py
+-rw-r--r--   0        0        0     1391 2022-06-22 14:20:39.932825 anitya-1.8.0/anitya/db/migrations/versions/1bf8aead6179_add_check_times.py
+-rw-r--r--   0        0        0      663 2022-06-22 14:20:39.932825 anitya-1.8.0/anitya/db/migrations/versions/1f839c54e428_add_archive_flag.py
+-rw-r--r--   0        0        0      635 2022-06-22 14:20:39.932825 anitya-1.8.0/anitya/db/migrations/versions/24b6734e8565_creation_date_on_version.py
+-rw-r--r--   0        0        0      747 2022-06-22 14:20:39.932825 anitya-1.8.0/anitya/db/migrations/versions/27342bce1d0f_populate_project_version_scheme.py
+-rw-r--r--   0        0        0      591 2022-06-22 14:20:39.933825 anitya-1.8.0/anitya/db/migrations/versions/2925648d8cc3_add_a_version_prefix_field.py
+-rw-r--r--   0        0        0      557 2021-03-18 13:23:05.984865 anitya-1.8.0/anitya/db/migrations/versions/2d1aa7ff82a5_remove_code_google_backend.py
+-rw-r--r--   0        0        0      803 2022-06-22 14:20:39.933825 anitya-1.8.0/anitya/db/migrations/versions/314651690dc7_add_error_counter_to_project.py
+-rw-r--r--   0        0        0     1810 2020-12-02 09:02:04.976902 anitya-1.8.0/anitya/db/migrations/versions/34b9bb5fa388_make_ecosystem_non_nullable.py
+-rw-r--r--   0        0        0     3722 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/3fae8239eeec_add_an_api_token_table.py
+-rw-r--r--   0        0        0      882 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/540bdcf7edbc_convert_github_url_to_owner_project.py
+-rw-r--r--   0        0        0      676 2022-06-22 14:20:39.933825 anitya-1.8.0/anitya/db/migrations/versions/571bd07533a9_add_insecure_column_to_projects_table.py
+-rw-r--r--   0        0        0      590 2022-06-22 14:20:39.933825 anitya-1.8.0/anitya/db/migrations/versions/5b8b587d7dbe_add_version_filter_column.py
+-rw-r--r--   0        0        0      695 2022-06-22 14:20:39.934825 anitya-1.8.0/anitya/db/migrations/versions/5e209766aead_add_release_check_to_project.py
+-rw-r--r--   0        0        0     1738 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/6ac0e42df937_drop_logs_table.py
+-rw-r--r--   0        0        0      557 2022-06-22 14:20:39.934825 anitya-1.8.0/anitya/db/migrations/versions/708f6f26b4b6_add_version_pattern.py
+-rw-r--r--   0        0        0     1023 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/7a8c4aa92678_add_missing_github_owner_project_pairs.py
+-rw-r--r--   0        0        0      610 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/8040ef9a9dda_add_a_version_scheme_column_to_projects.py
+-rw-r--r--   0        0        0      684 2021-02-12 16:21:32.439942 anitya-1.8.0/anitya/db/migrations/versions/8be6e153962c_remove_cursor.py
+-rw-r--r--   0        0        0      970 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/921c612ba0da_model_upstream_ecosystems.py
+-rw-r--r--   0        0        0      544 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/92a2e9eba0a7_add_project_latest_known_cursor.py
+-rw-r--r--   0        0        0      928 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/9c29da0af3af_populate_ecosystem_data.py
+-rw-r--r--   0        0        0        0 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/__init__.py
+-rw-r--r--   0        0        0     3126 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/a52d2fe99d4f_users.py
+-rw-r--r--   0        0        0      301 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/ac10bf3f974c_.py
+-rw-r--r--   0        0        0      495 2022-06-22 14:20:39.934825 anitya-1.8.0/anitya/db/migrations/versions/b13662e5d288_add_admin_flag.py
+-rw-r--r--   0        0        0     2881 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/b9201d816075_remove_the_backends_and_ecosystems_.py
+-rw-r--r--   0        0        0      409 2022-06-22 14:20:39.934825 anitya-1.8.0/anitya/db/migrations/versions/c8735fa14a0a_add_cascade_delete.py
+-rw-r--r--   0        0        0      596 2020-12-02 09:04:10.562083 anitya-1.8.0/anitya/db/migrations/versions/d6170cfc2814_add_pre_release_flag.py
+-rw-r--r--   0        0        0     1148 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/e34988f3e2f4_add_statistics_to_run.py
+-rw-r--r--   0        0        0     6582 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/db/migrations/versions/feeaa70ead67_social_authentication_table.py
+-rw-r--r--   0        0        0    35192 2023-04-24 16:04:41.038772 anitya-1.8.0/anitya/db/models.py
+-rw-r--r--   0        0        0     3507 2022-06-22 14:20:39.935825 anitya-1.8.0/anitya/forms.py
+-rw-r--r--   0        0        0      152 2020-12-02 09:02:04.977902 anitya-1.8.0/anitya/lib/__init__.py
+-rw-r--r--   0        0        0    15820 2023-04-24 16:04:41.038772 anitya-1.8.0/anitya/lib/backends/__init__.py
+-rw-r--r--   0        0        0     2495 2023-01-26 12:16:19.279657 anitya-1.8.0/anitya/lib/backends/bitbucket.py
+-rw-r--r--   0        0        0     2492 2022-12-14 14:15:40.081732 anitya-1.8.0/anitya/lib/backends/cgit.py
+-rw-r--r--   0        0        0     3059 2022-12-14 14:15:40.082732 anitya-1.8.0/anitya/lib/backends/cpan.py
+-rw-r--r--   0        0        0     7766 2020-12-16 13:18:27.989536 anitya-1.8.0/anitya/lib/backends/cran.py
+-rw-r--r--   0        0        0     8182 2022-06-22 14:20:39.936825 anitya-1.8.0/anitya/lib/backends/crates.py
+-rw-r--r--   0        0        0     2346 2022-12-14 14:15:40.082732 anitya-1.8.0/anitya/lib/backends/custom.py
+-rw-r--r--   0        0        0     2460 2022-12-14 14:15:40.083732 anitya-1.8.0/anitya/lib/backends/debian.py
+-rw-r--r--   0        0        0     2700 2022-12-14 14:15:40.083732 anitya-1.8.0/anitya/lib/backends/drupal6.py
+-rw-r--r--   0        0        0     2700 2022-12-14 14:15:40.084732 anitya-1.8.0/anitya/lib/backends/drupal7.py
+-rw-r--r--   0        0        0     2737 2022-12-14 14:15:40.084732 anitya-1.8.0/anitya/lib/backends/folder.py
+-rw-r--r--   0        0        0     1947 2022-12-14 14:15:40.084732 anitya-1.8.0/anitya/lib/backends/freshmeat.py
+-rw-r--r--   0        0        0     9388 2023-01-26 12:16:19.280657 anitya-1.8.0/anitya/lib/backends/github.py
+-rw-r--r--   0        0        0     4313 2022-12-14 14:15:40.087732 anitya-1.8.0/anitya/lib/backends/gitlab.py
+-rw-r--r--   0        0        0     3089 2022-12-14 14:15:40.087732 anitya-1.8.0/anitya/lib/backends/gnome.py
+-rw-r--r--   0        0        0     2647 2022-12-14 14:15:40.088732 anitya-1.8.0/anitya/lib/backends/gnu.py
+-rw-r--r--   0        0        0     2993 2022-12-14 14:15:40.088732 anitya-1.8.0/anitya/lib/backends/gogs.py
+-rw-r--r--   0        0        0     2237 2022-12-14 14:15:40.089732 anitya-1.8.0/anitya/lib/backends/hackage.py
+-rw-r--r--   0        0        0     1869 2022-12-14 14:15:40.089732 anitya-1.8.0/anitya/lib/backends/launchpad.py
+-rw-r--r--   0        0        0     2631 2023-01-26 12:16:19.280657 anitya-1.8.0/anitya/lib/backends/maven.py
+-rw-r--r--   0        0        0     5116 2020-12-16 13:18:27.990536 anitya-1.8.0/anitya/lib/backends/npmjs.py
+-rw-r--r--   0        0        0     3263 2022-12-14 14:15:40.090732 anitya-1.8.0/anitya/lib/backends/packagist.py
+-rw-r--r--   0        0        0     3121 2022-06-22 14:20:39.938825 anitya-1.8.0/anitya/lib/backends/pagure.py
+-rw-r--r--   0        0        0     4418 2022-06-22 14:20:39.938825 anitya-1.8.0/anitya/lib/backends/pear.py
+-rw-r--r--   0        0        0     4407 2022-06-22 14:20:39.938825 anitya-1.8.0/anitya/lib/backends/pecl.py
+-rw-r--r--   0        0        0     5059 2022-12-14 14:15:40.091732 anitya-1.8.0/anitya/lib/backends/pypi.py
+-rw-r--r--   0        0        0     3465 2022-12-14 14:15:40.091732 anitya-1.8.0/anitya/lib/backends/rubygems.py
+-rw-r--r--   0        0        0     2066 2022-12-14 14:15:40.092732 anitya-1.8.0/anitya/lib/backends/sourceforge.py
+-rw-r--r--   0        0        0     4289 2022-12-14 14:15:40.092732 anitya-1.8.0/anitya/lib/backends/sourceforge_git.py
+-rw-r--r--   0        0        0     3524 2022-12-14 14:15:40.092732 anitya-1.8.0/anitya/lib/backends/sourcehut.py
+-rw-r--r--   0        0        0     2030 2022-12-14 14:15:40.093732 anitya-1.8.0/anitya/lib/backends/stackage.py
+-rw-r--r--   0        0        0     1086 2022-06-22 14:20:39.939825 anitya-1.8.0/anitya/lib/ecosystems/__init__.py
+-rw-r--r--   0        0        0     1072 2022-06-22 14:20:39.939825 anitya-1.8.0/anitya/lib/ecosystems/crates.py
+-rw-r--r--   0        0        0      278 2022-06-22 14:20:39.939825 anitya-1.8.0/anitya/lib/ecosystems/maven.py
+-rw-r--r--   0        0        0      264 2022-06-22 14:20:39.939825 anitya-1.8.0/anitya/lib/ecosystems/npm.py
+-rw-r--r--   0        0        0      266 2022-06-22 14:20:39.939825 anitya-1.8.0/anitya/lib/ecosystems/pypi.py
+-rw-r--r--   0        0        0      282 2022-06-22 14:20:39.939825 anitya-1.8.0/anitya/lib/ecosystems/rubygems.py
+-rw-r--r--   0        0        0     4084 2022-06-22 14:20:39.940825 anitya-1.8.0/anitya/lib/exceptions.py
+-rw-r--r--   0        0        0     3430 2022-06-22 14:20:39.940825 anitya-1.8.0/anitya/lib/plugins.py
+-rw-r--r--   0        0        0    18381 2022-12-14 14:15:40.100732 anitya-1.8.0/anitya/lib/utilities.py
+-rw-r--r--   0        0        0     2186 2020-12-02 09:02:04.979902 anitya-1.8.0/anitya/lib/versions/__init__.py
+-rw-r--r--   0        0        0     7346 2022-06-22 14:20:39.941825 anitya-1.8.0/anitya/lib/versions/base.py
+-rw-r--r--   0        0        0    15319 2022-06-22 14:20:39.941825 anitya-1.8.0/anitya/lib/versions/calver.py
+-rw-r--r--   0        0        0     3084 2023-01-26 12:16:19.280657 anitya-1.8.0/anitya/lib/versions/python.py
+-rw-r--r--   0        0        0     7547 2022-12-14 14:15:40.103732 anitya-1.8.0/anitya/lib/versions/rpm.py
+-rw-r--r--   0        0        0     3766 2020-12-02 09:04:10.567083 anitya-1.8.0/anitya/lib/versions/semver.py
+-rw-r--r--   0        0        0     2822 2023-04-24 16:04:41.039772 anitya-1.8.0/anitya/lib/xml2dict.py
+-rw-r--r--   0        0        0     7366 2022-12-14 14:15:40.104732 anitya-1.8.0/anitya/librariesio_consumer.py
+-rw-r--r--   0        0        0     6251 2022-06-22 14:20:39.943825 anitya-1.8.0/anitya/mail_logging.py
+-rw-r--r--   0        0        0     2946 2023-02-01 10:21:00.258944 anitya-1.8.0/anitya/sar.py
+-rw-r--r--   0        0        0       54 2022-11-14 14:56:56.902921 anitya-1.8.0/anitya/static/css/avatars.css
+-rw-r--r--   0        0        0      888 2022-11-14 14:57:00.636935 anitya-1.8.0/anitya/static/css/cnucnu.css
+-rw-r--r--   0        0        0    24734 2022-11-14 14:57:06.871959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-Bold-webfont.eot
+-rw-r--r--   0        0        0    28113 2022-11-14 14:57:06.871959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-Bold-webfont.svg
+-rw-r--r--   0        0        0    49276 2022-11-14 14:57:06.872959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-Bold-webfont.ttf
+-rw-r--r--   0        0        0    16708 2022-11-14 14:57:06.872959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-Bold-webfont.woff
+-rw-r--r--   0        0        0    27450 2022-11-14 14:57:06.872959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.eot
+-rw-r--r--   0        0        0    29130 2022-11-14 14:57:06.873959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.svg
+-rw-r--r--   0        0        0    52200 2022-11-14 14:57:06.873959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.ttf
+-rw-r--r--   0        0        0    17988 2022-11-14 14:57:06.873959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.woff
+-rw-r--r--   0        0        0    27610 2022-11-14 14:57:06.873959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.eot
+-rw-r--r--   0        0        0    29402 2022-11-14 14:57:06.874959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.svg
+-rw-r--r--   0        0        0    50068 2022-11-14 14:57:06.874959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.ttf
+-rw-r--r--   0        0        0    17980 2022-11-14 14:57:06.874959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.woff
+-rw-r--r--   0        0        0    24350 2022-11-14 14:57:06.874959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-Regular-webfont.eot
+-rw-r--r--   0        0        0    28095 2022-11-14 14:57:06.874959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-Regular-webfont.svg
+-rw-r--r--   0        0        0    47504 2022-11-14 14:57:06.875959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-Regular-webfont.ttf
+-rw-r--r--   0        0        0    16400 2022-11-14 14:57:06.875959 anitya-1.8.0/anitya/static/css/fonts/Cantarell-Regular-webfont.woff
+-rw-r--r--   0        0        0    94588 2022-11-14 14:57:06.876959 anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.eot
+-rw-r--r--   0        0        0   171329 2022-11-14 14:57:06.876959 anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.svg
+-rw-r--r--   0        0        0   170608 2022-11-14 14:57:06.878960 anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.ttf
+-rw-r--r--   0        0        0    56608 2022-11-14 14:57:06.878960 anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.woff
+-rw-r--r--   0        0        0    91164 2022-11-14 14:57:06.878960 anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.eot
+-rw-r--r--   0        0        0   169419 2022-11-14 14:57:06.879959 anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.svg
+-rw-r--r--   0        0        0   170388 2022-11-14 14:57:06.880959 anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.ttf
+-rw-r--r--   0        0        0    54684 2022-11-14 14:57:06.880959 anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.woff
+-rw-r--r--   0        0        0    95020 2022-11-14 14:57:06.881960 anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.eot
+-rw-r--r--   0        0        0   167898 2022-11-14 14:57:06.882959 anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.svg
+-rw-r--r--   0        0        0   170308 2022-11-14 14:57:06.883959 anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.ttf
+-rw-r--r--   0        0        0    56100 2022-11-14 14:57:06.883959 anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.woff
+-rw-r--r--   0        0        0      279 2022-11-14 14:57:22.414019 anitya-1.8.0/anitya/static/css/footer.css
+-rw-r--r--   0        0        0      212 2022-11-14 14:57:16.686997 anitya-1.8.0/anitya/static/css/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-r--r--   0        0        0      220 2022-11-14 14:57:16.686997 anitya-1.8.0/anitya/static/css/images/ui-bg_flat_0_eeeeee_40x100.png
+-rw-r--r--   0        0        0      208 2022-11-14 14:57:16.686997 anitya-1.8.0/anitya/static/css/images/ui-bg_flat_55_ffffff_40x100.png
+-rw-r--r--   0        0        0      208 2022-11-14 14:57:16.686997 anitya-1.8.0/anitya/static/css/images/ui-bg_flat_75_ffffff_40x100.png
+-rw-r--r--   0        0        0      207 2022-11-14 14:57:16.686997 anitya-1.8.0/anitya/static/css/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0        0        0      277 2022-11-14 14:57:16.686997 anitya-1.8.0/anitya/static/css/images/ui-bg_highlight-soft_100_f6f6f6_1x100.png
+-rw-r--r--   0        0        0      338 2022-11-14 14:57:16.687997 anitya-1.8.0/anitya/static/css/images/ui-bg_highlight-soft_25_0073ea_1x100.png
+-rw-r--r--   0        0        0      280 2022-11-14 14:57:16.687997 anitya-1.8.0/anitya/static/css/images/ui-bg_highlight-soft_50_dddddd_1x100.png
+-rw-r--r--   0        0        0     4549 2022-11-14 14:57:16.687997 anitya-1.8.0/anitya/static/css/images/ui-icons_0073ea_256x240.png
+-rw-r--r--   0        0        0     6992 2022-11-14 14:57:16.687997 anitya-1.8.0/anitya/static/css/images/ui-icons_454545_256x240.png
+-rw-r--r--   0        0        0     6988 2022-11-14 14:57:16.688997 anitya-1.8.0/anitya/static/css/images/ui-icons_666666_256x240.png
+-rw-r--r--   0        0        0     4549 2022-11-14 14:57:16.688997 anitya-1.8.0/anitya/static/css/images/ui-icons_ff0084_256x240.png
+-rw-r--r--   0        0        0     6299 2022-11-14 14:57:16.688997 anitya-1.8.0/anitya/static/css/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0      125 2022-11-14 14:57:29.052045 anitya-1.8.0/anitya/static/css/navbar.css
+-rw-r--r--   0        0        0     2519 2022-11-14 14:57:32.802060 anitya-1.8.0/anitya/static/css/text.css
+-rw-r--r--   0        0        0    33392 2021-01-15 12:47:19.805568 anitya-1.8.0/anitya/static/docs/_images/database.png
+-rw-r--r--   0        0        0    13224 2021-01-15 12:47:19.813568 anitya-1.8.0/anitya/static/docs/_modules/anitya/db/events.html
+-rw-r--r--   0        0        0    20589 2021-01-15 12:47:19.814568 anitya-1.8.0/anitya/static/docs/_modules/anitya/db/meta.html
+-rw-r--r--   0        0        0   150267 2021-01-15 12:47:19.816568 anitya-1.8.0/anitya/static/docs/_modules/anitya/db/models.html
+-rw-r--r--   0        0        0    52067 2021-01-15 12:47:19.818568 anitya-1.8.0/anitya/static/docs/_modules/anitya/lib/backends.html
+-rw-r--r--   0        0        0     6469 2021-01-15 12:47:19.819568 anitya-1.8.0/anitya/static/docs/_modules/anitya/lib/ecosystems.html
+-rw-r--r--   0        0        0    18072 2021-01-15 12:47:19.821568 anitya-1.8.0/anitya/static/docs/_modules/anitya/lib/exceptions.html
+-rw-r--r--   0        0        0    15350 2021-01-15 12:47:19.822568 anitya-1.8.0/anitya/static/docs/_modules/anitya/lib/plugins.html
+-rw-r--r--   0        0        0    26768 2021-01-15 12:47:19.824568 anitya-1.8.0/anitya/static/docs/_modules/anitya/lib/versions/base.html
+-rw-r--r--   0        0        0     5081 2021-01-15 12:47:19.841568 anitya-1.8.0/anitya/static/docs/_modules/index.html
+-rw-r--r--   0        0        0    76032 2021-01-15 12:47:19.827568 anitya-1.8.0/anitya/static/docs/_modules/sqlalchemy/ext/declarative/api.html
+-rw-r--r--   0        0        0   245360 2021-01-15 12:47:19.830568 anitya-1.8.0/anitya/static/docs/_modules/sqlalchemy/orm/attributes.html
+-rw-r--r--   0        0        0    23324 2021-01-15 12:47:19.832568 anitya-1.8.0/anitya/static/docs/_modules/sqlalchemy/orm/scoping.html
+-rw-r--r--   0        0        0   500489 2021-01-15 12:47:19.837568 anitya-1.8.0/anitya/static/docs/_modules/sqlalchemy/sql/schema.html
+-rw-r--r--   0        0        0   296008 2021-01-15 12:47:19.840568 anitya-1.8.0/anitya/static/docs/_modules/sqlalchemy/sql/sqltypes.html
+-rw-r--r--   0        0        0     5095 2021-01-15 12:47:19.850568 anitya-1.8.0/anitya/static/docs/_sources/admin-guide.rst.txt
+-rw-r--r--   0        0        0     8467 2021-01-15 12:47:19.851568 anitya-1.8.0/anitya/static/docs/_sources/admin-user-guide.rst.txt
+-rw-r--r--   0        0        0     1756 2021-01-15 12:47:19.852568 anitya-1.8.0/anitya/static/docs/_sources/api.rst.txt
+-rw-r--r--   0        0        0     9534 2021-01-15 12:47:19.853568 anitya-1.8.0/anitya/static/docs/_sources/contributing.rst.txt
+-rw-r--r--   0        0        0      314 2021-01-15 12:47:19.854568 anitya-1.8.0/anitya/static/docs/_sources/database.rst.txt
+-rw-r--r--   0        0        0      306 2021-01-15 12:47:19.856568 anitya-1.8.0/anitya/static/docs/_sources/docblocks/anitya.db.models.rst.txt
+-rw-r--r--   0        0        0      510 2021-01-15 12:47:19.857568 anitya-1.8.0/anitya/static/docs/_sources/glossary.rst.txt
+-rw-r--r--   0        0        0     1279 2021-01-15 12:47:19.858568 anitya-1.8.0/anitya/static/docs/_sources/index.rst.txt
+-rw-r--r--   0        0        0     2624 2021-01-15 12:47:19.859568 anitya-1.8.0/anitya/static/docs/_sources/integrating-with-anitya.rst.txt
+-rw-r--r--   0        0        0     2229 2020-12-02 12:47:56.984892 anitya-1.8.0/anitya/static/docs/_sources/release-monitoring-admin-guide.rst.txt
+-rw-r--r--   0        0        0    23367 2021-01-15 12:47:19.860568 anitya-1.8.0/anitya/static/docs/_sources/release-notes.rst.txt
+-rw-r--r--   0        0        0    19248 2021-01-15 12:47:19.861568 anitya-1.8.0/anitya/static/docs/_sources/user-guide.rst.txt
+-rw-r--r--   0        0        0    11187 2021-01-15 12:47:19.881568 anitya-1.8.0/anitya/static/docs/_static/alabaster.css
+-rw-r--r--   0        0        0    12171 2021-01-15 12:47:19.864568 anitya-1.8.0/anitya/static/docs/_static/basic.css
+-rw-r--r--   0        0        0       42 2021-01-15 12:47:19.880568 anitya-1.8.0/anitya/static/docs/_static/custom.css
+-rw-r--r--   0        0        0     9270 2021-01-15 12:47:19.874568 anitya-1.8.0/anitya/static/docs/_static/doctools.js
+-rw-r--r--   0        0        0      307 2021-01-15 12:47:19.873568 anitya-1.8.0/anitya/static/docs/_static/documentation_options.js
+-rw-r--r--   0        0        0      286 2021-01-15 12:47:19.866568 anitya-1.8.0/anitya/static/docs/_static/file.png
+-rw-r--r--   0        0        0   280364 2021-01-15 12:47:19.884568 anitya-1.8.0/anitya/static/docs/_static/jquery-3.4.1.js
+-rw-r--r--   0        0        0   287630 2021-01-15 12:47:19.871568 anitya-1.8.0/anitya/static/docs/_static/jquery-3.5.1.js
+-rw-r--r--   0        0        0    88145 2021-01-15 12:47:19.868568 anitya-1.8.0/anitya/static/docs/_static/jquery.js
+-rw-r--r--   0        0        0    10847 2021-01-15 12:47:19.879568 anitya-1.8.0/anitya/static/docs/_static/language_data.js
+-rw-r--r--   0        0        0       90 2021-01-15 12:47:19.878568 anitya-1.8.0/anitya/static/docs/_static/minus.png
+-rw-r--r--   0        0        0       90 2021-01-15 12:47:19.877568 anitya-1.8.0/anitya/static/docs/_static/plus.png
+-rw-r--r--   0        0        0     4395 2021-01-15 12:47:19.863568 anitya-1.8.0/anitya/static/docs/_static/pygments.css
+-rw-r--r--   0        0        0    15987 2021-01-15 12:47:19.875568 anitya-1.8.0/anitya/static/docs/_static/searchtools.js
+-rw-r--r--   0        0        0    35168 2021-01-15 12:47:19.876568 anitya-1.8.0/anitya/static/docs/_static/underscore-1.3.1.js
+-rw-r--r--   0        0        0    12140 2021-01-15 12:47:19.865568 anitya-1.8.0/anitya/static/docs/_static/underscore.js
+-rw-r--r--   0        0        0    17984 2021-01-15 12:47:19.782568 anitya-1.8.0/anitya/static/docs/admin-guide.html
+-rw-r--r--   0        0        0    19172 2021-01-15 12:47:19.785568 anitya-1.8.0/anitya/static/docs/admin-user-guide.html
+-rw-r--r--   0        0        0   186318 2021-01-15 12:47:19.790568 anitya-1.8.0/anitya/static/docs/api.html
+-rw-r--r--   0        0        0    24463 2021-01-15 12:47:19.792568 anitya-1.8.0/anitya/static/docs/contributing.html
+-rw-r--r--   0        0        0     5793 2021-01-15 12:47:19.794568 anitya-1.8.0/anitya/static/docs/database.html
+-rw-r--r--   0        0        0     6755 2021-01-15 12:47:19.797568 anitya-1.8.0/anitya/static/docs/docblocks/anitya.db.models.html
+-rw-r--r--   0        0        0    21157 2021-01-15 12:47:19.799568 anitya-1.8.0/anitya/static/docs/genindex.html
+-rw-r--r--   0        0        0     5045 2021-01-15 12:47:19.801568 anitya-1.8.0/anitya/static/docs/glossary.html
+-rw-r--r--   0        0        0     9045 2021-01-15 12:47:19.803568 anitya-1.8.0/anitya/static/docs/http-routingtable.html
+-rw-r--r--   0        0        0    13545 2021-01-15 12:47:19.807568 anitya-1.8.0/anitya/static/docs/index.html
+-rw-r--r--   0        0        0     8658 2021-01-15 12:47:19.809568 anitya-1.8.0/anitya/static/docs/integrating-with-anitya.html
+-rw-r--r--   0        0        0     1672 2021-01-15 12:47:19.842568 anitya-1.8.0/anitya/static/docs/objects.inv
+-rw-r--r--   0        0        0     6028 2021-01-15 12:47:19.844568 anitya-1.8.0/anitya/static/docs/py-modindex.html
+-rw-r--r--   0        0        0     8309 2020-12-02 12:47:56.964892 anitya-1.8.0/anitya/static/docs/release-monitoring-admin-guide.html
+-rw-r--r--   0        0        0    48756 2021-01-15 12:47:19.846568 anitya-1.8.0/anitya/static/docs/release-notes.html
+-rw-r--r--   0        0        0     4548 2021-01-15 12:47:19.847568 anitya-1.8.0/anitya/static/docs/search.html
+-rw-r--r--   0        0        0    24161 2021-01-15 12:47:19.848568 anitya-1.8.0/anitya/static/docs/searchindex.js
+-rw-r--r--   0        0        0    38361 2021-01-15 12:47:19.885568 anitya-1.8.0/anitya/static/docs/user-guide.html
+-rw-r--r--   0        0        0     4683 2020-12-02 09:02:04.991902 anitya-1.8.0/anitya/static/google_logo.png
+-rw-r--r--   0        0        0     5430 2022-11-14 16:27:56.526971 anitya-1.8.0/anitya/static/ico/favicon.ico
+-rw-r--r--   0        0        0     4077 2022-11-14 14:58:19.913241 anitya-1.8.0/anitya/static/img/spinner.gif
+-rw-r--r--   0        0        0     1957 2023-04-26 13:29:52.891981 anitya-1.8.0/anitya/static/node_modules/.package-lock.json
+-rw-r--r--   0        0        0     1082 2022-11-14 15:08:03.408809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/LICENSE.md
+-rw-r--r--   0        0        0    13561 2022-11-14 15:08:03.409809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/README.md
+-rw-r--r--   0        0        0     2037 2022-11-14 15:08:03.426809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/enums.js
+-rw-r--r--   0        0        0       45 2022-11-14 15:08:03.426809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/enums.js.flow
+-rw-r--r--   0        0        0     4234 2022-11-14 15:08:03.427809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/enums.js.map
+-rw-r--r--   0        0        0    36698 2022-11-14 15:08:03.428809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-base.js
+-rw-r--r--   0        0        0       51 2022-11-14 15:08:03.429809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-base.js.flow
+-rw-r--r--   0        0        0    87394 2022-11-14 15:08:03.433809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-base.js.map
+-rw-r--r--   0        0        0    47193 2022-11-14 15:08:03.436809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js
+-rw-r--r--   0        0        0       51 2022-11-14 15:08:03.437809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js.flow
+-rw-r--r--   0        0        0   110974 2022-11-14 15:08:03.441809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js.map
+-rw-r--r--   0        0        0    67554 2022-11-14 15:08:03.449809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper.js
+-rw-r--r--   0        0        0       46 2022-11-14 15:08:03.450809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper.js.flow
+-rw-r--r--   0        0        0   158154 2022-11-14 15:08:03.455809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper.js.map
+-rw-r--r--   0        0        0    10007 2022-11-14 15:08:03.457809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/createPopper.js
+-rw-r--r--   0        0        0      677 2022-11-14 15:08:03.578809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/contains.js
+-rw-r--r--   0        0        0     1371 2022-11-14 15:08:03.579810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getBoundingClientRect.js
+-rw-r--r--   0        0        0     3400 2022-11-14 15:08:03.579810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getClippingRect.js
+-rw-r--r--   0        0        0     2072 2022-11-14 15:08:03.579810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getCompositeRect.js
+-rw-r--r--   0        0        0      148 2022-11-14 15:08:03.579810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getComputedStyle.js
+-rw-r--r--   0        0        0      311 2022-11-14 15:08:03.580809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getDocumentElement.js
+-rw-r--r--   0        0        0     1227 2022-11-14 15:08:03.580809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getDocumentRect.js
+-rw-r--r--   0        0        0      142 2022-11-14 15:08:03.580809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getHTMLElementScroll.js
+-rw-r--r--   0        0        0      767 2022-11-14 15:08:03.581809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getLayoutRect.js
+-rw-r--r--   0        0        0      114 2022-11-14 15:08:03.581809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getNodeName.js
+-rw-r--r--   0        0        0      396 2022-11-14 15:08:03.581809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getNodeScroll.js
+-rw-r--r--   0        0        0     2613 2022-11-14 15:08:03.582810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getOffsetParent.js
+-rw-r--r--   0        0        0      759 2022-11-14 15:08:03.582810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getParentNode.js
+-rw-r--r--   0        0        0      546 2022-11-14 15:08:03.582810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getScrollParent.js
+-rw-r--r--   0        0        0      881 2022-11-14 15:08:03.583809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getViewportRect.js
+-rw-r--r--   0        0        0      273 2022-11-14 15:08:03.583809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindow.js
+-rw-r--r--   0        0        0      258 2022-11-14 15:08:03.583809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindowScroll.js
+-rw-r--r--   0        0        0      721 2022-11-14 15:08:03.583809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindowScrollBarX.js
+-rw-r--r--   0        0        0      621 2022-11-14 15:08:03.584809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/instanceOf.js
+-rw-r--r--   0        0        0      159 2022-11-14 15:08:03.584809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/isLayoutViewport.js
+-rw-r--r--   0        0        0      440 2022-11-14 15:08:03.584809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/isScrollParent.js
+-rw-r--r--   0        0        0      162 2022-11-14 15:08:03.585809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/isTableElement.js
+-rw-r--r--   0        0        0     1177 2022-11-14 15:08:03.585809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/listScrollParents.js
+-rw-r--r--   0        0        0     1335 2022-11-14 15:08:03.457809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/enums.js
+-rw-r--r--   0        0        0      443 2022-11-14 15:08:03.458809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/index.js
+-rw-r--r--   0        0        0     2527 2022-11-14 15:08:03.586809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/applyStyles.js
+-rw-r--r--   0        0        0     3878 2022-11-14 15:08:03.586809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/arrow.js
+-rw-r--r--   0        0        0     6566 2022-11-14 15:08:03.587809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/computeStyles.js
+-rw-r--r--   0        0        0     1330 2022-11-14 15:08:03.587809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/eventListeners.js
+-rw-r--r--   0        0        0     4910 2022-11-14 15:08:03.587809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/flip.js
+-rw-r--r--   0        0        0     1954 2022-11-14 15:08:03.588809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/hide.js
+-rw-r--r--   0        0        0      502 2022-11-14 15:08:03.588809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/index.js
+-rw-r--r--   0        0        0     1613 2022-11-14 15:08:03.589810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/offset.js
+-rw-r--r--   0        0        0      706 2022-11-14 15:08:03.589810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/popperOffsets.js
+-rw-r--r--   0        0        0     6585 2022-11-14 15:08:03.589810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/preventOverflow.js
+-rw-r--r--   0        0        0      193 2022-11-14 15:08:03.458809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/popper-base.js
+-rw-r--r--   0        0        0      603 2022-11-14 15:08:03.459809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/popper-lite.js
+-rw-r--r--   0        0        0     1090 2022-11-14 15:08:03.459809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/popper.js
+-rw-r--r--   0        0        0        0 2022-11-14 15:08:03.459809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/types.js
+-rw-r--r--   0        0        0     1991 2022-11-14 15:08:03.590809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/computeAutoPlacement.js
+-rw-r--r--   0        0        0     1738 2022-11-14 15:08:03.591809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/computeOffsets.js
+-rw-r--r--   0        0        0      302 2022-11-14 15:08:03.591809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/debounce.js
+-rw-r--r--   0        0        0     3528 2022-11-14 15:08:03.591809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/detectOverflow.js
+-rw-r--r--   0        0        0      159 2022-11-14 15:08:03.592810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/expandToHashMap.js
+-rw-r--r--   0        0        0      286 2022-11-14 15:08:03.592810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/format.js
+-rw-r--r--   0        0        0       79 2022-11-14 15:08:03.592810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getAltAxis.js
+-rw-r--r--   0        0        0       89 2022-11-14 15:08:03.592810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getAltLen.js
+-rw-r--r--   0        0        0      125 2022-11-14 15:08:03.593809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getBasePlacement.js
+-rw-r--r--   0        0        0      117 2022-11-14 15:08:03.593809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getFreshSideObject.js
+-rw-r--r--   0        0        0      127 2022-11-14 15:08:03.593809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getMainAxisFromPlacement.js
+-rw-r--r--   0        0        0      248 2022-11-14 15:08:03.594809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getOppositePlacement.js
+-rw-r--r--   0        0        0      209 2022-11-14 15:08:03.594809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getOppositeVariationPlacement.js
+-rw-r--r--   0        0        0       85 2022-11-14 15:08:03.594809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/getVariation.js
+-rw-r--r--   0        0        0       84 2022-11-14 15:08:03.595810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/math.js
+-rw-r--r--   0        0        0      524 2022-11-14 15:08:03.595810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/mergeByName.js
+-rw-r--r--   0        0        0      184 2022-11-14 15:08:03.595810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/mergePaddingObject.js
+-rw-r--r--   0        0        0     1240 2022-11-14 15:08:03.596809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/orderModifiers.js
+-rw-r--r--   0        0        0      191 2022-11-14 15:08:03.596809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/rectToClientRect.js
+-rw-r--r--   0        0        0      252 2022-11-14 15:08:03.597809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/uniqueBy.js
+-rw-r--r--   0        0        0      269 2022-11-14 15:08:03.597809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/userAgent.js
+-rw-r--r--   0        0        0     3261 2022-11-14 15:08:03.597809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/validateModifiers.js
+-rw-r--r--   0        0        0      262 2022-11-14 15:08:03.597809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/within.js
+-rw-r--r--   0        0        0     2479 2022-11-14 15:08:03.461809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.js
+-rw-r--r--   0        0        0     4240 2022-11-14 15:08:03.461809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.js.map
+-rw-r--r--   0        0        0     1108 2022-11-14 15:08:03.462809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.min.js
+-rw-r--r--   0        0        0       45 2022-11-14 15:08:03.463809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.min.js.flow
+-rw-r--r--   0        0        0     3736 2022-11-14 15:08:03.464809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.min.js.map
+-rw-r--r--   0        0        0    38668 2022-11-14 15:08:03.465809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.js
+-rw-r--r--   0        0        0    87396 2022-11-14 15:08:03.467809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.js.map
+-rw-r--r--   0        0        0     9755 2022-11-14 15:08:03.467809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js
+-rw-r--r--   0        0        0       51 2022-11-14 15:08:03.467809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js.flow
+-rw-r--r--   0        0        0    60851 2022-11-14 15:08:03.468809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js.map
+-rw-r--r--   0        0        0    49678 2022-11-14 15:08:03.471809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.js
+-rw-r--r--   0        0        0   110975 2022-11-14 15:08:03.474809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.js.map
+-rw-r--r--   0        0        0    13539 2022-11-14 15:08:03.475809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js
+-rw-r--r--   0        0        0       51 2022-11-14 15:08:03.476809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js.flow
+-rw-r--r--   0        0        0    78475 2022-11-14 15:08:03.477809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js.map
+-rw-r--r--   0        0        0    70878 2022-11-14 15:08:03.479809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.js
+-rw-r--r--   0        0        0   158154 2022-11-14 15:08:03.482809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.js.map
+-rw-r--r--   0        0        0    20095 2022-11-14 15:08:03.484809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.min.js
+-rw-r--r--   0        0        0       46 2022-11-14 15:08:03.485809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.min.js.flow
+-rw-r--r--   0        0        0   114779 2022-11-14 15:08:03.487809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.min.js.map
+-rw-r--r--   0        0        0       23 2022-11-14 15:08:03.411809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/index.d.ts
+-rw-r--r--   0        0        0      750 2022-11-14 15:08:03.412809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/createPopper.d.ts
+-rw-r--r--   0        0        0    10135 2022-11-14 15:08:03.413809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/createPopper.js
+-rw-r--r--   0        0        0     9415 2022-11-14 15:08:03.414809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/createPopper.js.flow
+-rw-r--r--   0        0        0       76 2022-11-14 15:08:03.488809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/contains.d.ts
+-rw-r--r--   0        0        0      677 2022-11-14 15:08:03.489809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/contains.js
+-rw-r--r--   0        0        0      697 2022-11-14 15:08:03.490809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/contains.js.flow
+-rw-r--r--   0        0        0      217 2022-11-14 15:08:03.490809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.d.ts
+-rw-r--r--   0        0        0     1371 2022-11-14 15:08:03.491809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.js
+-rw-r--r--   0        0        0     1485 2022-11-14 15:08:03.491809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.js.flow
+-rw-r--r--   0        0        0      283 2022-11-14 15:08:03.492809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.d.ts
+-rw-r--r--   0        0        0     3400 2022-11-14 15:08:03.492809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.js
+-rw-r--r--   0        0        0     3782 2022-11-14 15:08:03.493809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.js.flow
+-rw-r--r--   0        0        0      212 2022-11-14 15:08:03.493809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.d.ts
+-rw-r--r--   0        0        0     2072 2022-11-14 15:08:03.494809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.js
+-rw-r--r--   0        0        0     2192 2022-11-14 15:08:03.494809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.js.flow
+-rw-r--r--   0        0        0       81 2022-11-14 15:08:03.496809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getComputedStyle.d.ts
+-rw-r--r--   0        0        0      148 2022-11-14 15:08:03.496809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getComputedStyle.js
+-rw-r--r--   0        0        0      190 2022-11-14 15:08:03.497809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getComputedStyle.js.flow
+-rw-r--r--   0        0        0      124 2022-11-14 15:08:03.497809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentElement.d.ts
+-rw-r--r--   0        0        0      311 2022-11-14 15:08:03.498809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentElement.js
+-rw-r--r--   0        0        0      420 2022-11-14 15:08:03.498809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentElement.js.flow
+-rw-r--r--   0        0        0      107 2022-11-14 15:08:03.499809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.d.ts
+-rw-r--r--   0        0        0     1227 2022-11-14 15:08:03.501809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.js
+-rw-r--r--   0        0        0     1198 2022-11-14 15:08:03.502809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.js.flow
+-rw-r--r--   0        0        0      120 2022-11-14 15:08:03.502809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getHTMLElementScroll.d.ts
+-rw-r--r--   0        0        0      142 2022-11-14 15:08:03.503809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getHTMLElementScroll.js
+-rw-r--r--   0        0        0      167 2022-11-14 15:08:03.504809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getHTMLElementScroll.js.flow
+-rw-r--r--   0        0        0      105 2022-11-14 15:08:03.505809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.d.ts
+-rw-r--r--   0        0        0      767 2022-11-14 15:08:03.509809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.js
+-rw-r--r--   0        0        0      821 2022-11-14 15:08:03.509809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.js.flow
+-rw-r--r--   0        0        0      149 2022-11-14 15:08:03.510809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeName.d.ts
+-rw-r--r--   0        0        0      114 2022-11-14 15:08:03.511809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeName.js
+-rw-r--r--   0        0        0      190 2022-11-14 15:08:03.511809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeName.js.flow
+-rw-r--r--   0        0        0      146 2022-11-14 15:08:03.512809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeScroll.d.ts
+-rw-r--r--   0        0        0      396 2022-11-14 15:08:03.512809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeScroll.js
+-rw-r--r--   0        0        0      450 2022-11-14 15:08:03.513809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getNodeScroll.js.flow
+-rw-r--r--   0        0        0       64 2022-11-14 15:08:03.513809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.d.ts
+-rw-r--r--   0        0        0     2613 2022-11-14 15:08:03.514809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.js
+-rw-r--r--   0        0        0     2767 2022-11-14 15:08:03.514809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.js.flow
+-rw-r--r--   0        0        0       73 2022-11-14 15:08:03.515809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.d.ts
+-rw-r--r--   0        0        0      759 2022-11-14 15:08:03.515809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.js
+-rw-r--r--   0        0        0      789 2022-11-14 15:08:03.515809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.js.flow
+-rw-r--r--   0        0        0       66 2022-11-14 15:08:03.516809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.d.ts
+-rw-r--r--   0        0        0      546 2022-11-14 15:08:03.516809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.js
+-rw-r--r--   0        0        0      564 2022-11-14 15:08:03.517809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.js.flow
+-rw-r--r--   0        0        0      217 2022-11-14 15:08:03.517809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.d.ts
+-rw-r--r--   0        0        0      881 2022-11-14 15:08:03.518809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.js
+-rw-r--r--   0        0        0      964 2022-11-14 15:08:03.518809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.js.flow
+-rw-r--r--   0        0        0       51 2022-11-14 15:08:03.519809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindow.d.ts
+-rw-r--r--   0        0        0      273 2022-11-14 15:08:03.519809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindow.js
+-rw-r--r--   0        0        0      383 2022-11-14 15:08:03.520809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindow.js.flow
+-rw-r--r--   0        0        0      148 2022-11-14 15:08:03.520809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScroll.d.ts
+-rw-r--r--   0        0        0      258 2022-11-14 15:08:03.521809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScroll.js
+-rw-r--r--   0        0        0      306 2022-11-14 15:08:03.521809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScroll.js.flow
+-rw-r--r--   0        0        0       71 2022-11-14 15:08:03.521809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.d.ts
+-rw-r--r--   0        0        0      721 2022-11-14 15:08:03.522809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.js
+-rw-r--r--   0        0        0      754 2022-11-14 15:08:03.522809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.js.flow
+-rw-r--r--   0        0        0      214 2022-11-14 15:08:03.523809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.d.ts
+-rw-r--r--   0        0        0      621 2022-11-14 15:08:03.523809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.js
+-rw-r--r--   0        0        0      902 2022-11-14 15:08:03.524809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.js.flow
+-rw-r--r--   0        0        0       53 2022-11-14 15:08:03.525809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isLayoutViewport.d.ts
+-rw-r--r--   0        0        0      159 2022-11-14 15:08:03.525809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isLayoutViewport.js
+-rw-r--r--   0        0        0      167 2022-11-14 15:08:03.525809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isLayoutViewport.js.flow
+-rw-r--r--   0        0        0       71 2022-11-14 15:08:03.526809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isScrollParent.d.ts
+-rw-r--r--   0        0        0      440 2022-11-14 15:08:03.526809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isScrollParent.js
+-rw-r--r--   0        0        0      349 2022-11-14 15:08:03.527809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isScrollParent.js.flow
+-rw-r--r--   0        0        0       67 2022-11-14 15:08:03.527809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isTableElement.d.ts
+-rw-r--r--   0        0        0      162 2022-11-14 15:08:03.527809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isTableElement.js
+-rw-r--r--   0        0        0      188 2022-11-14 15:08:03.528809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/isTableElement.js.flow
+-rw-r--r--   0        0        0      188 2022-11-14 15:08:03.528809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.d.ts
+-rw-r--r--   0        0        0     1177 2022-11-14 15:08:03.529809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.js
+-rw-r--r--   0        0        0     1227 2022-11-14 15:08:03.529809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.js.flow
+-rw-r--r--   0        0        0     2008 2022-11-14 15:08:03.414809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/enums.d.ts
+-rw-r--r--   0        0        0     1335 2022-11-14 15:08:03.415809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/enums.js
+-rw-r--r--   0        0        0     2763 2022-11-14 15:08:03.416809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/enums.js.flow
+-rw-r--r--   0        0        0      286 2022-11-14 15:08:03.417809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/index.d.ts
+-rw-r--r--   0        0        0      443 2022-11-14 15:08:03.417809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/index.js
+-rw-r--r--   0        0        0      462 2022-11-14 15:08:03.418809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/index.js.flow
+-rw-r--r--   0        0        0      183 2022-11-14 15:08:03.530809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.d.ts
+-rw-r--r--   0        0        0     2527 2022-11-14 15:08:03.530809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.js
+-rw-r--r--   0        0        0     2723 2022-11-14 15:08:03.531809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.js.flow
+-rw-r--r--   0        0        0      435 2022-11-14 15:08:03.532809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/arrow.d.ts
+-rw-r--r--   0        0        0     3942 2022-11-14 15:08:03.534809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/arrow.js
+-rw-r--r--   0        0        0     4208 2022-11-14 15:08:03.536809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/arrow.js.flow
+-rw-r--r--   0        0        0     1208 2022-11-14 15:08:03.537809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.d.ts
+-rw-r--r--   0        0        0     6598 2022-11-14 15:08:03.537809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.js
+-rw-r--r--   0        0        0     6945 2022-11-14 15:08:03.538809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.js.flow
+-rw-r--r--   0        0        0      274 2022-11-14 15:08:03.539809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.d.ts
+-rw-r--r--   0        0        0     1330 2022-11-14 15:08:03.540809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.js
+-rw-r--r--   0        0        0     1341 2022-11-14 15:08:03.540809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.js.flow
+-rw-r--r--   0        0        0      543 2022-11-14 15:08:03.540809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.d.ts
+-rw-r--r--   0        0        0     4910 2022-11-14 15:08:03.541809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.js
+-rw-r--r--   0        0        0     4893 2022-11-14 15:08:03.542809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.js.flow
+-rw-r--r--   0        0        0      162 2022-11-14 15:08:03.542809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/hide.d.ts
+-rw-r--r--   0        0        0     1954 2022-11-14 15:08:03.543809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/hide.js
+-rw-r--r--   0        0        0     2034 2022-11-14 15:08:03.543809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/hide.js.flow
+-rw-r--r--   0        0        0      476 2022-11-14 15:08:03.544809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/index.d.ts
+-rw-r--r--   0        0        0      502 2022-11-14 15:08:03.544809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/index.js
+-rw-r--r--   0        0        0      485 2022-11-14 15:08:03.544809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/index.js.flow
+-rw-r--r--   0        0        0      703 2022-11-14 15:08:03.545809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.d.ts
+-rw-r--r--   0        0        0     1613 2022-11-14 15:08:03.545809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.js
+-rw-r--r--   0        0        0     1933 2022-11-14 15:08:03.546809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.js.flow
+-rw-r--r--   0        0        0      189 2022-11-14 15:08:03.547809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.d.ts
+-rw-r--r--   0        0        0      706 2022-11-14 15:08:03.547809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.js
+-rw-r--r--   0        0        0      855 2022-11-14 15:08:03.547809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.js.flow
+-rw-r--r--   0        0        0      862 2022-11-14 15:08:03.548809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.d.ts
+-rw-r--r--   0        0        0     6585 2022-11-14 15:08:03.548809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.js
+-rw-r--r--   0        0        0     7439 2022-11-14 15:08:03.548809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.js.flow
+-rw-r--r--   0        0        0      163 2022-11-14 15:08:03.419809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper-base.d.ts
+-rw-r--r--   0        0        0      193 2022-11-14 15:08:03.419809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper-base.js
+-rw-r--r--   0        0        0      232 2022-11-14 15:08:03.420809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper-base.js.flow
+-rw-r--r--   0        0        0      705 2022-11-14 15:08:03.420809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper-lite.d.ts
+-rw-r--r--   0        0        0      603 2022-11-14 15:08:03.420809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper-lite.js
+-rw-r--r--   0        0        0      614 2022-11-14 15:08:03.421809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper-lite.js.flow
+-rw-r--r--   0        0        0     1038 2022-11-14 15:08:03.421809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper.d.ts
+-rw-r--r--   0        0        0     1090 2022-11-14 15:08:03.422809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper.js
+-rw-r--r--   0        0        0     1082 2022-11-14 15:08:03.422809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper.js.flow
+-rw-r--r--   0        0        0     5224 2022-11-14 15:08:03.422809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/types.d.ts
+-rw-r--r--   0        0        0        0 2022-11-14 15:08:03.422809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/types.js
+-rw-r--r--   0        0        0     4933 2022-11-14 15:08:03.424809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/types.js.flow
+-rw-r--r--   0        0        0      466 2022-11-14 15:08:03.549809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.d.ts
+-rw-r--r--   0        0        0     2023 2022-11-14 15:08:03.549809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.js
+-rw-r--r--   0        0        0     2178 2022-11-14 15:08:03.550809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.js.flow
+-rw-r--r--   0        0        0      353 2022-11-14 15:08:03.550809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeOffsets.d.ts
+-rw-r--r--   0        0        0     1738 2022-11-14 15:08:03.550809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeOffsets.js
+-rw-r--r--   0        0        0     1971 2022-11-14 15:08:03.550809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeOffsets.js.flow
+-rw-r--r--   0        0        0       89 2022-11-14 15:08:03.551809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/debounce.d.ts
+-rw-r--r--   0        0        0      302 2022-11-14 15:08:03.551809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/debounce.js
+-rw-r--r--   0        0        0      327 2022-11-14 15:08:03.551809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/debounce.js.flow
+-rw-r--r--   0        0        0      480 2022-11-14 15:08:03.551809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/detectOverflow.d.ts
+-rw-r--r--   0        0        0     3528 2022-11-14 15:08:03.552809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/detectOverflow.js
+-rw-r--r--   0        0        0     3265 2022-11-14 15:08:03.552809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/detectOverflow.js.flow
+-rw-r--r--   0        0        0      149 2022-11-14 15:08:03.555809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/expandToHashMap.d.ts
+-rw-r--r--   0        0        0      159 2022-11-14 15:08:03.555809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/expandToHashMap.js
+-rw-r--r--   0        0        0      246 2022-11-14 15:08:03.555809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/expandToHashMap.js.flow
+-rw-r--r--   0        0        0       77 2022-11-14 15:08:03.556809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/format.d.ts
+-rw-r--r--   0        0        0      286 2022-11-14 15:08:03.556809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/format.js
+-rw-r--r--   0        0        0      144 2022-11-14 15:08:03.556809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/format.js.flow
+-rw-r--r--   0        0        0       64 2022-11-14 15:08:03.557809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getAltAxis.d.ts
+-rw-r--r--   0        0        0       79 2022-11-14 15:08:03.557809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getAltAxis.js
+-rw-r--r--   0        0        0      112 2022-11-14 15:08:03.558809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getAltAxis.js.flow
+-rw-r--r--   0        0        0       80 2022-11-14 15:08:03.558809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getAltLen.d.ts
+-rw-r--r--   0        0        0       89 2022-11-14 15:08:03.558809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getAltLen.js
+-rw-r--r--   0        0        0      140 2022-11-14 15:08:03.559809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getAltLen.js.flow
+-rw-r--r--   0        0        0      152 2022-11-14 15:08:03.559809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getBasePlacement.d.ts
+-rw-r--r--   0        0        0      125 2022-11-14 15:08:03.559809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getBasePlacement.js
+-rw-r--r--   0        0        0      220 2022-11-14 15:08:03.559809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getBasePlacement.js.flow
+-rw-r--r--   0        0        0      102 2022-11-14 15:08:03.560809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getFreshSideObject.d.ts
+-rw-r--r--   0        0        0      117 2022-11-14 15:08:03.560809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getFreshSideObject.js
+-rw-r--r--   0        0        0      185 2022-11-14 15:08:03.560809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getFreshSideObject.js.flow
+-rw-r--r--   0        0        0      126 2022-11-14 15:08:03.561809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getMainAxisFromPlacement.d.ts
+-rw-r--r--   0        0        0      127 2022-11-14 15:08:03.561809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getMainAxisFromPlacement.js
+-rw-r--r--   0        0        0      207 2022-11-14 15:08:03.562809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getMainAxisFromPlacement.js.flow
+-rw-r--r--   0        0        0      122 2022-11-14 15:08:03.562809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositePlacement.d.ts
+-rw-r--r--   0        0        0      248 2022-11-14 15:08:03.563809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositePlacement.js
+-rw-r--r--   0        0        0      312 2022-11-14 15:08:03.564809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositePlacement.js.flow
+-rw-r--r--   0        0        0      131 2022-11-14 15:08:03.564809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositeVariationPlacement.d.ts
+-rw-r--r--   0        0        0      209 2022-11-14 15:08:03.564809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositeVariationPlacement.js
+-rw-r--r--   0        0        0      269 2022-11-14 15:08:03.565809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getOppositeVariationPlacement.js.flow
+-rw-r--r--   0        0        0      139 2022-11-14 15:08:03.565809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getVariation.d.ts
+-rw-r--r--   0        0        0       85 2022-11-14 15:08:03.565809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getVariation.js
+-rw-r--r--   0        0        0      185 2022-11-14 15:08:03.566809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/getVariation.js.flow
+-rw-r--r--   0        0        0      169 2022-11-14 15:08:03.566809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/math.d.ts
+-rw-r--r--   0        0        0       84 2022-11-14 15:08:03.567809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/math.js
+-rw-r--r--   0        0        0      100 2022-11-14 15:08:03.567809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/math.js.flow
+-rw-r--r--   0        0        0      162 2022-11-14 15:08:03.568809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergeByName.d.ts
+-rw-r--r--   0        0        0      524 2022-11-14 15:08:03.568809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergeByName.js
+-rw-r--r--   0        0        0      639 2022-11-14 15:08:03.569809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergeByName.js.flow
+-rw-r--r--   0        0        0      136 2022-11-14 15:08:03.569809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergePaddingObject.d.ts
+-rw-r--r--   0        0        0      184 2022-11-14 15:08:03.570809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergePaddingObject.js
+-rw-r--r--   0        0        0      274 2022-11-14 15:08:03.571809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergePaddingObject.js.flow
+-rw-r--r--   0        0        0      147 2022-11-14 15:08:03.571809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/orderModifiers.d.ts
+-rw-r--r--   0        0        0     1240 2022-11-14 15:08:03.571809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/orderModifiers.js
+-rw-r--r--   0        0        0     1360 2022-11-14 15:08:03.572809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/orderModifiers.js.flow
+-rw-r--r--   0        0        0      128 2022-11-14 15:08:03.572809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/rectToClientRect.d.ts
+-rw-r--r--   0        0        0      191 2022-11-14 15:08:03.572809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/rectToClientRect.js
+-rw-r--r--   0        0        0      271 2022-11-14 15:08:03.573809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/rectToClientRect.js.flow
+-rw-r--r--   0        0        0       84 2022-11-14 15:08:03.573809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/uniqueBy.d.ts
+-rw-r--r--   0        0        0      252 2022-11-14 15:08:03.573809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/uniqueBy.js
+-rw-r--r--   0        0        0      293 2022-11-14 15:08:03.574809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/uniqueBy.js.flow
+-rw-r--r--   0        0        0       47 2022-11-14 15:08:03.574809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/userAgent.d.ts
+-rw-r--r--   0        0        0      269 2022-11-14 15:08:03.575809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/userAgent.js
+-rw-r--r--   0        0        0      461 2022-11-14 15:08:03.575809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/userAgent.js.flow
+-rw-r--r--   0        0        0       72 2022-11-14 15:08:03.575809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/validateModifiers.d.ts
+-rw-r--r--   0        0        0     3261 2022-11-14 15:08:03.576810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/validateModifiers.js
+-rw-r--r--   0        0        0     4504 2022-11-14 15:08:03.576810 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/validateModifiers.js.flow
+-rw-r--r--   0        0        0      170 2022-11-14 15:08:03.577809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/within.d.ts
+-rw-r--r--   0        0        0      262 2022-11-14 15:08:03.577809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/within.js
+-rw-r--r--   0        0        0      329 2022-11-14 15:08:03.577809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/within.js.flow
+-rw-r--r--   0        0        0     4230 2022-11-14 15:08:03.411809 anitya-1.8.0/anitya/static/node_modules/@popperjs/core/package.json
+-rw-r--r--   0        0        0     1131 2022-11-16 11:34:15.722286 anitya-1.8.0/anitya/static/node_modules/bootstrap/LICENSE
+-rw-r--r--   0        0        0    13659 2022-11-16 11:34:15.764286 anitya-1.8.0/anitya/static/node_modules/bootstrap/README.md
+-rw-r--r--   0        0        0    71861 2022-11-16 11:34:15.723286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   210357 2022-11-16 11:34:15.745286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    53265 2022-11-16 11:34:15.724286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   131395 2022-11-16 11:34:15.746286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    71935 2022-11-16 11:34:15.725286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   210361 2022-11-16 11:34:15.746286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    53340 2022-11-16 11:34:15.725286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   131472 2022-11-16 11:34:15.747286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0     7965 2022-11-16 11:34:15.725286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   110875 2022-11-16 11:34:15.747286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0     6490 2022-11-16 11:34:15.726286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    40331 2022-11-16 11:34:15.747286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0     7958 2022-11-16 11:34:15.726286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   110888 2022-11-16 11:34:15.748286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0     6562 2022-11-16 11:34:15.727286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    48693 2022-11-16 11:34:15.748286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0    74135 2022-11-16 11:34:15.727286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   196435 2022-11-16 11:34:15.748286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    56365 2022-11-16 11:34:15.728286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   115588 2022-11-16 11:34:15.749286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0    74002 2022-11-16 11:34:15.728286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   196378 2022-11-16 11:34:15.749286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    56293 2022-11-16 11:34:15.729286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   115423 2022-11-16 11:34:15.750286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   237994 2022-11-16 11:34:15.729286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.css
+-rw-r--r--   0        0        0   608416 2022-11-16 11:34:15.753286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.css.map
+-rw-r--r--   0        0        0   194901 2022-11-16 11:34:15.730286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.min.css
+-rw-r--r--   0        0        0   522733 2022-11-16 11:34:15.756286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   237526 2022-11-16 11:34:15.731286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   608236 2022-11-16 11:34:15.758286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   195007 2022-11-16 11:34:15.731286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   767573 2022-11-16 11:34:15.760286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0   208123 2022-11-16 11:34:15.734286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   452089 2022-11-16 11:34:15.751286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80496 2022-11-16 11:34:15.734286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   333304 2022-11-16 11:34:15.752286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   136335 2022-11-16 11:34:15.735286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   308526 2022-11-16 11:34:15.754286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    74054 2022-11-16 11:34:15.735286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   221402 2022-11-16 11:34:15.755286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145677 2022-11-16 11:34:15.736286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.js
+-rw-r--r--   0        0        0   309667 2022-11-16 11:34:15.755286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60480 2022-11-16 11:34:15.736286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.min.js
+-rw-r--r--   0        0        0   217134 2022-11-16 11:34:15.757286 anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0     3140 2022-11-16 11:34:15.732286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/alert.js
+-rw-r--r--   0        0        0     4294 2022-11-16 11:34:15.744286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/alert.js.map
+-rw-r--r--   0        0        0     3224 2022-11-16 11:34:15.733286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/base-component.js
+-rw-r--r--   0        0        0     4602 2022-11-16 11:34:15.745286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/base-component.js.map
+-rw-r--r--   0        0        0     2756 2022-11-16 11:34:15.736286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/button.js
+-rw-r--r--   0        0        0     3466 2022-11-16 11:34:15.761286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/button.js.map
+-rw-r--r--   0        0        0    14281 2022-11-16 11:34:15.737286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/carousel.js
+-rw-r--r--   0        0        0    27442 2022-11-16 11:34:15.761286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/carousel.js.map
+-rw-r--r--   0        0        0     9455 2022-11-16 11:34:15.737286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/collapse.js
+-rw-r--r--   0        0        0    18212 2022-11-16 11:34:15.761286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/collapse.js.map
+-rw-r--r--   0        0        0     2119 2022-11-16 11:34:15.738286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/data.js
+-rw-r--r--   0        0        0     3047 2022-11-16 11:34:15.761286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/data.js.map
+-rw-r--r--   0        0        0     9578 2022-11-16 11:34:15.739286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/event-handler.js
+-rw-r--r--   0        0        0    19800 2022-11-16 11:34:15.762286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/event-handler.js.map
+-rw-r--r--   0        0        0     2438 2022-11-16 11:34:15.740286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/manipulator.js
+-rw-r--r--   0        0        0     4319 2022-11-16 11:34:15.762286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/manipulator.js.map
+-rw-r--r--   0        0        0     2700 2022-11-16 11:34:15.742286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/selector-engine.js
+-rw-r--r--   0        0        0     4619 2022-11-16 11:34:15.763286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/selector-engine.js.map
+-rw-r--r--   0        0        0    16199 2022-11-16 11:34:15.739286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dropdown.js
+-rw-r--r--   0        0        0    29448 2022-11-16 11:34:15.762286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dropdown.js.map
+-rw-r--r--   0        0        0    12194 2022-11-16 11:34:15.741286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/modal.js
+-rw-r--r--   0        0        0    22634 2022-11-16 11:34:15.762286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/modal.js.map
+-rw-r--r--   0        0        0     9166 2022-11-16 11:34:15.741286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/offcanvas.js
+-rw-r--r--   0        0        0    16142 2022-11-16 11:34:15.763286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/offcanvas.js.map
+-rw-r--r--   0        0        0     2883 2022-11-16 11:34:15.741286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/popover.js
+-rw-r--r--   0        0        0     4053 2022-11-16 11:34:15.763286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/popover.js.map
+-rw-r--r--   0        0        0    10303 2022-11-16 11:34:15.742286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/scrollspy.js
+-rw-r--r--   0        0        0    18973 2022-11-16 11:34:15.763286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/scrollspy.js.map
+-rw-r--r--   0        0        0    10647 2022-11-16 11:34:15.743286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/tab.js
+-rw-r--r--   0        0        0    19947 2022-11-16 11:34:15.764286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/tab.js.map
+-rw-r--r--   0        0        0     6632 2022-11-16 11:34:15.744286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/toast.js
+-rw-r--r--   0        0        0    12018 2022-11-16 11:34:15.764286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/toast.js.map
+-rw-r--r--   0        0        0    19359 2022-11-16 11:34:15.744286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/tooltip.js
+-rw-r--r--   0        0        0    37922 2022-11-16 11:34:15.764286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/tooltip.js.map
+-rw-r--r--   0        0        0     4413 2022-11-16 11:34:15.732286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/backdrop.js
+-rw-r--r--   0        0        0     7172 2022-11-16 11:34:15.745286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/backdrop.js.map
+-rw-r--r--   0        0        0     2174 2022-11-16 11:34:15.738286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/component-functions.js
+-rw-r--r--   0        0        0     2310 2022-11-16 11:34:15.761286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/component-functions.js.map
+-rw-r--r--   0        0        0     2808 2022-11-16 11:34:15.738286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/config.js
+-rw-r--r--   0        0        0     4073 2022-11-16 11:34:15.761286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/config.js.map
+-rw-r--r--   0        0        0     3913 2022-11-16 11:34:15.740286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/focustrap.js
+-rw-r--r--   0        0        0     5891 2022-11-16 11:34:15.762286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/focustrap.js.map
+-rw-r--r--   0        0        0    10248 2022-11-16 11:34:15.740286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/index.js
+-rw-r--r--   0        0        0    18675 2022-11-16 11:34:15.762286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/index.js.map
+-rw-r--r--   0        0        0     4253 2022-11-16 11:34:15.742286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/sanitizer.js
+-rw-r--r--   0        0        0     7572 2022-11-16 11:34:15.763286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/sanitizer.js.map
+-rw-r--r--   0        0        0     5031 2022-11-16 11:34:15.742286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/scrollbar.js
+-rw-r--r--   0        0        0     8041 2022-11-16 11:34:15.763286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/scrollbar.js.map
+-rw-r--r--   0        0        0     4733 2022-11-16 11:34:15.743286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/swipe.js
+-rw-r--r--   0        0        0     8335 2022-11-16 11:34:15.763286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/swipe.js.map
+-rw-r--r--   0        0        0     4980 2022-11-16 11:34:15.743286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/template-factory.js
+-rw-r--r--   0        0        0     8655 2022-11-16 11:34:15.764286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/template-factory.js.map
+-rw-r--r--   0        0        0     1901 2022-11-16 11:34:15.732286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/alert.js
+-rw-r--r--   0        0        0     1930 2022-11-16 11:34:15.733286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/base-component.js
+-rw-r--r--   0        0        0     1626 2022-11-16 11:34:15.737286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/button.js
+-rw-r--r--   0        0        0    11820 2022-11-16 11:34:15.737286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/carousel.js
+-rw-r--r--   0        0        0     7669 2022-11-16 11:34:15.737286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/collapse.js
+-rw-r--r--   0        0        0     1405 2022-11-16 11:34:15.739286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/dom/data.js
+-rw-r--r--   0        0        0     8450 2022-11-16 11:34:15.739286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/dom/event-handler.js
+-rw-r--r--   0        0        0     1668 2022-11-16 11:34:15.740286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/dom/manipulator.js
+-rw-r--r--   0        0        0     1968 2022-11-16 11:34:15.743286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/dom/selector-engine.js
+-rw-r--r--   0        0        0    13257 2022-11-16 11:34:15.739286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/dropdown.js
+-rw-r--r--   0        0        0     9629 2022-11-16 11:34:15.741286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/modal.js
+-rw-r--r--   0        0        0     6804 2022-11-16 11:34:15.741286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/offcanvas.js
+-rw-r--r--   0        0        0     1874 2022-11-16 11:34:15.741286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/popover.js
+-rw-r--r--   0        0        0     8448 2022-11-16 11:34:15.742286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/scrollspy.js
+-rw-r--r--   0        0        0     8756 2022-11-16 11:34:15.743286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/tab.js
+-rw-r--r--   0        0        0     5037 2022-11-16 11:34:15.744286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/toast.js
+-rw-r--r--   0        0        0    16305 2022-11-16 11:34:15.744286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/tooltip.js
+-rw-r--r--   0        0        0     3126 2022-11-16 11:34:15.733286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/backdrop.js
+-rw-r--r--   0        0        0     1072 2022-11-16 11:34:15.738286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/component-functions.js
+-rw-r--r--   0        0        0     1818 2022-11-16 11:34:15.738286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/config.js
+-rw-r--r--   0        0        0     2519 2022-11-16 11:34:15.740286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/focustrap.js
+-rw-r--r--   0        0        0     8436 2022-11-16 11:34:15.740286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/index.js
+-rw-r--r--   0        0        0     3253 2022-11-16 11:34:15.742286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/sanitizer.js
+-rw-r--r--   0        0        0     3755 2022-11-16 11:34:15.742286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/scrollbar.js
+-rw-r--r--   0        0        0     3410 2022-11-16 11:34:15.743286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/swipe.js
+-rw-r--r--   0        0        0     3630 2022-11-16 11:34:15.743286 anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/template-factory.js
+-rw-r--r--   0        0        0     9330 2022-11-16 11:34:15.744286 anitya-1.8.0/anitya/static/node_modules/bootstrap/package.json
+-rw-r--r--   0        0        0     4790 2022-11-16 11:34:15.765286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_accordion.scss
+-rw-r--r--   0        0        0     2126 2022-11-16 11:34:15.765286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_alert.scss
+-rw-r--r--   0        0        0     1118 2022-11-16 11:34:15.765286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_badge.scss
+-rw-r--r--   0        0        0     1751 2022-11-16 11:34:15.766286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_breadcrumb.scss
+-rw-r--r--   0        0        0     3073 2022-11-16 11:34:15.766286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_button-group.scss
+-rw-r--r--   0        0        0     6685 2022-11-16 11:34:15.766286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_buttons.scss
+-rw-r--r--   0        0        0     6736 2022-11-16 11:34:15.766286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_card.scss
+-rw-r--r--   0        0        0     5625 2022-11-16 11:34:15.767286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_carousel.scss
+-rw-r--r--   0        0        0     1127 2022-11-16 11:34:15.767286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_close.scss
+-rw-r--r--   0        0        0     1201 2022-11-16 11:34:15.769286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_containers.scss
+-rw-r--r--   0        0        0     8018 2022-11-16 11:34:15.770286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_dropdown.scss
+-rw-r--r--   0        0        0      256 2022-11-16 11:34:15.773286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_forms.scss
+-rw-r--r--   0        0        0    10553 2022-11-16 11:34:15.773286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_functions.scss
+-rw-r--r--   0        0        0      575 2022-11-16 11:34:15.774286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_grid.scss
+-rw-r--r--   0        0        0      294 2022-11-16 11:34:15.774286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_helpers.scss
+-rw-r--r--   0        0        0     1158 2022-11-16 11:34:15.774286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_images.scss
+-rw-r--r--   0        0        0     6475 2022-11-16 11:34:15.775287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_list-group.scss
+-rw-r--r--   0        0        0     1648 2022-11-16 11:34:15.776286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_maps.scss
+-rw-r--r--   0        0        0      899 2022-11-16 11:34:15.776286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_mixins.scss
+-rw-r--r--   0        0        0     7762 2022-11-16 11:34:15.776286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_modal.scss
+-rw-r--r--   0        0        0     4665 2022-11-16 11:34:15.777286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_nav.scss
+-rw-r--r--   0        0        0     8936 2022-11-16 11:34:15.777286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_navbar.scss
+-rw-r--r--   0        0        0     4555 2022-11-16 11:34:15.777286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_offcanvas.scss
+-rw-r--r--   0        0        0     3940 2022-11-16 11:34:15.777286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_pagination.scss
+-rw-r--r--   0        0        0      859 2022-11-16 11:34:15.778287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_placeholders.scss
+-rw-r--r--   0        0        0     6907 2022-11-16 11:34:15.778287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_popover.scss
+-rw-r--r--   0        0        0     1875 2022-11-16 11:34:15.778287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_progress.scss
+-rw-r--r--   0        0        0    12311 2022-11-16 11:34:15.779286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_reboot.scss
+-rw-r--r--   0        0        0     2395 2022-11-16 11:34:15.780286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_root.scss
+-rw-r--r--   0        0        0     2429 2022-11-16 11:34:15.780286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_spinners.scss
+-rw-r--r--   0        0        0     4358 2022-11-16 11:34:15.780286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_tables.scss
+-rw-r--r--   0        0        0     2490 2022-11-16 11:34:15.781287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_toasts.scss
+-rw-r--r--   0        0        0     3939 2022-11-16 11:34:15.781287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_tooltip.scss
+-rw-r--r--   0        0        0      425 2022-11-16 11:34:15.782287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_transitions.scss
+-rw-r--r--   0        0        0     1420 2022-11-16 11:34:15.782287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_type.scss
+-rw-r--r--   0        0        0    14817 2022-11-16 11:34:15.782287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_utilities.scss
+-rw-r--r--   0        0        0    68610 2022-11-16 11:34:15.783286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_variables.scss
+-rw-r--r--   0        0        0     1198 2022-11-16 11:34:15.783286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/bootstrap-grid.scss
+-rw-r--r--   0        0        0      163 2022-11-16 11:34:15.784287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/bootstrap-reboot.scss
+-rw-r--r--   0        0        0      240 2022-11-16 11:34:15.784287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/bootstrap-utilities.scss
+-rw-r--r--   0        0        0      912 2022-11-16 11:34:15.784287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/bootstrap.scss
+-rw-r--r--   0        0        0     2030 2022-11-16 11:34:15.771286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_floating-labels.scss
+-rw-r--r--   0        0        0     4287 2022-11-16 11:34:15.771286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_form-check.scss
+-rw-r--r--   0        0        0     5695 2022-11-16 11:34:15.771286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_form-control.scss
+-rw-r--r--   0        0        0     2796 2022-11-16 11:34:15.771286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_form-range.scss
+-rw-r--r--   0        0        0     2316 2022-11-16 11:34:15.771286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_form-select.scss
+-rw-r--r--   0        0        0      219 2022-11-16 11:34:15.771286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_form-text.scss
+-rw-r--r--   0        0        0     3835 2022-11-16 11:34:15.775287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_input-group.scss
+-rw-r--r--   0        0        0     1142 2022-11-16 11:34:15.775287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_labels.scss
+-rw-r--r--   0        0        0      478 2022-11-16 11:34:15.782287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_validation.scss
+-rw-r--r--   0        0        0       37 2022-11-16 11:34:15.767286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/helpers/_clearfix.scss
+-rw-r--r--   0        0        0      454 2022-11-16 11:34:15.767286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/helpers/_color-bg.scss
+-rw-r--r--   0        0        0      450 2022-11-16 11:34:15.769286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/helpers/_colored-links.scss
+-rw-r--r--   0        0        0      621 2022-11-16 11:34:15.778287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/helpers/_position.scss
+-rw-r--r--   0        0        0      399 2022-11-16 11:34:15.779286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/helpers/_ratio.scss
+-rw-r--r--   0        0        0      245 2022-11-16 11:34:15.780286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/helpers/_stacks.scss
+-rw-r--r--   0        0        0      223 2022-11-16 11:34:15.780286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/helpers/_stretched-link.scss
+-rw-r--r--   0        0        0       73 2022-11-16 11:34:15.781287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/helpers/_text-truncation.scss
+-rw-r--r--   0        0        0      136 2022-11-16 11:34:15.783286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/helpers/_visually-hidden.scss
+-rw-r--r--   0        0        0      147 2022-11-16 11:34:15.783286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/helpers/_vr.scss
+-rw-r--r--   0        0        0      393 2022-11-16 11:34:15.765286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_alert.scss
+-rw-r--r--   0        0        0      328 2022-11-16 11:34:15.765286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_backdrop.scss
+-rw-r--r--   0        0        0      263 2022-11-16 11:34:15.765286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_banner.scss
+-rw-r--r--   0        0        0     2031 2022-11-16 11:34:15.766286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_border-radius.scss
+-rw-r--r--   0        0        0      398 2022-11-16 11:34:15.766286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_box-shadow.scss
+-rw-r--r--   0        0        0     4580 2022-11-16 11:34:15.766286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_breakpoints.scss
+-rw-r--r--   0        0        0     3220 2022-11-16 11:34:15.766286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_buttons.scss
+-rw-r--r--   0        0        0     1473 2022-11-16 11:34:15.767286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_caret.scss
+-rw-r--r--   0        0        0      147 2022-11-16 11:34:15.767286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_clearfix.scss
+-rw-r--r--   0        0        0      167 2022-11-16 11:34:15.769286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_color-scheme.scss
+-rw-r--r--   0        0        0      410 2022-11-16 11:34:15.769286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_container.scss
+-rw-r--r--   0        0        0      613 2022-11-16 11:34:15.770286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_deprecate.scss
+-rw-r--r--   0        0        0     4122 2022-11-16 11:34:15.773286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_forms.scss
+-rw-r--r--   0        0        0     1956 2022-11-16 11:34:15.773286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_gradients.scss
+-rw-r--r--   0        0        0     4726 2022-11-16 11:34:15.774286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_grid.scss
+-rw-r--r--   0        0        0      395 2022-11-16 11:34:15.774286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_image.scss
+-rw-r--r--   0        0        0      509 2022-11-16 11:34:15.776286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_list-group.scss
+-rw-r--r--   0        0        0      168 2022-11-16 11:34:15.776286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_lists.scss
+-rw-r--r--   0        0        0      387 2022-11-16 11:34:15.778287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_pagination.scss
+-rw-r--r--   0        0        0      495 2022-11-16 11:34:15.779286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_reset-text.scss
+-rw-r--r--   0        0        0      202 2022-11-16 11:34:15.779286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_resize.scss
+-rw-r--r--   0        0        0     1101 2022-11-16 11:34:15.780286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_table-variants.scss
+-rw-r--r--   0        0        0      168 2022-11-16 11:34:15.781287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_text-truncate.scss
+-rw-r--r--   0        0        0      661 2022-11-16 11:34:15.781287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_transition.scss
+-rw-r--r--   0        0        0     3380 2022-11-16 11:34:15.782287 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_utilities.scss
+-rw-r--r--   0        0        0     1012 2022-11-16 11:34:15.783286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_visually-hidden.scss
+-rw-r--r--   0        0        0     1737 2022-11-16 11:34:15.765286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/utilities/_api.scss
+-rw-r--r--   0        0        0    10029 2022-11-16 11:34:15.779286 anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/vendor/_rfs.scss
+-rw-r--r--   0        0        0    12631 2022-11-14 15:08:03.532809 anitya-1.8.0/anitya/static/node_modules/jquery/AUTHORS.txt
+-rw-r--r--   0        0        0     1097 2022-11-14 15:08:03.538809 anitya-1.8.0/anitya/static/node_modules/jquery/LICENSE.txt
+-rw-r--r--   0        0        0     2004 2022-11-14 15:08:03.531809 anitya-1.8.0/anitya/static/node_modules/jquery/README.md
+-rw-r--r--   0        0        0      190 2022-11-14 15:08:03.522809 anitya-1.8.0/anitya/static/node_modules/jquery/bower.json
+-rw-r--r--   0        0        0   289812 2022-11-14 15:08:03.468809 anitya-1.8.0/anitya/static/node_modules/jquery/dist/jquery.js
+-rw-r--r--   0        0        0    89664 2022-11-14 15:08:03.472809 anitya-1.8.0/anitya/static/node_modules/jquery/dist/jquery.min.js
+-rw-r--r--   0        0        0   138161 2022-11-14 15:08:03.526809 anitya-1.8.0/anitya/static/node_modules/jquery/dist/jquery.min.map
+-rw-r--r--   0        0        0   236513 2022-11-14 15:08:03.477809 anitya-1.8.0/anitya/static/node_modules/jquery/dist/jquery.slim.js
+-rw-r--r--   0        0        0    72535 2022-11-14 15:08:03.479809 anitya-1.8.0/anitya/static/node_modules/jquery/dist/jquery.slim.min.js
+-rw-r--r--   0        0        0   110515 2022-11-14 15:08:03.529809 anitya-1.8.0/anitya/static/node_modules/jquery/dist/jquery.slim.min.map
+-rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.537809 anitya-1.8.0/anitya/static/node_modules/jquery/external/sizzle/LICENSE.txt
+-rw-r--r--   0        0        0    70555 2022-11-14 15:08:03.509809 anitya-1.8.0/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.js
+-rw-r--r--   0        0        0    20245 2022-11-14 15:08:03.510809 anitya-1.8.0/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.min.js
+-rw-r--r--   0        0        0    31112 2022-11-14 15:08:03.530809 anitya-1.8.0/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.min.map
+-rw-r--r--   0        0        0     3284 2022-11-14 15:08:03.523809 anitya-1.8.0/anitya/static/node_modules/jquery/package.json
+-rw-r--r--   0        0        0     2753 2022-11-14 15:08:03.480809 anitya-1.8.0/anitya/static/node_modules/jquery/src/ajax/jsonp.js
+-rw-r--r--   0        0        0     1904 2022-11-14 15:08:03.480809 anitya-1.8.0/anitya/static/node_modules/jquery/src/ajax/load.js
+-rw-r--r--   0        0        0     1637 2022-11-14 15:08:03.496809 anitya-1.8.0/anitya/static/node_modules/jquery/src/ajax/script.js
+-rw-r--r--   0        0        0       67 2022-11-14 15:08:03.481809 anitya-1.8.0/anitya/static/node_modules/jquery/src/ajax/var/location.js
+-rw-r--r--   0        0        0       72 2022-11-14 15:08:03.482809 anitya-1.8.0/anitya/static/node_modules/jquery/src/ajax/var/nonce.js
+-rw-r--r--   0        0        0       60 2022-11-14 15:08:03.492809 anitya-1.8.0/anitya/static/node_modules/jquery/src/ajax/var/rquery.js
+-rw-r--r--   0        0        0     4355 2022-11-14 15:08:03.521809 anitya-1.8.0/anitya/static/node_modules/jquery/src/ajax/xhr.js
+-rw-r--r--   0        0        0    22924 2022-11-14 15:08:03.421809 anitya-1.8.0/anitya/static/node_modules/jquery/src/ajax.js
+-rw-r--r--   0        0        0     3272 2022-11-14 15:08:03.425809 anitya-1.8.0/anitya/static/node_modules/jquery/src/attributes/attr.js
+-rw-r--r--   0        0        0     4527 2022-11-14 15:08:03.428809 anitya-1.8.0/anitya/static/node_modules/jquery/src/attributes/classes.js
+-rw-r--r--   0        0        0     2857 2022-11-14 15:08:03.486809 anitya-1.8.0/anitya/static/node_modules/jquery/src/attributes/prop.js
+-rw-r--r--   0        0        0      786 2022-11-14 15:08:03.513809 anitya-1.8.0/anitya/static/node_modules/jquery/src/attributes/support.js
+-rw-r--r--   0        0        0     4261 2022-11-14 15:08:03.519809 anitya-1.8.0/anitya/static/node_modules/jquery/src/attributes/val.js
+-rw-r--r--   0        0        0      217 2022-11-14 15:08:03.425809 anitya-1.8.0/anitya/static/node_modules/jquery/src/attributes.js
+-rw-r--r--   0        0        0     5552 2022-11-14 15:08:03.427809 anitya-1.8.0/anitya/static/node_modules/jquery/src/callbacks.js
+-rw-r--r--   0        0        0     1160 2022-11-14 15:08:03.449809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/DOMEval.js
+-rw-r--r--   0        0        0     1314 2022-11-14 15:08:03.414809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/access.js
+-rw-r--r--   0        0        0      550 2022-11-14 15:08:03.427809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/camelCase.js
+-rw-r--r--   0        0        0     3345 2022-11-14 15:08:03.460809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/init.js
+-rw-r--r--   0        0        0      789 2022-11-14 15:08:03.461809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/isAttached.js
+-rw-r--r--   0        0        0      176 2022-11-14 15:08:03.482809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/nodeName.js
+-rw-r--r--   0        0        0     1604 2022-11-14 15:08:03.485809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/parseHTML.js
+-rw-r--r--   0        0        0      739 2022-11-14 15:08:03.486809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/parseXML.js
+-rw-r--r--   0        0        0     2268 2022-11-14 15:08:03.489809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/ready-no-deferred.js
+-rw-r--r--   0        0        0     2101 2022-11-14 15:08:03.490809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/ready.js
+-rw-r--r--   0        0        0      168 2022-11-14 15:08:03.490809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/readyException.js
+-rw-r--r--   0        0        0      362 2022-11-14 15:08:03.512809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/stripAndCollapse.js
+-rw-r--r--   0        0        0      631 2022-11-14 15:08:03.513809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/support.js
+-rw-r--r--   0        0        0      379 2022-11-14 15:08:03.516809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/toType.js
+-rw-r--r--   0        0        0      244 2022-11-14 15:08:03.494809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core/var/rsingleTag.js
+-rw-r--r--   0        0        0     9183 2022-11-14 15:08:03.429809 anitya-1.8.0/anitya/static/node_modules/jquery/src/core.js
+-rw-r--r--   0        0        0      530 2022-11-14 15:08:03.416809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/addGetHookIf.js
+-rw-r--r--   0        0        0     2002 2022-11-14 15:08:03.417809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/adjustCSS.js
+-rw-r--r--   0        0        0     2191 2022-11-14 15:08:03.434809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/curCSS.js
+-rw-r--r--   0        0        0      870 2022-11-14 15:08:03.454809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/finalPropName.js
+-rw-r--r--   0        0        0      317 2022-11-14 15:08:03.460809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/hiddenVisibleSelectors.js
+-rw-r--r--   0        0        0     2304 2022-11-14 15:08:03.499809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/showHide.js
+-rw-r--r--   0        0        0     4829 2022-11-14 15:08:03.514809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/support.js
+-rw-r--r--   0        0        0       88 2022-11-14 15:08:03.433809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/var/cssExpand.js
+-rw-r--r--   0        0        0      409 2022-11-14 15:08:03.458809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/var/getStyles.js
+-rw-r--r--   0        0        0     1284 2022-11-14 15:08:03.461809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/var/isHiddenWithinTree.js
+-rw-r--r--   0        0        0      123 2022-11-14 15:08:03.487809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/var/rboxStyle.js
+-rw-r--r--   0        0        0       57 2022-11-14 15:08:03.489809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/var/rcustomProp.js
+-rw-r--r--   0        0        0      131 2022-11-14 15:08:03.492809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/var/rnumnonpx.js
+-rw-r--r--   0        0        0      501 2022-11-14 15:08:03.515809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css/var/swap.js
+-rw-r--r--   0        0        0    14195 2022-11-14 15:08:03.430809 anitya-1.8.0/anitya/static/node_modules/jquery/src/css.js
+-rw-r--r--   0        0        0     3956 2022-11-14 15:08:03.436809 anitya-1.8.0/anitya/static/node_modules/jquery/src/data/Data.js
+-rw-r--r--   0        0        0      318 2022-11-14 15:08:03.412809 anitya-1.8.0/anitya/static/node_modules/jquery/src/data/var/acceptData.js
+-rw-r--r--   0        0        0       84 2022-11-14 15:08:03.437809 anitya-1.8.0/anitya/static/node_modules/jquery/src/data/var/dataPriv.js
+-rw-r--r--   0        0        0       84 2022-11-14 15:08:03.437809 anitya-1.8.0/anitya/static/node_modules/jquery/src/data/var/dataUser.js
+-rw-r--r--   0        0        0     4325 2022-11-14 15:08:03.435809 anitya-1.8.0/anitya/static/node_modules/jquery/src/data.js
+-rw-r--r--   0        0        0      640 2022-11-14 15:08:03.452809 anitya-1.8.0/anitya/static/node_modules/jquery/src/deferred/exceptionHook.js
+-rw-r--r--   0        0        0    11007 2022-11-14 15:08:03.438809 anitya-1.8.0/anitya/static/node_modules/jquery/src/deferred.js
+-rw-r--r--   0        0        0      296 2022-11-14 15:08:03.419809 anitya-1.8.0/anitya/static/node_modules/jquery/src/deprecated/ajax-event-alias.js
+-rw-r--r--   0        0        0     1140 2022-11-14 15:08:03.451809 anitya-1.8.0/anitya/static/node_modules/jquery/src/deprecated/event.js
+-rw-r--r--   0        0        0     2406 2022-11-14 15:08:03.440809 anitya-1.8.0/anitya/static/node_modules/jquery/src/deprecated.js
+-rw-r--r--   0        0        0     1756 2022-11-14 15:08:03.441809 anitya-1.8.0/anitya/static/node_modules/jquery/src/dimensions.js
+-rw-r--r--   0        0        0     3291 2022-11-14 15:08:03.518809 anitya-1.8.0/anitya/static/node_modules/jquery/src/effects/Tween.js
+-rw-r--r--   0        0        0      244 2022-11-14 15:08:03.423809 anitya-1.8.0/anitya/static/node_modules/jquery/src/effects/animatedSelector.js
+-rw-r--r--   0        0        0    17417 2022-11-14 15:08:03.450809 anitya-1.8.0/anitya/static/node_modules/jquery/src/effects.js
+-rw-r--r--   0        0        0     1665 2022-11-14 15:08:03.457809 anitya-1.8.0/anitya/static/node_modules/jquery/src/event/focusin.js
+-rw-r--r--   0        0        0      133 2022-11-14 15:08:03.514809 anitya-1.8.0/anitya/static/node_modules/jquery/src/event/support.js
+-rw-r--r--   0        0        0     5438 2022-11-14 15:08:03.518809 anitya-1.8.0/anitya/static/node_modules/jquery/src/event/trigger.js
+-rw-r--r--   0        0        0    24505 2022-11-14 15:08:03.452809 anitya-1.8.0/anitya/static/node_modules/jquery/src/event.js
+-rw-r--r--   0        0        0     1024 2022-11-14 15:08:03.422809 anitya-1.8.0/anitya/static/node_modules/jquery/src/exports/amd.js
+-rw-r--r--   0        0        0      628 2022-11-14 15:08:03.459809 anitya-1.8.0/anitya/static/node_modules/jquery/src/exports/global.js
+-rw-r--r--   0        0        0      646 2022-11-14 15:08:03.470809 anitya-1.8.0/anitya/static/node_modules/jquery/src/jquery.js
+-rw-r--r--   0        0        0      690 2022-11-14 15:08:03.409809 anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation/_evalUrl.js
+-rw-r--r--   0        0        0     2490 2022-11-14 15:08:03.426809 anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation/buildFragment.js
+-rw-r--r--   0        0        0      654 2022-11-14 15:08:03.457809 anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation/getAll.js
+-rw-r--r--   0        0        0      381 2022-11-14 15:08:03.499809 anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation/setGlobalEval.js
+-rw-r--r--   0        0        0     1244 2022-11-14 15:08:03.514809 anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation/support.js
+-rw-r--r--   0        0        0       92 2022-11-14 15:08:03.493809 anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation/var/rscriptType.js
+-rw-r--r--   0        0        0      304 2022-11-14 15:08:03.494809 anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation/var/rtagName.js
+-rw-r--r--   0        0        0      823 2022-11-14 15:08:03.520809 anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation/wrapMap.js
+-rw-r--r--   0        0        0    12674 2022-11-14 15:08:03.481809 anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation.js
+-rw-r--r--   0        0        0     6828 2022-11-14 15:08:03.484809 anitya-1.8.0/anitya/static/node_modules/jquery/src/offset.js
+-rw-r--r--   0        0        0      534 2022-11-14 15:08:03.439809 anitya-1.8.0/anitya/static/node_modules/jquery/src/queue/delay.js
+-rw-r--r--   0        0        0     3091 2022-11-14 15:08:03.487809 anitya-1.8.0/anitya/static/node_modules/jquery/src/queue.js
+-rw-r--r--   0        0        0     6463 2022-11-14 15:08:03.497809 anitya-1.8.0/anitya/static/node_modules/jquery/src/selector-native.js
+-rw-r--r--   0        0        0      411 2022-11-14 15:08:03.497809 anitya-1.8.0/anitya/static/node_modules/jquery/src/selector-sizzle.js
+-rw-r--r--   0        0        0       66 2022-11-14 15:08:03.498809 anitya-1.8.0/anitya/static/node_modules/jquery/src/selector.js
+-rw-r--r--   0        0        0     3236 2022-11-14 15:08:03.498809 anitya-1.8.0/anitya/static/node_modules/jquery/src/serialize.js
+-rw-r--r--   0        0        0     2352 2022-11-14 15:08:03.455809 anitya-1.8.0/anitya/static/node_modules/jquery/src/traversing/findFilter.js
+-rw-r--r--   0        0        0      371 2022-11-14 15:08:03.447809 anitya-1.8.0/anitya/static/node_modules/jquery/src/traversing/var/dir.js
+-rw-r--r--   0        0        0      128 2022-11-14 15:08:03.491809 anitya-1.8.0/anitya/static/node_modules/jquery/src/traversing/var/rneedsContext.js
+-rw-r--r--   0        0        0      218 2022-11-14 15:08:03.500809 anitya-1.8.0/anitya/static/node_modules/jquery/src/traversing/var/siblings.js
+-rw-r--r--   0        0        0     4692 2022-11-14 15:08:03.517809 anitya-1.8.0/anitya/static/node_modules/jquery/src/traversing.js
+-rw-r--r--   0        0        0      110 2022-11-14 15:08:03.483809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/ObjectFunctionString.js
+-rw-r--r--   0        0        0       54 2022-11-14 15:08:03.424809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/arr.js
+-rw-r--r--   0        0        0       82 2022-11-14 15:08:03.428809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/class2type.js
+-rw-r--r--   0        0        0       67 2022-11-14 15:08:03.448809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/document.js
+-rw-r--r--   0        0        0      105 2022-11-14 15:08:03.448809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/documentElement.js
+-rw-r--r--   0        0        0      372 2022-11-14 15:08:03.455809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/flat.js
+-rw-r--r--   0        0        0       92 2022-11-14 15:08:03.456809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/fnToString.js
+-rw-r--r--   0        0        0       73 2022-11-14 15:08:03.458809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/getProto.js
+-rw-r--r--   0        0        0      110 2022-11-14 15:08:03.459809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/hasOwn.js
+-rw-r--r--   0        0        0       82 2022-11-14 15:08:03.460809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/indexOf.js
+-rw-r--r--   0        0        0      674 2022-11-14 15:08:03.461809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/isFunction.js
+-rw-r--r--   0        0        0      126 2022-11-14 15:08:03.462809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/isWindow.js
+-rw-r--r--   0        0        0      100 2022-11-14 15:08:03.486809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/pnum.js
+-rw-r--r--   0        0        0       79 2022-11-14 15:08:03.486809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/push.js
+-rw-r--r--   0        0        0       79 2022-11-14 15:08:03.488809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/rcheckableType.js
+-rw-r--r--   0        0        0      136 2022-11-14 15:08:03.488809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/rcssNum.js
+-rw-r--r--   0        0        0      202 2022-11-14 15:08:03.491809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/rnothtmlwhite.js
+-rw-r--r--   0        0        0      174 2022-11-14 15:08:03.494809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/rtrimCSS.js
+-rw-r--r--   0        0        0       80 2022-11-14 15:08:03.512809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/slice.js
+-rw-r--r--   0        0        0      117 2022-11-14 15:08:03.515809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/support.js
+-rw-r--r--   0        0        0      104 2022-11-14 15:08:03.516809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/toString.js
+-rw-r--r--   0        0        0      125 2022-11-14 15:08:03.519809 anitya-1.8.0/anitya/static/node_modules/jquery/src/var/whitespace.js
+-rw-r--r--   0        0        0     1477 2022-11-14 15:08:03.520809 anitya-1.8.0/anitya/static/node_modules/jquery/src/wrap.js
+-rw-r--r--   0        0        0      115 2022-11-14 15:08:03.829810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/.github/dependabot.yml
+-rw-r--r--   0        0        0     1484 2022-11-14 15:08:03.829810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/.github/workflows/test.yml
+-rw-r--r--   0        0        0    14243 2022-11-14 15:08:03.819810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/AUTHORS.txt
+-rw-r--r--   0        0        0     4545 2022-11-14 15:08:03.751810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1817 2022-11-14 15:08:03.824810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/LICENSE.txt
+-rw-r--r--   0        0        0     2470 2022-11-14 15:08:03.751810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/README.md
+-rw-r--r--   0        0        0     2262 2022-11-14 15:08:03.751810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/bower.json
+-rw-r--r--   0        0        0     1241 2022-11-14 15:08:03.746810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/build/release-test.js
+-rw-r--r--   0        0        0     4749 2022-11-14 15:08:03.746810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/build/release.js
+-rw-r--r--   0        0        0     1108 2022-11-14 15:08:03.593809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/build/tasks/build.js
+-rw-r--r--   0        0        0     3110 2022-11-14 15:08:03.750810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/build/tasks/testswarm.js
+-rw-r--r--   0        0        0    60060 2022-11-14 15:08:03.413809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/build/themes
+-rw-r--r--   0        0        0   529159 2022-11-14 15:08:03.637810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/jquery-ui.js
+-rw-r--r--   0        0        0   255084 2022-11-14 15:08:03.640810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/jquery-ui.min.js
+-rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.792810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     7126 2022-11-14 15:08:03.795810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.797810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.797810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.806810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.814810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36099 2022-11-14 15:08:03.424809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/jquery-ui.css
+-rw-r--r--   0        0        0    30778 2022-11-14 15:08:03.525809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/jquery-ui.min.css
+-rw-r--r--   0        0        0    17432 2022-11-14 15:08:03.565809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/theme.css
+-rw-r--r--   0        0        0      435 2022-11-14 15:08:03.756810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_diagonals-thick_8_333333_40x40.png
+-rw-r--r--   0        0        0      375 2022-11-14 15:08:03.768810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_glass_40_111111_1x400.png
+-rw-r--r--   0        0        0      375 2022-11-14 15:08:03.769810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_glass_55_1c1c1c_1x400.png
+-rw-r--r--   0        0        0      367 2022-11-14 15:08:03.778810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_highlight-hard_100_f9f9f9_1x100.png
+-rw-r--r--   0        0        0      368 2022-11-14 15:08:03.779810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_highlight-hard_40_aaaaaa_1x100.png
+-rw-r--r--   0        0        0      379 2022-11-14 15:08:03.783810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_highlight-soft_50_aaaaaa_1x100.png
+-rw-r--r--   0        0        0      434 2022-11-14 15:08:03.785810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_inset-hard_45_cd0a0a_1x100.png
+-rw-r--r--   0        0        0      419 2022-11-14 15:08:03.785810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-bg_inset-hard_55_ffeb80_1x100.png
+-rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_222222_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_4ca300_256x240.png
+-rw-r--r--   0        0        0     7144 2022-11-14 15:08:03.802810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_bbbbbb_256x240.png
+-rw-r--r--   0        0        0     7063 2022-11-14 15:08:03.810810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ededed_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ffcf29_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.814810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36800 2022-11-14 15:08:03.427809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/jquery-ui.css
+-rw-r--r--   0        0        0    31457 2022-11-14 15:08:03.526809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/jquery-ui.min.css
+-rw-r--r--   0        0        0    18133 2022-11-14 15:08:03.566809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/theme.css
+-rw-r--r--   0        0        0      523 2022-11-14 15:08:03.756810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_diagonals-thick_75_f3d8d8_40x40.png
+-rw-r--r--   0        0        0      318 2022-11-14 15:08:03.760810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_dots-small_65_a6a6a6_2x2.png
+-rw-r--r--   0        0        0      450 2022-11-14 15:08:03.770810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_glass_55_fbf8ee_1x400.png
+-rw-r--r--   0        0        0      368 2022-11-14 15:08:03.778810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_highlight-hard_100_eeeeee_1x100.png
+-rw-r--r--   0        0        0      368 2022-11-14 15:08:03.778810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_highlight-hard_100_f6f6f6_1x100.png
+-rw-r--r--   0        0        0      437 2022-11-14 15:08:03.781810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_highlight-soft_15_cc0000_1x100.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.787810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_004276_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.806810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.814810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36693 2022-11-14 15:08:03.430809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/jquery-ui.css
+-rw-r--r--   0        0        0    31359 2022-11-14 15:08:03.527809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/jquery-ui.min.css
+-rw-r--r--   0        0        0    18026 2022-11-14 15:08:03.568809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/theme.css
+-rw-r--r--   0        0        0      432 2022-11-14 15:08:03.757810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_diagonals-thick_90_eeeeee_40x40.png
+-rw-r--r--   0        0        0      460 2022-11-14 15:08:03.765810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_glass_100_e4f1fb_1x400.png
+-rw-r--r--   0        0        0      446 2022-11-14 15:08:03.769810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_glass_50_3baae3_1x400.png
+-rw-r--r--   0        0        0      456 2022-11-14 15:08:03.772810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_glass_80_d7ebf9_1x400.png
+-rw-r--r--   0        0        0      442 2022-11-14 15:08:03.778810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_highlight-hard_100_f2f5f7_1x100.png
+-rw-r--r--   0        0        0      362 2022-11-14 15:08:03.780810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_highlight-hard_70_000000_1x100.png
+-rw-r--r--   0        0        0      497 2022-11-14 15:08:03.780810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_highlight-soft_100_deedf7_1x100.png
+-rw-r--r--   0        0        0      419 2022-11-14 15:08:03.782810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-bg_highlight-soft_25_ffef8f_1x100.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.790810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_2694e8_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_3d80b3_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_72a7cf_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.814810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36850 2022-11-14 15:08:03.437809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/jquery-ui.css
+-rw-r--r--   0        0        0    31543 2022-11-14 15:08:03.528809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/jquery-ui.min.css
+-rw-r--r--   0        0        0    18183 2022-11-14 15:08:03.570809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/theme.css
+-rw-r--r--   0        0        0      426 2022-11-14 15:08:03.768810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_glass_40_ffc73d_1x400.png
+-rw-r--r--   0        0        0      433 2022-11-14 15:08:03.779810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-hard_20_0972a5_1x100.png
+-rw-r--r--   0        0        0      453 2022-11-14 15:08:03.782810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-soft_33_003147_1x100.png
+-rw-r--r--   0        0        0      394 2022-11-14 15:08:03.783810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-soft_35_222222_1x100.png
+-rw-r--r--   0        0        0      380 2022-11-14 15:08:03.783810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-soft_44_444444_1x100.png
+-rw-r--r--   0        0        0      387 2022-11-14 15:08:03.784810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_highlight-soft_80_eeeeee_1x100.png
+-rw-r--r--   0        0        0      430 2022-11-14 15:08:03.787810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-bg_loop_25_000000_21x21.png
+-rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_222222_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_4b8e0b_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_a83300_256x240.png
+-rw-r--r--   0        0        0     7086 2022-11-14 15:08:03.806810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_cccccc_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.815810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36796 2022-11-14 15:08:03.441809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/jquery-ui.css
+-rw-r--r--   0        0        0    31444 2022-11-14 15:08:03.530809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/jquery-ui.min.css
+-rw-r--r--   0        0        0    18129 2022-11-14 15:08:03.571809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/theme.css
+-rw-r--r--   0        0        0      534 2022-11-14 15:08:03.755810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_diagonals-thick_15_0b3e6f_40x40.png
+-rw-r--r--   0        0        0      347 2022-11-14 15:08:03.759810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_dots-medium_30_0b58a2_4x4.png
+-rw-r--r--   0        0        0      318 2022-11-14 15:08:03.759810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_dots-small_20_333333_2x2.png
+-rw-r--r--   0        0        0      328 2022-11-14 15:08:03.759810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_dots-small_30_a32d00_2x2.png
+-rw-r--r--   0        0        0      334 2022-11-14 15:08:03.760810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_dots-small_40_00498f_2x2.png
+-rw-r--r--   0        0        0     4042 2022-11-14 15:08:03.774810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_gloss-wave_20_111111_500x100.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.787810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_00498f_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_98d2fb_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_9ccdfc_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.815810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36666 2022-11-14 15:08:03.451809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/jquery-ui.css
+-rw-r--r--   0        0        0    31341 2022-11-14 15:08:03.531809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/jquery-ui.min.css
+-rw-r--r--   0        0        0    17999 2022-11-14 15:08:03.572809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/theme.css
+-rw-r--r--   0        0        0     6051 2022-11-14 15:08:03.774810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_gloss-wave_30_3d3644_500x100.png
+-rw-r--r--   0        0        0      452 2022-11-14 15:08:03.780810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_highlight-soft_100_dcd9de_1x100.png
+-rw-r--r--   0        0        0      483 2022-11-14 15:08:03.781810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_highlight-soft_100_eae6ea_1x100.png
+-rw-r--r--   0        0        0      472 2022-11-14 15:08:03.782810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_highlight-soft_25_30273a_1x100.png
+-rw-r--r--   0        0        0      457 2022-11-14 15:08:03.783810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_highlight-soft_45_5f5964_1x100.png
+-rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.792810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_454545_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_734d99_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_8d78a5_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_a8a3ae_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_ebccce_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.815810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36720 2022-11-14 15:08:03.455809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/jquery-ui.css
+-rw-r--r--   0        0        0    31404 2022-11-14 15:08:03.534809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/jquery-ui.min.css
+-rw-r--r--   0        0        0    18053 2022-11-14 15:08:03.573809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/theme.css
+-rw-r--r--   0        0        0      452 2022-11-14 15:08:03.753810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-small_25_c5ddfc_40x40.png
+-rw-r--r--   0        0        0      527 2022-11-14 15:08:03.755810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_20_e69700_40x40.png
+-rw-r--r--   0        0        0      519 2022-11-14 15:08:03.756810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_22_1484e6_40x40.png
+-rw-r--r--   0        0        0      516 2022-11-14 15:08:03.756810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_26_2293f7_40x40.png
+-rw-r--r--   0        0        0      377 2022-11-14 15:08:03.781810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_highlight-soft_100_f9f9f9_1x100.png
+-rw-r--r--   0        0        0      366 2022-11-14 15:08:03.785810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_inset-hard_100_eeeeee_1x100.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_0a82eb_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_0b54d5_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.795810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_5fa5e3_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_fcdd4a_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.815810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36824 2022-11-14 15:08:03.459809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/jquery-ui.css
+-rw-r--r--   0        0        0    31486 2022-11-14 15:08:03.536809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/jquery-ui.min.css
+-rw-r--r--   0        0        0    18157 2022-11-14 15:08:03.575809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/theme.css
+-rw-r--r--   0        0        0      317 2022-11-14 15:08:03.771810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0        0        0      382 2022-11-14 15:08:03.781810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-bg_highlight-soft_100_f6f6f6_1x100.png
+-rw-r--r--   0        0        0      445 2022-11-14 15:08:03.782810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-bg_highlight-soft_25_0073ea_1x100.png
+-rw-r--r--   0        0        0      391 2022-11-14 15:08:03.783810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-bg_highlight-soft_50_dddddd_1x100.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_0073ea_256x240.png
+-rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.792810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_454545_256x240.png
+-rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.795810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_666666_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_ff0084_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.816810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36570 2022-11-14 15:08:03.462809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/jquery-ui.css
+-rw-r--r--   0        0        0    31215 2022-11-14 15:08:03.538809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/jquery-ui.min.css
+-rw-r--r--   0        0        0    17903 2022-11-14 15:08:03.575809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/theme.css
+-rw-r--r--   0        0        0      442 2022-11-14 15:08:03.754810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_diagonals-small_40_db4865_40x40.png
+-rw-r--r--   0        0        0      443 2022-11-14 15:08:03.754810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_diagonals-small_50_93c3cd_40x40.png
+-rw-r--r--   0        0        0      440 2022-11-14 15:08:03.754810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_diagonals-small_50_ff3853_40x40.png
+-rw-r--r--   0        0        0      443 2022-11-14 15:08:03.754810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_diagonals-small_75_ccd232_40x40.png
+-rw-r--r--   0        0        0      335 2022-11-14 15:08:03.759810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_dots-medium_80_ffff38_4x4.png
+-rw-r--r--   0        0        0      333 2022-11-14 15:08:03.760810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_dots-small_35_35414f_2x2.png
+-rw-r--r--   0        0        0      474 2022-11-14 15:08:03.787810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-bg_white-lines_85_f7f7ba_40x100.png
+-rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.793810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_454545_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.798810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_88a206_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.804810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_c02669_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_e1e463_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.814810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_ffeb33_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36804 2022-11-14 15:08:03.466809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/jquery-ui.css
+-rw-r--r--   0        0        0    31500 2022-11-14 15:08:03.540809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/jquery-ui.min.css
+-rw-r--r--   0        0        0    18137 2022-11-14 15:08:03.576810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/theme.css
+-rw-r--r--   0        0        0      464 2022-11-14 15:08:03.766810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_glass_100_f5f0e5_1x400.png
+-rw-r--r--   0        0        0      445 2022-11-14 15:08:03.767810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_glass_25_cb842e_1x400.png
+-rw-r--r--   0        0        0      464 2022-11-14 15:08:03.772810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_glass_70_ede4d4_1x400.png
+-rw-r--r--   0        0        0      437 2022-11-14 15:08:03.778810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_highlight-hard_100_f4f0ec_1x100.png
+-rw-r--r--   0        0        0      424 2022-11-14 15:08:03.780810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_highlight-hard_65_fee4bd_1x100.png
+-rw-r--r--   0        0        0      433 2022-11-14 15:08:03.780810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_highlight-hard_75_f5f5b5_1x100.png
+-rw-r--r--   0        0        0      513 2022-11-14 15:08:03.786810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_inset-soft_100_f4f0ec_1x100.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.805810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_c47a23_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.805810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_cb672b_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.810810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_f08000_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_f35f07_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_ff7519_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36789 2022-11-14 15:08:03.468809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/jquery-ui.css
+-rw-r--r--   0        0        0    31503 2022-11-14 15:08:03.541809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/jquery-ui.min.css
+-rw-r--r--   0        0        0    18122 2022-11-14 15:08:03.577809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/theme.css
+-rw-r--r--   0        0        0      317 2022-11-14 15:08:03.752810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_diagonals-small_0_aaaaaa_40x40.png
+-rw-r--r--   0        0        0      435 2022-11-14 15:08:03.755810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_diagonals-thick_15_444444_40x40.png
+-rw-r--r--   0        0        0      521 2022-11-14 15:08:03.757810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_diagonals-thick_95_ffdc2e_40x40.png
+-rw-r--r--   0        0        0      446 2022-11-14 15:08:03.770810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_glass_55_fbf5d0_1x400.png
+-rw-r--r--   0        0        0      434 2022-11-14 15:08:03.779810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_highlight-hard_30_285c00_1x100.png
+-rw-r--r--   0        0        0      455 2022-11-14 15:08:03.782810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_highlight-soft_33_3a8104_1x100.png
+-rw-r--r--   0        0        0      461 2022-11-14 15:08:03.783810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_highlight-soft_50_4eb305_1x100.png
+-rw-r--r--   0        0        0      469 2022-11-14 15:08:03.783810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_highlight-soft_60_4ca20b_1x100.png
+-rw-r--r--   0        0        0      476 2022-11-14 15:08:03.786810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_inset-soft_10_285c00_1x100.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_4eb305_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_72b42d_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36964 2022-11-14 15:08:03.471809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/jquery-ui.css
+-rw-r--r--   0        0        0    31647 2022-11-14 15:08:03.542809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/jquery-ui.min.css
+-rw-r--r--   0        0        0    18297 2022-11-14 15:08:03.578809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/theme.css
+-rw-r--r--   0        0        0      445 2022-11-14 15:08:03.767810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_glass_15_5f391b_1x400.png
+-rw-r--r--   0        0        0     5903 2022-11-14 15:08:03.774810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_20_1c160d_500x100.png
+-rw-r--r--   0        0        0     5962 2022-11-14 15:08:03.774810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_25_453326_500x100.png
+-rw-r--r--   0        0        0     6024 2022-11-14 15:08:03.775810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_30_44372c_500x100.png
+-rw-r--r--   0        0        0      485 2022-11-14 15:08:03.781810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_highlight-soft_20_201913_1x100.png
+-rw-r--r--   0        0        0      453 2022-11-14 15:08:03.782810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_highlight-soft_20_619226_1x100.png
+-rw-r--r--   0        0        0      490 2022-11-14 15:08:03.786810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_inset-soft_10_201913_1x100.png
+-rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_222222_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_9bcc60_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_add978_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_e3ddc9_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_f1fd86_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36822 2022-11-14 15:08:03.474809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/jquery-ui.css
+-rw-r--r--   0        0        0    31521 2022-11-14 15:08:03.543809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/jquery-ui.min.css
+-rw-r--r--   0        0        0    18155 2022-11-14 15:08:03.579810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/theme.css
+-rw-r--r--   0        0        0      376 2022-11-14 15:08:03.766810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_glass_100_f8f8f8_1x400.png
+-rw-r--r--   0        0        0      375 2022-11-14 15:08:03.767810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_glass_35_dddddd_1x400.png
+-rw-r--r--   0        0        0      375 2022-11-14 15:08:03.771810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_glass_60_eeeeee_1x400.png
+-rw-r--r--   0        0        0      362 2022-11-14 15:08:03.785810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_inset-hard_75_999999_1x100.png
+-rw-r--r--   0        0        0      381 2022-11-14 15:08:03.787810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-bg_inset-soft_50_c9c9c9_1x100.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_3383bb_256x240.png
+-rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.793810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_454545_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_70b2e1_256x240.png
+-rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.799810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_999999_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_fbc856_256x240.png
+-rw-r--r--   0        0        0    36646 2022-11-14 15:08:03.477809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/jquery-ui.css
+-rw-r--r--   0        0        0    31288 2022-11-14 15:08:03.544809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/jquery-ui.min.css
+-rw-r--r--   0        0        0    17979 2022-11-14 15:08:03.579810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/theme.css
+-rw-r--r--   0        0        0      406 2022-11-14 15:08:03.752810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_diagonal-maze_20_6e4f1c_10x10.png
+-rw-r--r--   0        0        0      353 2022-11-14 15:08:03.752810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_diagonal-maze_40_000000_10x10.png
+-rw-r--r--   0        0        0    10869 2022-11-14 15:08:03.760810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_10_eceadf_60x60.png
+-rw-r--r--   0        0        0    10014 2022-11-14 15:08:03.762810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_10_f8f7f6_60x60.png
+-rw-r--r--   0        0        0    10639 2022-11-14 15:08:03.763810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_eceadf_60x60.png
+-rw-r--r--   0        0        0    11001 2022-11-14 15:08:03.764810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_f7f3de_60x60.png
+-rw-r--r--   0        0        0     4314 2022-11-14 15:08:03.764810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_ffffff_60x60.png
+-rw-r--r--   0        0        0    14555 2022-11-14 15:08:03.764810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_65_654b24_60x60.png
+-rw-r--r--   0        0        0    11987 2022-11-14 15:08:03.764810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_68_b83400_60x60.png
+-rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_222222_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_3572ac_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.798810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_8c291d_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.802810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_b83400_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_fbdb93_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.817810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36906 2022-11-14 15:08:03.480809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/jquery-ui.css
+-rw-r--r--   0        0        0    31611 2022-11-14 15:08:03.545809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/jquery-ui.min.css
+-rw-r--r--   0        0        0    18239 2022-11-14 15:08:03.580809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/theme.css
+-rw-r--r--   0        0        0      446 2022-11-14 15:08:03.772810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_glass_75_d0e5f5_1x400.png
+-rw-r--r--   0        0        0      451 2022-11-14 15:08:03.773810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_glass_85_dfeffc_1x400.png
+-rw-r--r--   0        0        0      442 2022-11-14 15:08:03.773810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0        0        0     5934 2022-11-14 15:08:03.776810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_gloss-wave_55_5c9ccc_500x100.png
+-rw-r--r--   0        0        0      443 2022-11-14 15:08:03.785810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_inset-hard_100_f5f8f9_1x100.png
+-rw-r--r--   0        0        0      402 2022-11-14 15:08:03.785810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_inset-hard_100_fcfdfd_1x100.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.789810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_217bc0_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_469bdd_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.796810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_6da8d5_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_d8e7f3_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_f9bd01_256x240.png
+-rw-r--r--   0        0        0    36735 2022-11-14 15:08:03.482809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/jquery-ui.css
+-rw-r--r--   0        0        0    31443 2022-11-14 15:08:03.547809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/jquery-ui.min.css
+-rw-r--r--   0        0        0    18068 2022-11-14 15:08:03.581809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/theme.css
+-rw-r--r--   0        0        0      445 2022-11-14 15:08:03.770810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0        0        0      317 2022-11-14 15:08:03.771810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0        0        0      375 2022-11-14 15:08:03.772810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0        0        0      376 2022-11-14 15:08:03.772810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0        0        0      442 2022-11-14 15:08:03.773810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0        0        0      377 2022-11-14 15:08:03.784810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.790810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.791810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0        0        0     7142 2022-11-14 15:08:03.794810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.798810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0        0        0    36662 2022-11-14 15:08:03.486809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/jquery-ui.css
+-rw-r--r--   0        0        0    31340 2022-11-14 15:08:03.548809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/jquery-ui.min.css
+-rw-r--r--   0        0        0    17995 2022-11-14 15:08:03.582810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/theme.css
+-rw-r--r--   0        0        0      443 2022-11-14 15:08:03.771810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_glass_55_fcf0ba_1x400.png
+-rw-r--r--   0        0        0     5869 2022-11-14 15:08:03.773810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_gloss-wave_100_ece8da_500x100.png
+-rw-r--r--   0        0        0      446 2022-11-14 15:08:03.778810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-hard_100_f5f3e5_1x100.png
+-rw-r--r--   0        0        0      431 2022-11-14 15:08:03.779810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-hard_100_fafaf4_1x100.png
+-rw-r--r--   0        0        0      432 2022-11-14 15:08:03.779810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-hard_15_459e00_1x100.png
+-rw-r--r--   0        0        0      369 2022-11-14 15:08:03.780810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-hard_95_cccccc_1x100.png
+-rw-r--r--   0        0        0      463 2022-11-14 15:08:03.782810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-soft_25_67b021_1x100.png
+-rw-r--r--   0        0        0      461 2022-11-14 15:08:03.784810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_highlight-soft_95_ffedad_1x100.png
+-rw-r--r--   0        0        0      432 2022-11-14 15:08:03.786810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_inset-soft_15_2b2922_1x100.png
+-rw-r--r--   0        0        0     7169 2022-11-14 15:08:03.798810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_808080_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.798810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_847e71_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.799810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_8DC262_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0        0        0     7062 2022-11-14 15:08:03.810810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_eeeeee_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.818810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36912 2022-11-14 15:08:03.489809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/jquery-ui.css
+-rw-r--r--   0        0        0    31623 2022-11-14 15:08:03.549809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/jquery-ui.min.css
+-rw-r--r--   0        0        0    18245 2022-11-14 15:08:03.583809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/theme.css
+-rw-r--r--   0        0        0      455 2022-11-14 15:08:03.769810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_glass_45_0078ae_1x400.png
+-rw-r--r--   0        0        0      455 2022-11-14 15:08:03.770810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_glass_55_f8da4e_1x400.png
+-rw-r--r--   0        0        0      458 2022-11-14 15:08:03.772810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_glass_75_79c9ec_1x400.png
+-rw-r--r--   0        0        0     5974 2022-11-14 15:08:03.775810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_45_e14f1c_500x100.png
+-rw-r--r--   0        0        0     6016 2022-11-14 15:08:03.776810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_50_6eac2c_500x100.png
+-rw-r--r--   0        0        0     6087 2022-11-14 15:08:03.777810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_75_2191c0_500x100.png
+-rw-r--r--   0        0        0      402 2022-11-14 15:08:03.785810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_inset-hard_100_fcfdfd_1x100.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_0078ae_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_056b93_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_d8e7f3_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_e0fdff_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_f5e175_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_f7a50d_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_fcd113_256x240.png
+-rw-r--r--   0        0        0    36755 2022-11-14 15:08:03.493809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/jquery-ui.css
+-rw-r--r--   0        0        0    31441 2022-11-14 15:08:03.550809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/jquery-ui.min.css
+-rw-r--r--   0        0        0    18088 2022-11-14 15:08:03.584809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/theme.css
+-rw-r--r--   0        0        0      492 2022-11-14 15:08:03.752810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_diagonals-medium_20_d34d17_40x40.png
+-rw-r--r--   0        0        0     6000 2022-11-14 15:08:03.775810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_45_817865_500x100.png
+-rw-r--r--   0        0        0     5960 2022-11-14 15:08:03.777810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_60_fece2f_500x100.png
+-rw-r--r--   0        0        0     5653 2022-11-14 15:08:03.777810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_70_ffdd57_500x100.png
+-rw-r--r--   0        0        0     5499 2022-11-14 15:08:03.777810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_90_fff9e5_500x100.png
+-rw-r--r--   0        0        0      453 2022-11-14 15:08:03.781810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_highlight-soft_100_feeebd_1x100.png
+-rw-r--r--   0        0        0      313 2022-11-14 15:08:03.787810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_inset-soft_30_ffffff_1x100.png
+-rw-r--r--   0        0        0     7126 2022-11-14 15:08:03.791810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_3d3d3d_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.804810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_bd7b00_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_d19405_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_eb990f_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.810810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_ed9f26_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_fadc7a_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.814810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_ffe180_256x240.png
+-rw-r--r--   0        0        0    36805 2022-11-14 15:08:03.498809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/jquery-ui.css
+-rw-r--r--   0        0        0    31510 2022-11-14 15:08:03.550809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/jquery-ui.min.css
+-rw-r--r--   0        0        0    18138 2022-11-14 15:08:03.585809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/theme.css
+-rw-r--r--   0        0        0      417 2022-11-14 15:08:03.757810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_10_4f4221_10x8.png
+-rw-r--r--   0        0        0      420 2022-11-14 15:08:03.758810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_20_372806_10x8.png
+-rw-r--r--   0        0        0      422 2022-11-14 15:08:03.758810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_25_675423_10x8.png
+-rw-r--r--   0        0        0      423 2022-11-14 15:08:03.758810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_25_d5ac5d_10x8.png
+-rw-r--r--   0        0        0      420 2022-11-14 15:08:03.758810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_8_261803_10x8.png
+-rw-r--r--   0        0        0      420 2022-11-14 15:08:03.758810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_diamond_8_443113_10x8.png
+-rw-r--r--   0        0        0      424 2022-11-14 15:08:03.780810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-bg_highlight-hard_65_fee4bd_1x100.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.788810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_070603_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_e8e2b5_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.809810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_e9cd86_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.810810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_efec9f_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_f2ec64_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.812810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_f9f2bd_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_ff7519_256x240.png
+-rw-r--r--   0        0        0    36812 2022-11-14 15:08:03.504809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/jquery-ui.css
+-rw-r--r--   0        0        0    31541 2022-11-14 15:08:03.551809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/jquery-ui.min.css
+-rw-r--r--   0        0        0    18145 2022-11-14 15:08:03.586809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/theme.css
+-rw-r--r--   0        0        0      373 2022-11-14 15:08:03.754810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_diagonals-small_50_262626_40x40.png
+-rw-r--r--   0        0        0      374 2022-11-14 15:08:03.768810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_glass_40_0a0a0a_1x400.png
+-rw-r--r--   0        0        0      458 2022-11-14 15:08:03.770810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_glass_55_f1fbe5_1x400.png
+-rw-r--r--   0        0        0      375 2022-11-14 15:08:03.771810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_glass_60_000000_1x400.png
+-rw-r--r--   0        0        0     4412 2022-11-14 15:08:03.776810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_55_000000_500x100.png
+-rw-r--r--   0        0        0     6050 2022-11-14 15:08:03.777810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_85_9fda58_500x100.png
+-rw-r--r--   0        0        0     5908 2022-11-14 15:08:03.778810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_95_f6ecd5_500x100.png
+-rw-r--r--   0        0        0     5634 2022-11-14 15:08:03.787810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_000000_256x240.png
+-rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.789810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_1f1f1f_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_9fda58_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.802810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_b8ec79_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.807810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.818810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36792 2022-11-14 15:08:03.513809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/jquery-ui.css
+-rw-r--r--   0        0        0    31488 2022-11-14 15:08:03.552809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/jquery-ui.min.css
+-rw-r--r--   0        0        0    18125 2022-11-14 15:08:03.587809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/theme.css
+-rw-r--r--   0        0        0      370 2022-11-14 15:08:03.767810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_glass_20_555555_1x400.png
+-rw-r--r--   0        0        0      452 2022-11-14 15:08:03.767810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_glass_40_0078a3_1x400.png
+-rw-r--r--   0        0        0      426 2022-11-14 15:08:03.768810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_glass_40_ffc73d_1x400.png
+-rw-r--r--   0        0        0     4028 2022-11-14 15:08:03.774810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_gloss-wave_25_333333_500x100.png
+-rw-r--r--   0        0        0      387 2022-11-14 15:08:03.784810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_highlight-soft_80_eeeeee_1x100.png
+-rw-r--r--   0        0        0      364 2022-11-14 15:08:03.786810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_inset-soft_25_000000_1x100.png
+-rw-r--r--   0        0        0      450 2022-11-14 15:08:03.786810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_inset-soft_30_f58400_1x100.png
+-rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.790810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.794810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_4b8e0b_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.800810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_a83300_256x240.png
+-rw-r--r--   0        0        0     7086 2022-11-14 15:08:03.806810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_cccccc_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.818810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36760 2022-11-14 15:08:03.517809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/jquery-ui.css
+-rw-r--r--   0        0        0    31408 2022-11-14 15:08:03.555809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/jquery-ui.min.css
+-rw-r--r--   0        0        0    18093 2022-11-14 15:08:03.588809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/theme.css
+-rw-r--r--   0        0        0      528 2022-11-14 15:08:03.755810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_diagonals-thick_18_b81900_40x40.png
+-rw-r--r--   0        0        0      436 2022-11-14 15:08:03.755810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_diagonals-thick_20_666666_40x40.png
+-rw-r--r--   0        0        0      376 2022-11-14 15:08:03.766810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_glass_100_f6f6f6_1x400.png
+-rw-r--r--   0        0        0      458 2022-11-14 15:08:03.766810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_glass_100_fdf5ce_1x400.png
+-rw-r--r--   0        0        0      317 2022-11-14 15:08:03.771810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0        0        0     5925 2022-11-14 15:08:03.775810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_gloss-wave_35_f6a828_500x100.png
+-rw-r--r--   0        0        0      394 2022-11-14 15:08:03.781810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_highlight-soft_100_eeeeee_1x100.png
+-rw-r--r--   0        0        0      438 2022-11-14 15:08:03.784810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_highlight-soft_75_ffe45c_1x100.png
+-rw-r--r--   0        0        0     7077 2022-11-14 15:08:03.790810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.790810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_228ef1_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.810810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ef8c08_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.813810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ffd27a_256x240.png
+-rw-r--r--   0        0        0     6539 2022-11-14 15:08:03.819810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    36922 2022-11-14 15:08:03.520809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/jquery-ui.css
+-rw-r--r--   0        0        0    31606 2022-11-14 15:08:03.556809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/jquery-ui.min.css
+-rw-r--r--   0        0        0    18255 2022-11-14 15:08:03.588809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/theme.css
+-rw-r--r--   0        0        0      442 2022-11-14 15:08:03.773810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0        0        0     4083 2022-11-14 15:08:03.774810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_gloss-wave_16_121212_500x100.png
+-rw-r--r--   0        0        0      363 2022-11-14 15:08:03.779810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_highlight-hard_15_888888_1x100.png
+-rw-r--r--   0        0        0      363 2022-11-14 15:08:03.779810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_highlight-hard_55_555555_1x100.png
+-rw-r--r--   0        0        0      378 2022-11-14 15:08:03.783810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_highlight-soft_35_adadad_1x100.png
+-rw-r--r--   0        0        0      394 2022-11-14 15:08:03.784810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_highlight-soft_60_dddddd_1x100.png
+-rw-r--r--   0        0        0      374 2022-11-14 15:08:03.786810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_inset-soft_15_121212_1x100.png
+-rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.795810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_666666_256x240.png
+-rw-r--r--   0        0        0     7163 2022-11-14 15:08:03.797810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     7127 2022-11-14 15:08:03.800810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_aaaaaa_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.805810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_c98000_256x240.png
+-rw-r--r--   0        0        0     7086 2022-11-14 15:08:03.806810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_cccccc_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.808810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0        0        0     4670 2022-11-14 15:08:03.811810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_f29a00_256x240.png
+-rw-r--r--   0        0        0    36802 2022-11-14 15:08:03.524809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/jquery-ui.css
+-rw-r--r--   0        0        0    31448 2022-11-14 15:08:03.557809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/jquery-ui.min.css
+-rw-r--r--   0        0        0    18135 2022-11-14 15:08:03.589810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/theme.css
+-rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.410809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/globalize/LICENSE
+-rw-r--r--   0        0        0     1898 2022-11-14 15:08:03.633810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/globalize/globalize.culture.de-DE.js
+-rw-r--r--   0        0        0     2859 2022-11-14 15:08:03.633810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/globalize/globalize.culture.ja-JP.js
+-rw-r--r--   0        0        0    45705 2022-11-14 15:08:03.633810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/globalize/globalize.js
+-rw-r--r--   0        0        0     1097 2022-11-14 15:08:03.823810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery/LICENSE.txt
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   288580 2022-11-14 15:08:03.741810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.824810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.0/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   273809 2022-11-14 15:08:03.644810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.0/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.824810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.1/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   274080 2022-11-14 15:08:03.650810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.1/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.824810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.2/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   273199 2022-11-14 15:08:03.655810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.2/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.0/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   282944 2022-11-14 15:08:03.658810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.0/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.1/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   282766 2022-11-14 15:08:03.662810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.1/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.2/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   284184 2022-11-14 15:08:03.666810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.2/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.3/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   284394 2022-11-14 15:08:03.671810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.3/jquery.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.819810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.0/LICENSE.txt
+-rw-r--r--   0        0        0   294161 2022-11-14 15:08:03.688810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.0/jquery.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.819810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.1/LICENSE.txt
+-rw-r--r--   0        0        0   294199 2022-11-14 15:08:03.693810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.1/jquery.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.2/LICENSE.txt
+-rw-r--r--   0        0        0   293840 2022-11-14 15:08:03.700810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.2/jquery.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.3/LICENSE.txt
+-rw-r--r--   0        0        0   293650 2022-11-14 15:08:03.702810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.3/jquery.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.4/LICENSE.txt
+-rw-r--r--   0        0        0   293430 2022-11-14 15:08:03.705810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.4/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.0/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   258377 2022-11-14 15:08:03.706810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.0/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.1/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   259996 2022-11-14 15:08:03.707810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.1/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.825810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.2/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   265217 2022-11-14 15:08:03.707810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.2/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.3/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   418275 2022-11-14 15:08:03.709810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.3/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.0/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   267320 2022-11-14 15:08:03.710810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.0/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.1/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   268380 2022-11-14 15:08:03.711810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.1/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.0/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   240196 2022-11-14 15:08:03.711810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.0/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.1/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   242727 2022-11-14 15:08:03.712810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.1/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.2/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   242915 2022-11-14 15:08:03.713810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.2/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.826810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.3/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   242142 2022-11-14 15:08:03.714810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.3/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.0/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   244963 2022-11-14 15:08:03.715810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.0/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.1/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   247351 2022-11-14 15:08:03.715810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.1/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.2/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   247380 2022-11-14 15:08:03.716810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.2/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.3/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   247387 2022-11-14 15:08:03.717810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.3/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.4/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   247597 2022-11-14 15:08:03.718810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.4/jquery.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.0/LICENSE.txt
+-rw-r--r--   0        0        0   258388 2022-11-14 15:08:03.719810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.0/jquery.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.1/LICENSE.txt
+-rw-r--r--   0        0        0   258549 2022-11-14 15:08:03.720810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.1/jquery.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.820810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.2/LICENSE.txt
+-rw-r--r--   0        0        0   258648 2022-11-14 15:08:03.721810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.2/jquery.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.3/LICENSE.txt
+-rw-r--r--   0        0        0   258648 2022-11-14 15:08:03.722810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.3/jquery.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.4/LICENSE.txt
+-rw-r--r--   0        0        0   257551 2022-11-14 15:08:03.723810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.4/jquery.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.0.0/LICENSE.txt
+-rw-r--r--   0        0        0   263268 2022-11-14 15:08:03.723810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.0.0/jquery.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.0/LICENSE.txt
+-rw-r--r--   0        0        0   263767 2022-11-14 15:08:03.724810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.0/jquery.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.821810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.1/LICENSE.txt
+-rw-r--r--   0        0        0   267194 2022-11-14 15:08:03.725810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.1/jquery.js
+-rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.821810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.0/LICENSE.txt
+-rw-r--r--   0        0        0   267686 2022-11-14 15:08:03.726810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.0/jquery.js
+-rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.821810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.1/LICENSE.txt
+-rw-r--r--   0        0        0   268039 2022-11-14 15:08:03.727810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.1/jquery.js
+-rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.822810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.0/LICENSE.txt
+-rw-r--r--   0        0        0   271751 2022-11-14 15:08:03.728810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.0/jquery.js
+-rw-r--r--   0        0        0     1605 2022-11-14 15:08:03.822810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.1/LICENSE.txt
+-rw-r--r--   0        0        0   271751 2022-11-14 15:08:03.728810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.1/jquery.js
+-rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.822810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.0/LICENSE.txt
+-rw-r--r--   0        0        0   279860 2022-11-14 15:08:03.729810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.0/jquery.js
+-rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.822810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.1/LICENSE.txt
+-rw-r--r--   0        0        0   280364 2022-11-14 15:08:03.730810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.1/jquery.js
+-rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.822810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.0/LICENSE.txt
+-rw-r--r--   0        0        0   287649 2022-11-14 15:08:03.734810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.0/jquery.js
+-rw-r--r--   0        0        0     1095 2022-11-14 15:08:03.822810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.1/LICENSE.txt
+-rw-r--r--   0        0        0   287630 2022-11-14 15:08:03.735810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.1/jquery.js
+-rw-r--r--   0        0        0     1097 2022-11-14 15:08:03.822810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.6.0/LICENSE.txt
+-rw-r--r--   0        0        0   288580 2022-11-14 15:08:03.737810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.6.0/jquery.js
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.827810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-custom/MIT-LICENSE.txt
+-rw-r--r--   0        0        0   283248 2022-11-14 15:08:03.739810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-custom/jquery.js
+-rw-r--r--   0        0        0     1614 2022-11-14 15:08:03.822810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-1.4.1/LICENSE.txt
+-rw-r--r--   0        0        0    23497 2022-11-14 15:08:03.634810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-1.4.1/jquery-migrate.js
+-rw-r--r--   0        0        0     1615 2022-11-14 15:08:03.823810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-3.3.2/LICENSE.txt
+-rw-r--r--   0        0        0    25300 2022-11-14 15:08:03.635810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-3.3.2/jquery-migrate.js
+-rw-r--r--   0        0        0     1084 2022-11-14 15:08:03.823810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-mousewheel/LICENSE.txt
+-rw-r--r--   0        0        0     8279 2022-11-14 15:08:03.741810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-mousewheel/jquery.mousewheel.js
+-rw-r--r--   0        0        0     1615 2022-11-14 15:08:03.823810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-simulate/LICENSE.txt
+-rw-r--r--   0        0        0     8710 2022-11-14 15:08:03.742810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-simulate/jquery.simulate.js
+-rw-r--r--   0        0        0     1590 2022-11-14 15:08:03.824810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit/LICENSE.txt
+-rw-r--r--   0        0        0     1099 2022-11-14 15:08:03.828810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit/MIT-LICENSE.txt
+-rw-r--r--   0        0        0     5146 2022-11-14 15:08:03.560809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit/qunit.css
+-rw-r--r--   0        0        0   115758 2022-11-14 15:08:03.746810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit/qunit.js
+-rw-r--r--   0        0        0     1085 2022-11-14 15:08:03.823810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-classes/LICENSE.txt
+-rw-r--r--   0        0        0     5295 2022-11-14 15:08:03.744810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-classes/qunit-assert-classes.js
+-rw-r--r--   0        0        0     1094 2022-11-14 15:08:03.828810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-close/MIT-LICENSE.txt
+-rw-r--r--   0        0        0     4181 2022-11-14 15:08:03.745810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-close/qunit-assert-close.js
+-rw-r--r--   0        0        0     1606 2022-11-14 15:08:03.823810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit-composite/LICENSE.txt
+-rw-r--r--   0        0        0      196 2022-11-14 15:08:03.559809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit-composite/qunit-composite.css
+-rw-r--r--   0        0        0     4768 2022-11-14 15:08:03.745810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit-composite/qunit-composite.js
+-rw-r--r--   0        0        0    83083 2022-11-14 15:08:03.746810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/requirejs/require.js
+-rw-r--r--   0        0        0     1812 2022-11-14 15:08:03.751810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/package.json
+-rw-r--r--   0        0        0      489 2022-11-14 15:08:03.414809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/accordion.css
+-rw-r--r--   0        0        0      275 2022-11-14 15:08:03.415809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/all.css
+-rw-r--r--   0        0        0      316 2022-11-14 15:08:03.415809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/autocomplete.css
+-rw-r--r--   0        0        0      791 2022-11-14 15:08:03.417809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/base.css
+-rw-r--r--   0        0        0     1497 2022-11-14 15:08:03.417809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/button.css
+-rw-r--r--   0        0        0      789 2022-11-14 15:08:03.418809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/checkboxradio.css
+-rw-r--r--   0        0        0     1526 2022-11-14 15:08:03.419809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/controlgroup.css
+-rw-r--r--   0        0        0     1581 2022-11-14 15:08:03.419809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/core.css
+-rw-r--r--   0        0        0     3788 2022-11-14 15:08:03.420809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/datepicker.css
+-rw-r--r--   0        0        0     1753 2022-11-14 15:08:03.420809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/dialog.css
+-rw-r--r--   0        0        0      253 2022-11-14 15:08:03.421809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/draggable.css
+-rw-r--r--   0        0        0       86 2022-11-14 15:08:03.765810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-r--r--   0        0        0     3266 2022-11-14 15:08:03.792810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     3274 2022-11-14 15:08:03.795810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     3262 2022-11-14 15:08:03.797810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     3266 2022-11-14 15:08:03.797810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     3262 2022-11-14 15:08:03.806810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     3264 2022-11-14 15:08:03.819810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0     1124 2022-11-14 15:08:03.557809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/menu.css
+-rw-r--r--   0        0        0     2952 2022-11-14 15:08:03.558809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/progressbar.css
+-rw-r--r--   0        0        0     1198 2022-11-14 15:08:03.561809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/resizable.css
+-rw-r--r--   0        0        0      337 2022-11-14 15:08:03.562809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/selectable.css
+-rw-r--r--   0        0        0      916 2022-11-14 15:08:03.563809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/selectmenu.css
+-rw-r--r--   0        0        0     1359 2022-11-14 15:08:03.563809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/slider.css
+-rw-r--r--   0        0        0      251 2022-11-14 15:08:03.564809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/sortable.css
+-rw-r--r--   0        0        0      964 2022-11-14 15:08:03.564809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/spinner.css
+-rw-r--r--   0        0        0     1217 2022-11-14 15:08:03.565809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/tabs.css
+-rw-r--r--   0        0        0    18128 2022-11-14 15:08:03.590809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/theme.css
+-rw-r--r--   0        0        0      355 2022-11-14 15:08:03.591809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/tooltip.css
+-rw-r--r--   0        0        0      361 2022-11-14 15:08:03.596809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/core.js
+-rw-r--r--   0        0        0      934 2022-11-14 15:08:03.597809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/data.js
+-rw-r--r--   0        0        0     1079 2022-11-14 15:08:03.623810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/disable-selection.js
+-rw-r--r--   0        0        0    24612 2022-11-14 15:08:03.629810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effect.js
+-rw-r--r--   0        0        0     1640 2022-11-14 15:08:03.624810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-blind.js
+-rw-r--r--   0        0        0     2656 2022-11-14 15:08:03.624810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-bounce.js
+-rw-r--r--   0        0        0     1573 2022-11-14 15:08:03.625810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-clip.js
+-rw-r--r--   0        0        0     1591 2022-11-14 15:08:03.625810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-drop.js
+-rw-r--r--   0        0        0     2920 2022-11-14 15:08:03.625810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-explode.js
+-rw-r--r--   0        0        0      964 2022-11-14 15:08:03.625810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-fade.js
+-rw-r--r--   0        0        0     2181 2022-11-14 15:08:03.625810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-fold.js
+-rw-r--r--   0        0        0     1239 2022-11-14 15:08:03.626810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-highlight.js
+-rw-r--r--   0        0        0      991 2022-11-14 15:08:03.626810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-puff.js
+-rw-r--r--   0        0        0     1563 2022-11-14 15:08:03.626810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-pulsate.js
+-rw-r--r--   0        0        0     1369 2022-11-14 15:08:03.626810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-scale.js
+-rw-r--r--   0        0        0     1880 2022-11-14 15:08:03.628810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-shake.js
+-rw-r--r--   0        0        0     5414 2022-11-14 15:08:03.628810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-size.js
+-rw-r--r--   0        0        0     1963 2022-11-14 15:08:03.628810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-slide.js
+-rw-r--r--   0        0        0      884 2022-11-14 15:08:03.628810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-transfer.js
+-rw-r--r--   0        0        0     2295 2022-11-14 15:08:03.629810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/focusable.js
+-rw-r--r--   0        0        0     1827 2022-11-14 15:08:03.629810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/form-reset-mixin.js
+-rw-r--r--   0        0        0      581 2022-11-14 15:08:03.629810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/form.js
+-rw-r--r--   0        0        0     1207 2022-11-14 15:08:03.597809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-af.js
+-rw-r--r--   0        0        0     1532 2022-11-14 15:08:03.597809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ar-DZ.js
+-rw-r--r--   0        0        0     1499 2022-11-14 15:08:03.598810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ar.js
+-rw-r--r--   0        0        0     1241 2022-11-14 15:08:03.598810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-az.js
+-rw-r--r--   0        0        0     1467 2022-11-14 15:08:03.598810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-be.js
+-rw-r--r--   0        0        0     1444 2022-11-14 15:08:03.599810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-bg.js
+-rw-r--r--   0        0        0     1183 2022-11-14 15:08:03.599810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-bs.js
+-rw-r--r--   0        0        0     1207 2022-11-14 15:08:03.599810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ca.js
+-rw-r--r--   0        0        0     1232 2022-11-14 15:08:03.599810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-cs.js
+-rw-r--r--   0        0        0     1248 2022-11-14 15:08:03.599810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-cy-GB.js
+-rw-r--r--   0        0        0     1212 2022-11-14 15:08:03.600809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-da.js
+-rw-r--r--   0        0        0     1227 2022-11-14 15:08:03.600809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-de-AT.js
+-rw-r--r--   0        0        0     1202 2022-11-14 15:08:03.600809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-de.js
+-rw-r--r--   0        0        0     1521 2022-11-14 15:08:03.600809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-el.js
+-rw-r--r--   0        0        0     1226 2022-11-14 15:08:03.600809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-AU.js
+-rw-r--r--   0        0        0     1203 2022-11-14 15:08:03.601810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-GB.js
+-rw-r--r--   0        0        0     1228 2022-11-14 15:08:03.601810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-NZ.js
+-rw-r--r--   0        0        0     1214 2022-11-14 15:08:03.601810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-eo.js
+-rw-r--r--   0        0        0     1209 2022-11-14 15:08:03.601810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-es.js
+-rw-r--r--   0        0        0     1277 2022-11-14 15:08:03.601810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-et.js
+-rw-r--r--   0        0        0     1164 2022-11-14 15:08:03.601810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-eu.js
+-rw-r--r--   0        0        0     1420 2022-11-14 15:08:03.602810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fa.js
+-rw-r--r--   0        0        0     1266 2022-11-14 15:08:03.602810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fi.js
+-rw-r--r--   0        0        0     1254 2022-11-14 15:08:03.602810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fo.js
+-rw-r--r--   0        0        0     1221 2022-11-14 15:08:03.602810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr-CA.js
+-rw-r--r--   0        0        0     1258 2022-11-14 15:08:03.603809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr-CH.js
+-rw-r--r--   0        0        0     1341 2022-11-14 15:08:03.604810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr.js
+-rw-r--r--   0        0        0     1211 2022-11-14 15:08:03.604810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-gl.js
+-rw-r--r--   0        0        0     1325 2022-11-14 15:08:03.604810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-he.js
+-rw-r--r--   0        0        0     1618 2022-11-14 15:08:03.604810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hi.js
+-rw-r--r--   0        0        0     1208 2022-11-14 15:08:03.604810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hr.js
+-rw-r--r--   0        0        0     1187 2022-11-14 15:08:03.605810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hu.js
+-rw-r--r--   0        0        0     1495 2022-11-14 15:08:03.605810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hy.js
+-rw-r--r--   0        0        0     1266 2022-11-14 15:08:03.605810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-id.js
+-rw-r--r--   0        0        0     1281 2022-11-14 15:08:03.605810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-is.js
+-rw-r--r--   0        0        0     1257 2022-11-14 15:08:03.605810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-it-CH.js
+-rw-r--r--   0        0        0     1233 2022-11-14 15:08:03.606809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-it.js
+-rw-r--r--   0        0        0     1223 2022-11-14 15:08:03.606809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ja.js
+-rw-r--r--   0        0        0     1761 2022-11-14 15:08:03.606809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ka.js
+-rw-r--r--   0        0        0     1438 2022-11-14 15:08:03.606809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-kk.js
+-rw-r--r--   0        0        0     1645 2022-11-14 15:08:03.608810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-km.js
+-rw-r--r--   0        0        0     1264 2022-11-14 15:08:03.609809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ko.js
+-rw-r--r--   0        0        0     1416 2022-11-14 15:08:03.609809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ky.js
+-rw-r--r--   0        0        0     1260 2022-11-14 15:08:03.609809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lb.js
+-rw-r--r--   0        0        0     1297 2022-11-14 15:08:03.609809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lt.js
+-rw-r--r--   0        0        0     1290 2022-11-14 15:08:03.610809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lv.js
+-rw-r--r--   0        0        0     1408 2022-11-14 15:08:03.610809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-mk.js
+-rw-r--r--   0        0        0     1747 2022-11-14 15:08:03.610809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ml.js
+-rw-r--r--   0        0        0     1212 2022-11-14 15:08:03.611810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ms.js
+-rw-r--r--   0        0        0     1244 2022-11-14 15:08:03.612810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nb.js
+-rw-r--r--   0        0        0     1238 2022-11-14 15:08:03.612810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nl-BE.js
+-rw-r--r--   0        0        0     1230 2022-11-14 15:08:03.612810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nl.js
+-rw-r--r--   0        0        0     1241 2022-11-14 15:08:03.613809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nn.js
+-rw-r--r--   0        0        0     1236 2022-11-14 15:08:03.613809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-no.js
+-rw-r--r--   0        0        0     1238 2022-11-14 15:08:03.614810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pl.js
+-rw-r--r--   0        0        0     1299 2022-11-14 15:08:03.614810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pt-BR.js
+-rw-r--r--   0        0        0     1216 2022-11-14 15:08:03.615810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pt.js
+-rw-r--r--   0        0        0     1278 2022-11-14 15:08:03.615810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-rm.js
+-rw-r--r--   0        0        0     1287 2022-11-14 15:08:03.615810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ro.js
+-rw-r--r--   0        0        0     1438 2022-11-14 15:08:03.615810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ru.js
+-rw-r--r--   0        0        0     1226 2022-11-14 15:08:03.616809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sk.js
+-rw-r--r--   0        0        0     1264 2022-11-14 15:08:03.617810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sl.js
+-rw-r--r--   0        0        0     1208 2022-11-14 15:08:03.617810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sq.js
+-rw-r--r--   0        0        0     1205 2022-11-14 15:08:03.617810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sr-SR.js
+-rw-r--r--   0        0        0     1390 2022-11-14 15:08:03.618810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sr.js
+-rw-r--r--   0        0        0     1222 2022-11-14 15:08:03.618810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sv.js
+-rw-r--r--   0        0        0     1859 2022-11-14 15:08:03.618810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ta.js
+-rw-r--r--   0        0        0     1583 2022-11-14 15:08:03.619809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-th.js
+-rw-r--r--   0        0        0     1395 2022-11-14 15:08:03.619809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-tj.js
+-rw-r--r--   0        0        0     1205 2022-11-14 15:08:03.619809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-tr.js
+-rw-r--r--   0        0        0     1544 2022-11-14 15:08:03.620810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-uk.js
+-rw-r--r--   0        0        0     1377 2022-11-14 15:08:03.620810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-vi.js
+-rw-r--r--   0        0        0     1322 2022-11-14 15:08:03.621810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-CN.js
+-rw-r--r--   0        0        0     1320 2022-11-14 15:08:03.621810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-HK.js
+-rw-r--r--   0        0        0     1322 2022-11-14 15:08:03.621810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-TW.js
+-rw-r--r--   0        0        0      385 2022-11-14 15:08:03.633810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/ie.js
+-rw-r--r--   0        0        0     2168 2022-11-14 15:08:03.635810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/jquery-patch.js
+-rw-r--r--   0        0        0      530 2022-11-14 15:08:03.640810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/jquery-var-for-color.js
+-rw-r--r--   0        0        0      820 2022-11-14 15:08:03.742810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/keycode.js
+-rw-r--r--   0        0        0     1775 2022-11-14 15:08:03.742810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/labels.js
+-rw-r--r--   0        0        0     1020 2022-11-14 15:08:03.743810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/plugin.js
+-rw-r--r--   0        0        0    15125 2022-11-14 15:08:03.743810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/position.js
+-rw-r--r--   0        0        0     1014 2022-11-14 15:08:03.747810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/safe-active-element.js
+-rw-r--r--   0        0        0      523 2022-11-14 15:08:03.747810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/safe-blur.js
+-rw-r--r--   0        0        0     1280 2022-11-14 15:08:03.747810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/scroll-parent.js
+-rw-r--r--   0        0        0      883 2022-11-14 15:08:03.749810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/tabbable.js
+-rw-r--r--   0        0        0      976 2022-11-14 15:08:03.750810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/unique-id.js
+-rw-r--r--   0        0        0     1811 2022-11-14 15:08:03.824810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/vendor/jquery-color/LICENSE.txt
+-rw-r--r--   0        0        0    17418 2022-11-14 15:08:03.641810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/vendor/jquery-color/jquery.color.js
+-rw-r--r--   0        0        0      322 2022-11-14 15:08:03.750810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/version.js
+-rw-r--r--   0        0        0    20283 2022-11-14 15:08:03.751810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widget.js
+-rw-r--r--   0        0        0    16134 2022-11-14 15:08:03.592810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/accordion.js
+-rw-r--r--   0        0        0    17526 2022-11-14 15:08:03.593809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/autocomplete.js
+-rw-r--r--   0        0        0    11702 2022-11-14 15:08:03.594809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/button.js
+-rw-r--r--   0        0        0     7585 2022-11-14 15:08:03.594809 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/checkboxradio.js
+-rw-r--r--   0        0        0     8622 2022-11-14 15:08:03.595810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/controlgroup.js
+-rw-r--r--   0        0        0    82518 2022-11-14 15:08:03.622810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/datepicker.js
+-rw-r--r--   0        0        0    23738 2022-11-14 15:08:03.622810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/dialog.js
+-rw-r--r--   0        0        0    35541 2022-11-14 15:08:03.623810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/draggable.js
+-rw-r--r--   0        0        0    12895 2022-11-14 15:08:03.624810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/droppable.js
+-rw-r--r--   0        0        0    18956 2022-11-14 15:08:03.743810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/menu.js
+-rw-r--r--   0        0        0     6224 2022-11-14 15:08:03.743810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/mouse.js
+-rw-r--r--   0        0        0     4235 2022-11-14 15:08:03.744810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/progressbar.js
+-rw-r--r--   0        0        0    30395 2022-11-14 15:08:03.747810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/resizable.js
+-rw-r--r--   0        0        0     8125 2022-11-14 15:08:03.748810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/selectable.js
+-rw-r--r--   0        0        0    16249 2022-11-14 15:08:03.748810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/selectmenu.js
+-rw-r--r--   0        0        0    19595 2022-11-14 15:08:03.748810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/slider.js
+-rw-r--r--   0        0        0    47637 2022-11-14 15:08:03.749810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/sortable.js
+-rw-r--r--   0        0        0    14430 2022-11-14 15:08:03.749810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/spinner.js
+-rw-r--r--   0        0        0    23658 2022-11-14 15:08:03.750810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/tabs.js
+-rw-r--r--   0        0        0    14472 2022-11-14 15:08:03.750810 anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/tooltip.js
+-rw-r--r--   0        0        0    45726 2022-11-14 15:08:03.705810 anitya-1.8.0/anitya/static/node_modules/moment/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2022-11-14 15:08:03.408809 anitya-1.8.0/anitya/static/node_modules/moment/LICENSE
+-rw-r--r--   0        0        0     2468 2022-11-14 15:08:03.705810 anitya-1.8.0/anitya/static/node_modules/moment/README.md
+-rw-r--r--   0        0        0     2149 2022-11-14 15:08:03.420809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/af.js
+-rw-r--r--   0        0        0     4449 2022-11-14 15:08:03.427809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar-dz.js
+-rw-r--r--   0        0        0     1934 2022-11-14 15:08:03.428809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar-kw.js
+-rw-r--r--   0        0        0     4648 2022-11-14 15:08:03.429809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar-ly.js
+-rw-r--r--   0        0        0     1989 2022-11-14 15:08:03.433809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar-ma.js
+-rw-r--r--   0        0        0     3042 2022-11-14 15:08:03.436809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar-sa.js
+-rw-r--r--   0        0        0     1936 2022-11-14 15:08:03.439809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar-tn.js
+-rw-r--r--   0        0        0     5072 2022-11-14 15:08:03.440809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar.js
+-rw-r--r--   0        0        0     2846 2022-11-14 15:08:03.448809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/az.js
+-rw-r--r--   0        0        0     5154 2022-11-14 15:08:03.452809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/be.js
+-rw-r--r--   0        0        0     2955 2022-11-14 15:08:03.455809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/bg.js
+-rw-r--r--   0        0        0     1784 2022-11-14 15:08:03.457809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/bm.js
+-rw-r--r--   0        0        0     4349 2022-11-14 15:08:03.459809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/bn-bd.js
+-rw-r--r--   0        0        0     3898 2022-11-14 15:08:03.461809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/bn.js
+-rw-r--r--   0        0        0     4399 2022-11-14 15:08:03.462809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/bo.js
+-rw-r--r--   0        0        0     4544 2022-11-14 15:08:03.464809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/br.js
+-rw-r--r--   0        0        0     4475 2022-11-14 15:08:03.466809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/bs.js
+-rw-r--r--   0        0        0     3031 2022-11-14 15:08:03.466809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ca.js
+-rw-r--r--   0        0        0     6718 2022-11-14 15:08:03.475809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/cs.js
+-rw-r--r--   0        0        0     2341 2022-11-14 15:08:03.476809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/cv.js
+-rw-r--r--   0        0        0     2834 2022-11-14 15:08:03.477809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/cy.js
+-rw-r--r--   0        0        0     1629 2022-11-14 15:08:03.478809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/da.js
+-rw-r--r--   0        0        0     2635 2022-11-14 15:08:03.480809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/de-at.js
+-rw-r--r--   0        0        0     2563 2022-11-14 15:08:03.482809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/de-ch.js
+-rw-r--r--   0        0        0     2562 2022-11-14 15:08:03.484809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/de.js
+-rw-r--r--   0        0        0     2464 2022-11-14 15:08:03.487809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/dv.js
+-rw-r--r--   0        0        0     3877 2022-11-14 15:08:03.488809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/el.js
+-rw-r--r--   0        0        0     2029 2022-11-14 15:08:03.490809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-au.js
+-rw-r--r--   0        0        0     1878 2022-11-14 15:08:03.491809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-ca.js
+-rw-r--r--   0        0        0     2035 2022-11-14 15:08:03.493809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-gb.js
+-rw-r--r--   0        0        0     2033 2022-11-14 15:08:03.496809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-ie.js
+-rw-r--r--   0        0        0     1871 2022-11-14 15:08:03.498809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-il.js
+-rw-r--r--   0        0        0     2029 2022-11-14 15:08:03.500809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-in.js
+-rw-r--r--   0        0        0     2038 2022-11-14 15:08:03.502809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-nz.js
+-rw-r--r--   0        0        0     2047 2022-11-14 15:08:03.505809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-sg.js
+-rw-r--r--   0        0        0     2338 2022-11-14 15:08:03.512809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/eo.js
+-rw-r--r--   0        0        0     3441 2022-11-14 15:08:03.515809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/es-do.js
+-rw-r--r--   0        0        0     3510 2022-11-14 15:08:03.517809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/es-mx.js
+-rw-r--r--   0        0        0     3538 2022-11-14 15:08:03.519809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/es-us.js
+-rw-r--r--   0        0        0     3498 2022-11-14 15:08:03.521809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/es.js
+-rw-r--r--   0        0        0     2631 2022-11-14 15:08:03.523809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/et.js
+-rw-r--r--   0        0        0     1964 2022-11-14 15:08:03.525809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/eu.js
+-rw-r--r--   0        0        0     3230 2022-11-14 15:08:03.526809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fa.js
+-rw-r--r--   0        0        0     3632 2022-11-14 15:08:03.528809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fi.js
+-rw-r--r--   0        0        0     1776 2022-11-14 15:08:03.530809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fil.js
+-rw-r--r--   0        0        0     1772 2022-11-14 15:08:03.531809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fo.js
+-rw-r--r--   0        0        0     2104 2022-11-14 15:08:03.540809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fr-ca.js
+-rw-r--r--   0        0        0     2263 2022-11-14 15:08:03.542809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fr-ch.js
+-rw-r--r--   0        0        0     3471 2022-11-14 15:08:03.543809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fr.js
+-rw-r--r--   0        0        0     2275 2022-11-14 15:08:03.548809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fy.js
+-rw-r--r--   0        0        0     2360 2022-11-14 15:08:03.549809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ga.js
+-rw-r--r--   0        0        0     2380 2022-11-14 15:08:03.551809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/gd.js
+-rw-r--r--   0        0        0     2347 2022-11-14 15:08:03.552809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/gl.js
+-rw-r--r--   0        0        0     5506 2022-11-14 15:08:03.555809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/gom-deva.js
+-rw-r--r--   0        0        0     4130 2022-11-14 15:08:03.557809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/gom-latn.js
+-rw-r--r--   0        0        0     4132 2022-11-14 15:08:03.559809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/gu.js
+-rw-r--r--   0        0        0     3211 2022-11-14 15:08:03.560809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/he.js
+-rw-r--r--   0        0        0     6421 2022-11-14 15:08:03.562809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/hi.js
+-rw-r--r--   0        0        0     4718 2022-11-14 15:08:03.564809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/hr.js
+-rw-r--r--   0        0        0     3815 2022-11-14 15:08:03.566809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/hu.js
+-rw-r--r--   0        0        0     3236 2022-11-14 15:08:03.568809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/hy-am.js
+-rw-r--r--   0        0        0     2375 2022-11-14 15:08:03.571809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/id.js
+-rw-r--r--   0        0        0     4458 2022-11-14 15:08:03.577809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/is.js
+-rw-r--r--   0        0        0     1941 2022-11-14 15:08:03.578809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/it-ch.js
+-rw-r--r--   0        0        0     3251 2022-11-14 15:08:03.579810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/it.js
+-rw-r--r--   0        0        0     3955 2022-11-14 15:08:03.580809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ja.js
+-rw-r--r--   0        0        0     2384 2022-11-14 15:08:03.582810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/jv.js
+-rw-r--r--   0        0        0     3504 2022-11-14 15:08:03.583809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ka.js
+-rw-r--r--   0        0        0     2495 2022-11-14 15:08:03.584809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/kk.js
+-rw-r--r--   0        0        0     3362 2022-11-14 15:08:03.586809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/km.js
+-rw-r--r--   0        0        0     4252 2022-11-14 15:08:03.587809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/kn.js
+-rw-r--r--   0        0        0     2223 2022-11-14 15:08:03.589810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ko.js
+-rw-r--r--   0        0        0     3330 2022-11-14 15:08:03.590809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ku.js
+-rw-r--r--   0        0        0     2521 2022-11-14 15:08:03.591809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ky.js
+-rw-r--r--   0        0        0     4269 2022-11-14 15:08:03.593809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/lb.js
+-rw-r--r--   0        0        0     2585 2022-11-14 15:08:03.595810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/lo.js
+-rw-r--r--   0        0        0     4005 2022-11-14 15:08:03.610809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/lt.js
+-rw-r--r--   0        0        0     3449 2022-11-14 15:08:03.612810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/lv.js
+-rw-r--r--   0        0        0     3661 2022-11-14 15:08:03.613809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/me.js
+-rw-r--r--   0        0        0     2023 2022-11-14 15:08:03.615810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/mi.js
+-rw-r--r--   0        0        0     3021 2022-11-14 15:08:03.617810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/mk.js
+-rw-r--r--   0        0        0     3287 2022-11-14 15:08:03.619809 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ml.js
+-rw-r--r--   0        0        0     3414 2022-11-14 15:08:03.620810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/mn.js
+-rw-r--r--   0        0        0     6574 2022-11-14 15:08:03.637810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/mr.js
+-rw-r--r--   0        0        0     2330 2022-11-14 15:08:03.637810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ms-my.js
+-rw-r--r--   0        0        0     2277 2022-11-14 15:08:03.638810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ms.js
+-rw-r--r--   0        0        0     1684 2022-11-14 15:08:03.639810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/mt.js
+-rw-r--r--   0        0        0     3094 2022-11-14 15:08:03.639810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/my.js
+-rw-r--r--   0        0        0     1899 2022-11-14 15:08:03.640810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/nb.js
+-rw-r--r--   0        0        0     4031 2022-11-14 15:08:03.640810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ne.js
+-rw-r--r--   0        0        0     3169 2022-11-14 15:08:03.641810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/nl-be.js
+-rw-r--r--   0        0        0     3202 2022-11-14 15:08:03.642810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/nl.js
+-rw-r--r--   0        0        0     1828 2022-11-14 15:08:03.642810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/nn.js
+-rw-r--r--   0        0        0     2472 2022-11-14 15:08:03.643810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/oc-lnc.js
+-rw-r--r--   0        0        0     4198 2022-11-14 15:08:03.644810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/pa-in.js
+-rw-r--r--   0        0        0     4166 2022-11-14 15:08:03.647810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/pl.js
+-rw-r--r--   0        0        0     1854 2022-11-14 15:08:03.649810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/pt-br.js
+-rw-r--r--   0        0        0     1968 2022-11-14 15:08:03.650810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/pt.js
+-rw-r--r--   0        0        0     2319 2022-11-14 15:08:03.652810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ro.js
+-rw-r--r--   0        0        0     8418 2022-11-14 15:08:03.654810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ru.js
+-rw-r--r--   0        0        0     2153 2022-11-14 15:08:03.655810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sd.js
+-rw-r--r--   0        0        0     1849 2022-11-14 15:08:03.655810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/se.js
+-rw-r--r--   0        0        0     2681 2022-11-14 15:08:03.656810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/si.js
+-rw-r--r--   0        0        0     5173 2022-11-14 15:08:03.657810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sk.js
+-rw-r--r--   0        0        0     6115 2022-11-14 15:08:03.657810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sl.js
+-rw-r--r--   0        0        0     1987 2022-11-14 15:08:03.658810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sq.js
+-rw-r--r--   0        0        0     4762 2022-11-14 15:08:03.659810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sr-cyrl.js
+-rw-r--r--   0        0        0     4209 2022-11-14 15:08:03.659810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sr.js
+-rw-r--r--   0        0        0     2572 2022-11-14 15:08:03.660810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ss.js
+-rw-r--r--   0        0        0     2066 2022-11-14 15:08:03.662810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sv.js
+-rw-r--r--   0        0        0     1651 2022-11-14 15:08:03.663810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sw.js
+-rw-r--r--   0        0        0     4800 2022-11-14 15:08:03.663810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ta.js
+-rw-r--r--   0        0        0     3392 2022-11-14 15:08:03.664810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/te.js
+-rw-r--r--   0        0        0     2155 2022-11-14 15:08:03.665810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tet.js
+-rw-r--r--   0        0        0     3604 2022-11-14 15:08:03.666810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tg.js
+-rw-r--r--   0        0        0     2736 2022-11-14 15:08:03.667810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/th.js
+-rw-r--r--   0        0        0     2488 2022-11-14 15:08:03.668810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tk.js
+-rw-r--r--   0        0        0     1735 2022-11-14 15:08:03.669810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tl-ph.js
+-rw-r--r--   0        0        0     3755 2022-11-14 15:08:03.670810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tlh.js
+-rw-r--r--   0        0        0     2927 2022-11-14 15:08:03.672810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tr.js
+-rw-r--r--   0        0        0     3109 2022-11-14 15:08:03.674810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tzl.js
+-rw-r--r--   0        0        0     1691 2022-11-14 15:08:03.674810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tzm-latn.js
+-rw-r--r--   0        0        0     2322 2022-11-14 15:08:03.675810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tzm.js
+-rw-r--r--   0        0        0     3880 2022-11-14 15:08:03.687810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ug-cn.js
+-rw-r--r--   0        0        0     5955 2022-11-14 15:08:03.688810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/uk.js
+-rw-r--r--   0        0        0     2200 2022-11-14 15:08:03.689810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ur.js
+-rw-r--r--   0        0        0     1639 2022-11-14 15:08:03.691810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/uz-latn.js
+-rw-r--r--   0        0        0     1885 2022-11-14 15:08:03.692810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/uz.js
+-rw-r--r--   0        0        0     2430 2022-11-14 15:08:03.693810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/vi.js
+-rw-r--r--   0        0        0     2348 2022-11-14 15:08:03.695810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/x-pseudo.js
+-rw-r--r--   0        0        0     1887 2022-11-14 15:08:03.696810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/yo.js
+-rw-r--r--   0        0        0     3711 2022-11-14 15:08:03.698810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/zh-cn.js
+-rw-r--r--   0        0        0     3116 2022-11-14 15:08:03.700810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/zh-hk.js
+-rw-r--r--   0        0        0     3066 2022-11-14 15:08:03.701810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/zh-mo.js
+-rw-r--r--   0        0        0     3013 2022-11-14 15:08:03.701810 anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/zh-tw.js
+-rw-r--r--   0        0        0   154671 2022-11-14 15:08:03.635810 anitya-1.8.0/anitya/static/node_modules/moment/dist/moment.js
+-rw-r--r--   0        0        0       39 2022-11-14 15:08:03.512809 anitya-1.8.0/anitya/static/node_modules/moment/ender.js
+-rw-r--r--   0        0        0     2753 2022-11-14 15:08:03.421809 anitya-1.8.0/anitya/static/node_modules/moment/locale/af.js
+-rw-r--r--   0        0        0     5377 2022-11-14 15:08:03.427809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ar-dz.js
+-rw-r--r--   0        0        0     2478 2022-11-14 15:08:03.428809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ar-kw.js
+-rw-r--r--   0        0        0     5652 2022-11-14 15:08:03.430809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ar-ly.js
+-rw-r--r--   0        0        0     2533 2022-11-14 15:08:03.435809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ar-ma.js
+-rw-r--r--   0        0        0     3782 2022-11-14 15:08:03.437809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ar-sa.js
+-rw-r--r--   0        0        0     2480 2022-11-14 15:08:03.439809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ar-tn.js
+-rw-r--r--   0        0        0     6136 2022-11-14 15:08:03.440809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ar.js
+-rw-r--r--   0        0        0     3570 2022-11-14 15:08:03.449809 anitya-1.8.0/anitya/static/node_modules/moment/locale/az.js
+-rw-r--r--   0        0        0     6030 2022-11-14 15:08:03.454809 anitya-1.8.0/anitya/static/node_modules/moment/locale/be.js
+-rw-r--r--   0        0        0     3623 2022-11-14 15:08:03.456809 anitya-1.8.0/anitya/static/node_modules/moment/locale/bg.js
+-rw-r--r--   0        0        0     2233 2022-11-14 15:08:03.457809 anitya-1.8.0/anitya/static/node_modules/moment/locale/bm.js
+-rw-r--r--   0        0        0     5177 2022-11-14 15:08:03.460809 anitya-1.8.0/anitya/static/node_modules/moment/locale/bn-bd.js
+-rw-r--r--   0        0        0     4690 2022-11-14 15:08:03.461809 anitya-1.8.0/anitya/static/node_modules/moment/locale/bn.js
+-rw-r--r--   0        0        0     5211 2022-11-14 15:08:03.463809 anitya-1.8.0/anitya/static/node_modules/moment/locale/bo.js
+-rw-r--r--   0        0        0     5520 2022-11-14 15:08:03.465809 anitya-1.8.0/anitya/static/node_modules/moment/locale/br.js
+-rw-r--r--   0        0        0     5387 2022-11-14 15:08:03.466809 anitya-1.8.0/anitya/static/node_modules/moment/locale/bs.js
+-rw-r--r--   0        0        0     3751 2022-11-14 15:08:03.467809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ca.js
+-rw-r--r--   0        0        0     7750 2022-11-14 15:08:03.475809 anitya-1.8.0/anitya/static/node_modules/moment/locale/cs.js
+-rw-r--r--   0        0        0     2913 2022-11-14 15:08:03.476809 anitya-1.8.0/anitya/static/node_modules/moment/locale/cv.js
+-rw-r--r--   0        0        0     3542 2022-11-14 15:08:03.477809 anitya-1.8.0/anitya/static/node_modules/moment/locale/cy.js
+-rw-r--r--   0        0        0     2161 2022-11-14 15:08:03.478809 anitya-1.8.0/anitya/static/node_modules/moment/locale/da.js
+-rw-r--r--   0        0        0     3259 2022-11-14 15:08:03.481809 anitya-1.8.0/anitya/static/node_modules/moment/locale/de-at.js
+-rw-r--r--   0        0        0     3094 2022-11-14 15:08:03.482809 anitya-1.8.0/anitya/static/node_modules/moment/locale/de-ch.js
+-rw-r--r--   0        0        0     3182 2022-11-14 15:08:03.485809 anitya-1.8.0/anitya/static/node_modules/moment/locale/de.js
+-rw-r--r--   0        0        0     3140 2022-11-14 15:08:03.487809 anitya-1.8.0/anitya/static/node_modules/moment/locale/dv.js
+-rw-r--r--   0        0        0     4617 2022-11-14 15:08:03.489809 anitya-1.8.0/anitya/static/node_modules/moment/locale/el.js
+-rw-r--r--   0        0        0     2625 2022-11-14 15:08:03.490809 anitya-1.8.0/anitya/static/node_modules/moment/locale/en-au.js
+-rw-r--r--   0        0        0     2458 2022-11-14 15:08:03.492809 anitya-1.8.0/anitya/static/node_modules/moment/locale/en-ca.js
+-rw-r--r--   0        0        0     2631 2022-11-14 15:08:03.494809 anitya-1.8.0/anitya/static/node_modules/moment/locale/en-gb.js
+-rw-r--r--   0        0        0     2629 2022-11-14 15:08:03.496809 anitya-1.8.0/anitya/static/node_modules/moment/locale/en-ie.js
+-rw-r--r--   0        0        0     2451 2022-11-14 15:08:03.499809 anitya-1.8.0/anitya/static/node_modules/moment/locale/en-il.js
+-rw-r--r--   0        0        0     2625 2022-11-14 15:08:03.501809 anitya-1.8.0/anitya/static/node_modules/moment/locale/en-in.js
+-rw-r--r--   0        0        0     2634 2022-11-14 15:08:03.503809 anitya-1.8.0/anitya/static/node_modules/moment/locale/en-nz.js
+-rw-r--r--   0        0        0     2643 2022-11-14 15:08:03.509809 anitya-1.8.0/anitya/static/node_modules/moment/locale/en-sg.js
+-rw-r--r--   0        0        0     2918 2022-11-14 15:08:03.513809 anitya-1.8.0/anitya/static/node_modules/moment/locale/eo.js
+-rw-r--r--   0        0        0     4197 2022-11-14 15:08:03.516809 anitya-1.8.0/anitya/static/node_modules/moment/locale/es-do.js
+-rw-r--r--   0        0        0     4270 2022-11-14 15:08:03.518809 anitya-1.8.0/anitya/static/node_modules/moment/locale/es-mx.js
+-rw-r--r--   0        0        0     4294 2022-11-14 15:08:03.520809 anitya-1.8.0/anitya/static/node_modules/moment/locale/es-us.js
+-rw-r--r--   0        0        0     4254 2022-11-14 15:08:03.522809 anitya-1.8.0/anitya/static/node_modules/moment/locale/es.js
+-rw-r--r--   0        0        0     3255 2022-11-14 15:08:03.524809 anitya-1.8.0/anitya/static/node_modules/moment/locale/et.js
+-rw-r--r--   0        0        0     2544 2022-11-14 15:08:03.525809 anitya-1.8.0/anitya/static/node_modules/moment/locale/eu.js
+-rw-r--r--   0        0        0     3998 2022-11-14 15:08:03.527809 anitya-1.8.0/anitya/static/node_modules/moment/locale/fa.js
+-rw-r--r--   0        0        0     4444 2022-11-14 15:08:03.529809 anitya-1.8.0/anitya/static/node_modules/moment/locale/fi.js
+-rw-r--r--   0        0        0     2326 2022-11-14 15:08:03.530809 anitya-1.8.0/anitya/static/node_modules/moment/locale/fil.js
+-rw-r--r--   0        0        0     2316 2022-11-14 15:08:03.534809 anitya-1.8.0/anitya/static/node_modules/moment/locale/fo.js
+-rw-r--r--   0        0        0     2704 2022-11-14 15:08:03.541809 anitya-1.8.0/anitya/static/node_modules/moment/locale/fr-ca.js
+-rw-r--r--   0        0        0     2879 2022-11-14 15:08:03.542809 anitya-1.8.0/anitya/static/node_modules/moment/locale/fr-ch.js
+-rw-r--r--   0        0        0     4211 2022-11-14 15:08:03.544809 anitya-1.8.0/anitya/static/node_modules/moment/locale/fr.js
+-rw-r--r--   0        0        0     2891 2022-11-14 15:08:03.549809 anitya-1.8.0/anitya/static/node_modules/moment/locale/fy.js
+-rw-r--r--   0        0        0     3056 2022-11-14 15:08:03.550809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ga.js
+-rw-r--r--   0        0        0     3076 2022-11-14 15:08:03.551809 anitya-1.8.0/anitya/static/node_modules/moment/locale/gd.js
+-rw-r--r--   0        0        0     2967 2022-11-14 15:08:03.552809 anitya-1.8.0/anitya/static/node_modules/moment/locale/gl.js
+-rw-r--r--   0        0        0     6336 2022-11-14 15:08:03.556809 anitya-1.8.0/anitya/static/node_modules/moment/locale/gom-deva.js
+-rw-r--r--   0        0        0     4952 2022-11-14 15:08:03.558809 anitya-1.8.0/anitya/static/node_modules/moment/locale/gom-latn.js
+-rw-r--r--   0        0        0     4936 2022-11-14 15:08:03.559809 anitya-1.8.0/anitya/static/node_modules/moment/locale/gu.js
+-rw-r--r--   0        0        0     3899 2022-11-14 15:08:03.560809 anitya-1.8.0/anitya/static/node_modules/moment/locale/he.js
+-rw-r--r--   0        0        0     7385 2022-11-14 15:08:03.562809 anitya-1.8.0/anitya/static/node_modules/moment/locale/hi.js
+-rw-r--r--   0        0        0     5658 2022-11-14 15:08:03.565809 anitya-1.8.0/anitya/static/node_modules/moment/locale/hr.js
+-rw-r--r--   0        0        0     4599 2022-11-14 15:08:03.566809 anitya-1.8.0/anitya/static/node_modules/moment/locale/hu.js
+-rw-r--r--   0        0        0     3936 2022-11-14 15:08:03.569809 anitya-1.8.0/anitya/static/node_modules/moment/locale/hy-am.js
+-rw-r--r--   0        0        0     2995 2022-11-14 15:08:03.571809 anitya-1.8.0/anitya/static/node_modules/moment/locale/id.js
+-rw-r--r--   0        0        0     5334 2022-11-14 15:08:03.577809 anitya-1.8.0/anitya/static/node_modules/moment/locale/is.js
+-rw-r--r--   0        0        0     2521 2022-11-14 15:08:03.578809 anitya-1.8.0/anitya/static/node_modules/moment/locale/it-ch.js
+-rw-r--r--   0        0        0     3987 2022-11-14 15:08:03.579810 anitya-1.8.0/anitya/static/node_modules/moment/locale/it.js
+-rw-r--r--   0        0        0     4867 2022-11-14 15:08:03.581809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ja.js
+-rw-r--r--   0        0        0     3004 2022-11-14 15:08:03.582810 anitya-1.8.0/anitya/static/node_modules/moment/locale/jv.js
+-rw-r--r--   0        0        0     4192 2022-11-14 15:08:03.583809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ka.js
+-rw-r--r--   0        0        0     3139 2022-11-14 15:08:03.585809 anitya-1.8.0/anitya/static/node_modules/moment/locale/kk.js
+-rw-r--r--   0        0        0     4090 2022-11-14 15:08:03.586809 anitya-1.8.0/anitya/static/node_modules/moment/locale/km.js
+-rw-r--r--   0        0        0     5064 2022-11-14 15:08:03.588809 anitya-1.8.0/anitya/static/node_modules/moment/locale/kn.js
+-rw-r--r--   0        0        0     2839 2022-11-14 15:08:03.589810 anitya-1.8.0/anitya/static/node_modules/moment/locale/ko.js
+-rw-r--r--   0        0        0     4118 2022-11-14 15:08:03.590809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ku.js
+-rw-r--r--   0        0        0     3173 2022-11-14 15:08:03.591809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ky.js
+-rw-r--r--   0        0        0     5129 2022-11-14 15:08:03.593809 anitya-1.8.0/anitya/static/node_modules/moment/locale/lb.js
+-rw-r--r--   0        0        0     3169 2022-11-14 15:08:03.595810 anitya-1.8.0/anitya/static/node_modules/moment/locale/lo.js
+-rw-r--r--   0        0        0     4825 2022-11-14 15:08:03.610809 anitya-1.8.0/anitya/static/node_modules/moment/locale/lt.js
+-rw-r--r--   0        0        0     4137 2022-11-14 15:08:03.612810 anitya-1.8.0/anitya/static/node_modules/moment/locale/lv.js
+-rw-r--r--   0        0        0     4441 2022-11-14 15:08:03.614810 anitya-1.8.0/anitya/static/node_modules/moment/locale/me.js
+-rw-r--r--   0        0        0     2583 2022-11-14 15:08:03.615810 anitya-1.8.0/anitya/static/node_modules/moment/locale/mi.js
+-rw-r--r--   0        0        0     3682 2022-11-14 15:08:03.618810 anitya-1.8.0/anitya/static/node_modules/moment/locale/mk.js
+-rw-r--r--   0        0        0     3935 2022-11-14 15:08:03.619809 anitya-1.8.0/anitya/static/node_modules/moment/locale/ml.js
+-rw-r--r--   0        0        0     4130 2022-11-14 15:08:03.621810 anitya-1.8.0/anitya/static/node_modules/moment/locale/mn.js
+-rw-r--r--   0        0        0     7694 2022-11-14 15:08:03.637810 anitya-1.8.0/anitya/static/node_modules/moment/locale/mr.js
+-rw-r--r--   0        0        0     2954 2022-11-14 15:08:03.638810 anitya-1.8.0/anitya/static/node_modules/moment/locale/ms-my.js
+-rw-r--r--   0        0        0     2897 2022-11-14 15:08:03.638810 anitya-1.8.0/anitya/static/node_modules/moment/locale/ms.js
+-rw-r--r--   0        0        0     2228 2022-11-14 15:08:03.639810 anitya-1.8.0/anitya/static/node_modules/moment/locale/mt.js
+-rw-r--r--   0        0        0     3762 2022-11-14 15:08:03.639810 anitya-1.8.0/anitya/static/node_modules/moment/locale/my.js
+-rw-r--r--   0        0        0     2451 2022-11-14 15:08:03.640810 anitya-1.8.0/anitya/static/node_modules/moment/locale/nb.js
+-rw-r--r--   0        0        0     4831 2022-11-14 15:08:03.641810 anitya-1.8.0/anitya/static/node_modules/moment/locale/ne.js
+-rw-r--r--   0        0        0     3881 2022-11-14 15:08:03.641810 anitya-1.8.0/anitya/static/node_modules/moment/locale/nl-be.js
+-rw-r--r--   0        0        0     3918 2022-11-14 15:08:03.642810 anitya-1.8.0/anitya/static/node_modules/moment/locale/nl.js
+-rw-r--r--   0        0        0     2380 2022-11-14 15:08:03.642810 anitya-1.8.0/anitya/static/node_modules/moment/locale/nn.js
+-rw-r--r--   0        0        0     3138 2022-11-14 15:08:03.643810 anitya-1.8.0/anitya/static/node_modules/moment/locale/oc-lnc.js
+-rw-r--r--   0        0        0     5006 2022-11-14 15:08:03.646810 anitya-1.8.0/anitya/static/node_modules/moment/locale/pa-in.js
+-rw-r--r--   0        0        0     5026 2022-11-14 15:08:03.647810 anitya-1.8.0/anitya/static/node_modules/moment/locale/pl.js
+-rw-r--r--   0        0        0     2410 2022-11-14 15:08:03.649810 anitya-1.8.0/anitya/static/node_modules/moment/locale/pt-br.js
+-rw-r--r--   0        0        0     2540 2022-11-14 15:08:03.650810 anitya-1.8.0/anitya/static/node_modules/moment/locale/pt.js
+-rw-r--r--   0        0        0     2931 2022-11-14 15:08:03.652810 anitya-1.8.0/anitya/static/node_modules/moment/locale/ro.js
+-rw-r--r--   0        0        0     9562 2022-11-14 15:08:03.654810 anitya-1.8.0/anitya/static/node_modules/moment/locale/ru.js
+-rw-r--r--   0        0        0     2793 2022-11-14 15:08:03.655810 anitya-1.8.0/anitya/static/node_modules/moment/locale/sd.js
+-rw-r--r--   0        0        0     2397 2022-11-14 15:08:03.655810 anitya-1.8.0/anitya/static/node_modules/moment/locale/se.js
+-rw-r--r--   0        0        0     3277 2022-11-14 15:08:03.656810 anitya-1.8.0/anitya/static/node_modules/moment/locale/si.js
+-rw-r--r--   0        0        0     6065 2022-11-14 15:08:03.657810 anitya-1.8.0/anitya/static/node_modules/moment/locale/sk.js
+-rw-r--r--   0        0        0     7111 2022-11-14 15:08:03.657810 anitya-1.8.0/anitya/static/node_modules/moment/locale/sl.js
+-rw-r--r--   0        0        0     2559 2022-11-14 15:08:03.658810 anitya-1.8.0/anitya/static/node_modules/moment/locale/sq.js
+-rw-r--r--   0        0        0     5578 2022-11-14 15:08:03.659810 anitya-1.8.0/anitya/static/node_modules/moment/locale/sr-cyrl.js
+-rw-r--r--   0        0        0     5025 2022-11-14 15:08:03.660810 anitya-1.8.0/anitya/static/node_modules/moment/locale/sr.js
+-rw-r--r--   0        0        0     3228 2022-11-14 15:08:03.661810 anitya-1.8.0/anitya/static/node_modules/moment/locale/ss.js
+-rw-r--r--   0        0        0     2658 2022-11-14 15:08:03.662810 anitya-1.8.0/anitya/static/node_modules/moment/locale/sv.js
+-rw-r--r--   0        0        0     2191 2022-11-14 15:08:03.663810 anitya-1.8.0/anitya/static/node_modules/moment/locale/sw.js
+-rw-r--r--   0        0        0     5640 2022-11-14 15:08:03.664810 anitya-1.8.0/anitya/static/node_modules/moment/locale/ta.js
+-rw-r--r--   0        0        0     4064 2022-11-14 15:08:03.665810 anitya-1.8.0/anitya/static/node_modules/moment/locale/te.js
+-rw-r--r--   0        0        0     2741 2022-11-14 15:08:03.666810 anitya-1.8.0/anitya/static/node_modules/moment/locale/tet.js
+-rw-r--r--   0        0        0     4388 2022-11-14 15:08:03.667810 anitya-1.8.0/anitya/static/node_modules/moment/locale/tg.js
+-rw-r--r--   0        0        0     3316 2022-11-14 15:08:03.667810 anitya-1.8.0/anitya/static/node_modules/moment/locale/th.js
+-rw-r--r--   0        0        0     3168 2022-11-14 15:08:03.669810 anitya-1.8.0/anitya/static/node_modules/moment/locale/tk.js
+-rw-r--r--   0        0        0     2287 2022-11-14 15:08:03.670810 anitya-1.8.0/anitya/static/node_modules/moment/locale/tl-ph.js
+-rw-r--r--   0        0        0     4553 2022-11-14 15:08:03.670810 anitya-1.8.0/anitya/static/node_modules/moment/locale/tlh.js
+-rw-r--r--   0        0        0     3663 2022-11-14 15:08:03.673810 anitya-1.8.0/anitya/static/node_modules/moment/locale/tr.js
+-rw-r--r--   0        0        0     3779 2022-11-14 15:08:03.674810 anitya-1.8.0/anitya/static/node_modules/moment/locale/tzl.js
+-rw-r--r--   0        0        0     2237 2022-11-14 15:08:03.675810 anitya-1.8.0/anitya/static/node_modules/moment/locale/tzm-latn.js
+-rw-r--r--   0        0        0     2860 2022-11-14 15:08:03.676810 anitya-1.8.0/anitya/static/node_modules/moment/locale/tzm.js
+-rw-r--r--   0        0        0     4644 2022-11-14 15:08:03.688810 anitya-1.8.0/anitya/static/node_modules/moment/locale/ug-cn.js
+-rw-r--r--   0        0        0     6927 2022-11-14 15:08:03.689810 anitya-1.8.0/anitya/static/node_modules/moment/locale/uk.js
+-rw-r--r--   0        0        0     2840 2022-11-14 15:08:03.690810 anitya-1.8.0/anitya/static/node_modules/moment/locale/ur.js
+-rw-r--r--   0        0        0     2183 2022-11-14 15:08:03.691810 anitya-1.8.0/anitya/static/node_modules/moment/locale/uz-latn.js
+-rw-r--r--   0        0        0     2409 2022-11-14 15:08:03.692810 anitya-1.8.0/anitya/static/node_modules/moment/locale/uz.js
+-rw-r--r--   0        0        0     3066 2022-11-14 15:08:03.694810 anitya-1.8.0/anitya/static/node_modules/moment/locale/vi.js
+-rw-r--r--   0        0        0     2970 2022-11-14 15:08:03.695810 anitya-1.8.0/anitya/static/node_modules/moment/locale/x-pseudo.js
+-rw-r--r--   0        0        0     2419 2022-11-14 15:08:03.696810 anitya-1.8.0/anitya/static/node_modules/moment/locale/yo.js
+-rw-r--r--   0        0        0     4507 2022-11-14 15:08:03.699810 anitya-1.8.0/anitya/static/node_modules/moment/locale/zh-cn.js
+-rw-r--r--   0        0        0     3832 2022-11-14 15:08:03.700810 anitya-1.8.0/anitya/static/node_modules/moment/locale/zh-hk.js
+-rw-r--r--   0        0        0     3782 2022-11-14 15:08:03.701810 anitya-1.8.0/anitya/static/node_modules/moment/locale/zh-mo.js
+-rw-r--r--   0        0        0     3729 2022-11-14 15:08:03.701810 anitya-1.8.0/anitya/static/node_modules/moment/locale/zh-tw.js
+-rw-r--r--   0        0        0   448027 2022-11-14 15:08:03.602810 anitya-1.8.0/anitya/static/node_modules/moment/min/locales.js
+-rw-r--r--   0        0        0   310773 2022-11-14 15:08:03.609809 anitya-1.8.0/anitya/static/node_modules/moment/min/locales.min.js
+-rw-r--r--   0        0        0   140130 2022-11-14 15:08:03.702810 anitya-1.8.0/anitya/static/node_modules/moment/min/locales.min.js.map
+-rw-r--r--   0        0        0   622045 2022-11-14 15:08:03.629810 anitya-1.8.0/anitya/static/node_modules/moment/min/moment-with-locales.js
+-rw-r--r--   0        0        0   369019 2022-11-14 15:08:03.634810 anitya-1.8.0/anitya/static/node_modules/moment/min/moment-with-locales.min.js
+-rw-r--r--   0        0        0   230173 2022-11-14 15:08:03.704810 anitya-1.8.0/anitya/static/node_modules/moment/min/moment-with-locales.min.js.map
+-rw-r--r--   0        0        0    58103 2022-11-14 15:08:03.636810 anitya-1.8.0/anitya/static/node_modules/moment/min/moment.min.js
+-rw-r--r--   0        0        0    86041 2022-11-14 15:08:03.705810 anitya-1.8.0/anitya/static/node_modules/moment/min/moment.min.js.map
+-rw-r--r--   0        0        0    23820 2022-11-14 15:08:03.705810 anitya-1.8.0/anitya/static/node_modules/moment/moment.d.ts
+-rw-r--r--   0        0        0   174604 2022-11-14 15:08:03.636810 anitya-1.8.0/anitya/static/node_modules/moment/moment.js
+-rw-r--r--   0        0        0      273 2022-11-14 15:08:03.646810 anitya-1.8.0/anitya/static/node_modules/moment/package.js
+-rw-r--r--   0        0        0     3418 2022-11-14 15:08:03.702810 anitya-1.8.0/anitya/static/node_modules/moment/package.json
+-rw-r--r--   0        0        0     1542 2022-11-14 15:08:03.470809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/check-overflow.js
+-rw-r--r--   0        0        0     1076 2022-11-14 15:08:03.479809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/date-from-array.js
+-rw-r--r--   0        0        0     3351 2022-11-14 15:08:03.545809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/from-anything.js
+-rw-r--r--   0        0        0     5585 2022-11-14 15:08:03.546809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/from-array.js
+-rw-r--r--   0        0        0      549 2022-11-14 15:08:03.546809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/from-object.js
+-rw-r--r--   0        0        0     2011 2022-11-14 15:08:03.546809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/from-string-and-array.js
+-rw-r--r--   0        0        0     4092 2022-11-14 15:08:03.547809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/from-string-and-format.js
+-rw-r--r--   0        0        0     8007 2022-11-14 15:08:03.547809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/from-string.js
+-rw-r--r--   0        0        0      183 2022-11-14 15:08:03.596809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/local.js
+-rw-r--r--   0        0        0      644 2022-11-14 15:08:03.646810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/parsing-flags.js
+-rw-r--r--   0        0        0      186 2022-11-14 15:08:03.690810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/utc.js
+-rw-r--r--   0        0        0     1514 2022-11-14 15:08:03.692810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/valid.js
+-rw-r--r--   0        0        0      484 2022-11-14 15:08:03.414809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/abs.js
+-rw-r--r--   0        0        0      644 2022-11-14 15:08:03.415809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/add-subtract.js
+-rw-r--r--   0        0        0     2360 2022-11-14 15:08:03.441809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/as.js
+-rw-r--r--   0        0        0     1774 2022-11-14 15:08:03.466809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/bubble.js
+-rw-r--r--   0        0        0      105 2022-11-14 15:08:03.470809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/clone.js
+-rw-r--r--   0        0        0     1593 2022-11-14 15:08:03.472809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/constructor.js
+-rw-r--r--   0        0        0     4335 2022-11-14 15:08:03.474809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/create.js
+-rw-r--r--   0        0        0      342 2022-11-14 15:08:03.487809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/duration.js
+-rw-r--r--   0        0        0      728 2022-11-14 15:08:03.552809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/get.js
+-rw-r--r--   0        0        0     3493 2022-11-14 15:08:03.567809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/humanize.js
+-rw-r--r--   0        0        0     2078 2022-11-14 15:08:03.578809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/iso-string.js
+-rw-r--r--   0        0        0     1739 2022-11-14 15:08:03.647810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/prototype.js
+-rw-r--r--   0        0        0     1184 2022-11-14 15:08:03.693810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/valid.js
+-rw-r--r--   0        0        0     2911 2022-11-14 15:08:03.538809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/format/format.js
+-rw-r--r--   0        0        0     1187 2022-11-14 15:08:03.452809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/base-config.js
+-rw-r--r--   0        0        0      442 2022-11-14 15:08:03.467809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/calendar.js
+-rw-r--r--   0        0        0       93 2022-11-14 15:08:03.472809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/constructor.js
+-rw-r--r--   0        0        0      989 2022-11-14 15:08:03.511809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/en.js
+-rw-r--r--   0        0        0      876 2022-11-14 15:08:03.540809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/formats.js
+-rw-r--r--   0        0        0      113 2022-11-14 15:08:03.572809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/invalid.js
+-rw-r--r--   0        0        0     2188 2022-11-14 15:08:03.594809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/lists.js
+-rw-r--r--   0        0        0      829 2022-11-14 15:08:03.596809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/locale.js
+-rw-r--r--   0        0        0     7728 2022-11-14 15:08:03.602810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/locales.js
+-rw-r--r--   0        0        0      218 2022-11-14 15:08:03.643810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/ordinal.js
+-rw-r--r--   0        0        0       66 2022-11-14 15:08:03.647810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/pre-post-format.js
+-rw-r--r--   0        0        0     2229 2022-11-14 15:08:03.648810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/prototype.js
+-rw-r--r--   0        0        0      842 2022-11-14 15:08:03.652810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/relative.js
+-rw-r--r--   0        0        0     1831 2022-11-14 15:08:03.656810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/set.js
+-rw-r--r--   0        0        0     1869 2022-11-14 15:08:03.419809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/add-subtract.js
+-rw-r--r--   0        0        0     1737 2022-11-14 15:08:03.467809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/calendar.js
+-rw-r--r--   0        0        0       98 2022-11-14 15:08:03.471809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/clone.js
+-rw-r--r--   0        0        0     2379 2022-11-14 15:08:03.471809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/compare.js
+-rw-r--r--   0        0        0     2106 2022-11-14 15:08:03.473809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/constructor.js
+-rw-r--r--   0        0        0      192 2022-11-14 15:08:03.475809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/creation-data.js
+-rw-r--r--   0        0        0     2345 2022-11-14 15:08:03.486809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/diff.js
+-rw-r--r--   0        0        0     2340 2022-11-14 15:08:03.539809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/format.js
+-rw-r--r--   0        0        0      609 2022-11-14 15:08:03.547809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/from.js
+-rw-r--r--   0        0        0     2041 2022-11-14 15:08:03.552809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/get-set.js
+-rw-r--r--   0        0        0      946 2022-11-14 15:08:03.596809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/locale.js
+-rw-r--r--   0        0        0     1922 2022-11-14 15:08:03.617810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/min-max.js
+-rw-r--r--   0        0        0      609 2022-11-14 15:08:03.636810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/moment.js
+-rw-r--r--   0        0        0       82 2022-11-14 15:08:03.643810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/now.js
+-rw-r--r--   0        0        0     5511 2022-11-14 15:08:03.648810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/prototype.js
+-rw-r--r--   0        0        0     4819 2022-11-14 15:08:03.661810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/start-end-of.js
+-rw-r--r--   0        0        0      834 2022-11-14 15:08:03.672810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/to-type.js
+-rw-r--r--   0        0        0      603 2022-11-14 15:08:03.672810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/to.js
+-rw-r--r--   0        0        0      364 2022-11-14 15:08:03.693810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/valid.js
+-rw-r--r--   0        0        0     2500 2022-11-14 15:08:03.652810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/parse/regex.js
+-rw-r--r--   0        0        0      958 2022-11-14 15:08:03.672810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/parse/token.js
+-rw-r--r--   0        0        0      809 2022-11-14 15:08:03.426809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/aliases.js
+-rw-r--r--   0        0        0      148 2022-11-14 15:08:03.471809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/constants.js
+-rw-r--r--   0        0        0     1065 2022-11-14 15:08:03.479809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/day-of-month.js
+-rw-r--r--   0        0        0    12904 2022-11-14 15:08:03.480809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/day-of-week.js
+-rw-r--r--   0        0        0      920 2022-11-14 15:08:03.480809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/day-of-year.js
+-rw-r--r--   0        0        0     7984 2022-11-14 15:08:03.514809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/era.js
+-rw-r--r--   0        0        0     4475 2022-11-14 15:08:03.564809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/hour.js
+-rw-r--r--   0        0        0     1870 2022-11-14 15:08:03.616809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/millisecond.js
+-rw-r--r--   0        0        0      679 2022-11-14 15:08:03.617810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/minute.js
+-rw-r--r--   0        0        0    10021 2022-11-14 15:08:03.637810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/month.js
+-rw-r--r--   0        0        0     7070 2022-11-14 15:08:03.643810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/offset.js
+-rw-r--r--   0        0        0      480 2022-11-14 15:08:03.647810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/priorities.js
+-rw-r--r--   0        0        0      780 2022-11-14 15:08:03.651810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/quarter.js
+-rw-r--r--   0        0        0      679 2022-11-14 15:08:03.656810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/second.js
+-rw-r--r--   0        0        0      590 2022-11-14 15:08:03.668810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/timestamp.js
+-rw-r--r--   0        0        0      325 2022-11-14 15:08:03.668810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/timezone.js
+-rw-r--r--   0        0        0      404 2022-11-14 15:08:03.689810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/units.js
+-rw-r--r--   0        0        0     2107 2022-11-14 15:08:03.694810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/week-calendar-utils.js
+-rw-r--r--   0        0        0     3483 2022-11-14 15:08:03.694810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/week-year.js
+-rw-r--r--   0        0        0     1664 2022-11-14 15:08:03.694810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/week.js
+-rw-r--r--   0        0        0     2001 2022-11-14 15:08:03.695810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/year.js
+-rw-r--r--   0        0        0      154 2022-11-14 15:08:03.411809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/abs-ceil.js
+-rw-r--r--   0        0        0      179 2022-11-14 15:08:03.411809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/abs-floor.js
+-rw-r--r--   0        0        0      166 2022-11-14 15:08:03.412809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/abs-round.js
+-rw-r--r--   0        0        0      553 2022-11-14 15:08:03.471809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/compare-arrays.js
+-rw-r--r--   0        0        0      203 2022-11-14 15:08:03.486809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/defaults.js
+-rw-r--r--   0        0        0     1946 2022-11-14 15:08:03.486809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/deprecate.js
+-rw-r--r--   0        0        0      345 2022-11-14 15:08:03.526809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/extend.js
+-rw-r--r--   0        0        0      100 2022-11-14 15:08:03.560809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/has-own-prop.js
+-rw-r--r--   0        0        0      296 2022-11-14 15:08:03.563809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/hooks.js
+-rw-r--r--   0        0        0      342 2022-11-14 15:08:03.572809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/index-of.js
+-rw-r--r--   0        0        0      164 2022-11-14 15:08:03.573809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/is-array.js
+-rw-r--r--   0        0        0      670 2022-11-14 15:08:03.573809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/is-calendar-spec.js
+-rw-r--r--   0        0        0      161 2022-11-14 15:08:03.573809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/is-date.js
+-rw-r--r--   0        0        0      210 2022-11-14 15:08:03.574809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/is-function.js
+-rw-r--r--   0        0        0      106 2022-11-14 15:08:03.574809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/is-leap-year.js
+-rw-r--r--   0        0        0     1988 2022-11-14 15:08:03.574809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/is-moment-input.js
+-rw-r--r--   0        0        0      169 2022-11-14 15:08:03.575809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/is-number.js
+-rw-r--r--   0        0        0      360 2022-11-14 15:08:03.575809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/is-object-empty.js
+-rw-r--r--   0        0        0      246 2022-11-14 15:08:03.576810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/is-object.js
+-rw-r--r--   0        0        0      109 2022-11-14 15:08:03.576810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/is-string.js
+-rw-r--r--   0        0        0       76 2022-11-14 15:08:03.576810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/is-undefined.js
+-rw-r--r--   0        0        0      344 2022-11-14 15:08:03.584809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/keys.js
+-rw-r--r--   0        0        0      189 2022-11-14 15:08:03.613809 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/map.js
+-rw-r--r--   0        0        0       68 2022-11-14 15:08:03.622810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/mod.js
+-rw-r--r--   0        0        0      394 2022-11-14 15:08:03.658810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/some.js
+-rw-r--r--   0        0        0      282 2022-11-14 15:08:03.671810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/to-int.js
+-rw-r--r--   0        0        0      352 2022-11-14 15:08:03.697810 anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/zero-fill.js
+-rw-r--r--   0        0        0     2149 2022-11-14 15:08:03.424809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/af.js
+-rw-r--r--   0        0        0     4449 2022-11-14 15:08:03.428809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar-dz.js
+-rw-r--r--   0        0        0     1934 2022-11-14 15:08:03.429809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar-kw.js
+-rw-r--r--   0        0        0     4648 2022-11-14 15:08:03.432809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar-ly.js
+-rw-r--r--   0        0        0     1989 2022-11-14 15:08:03.436809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar-ma.js
+-rw-r--r--   0        0        0     3042 2022-11-14 15:08:03.438809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar-sa.js
+-rw-r--r--   0        0        0     1936 2022-11-14 15:08:03.439809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar-tn.js
+-rw-r--r--   0        0        0     5072 2022-11-14 15:08:03.441809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar.js
+-rw-r--r--   0        0        0     2846 2022-11-14 15:08:03.449809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/az.js
+-rw-r--r--   0        0        0     5154 2022-11-14 15:08:03.454809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/be.js
+-rw-r--r--   0        0        0     2955 2022-11-14 15:08:03.456809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/bg.js
+-rw-r--r--   0        0        0     1784 2022-11-14 15:08:03.459809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/bm.js
+-rw-r--r--   0        0        0     4349 2022-11-14 15:08:03.460809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/bn-bd.js
+-rw-r--r--   0        0        0     3898 2022-11-14 15:08:03.462809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/bn.js
+-rw-r--r--   0        0        0     4399 2022-11-14 15:08:03.464809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/bo.js
+-rw-r--r--   0        0        0     4544 2022-11-14 15:08:03.465809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/br.js
+-rw-r--r--   0        0        0     4475 2022-11-14 15:08:03.466809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/bs.js
+-rw-r--r--   0        0        0     3031 2022-11-14 15:08:03.467809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ca.js
+-rw-r--r--   0        0        0     6718 2022-11-14 15:08:03.476809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/cs.js
+-rw-r--r--   0        0        0     2341 2022-11-14 15:08:03.476809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/cv.js
+-rw-r--r--   0        0        0     2834 2022-11-14 15:08:03.478809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/cy.js
+-rw-r--r--   0        0        0     1629 2022-11-14 15:08:03.478809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/da.js
+-rw-r--r--   0        0        0     2635 2022-11-14 15:08:03.481809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/de-at.js
+-rw-r--r--   0        0        0     2563 2022-11-14 15:08:03.483809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/de-ch.js
+-rw-r--r--   0        0        0     2562 2022-11-14 15:08:03.485809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/de.js
+-rw-r--r--   0        0        0     2464 2022-11-14 15:08:03.488809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/dv.js
+-rw-r--r--   0        0        0     3877 2022-11-14 15:08:03.489809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/el.js
+-rw-r--r--   0        0        0     2029 2022-11-14 15:08:03.491809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-au.js
+-rw-r--r--   0        0        0     1878 2022-11-14 15:08:03.492809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-ca.js
+-rw-r--r--   0        0        0     2035 2022-11-14 15:08:03.494809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-gb.js
+-rw-r--r--   0        0        0     2033 2022-11-14 15:08:03.497809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-ie.js
+-rw-r--r--   0        0        0     1871 2022-11-14 15:08:03.500809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-il.js
+-rw-r--r--   0        0        0     2029 2022-11-14 15:08:03.502809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-in.js
+-rw-r--r--   0        0        0     2038 2022-11-14 15:08:03.504809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-nz.js
+-rw-r--r--   0        0        0     2047 2022-11-14 15:08:03.510809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-sg.js
+-rw-r--r--   0        0        0     2338 2022-11-14 15:08:03.513809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/eo.js
+-rw-r--r--   0        0        0     3441 2022-11-14 15:08:03.517809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/es-do.js
+-rw-r--r--   0        0        0     3510 2022-11-14 15:08:03.518809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/es-mx.js
+-rw-r--r--   0        0        0     3538 2022-11-14 15:08:03.521809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/es-us.js
+-rw-r--r--   0        0        0     3498 2022-11-14 15:08:03.523809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/es.js
+-rw-r--r--   0        0        0     2631 2022-11-14 15:08:03.524809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/et.js
+-rw-r--r--   0        0        0     1964 2022-11-14 15:08:03.526809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/eu.js
+-rw-r--r--   0        0        0     3230 2022-11-14 15:08:03.527809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fa.js
+-rw-r--r--   0        0        0     3632 2022-11-14 15:08:03.529809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fi.js
+-rw-r--r--   0        0        0     1776 2022-11-14 15:08:03.531809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fil.js
+-rw-r--r--   0        0        0     1772 2022-11-14 15:08:03.534809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fo.js
+-rw-r--r--   0        0        0     2104 2022-11-14 15:08:03.541809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fr-ca.js
+-rw-r--r--   0        0        0     2263 2022-11-14 15:08:03.543809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fr-ch.js
+-rw-r--r--   0        0        0     3471 2022-11-14 15:08:03.544809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fr.js
+-rw-r--r--   0        0        0     2275 2022-11-14 15:08:03.549809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fy.js
+-rw-r--r--   0        0        0     2360 2022-11-14 15:08:03.550809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ga.js
+-rw-r--r--   0        0        0     2380 2022-11-14 15:08:03.551809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/gd.js
+-rw-r--r--   0        0        0     2347 2022-11-14 15:08:03.555809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/gl.js
+-rw-r--r--   0        0        0     5506 2022-11-14 15:08:03.556809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/gom-deva.js
+-rw-r--r--   0        0        0     4130 2022-11-14 15:08:03.558809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/gom-latn.js
+-rw-r--r--   0        0        0     4132 2022-11-14 15:08:03.559809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/gu.js
+-rw-r--r--   0        0        0     3211 2022-11-14 15:08:03.561809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/he.js
+-rw-r--r--   0        0        0     6421 2022-11-14 15:08:03.563809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/hi.js
+-rw-r--r--   0        0        0     4718 2022-11-14 15:08:03.566809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/hr.js
+-rw-r--r--   0        0        0     3815 2022-11-14 15:08:03.567809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/hu.js
+-rw-r--r--   0        0        0     3236 2022-11-14 15:08:03.570809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/hy-am.js
+-rw-r--r--   0        0        0     2375 2022-11-14 15:08:03.571809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/id.js
+-rw-r--r--   0        0        0     4458 2022-11-14 15:08:03.577809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/is.js
+-rw-r--r--   0        0        0     1941 2022-11-14 15:08:03.579810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/it-ch.js
+-rw-r--r--   0        0        0     3251 2022-11-14 15:08:03.580809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/it.js
+-rw-r--r--   0        0        0     3955 2022-11-14 15:08:03.581809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ja.js
+-rw-r--r--   0        0        0     2384 2022-11-14 15:08:03.583809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/jv.js
+-rw-r--r--   0        0        0     3504 2022-11-14 15:08:03.584809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ka.js
+-rw-r--r--   0        0        0     2495 2022-11-14 15:08:03.585809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/kk.js
+-rw-r--r--   0        0        0     3362 2022-11-14 15:08:03.587809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/km.js
+-rw-r--r--   0        0        0     4252 2022-11-14 15:08:03.588809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/kn.js
+-rw-r--r--   0        0        0     2223 2022-11-14 15:08:03.590809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ko.js
+-rw-r--r--   0        0        0     3330 2022-11-14 15:08:03.591809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ku.js
+-rw-r--r--   0        0        0     2521 2022-11-14 15:08:03.592810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ky.js
+-rw-r--r--   0        0        0     4269 2022-11-14 15:08:03.594809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/lb.js
+-rw-r--r--   0        0        0     2585 2022-11-14 15:08:03.595810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/lo.js
+-rw-r--r--   0        0        0     4005 2022-11-14 15:08:03.610809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/lt.js
+-rw-r--r--   0        0        0     3449 2022-11-14 15:08:03.613809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/lv.js
+-rw-r--r--   0        0        0     3661 2022-11-14 15:08:03.614810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/me.js
+-rw-r--r--   0        0        0     2023 2022-11-14 15:08:03.616809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/mi.js
+-rw-r--r--   0        0        0     3021 2022-11-14 15:08:03.619809 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/mk.js
+-rw-r--r--   0        0        0     3287 2022-11-14 15:08:03.620810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ml.js
+-rw-r--r--   0        0        0     3414 2022-11-14 15:08:03.621810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/mn.js
+-rw-r--r--   0        0        0     6574 2022-11-14 15:08:03.637810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/mr.js
+-rw-r--r--   0        0        0     2330 2022-11-14 15:08:03.638810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ms-my.js
+-rw-r--r--   0        0        0     2277 2022-11-14 15:08:03.638810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ms.js
+-rw-r--r--   0        0        0     1684 2022-11-14 15:08:03.639810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/mt.js
+-rw-r--r--   0        0        0     3094 2022-11-14 15:08:03.640810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/my.js
+-rw-r--r--   0        0        0     1899 2022-11-14 15:08:03.640810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/nb.js
+-rw-r--r--   0        0        0     4031 2022-11-14 15:08:03.641810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ne.js
+-rw-r--r--   0        0        0     3169 2022-11-14 15:08:03.641810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/nl-be.js
+-rw-r--r--   0        0        0     3202 2022-11-14 15:08:03.642810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/nl.js
+-rw-r--r--   0        0        0     1828 2022-11-14 15:08:03.642810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/nn.js
+-rw-r--r--   0        0        0     2472 2022-11-14 15:08:03.643810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/oc-lnc.js
+-rw-r--r--   0        0        0     4198 2022-11-14 15:08:03.646810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/pa-in.js
+-rw-r--r--   0        0        0     4166 2022-11-14 15:08:03.647810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/pl.js
+-rw-r--r--   0        0        0     1854 2022-11-14 15:08:03.650810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/pt-br.js
+-rw-r--r--   0        0        0     1968 2022-11-14 15:08:03.650810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/pt.js
+-rw-r--r--   0        0        0     2319 2022-11-14 15:08:03.652810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ro.js
+-rw-r--r--   0        0        0     8418 2022-11-14 15:08:03.654810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ru.js
+-rw-r--r--   0        0        0     2153 2022-11-14 15:08:03.655810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sd.js
+-rw-r--r--   0        0        0     1849 2022-11-14 15:08:03.656810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/se.js
+-rw-r--r--   0        0        0     2681 2022-11-14 15:08:03.656810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/si.js
+-rw-r--r--   0        0        0     5173 2022-11-14 15:08:03.657810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sk.js
+-rw-r--r--   0        0        0     6115 2022-11-14 15:08:03.658810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sl.js
+-rw-r--r--   0        0        0     1987 2022-11-14 15:08:03.658810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sq.js
+-rw-r--r--   0        0        0     4762 2022-11-14 15:08:03.659810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sr-cyrl.js
+-rw-r--r--   0        0        0     4209 2022-11-14 15:08:03.660810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sr.js
+-rw-r--r--   0        0        0     2572 2022-11-14 15:08:03.661810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ss.js
+-rw-r--r--   0        0        0     2066 2022-11-14 15:08:03.663810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sv.js
+-rw-r--r--   0        0        0     1651 2022-11-14 15:08:03.663810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sw.js
+-rw-r--r--   0        0        0     4800 2022-11-14 15:08:03.664810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ta.js
+-rw-r--r--   0        0        0     3392 2022-11-14 15:08:03.665810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/te.js
+-rw-r--r--   0        0        0     2155 2022-11-14 15:08:03.666810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tet.js
+-rw-r--r--   0        0        0     3604 2022-11-14 15:08:03.667810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tg.js
+-rw-r--r--   0        0        0     2736 2022-11-14 15:08:03.668810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/th.js
+-rw-r--r--   0        0        0     2488 2022-11-14 15:08:03.669810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tk.js
+-rw-r--r--   0        0        0     1735 2022-11-14 15:08:03.670810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tl-ph.js
+-rw-r--r--   0        0        0     3755 2022-11-14 15:08:03.671810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tlh.js
+-rw-r--r--   0        0        0     2927 2022-11-14 15:08:03.673810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tr.js
+-rw-r--r--   0        0        0     3109 2022-11-14 15:08:03.674810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tzl.js
+-rw-r--r--   0        0        0     1691 2022-11-14 15:08:03.675810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tzm-latn.js
+-rw-r--r--   0        0        0     2322 2022-11-14 15:08:03.681810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tzm.js
+-rw-r--r--   0        0        0     3880 2022-11-14 15:08:03.688810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ug-cn.js
+-rw-r--r--   0        0        0     5955 2022-11-14 15:08:03.689810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/uk.js
+-rw-r--r--   0        0        0     2200 2022-11-14 15:08:03.690810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ur.js
+-rw-r--r--   0        0        0     1639 2022-11-14 15:08:03.691810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/uz-latn.js
+-rw-r--r--   0        0        0     1885 2022-11-14 15:08:03.692810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/uz.js
+-rw-r--r--   0        0        0     2430 2022-11-14 15:08:03.694810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/vi.js
+-rw-r--r--   0        0        0     2348 2022-11-14 15:08:03.695810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/x-pseudo.js
+-rw-r--r--   0        0        0     1887 2022-11-14 15:08:03.696810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/yo.js
+-rw-r--r--   0        0        0     3711 2022-11-14 15:08:03.700810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/zh-cn.js
+-rw-r--r--   0        0        0     3116 2022-11-14 15:08:03.701810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/zh-hk.js
+-rw-r--r--   0        0        0     3066 2022-11-14 15:08:03.701810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/zh-mo.js
+-rw-r--r--   0        0        0     3013 2022-11-14 15:08:03.702810 anitya-1.8.0/anitya/static/node_modules/moment/src/locale/zh-tw.js
+-rw-r--r--   0        0        0     2694 2022-11-14 15:08:03.636810 anitya-1.8.0/anitya/static/node_modules/moment/src/moment.js
+-rw-r--r--   0        0        0    23327 2022-11-14 15:08:03.705810 anitya-1.8.0/anitya/static/node_modules/moment/ts3.1-typings/moment.d.ts
+-rw-r--r--   0        0        0     3584 2023-04-26 13:29:52.886981 anitya-1.8.0/anitya/static/package-lock.json
+-rw-r--r--   0        0        0      765 2023-01-26 12:16:19.281657 anitya-1.8.0/anitya/static/package.json
+-rw-r--r--   0        0        0     2970 2020-12-02 09:02:04.993902 anitya-1.8.0/anitya/static/yahoo_logo.png
+-rw-r--r--   0        0        0        0 2020-12-02 09:02:04.993902 anitya-1.8.0/anitya/templates/__init__.py
+-rw-r--r--   0        0        0     3236 2023-01-26 12:16:19.281657 anitya-1.8.0/anitya/templates/distro_add_edit.html
+-rw-r--r--   0        0        0      596 2023-01-26 12:16:19.282657 anitya-1.8.0/anitya/templates/distro_delete.html
+-rw-r--r--   0        0        0     2293 2023-01-26 12:16:19.282657 anitya-1.8.0/anitya/templates/distros.html
+-rw-r--r--   0        0        0     4148 2023-01-26 12:16:19.282657 anitya-1.8.0/anitya/templates/flags.html
+-rw-r--r--   0        0        0      438 2020-12-02 09:02:04.994902 anitya-1.8.0/anitya/templates/functions.html
+-rw-r--r--   0        0        0     1626 2023-01-26 12:16:19.282657 anitya-1.8.0/anitya/templates/index.html
+-rw-r--r--   0        0        0     1019 2023-01-26 12:16:19.283657 anitya-1.8.0/anitya/templates/login.html
+-rw-r--r--   0        0        0     2388 2023-01-26 12:16:19.283657 anitya-1.8.0/anitya/templates/logs.html
+-rw-r--r--   0        0        0     1762 2023-01-26 12:16:19.283657 anitya-1.8.0/anitya/templates/mapping.html
+-rw-r--r--   0        0        0     9973 2023-01-26 12:16:19.284657 anitya-1.8.0/anitya/templates/master.html
+-rw-r--r--   0        0        0    14953 2023-04-24 16:04:41.039772 anitya-1.8.0/anitya/templates/project.html
+-rw-r--r--   0        0        0     3734 2023-01-26 12:16:19.284657 anitya-1.8.0/anitya/templates/project_archive.html
+-rw-r--r--   0        0        0     3053 2023-01-26 12:16:19.285657 anitya-1.8.0/anitya/templates/project_delete.html
+-rw-r--r--   0        0        0     1134 2023-01-26 12:16:19.285657 anitya-1.8.0/anitya/templates/project_flag.html
+-rw-r--r--   0        0        0    17245 2023-01-26 12:16:19.285657 anitya-1.8.0/anitya/templates/project_new.html
+-rw-r--r--   0        0        0      999 2023-01-26 12:16:19.286657 anitya-1.8.0/anitya/templates/project_versions_delete.html
+-rw-r--r--   0        0        0     3751 2023-01-26 12:16:19.286657 anitya-1.8.0/anitya/templates/projects.html
+-rw-r--r--   0        0        0     1354 2023-01-26 12:16:19.286657 anitya-1.8.0/anitya/templates/regex_delete.html
+-rw-r--r--   0        0        0     3543 2023-01-26 12:16:19.286657 anitya-1.8.0/anitya/templates/search.html
+-rw-r--r--   0        0        0     2101 2023-01-26 12:16:19.286657 anitya-1.8.0/anitya/templates/settings.html
+-rw-r--r--   0        0        0     4848 2023-01-26 12:16:19.286657 anitya-1.8.0/anitya/templates/updates.html
+-rw-r--r--   0        0        0     4393 2023-01-26 12:16:19.286657 anitya-1.8.0/anitya/templates/users.html
+-rw-r--r--   0        0        0     1250 2023-01-26 12:16:19.286657 anitya-1.8.0/anitya/templates/version_delete.html
+-rw-r--r--   0        0        0    24066 2023-04-24 16:04:41.041772 anitya-1.8.0/anitya/ui.py
+-rw-r--r--   0        0        0      835 2020-12-02 09:02:05.009902 anitya-1.8.0/anitya/wsgi.py
+-rw-r--r--   0        0        0     1866 2020-12-02 09:02:05.011902 anitya-1.8.0/createdb.py
+-rw-r--r--   0        0        0     3954 2022-12-14 14:15:41.913739 anitya-1.8.0/files/anitya.toml.sample
+-rw-r--r--   0        0        0      364 2020-12-02 09:02:05.012902 anitya-1.8.0/files/config.toml.sample
+-rw-r--r--   0        0        0     3488 2023-04-27 10:09:02.802113 anitya-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0    16614 1970-01-01 00:00:00.000000 anitya-1.8.0/setup.py
+-rw-r--r--   0        0        0     3843 1970-01-01 00:00:00.000000 anitya-1.8.0/PKG-INFO
```

### Comparing `anitya-1.7.0/LICENSE` & `anitya-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/README.rst` & `anitya-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/alembic.ini` & `anitya-1.8.0/alembic.ini`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/admin.py` & `anitya-1.8.0/anitya/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     if user.is_authenticated:
         return user.is_admin
 
 
 @ui_blueprint.route("/distro/<distro_name>/edit", methods=["GET", "POST"])
 @login_required
 def edit_distro(distro_name):
-
     distro = models.Distro.by_name(Session, distro_name)
     if not distro:
         flask.abort(404)
 
     if not is_admin():
         flask.abort(401)
 
@@ -96,15 +95,14 @@
         "distro_delete.html", current="distros", distro=distro, form=form
     )
 
 
 @ui_blueprint.route("/project/<project_id>/delete", methods=["GET", "POST"])
 @login_required
 def delete_project(project_id):
-
     project = models.Project.get(Session, project_id)
     if not project:
         flask.abort(404)
 
     if not is_admin():
         flask.abort(401)
 
@@ -139,15 +137,14 @@
 
 
 @ui_blueprint.route(
     "/project/<project_id>/archive/set/<state>", methods=["GET", "POST"]
 )
 @login_required
 def set_project_archive_state(project_id, state):
-
     if not is_admin():
         flask.abort(401)
 
     if state not in ("true", "false"):
         flask.abort(422)
 
     project = models.Project.get(Session, project_id)
@@ -203,15 +200,14 @@
 
 
 @ui_blueprint.route(
     "/project/<project_id>/delete/<distro_name>/<pkg_name>", methods=["GET", "POST"]
 )
 @login_required
 def delete_project_mapping(project_id, distro_name, pkg_name):
-
     project = models.Project.get(Session, project_id)
     if not project:
         flask.abort(404)
 
     distro = models.Distro.get(Session, distro_name)
     if not distro:
         flask.abort(404)
@@ -252,15 +248,14 @@
         form=form,
     )
 
 
 @ui_blueprint.route("/project/<project_id>/delete/<version>", methods=["GET", "POST"])
 @login_required
 def delete_project_version(project_id, version):
-
     project = models.Project.get(Session, project_id)
     if not project:
         flask.abort(404)
 
     version_obj = None
     for vers in project.versions_obj:
         if version == vers.version:
@@ -365,15 +360,14 @@
         form=form,
     )
 
 
 @ui_blueprint.route("/flags")
 @login_required
 def browse_flags():
-
     if not is_admin():
         flask.abort(401)
 
     from_date = flask.request.args.get("from_date", None)
     state = flask.request.args.get("state", "open")
     project = flask.request.args.get("project", None)
     flags_for_user = flask.request.args.get("user", None)
@@ -450,15 +444,14 @@
         state=state or "",
     )
 
 
 @ui_blueprint.route("/flags/<flag_id>/set/<state>", methods=["POST"])
 @login_required
 def set_flag_state(flag_id, state):
-
     if not is_admin():
         flask.abort(401)
 
     if state not in ("open", "closed"):
         flask.abort(422)
 
     flag = models.ProjectFlag.get(Session, flag_id)
@@ -479,15 +472,14 @@
 
     return flask.redirect(flask.url_for("anitya_ui.browse_flags"))
 
 
 @ui_blueprint.route("/users", methods=["GET"])
 @login_required
 def browse_users():
-
     if not is_admin():
         flask.abort(401)
 
     user_id = flask.request.args.get("user_id", None)
     username = flask.request.args.get("username", None)
     email = flask.request.args.get("email", None)
     admin = flask.request.args.get("admin", None)
@@ -579,15 +571,14 @@
         active=active,
     )
 
 
 @ui_blueprint.route("/users/<user_id>/admin/<state>", methods=["POST"])
 @login_required
 def set_user_admin_state(user_id, state):
-
     if not is_admin():
         flask.abort(401)
 
     if state.upper() == "TRUE":
         state = True
     elif state.upper() == "FALSE":
         state = False
@@ -621,15 +612,14 @@
 
     return flask.redirect(flask.url_for("anitya_ui.browse_users"))
 
 
 @ui_blueprint.route("/users/<user_id>/active/<state>", methods=["POST"])
 @login_required
 def set_user_active_state(user_id, state):
-
     if not is_admin():
         flask.abort(401)
 
     if state.upper() == "TRUE":
         state = True
     elif state.upper() == "FALSE":
         state = False
```

### Comparing `anitya-1.7.0/anitya/api.py` & `anitya-1.8.0/anitya/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,14 @@
     if not project_id:
         errors = []
         if not project_id:
             errors.append("No project id specified")
         output = {"output": "notok", "error": errors}
         httpcode = 400
     else:
-
         project = models.Project.get(Session, project_id=project_id)
 
         if not project:
             output = {"output": "notok", "error": "No such project"}
             httpcode = 404
         else:
             try:
```

### Comparing `anitya-1.7.0/anitya/api_v2.py` & `anitya-1.8.0/anitya/api_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,16 @@
             {
                 "items": [
                     {
                         "distribution": "Fedora",
                         "name": "python-requests"
                         "project": "requests",
                         "ecosystem": "pypi",
-                        "version": "2.28.1"
+                        "version": "2.28.1",
+                        "stable_version": "2.28.1"
                     }
                 ],
                 "items_per_page": 25,
                 "page": 1,
                 "total_items": 1
             }
 
@@ -164,14 +165,15 @@
             "items": [
                 {
                     "distribution": package.distro_name,
                     "name": package.package_name,
                     "project": package.project.name,
                     "ecosystem": package.project.ecosystem_name,
                     "version": package.project.latest_version,
+                    "stable_version": package.project.latest_stable_version,
                 }
                 for package in page.items
             ],
             "page": page.page,
             "items_per_page": page.items_per_page,
             "total_items": page.total_items,
         }
```

### Comparing `anitya-1.7.0/anitya/app.py` & `anitya-1.8.0/anitya/app.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/authentication.py` & `anitya-1.8.0/anitya/authentication.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/check_service.py` & `anitya-1.8.0/anitya/check_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
         Returns:
             Queue of project's ids to check. Blacklisted projects will be on start of
             the queue
         """
         queue = []
         # Add blacklisted items first
         backends = []
-        for (backend, reset_time) in self.blacklist_dict.items():
+        for backend, reset_time in self.blacklist_dict.items():
             if reset_time < time:
                 with self.ratelimit_queue_lock:
                     queue += self.ratelimit_queue[backend]
                     # Erase project list after adding it to queue
                     del self.ratelimit_queue[backend]
 
                 backends.append(backend)
```

### Comparing `anitya-1.7.0/anitya/compat.py` & `anitya-1.8.0/anitya/compat.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/config.py` & `anitya-1.8.0/anitya/config.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/__init__.py` & `anitya-1.8.0/anitya/db/__init__.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/events.py` & `anitya-1.8.0/anitya/db/events.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/meta.py` & `anitya-1.8.0/anitya/db/meta.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/env.py` & `anitya-1.8.0/anitya/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/136d119ab015_rename_project_latest_known_cursor_to_.py` & `anitya-1.8.0/anitya/db/migrations/versions/136d119ab015_rename_project_latest_known_cursor_to_.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/16aa7da2764c_add_projectversion_commit_url.py` & `anitya-1.8.0/anitya/db/migrations/versions/16aa7da2764c_add_projectversion_commit_url.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/1ab95561edae_convert_date_to_rpm.py` & `anitya-1.8.0/anitya/db/migrations/versions/1ab95561edae_convert_date_to_rpm.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/1bf8aead6179_add_check_times.py` & `anitya-1.8.0/anitya/db/migrations/versions/1bf8aead6179_add_check_times.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/1f839c54e428_add_archive_flag.py` & `anitya-1.8.0/anitya/db/migrations/versions/1f839c54e428_add_archive_flag.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/24b6734e8565_creation_date_on_version.py` & `anitya-1.8.0/anitya/db/migrations/versions/24b6734e8565_creation_date_on_version.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/27342bce1d0f_populate_project_version_scheme.py` & `anitya-1.8.0/anitya/db/migrations/versions/27342bce1d0f_populate_project_version_scheme.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/2925648d8cc3_add_a_version_prefix_field.py` & `anitya-1.8.0/anitya/db/migrations/versions/2925648d8cc3_add_a_version_prefix_field.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/2d1aa7ff82a5_remove_code_google_backend.py` & `anitya-1.8.0/anitya/db/migrations/versions/2d1aa7ff82a5_remove_code_google_backend.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/314651690dc7_add_error_counter_to_project.py` & `anitya-1.8.0/anitya/db/migrations/versions/314651690dc7_add_error_counter_to_project.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/34b9bb5fa388_make_ecosystem_non_nullable.py` & `anitya-1.8.0/anitya/db/migrations/versions/34b9bb5fa388_make_ecosystem_non_nullable.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/3fae8239eeec_add_an_api_token_table.py` & `anitya-1.8.0/anitya/db/migrations/versions/3fae8239eeec_add_an_api_token_table.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/540bdcf7edbc_convert_github_url_to_owner_project.py` & `anitya-1.8.0/anitya/db/migrations/versions/540bdcf7edbc_convert_github_url_to_owner_project.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/571bd07533a9_add_insecure_column_to_projects_table.py` & `anitya-1.8.0/anitya/db/migrations/versions/571bd07533a9_add_insecure_column_to_projects_table.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/5b8b587d7dbe_add_version_filter_column.py` & `anitya-1.8.0/anitya/db/migrations/versions/5b8b587d7dbe_add_version_filter_column.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/5e209766aead_add_release_check_to_project.py` & `anitya-1.8.0/anitya/db/migrations/versions/5e209766aead_add_release_check_to_project.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/6ac0e42df937_drop_logs_table.py` & `anitya-1.8.0/anitya/db/migrations/versions/6ac0e42df937_drop_logs_table.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/708f6f26b4b6_add_version_pattern.py` & `anitya-1.8.0/anitya/db/migrations/versions/708f6f26b4b6_add_version_pattern.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/7a8c4aa92678_add_missing_github_owner_project_pairs.py` & `anitya-1.8.0/anitya/db/migrations/versions/7a8c4aa92678_add_missing_github_owner_project_pairs.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/8040ef9a9dda_add_a_version_scheme_column_to_projects.py` & `anitya-1.8.0/anitya/db/migrations/versions/8040ef9a9dda_add_a_version_scheme_column_to_projects.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/8be6e153962c_remove_cursor.py` & `anitya-1.8.0/anitya/db/migrations/versions/8be6e153962c_remove_cursor.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/921c612ba0da_model_upstream_ecosystems.py` & `anitya-1.8.0/anitya/db/migrations/versions/921c612ba0da_model_upstream_ecosystems.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/92a2e9eba0a7_add_project_latest_known_cursor.py` & `anitya-1.8.0/anitya/db/migrations/versions/92a2e9eba0a7_add_project_latest_known_cursor.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/9c29da0af3af_populate_ecosystem_data.py` & `anitya-1.8.0/anitya/db/migrations/versions/9c29da0af3af_populate_ecosystem_data.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/a52d2fe99d4f_users.py` & `anitya-1.8.0/anitya/db/migrations/versions/a52d2fe99d4f_users.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/b9201d816075_remove_the_backends_and_ecosystems_.py` & `anitya-1.8.0/anitya/db/migrations/versions/b9201d816075_remove_the_backends_and_ecosystems_.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/d6170cfc2814_add_pre_release_flag.py` & `anitya-1.8.0/anitya/db/migrations/versions/d6170cfc2814_add_pre_release_flag.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/e34988f3e2f4_add_statistics_to_run.py` & `anitya-1.8.0/anitya/db/migrations/versions/e34988f3e2f4_add_statistics_to_run.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/migrations/versions/feeaa70ead67_social_authentication_table.py` & `anitya-1.8.0/anitya/db/migrations/versions/feeaa70ead67_social_authentication_table.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/db/models.py` & `anitya-1.8.0/anitya/db/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,14 +300,27 @@
 
         Returns:
            list(`anitya.lib.versions.Base`): List of stable version objects
         """
         sorted_versions = self.get_sorted_version_objects()
         return [version for version in sorted_versions if not version.prerelease()]
 
+    @property
+    def latest_stable_version(self):
+        """
+        Return latest stable version.
+
+        Returns:
+           `string`: Latest stable version if exists, otherwise None.
+        """
+        stable_versions = self.stable_versions
+        if stable_versions:
+            return str(stable_versions[0])
+        return None
+
     def get_last_created_version(self):
         """
         Returns last obtained release by date.
 
         Returns:
             (`ProjectVersion`): Version object or None, if project doesn't have any version yet.
         """
```

### Comparing `anitya-1.7.0/anitya/forms.py` & `anitya-1.8.0/anitya/forms.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/__init__.py` & `anitya-1.8.0/anitya/lib/backends/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,14 @@
 
     try:
         upstream_versions = list(set(re.findall(regex, text)))
     except sre_constants.error:  # pragma: no cover
         raise AnityaPluginException("%s: invalid regular expression" % project.name)
 
     for index, version in enumerate(upstream_versions):
-
         # If the version retrieved is a tuple, re-constitute it
         if type(version) == tuple:
             version = ".".join([v for v in version if not v == ""])
 
         upstream_versions[index] = version
 
         if " " in version:
```

### Comparing `anitya-1.7.0/anitya/lib/backends/bitbucket.py` & `anitya-1.8.0/anitya/lib/backends/bitbucket.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/cgit.py` & `anitya-1.8.0/anitya/lib/backends/cgit.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/cpan.py` & `anitya-1.8.0/anitya/lib/backends/cpan.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/cran.py` & `anitya-1.8.0/anitya/lib/backends/cran.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/crates.py` & `anitya-1.8.0/anitya/lib/backends/crates.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/custom.py` & `anitya-1.8.0/anitya/lib/backends/custom.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/debian.py` & `anitya-1.8.0/anitya/lib/backends/debian.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/drupal6.py` & `anitya-1.8.0/anitya/lib/backends/drupal6.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/drupal7.py` & `anitya-1.8.0/anitya/lib/backends/drupal7.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/folder.py` & `anitya-1.8.0/anitya/lib/backends/folder.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/freshmeat.py` & `anitya-1.8.0/anitya/lib/backends/freshmeat.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/github.py` & `anitya-1.8.0/anitya/lib/backends/github.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/gitlab.py` & `anitya-1.8.0/anitya/lib/backends/gitlab.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/gnome.py` & `anitya-1.8.0/anitya/lib/backends/gnome.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/gnu.py` & `anitya-1.8.0/anitya/lib/backends/gnu.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/gogs.py` & `anitya-1.8.0/anitya/lib/backends/gogs.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/hackage.py` & `anitya-1.8.0/anitya/lib/backends/hackage.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/launchpad.py` & `anitya-1.8.0/anitya/lib/backends/launchpad.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/maven.py` & `anitya-1.8.0/anitya/lib/backends/maven.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/npmjs.py` & `anitya-1.8.0/anitya/lib/backends/npmjs.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/packagist.py` & `anitya-1.8.0/anitya/lib/backends/packagist.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/pagure.py` & `anitya-1.8.0/anitya/lib/backends/pagure.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/pear.py` & `anitya-1.8.0/anitya/lib/backends/pear.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/pecl.py` & `anitya-1.8.0/anitya/lib/backends/pecl.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/pypi.py` & `anitya-1.8.0/anitya/lib/backends/pypi.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/rubygems.py` & `anitya-1.8.0/anitya/lib/backends/rubygems.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/sourceforge.py` & `anitya-1.8.0/anitya/lib/backends/sourceforge.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/sourceforge_git.py` & `anitya-1.8.0/anitya/lib/backends/sourceforge_git.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/sourcehut.py` & `anitya-1.8.0/anitya/lib/backends/sourcehut.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/backends/stackage.py` & `anitya-1.8.0/anitya/lib/backends/stackage.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/ecosystems/__init__.py` & `anitya-1.8.0/anitya/lib/ecosystems/__init__.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/ecosystems/crates.py` & `anitya-1.8.0/anitya/lib/ecosystems/crates.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/exceptions.py` & `anitya-1.8.0/anitya/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/plugins.py` & `anitya-1.8.0/anitya/lib/plugins.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/utilities.py` & `anitya-1.8.0/anitya/lib/utilities.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/versions/__init__.py` & `anitya-1.8.0/anitya/lib/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/versions/base.py` & `anitya-1.8.0/anitya/lib/versions/base.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/versions/calver.py` & `anitya-1.8.0/anitya/lib/versions/calver.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/versions/python.py` & `anitya-1.8.0/anitya/lib/versions/python.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/versions/rpm.py` & `anitya-1.8.0/anitya/lib/versions/rpm.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/versions/semver.py` & `anitya-1.8.0/anitya/lib/versions/semver.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/lib/xml2dict.py` & `anitya-1.8.0/anitya/lib/xml2dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 class XML2Dict(object):
     def _parse_node(self, node):
         node_tree = object_dict()
         # Save attrs and text, hope there will not be a child with same name
         if node.text:
             node_tree.value = node.text
-        for (k, v) in node.attrib.items():
+        for k, v in node.attrib.items():
             k, v = self._namespace_split(k, object_dict({"value": v}))
             node_tree[k] = v
         # Save childrens
         for child in list(node):
             tag, tree = self._namespace_split(child.tag, self._parse_node(child))
             # the first time, so store it in dict
             if tag not in node_tree:
```

### Comparing `anitya-1.7.0/anitya/librariesio_consumer.py` & `anitya-1.8.0/anitya/librariesio_consumer.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/mail_logging.py` & `anitya-1.8.0/anitya/mail_logging.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/sar.py` & `anitya-1.8.0/anitya/sar.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/cnucnu.css` & `anitya-1.8.0/anitya/static/css/cnucnu.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-Bold-webfont.eot` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-Bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-Bold-webfont.svg` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-Bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-Bold-webfont.ttf` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-Bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-Bold-webfont.woff` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.eot` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.svg` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.ttf` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.woff` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-BoldOblique-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.eot` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.svg` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.ttf` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.woff` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-Oblique-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-Regular-webfont.eot` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-Regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-Regular-webfont.svg` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-Regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-Regular-webfont.ttf` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-Regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Cantarell-Regular-webfont.woff` & `anitya-1.8.0/anitya/static/css/fonts/Cantarell-Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.eot` & `anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.svg` & `anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.ttf` & `anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.woff` & `anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.eot` & `anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.svg` & `anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.ttf` & `anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.woff` & `anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.eot` & `anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.eot`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.svg` & `anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.svg`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.ttf` & `anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.ttf`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.woff` & `anitya-1.8.0/anitya/static/css/fonts/Comfortaa_Thin-webfont.woff`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/images/ui-icons_0073ea_256x240.png` & `anitya-1.8.0/anitya/static/css/images/ui-icons_0073ea_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/images/ui-icons_454545_256x240.png` & `anitya-1.8.0/anitya/static/css/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/images/ui-icons_666666_256x240.png` & `anitya-1.8.0/anitya/static/css/images/ui-icons_666666_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/images/ui-icons_ff0084_256x240.png` & `anitya-1.8.0/anitya/static/css/images/ui-icons_ff0084_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/css/text.css` & `anitya-1.8.0/anitya/static/css/text.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_images/database.png` & `anitya-1.8.0/anitya/static/docs/_images/database.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/anitya/db/events.html` & `anitya-1.8.0/anitya/static/docs/_modules/anitya/db/events.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/anitya/db/meta.html` & `anitya-1.8.0/anitya/static/docs/_modules/anitya/db/meta.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/anitya/db/models.html` & `anitya-1.8.0/anitya/static/docs/_modules/anitya/db/models.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/anitya/lib/backends.html` & `anitya-1.8.0/anitya/static/docs/_modules/anitya/lib/backends.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/anitya/lib/ecosystems.html` & `anitya-1.8.0/anitya/static/docs/_modules/anitya/lib/ecosystems.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/anitya/lib/exceptions.html` & `anitya-1.8.0/anitya/static/docs/_modules/anitya/lib/exceptions.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/anitya/lib/plugins.html` & `anitya-1.8.0/anitya/static/docs/_modules/anitya/lib/plugins.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/anitya/lib/versions/base.html` & `anitya-1.8.0/anitya/static/docs/_modules/anitya/lib/versions/base.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/index.html` & `anitya-1.8.0/anitya/static/docs/_modules/index.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/sqlalchemy/ext/declarative/api.html` & `anitya-1.8.0/anitya/static/docs/_modules/sqlalchemy/ext/declarative/api.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/sqlalchemy/orm/attributes.html` & `anitya-1.8.0/anitya/static/docs/_modules/sqlalchemy/orm/attributes.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/sqlalchemy/orm/scoping.html` & `anitya-1.8.0/anitya/static/docs/_modules/sqlalchemy/orm/scoping.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/sqlalchemy/sql/schema.html` & `anitya-1.8.0/anitya/static/docs/_modules/sqlalchemy/sql/schema.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_modules/sqlalchemy/sql/sqltypes.html` & `anitya-1.8.0/anitya/static/docs/_modules/sqlalchemy/sql/sqltypes.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_sources/admin-guide.rst.txt` & `anitya-1.8.0/anitya/static/docs/_sources/admin-guide.rst.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_sources/admin-user-guide.rst.txt` & `anitya-1.8.0/anitya/static/docs/_sources/admin-user-guide.rst.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_sources/api.rst.txt` & `anitya-1.8.0/anitya/static/docs/_sources/api.rst.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_sources/contributing.rst.txt` & `anitya-1.8.0/anitya/static/docs/_sources/contributing.rst.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_sources/index.rst.txt` & `anitya-1.8.0/anitya/static/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_sources/integrating-with-anitya.rst.txt` & `anitya-1.8.0/anitya/static/docs/_sources/integrating-with-anitya.rst.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_sources/release-monitoring-admin-guide.rst.txt` & `anitya-1.8.0/anitya/static/docs/_sources/release-monitoring-admin-guide.rst.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_sources/release-notes.rst.txt` & `anitya-1.8.0/anitya/static/docs/_sources/release-notes.rst.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_sources/user-guide.rst.txt` & `anitya-1.8.0/anitya/static/docs/_sources/user-guide.rst.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_static/alabaster.css` & `anitya-1.8.0/anitya/static/docs/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_static/basic.css` & `anitya-1.8.0/anitya/static/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_static/doctools.js` & `anitya-1.8.0/anitya/static/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_static/jquery-3.4.1.js` & `anitya-1.8.0/anitya/static/docs/_static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_static/jquery-3.5.1.js` & `anitya-1.8.0/anitya/static/docs/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_static/jquery.js` & `anitya-1.8.0/anitya/static/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_static/language_data.js` & `anitya-1.8.0/anitya/static/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_static/pygments.css` & `anitya-1.8.0/anitya/static/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_static/searchtools.js` & `anitya-1.8.0/anitya/static/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_static/underscore-1.3.1.js` & `anitya-1.8.0/anitya/static/docs/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/_static/underscore.js` & `anitya-1.8.0/anitya/static/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/admin-guide.html` & `anitya-1.8.0/anitya/static/docs/admin-guide.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/admin-user-guide.html` & `anitya-1.8.0/anitya/static/docs/admin-user-guide.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/api.html` & `anitya-1.8.0/anitya/static/docs/api.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/contributing.html` & `anitya-1.8.0/anitya/static/docs/contributing.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/database.html` & `anitya-1.8.0/anitya/static/docs/database.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/docblocks/anitya.db.models.html` & `anitya-1.8.0/anitya/static/docs/docblocks/anitya.db.models.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/genindex.html` & `anitya-1.8.0/anitya/static/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/glossary.html` & `anitya-1.8.0/anitya/static/docs/glossary.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/http-routingtable.html` & `anitya-1.8.0/anitya/static/docs/http-routingtable.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/index.html` & `anitya-1.8.0/anitya/static/docs/index.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/integrating-with-anitya.html` & `anitya-1.8.0/anitya/static/docs/integrating-with-anitya.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/objects.inv` & `anitya-1.8.0/anitya/static/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/py-modindex.html` & `anitya-1.8.0/anitya/static/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/release-monitoring-admin-guide.html` & `anitya-1.8.0/anitya/static/docs/release-monitoring-admin-guide.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/release-notes.html` & `anitya-1.8.0/anitya/static/docs/release-notes.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/search.html` & `anitya-1.8.0/anitya/static/docs/search.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/searchindex.js` & `anitya-1.8.0/anitya/static/docs/searchindex.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/docs/user-guide.html` & `anitya-1.8.0/anitya/static/docs/user-guide.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/google_logo.png` & `anitya-1.8.0/anitya/static/google_logo.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/ico/favicon.ico` & `anitya-1.8.0/anitya/static/ico/favicon.ico`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/img/spinner.gif` & `anitya-1.8.0/anitya/static/img/spinner.gif`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/.package-lock.json` & `anitya-1.8.0/anitya/static/node_modules/.package-lock.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'lockfileVersion'": '3'}*

```diff
@@ -1,9 +1,9 @@
 {
-    "lockfileVersion": 2,
+    "lockfileVersion": 3,
     "name": "anitya",
     "packages": {
         "node_modules/@popperjs/core": {
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/popperjs"
             },
```

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/LICENSE.md` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/LICENSE.md`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/README.md` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/README.md`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/enums.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/enums.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/enums.js.map` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/enums.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-base.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-base.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-base.js.map` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-base.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js.map` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper-lite.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper.js.map` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/cjs/popper.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/createPopper.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/createPopper.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/contains.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/contains.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getBoundingClientRect.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getBoundingClientRect.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getClippingRect.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getClippingRect.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getCompositeRect.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getCompositeRect.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getDocumentRect.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getDocumentRect.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getLayoutRect.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getLayoutRect.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getOffsetParent.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getOffsetParent.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getParentNode.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getParentNode.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getScrollParent.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getScrollParent.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getViewportRect.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getViewportRect.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindowScrollBarX.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/getWindowScrollBarX.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/instanceOf.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/instanceOf.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/listScrollParents.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/dom-utils/listScrollParents.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/enums.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/enums.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/applyStyles.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/applyStyles.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/arrow.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/arrow.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/computeStyles.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/computeStyles.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/eventListeners.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/eventListeners.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/flip.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/flip.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/hide.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/hide.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/offset.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/offset.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/popperOffsets.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/popperOffsets.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/preventOverflow.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/modifiers/preventOverflow.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/popper-lite.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/popper-lite.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/popper.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/popper.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/computeAutoPlacement.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/computeAutoPlacement.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/computeOffsets.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/computeOffsets.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/detectOverflow.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/detectOverflow.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/mergeByName.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/mergeByName.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/orderModifiers.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/orderModifiers.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/validateModifiers.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/esm/utils/validateModifiers.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.js.map` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.min.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.min.js.map` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/enums.min.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.js.map` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js.map` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-base.min.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.js.map` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js.map` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper-lite.min.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.js.map` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.min.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.min.js.map` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/dist/umd/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/createPopper.d.ts` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/createPopper.d.ts`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/createPopper.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/createPopper.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/createPopper.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/createPopper.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/contains.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/contains.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/contains.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/contains.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getBoundingClientRect.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getClippingRect.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getCompositeRect.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getDocumentRect.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getLayoutRect.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getOffsetParent.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getParentNode.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getScrollParent.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getViewportRect.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/getWindowScrollBarX.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/instanceOf.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/dom-utils/listScrollParents.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/enums.d.ts` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/enums.d.ts`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/enums.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/enums.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/enums.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/enums.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/applyStyles.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/arrow.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/arrow.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/arrow.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/arrow.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.d.ts` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.d.ts`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/computeStyles.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/eventListeners.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.d.ts` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.d.ts`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/flip.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/hide.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/hide.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/hide.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/hide.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.d.ts` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.d.ts`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/offset.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/popperOffsets.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.d.ts` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.d.ts`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/modifiers/preventOverflow.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper-lite.d.ts` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper-lite.d.ts`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper-lite.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper-lite.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper-lite.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper-lite.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper.d.ts` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper.d.ts`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/popper.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/popper.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/types.d.ts` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/types.d.ts`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/types.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/types.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeAutoPlacement.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeOffsets.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeOffsets.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeOffsets.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/computeOffsets.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/detectOverflow.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/detectOverflow.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/detectOverflow.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/detectOverflow.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergeByName.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergeByName.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergeByName.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/mergeByName.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/orderModifiers.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/orderModifiers.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/orderModifiers.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/orderModifiers.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/validateModifiers.js` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/validateModifiers.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/lib/utils/validateModifiers.js.flow` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/lib/utils/validateModifiers.js.flow`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/@popperjs/core/package.json` & `anitya-1.8.0/anitya/static/node_modules/@popperjs/core/package.json`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/LICENSE` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/LICENSE`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/README.md` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/README.md`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.min.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.min.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.min.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.min.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.min.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.min.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.min.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.min.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.min.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.min.css` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.min.css.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.min.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.min.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.min.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.min.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/alert.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/alert.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/alert.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/alert.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/base-component.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/base-component.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/base-component.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/base-component.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/button.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/button.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/button.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/button.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/carousel.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/carousel.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/carousel.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/carousel.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/collapse.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/collapse.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/collapse.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/collapse.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/data.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/data.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/data.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/data.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/event-handler.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/event-handler.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/event-handler.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/event-handler.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/manipulator.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/manipulator.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/manipulator.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/manipulator.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/selector-engine.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/selector-engine.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dom/selector-engine.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dom/selector-engine.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dropdown.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dropdown.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/dropdown.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/dropdown.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/modal.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/modal.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/modal.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/modal.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/offcanvas.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/offcanvas.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/offcanvas.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/offcanvas.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/popover.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/popover.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/popover.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/popover.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/scrollspy.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/scrollspy.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/scrollspy.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/scrollspy.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/tab.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/tab.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/tab.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/tab.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/toast.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/toast.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/toast.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/toast.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/tooltip.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/tooltip.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/tooltip.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/tooltip.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/backdrop.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/backdrop.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/backdrop.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/backdrop.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/component-functions.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/component-functions.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/component-functions.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/component-functions.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/config.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/config.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/config.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/config.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/focustrap.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/focustrap.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/focustrap.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/focustrap.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/index.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/index.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/index.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/index.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/sanitizer.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/sanitizer.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/sanitizer.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/sanitizer.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/scrollbar.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/scrollbar.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/scrollbar.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/scrollbar.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/swipe.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/swipe.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/swipe.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/swipe.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/template-factory.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/template-factory.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/dist/util/template-factory.js.map` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/dist/util/template-factory.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/alert.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/alert.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/base-component.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/base-component.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/button.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/button.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/carousel.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/carousel.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/collapse.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/collapse.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/dom/data.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/dom/data.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/dom/event-handler.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/dom/event-handler.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/dom/manipulator.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/dom/manipulator.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/dom/selector-engine.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/dom/selector-engine.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/dropdown.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/dropdown.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/modal.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/modal.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/offcanvas.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/offcanvas.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/popover.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/popover.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/scrollspy.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/scrollspy.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/tab.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/tab.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/toast.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/toast.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/tooltip.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/tooltip.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/backdrop.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/backdrop.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/component-functions.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/component-functions.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/config.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/config.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/focustrap.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/focustrap.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/index.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/index.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/sanitizer.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/sanitizer.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/scrollbar.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/scrollbar.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/swipe.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/swipe.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/js/src/util/template-factory.js` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/js/src/util/template-factory.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/package.json` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/package.json`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_accordion.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_alert.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_badge.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_breadcrumb.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_button-group.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_buttons.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_card.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_carousel.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_close.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_containers.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_dropdown.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_functions.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_grid.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_grid.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_images.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_list-group.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_maps.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_maps.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_mixins.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_modal.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_nav.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_navbar.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_offcanvas.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_pagination.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_placeholders.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_placeholders.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_popover.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_progress.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_reboot.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_root.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_spinners.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_tables.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_toasts.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_tooltip.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_type.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_utilities.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/_variables.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/bootstrap-grid.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/bootstrap.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_floating-labels.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_form-check.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_form-control.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_form-range.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_form-select.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_input-group.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/forms/_labels.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/helpers/_position.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/helpers/_position.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_border-radius.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_breakpoints.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_buttons.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_caret.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_deprecate.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_forms.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_gradients.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_grid.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_table-variants.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_transition.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_utilities.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/mixins/_visually-hidden.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/utilities/_api.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/bootstrap/scss/vendor/_rfs.scss` & `anitya-1.8.0/anitya/static/node_modules/bootstrap/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/AUTHORS.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/README.md` & `anitya-1.8.0/anitya/static/node_modules/jquery/README.md`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/dist/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/dist/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/dist/jquery.min.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/dist/jquery.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/dist/jquery.min.map` & `anitya-1.8.0/anitya/static/node_modules/jquery/dist/jquery.min.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/dist/jquery.slim.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/dist/jquery.slim.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/dist/jquery.slim.min.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/dist/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/dist/jquery.slim.min.map` & `anitya-1.8.0/anitya/static/node_modules/jquery/dist/jquery.slim.min.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/external/sizzle/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery/external/sizzle/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.min.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.min.map` & `anitya-1.8.0/anitya/static/node_modules/jquery/external/sizzle/dist/sizzle.min.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/package.json` & `anitya-1.8.0/anitya/static/node_modules/jquery/package.json`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/ajax/jsonp.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/ajax/jsonp.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/ajax/load.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/ajax/load.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/ajax/script.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/ajax/script.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/ajax/xhr.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/ajax/xhr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/ajax.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/ajax.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/attributes/attr.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/attributes/attr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/attributes/classes.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/attributes/classes.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/attributes/prop.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/attributes/prop.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/attributes/support.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/attributes/support.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/attributes/val.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/attributes/val.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/callbacks.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/callbacks.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/core/DOMEval.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/core/DOMEval.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/core/access.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/core/access.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/core/camelCase.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/core/camelCase.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/core/init.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/core/init.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/core/isAttached.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/core/isAttached.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/core/parseHTML.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/core/parseHTML.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/core/parseXML.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/core/parseXML.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/core/ready-no-deferred.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/core/ready-no-deferred.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/core/ready.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/core/ready.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/core/support.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/core/support.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/core.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/core.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/css/addGetHookIf.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/css/addGetHookIf.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/css/adjustCSS.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/css/adjustCSS.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/css/curCSS.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/css/curCSS.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/css/finalPropName.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/css/finalPropName.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/css/showHide.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/css/showHide.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/css/support.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/css/support.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/css/var/isHiddenWithinTree.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/css/var/isHiddenWithinTree.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/css.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/css.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/data/Data.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/data/Data.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/data.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/data.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/deferred/exceptionHook.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/deferred/exceptionHook.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/deferred.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/deferred.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/deprecated/event.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/deprecated/event.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/deprecated.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/deprecated.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/dimensions.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/dimensions.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/effects/Tween.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/effects/Tween.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/effects.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/effects.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/event/focusin.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/event/focusin.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/event/trigger.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/event/trigger.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/event.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/event.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/exports/amd.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/exports/amd.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/exports/global.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/exports/global.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation/_evalUrl.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation/_evalUrl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation/buildFragment.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation/buildFragment.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation/getAll.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation/getAll.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation/support.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation/support.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation/wrapMap.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation/wrapMap.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/manipulation.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/manipulation.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/offset.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/offset.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/queue/delay.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/queue/delay.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/queue.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/queue.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/selector-native.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/selector-native.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/serialize.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/serialize.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/traversing/findFilter.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/traversing/findFilter.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/traversing.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/traversing.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/var/isFunction.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/var/isFunction.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery/src/wrap.js` & `anitya-1.8.0/anitya/static/node_modules/jquery/src/wrap.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/.github/workflows/test.yml` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/AUTHORS.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/CONTRIBUTING.md` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/README.md` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/README.md`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/bower.json` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/bower.json`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/build/release-test.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/build/release-test.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/build/release.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/build/release.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/build/tasks/build.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/build/tasks/build.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/build/tasks/testswarm.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/build/tasks/testswarm.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/build/themes` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/build/themes`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/jquery-ui.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/jquery-ui.min.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_444444_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_555555_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_777620_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_777777_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_cc0000_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/base/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/base/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_222222_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_4ca300_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_4ca300_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_bbbbbb_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_bbbbbb_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ededed_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ededed_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ffcf29_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ffcf29_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/black-tie/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_diagonals-thick_75_f3d8d8_40x40.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-bg_diagonals-thick_75_f3d8d8_40x40.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_004276_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_004276_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_cc0000_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/blitzer/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_2694e8_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_2694e8_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_2e83ff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_3d80b3_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_3d80b3_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_72a7cf_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_72a7cf_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/cupertino/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_222222_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_4b8e0b_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_4b8e0b_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_a83300_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_a83300_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_cccccc_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_cccccc_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dark-hive/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_diagonals-thick_15_0b3e6f_40x40.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_diagonals-thick_15_0b3e6f_40x40.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_gloss-wave_20_111111_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-bg_gloss-wave_20_111111_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_00498f_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_00498f_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_98d2fb_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_98d2fb_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_9ccdfc_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_9ccdfc_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/dot-luv/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_gloss-wave_30_3d3644_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-bg_gloss-wave_30_3d3644_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_454545_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_734d99_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_734d99_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_8d78a5_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_8d78a5_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_a8a3ae_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_a8a3ae_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_ebccce_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_ebccce_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/eggplant/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_20_e69700_40x40.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_20_e69700_40x40.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_22_1484e6_40x40.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_22_1484e6_40x40.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_26_2293f7_40x40.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-bg_diagonals-thick_26_2293f7_40x40.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_0a82eb_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_0a82eb_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_0b54d5_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_0b54d5_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_5fa5e3_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_5fa5e3_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_fcdd4a_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_fcdd4a_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/excite-bike/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_0073ea_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_0073ea_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_454545_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_666666_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_666666_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_ff0084_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_ff0084_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/flick/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_454545_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_88a206_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_88a206_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_c02669_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_c02669_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_e1e463_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_e1e463_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_ffeb33_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_ffeb33_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/hot-sneaks/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_inset-soft_100_f4f0ec_1x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-bg_inset-soft_100_f4f0ec_1x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_c47a23_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_c47a23_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_cb672b_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_cb672b_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_f08000_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_f08000_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_f35f07_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_f35f07_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_ff7519_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_ff7519_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/humanity/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_diagonals-thick_95_ffdc2e_40x40.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-bg_diagonals-thick_95_ffdc2e_40x40.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_4eb305_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_4eb305_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_72b42d_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_72b42d_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_cd0a0a_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/le-frog/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_20_1c160d_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_20_1c160d_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_25_453326_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_25_453326_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_30_44372c_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-bg_gloss-wave_30_44372c_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_222222_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_9bcc60_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_9bcc60_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_add978_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_add978_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_e3ddc9_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_e3ddc9_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_f1fd86_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_f1fd86_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/mint-choc/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_3383bb_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_3383bb_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_454545_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_70b2e1_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_70b2e1_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_999999_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_999999_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_fbc856_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/images/ui-icons_fbc856_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/overcast/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_10_eceadf_60x60.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_10_eceadf_60x60.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_10_f8f7f6_60x60.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_10_f8f7f6_60x60.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_eceadf_60x60.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_eceadf_60x60.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_f7f3de_60x60.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_f7f3de_60x60.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_ffffff_60x60.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_15_ffffff_60x60.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_65_654b24_60x60.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_65_654b24_60x60.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_68_b83400_60x60.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-bg_fine-grain_68_b83400_60x60.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_222222_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_3572ac_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_3572ac_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_8c291d_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_8c291d_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_b83400_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_b83400_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_fbdb93_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_fbdb93_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/pepper-grinder/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_gloss-wave_55_5c9ccc_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-bg_gloss-wave_55_5c9ccc_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_217bc0_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_217bc0_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_2e83ff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_469bdd_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_469bdd_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_6da8d5_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_6da8d5_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_cd0a0a_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_d8e7f3_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_d8e7f3_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_f9bd01_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/images/ui-icons_f9bd01_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/redmond/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_222222_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_2e83ff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_454545_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_888888_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_cd0a0a_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/smoothness/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_gloss-wave_100_ece8da_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-bg_gloss-wave_100_ece8da_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_808080_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_808080_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_847e71_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_847e71_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_8DC262_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_8DC262_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_cd0a0a_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_eeeeee_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_eeeeee_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/south-street/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_45_e14f1c_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_45_e14f1c_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_50_6eac2c_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_50_6eac2c_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_75_2191c0_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-bg_gloss-wave_75_2191c0_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_0078ae_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_0078ae_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_056b93_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_056b93_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_d8e7f3_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_d8e7f3_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_e0fdff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_e0fdff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_f5e175_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_f5e175_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_f7a50d_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_f7a50d_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_fcd113_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/images/ui-icons_fcd113_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/start/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/start/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_45_817865_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_45_817865_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_60_fece2f_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_60_fece2f_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_70_ffdd57_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_70_ffdd57_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_90_fff9e5_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-bg_gloss-wave_90_fff9e5_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_3d3d3d_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_3d3d3d_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_bd7b00_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_bd7b00_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_d19405_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_d19405_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_eb990f_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_eb990f_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_ed9f26_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_ed9f26_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_fadc7a_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_fadc7a_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_ffe180_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/images/ui-icons_ffe180_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/sunny/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_070603_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_070603_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_e8e2b5_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_e8e2b5_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_e9cd86_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_e9cd86_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_efec9f_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_efec9f_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_f2ec64_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_f2ec64_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_f9f2bd_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_f9f2bd_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_ff7519_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/images/ui-icons_ff7519_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/swanky-purse/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_55_000000_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_55_000000_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_85_9fda58_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_85_9fda58_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_95_f6ecd5_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-bg_gloss-wave_95_f6ecd5_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_000000_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_000000_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_1f1f1f_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_1f1f1f_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_9fda58_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_9fda58_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_b8ec79_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_b8ec79_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_cd0a0a_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/trontastic/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_gloss-wave_25_333333_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-bg_gloss-wave_25_333333_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_222222_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_4b8e0b_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_4b8e0b_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_a83300_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_a83300_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_cccccc_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_cccccc_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-darkness/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_diagonals-thick_18_b81900_40x40.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_diagonals-thick_18_b81900_40x40.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_gloss-wave_35_f6a828_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-bg_gloss-wave_35_f6a828_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_222222_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_228ef1_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_228ef1_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ef8c08_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ef8c08_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ffd27a_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ffd27a_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/ui-lightness/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_gloss-wave_16_121212_500x100.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-bg_gloss-wave_16_121212_500x100.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_666666_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_666666_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_777777_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_aaaaaa_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_aaaaaa_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_c98000_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_c98000_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_cccccc_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_cccccc_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_cd0a0a_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_f29a00_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/images/ui-icons_f29a00_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/jquery-ui.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/jquery-ui.min.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/dist/themes/vader/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/globalize/LICENSE` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/globalize/LICENSE`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/globalize/globalize.culture.de-DE.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/globalize/globalize.culture.de-DE.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/globalize/globalize.culture.ja-JP.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/globalize/globalize.culture.ja-JP.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/globalize/globalize.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/globalize/globalize.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.0/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.0/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.1/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.1/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.1/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.1/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.2/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.2/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.2/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.10.2/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.0/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.0/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.1/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.1/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.1/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.1/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.2/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.2/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.2/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.2/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.3/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.3/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.3/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.11.3/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.0/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.1/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.1/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.1/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.2/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.2/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.2/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.3/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.3/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.3/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.4/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.4/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.12.4/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.0/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.0/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.1/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.1/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.1/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.1/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.2/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.2/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.2/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.2/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.3/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.3/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.3/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.8.3/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.0/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.0/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.1/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.1/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.1/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-1.9.1/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.0/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.0/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.1/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.1/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.1/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.1/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.2/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.2/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.2/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.2/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.3/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.3/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.3/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.0.3/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.0/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.0/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.1/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.1/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.1/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.1/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.2/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.2/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.2/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.2/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.3/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.3/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.3/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.3/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.4/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.4/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.4/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.1.4/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.0/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.1/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.1/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.1/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.2/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.2/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.2/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.3/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.3/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.3/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.4/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.4/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-2.2.4/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.0.0/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.0.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.0.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.0/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.1/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.1/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.1.1/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.0/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.1/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.1/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.2.1/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.0/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.1/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.1/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.3.1/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.0/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.1/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.1/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.4.1/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.0/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.1/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.1/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.5.1/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.6.0/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-3.6.0/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-3.6.0/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-custom/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-custom/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-custom/jquery.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-custom/jquery.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-1.4.1/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-1.4.1/jquery-migrate.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-1.4.1/jquery-migrate.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-3.3.2/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-3.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-3.3.2/jquery-migrate.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-migrate-3.3.2/jquery-migrate.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-mousewheel/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-mousewheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-mousewheel/jquery.mousewheel.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-mousewheel/jquery.mousewheel.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-simulate/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-simulate/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/jquery-simulate/jquery.simulate.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/jquery-simulate/jquery.simulate.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit/qunit.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit/qunit.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit/qunit.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit/qunit.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-classes/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-classes/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-classes/qunit-assert-classes.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-classes/qunit-assert-classes.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-close/MIT-LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-close/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-close/qunit-assert-close.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit-assert-close/qunit-assert-close.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit-composite/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit-composite/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/qunit-composite/qunit-composite.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/qunit-composite/qunit-composite.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/external/requirejs/require.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/external/requirejs/require.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/package.json` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/package.json`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/base.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/base.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/button.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/button.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/checkboxradio.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/checkboxradio.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/controlgroup.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/controlgroup.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/core.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/core.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/datepicker.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/datepicker.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/dialog.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/dialog.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_444444_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_555555_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_777620_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_777777_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_cc0000_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_ffffff_256x240.png` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/menu.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/menu.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/progressbar.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/progressbar.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/resizable.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/resizable.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/selectmenu.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/selectmenu.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/slider.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/slider.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/spinner.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/spinner.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/tabs.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/tabs.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/themes/base/theme.css` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/themes/base/theme.css`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/data.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/data.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/disable-selection.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/disable-selection.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effect.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effect.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-blind.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-blind.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-bounce.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-bounce.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-clip.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-clip.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-drop.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-drop.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-explode.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-explode.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-fade.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-fade.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-fold.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-fold.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-highlight.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-highlight.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-puff.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-puff.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-pulsate.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-pulsate.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-scale.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-scale.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-shake.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-shake.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-size.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-size.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-slide.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-slide.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-transfer.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/effects/effect-transfer.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/focusable.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/focusable.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/form-reset-mixin.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/form-reset-mixin.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/form.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/form.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-af.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-af.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ar-DZ.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ar-DZ.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ar.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ar.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-az.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-az.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-be.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-be.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-bg.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-bg.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-bs.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-bs.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ca.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ca.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-cs.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-cs.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-cy-GB.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-cy-GB.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-da.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-da.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-de-AT.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-de-AT.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-de.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-de.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-el.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-el.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-AU.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-AU.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-GB.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-GB.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-NZ.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-en-NZ.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-eo.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-eo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-es.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-es.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-et.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-et.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-eu.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-eu.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fa.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fa.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fi.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fo.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr-CA.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr-CA.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr-CH.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr-CH.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-fr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-gl.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-gl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-he.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-he.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hi.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hr.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hu.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hu.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hy.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-hy.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-id.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-id.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-is.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-is.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-it-CH.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-it-CH.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-it.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-it.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ja.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ja.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ka.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ka.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-kk.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-kk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-km.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-km.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ko.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ko.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ky.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ky.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lb.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lb.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lt.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lt.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lv.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-lv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-mk.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-mk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ml.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ml.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ms.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ms.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nb.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nb.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nl-BE.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nl-BE.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nl.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nn.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-nn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-no.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-no.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pl.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pt-BR.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pt-BR.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pt.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-pt.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-rm.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-rm.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ro.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ro.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ru.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ru.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sk.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sl.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sq.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sq.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sr-SR.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sr-SR.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sr.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sv.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-sv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ta.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-ta.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-th.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-th.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-tj.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-tj.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-tr.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-tr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-uk.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-uk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-vi.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-vi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-CN.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-CN.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-HK.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-HK.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-TW.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/i18n/datepicker-zh-TW.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/jquery-patch.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/jquery-patch.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/jquery-var-for-color.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/jquery-var-for-color.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/keycode.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/keycode.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/labels.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/labels.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/plugin.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/plugin.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/position.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/position.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/safe-active-element.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/safe-active-element.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/safe-blur.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/safe-blur.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/scroll-parent.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/scroll-parent.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/tabbable.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/tabbable.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/unique-id.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/unique-id.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/vendor/jquery-color/LICENSE.txt` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/vendor/jquery-color/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/vendor/jquery-color/jquery.color.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/vendor/jquery-color/jquery.color.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widget.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widget.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/accordion.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/accordion.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/autocomplete.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/autocomplete.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/button.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/button.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/checkboxradio.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/checkboxradio.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/controlgroup.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/controlgroup.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/datepicker.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/datepicker.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/dialog.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/dialog.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/draggable.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/draggable.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/droppable.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/droppable.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/menu.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/menu.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/mouse.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/mouse.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/progressbar.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/progressbar.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/resizable.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/resizable.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/selectable.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/selectable.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/selectmenu.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/selectmenu.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/slider.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/slider.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/sortable.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/sortable.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/spinner.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/spinner.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/tabs.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/tabs.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/jquery-ui/ui/widgets/tooltip.js` & `anitya-1.8.0/anitya/static/node_modules/jquery-ui/ui/widgets/tooltip.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/CHANGELOG.md` & `anitya-1.8.0/anitya/static/node_modules/moment/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/LICENSE` & `anitya-1.8.0/anitya/static/node_modules/moment/LICENSE`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/README.md` & `anitya-1.8.0/anitya/static/node_modules/moment/README.md`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/af.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/af.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar-dz.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar-dz.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar-kw.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar-kw.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar-ly.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar-ly.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar-ma.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar-ma.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar-sa.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar-sa.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar-tn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar-tn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ar.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ar.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/az.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/az.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/be.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/be.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/bg.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/bg.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/bm.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/bm.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/bn-bd.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/bn-bd.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/bn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/bn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/bo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/bo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/br.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/br.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/bs.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/bs.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ca.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ca.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/cs.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/cs.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/cv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/cv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/cy.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/cy.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/da.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/da.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/de-at.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/de-at.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/de-ch.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/de-ch.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/de.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/de.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/dv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/dv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/el.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/el.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-au.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-au.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-ca.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-ca.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-gb.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-gb.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-ie.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-ie.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-il.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-il.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-in.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-in.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-nz.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-nz.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/en-sg.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/en-sg.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/eo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/eo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/es-do.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/es-do.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/es-mx.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/es-mx.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/es-us.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/es-us.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/es.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/es.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/et.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/et.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/eu.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/eu.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fa.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fa.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fi.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fil.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fil.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fr-ca.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fr-ca.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fr-ch.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fr-ch.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/fy.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/fy.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ga.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ga.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/gd.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/gd.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/gl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/gl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/gom-deva.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/gom-deva.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/gom-latn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/gom-latn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/gu.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/gu.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/he.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/he.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/hi.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/hi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/hr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/hr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/hu.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/hu.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/hy-am.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/hy-am.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/id.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/id.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/is.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/is.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/it-ch.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/it-ch.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/it.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/it.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ja.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ja.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/jv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/jv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ka.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ka.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/kk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/kk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/km.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/km.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/kn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/kn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ko.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ko.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ku.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ku.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ky.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ky.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/lb.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/lb.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/lo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/lo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/lt.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/lt.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/lv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/lv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/me.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/me.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/mi.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/mi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/mk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/mk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ml.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ml.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/mn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/mn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/mr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/mr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ms-my.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ms-my.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ms.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ms.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/mt.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/mt.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/my.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/my.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/nb.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/nb.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ne.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ne.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/nl-be.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/nl-be.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/nl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/nl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/nn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/nn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/oc-lnc.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/oc-lnc.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/pa-in.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/pa-in.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/pl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/pl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/pt-br.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/pt-br.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/pt.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/pt.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ro.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ro.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ru.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ru.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sd.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sd.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/se.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/se.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/si.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/si.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sq.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sq.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sr-cyrl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sr-cyrl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ss.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ss.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/sw.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/sw.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ta.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ta.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/te.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/te.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tet.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tet.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tg.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tg.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/th.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/th.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tl-ph.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tl-ph.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tlh.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tlh.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tzl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tzl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tzm-latn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tzm-latn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/tzm.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/tzm.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ug-cn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ug-cn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/uk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/uk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/ur.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/ur.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/uz-latn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/uz-latn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/uz.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/uz.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/vi.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/vi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/x-pseudo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/x-pseudo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/yo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/yo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/zh-cn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/zh-cn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/zh-hk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/zh-hk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/zh-mo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/zh-mo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/locale/zh-tw.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/locale/zh-tw.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/dist/moment.js` & `anitya-1.8.0/anitya/static/node_modules/moment/dist/moment.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/af.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/af.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ar-dz.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ar-dz.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ar-kw.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ar-kw.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ar-ly.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ar-ly.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ar-ma.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ar-ma.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ar-sa.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ar-sa.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ar-tn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ar-tn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ar.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ar.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/az.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/az.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/be.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/be.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/bg.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/bg.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/bm.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/bm.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/bn-bd.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/bn-bd.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/bn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/bn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/bo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/bo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/br.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/br.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/bs.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/bs.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ca.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ca.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/cs.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/cs.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/cv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/cv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/cy.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/cy.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/da.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/da.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/de-at.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/de-at.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/de-ch.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/de-ch.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/de.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/de.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/dv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/dv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/el.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/el.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/en-au.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/en-au.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/en-ca.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/en-ca.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/en-gb.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/en-gb.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/en-ie.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/en-ie.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/en-il.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/en-il.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/en-in.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/en-in.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/en-nz.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/en-nz.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/en-sg.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/en-sg.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/eo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/eo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/es-do.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/es-do.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/es-mx.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/es-mx.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/es-us.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/es-us.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/es.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/es.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/et.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/et.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/eu.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/eu.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/fa.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/fa.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/fi.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/fi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/fil.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/fil.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/fo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/fo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/fr-ca.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/fr-ca.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/fr-ch.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/fr-ch.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/fr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/fr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/fy.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/fy.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ga.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ga.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/gd.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/gd.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/gl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/gl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/gom-deva.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/gom-deva.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/gom-latn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/gom-latn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/gu.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/gu.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/he.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/he.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/hi.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/hi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/hr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/hr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/hu.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/hu.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/hy-am.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/hy-am.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/id.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/id.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/is.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/is.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/it-ch.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/it-ch.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/it.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/it.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ja.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ja.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/jv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/jv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ka.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ka.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/kk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/kk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/km.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/km.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/kn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/kn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ko.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ko.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ku.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ku.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ky.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ky.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/lb.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/lb.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/lo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/lo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/lt.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/lt.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/lv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/lv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/me.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/me.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/mi.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/mi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/mk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/mk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ml.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ml.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/mn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/mn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/mr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/mr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ms-my.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ms-my.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ms.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ms.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/mt.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/mt.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/my.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/my.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/nb.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/nb.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ne.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ne.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/nl-be.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/nl-be.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/nl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/nl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/nn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/nn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/oc-lnc.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/oc-lnc.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/pa-in.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/pa-in.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/pl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/pl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/pt-br.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/pt-br.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/pt.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/pt.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ro.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ro.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ru.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ru.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/sd.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/sd.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/se.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/se.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/si.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/si.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/sk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/sk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/sl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/sl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/sq.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/sq.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/sr-cyrl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/sr-cyrl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/sr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/sr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ss.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ss.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/sv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/sv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/sw.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/sw.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ta.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ta.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/te.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/te.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/tet.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/tet.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/tg.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/tg.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/th.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/th.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/tk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/tk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/tl-ph.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/tl-ph.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/tlh.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/tlh.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/tr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/tr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/tzl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/tzl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/tzm-latn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/tzm-latn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/tzm.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/tzm.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ug-cn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ug-cn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/uk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/uk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/ur.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/ur.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/uz-latn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/uz-latn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/uz.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/uz.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/vi.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/vi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/x-pseudo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/x-pseudo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/yo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/yo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/zh-cn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/zh-cn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/zh-hk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/zh-hk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/zh-mo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/zh-mo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/locale/zh-tw.js` & `anitya-1.8.0/anitya/static/node_modules/moment/locale/zh-tw.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/min/locales.js` & `anitya-1.8.0/anitya/static/node_modules/moment/min/locales.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/min/locales.min.js` & `anitya-1.8.0/anitya/static/node_modules/moment/min/locales.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/min/locales.min.js.map` & `anitya-1.8.0/anitya/static/node_modules/moment/min/locales.min.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/min/moment-with-locales.js` & `anitya-1.8.0/anitya/static/node_modules/moment/min/moment-with-locales.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/min/moment-with-locales.min.js` & `anitya-1.8.0/anitya/static/node_modules/moment/min/moment-with-locales.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/min/moment-with-locales.min.js.map` & `anitya-1.8.0/anitya/static/node_modules/moment/min/moment-with-locales.min.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/min/moment.min.js` & `anitya-1.8.0/anitya/static/node_modules/moment/min/moment.min.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/min/moment.min.js.map` & `anitya-1.8.0/anitya/static/node_modules/moment/min/moment.min.js.map`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/moment.d.ts` & `anitya-1.8.0/anitya/static/node_modules/moment/moment.d.ts`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/moment.js` & `anitya-1.8.0/anitya/static/node_modules/moment/moment.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/package.json` & `anitya-1.8.0/anitya/static/node_modules/moment/package.json`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/check-overflow.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/check-overflow.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/date-from-array.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/date-from-array.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/from-anything.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/from-anything.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/from-array.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/from-array.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/from-object.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/from-object.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/from-string-and-array.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/from-string-and-array.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/from-string-and-format.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/from-string-and-format.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/from-string.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/from-string.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/parsing-flags.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/parsing-flags.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/create/valid.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/create/valid.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/add-subtract.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/add-subtract.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/as.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/as.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/bubble.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/bubble.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/constructor.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/constructor.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/create.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/create.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/get.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/get.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/humanize.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/humanize.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/iso-string.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/iso-string.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/prototype.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/prototype.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/duration/valid.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/duration/valid.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/format/format.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/format/format.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/base-config.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/base-config.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/en.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/en.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/formats.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/formats.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/lists.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/lists.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/locale.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/locale.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/locales.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/locales.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/prototype.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/prototype.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/relative.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/relative.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/locale/set.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/locale/set.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/add-subtract.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/add-subtract.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/calendar.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/calendar.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/compare.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/compare.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/constructor.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/constructor.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/diff.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/diff.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/format.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/format.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/from.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/from.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/get-set.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/get-set.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/locale.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/locale.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/min-max.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/min-max.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/moment.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/moment.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/prototype.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/prototype.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/start-end-of.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/start-end-of.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/to-type.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/to-type.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/moment/to.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/moment/to.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/parse/regex.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/parse/regex.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/parse/token.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/parse/token.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/aliases.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/aliases.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/day-of-month.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/day-of-month.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/day-of-week.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/day-of-week.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/day-of-year.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/day-of-year.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/era.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/era.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/hour.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/hour.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/millisecond.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/millisecond.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/minute.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/minute.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/month.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/month.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/offset.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/offset.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/quarter.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/quarter.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/second.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/second.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/timestamp.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/timestamp.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/week-calendar-utils.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/week-calendar-utils.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/week-year.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/week-year.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/week.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/week.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/units/year.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/units/year.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/compare-arrays.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/compare-arrays.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/deprecate.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/deprecate.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/is-calendar-spec.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/is-calendar-spec.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/lib/utils/is-moment-input.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/lib/utils/is-moment-input.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/af.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/af.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar-dz.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar-dz.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar-kw.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar-kw.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar-ly.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar-ly.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar-ma.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar-ma.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar-sa.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar-sa.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar-tn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar-tn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ar.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ar.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/az.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/az.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/be.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/be.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/bg.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/bg.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/bm.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/bm.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/bn-bd.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/bn-bd.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/bn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/bn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/bo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/bo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/br.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/br.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/bs.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/bs.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ca.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ca.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/cs.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/cs.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/cv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/cv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/cy.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/cy.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/da.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/da.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/de-at.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/de-at.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/de-ch.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/de-ch.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/de.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/de.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/dv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/dv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/el.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/el.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-au.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-au.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-ca.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-ca.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-gb.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-gb.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-ie.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-ie.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-il.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-il.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-in.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-in.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-nz.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-nz.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/en-sg.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/en-sg.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/eo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/eo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/es-do.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/es-do.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/es-mx.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/es-mx.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/es-us.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/es-us.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/es.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/es.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/et.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/et.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/eu.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/eu.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fa.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fa.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fi.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fil.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fil.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fr-ca.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fr-ca.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fr-ch.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fr-ch.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/fy.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/fy.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ga.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ga.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/gd.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/gd.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/gl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/gl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/gom-deva.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/gom-deva.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/gom-latn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/gom-latn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/gu.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/gu.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/he.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/he.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/hi.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/hi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/hr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/hr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/hu.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/hu.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/hy-am.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/hy-am.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/id.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/id.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/is.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/is.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/it-ch.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/it-ch.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/it.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/it.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ja.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ja.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/jv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/jv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ka.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ka.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/kk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/kk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/km.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/km.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/kn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/kn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ko.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ko.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ku.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ku.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ky.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ky.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/lb.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/lb.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/lo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/lo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/lt.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/lt.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/lv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/lv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/me.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/me.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/mi.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/mi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/mk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/mk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ml.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ml.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/mn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/mn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/mr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/mr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ms-my.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ms-my.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ms.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ms.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/mt.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/mt.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/my.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/my.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/nb.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/nb.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ne.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ne.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/nl-be.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/nl-be.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/nl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/nl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/nn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/nn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/oc-lnc.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/oc-lnc.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/pa-in.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/pa-in.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/pl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/pl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/pt-br.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/pt-br.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/pt.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/pt.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ro.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ro.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ru.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ru.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sd.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sd.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/se.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/se.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/si.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/si.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sq.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sq.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sr-cyrl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sr-cyrl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ss.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ss.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sv.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sv.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/sw.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/sw.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ta.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ta.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/te.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/te.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tet.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tet.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tg.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tg.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/th.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/th.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tl-ph.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tl-ph.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tlh.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tlh.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tr.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tr.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tzl.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tzl.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tzm-latn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tzm-latn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/tzm.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/tzm.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ug-cn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ug-cn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/uk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/uk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/ur.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/ur.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/uz-latn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/uz-latn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/uz.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/uz.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/vi.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/vi.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/x-pseudo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/x-pseudo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/yo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/yo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/zh-cn.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/zh-cn.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/zh-hk.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/zh-hk.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/zh-mo.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/zh-mo.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/locale/zh-tw.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/locale/zh-tw.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/src/moment.js` & `anitya-1.8.0/anitya/static/node_modules/moment/src/moment.js`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/node_modules/moment/ts3.1-typings/moment.d.ts` & `anitya-1.8.0/anitya/static/node_modules/moment/ts3.1-typings/moment.d.ts`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/package-lock.json` & `anitya-1.8.0/anitya/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/package.json` & `anitya-1.8.0/anitya/static/package.json`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/static/yahoo_logo.png` & `anitya-1.8.0/anitya/static/yahoo_logo.png`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/distro_add_edit.html` & `anitya-1.8.0/anitya/templates/distro_add_edit.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/distro_delete.html` & `anitya-1.8.0/anitya/templates/distro_delete.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/distros.html` & `anitya-1.8.0/anitya/templates/distros.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/flags.html` & `anitya-1.8.0/anitya/templates/flags.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/index.html` & `anitya-1.8.0/anitya/templates/index.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/login.html` & `anitya-1.8.0/anitya/templates/login.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/logs.html` & `anitya-1.8.0/anitya/templates/logs.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/mapping.html` & `anitya-1.8.0/anitya/templates/mapping.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/master.html` & `anitya-1.8.0/anitya/templates/master.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/project.html` & `anitya-1.8.0/anitya/templates/project.html`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     <p>This project is archived. It can't be edited and it's not checked for new versions. To unarchive project, please create a request using flag mechanism.</p>
   {% else %}
     <h1>Project: {{ project.name }}</h1>
   {% endif %}
 </div>
 
 <div class="row justify-content-center" resource="{{ project.homepage }}" typeof="doap:Project">
-  <div class="col-md-5 col-md-offset-1">
+  <div class="col col-md">
 
     <div class="d-grid gap-3">
       <div class="list-group">
         <div class="list-group-item list-group-item-secondary">
           <div class="row">
             <div class="col-8">
               <h3 property="doap:name">{{ project.name }}</h3>
@@ -234,15 +234,15 @@
           </div><!-- end group-item-text -->
         </div><!-- end group-item -->
         {% endif %}
       </div><!-- end-group -->
     </div><!-- end column -->
   </div><!-- end d-grid -->
 
-  <div class="col-md-5">
+  <div class="col col-md">
     <div class="d-grid gap-3">
       <div class="list-group">
         <div class="list-group-item list-group-item-secondary">
           <h3>Status</h3>
         </div>
         <span class="list-group-item">
           <table class="table table-condensed">
```

### Comparing `anitya-1.7.0/anitya/templates/project_archive.html` & `anitya-1.8.0/anitya/templates/project_archive.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/project_delete.html` & `anitya-1.8.0/anitya/templates/project_delete.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/project_flag.html` & `anitya-1.8.0/anitya/templates/project_flag.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/project_new.html` & `anitya-1.8.0/anitya/templates/project_new.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/project_versions_delete.html` & `anitya-1.8.0/anitya/templates/project_versions_delete.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/projects.html` & `anitya-1.8.0/anitya/templates/projects.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/regex_delete.html` & `anitya-1.8.0/anitya/templates/regex_delete.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/search.html` & `anitya-1.8.0/anitya/templates/search.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/settings.html` & `anitya-1.8.0/anitya/templates/settings.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/updates.html` & `anitya-1.8.0/anitya/templates/updates.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/users.html` & `anitya-1.8.0/anitya/templates/users.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/templates/version_delete.html` & `anitya-1.8.0/anitya/templates/version_delete.html`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/anitya/ui.py` & `anitya-1.8.0/anitya/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,19 @@
     new_path = flask.url_for("anitya_ui.static", filename="docs/index.html")
     return flask.redirect(new_path)
 
 
 @ui_blueprint.route("/login/", methods=("GET", "POST"))
 @ui_blueprint.route("/login", methods=("GET", "POST"))
 def login():
-    flask.session["next_url"] = flask.request.args.get("next", "/")
+    next_url = flask.request.args.get("next", "/")
+    if not next_url.startswith("/"):
+        next_url = "/"
+
+    flask.session["next_url"] = next_url
     return flask.render_template("login.html")
 
 
 @ui_blueprint.route("/logout/")
 @ui_blueprint.route("/logout")
 @login_required
 def logout():
@@ -99,15 +103,14 @@
     else:
         flask.abort(400)
 
 
 @ui_blueprint.route("/project/<int:project_id>")
 @ui_blueprint.route("/project/<int:project_id>/")
 def project(project_id):
-
     project = models.Project.by_id(Session, project_id)
 
     if not project:
         flask.abort(404)
 
     return flask.render_template(
         "project.html",
@@ -116,15 +119,14 @@
         links=anitya_config.get("DISTRO_MAPPING_LINKS", {}),
     )
 
 
 @ui_blueprint.route("/project/<project_name>")
 @ui_blueprint.route("/project/<project_name>/")
 def project_name(project_name):
-
     page = flask.request.args.get("page", 1)
 
     try:
         page = int(page)
     except ValueError:
         page = 1
 
@@ -146,15 +148,14 @@
         page=page,
     )
 
 
 @ui_blueprint.route("/projects")
 @ui_blueprint.route("/projects/")
 def projects():
-
     page = flask.request.args.get("page", 1)
 
     try:
         page = int(page)
     except ValueError:
         page = 1
 
@@ -173,15 +174,14 @@
     )
 
 
 @ui_blueprint.route("/projects/updates")
 @ui_blueprint.route("/projects/updates/")
 @ui_blueprint.route("/projects/updates/<status>")
 def projects_updated(status="updated"):
-
     page = flask.request.args.get("page", 1)
     name = flask.request.args.get("name", None)
     log = flask.request.args.get("log", None)
 
     try:
         page = int(page)
     except ValueError:
@@ -221,15 +221,14 @@
         log=log,
     )
 
 
 @ui_blueprint.route("/logs")
 @login_required
 def browse_logs():
-
     refresh = flask.request.args.get("refresh", False)
     page = flask.request.args.get("page", 1)
 
     try:
         page = int(page)
     except ValueError:
         page = 1
@@ -256,15 +255,14 @@
         page=page,
     )
 
 
 @ui_blueprint.route("/distros")
 @ui_blueprint.route("/distros/")
 def distros():
-
     page = flask.request.args.get("page", 1)
 
     try:
         page = int(page)
     except ValueError:
         page = 1
 
@@ -282,15 +280,14 @@
         page=page,
     )
 
 
 @ui_blueprint.route("/distro/<distroname>")
 @ui_blueprint.route("/distro/<distroname>/")
 def distro(distroname):
-
     page = flask.request.args.get("page", 1)
 
     try:
         page = int(page)
     except ValueError:
         page = 1
 
@@ -309,15 +306,14 @@
         page=page,
     )
 
 
 @ui_blueprint.route("/distro/add", methods=["GET", "POST"])
 @login_required
 def add_distro():
-
     form = anitya.forms.DistroForm()
 
     if form.validate_on_submit():
         name = form.name.data
 
         distro = models.Distro(name)
 
@@ -341,15 +337,14 @@
     )
 
 
 @ui_blueprint.route("/projects/search")
 @ui_blueprint.route("/projects/search/")
 @ui_blueprint.route("/projects/search/<pattern>")
 def projects_search(pattern=None):
-
     pattern = flask.request.args.get("pattern", pattern) or "*"
     page = flask.request.args.get("page", 1)
     exact = flask.request.args.get("exact", 0)
 
     try:
         page = int(page)
     except ValueError:
@@ -389,15 +384,14 @@
     )
 
 
 @ui_blueprint.route("/distro/<distroname>/search")
 @ui_blueprint.route("/distro/<distroname>/search/")
 @ui_blueprint.route("/distro/<distroname>/search/<pattern>")
 def distro_projects_search(distroname, pattern=None):
-
     pattern = flask.request.args.get("pattern", pattern) or "*"
     page = flask.request.args.get("page", 1)
     exact = flask.request.args.get("exact", 0)
 
     try:
         page = int(page)
     except ValueError:
@@ -554,15 +548,14 @@
         400,
     )
 
 
 @ui_blueprint.route("/project/<project_id>/edit", methods=["GET", "POST"])
 @login_required
 def edit_project(project_id):
-
     project = models.Project.get(Session, project_id)
     if not project:
         flask.abort(404)
 
     # Archived project is not editable
     if project.archived:
         flask.abort(404)
@@ -627,15 +620,14 @@
         plugins=backend_plugins,
     )
 
 
 @ui_blueprint.route("/project/<project_id>/flag", methods=["GET", "POST"])
 @login_required
 def flag_project(project_id):
-
     project = models.Project.get(Session, project_id)
     if not project:
         flask.abort(404)
 
     form = anitya.forms.FlagProjectForm(obj=project)
 
     if form.validate_on_submit():
@@ -661,15 +653,14 @@
         project=project,
     )
 
 
 @ui_blueprint.route("/project/<project_id>/map", methods=["GET", "POST"])
 @login_required
 def map_project(project_id):
-
     project = models.Project.get(Session, project_id)
     if not project:
         flask.abort(404)
 
     # Get all available distros name
     distros = models.Distro.all(Session)
     distro_names = []
@@ -705,15 +696,14 @@
         "mapping.html", current="projects", project=project, form=form
     )
 
 
 @ui_blueprint.route("/project/<project_id>/map/<pkg_id>", methods=["GET", "POST"])
 @login_required
 def edit_project_mapping(project_id, pkg_id):
-
     project = models.Project.get(Session, project_id)
     if not project:
         flask.abort(404)
 
     package = models.Packages.by_id(Session, pkg_id)
     if not package:
         flask.abort(404)
@@ -727,15 +717,14 @@
     form = anitya.forms.MappingForm(
         package_name=package.package_name,
         distro=package.distro_name,
         distros=distro_names,
     )
 
     if form.validate_on_submit():
-
         try:
             utilities.map_project(
                 Session,
                 project=project,
                 package_name=form.package_name.data,
                 distribution=form.distro.data,
                 user_id=flask.g.user.username,
```

### Comparing `anitya-1.7.0/anitya/wsgi.py` & `anitya-1.8.0/anitya/wsgi.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/createdb.py` & `anitya-1.8.0/createdb.py`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/files/anitya.toml.sample` & `anitya-1.8.0/files/anitya.toml.sample`

 * *Files identical despite different names*

### Comparing `anitya-1.7.0/pyproject.toml` & `anitya-1.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     | dist
   )/
 )
 '''
 
 [tool.poetry]
 name = "anitya"
-version = "1.7.0"
+version = "1.8.0"
 description = "A cross-distribution upstream release monitoring project"
 authors = ["Pierre-Yves Chibon <pingou@pingoured.fr>"]
 maintainers = ["Michal Konecny <mkonecny@redhat.com>"]
 readme = "README.rst"
 homepage = "https://release-monitoring.org"
 documentation = "https://anitya.readthedocs.io"
 repository = "https://github.com/fedora-infra/anitya"
@@ -101,29 +101,29 @@
 Flask-Login = "^0.6.2"
 Flask-WTF = "^1.0.1"
 # https://github.com/sphinx-doc/sphinx/issues/10306
 Jinja2 = "<3.1.3"
 ordered-set = "^4.1.0"
 packaging = "^23.0"
 python-dateutil = "^2.8.2"
-semver = "^2.13.0"
+semver = "^3.0.0"
 social-auth-app-flask = "^1.0.0"
 social-auth-app-flask-sqlalchemy = "^1.0.1"
 SQLAlchemy = "^1.4.41"
 sseclient = "^0.0.27"
 # Limit the package till https://github.com/maxcountryman/flask-login/issues/686 is fixed
-Werkzeug = "2.1.2"
+Werkzeug = "2.3.0"
 "straight.plugin" = "^1.5.0"
 toml = "^0.10.2"
 webargs = "^8.2.0"
 WTForms = "^3.0.1"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.4"
-black = "^22.8.0"
+black = "^23.0.0"
 coverage = "^7.0.0"
 diff-cover = "^7.0.1"
 flake8 = "^6.0.0"
 mock = "^5.0.0"
 pytest = "^7.1.3"
 pytest-cov = "^4.0.0"
 vcrpy = "^4.2.1"
@@ -135,15 +135,15 @@
 
 # Required to test building the docs
 Sphinx = "^6.0.0"
 sphinxcontrib-httpdomain = "^1.8.0"
 sqlalchemy_schemadisplay = "^1.3"
 
 # Mypy test requirements
-mypy = "^0.991"
+mypy = "^1.0"
 types-mock = "^4.0.15"
 types-python-dateutil = "^2.8.19"
 types-requests = "^2.28.11"
 types-setuptools = "^65.3.0"
 types-six = "^1.16.19"
 types-toml = "^0.10.8"
```

### Comparing `anitya-1.7.0/setup.py` & `anitya-1.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,40 +224,40 @@
 install_requires = \
 ['Flask-Login>=0.6.2,<0.7.0',
  'Flask-WTF>=1.0.1,<2.0.0',
  'Flask>=2.1.2,<3.0.0',
  'Jinja2<3.1.3',
  'SQLAlchemy>=1.4.41,<2.0.0',
  'WTForms>=3.0.1,<4.0.0',
- 'Werkzeug==2.1.2',
+ 'Werkzeug==2.3.0',
  'alembic>=1.8.1,<2.0.0',
  'anitya-schema>=2.0.1,<3.0.0',
  'arrow>=1.2.3,<2.0.0',
  'beautifulsoup4>=4.11.1,<5.0.0',
  'defusedxml>=0.7.1,<0.8.0',
  'fedora-messaging>=3.1.0,<4.0.0',
  'ordered-set>=4.1.0,<5.0.0',
  'packaging>=23.0,<24.0',
  'python-dateutil>=2.8.2,<3.0.0',
- 'semver>=2.13.0,<3.0.0',
+ 'semver>=3.0.0,<4.0.0',
  'social-auth-app-flask-sqlalchemy>=1.0.1,<2.0.0',
  'social-auth-app-flask>=1.0.0,<2.0.0',
  'sseclient>=0.0.27,<0.0.28',
  'straight.plugin>=1.5.0,<2.0.0',
  'toml>=0.10.2,<0.11.0',
  'webargs>=8.2.0,<9.0.0']
 
 entry_points = \
 {'console_scripts': ['check_service = anitya.check_service:main',
                      'librariesio_consumer = anitya.librariesio_consumer:main',
                      'sar = anitya.sar:main']}
 
 setup_kwargs = {
     'name': 'anitya',
-    'version': '1.7.0',
+    'version': '1.8.0',
     'description': 'A cross-distribution upstream release monitoring project',
     'long_description': '\n.. image:: https://img.shields.io/pypi/v/anitya.svg\n  :target: https://pypi.org/project/anitya/\n\n.. image:: https://img.shields.io/pypi/pyversions/anitya.svg\n  :target: https://pypi.org/project/anitya/\n\n.. image:: https://readthedocs.org/projects/anitya/badge/?version=latest\n  :alt: Documentation Status\n  :target: https://anitya.readthedocs.io/en/latest/?badge=latest\n\n.. image:: https://img.shields.io/lgtm/alerts/g/fedora-infra/anitya.svg?logo=lgtm&logoWidth=18\n  :target: https://lgtm.com/projects/g/fedora-infra/anitya/alerts/\n\n.. image:: https://img.shields.io/lgtm/grade/javascript/g/fedora-infra/anitya.svg?logo=lgtm&logoWidth=18\n  :target: https://lgtm.com/projects/g/fedora-infra/anitya/context:javascript\n  \n.. image:: https://img.shields.io/lgtm/grade/python/g/fedora-infra/anitya.svg?logo=lgtm&logoWidth=18\n  :target: https://lgtm.com/projects/g/fedora-infra/anitya/context:python\n  \n\n======\nAnitya\n======\n\nAnitya is a release monitoring project. It provides a user-friendly interface\nto add, edit, or browse projects. A cron job can be configured to regularly\nscan for new releases of projects. When Anitya discovers a new release for a\nproject, it publishes a RabbitMQ messages via `fedora messaging`_.\nThis makes it easy to integrate with Anitya and perform actions when a new\nrelease is created for a project. For example, the Fedora project runs a service\ncalled `the-new-hotness <https://github.com/fedora-infra/the-new-hotness/>`_\nwhich files a Bugzilla bug against a package when the upstream project makes a\nnew release.\n\nFor more information, check out the `documentation`_!\n\n\nDevelopment\n===========\n\nFor details on how to contribute, check out the `contribution guide`_.\n\n\n.. _documentation: https://anitya.readthedocs.io/\n.. _contribution guide: https://anitya.readthedocs.io/en/latest/contributing.html\n.. _fedora messaging: https://fedora-messaging.readthedocs.io/en/latest\n',
     'author': 'Pierre-Yves Chibon',
     'author_email': 'pingou@pingoured.fr',
     'maintainer': 'Michal Konecny',
     'maintainer_email': 'mkonecny@redhat.com',
     'url': 'https://release-monitoring.org',
```

### Comparing `anitya-1.7.0/PKG-INFO` & `anitya-1.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 Metadata-Version: 2.1
 Name: anitya
-Version: 1.7.0
+Version: 1.8.0
 Summary: A cross-distribution upstream release monitoring project
 Home-page: https://release-monitoring.org
 License: GPL-2.0-or-later
 Author: Pierre-Yves Chibon
 Author-email: pingou@pingoured.fr
 Maintainer: Michal Konecny
 Maintainer-email: mkonecny@redhat.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask (>=2.1.2,<3.0.0)
 Requires-Dist: Flask-Login (>=0.6.2,<0.7.0)
 Requires-Dist: Flask-WTF (>=1.0.1,<2.0.0)
 Requires-Dist: Jinja2 (<3.1.3)
 Requires-Dist: SQLAlchemy (>=1.4.41,<2.0.0)
 Requires-Dist: WTForms (>=3.0.1,<4.0.0)
-Requires-Dist: Werkzeug (==2.1.2)
+Requires-Dist: Werkzeug (==2.3.0)
 Requires-Dist: alembic (>=1.8.1,<2.0.0)
 Requires-Dist: anitya-schema (>=2.0.1,<3.0.0)
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: fedora-messaging (>=3.1.0,<4.0.0)
 Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
 Requires-Dist: packaging (>=23.0,<24.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: semver (>=2.13.0,<3.0.0)
+Requires-Dist: semver (>=3.0.0,<4.0.0)
 Requires-Dist: social-auth-app-flask (>=1.0.0,<2.0.0)
 Requires-Dist: social-auth-app-flask-sqlalchemy (>=1.0.1,<2.0.0)
 Requires-Dist: sseclient (>=0.0.27,<0.0.28)
 Requires-Dist: straight.plugin (>=1.5.0,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: webargs (>=8.2.0,<9.0.0)
 Project-URL: Documentation, https://anitya.readthedocs.io
```

