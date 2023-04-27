# Comparing `tmp/badi_users-0.9.7.tar.gz` & `tmp/badi_users-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badi_users-0.9.7.tar", last modified: Mon Apr 24 14:21:06 2023, max compression
+gzip compressed data, was "badi_users-0.9.8.tar", last modified: Thu Apr 27 08:35:12 2023, max compression
```

## Comparing `badi_users-0.9.7.tar` & `badi_users-0.9.8.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.462211 badi_users-0.9.7/
--rw-rw-rw-   0        0        0     1093 2022-09-24 06:05:13.000000 badi_users-0.9.7/LICENSE
--rw-rw-rw-   0        0        0     1066 2022-11-10 17:03:20.000000 badi_users-0.9.7/MANIFEST.in
--rw-rw-rw-   0        0        0      419 2023-04-24 14:21:06.462211 badi_users-0.9.7/PKG-INFO
--rw-rw-rw-   0        0        0      143 2022-10-02 09:04:41.000000 badi_users-0.9.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.296179 badi_users-0.9.7/badi_ticket/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/__init__.py
--rw-rw-rw-   0        0        0      143 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/admin.py
--rw-rw-rw-   0        0        0     9803 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/api.py
--rw-rw-rw-   0        0        0      129 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.206451 badi_users-0.9.7/badi_ticket/locale/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.207418 badi_users-0.9.7/badi_ticket/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.298174 badi_users-0.9.7/badi_ticket/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2781 2023-04-16 12:25:05.000000 badi_users-0.9.7/badi_ticket/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.299173 badi_users-0.9.7/badi_ticket/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.7/badi_ticket/migrations/__init__.py
--rw-rw-rw-   0        0        0     3657 2023-04-16 09:10:44.000000 badi_users-0.9.7/badi_ticket/models.py
--rw-rw-rw-   0        0        0      313 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/routers.py
--rw-rw-rw-   0        0        0     2082 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.208415 badi_users-0.9.7/badi_ticket/static/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.208415 badi_users-0.9.7/badi_ticket/static/ticket/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.308178 badi_users-0.9.7/badi_ticket/static/ticket/js/
--rw-rw-rw-   0        0        0     2448 2023-04-16 09:16:22.000000 badi_users-0.9.7/badi_ticket/static/ticket/js/chat.js
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.309144 badi_users-0.9.7/badi_ticket/templates/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.373972 badi_users-0.9.7/badi_ticket/templates/ticket/
--rw-rw-rw-   0        0        0     6358 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/templates/ticket/admin_tickets.html
--rw-rw-rw-   0        0        0     5265 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/templates/ticket/message_list.html
--rw-rw-rw-   0        0        0     9642 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/templates/ticket/my_tickets.html
--rw-rw-rw-   0        0        0     7097 2023-04-16 08:20:08.000000 badi_users-0.9.7/badi_ticket/templates/ticket/ticket_create.html
--rw-rw-rw-   0        0        0     1639 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/templates/ticket/ticket_update.html
--rw-rw-rw-   0        0        0       63 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/tests.py
--rw-rw-rw-   0        0        0      583 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/urls.py
--rw-rw-rw-   0        0        0     2057 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_ticket/views.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.400899 badi_users-0.9.7/badi_user/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/__init__.py
--rw-rw-rw-   0        0        0      166 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.426832 badi_users-0.9.7/badi_user/api/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/api/__init__.py
--rw-rw-rw-   0        0        0    29463 2023-04-24 07:10:08.000000 badi_users-0.9.7/badi_user/api/api.py
--rw-rw-rw-   0        0        0      485 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/api/routers.py
--rw-rw-rw-   0        0        0     6013 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/api/serializers.py
--rw-rw-rw-   0        0        0      183 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/apps.py
--rw-rw-rw-   0        0        0     3428 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/filter.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.211406 badi_users-0.9.7/badi_user/locale/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.212403 badi_users-0.9.7/badi_user/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.428826 badi_users-0.9.7/badi_user/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     4486 2023-04-16 12:25:06.000000 badi_users-0.9.7/badi_user/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.430820 badi_users-0.9.7/badi_user/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.7/badi_user/migrations/__init__.py
--rw-rw-rw-   0        0        0     6975 2023-04-24 14:19:52.000000 badi_users-0.9.7/badi_user/models.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.437832 badi_users-0.9.7/badi_user/templates/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/templates/__init__.py
--rw-rw-rw-   0        0        0       27 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/templates/badi-user-test.html
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.478693 badi_users-0.9.7/badi_user/templates/group/
--rw-rw-rw-   0        0        0     8558 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/templates/group/group_create.html
--rw-rw-rw-   0        0        0     5472 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/templates/group/group_update.html
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.493652 badi_users-0.9.7/badi_user/templates/log/
--rw-rw-rw-   0        0        0     3987 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/templates/log/log_list.html
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.509611 badi_users-0.9.7/badi_user/templates/login-theme/
--rw-rw-rw-   0        0        0     7336 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/templates/login-theme/login-1.html
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.585410 badi_users-0.9.7/badi_user/templates/member/
--rw-rw-rw-   0        0        0     6863 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/templates/member/member_create.html
--rw-rw-rw-   0        0        0    22635 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/templates/member/member_list.html
--rw-rw-rw-   0        0        0     4783 2023-03-28 07:29:01.000000 badi_users-0.9.7/badi_user/templates/member/member_self_update.html
--rw-rw-rw-   0        0        0     6525 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/templates/member/member_update.html
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.652577 badi_users-0.9.7/badi_user/templates/user/
--rw-rw-rw-   0        0        0     5056 2023-04-16 12:18:39.000000 badi_users-0.9.7/badi_user/templates/user/change_password.html
--rw-rw-rw-   0        0        0     6743 2023-04-24 04:38:27.000000 badi_users-0.9.7/badi_user/templates/user/user_create.html
--rw-rw-rw-   0        0        0     4019 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/templates/user/user_list.html
--rw-rw-rw-   0        0        0     5005 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/templates/user/user_update.html
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.662552 badi_users-0.9.7/badi_user/templatetags/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/templatetags/__init__.py
--rw-rw-rw-   0        0        0     5950 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/templatetags/appfilter.py
--rw-rw-rw-   0        0        0      500 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.723389 badi_users-0.9.7/badi_user/ui/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/ui/__init__.py
--rw-rw-rw-   0        0        0     1484 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/ui/forms.py
--rw-rw-rw-   0        0        0      320 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/ui/log_views.py
--rw-rw-rw-   0        0        0     1706 2023-03-28 08:00:41.000000 badi_users-0.9.7/badi_user/ui/member_views.py
--rw-rw-rw-   0        0        0      672 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/ui/notification_views.py
--rw-rw-rw-   0        0        0      644 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/ui/roles_views.py
--rw-rw-rw-   0        0        0     1624 2023-04-16 08:12:22.000000 badi_users-0.9.7/badi_user/ui/urls.py
--rw-rw-rw-   0        0        0     2633 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_user/ui/views.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.747323 badi_users-0.9.7/badi_users.egg-info/
--rw-rw-rw-   0        0        0      419 2023-04-24 14:21:03.000000 badi_users-0.9.7/badi_users.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10750 2023-04-24 14:21:03.000000 badi_users-0.9.7/badi_users.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 14:21:03.000000 badi_users-0.9.7/badi_users.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-24 14:21:03.000000 badi_users-0.9.7/badi_users.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.837085 badi_users-0.9.7/badi_utils/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/__init__.py
--rw-rw-rw-   0        0        0     6835 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/date_calc.py
--rw-rw-rw-   0        0        0    28225 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/dynamic.py
--rw-rw-rw-   0        0        0    22478 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/dynamic_api.py
--rw-rw-rw-   0        0        0     3412 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/dynamic_models.py
--rw-rw-rw-   0        0        0     2990 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/email.py
--rw-rw-rw-   0        0        0      252 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/errors.py
--rw-rw-rw-   0        0        0     1509 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/logging.py
--rw-rw-rw-   0        0        0      947 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/responses.py
--rw-rw-rw-   0        0        0      904 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/rss.py
--rw-rw-rw-   0        0        0     1529 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/select2.py
--rw-rw-rw-   0        0        0     2956 2023-04-16 12:07:37.000000 badi_users-0.9.7/badi_utils/sms.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.218390 badi_users-0.9.7/badi_utils/static/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.219386 badi_users-0.9.7/badi_utils/static/badi_utils/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.846060 badi_users-0.9.7/badi_utils/static/badi_utils/css/
--rw-rw-rw-   0        0        0    40504 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/custom.css
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:05.501624 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/
--rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot
--rw-rw-rw-   0        0        0    59532 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf
--rw-rw-rw-   0        0        0    38401 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff
--rw-rw-rw-   0        0        0    31304 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2
--rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot
--rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot
--rw-rw-rw-   0        0        0    57268 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf
--rw-rw-rw-   0        0        0    36069 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff
--rw-rw-rw-   0        0        0    28856 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2
--rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot
--rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot
--rw-rw-rw-   0        0        0    60584 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf
--rw-rw-rw-   0        0        0    39557 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff
--rw-rw-rw-   0        0        0    32344 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2
--rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot
--rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot
--rw-rw-rw-   0        0        0    58192 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf
--rw-rw-rw-   0        0        0    36145 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff
--rw-rw-rw-   0        0        0    28912 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2
--rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot
--rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot
--rw-rw-rw-   0        0        0    56352 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf
--rw-rw-rw-   0        0        0    36913 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff
--rw-rw-rw-   0        0        0    30072 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2
--rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot
--rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot
--rw-rw-rw-   0        0        0    38473 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff
--rw-rw-rw-   0        0        0    31320 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2
--rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot
--rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot
--rw-rw-rw-   0        0        0    57760 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf
--rw-rw-rw-   0        0        0    36629 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff
--rw-rw-rw-   0        0        0    29688 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2
--rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot
--rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot
--rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot
--rw-rw-rw-   0        0        0    59968 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf
--rw-rw-rw-   0        0        0    39693 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff
--rw-rw-rw-   0        0        0    32420 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2
--rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot
--rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot
--rw-rw-rw-   0        0        0    57544 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf
--rw-rw-rw-   0        0        0    36141 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff
--rw-rw-rw-   0        0        0    28916 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2
--rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot
--rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot
--rw-rw-rw-   0        0        0    55640 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf
--rw-rw-rw-   0        0        0    36945 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff
--rw-rw-rw-   0        0        0    29840 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2
--rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot
--rw-rw-rw-   0        0        0    93376 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf
--rw-rw-rw-   0        0        0    94304 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf
--rw-rw-rw-   0        0        0    94740 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/Ray.ttf
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:05.896975 badi_users-0.9.7/badi_utils/static/badi_utils/js/
--rw-rw-rw-   0        0        0   478686 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/apexchart.js
--rw-rw-rw-   0        0        0    19110 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/api-login.js
--rw-rw-rw-   0        0        0    20445 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/api.js
--rw-rw-rw-   0        0        0    25944 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/base.js
--rw-rw-rw-   0        0        0     2149 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/chat.js
--rw-rw-rw-   0        0        0     3167 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/custom-vue.js
--rw-rw-rw-   0        0        0    18429 2023-04-16 15:34:42.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/datatable.js
--rw-rw-rw-   0        0        0     2470 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/image-field.js
--rw-rw-rw-   0        0        0    30541 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/main.js
--rw-rw-rw-   0        0        0      959 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/notification.js
--rw-rw-rw-   0        0        0     2213 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/pagination-vue.js
--rw-rw-rw-   0        0        0    20317 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/tableexport.js
--rw-rw-rw-   0        0        0      654 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/transaction.js
--rw-rw-rw-   0        0        0   354110 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/vue.js
--rw-rw-rw-   0        0        0   268386 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/static/badi_utils/js/xlsx.mini.min.js
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:05.903957 badi_users-0.9.7/badi_utils/templates/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.008677 badi_users-0.9.7/badi_utils/templates/component/
--rw-rw-rw-   0        0        0     1777 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/createModal.html
--rw-rw-rw-   0        0        0     1645 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/createTitle.html
--rw-rw-rw-   0        0        0     1054 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/filter-form.html
--rw-rw-rw-   0        0        0      729 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/form-errors.html
--rw-rw-rw-   0        0        0     1340 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/form-progressbar-js.html
--rw-rw-rw-   0        0        0      491 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/form-progressbar.html
--rw-rw-rw-   0        0        0      342 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/form.html
--rw-rw-rw-   0        0        0     1231 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/image-field.html
--rw-rw-rw-   0        0        0    34439 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/index-menu.html
--rw-rw-rw-   0        0        0     2346 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/input.html
--rw-rw-rw-   0        0        0       69 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/loader.html
--rw-rw-rw-   0        0        0      468 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/menu-item.html
--rw-rw-rw-   0        0        0      362 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/menu-list.html
--rw-rw-rw-   0        0        0      746 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/messages.html
--rw-rw-rw-   0        0        0     1134 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/pagination-vue.html
--rw-rw-rw-   0        0        0      361 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/profile_item.html
--rw-rw-rw-   0        0        0      204 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/space-between.html
--rw-rw-rw-   0        0        0      430 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/svg-button-with-text.html
--rw-rw-rw-   0        0        0      428 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/svg-button.html
--rw-rw-rw-   0        0        0     1411 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/table-item.html
--rw-rw-rw-   0        0        0     2114 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/user-card.html
--rw-rw-rw-   0        0        0      257 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/component/yesno.html
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.249779 badi_users-0.9.7/badi_utils/templates/svg/
--rw-rw-rw-   0        0        0     1949 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/Incoming-box.html
--rw-rw-rw-   0        0        0     1159 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/add-user.html
--rw-rw-rw-   0        0        0     1092 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/address-book.html
--rw-rw-rw-   0        0        0     1095 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/arrow-left.html
--rw-rw-rw-   0        0        0     1081 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/arrow-right.html
--rw-rw-rw-   0        0        0     2024 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/bitcoin.html
--rw-rw-rw-   0        0        0      697 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/box.html
--rw-rw-rw-   0        0        0     1378 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/calendar-day.html
--rw-rw-rw-   0        0        0     1489 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/calendar-gym.html
--rw-rw-rw-   0        0        0      925 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/calendar.html
--rw-rw-rw-   0        0        0     1223 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/call.html
--rw-rw-rw-   0        0        0     1385 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/category.html
--rw-rw-rw-   0        0        0     1270 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/chat.html
--rw-rw-rw-   0        0        0      938 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/check.html
--rw-rw-rw-   0        0        0      344 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/circle.html
--rw-rw-rw-   0        0        0     1686 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/city.html
--rw-rw-rw-   0        0        0     1430 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/clipboard-list.html
--rw-rw-rw-   0        0        0     2247 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/clock.html
--rw-rw-rw-   0        0        0      645 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/close.html
--rw-rw-rw-   0        0        0     2483 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/collection.html
--rw-rw-rw-   0        0        0     1046 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/comment.html
--rw-rw-rw-   0        0        0     1103 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/dashboard.html
--rw-rw-rw-   0        0        0      893 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/delete.html
--rw-rw-rw-   0        0        0     1505 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/download.html
--rw-rw-rw-   0        0        0      901 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/edit.html
--rw-rw-rw-   0        0        0     1361 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/file-check.html
--rw-rw-rw-   0        0        0      988 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/file.html
--rw-rw-rw-   0        0        0     2111 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/film.html
--rw-rw-rw-   0        0        0      681 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/fire.html
--rw-rw-rw-   0        0        0     1648 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/group-chat.html
--rw-rw-rw-   0        0        0     1213 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/group.html
--rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/half_star.html
--rw-rw-rw-   0        0        0      944 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/home.html
--rw-rw-rw-   0        0        0     1906 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/hourse.html
--rw-rw-rw-   0        0        0      631 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/image.html
--rw-rw-rw-   0        0        0      508 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/info.html
--rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/interview.html
--rw-rw-rw-   0        0        0     1389 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/key.html
--rw-rw-rw-   0        0        0     2472 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/logout.html
--rw-rw-rw-   0        0        0      940 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/mail.html
--rw-rw-rw-   0        0        0      731 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/map.html
--rw-rw-rw-   0        0        0     1601 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/message.html
--rw-rw-rw-   0        0        0     1607 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/messages.html
--rw-rw-rw-   0        0        0      683 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/notification.html
--rw-rw-rw-   0        0        0      708 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/plus.html
--rw-rw-rw-   0        0        0      753 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/puzzle.html
--rw-rw-rw-   0        0        0      882 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/question.html
--rw-rw-rw-   0        0        0     1174 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/refresh.html
--rw-rw-rw-   0        0        0     1416 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/safe.html
--rw-rw-rw-   0        0        0     1091 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/search.html
--rw-rw-rw-   0        0        0     1114 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/shield-protected.html
--rw-rw-rw-   0        0        0     1219 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/shield-user.html
--rw-rw-rw-   0        0        0      451 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/slide.html
--rw-rw-rw-   0        0        0     1587 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/timer.html
--rw-rw-rw-   0        0        0     1043 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/town.html
--rw-rw-rw-   0        0        0      804 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/user.html
--rw-rw-rw-   0        0        0      936 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/wallet.html
--rw-rw-rw-   0        0        0      933 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/svg/warning.html
--rw-rw-rw-   0        0        0       19 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templates/test.html
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.259752 badi_users-0.9.7/badi_utils/templatetags/
--rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templatetags/__init__.py
--rw-rw-rw-   0        0        0      148 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/templatetags/badi_utils.py
--rw-rw-rw-   0        0        0     7102 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/utils.py
--rw-rw-rw-   0        0        0     1911 2023-04-11 07:22:40.000000 badi_users-0.9.7/badi_utils/validations.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.288675 badi_users-0.9.7/badi_visit/
--rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.7/badi_visit/__init__.py
--rw-rw-rw-   0        0        0      167 2022-11-10 16:59:20.000000 badi_users-0.9.7/badi_visit/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.305630 badi_users-0.9.7/badi_visit/api/
--rw-rw-rw-   0        0        0        0 2022-10-24 15:37:24.000000 badi_users-0.9.7/badi_visit/api/__init__.py
--rw-rw-rw-   0        0        0     2871 2022-11-10 16:59:20.000000 badi_users-0.9.7/badi_visit/api/api.py
--rw-rw-rw-   0        0        0      208 2022-11-10 16:59:20.000000 badi_users-0.9.7/badi_visit/api/routers.py
--rw-rw-rw-   0        0        0      185 2022-11-10 16:59:20.000000 badi_users-0.9.7/badi_visit/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.306627 badi_users-0.9.7/badi_visit/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.7/badi_visit/migrations/__init__.py
--rw-rw-rw-   0        0        0     1614 2022-11-10 16:59:20.000000 badi_users-0.9.7/badi_visit/models.py
--rw-rw-rw-   0        0        0       63 2022-08-14 04:14:27.000000 badi_users-0.9.7/badi_visit/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.349512 badi_users-0.9.7/badi_wallet/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_wallet/__init__.py
--rw-rw-rw-   0        0        0     8873 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_wallet/action.py
--rw-rw-rw-   0        0        0      202 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_wallet/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.374446 badi_users-0.9.7/badi_wallet/api/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_wallet/api/__init__.py
--rw-rw-rw-   0        0        0      241 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_wallet/api/routers.py
--rw-rw-rw-   0        0        0      543 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_wallet/api/serializers.py
--rw-rw-rw-   0        0        0     8037 2023-03-29 08:19:18.000000 badi_users-0.9.7/badi_wallet/api/view_sets.py
--rw-rw-rw-   0        0        0      243 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_wallet/apps.py
--rw-rw-rw-   0        0        0      350 2023-03-28 19:16:55.000000 badi_users-0.9.7/badi_wallet/filter.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.225369 badi_users-0.9.7/badi_wallet/locale/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:03.225369 badi_users-0.9.7/badi_wallet/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.381427 badi_users-0.9.7/badi_wallet/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1633 2023-04-16 12:25:06.000000 badi_users-0.9.7/badi_wallet/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.382424 badi_users-0.9.7/badi_wallet/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.7/badi_wallet/migrations/__init__.py
--rw-rw-rw-   0        0        0     3146 2023-03-30 05:05:34.000000 badi_users-0.9.7/badi_wallet/models.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.383423 badi_users-0.9.7/badi_wallet/templates/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_wallet/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.442266 badi_users-0.9.7/badi_wallet/templates/transaction/
--rw-rw-rw-   0        0        0     6145 2023-03-29 08:22:24.000000 badi_users-0.9.7/badi_wallet/templates/transaction/all_transaction_list.html
--rw-rw-rw-   0        0        0    10786 2023-03-30 06:06:20.000000 badi_users-0.9.7/badi_wallet/templates/transaction/all_transaction_report.html
--rw-rw-rw-   0        0        0     2251 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_wallet/templates/transaction/request-transaction.html
--rw-rw-rw-   0        0        0     6203 2023-03-29 08:22:11.000000 badi_users-0.9.7/badi_wallet/templates/transaction/transaction_list.html
--rw-rw-rw-   0        0        0     3547 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_wallet/templates/transaction/transaction_result.html
--rw-rw-rw-   0        0        0       63 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_wallet/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-24 14:21:06.460216 badi_users-0.9.7/badi_wallet/ui/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.7/badi_wallet/ui/__init__.py
--rw-rw-rw-   0        0        0      577 2023-03-28 19:11:37.000000 badi_users-0.9.7/badi_wallet/ui/urls.py
--rw-rw-rw-   0        0        0     1449 2023-03-28 19:16:42.000000 badi_users-0.9.7/badi_wallet/ui/views.py
--rw-rw-rw-   0        0        0       42 2023-04-24 14:21:06.463208 badi_users-0.9.7/setup.cfg
--rw-rw-rw-   0        0        0      498 2023-04-24 14:20:02.000000 badi_users-0.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.180599 badi_users-0.9.8/
+-rw-rw-rw-   0        0        0     1093 2022-09-24 06:05:13.000000 badi_users-0.9.8/LICENSE
+-rw-rw-rw-   0        0        0     1066 2022-11-10 17:03:20.000000 badi_users-0.9.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      419 2023-04-27 08:35:12.180599 badi_users-0.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2022-10-02 09:04:41.000000 badi_users-0.9.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.821560 badi_users-0.9.8/badi_ticket/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_ticket/__init__.py
+-rw-rw-rw-   0        0        0      143 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_ticket/admin.py
+-rw-rw-rw-   0        0        0     9892 2023-04-27 05:00:29.000000 badi_users-0.9.8/badi_ticket/api.py
+-rw-rw-rw-   0        0        0      129 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_ticket/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.775615 badi_users-0.9.8/badi_ticket/locale/
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.775615 badi_users-0.9.8/badi_ticket/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.823554 badi_users-0.9.8/badi_ticket/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2781 2023-04-16 12:25:05.000000 badi_users-0.9.8/badi_ticket/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.824551 badi_users-0.9.8/badi_ticket/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.8/badi_ticket/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4385 2023-04-26 10:23:20.000000 badi_users-0.9.8/badi_ticket/models.py
+-rw-rw-rw-   0        0        0      313 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_ticket/routers.py
+-rw-rw-rw-   0        0        0     2332 2023-04-26 10:22:58.000000 badi_users-0.9.8/badi_ticket/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.776611 badi_users-0.9.8/badi_ticket/static/
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.776611 badi_users-0.9.8/badi_ticket/static/ticket/
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.825548 badi_users-0.9.8/badi_ticket/static/ticket/js/
+-rw-rw-rw-   0        0        0     2448 2023-04-16 09:16:22.000000 badi_users-0.9.8/badi_ticket/static/ticket/js/chat.js
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.827546 badi_users-0.9.8/badi_ticket/templates/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_ticket/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.835522 badi_users-0.9.8/badi_ticket/templates/ticket/
+-rw-rw-rw-   0        0        0     6358 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_ticket/templates/ticket/admin_tickets.html
+-rw-rw-rw-   0        0        0     5265 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_ticket/templates/ticket/message_list.html
+-rw-rw-rw-   0        0        0     9642 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_ticket/templates/ticket/my_tickets.html
+-rw-rw-rw-   0        0        0     7214 2023-04-27 04:28:28.000000 badi_users-0.9.8/badi_ticket/templates/ticket/ticket_create.html
+-rw-rw-rw-   0        0        0     1639 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_ticket/templates/ticket/ticket_update.html
+-rw-rw-rw-   0        0        0       63 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_ticket/tests.py
+-rw-rw-rw-   0        0        0      583 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_ticket/urls.py
+-rw-rw-rw-   0        0        0     2099 2023-04-27 04:25:44.000000 badi_users-0.9.8/badi_ticket/views.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.844499 badi_users-0.9.8/badi_user/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.851479 badi_users-0.9.8/badi_user/api/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/api/__init__.py
+-rw-rw-rw-   0        0        0    29463 2023-04-24 07:10:08.000000 badi_users-0.9.8/badi_user/api/api.py
+-rw-rw-rw-   0        0        0      485 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/api/routers.py
+-rw-rw-rw-   0        0        0     6013 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/api/serializers.py
+-rw-rw-rw-   0        0        0      183 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/apps.py
+-rw-rw-rw-   0        0        0     3428 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/filter.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.785656 badi_users-0.9.8/badi_user/locale/
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.785656 badi_users-0.9.8/badi_user/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.852476 badi_users-0.9.8/badi_user/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     4486 2023-04-16 12:25:06.000000 badi_users-0.9.8/badi_user/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.854472 badi_users-0.9.8/badi_user/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.8/badi_user/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6975 2023-04-24 14:19:52.000000 badi_users-0.9.8/badi_user/models.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.856468 badi_users-0.9.8/badi_user/templates/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/templates/__init__.py
+-rw-rw-rw-   0        0        0       27 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/templates/badi-user-test.html
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.858460 badi_users-0.9.8/badi_user/templates/group/
+-rw-rw-rw-   0        0        0     8558 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/templates/group/group_create.html
+-rw-rw-rw-   0        0        0     5472 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/templates/group/group_update.html
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.859459 badi_users-0.9.8/badi_user/templates/log/
+-rw-rw-rw-   0        0        0     3987 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/templates/log/log_list.html
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.861453 badi_users-0.9.8/badi_user/templates/login-theme/
+-rw-rw-rw-   0        0        0     7336 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/templates/login-theme/login-1.html
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.866440 badi_users-0.9.8/badi_user/templates/member/
+-rw-rw-rw-   0        0        0     6863 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/templates/member/member_create.html
+-rw-rw-rw-   0        0        0    22635 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/templates/member/member_list.html
+-rw-rw-rw-   0        0        0     4783 2023-03-28 07:29:01.000000 badi_users-0.9.8/badi_user/templates/member/member_self_update.html
+-rw-rw-rw-   0        0        0     6525 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/templates/member/member_update.html
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.872424 badi_users-0.9.8/badi_user/templates/user/
+-rw-rw-rw-   0        0        0     5056 2023-04-16 12:18:39.000000 badi_users-0.9.8/badi_user/templates/user/change_password.html
+-rw-rw-rw-   0        0        0     6743 2023-04-24 04:38:27.000000 badi_users-0.9.8/badi_user/templates/user/user_create.html
+-rw-rw-rw-   0        0        0     4019 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/templates/user/user_list.html
+-rw-rw-rw-   0        0        0     5005 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/templates/user/user_update.html
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.874418 badi_users-0.9.8/badi_user/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     5950 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/templatetags/appfilter.py
+-rw-rw-rw-   0        0        0      500 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.886386 badi_users-0.9.8/badi_user/ui/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/ui/__init__.py
+-rw-rw-rw-   0        0        0     1484 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/ui/forms.py
+-rw-rw-rw-   0        0        0      320 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/ui/log_views.py
+-rw-rw-rw-   0        0        0     1706 2023-03-28 08:00:41.000000 badi_users-0.9.8/badi_user/ui/member_views.py
+-rw-rw-rw-   0        0        0      672 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/ui/notification_views.py
+-rw-rw-rw-   0        0        0      644 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/ui/roles_views.py
+-rw-rw-rw-   0        0        0     1624 2023-04-16 08:12:22.000000 badi_users-0.9.8/badi_user/ui/urls.py
+-rw-rw-rw-   0        0        0     2633 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_user/ui/views.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.908327 badi_users-0.9.8/badi_users.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-04-27 08:35:11.000000 badi_users-0.9.8/badi_users.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10750 2023-04-27 08:35:11.000000 badi_users-0.9.8/badi_users.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 08:35:11.000000 badi_users-0.9.8/badi_users.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-27 08:35:11.000000 badi_users-0.9.8/badi_users.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.928274 badi_users-0.9.8/badi_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/__init__.py
+-rw-rw-rw-   0        0        0     6835 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/date_calc.py
+-rw-rw-rw-   0        0        0    28225 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/dynamic.py
+-rw-rw-rw-   0        0        0    22478 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/dynamic_api.py
+-rw-rw-rw-   0        0        0     3412 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/dynamic_models.py
+-rw-rw-rw-   0        0        0     2990 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/email.py
+-rw-rw-rw-   0        0        0      252 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/errors.py
+-rw-rw-rw-   0        0        0     1509 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/logging.py
+-rw-rw-rw-   0        0        0      947 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/responses.py
+-rw-rw-rw-   0        0        0      904 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/rss.py
+-rw-rw-rw-   0        0        0     1529 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/select2.py
+-rw-rw-rw-   0        0        0     2956 2023-04-16 12:07:37.000000 badi_users-0.9.8/badi_utils/sms.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.792636 badi_users-0.9.8/badi_utils/static/
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.794631 badi_users-0.9.8/badi_utils/static/badi_utils/
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.929271 badi_users-0.9.8/badi_utils/static/badi_utils/css/
+-rw-rw-rw-   0        0        0    40504 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/custom.css
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.013047 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/
+-rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot
+-rw-rw-rw-   0        0        0    59532 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf
+-rw-rw-rw-   0        0        0    38401 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff
+-rw-rw-rw-   0        0        0    31304 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2
+-rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot
+-rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot
+-rw-rw-rw-   0        0        0    57268 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf
+-rw-rw-rw-   0        0        0    36069 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff
+-rw-rw-rw-   0        0        0    28856 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2
+-rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot
+-rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot
+-rw-rw-rw-   0        0        0    60584 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf
+-rw-rw-rw-   0        0        0    39557 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff
+-rw-rw-rw-   0        0        0    32344 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2
+-rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot
+-rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot
+-rw-rw-rw-   0        0        0    58192 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf
+-rw-rw-rw-   0        0        0    36145 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff
+-rw-rw-rw-   0        0        0    28912 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2
+-rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot
+-rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot
+-rw-rw-rw-   0        0        0    56352 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf
+-rw-rw-rw-   0        0        0    36913 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff
+-rw-rw-rw-   0        0        0    30072 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2
+-rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot
+-rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot
+-rw-rw-rw-   0        0        0    38473 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff
+-rw-rw-rw-   0        0        0    31320 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2
+-rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot
+-rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot
+-rw-rw-rw-   0        0        0    57760 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf
+-rw-rw-rw-   0        0        0    36629 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff
+-rw-rw-rw-   0        0        0    29688 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2
+-rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot
+-rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot
+-rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot
+-rw-rw-rw-   0        0        0    59968 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf
+-rw-rw-rw-   0        0        0    39693 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff
+-rw-rw-rw-   0        0        0    32420 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2
+-rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot
+-rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot
+-rw-rw-rw-   0        0        0    57544 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf
+-rw-rw-rw-   0        0        0    36141 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff
+-rw-rw-rw-   0        0        0    28916 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2
+-rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot
+-rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot
+-rw-rw-rw-   0        0        0    55640 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf
+-rw-rw-rw-   0        0        0    36945 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff
+-rw-rw-rw-   0        0        0    29840 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2
+-rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot
+-rw-rw-rw-   0        0        0    93376 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf
+-rw-rw-rw-   0        0        0    94304 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf
+-rw-rw-rw-   0        0        0    94740 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/Ray.ttf
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.035985 badi_users-0.9.8/badi_utils/static/badi_utils/js/
+-rw-rw-rw-   0        0        0   478686 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/apexchart.js
+-rw-rw-rw-   0        0        0    19110 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/api-login.js
+-rw-rw-rw-   0        0        0    20445 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/api.js
+-rw-rw-rw-   0        0        0    25944 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/base.js
+-rw-rw-rw-   0        0        0     2149 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/chat.js
+-rw-rw-rw-   0        0        0     3167 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/custom-vue.js
+-rw-rw-rw-   0        0        0    18429 2023-04-16 15:34:42.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/datatable.js
+-rw-rw-rw-   0        0        0     2470 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/image-field.js
+-rw-rw-rw-   0        0        0    30541 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/main.js
+-rw-rw-rw-   0        0        0      959 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/notification.js
+-rw-rw-rw-   0        0        0     2213 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/pagination-vue.js
+-rw-rw-rw-   0        0        0    20317 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/tableexport.js
+-rw-rw-rw-   0        0        0      654 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/transaction.js
+-rw-rw-rw-   0        0        0   354110 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/vue.js
+-rw-rw-rw-   0        0        0   268386 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/static/badi_utils/js/xlsx.mini.min.js
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.038979 badi_users-0.9.8/badi_utils/templates/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.067900 badi_users-0.9.8/badi_utils/templates/component/
+-rw-rw-rw-   0        0        0     1777 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/createModal.html
+-rw-rw-rw-   0        0        0     1645 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/createTitle.html
+-rw-rw-rw-   0        0        0     1054 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/filter-form.html
+-rw-rw-rw-   0        0        0      729 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/form-errors.html
+-rw-rw-rw-   0        0        0     1340 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/form-progressbar-js.html
+-rw-rw-rw-   0        0        0      491 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/form-progressbar.html
+-rw-rw-rw-   0        0        0      342 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/form.html
+-rw-rw-rw-   0        0        0     1231 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/image-field.html
+-rw-rw-rw-   0        0        0    34439 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/index-menu.html
+-rw-rw-rw-   0        0        0     2346 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/input.html
+-rw-rw-rw-   0        0        0       69 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/loader.html
+-rw-rw-rw-   0        0        0      468 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/menu-item.html
+-rw-rw-rw-   0        0        0      362 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/menu-list.html
+-rw-rw-rw-   0        0        0      746 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/messages.html
+-rw-rw-rw-   0        0        0     1134 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/pagination-vue.html
+-rw-rw-rw-   0        0        0      361 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/profile_item.html
+-rw-rw-rw-   0        0        0      204 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/space-between.html
+-rw-rw-rw-   0        0        0      430 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/svg-button-with-text.html
+-rw-rw-rw-   0        0        0      428 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/svg-button.html
+-rw-rw-rw-   0        0        0     1411 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/table-item.html
+-rw-rw-rw-   0        0        0     2114 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/user-card.html
+-rw-rw-rw-   0        0        0      257 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/component/yesno.html
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.137714 badi_users-0.9.8/badi_utils/templates/svg/
+-rw-rw-rw-   0        0        0     1949 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/Incoming-box.html
+-rw-rw-rw-   0        0        0     1159 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/add-user.html
+-rw-rw-rw-   0        0        0     1092 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/address-book.html
+-rw-rw-rw-   0        0        0     1095 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/arrow-left.html
+-rw-rw-rw-   0        0        0     1081 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/arrow-right.html
+-rw-rw-rw-   0        0        0     2024 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/bitcoin.html
+-rw-rw-rw-   0        0        0      697 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/box.html
+-rw-rw-rw-   0        0        0     1378 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/calendar-day.html
+-rw-rw-rw-   0        0        0     1489 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/calendar-gym.html
+-rw-rw-rw-   0        0        0      925 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/calendar.html
+-rw-rw-rw-   0        0        0     1223 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/call.html
+-rw-rw-rw-   0        0        0     1385 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/category.html
+-rw-rw-rw-   0        0        0     1270 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/chat.html
+-rw-rw-rw-   0        0        0      938 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/check.html
+-rw-rw-rw-   0        0        0      344 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/circle.html
+-rw-rw-rw-   0        0        0     1686 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/city.html
+-rw-rw-rw-   0        0        0     1430 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/clipboard-list.html
+-rw-rw-rw-   0        0        0     2247 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/clock.html
+-rw-rw-rw-   0        0        0      645 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/close.html
+-rw-rw-rw-   0        0        0     2483 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/collection.html
+-rw-rw-rw-   0        0        0     1046 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/comment.html
+-rw-rw-rw-   0        0        0     1103 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/dashboard.html
+-rw-rw-rw-   0        0        0      893 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/delete.html
+-rw-rw-rw-   0        0        0     1505 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/download.html
+-rw-rw-rw-   0        0        0      901 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/edit.html
+-rw-rw-rw-   0        0        0     1361 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/file-check.html
+-rw-rw-rw-   0        0        0      988 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/file.html
+-rw-rw-rw-   0        0        0     2111 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/film.html
+-rw-rw-rw-   0        0        0      681 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/fire.html
+-rw-rw-rw-   0        0        0     1648 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/group-chat.html
+-rw-rw-rw-   0        0        0     1213 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/group.html
+-rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/half_star.html
+-rw-rw-rw-   0        0        0      944 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/home.html
+-rw-rw-rw-   0        0        0     1906 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/hourse.html
+-rw-rw-rw-   0        0        0      631 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/image.html
+-rw-rw-rw-   0        0        0      508 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/info.html
+-rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/interview.html
+-rw-rw-rw-   0        0        0     1389 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/key.html
+-rw-rw-rw-   0        0        0     2472 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/logout.html
+-rw-rw-rw-   0        0        0      940 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/mail.html
+-rw-rw-rw-   0        0        0      731 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/map.html
+-rw-rw-rw-   0        0        0     1601 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/message.html
+-rw-rw-rw-   0        0        0     1607 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/messages.html
+-rw-rw-rw-   0        0        0      683 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/notification.html
+-rw-rw-rw-   0        0        0      708 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/plus.html
+-rw-rw-rw-   0        0        0      753 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/puzzle.html
+-rw-rw-rw-   0        0        0      882 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/question.html
+-rw-rw-rw-   0        0        0     1174 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/refresh.html
+-rw-rw-rw-   0        0        0     1416 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/safe.html
+-rw-rw-rw-   0        0        0     1091 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/search.html
+-rw-rw-rw-   0        0        0     1114 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/shield-protected.html
+-rw-rw-rw-   0        0        0     1219 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/shield-user.html
+-rw-rw-rw-   0        0        0      451 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/slide.html
+-rw-rw-rw-   0        0        0     1587 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/timer.html
+-rw-rw-rw-   0        0        0     1043 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/town.html
+-rw-rw-rw-   0        0        0      804 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/user.html
+-rw-rw-rw-   0        0        0      936 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/wallet.html
+-rw-rw-rw-   0        0        0      933 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/svg/warning.html
+-rw-rw-rw-   0        0        0       19 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templates/test.html
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.139708 badi_users-0.9.8/badi_utils/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      148 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/templatetags/badi_utils.py
+-rw-rw-rw-   0        0        0     7102 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/utils.py
+-rw-rw-rw-   0        0        0     1911 2023-04-11 07:22:40.000000 badi_users-0.9.8/badi_utils/validations.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.145692 badi_users-0.9.8/badi_visit/
+-rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.8/badi_visit/__init__.py
+-rw-rw-rw-   0        0        0      167 2022-11-10 16:59:20.000000 badi_users-0.9.8/badi_visit/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.149681 badi_users-0.9.8/badi_visit/api/
+-rw-rw-rw-   0        0        0        0 2022-10-24 15:37:24.000000 badi_users-0.9.8/badi_visit/api/__init__.py
+-rw-rw-rw-   0        0        0     2871 2022-11-10 16:59:20.000000 badi_users-0.9.8/badi_visit/api/api.py
+-rw-rw-rw-   0        0        0      208 2022-11-10 16:59:20.000000 badi_users-0.9.8/badi_visit/api/routers.py
+-rw-rw-rw-   0        0        0      185 2022-11-10 16:59:20.000000 badi_users-0.9.8/badi_visit/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.150679 badi_users-0.9.8/badi_visit/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.8/badi_visit/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1614 2022-11-10 16:59:20.000000 badi_users-0.9.8/badi_visit/models.py
+-rw-rw-rw-   0        0        0       63 2022-08-14 04:14:27.000000 badi_users-0.9.8/badi_visit/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.158657 badi_users-0.9.8/badi_wallet/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_wallet/__init__.py
+-rw-rw-rw-   0        0        0     8873 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_wallet/action.py
+-rw-rw-rw-   0        0        0      202 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_wallet/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.163644 badi_users-0.9.8/badi_wallet/api/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_wallet/api/__init__.py
+-rw-rw-rw-   0        0        0      241 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_wallet/api/routers.py
+-rw-rw-rw-   0        0        0      543 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_wallet/api/serializers.py
+-rw-rw-rw-   0        0        0     8037 2023-03-29 08:19:18.000000 badi_users-0.9.8/badi_wallet/api/view_sets.py
+-rw-rw-rw-   0        0        0      243 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_wallet/apps.py
+-rw-rw-rw-   0        0        0      350 2023-03-28 19:16:55.000000 badi_users-0.9.8/badi_wallet/filter.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.799617 badi_users-0.9.8/badi_wallet/locale/
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:11.799617 badi_users-0.9.8/badi_wallet/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.165639 badi_users-0.9.8/badi_wallet/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1633 2023-04-16 12:25:06.000000 badi_users-0.9.8/badi_wallet/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.166636 badi_users-0.9.8/badi_wallet/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.8/badi_wallet/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3146 2023-03-30 05:05:34.000000 badi_users-0.9.8/badi_wallet/models.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.167633 badi_users-0.9.8/badi_wallet/templates/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_wallet/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.174615 badi_users-0.9.8/badi_wallet/templates/transaction/
+-rw-rw-rw-   0        0        0     6145 2023-03-29 08:22:24.000000 badi_users-0.9.8/badi_wallet/templates/transaction/all_transaction_list.html
+-rw-rw-rw-   0        0        0    10786 2023-03-30 06:06:20.000000 badi_users-0.9.8/badi_wallet/templates/transaction/all_transaction_report.html
+-rw-rw-rw-   0        0        0     2251 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_wallet/templates/transaction/request-transaction.html
+-rw-rw-rw-   0        0        0     6203 2023-03-29 08:22:11.000000 badi_users-0.9.8/badi_wallet/templates/transaction/transaction_list.html
+-rw-rw-rw-   0        0        0     3547 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_wallet/templates/transaction/transaction_result.html
+-rw-rw-rw-   0        0        0       63 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_wallet/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-27 08:35:12.178605 badi_users-0.9.8/badi_wallet/ui/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.8/badi_wallet/ui/__init__.py
+-rw-rw-rw-   0        0        0      577 2023-03-28 19:11:37.000000 badi_users-0.9.8/badi_wallet/ui/urls.py
+-rw-rw-rw-   0        0        0     1449 2023-03-28 19:16:42.000000 badi_users-0.9.8/badi_wallet/ui/views.py
+-rw-rw-rw-   0        0        0       42 2023-04-27 08:35:12.180599 badi_users-0.9.8/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-04-27 08:35:06.000000 badi_users-0.9.8/setup.py
```

### Comparing `badi_users-0.9.7/LICENSE` & `badi_users-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/MANIFEST.in` & `badi_users-0.9.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_ticket/api.py` & `badi_users-0.9.8/badi_ticket/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,20 +37,21 @@
         count += 1
 
     BADI_AUTH_CONFIG.get('sms').get('sms_panel').board_send(users, message_text)
     return count
 
 
 class TicketViewSet(DynamicModelApi):
-    columns = ['id', 'writer', 'title', 'is_closed', 'created_at', ]
-    order_columns = ['id', 'writer', 'title', 'is_closed', 'created_at', ]
+    columns = ['id', 'writer', 'title', 'category', 'is_closed', 'created_at', ]
+    order_columns = ['id', 'writer', 'title', 'category', 'is_closed', 'created_at', ]
     model = Ticket
     queryset = Ticket.objects.all()
     serializer_class = TicketCreateSerializer
     custom_perms = {
+        'list': True,
         'datatable': True,
         'create': True,
     }
 
     def render_column(self, row, column):
         if column == 'is_closed':
             if self.request.user.is_admin:
@@ -223,14 +224,15 @@
                 'is_seen': msg.is_seen, 'is_seen_by_admin': msg.is_seen_by_admin,
                 'created_at': custom_change_date(msg.created_at, 4),
             } for msg in messages
         ]
         return JsonResponse({'response': res, 'ticket': {
             'fullname': ticket.writer.get_full_name(),
             'title': ticket.title,
+            'category': ticket.category,
             'is_closed': ticket.is_closed,
             'created_at': custom_change_date(ticket.created_at, 4),
         }})
 
     def filter_queryset(self, qs):
         return super().filter_queryset(qs)
```

### Comparing `badi_users-0.9.7/badi_ticket/locale/fa/LC_MESSAGES/django.mo` & `badi_users-0.9.8/badi_ticket/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_ticket/models.py` & `badi_users-0.9.8/badi_ticket/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from random import choices
+
 from django.utils.deconstruct import deconstructible
 
 from badi_utils.dynamic_models import BadiModel
 from django.core.validators import MaxLengthValidator, BaseValidator
 from django.db import models
 from rest_framework.exceptions import ValidationError
 from django.utils.translation import gettext_lazy as _, ngettext_lazy
@@ -38,23 +40,41 @@
     class Meta:
         verbose_name = _('Ticket')
         verbose_name_plural = _('Ticket')
         permissions = (
             ('can_ticket', _('Manage Tickets')),
         )
 
+    TICKET_CHOICES = (
+        ('sell', _('Sell')),
+        ('public_question', _('Public question')),
+        ('technical_question', _('Technical question')),
+        ('authentication', _('Authentication')),
+        ('complaint', _('Complaint')),
+        ('financial', _('Financial')),
+        ('other', _('Other')),
+    )
     writer = models.ForeignKey(User, null=True, related_name='tickets', on_delete=models.CASCADE,
                                verbose_name=_('Member'))
     title = models.CharField(max_length=255, verbose_name=_('Title'))
+    category = models.CharField(max_length=50, choices=TICKET_CHOICES, default="public_question", )
     is_closed = models.BooleanField(default=False, verbose_name=_('is Closed'))
     created_at = models.DateTimeField(auto_now_add=True, blank=True, verbose_name=_("Created at"))
 
     def __str__(self):
         return self.title + ' (' + self.writer.__str__() + ')'
 
+    def unread_count(self, user=None):
+        count = 0
+        if user.is_admin:
+            count = self.messages.filter(is_seen_by_admin=False).count()
+        else:
+            count = self.messages.filter(is_seen=False).count()
+        return count
+
     def unread_messages(self, user):
         if user.is_admin:
             return self.messages.filter(is_seen_by_admin=False)
         else:
             return self.messages.filter(is_seen=False)
 
     @staticmethod
```

### Comparing `badi_users-0.9.7/badi_ticket/serializers.py` & `badi_users-0.9.8/badi_ticket/serializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,38 @@
+from rest_framework import serializers
+
 from badi_utils.dynamic_api import api_error_creator, CustomValidation
 from badi_utils.dynamic_api import DynamicSerializer
 from badi_ticket.models import Ticket, Message
 
 
 class TicketCreateSerializer(DynamicSerializer):
     remove_field_view = {
     }
+    unread_messages = serializers.SerializerMethodField()
 
     class Meta:
         model = Ticket
         extra_kwargs = api_error_creator(Ticket,
-                                         ['writer', 'title', 'created_at', 'is_closed', ],
+                                         ['writer', 'title', 'category', 'created_at', 'is_closed', ],
                                          blank_fields=['writer'],
                                          required_fields=[])
         depth = 2
-        fields = ['id', 'writer', 'title', 'created_at', 'is_closed', ]
+        fields = ['id', 'writer', 'title', 'created_at', 'category', 'is_closed', 'unread_messages', ]
 
     def create(self, validated_data):
         creator = self.context['request'].user
         if creator.is_member():
             validated_data['writer'] = creator
         validated_data['is_closed'] = False
         return super().create(validated_data)
 
+    def get_unread_messages(self, obj):
+        return obj.unread_count(self.context['request'].user)
+
 
 class MessageCreateSerializer(DynamicSerializer):
     remove_field_view = {
     }
 
     class Meta:
         model = Message
```

### Comparing `badi_users-0.9.7/badi_ticket/static/ticket/js/chat.js` & `badi_users-0.9.8/badi_ticket/static/ticket/js/chat.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_ticket/templates/ticket/admin_tickets.html` & `badi_users-0.9.8/badi_ticket/templates/ticket/admin_tickets.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_ticket/templates/ticket/message_list.html` & `badi_users-0.9.8/badi_ticket/templates/ticket/message_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_ticket/templates/ticket/my_tickets.html` & `badi_users-0.9.8/badi_ticket/templates/ticket/my_tickets.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_ticket/templates/ticket/ticket_create.html` & `badi_users-0.9.8/badi_ticket/templates/ticket/ticket_create.html`

 * *Files 6% similar despite different names*

```diff
@@ -35,16 +35,17 @@
 														   placeholder="{% trans 'Title' %}..." name="title"
 														   id="ticket-name">
 												</div>
 												<label class="d-none">
 													<input type="hidden" value="{{ object.writer }}" name="writer">
 												</label>
 												{% if request.user.is_admin %}
-													{{ form.writer }}
+													{% include 'component/input.html' with input=form.writer %}
 												{% endif %}
+												{% include 'component/input.html' with input=form.category %}
 											</div>
 											<div class="card-footer p-2">
 												<button type="button"
 														class="btn mx-2 btn-light-primary font-weight-bold"
 														data-dismiss="modal">{% trans "Cancel" %}
 												</button>
 												<button class="btn btn-primary">
@@ -127,29 +128,29 @@
                     {% else %}
                     .html(
                 {% endif %}
                 `
     <a href="messages/${data[0]}" data-skin="dark" data-toggle="tooltip" data-placement="top" title="" data-original-title="{% trans 'Messages' %}" class="btn btn-sm btn-light-primary btn-icon"><span class="svg-icon svg-icon-md">{% include 'svg/message.html' %}</span></button>
                 `)
                 console.log('DATA', data)
-                const status_list = data[3]
+                const status_list = data[4]
                 const is_closed = status_list[0]
                 const count = status_list[1]
                 let last_message = status_list[2]
                 let color = 'dark'
                 if (last_message === -1) {
                     last_message = '{% trans "empty ticket" %}'
                 } else if (last_message === 0) {
                     last_message = '{% trans "waiting to answer" %}'
                     color = 'danger'
                 } else if (last_message === 1) {
                     last_message = '{% trans "answered" %}'
                     color = 'success'
                 }
-                $(`td:eq(1)`, row).html(
+                $(`td:eq(2)`, row).html(
                     `<label class="label label-xl label-inline font-weight-bold label-light-${color}">
 						<span class="label label-xl mr-2 label-dot label-${color}"></span> {% trans "Ticket" %}: ${is_closed ? '{% trans "close" %}' : '{% trans "open" %}'} - ${last_message}
 					</label>
 `
                 )
 
             },
```

#### html2text {}

```diff
@@ -1,14 +1,16 @@
 {% extends request.user.is_admin|yesno:"base.html,base-ui.html" %} {% load
 static %} {% load widget_tweaks %} {% load i18n %} {% block body %}
 **** {% trans "List" %} {{ model_name }} ****
 ** {% trans "Create" %} {% trans "Ticket" %} **
 
 {% csrf_token %}
 {% trans "Title" %}: [title               ]
-   {% if request.user.is_admin %} {{ form.writer }} {% endif %}
+   {% if request.user.is_admin %} {% include 'component/input.html' with
+input=form.writer %} {% endif %} {% include 'component/input.html' with
+input=form.category %}
 {% trans "Cancel" %}   {% trans "Submit" %} {% trans "Ticket" %}
  {% trans "Submit" %} {% trans "Ticket" %}
 {% if not disableTable %}
 {% endif %}
  {% endblock %} {% block script %}
  {% endblock %}
```

### Comparing `badi_users-0.9.7/badi_ticket/templates/ticket/ticket_update.html` & `badi_users-0.9.8/badi_ticket/templates/ticket/ticket_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_ticket/urls.py` & `badi_users-0.9.8/badi_ticket/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_ticket/views.py` & `badi_users-0.9.8/badi_ticket/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 User = get_user_model()
 
 
 class TicketListView(DynamicListView):
     # permission_required = ROLES_ADMIN_TEACHER
     permission_required = True
     model = Ticket
-    datatable_cols = ['#', _('Member'), _('Title'), _('Status'), _("Created at")]
+    datatable_cols = ['#', _('Member'), _('Title'), _('Category'), _('Status'), _("Created at")]
 
 
 class TicketCreateView(DynamicCreateView):
     model = Ticket
     success_url = '/ticket/ticket/list'
     permission_required = True
-    datatable_cols = ['#', _('Member'), _('Title'), _('Status'), _("Created at")]
+    datatable_cols = ['#', _('Member'), _('Title'), _('Category'), _('Status'), _("Created at")]
     # permission_required = ROLES_ADMIN_TEACHER
-    form_fields = ['title', 'writer']
+    form_fields = ['title', 'writer', 'category']
 
     # updateURL = '/ticket/ticket/update/0'
 
     def get_extra_context(self, context):
         context['form'].fields['writer'].queryset = User.objects.none()
         return super().get_extra_context(context)
```

### Comparing `badi_users-0.9.7/badi_user/api/api.py` & `badi_users-0.9.8/badi_user/api/api.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/api/serializers.py` & `badi_users-0.9.8/badi_user/api/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/filter.py` & `badi_users-0.9.8/badi_user/filter.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/locale/fa/LC_MESSAGES/django.mo` & `badi_users-0.9.8/badi_user/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/models.py` & `badi_users-0.9.8/badi_user/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/templates/group/group_create.html` & `badi_users-0.9.8/badi_user/templates/group/group_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/templates/group/group_update.html` & `badi_users-0.9.8/badi_user/templates/group/group_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/templates/log/log_list.html` & `badi_users-0.9.8/badi_user/templates/log/log_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/templates/login-theme/login-1.html` & `badi_users-0.9.8/badi_user/templates/login-theme/login-1.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/templates/member/member_create.html` & `badi_users-0.9.8/badi_user/templates/member/member_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/templates/member/member_list.html` & `badi_users-0.9.8/badi_user/templates/member/member_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/templates/member/member_self_update.html` & `badi_users-0.9.8/badi_user/templates/member/member_self_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/templates/member/member_update.html` & `badi_users-0.9.8/badi_user/templates/member/member_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/templates/user/change_password.html` & `badi_users-0.9.8/badi_user/templates/user/change_password.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/templates/user/user_create.html` & `badi_users-0.9.8/badi_user/templates/user/user_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/templates/user/user_list.html` & `badi_users-0.9.8/badi_user/templates/user/user_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/templates/user/user_update.html` & `badi_users-0.9.8/badi_user/templates/user/user_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/templatetags/appfilter.py` & `badi_users-0.9.8/badi_user/templatetags/appfilter.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/ui/forms.py` & `badi_users-0.9.8/badi_user/ui/forms.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/ui/member_views.py` & `badi_users-0.9.8/badi_user/ui/member_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/ui/notification_views.py` & `badi_users-0.9.8/badi_user/ui/notification_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/ui/roles_views.py` & `badi_users-0.9.8/badi_user/ui/roles_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/ui/urls.py` & `badi_users-0.9.8/badi_user/ui/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_user/ui/views.py` & `badi_users-0.9.8/badi_user/ui/views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_users.egg-info/SOURCES.txt` & `badi_users-0.9.8/badi_users.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/date_calc.py` & `badi_users-0.9.8/badi_utils/date_calc.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/dynamic.py` & `badi_users-0.9.8/badi_utils/dynamic.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/dynamic_api.py` & `badi_users-0.9.8/badi_utils/dynamic_api.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/dynamic_models.py` & `badi_users-0.9.8/badi_utils/dynamic_models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/email.py` & `badi_users-0.9.8/badi_utils/email.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/logging.py` & `badi_users-0.9.8/badi_utils/logging.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/responses.py` & `badi_users-0.9.8/badi_utils/responses.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/rss.py` & `badi_users-0.9.8/badi_utils/rss.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/select2.py` & `badi_users-0.9.8/badi_utils/select2.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/sms.py` & `badi_users-0.9.8/badi_utils/sms.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/custom.css` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/custom.css`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/css/fonts/Ray.ttf` & `badi_users-0.9.8/badi_utils/static/badi_utils/css/fonts/Ray.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/apexchart.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/apexchart.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/api-login.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/api-login.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/api.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/api.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/base.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/base.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/chat.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/chat.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/custom-vue.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/custom-vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/datatable.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/datatable.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/image-field.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/image-field.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/main.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/main.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/notification.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/notification.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/pagination-vue.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/pagination-vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/tableexport.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/tableexport.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/transaction.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/transaction.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/vue.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/static/badi_utils/js/xlsx.mini.min.js` & `badi_users-0.9.8/badi_utils/static/badi_utils/js/xlsx.mini.min.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/component/createModal.html` & `badi_users-0.9.8/badi_utils/templates/component/createModal.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/component/createTitle.html` & `badi_users-0.9.8/badi_utils/templates/component/createTitle.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/component/filter-form.html` & `badi_users-0.9.8/badi_utils/templates/component/filter-form.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/component/form-errors.html` & `badi_users-0.9.8/badi_utils/templates/component/form-errors.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/component/form-progressbar-js.html` & `badi_users-0.9.8/badi_utils/templates/component/form-progressbar-js.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/component/image-field.html` & `badi_users-0.9.8/badi_utils/templates/component/image-field.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/component/index-menu.html` & `badi_users-0.9.8/badi_utils/templates/component/index-menu.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/component/input.html` & `badi_users-0.9.8/badi_utils/templates/component/input.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/component/messages.html` & `badi_users-0.9.8/badi_utils/templates/component/messages.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/component/pagination-vue.html` & `badi_users-0.9.8/badi_utils/templates/component/pagination-vue.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/component/table-item.html` & `badi_users-0.9.8/badi_utils/templates/component/table-item.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/component/user-card.html` & `badi_users-0.9.8/badi_utils/templates/component/user-card.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/Incoming-box.html` & `badi_users-0.9.8/badi_utils/templates/svg/Incoming-box.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/add-user.html` & `badi_users-0.9.8/badi_utils/templates/svg/add-user.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/address-book.html` & `badi_users-0.9.8/badi_utils/templates/svg/address-book.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/arrow-left.html` & `badi_users-0.9.8/badi_utils/templates/svg/arrow-left.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/arrow-right.html` & `badi_users-0.9.8/badi_utils/templates/svg/arrow-right.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/bitcoin.html` & `badi_users-0.9.8/badi_utils/templates/svg/bitcoin.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/box.html` & `badi_users-0.9.8/badi_utils/templates/svg/box.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/calendar-day.html` & `badi_users-0.9.8/badi_utils/templates/svg/calendar-day.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/calendar-gym.html` & `badi_users-0.9.8/badi_utils/templates/svg/calendar-gym.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/calendar.html` & `badi_users-0.9.8/badi_utils/templates/svg/calendar.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/call.html` & `badi_users-0.9.8/badi_utils/templates/svg/call.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/category.html` & `badi_users-0.9.8/badi_utils/templates/svg/category.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/chat.html` & `badi_users-0.9.8/badi_utils/templates/svg/chat.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/check.html` & `badi_users-0.9.8/badi_utils/templates/svg/check.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/city.html` & `badi_users-0.9.8/badi_utils/templates/svg/city.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/clipboard-list.html` & `badi_users-0.9.8/badi_utils/templates/svg/clipboard-list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/clock.html` & `badi_users-0.9.8/badi_utils/templates/svg/clock.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/close.html` & `badi_users-0.9.8/badi_utils/templates/svg/close.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/collection.html` & `badi_users-0.9.8/badi_utils/templates/svg/collection.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/comment.html` & `badi_users-0.9.8/badi_utils/templates/svg/comment.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/dashboard.html` & `badi_users-0.9.8/badi_utils/templates/svg/dashboard.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/delete.html` & `badi_users-0.9.8/badi_utils/templates/svg/delete.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/download.html` & `badi_users-0.9.8/badi_utils/templates/svg/download.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/edit.html` & `badi_users-0.9.8/badi_utils/templates/svg/edit.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/file-check.html` & `badi_users-0.9.8/badi_utils/templates/svg/file-check.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/file.html` & `badi_users-0.9.8/badi_utils/templates/svg/file.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/film.html` & `badi_users-0.9.8/badi_utils/templates/svg/film.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/fire.html` & `badi_users-0.9.8/badi_utils/templates/svg/fire.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/group-chat.html` & `badi_users-0.9.8/badi_utils/templates/svg/group-chat.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/group.html` & `badi_users-0.9.8/badi_utils/templates/svg/group.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/half_star.html` & `badi_users-0.9.8/badi_utils/templates/svg/half_star.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/home.html` & `badi_users-0.9.8/badi_utils/templates/svg/home.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/hourse.html` & `badi_users-0.9.8/badi_utils/templates/svg/hourse.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/image.html` & `badi_users-0.9.8/badi_utils/templates/svg/image.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/interview.html` & `badi_users-0.9.8/badi_utils/templates/svg/interview.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/key.html` & `badi_users-0.9.8/badi_utils/templates/svg/key.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/logout.html` & `badi_users-0.9.8/badi_utils/templates/svg/logout.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/mail.html` & `badi_users-0.9.8/badi_utils/templates/svg/mail.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/map.html` & `badi_users-0.9.8/badi_utils/templates/svg/map.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/message.html` & `badi_users-0.9.8/badi_utils/templates/svg/message.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/messages.html` & `badi_users-0.9.8/badi_utils/templates/svg/messages.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/notification.html` & `badi_users-0.9.8/badi_utils/templates/svg/notification.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/plus.html` & `badi_users-0.9.8/badi_utils/templates/svg/plus.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/puzzle.html` & `badi_users-0.9.8/badi_utils/templates/svg/puzzle.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/question.html` & `badi_users-0.9.8/badi_utils/templates/svg/question.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/refresh.html` & `badi_users-0.9.8/badi_utils/templates/svg/refresh.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/safe.html` & `badi_users-0.9.8/badi_utils/templates/svg/safe.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/search.html` & `badi_users-0.9.8/badi_utils/templates/svg/search.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/shield-protected.html` & `badi_users-0.9.8/badi_utils/templates/svg/shield-protected.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/shield-user.html` & `badi_users-0.9.8/badi_utils/templates/svg/shield-user.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/timer.html` & `badi_users-0.9.8/badi_utils/templates/svg/timer.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/town.html` & `badi_users-0.9.8/badi_utils/templates/svg/town.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/user.html` & `badi_users-0.9.8/badi_utils/templates/svg/user.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/wallet.html` & `badi_users-0.9.8/badi_utils/templates/svg/wallet.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/templates/svg/warning.html` & `badi_users-0.9.8/badi_utils/templates/svg/warning.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/utils.py` & `badi_users-0.9.8/badi_utils/utils.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_utils/validations.py` & `badi_users-0.9.8/badi_utils/validations.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_visit/api/api.py` & `badi_users-0.9.8/badi_visit/api/api.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_visit/models.py` & `badi_users-0.9.8/badi_visit/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_wallet/action.py` & `badi_users-0.9.8/badi_wallet/action.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_wallet/api/serializers.py` & `badi_users-0.9.8/badi_wallet/api/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_wallet/api/view_sets.py` & `badi_users-0.9.8/badi_wallet/api/view_sets.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_wallet/locale/fa/LC_MESSAGES/django.mo` & `badi_users-0.9.8/badi_wallet/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_wallet/models.py` & `badi_users-0.9.8/badi_wallet/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_wallet/templates/transaction/all_transaction_list.html` & `badi_users-0.9.8/badi_wallet/templates/transaction/all_transaction_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_wallet/templates/transaction/all_transaction_report.html` & `badi_users-0.9.8/badi_wallet/templates/transaction/all_transaction_report.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_wallet/templates/transaction/request-transaction.html` & `badi_users-0.9.8/badi_wallet/templates/transaction/request-transaction.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_wallet/templates/transaction/transaction_list.html` & `badi_users-0.9.8/badi_wallet/templates/transaction/transaction_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_wallet/templates/transaction/transaction_result.html` & `badi_users-0.9.8/badi_wallet/templates/transaction/transaction_result.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_wallet/ui/urls.py` & `badi_users-0.9.8/badi_wallet/ui/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.7/badi_wallet/ui/views.py` & `badi_users-0.9.8/badi_wallet/ui/views.py`

 * *Files identical despite different names*

