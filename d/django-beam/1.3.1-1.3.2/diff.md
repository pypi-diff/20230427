# Comparing `tmp/django-beam-1.3.1.tar.gz` & `tmp/django-beam-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-beam-1.3.1.tar", last modified: Fri Mar 31 10:14:16 2023, max compression
+gzip compressed data, was "django-beam-1.3.2.tar", last modified: Thu Apr 27 06:09:03 2023, max compression
```

## Comparing `django-beam-1.3.1.tar` & `django-beam-1.3.2.tar`

### file list

```diff
@@ -1,108 +1,122 @@
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.305881 django-beam-1.3.1/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1511 2022-04-27 09:12:32.000000 django-beam-1.3.1/LICENSE
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      284 2023-01-09 10:44:11.000000 django-beam-1.3.1/MANIFEST.in
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-03-31 10:14:16.305959 django-beam-1.3.1/PKG-INFO
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2954 2023-03-28 08:37:32.000000 django-beam-1.3.1/README.md
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      740 2023-03-31 10:14:16.306249 django-beam-1.3.1/setup.cfg
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)       53 2022-04-27 09:12:32.000000 django-beam-1.3.1/setup.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.292045 django-beam-1.3.1/src/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.295236 django-beam-1.3.1/src/beam/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      105 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4680 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/actions.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7485 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/components.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.295397 django-beam-1.3.1/src/beam/contrib/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.296305 django-beam-1.3.1/src/beam/contrib/auth/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      196 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/apps.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      903 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/forms.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.290639 django-beam-1.3.1/src/beam/contrib/auth/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.297974 django-beam-1.3.1/src/beam/contrib/auth/templates/registration/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      296 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/templates/registration/logged_out.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1136 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/templates/registration/login.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/templates/registration/password_change_done.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      837 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/templates/registration/password_change_form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      364 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/templates/registration/password_reset_complete.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      980 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/templates/registration/password_reset_confirm.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      535 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/templates/registration/password_reset_done.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      616 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/templates/registration/password_reset_email.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      531 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/templates/registration/password_reset_form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      230 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3881 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/auth/views.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.298153 django-beam-1.3.1/src/beam/contrib/autocomplete_light/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2940 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/autocomplete_light/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.290847 django-beam-1.3.1/src/beam/contrib/autocomplete_light/static/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.298331 django-beam-1.3.1/src/beam/contrib/autocomplete_light/static/autocomplete_light/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1011 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.299016 django-beam-1.3.1/src/beam/contrib/reversion/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/reversion/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      150 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/reversion/apps.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.291068 django-beam-1.3.1/src/beam/contrib/reversion/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.299435 django-beam-1.3.1/src/beam/contrib/reversion/templates/beam_reversion/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1140 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1879 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/contrib/reversion/templates/beam_reversion/version_list.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4032 2023-03-31 10:10:44.000000 django-beam-1.3.1/src/beam/contrib/reversion/views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7137 2023-03-30 13:36:34.000000 django-beam-1.3.1/src/beam/contrib/reversion/viewsets.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    11062 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/inlines.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1235 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/layouts.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.291200 django-beam-1.3.1/src/beam/locale/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.291257 django-beam-1.3.1/src/beam/locale/de/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.299594 django-beam-1.3.1/src/beam/locale/de/LC_MESSAGES/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5525 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2814 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/registry.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.299846 django-beam-1.3.1/src/beam/templatetags/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/templatetags/__init__.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8414 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/templatetags/beam_tags.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.299993 django-beam-1.3.1/src/beam/themes/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.300183 django-beam-1.3.1/src/beam/themes/bootstrap4/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/__init__.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.291617 django-beam-1.3.1/src/beam/themes/bootstrap4/static/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.291769 django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.300326 django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/css/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    12660 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.301245 django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/js/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3291 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/js/actions.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1177 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/js/add_related.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    94341 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6007 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/js/inlines.js
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    24467 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.291890 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.302847 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3352 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/base.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/create.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1668 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/dashboard.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2444 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/delete.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2894 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/detail.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4361 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/form.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8134 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/list.html
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.305177 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1756 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/actions.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1954 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4380 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3284 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1289 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/filters.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      553 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6084 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2836 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2643 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4519 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2072 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/layout.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      666 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/links.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      635 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      776 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/messages.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4788 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4968 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1489 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/update.html
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      946 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/themes/bootstrap4/widgets.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      127 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/types.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)      983 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/urls.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1584 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/utils.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)    21601 2023-03-31 09:36:48.000000 django-beam-1.3.1/src/beam/views.py
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7528 2023-03-30 10:38:46.000000 django-beam-1.3.1/src/beam/viewsets.py
-drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-03-31 10:14:16.305769 django-beam-1.3.1/src/django_beam.egg-info/
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-03-31 10:14:16.000000 django-beam-1.3.1/src/django_beam.egg-info/PKG-INFO
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3768 2023-03-31 10:14:16.000000 django-beam-1.3.1/src/django_beam.egg-info/SOURCES.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        1 2023-03-31 10:14:16.000000 django-beam-1.3.1/src/django_beam.egg-info/dependency_links.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)       88 2023-03-31 10:14:16.000000 django-beam-1.3.1/src/django_beam.egg-info/requires.txt
--rw-r--r--   0 raphaelkimmig   (502) staff       (20)        5 2023-03-31 10:14:16.000000 django-beam-1.3.1/src/django_beam.egg-info/top_level.txt
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.048680 django-beam-1.3.2/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1511 2022-04-27 09:12:32.000000 django-beam-1.3.2/LICENSE
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      284 2023-01-09 10:44:11.000000 django-beam-1.3.2/MANIFEST.in
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-04-27 06:09:03.048769 django-beam-1.3.2/PKG-INFO
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2954 2023-03-28 08:37:32.000000 django-beam-1.3.2/README.md
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      740 2023-04-27 06:09:03.049088 django-beam-1.3.2/setup.cfg
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)       53 2022-04-27 09:12:32.000000 django-beam-1.3.2/setup.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.031710 django-beam-1.3.2/src/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.034695 django-beam-1.3.2/src/beam/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      105 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4680 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/actions.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7485 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/components.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.034841 django-beam-1.3.2/src/beam/contrib/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.035669 django-beam-1.3.2/src/beam/contrib/auth/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      196 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/apps.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      903 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/forms.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.030465 django-beam-1.3.2/src/beam/contrib/auth/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.037078 django-beam-1.3.2/src/beam/contrib/auth/templates/registration/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      296 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/templates/registration/logged_out.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1136 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/templates/registration/login.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/templates/registration/password_change_done.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      837 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/templates/registration/password_change_form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      364 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/templates/registration/password_reset_complete.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      980 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      535 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/templates/registration/password_reset_done.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      616 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/templates/registration/password_reset_email.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      531 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/templates/registration/password_reset_form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      230 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3881 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/auth/views.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.037238 django-beam-1.3.2/src/beam/contrib/autocomplete_light/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2940 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/autocomplete_light/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.030653 django-beam-1.3.2/src/beam/contrib/autocomplete_light/static/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.037393 django-beam-1.3.2/src/beam/contrib/autocomplete_light/static/autocomplete_light/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1011 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.037993 django-beam-1.3.2/src/beam/contrib/reversion/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/reversion/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      150 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/reversion/apps.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.030837 django-beam-1.3.2/src/beam/contrib/reversion/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.038284 django-beam-1.3.2/src/beam/contrib/reversion/templates/beam_reversion/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1140 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1879 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/reversion/templates/beam_reversion/version_list.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4032 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/reversion/views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7137 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/contrib/reversion/viewsets.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    11062 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/inlines.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1235 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/layouts.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.030953 django-beam-1.3.2/src/beam/locale/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.031000 django-beam-1.3.2/src/beam/locale/de/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.038449 django-beam-1.3.2/src/beam/locale/de/LC_MESSAGES/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     5525 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2814 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/registry.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.038700 django-beam-1.3.2/src/beam/templatetags/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/templatetags/__init__.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8414 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/templatetags/beam_tags.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.038953 django-beam-1.3.2/src/beam/themes/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.039150 django-beam-1.3.2/src/beam/themes/bootstrap4/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/__init__.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.031327 django-beam-1.3.2/src/beam/themes/bootstrap4/static/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.031443 django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.039427 django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/css/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    12660 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.040834 django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/js/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3291 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/js/actions.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1177 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/js/add_related.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    94341 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6007 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/js/inlines.js
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    24467 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.031564 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.042140 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3352 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/base.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      261 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/create.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1668 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/dashboard.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2444 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/delete.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2894 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/detail.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4361 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/form.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     8134 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/list.html
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.044865 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1756 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/actions.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1954 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4380 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3284 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1289 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/filters.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      553 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     6084 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3061 2023-04-27 06:08:23.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2865 2023-04-27 06:08:23.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4586 2023-04-27 06:08:23.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2072 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/layout.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      666 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/links.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      635 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      776 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/messages.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4788 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4968 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1489 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/update.html
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      946 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/themes/bootstrap4/widgets.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      127 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/types.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      983 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1584 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/utils.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    21601 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     7528 2023-04-03 10:36:16.000000 django-beam-1.3.2/src/beam/viewsets.py
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.045528 django-beam-1.3.2/src/django_beam.egg-info/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3403 2023-04-27 06:09:03.000000 django-beam-1.3.2/src/django_beam.egg-info/PKG-INFO
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4077 2023-04-27 06:09:03.000000 django-beam-1.3.2/src/django_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        1 2023-04-27 06:09:03.000000 django-beam-1.3.2/src/django_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)       88 2023-04-27 06:09:03.000000 django-beam-1.3.2/src/django_beam.egg-info/requires.txt
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        5 2023-04-27 06:09:03.000000 django-beam-1.3.2/src/django_beam.egg-info/top_level.txt
+drwxr-xr-x   0 raphaelkimmig   (502) staff       (20)        0 2023-04-27 06:09:03.048406 django-beam-1.3.2/tests/
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    15449 2022-04-27 09:12:32.000000 django-beam-1.3.2/tests/test_actions.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2782 2023-01-11 09:59:58.000000 django-beam-1.3.2/tests/test_components.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    14309 2023-01-23 10:38:56.000000 django-beam-1.3.2/tests/test_contrib_auth.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2040 2022-04-27 09:12:32.000000 django-beam-1.3.2/tests/test_contrib_autocomplete.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    10694 2023-04-27 06:08:23.000000 django-beam-1.3.2/tests/test_contrib_reversion.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)      850 2022-04-27 09:12:32.000000 django-beam-1.3.2/tests/test_inlines.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)        0 2022-04-27 09:12:32.000000 django-beam-1.3.2/tests/test_layouts.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     1849 2022-04-27 09:12:32.000000 django-beam-1.3.2/tests/test_registry.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     2352 2023-01-11 09:59:58.000000 django-beam-1.3.2/tests/test_tags.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4771 2023-01-11 09:59:58.000000 django-beam-1.3.2/tests/test_urls.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     3946 2023-01-11 09:59:58.000000 django-beam-1.3.2/tests/test_utils.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)    31258 2023-03-30 10:35:40.000000 django-beam-1.3.2/tests/test_views.py
+-rw-r--r--   0 raphaelkimmig   (502) staff       (20)     4275 2022-04-27 09:12:32.000000 django-beam-1.3.2/tests/test_viewsets.py
```

### Comparing `django-beam-1.3.1/LICENSE` & `django-beam-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/PKG-INFO` & `django-beam-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-beam
-Version: 1.3.1
+Version: 1.3.2
 Summary: A crud library for python
 Home-page: https://github.com/django-beam/django-beam
-Download-URL: https://github.com/django-beam/django-beam/archive/1.3.1.tar.gz
+Download-URL: https://github.com/django-beam/django-beam/archive/1.3.2.tar.gz
 Author: Raphael Kimmig
 Author-email: raphael@ampad.de
 License: BSD 3-Clause License
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `django-beam-1.3.1/README.md` & `django-beam-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/setup.cfg` & `django-beam-1.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [metadata]
 name = django-beam
-version = 1.3.1
+version = 1.3.2
 description = A crud library for python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/django-beam/django-beam
-download_url = https://github.com/django-beam/django-beam/archive/1.3.1.tar.gz
+download_url = https://github.com/django-beam/django-beam/archive/1.3.2.tar.gz
 author = Raphael Kimmig
 author_email = raphael@ampad.de
 keywords = 
 license = BSD 3-Clause License
 classifiers = 
 	Framework :: Django
 	Programming Language :: Python :: 3
```

### Comparing `django-beam-1.3.1/src/beam/actions.py` & `django-beam-1.3.2/src/beam/actions.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/components.py` & `django-beam-1.3.2/src/beam/components.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/auth/forms.py` & `django-beam-1.3.2/src/beam/contrib/auth/forms.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/auth/templates/registration/login.html` & `django-beam-1.3.2/src/beam/contrib/auth/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/auth/templates/registration/password_change_form.html` & `django-beam-1.3.2/src/beam/contrib/auth/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/auth/templates/registration/password_reset_confirm.html` & `django-beam-1.3.2/src/beam/contrib/auth/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/auth/templates/registration/password_reset_done.html` & `django-beam-1.3.2/src/beam/contrib/auth/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/auth/templates/registration/password_reset_email.html` & `django-beam-1.3.2/src/beam/contrib/auth/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/auth/templates/registration/password_reset_form.html` & `django-beam-1.3.2/src/beam/contrib/auth/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/auth/views.py` & `django-beam-1.3.2/src/beam/contrib/auth/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/autocomplete_light/__init__.py` & `django-beam-1.3.2/src/beam/contrib/autocomplete_light/__init__.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css` & `django-beam-1.3.2/src/beam/contrib/autocomplete_light/static/autocomplete_light/select2.css`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html` & `django-beam-1.3.2/src/beam/contrib/reversion/templates/beam_reversion/version_detail.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/reversion/templates/beam_reversion/version_list.html` & `django-beam-1.3.2/src/beam/contrib/reversion/templates/beam_reversion/version_list.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/reversion/views.py` & `django-beam-1.3.2/src/beam/contrib/reversion/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/contrib/reversion/viewsets.py` & `django-beam-1.3.2/src/beam/contrib/reversion/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/inlines.py` & `django-beam-1.3.2/src/beam/inlines.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/layouts.py` & `django-beam-1.3.2/src/beam/layouts.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/locale/de/LC_MESSAGES/django.mo` & `django-beam-1.3.2/src/beam/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/registry.py` & `django-beam-1.3.2/src/beam/registry.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/templatetags/beam_tags.py` & `django-beam-1.3.2/src/beam/templatetags/beam_tags.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css` & `django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/css/bootstrap-select.min.css`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/js/actions.js` & `django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/js/actions.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/js/add_related.js` & `django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/js/add_related.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js` & `django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/js/bootstrap-select.min.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/js/inlines.js` & `django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/js/inlines.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js` & `django-beam-1.3.2/src/beam/themes/bootstrap4/static/beam/js/sortable.min.js`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/base.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/base.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/dashboard.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/delete.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/delete.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/detail.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/detail.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/form.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/form.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/list.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/list.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/actions.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/actions.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_field.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/detail_inline_tabular.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/filters.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/filters.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/form_field.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular.html`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,25 @@
 
             {% block inline_group_head %}
             <thead>
                 <tr>
                     {% if inline.can_order %}<th scope="col"></th>{% endif %}
 
                     {% for field in inline.fields %}
+                        {% if inline.can_order and inline.order_field == field %}
+                            {# skip order field #}
+                        {% else %}
                         {% block label_container %}
-                        <th scope="col">
-                            {% block label %}
-                                {{ inline.model|field_verbose_name:field|capfirst }}
-                            {% endblock %}
-                        </th>
+                            <th scope="col">
+                                {% block label %}
+                                    {{ inline.model|field_verbose_name:field|capfirst }}
+                                {% endblock %}
+                            </th>
                         {% endblock %}
+                        {% endif %}
                     {% endfor %}
 
                     {% if inline.formset.can_delete %}<th scope="col"></th>{% endif %}
                 </tr>
             </thead>
             {% endblock %}
 
@@ -69,8 +73,8 @@
                 {% include "beam/partials/form_inline_tabular_row.html" with form=inline.formset.empty_form fields=inline.fields inline_item_id="__prefix__" empty_form=True %}
             </tbody>
             {% endblock %}
 
         {% endblock %}
     </table>
     </div>
-{% endblock %}
+{% endblock %}
```

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/form_inline_tabular_row.html`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,21 @@
                 {% endblock %}
             </td>
         {% endif %}
         {% endblock %}
 
         {% block inline_layout %}
         {% for field in form.fields %}
+            {# FIXME field can't be html as we iterate over form.fields not inline.fields or inline.layout #}
             {% if field.is_html %}
                 <td class="beam-field-{{ field }}">
                     {{ field.content|safe }}
                 </td>
+            {% elif inline.can_order and inline.order_field == field %}
+                {# skip order field #}
             {% else %}
                 {% get_form_field form field as form_field %}
                 {% if form_field is None %}
                     <td class="beam-field-{{ field }}">
                         {% include "beam/partials/detail_field.html" with object=form.instance field=field %}
                     </td>
                 {% elif not form_field.is_hidden %}
@@ -62,8 +65,8 @@
             </td>
         {% endif %}
         {% endblock %}
 
     {% endblock %}
 
 </tr>
-{% endblock %}
+{% endblock %}
```

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/form_layout.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 {% load beam_tags %}
 {% load i18n %}
 
 
 {% if fields and not layout %}
+    {# FIXME: shouldn't this use fields instead of form.fields? #}
     {% fields_to_layout form.fields as layout %}
 {% elif not fields and not layout %}
     {% fields_to_layout form.fields as layout %}
 {% endif %}
 
 
 {% block layout %}
```

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/layout.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/layout.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/links.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/links.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/list_links.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/messages.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/messages.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/navigation.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/partials/pagination.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/templates/beam/update.html` & `django-beam-1.3.2/src/beam/themes/bootstrap4/templates/beam/update.html`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/themes/bootstrap4/widgets.py` & `django-beam-1.3.2/src/beam/themes/bootstrap4/widgets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/urls.py` & `django-beam-1.3.2/src/beam/urls.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/utils.py` & `django-beam-1.3.2/src/beam/utils.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/views.py` & `django-beam-1.3.2/src/beam/views.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/beam/viewsets.py` & `django-beam-1.3.2/src/beam/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-beam-1.3.1/src/django_beam.egg-info/PKG-INFO` & `django-beam-1.3.2/src/django_beam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-beam
-Version: 1.3.1
+Version: 1.3.2
 Summary: A crud library for python
 Home-page: https://github.com/django-beam/django-beam
-Download-URL: https://github.com/django-beam/django-beam/archive/1.3.1.tar.gz
+Download-URL: https://github.com/django-beam/django-beam/archive/1.3.2.tar.gz
 Author: Raphael Kimmig
 Author-email: raphael@ampad.de
 License: BSD 3-Clause License
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `django-beam-1.3.1/src/django_beam.egg-info/SOURCES.txt` & `django-beam-1.3.2/src/django_beam.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -73,8 +73,21 @@
 src/beam/themes/bootstrap4/templates/beam/partials/messages.html
 src/beam/themes/bootstrap4/templates/beam/partials/navigation.html
 src/beam/themes/bootstrap4/templates/beam/partials/pagination.html
 src/django_beam.egg-info/PKG-INFO
 src/django_beam.egg-info/SOURCES.txt
 src/django_beam.egg-info/dependency_links.txt
 src/django_beam.egg-info/requires.txt
-src/django_beam.egg-info/top_level.txt
+src/django_beam.egg-info/top_level.txt
+tests/test_actions.py
+tests/test_components.py
+tests/test_contrib_auth.py
+tests/test_contrib_autocomplete.py
+tests/test_contrib_reversion.py
+tests/test_inlines.py
+tests/test_layouts.py
+tests/test_registry.py
+tests/test_tags.py
+tests/test_urls.py
+tests/test_utils.py
+tests/test_views.py
+tests/test_viewsets.py
```

