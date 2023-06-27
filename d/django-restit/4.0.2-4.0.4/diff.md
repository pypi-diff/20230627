# Comparing `tmp/django_restit-4.0.2.tar.gz` & `tmp/django_restit-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_restit-4.0.2.tar", max compression
+gzip compressed data, was "django_restit-4.0.4.tar", max compression
```

## Comparing `django_restit-4.0.2.tar` & `django_restit-4.0.4.tar`

### file list

```diff
@@ -1,447 +1,452 @@
--rw-r--r--   0        0        0     1068 2023-06-23 21:15:35.136818 django_restit-4.0.2/LICENSE.md
--rw-r--r--   0        0        0     6234 2023-06-23 21:15:35.136901 django_restit-4.0.2/README.md
--rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/__init__.py
--rw-r--r--   0        0        0     1839 2023-06-23 21:15:35.137029 django_restit-4.0.2/account/admin.py
--rw-r--r--   0        0        0      980 2023-06-23 21:15:35.137125 django_restit-4.0.2/account/fcm/__init__.py
--rw-r--r--   0        0        0    15894 2022-09-27 04:43:03.000000 django_restit-4.0.2/account/migrations/0001_initial.py
--rw-r--r--   0        0        0      738 2023-06-23 21:15:35.137234 django_restit-4.0.2/account/migrations/0003_member_phone_number.py
--rw-r--r--   0        0        0      551 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/migrations/0004_group_modified_alter_group_created.py
--rw-r--r--   0        0        0      437 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/migrations/0005_member_auth_code_expires.py
--rw-r--r--   0        0        0      450 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/migrations/0006_member_security_token.py
--rw-r--r--   0        0        0     1654 2022-09-24 21:52:53.000000 django_restit-4.0.2/account/migrations/0007_authtoken_signature_authsession.py
--rw-r--r--   0        0        0     2379 2022-08-11 21:50:51.000000 django_restit-4.0.2/account/migrations/0008_memberdevice_memberdevicemetadata.py
--rw-r--r--   0        0        0      468 2022-09-24 21:54:39.000000 django_restit-4.0.2/account/migrations/0009_alter_member_phone_number.py
--rw-r--r--   0        0        0      305 2022-09-24 21:54:43.000000 django_restit-4.0.2/account/migrations/0010_delete_authtoken.py
--rw-r--r--   0        0        0     1062 2022-09-24 21:56:14.000000 django_restit-4.0.2/account/migrations/0011_authtoken.py
--rw-r--r--   0        0        0     2043 2023-06-23 21:15:35.137371 django_restit-4.0.2/account/migrations/0012_settings_settingsmetadata.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/migrations/__init__.py
--rw-r--r--   0        0        0      341 2023-06-23 21:15:35.137581 django_restit-4.0.2/account/models/__init__.py
--rw-r--r--   0        0        0     3070 2022-11-13 00:07:37.000000 django_restit-4.0.2/account/models/device.py
--rw-r--r--   0        0        0     1437 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/models/feeds.py
--rw-r--r--   0        0        0    18161 2023-06-23 21:15:35.137723 django_restit-4.0.2/account/models/group.py
--rw-r--r--   0        0        0     2720 2022-09-24 05:45:19.000000 django_restit-4.0.2/account/models/legacy.py
--rw-r--r--   0        0        0    45805 2023-06-23 21:15:35.137966 django_restit-4.0.2/account/models/member.py
--rw-r--r--   0        0        0     6842 2023-06-23 21:15:35.138172 django_restit-4.0.2/account/models/membership.py
--rw-r--r--   0        0        0    10739 2023-06-23 21:15:35.138283 django_restit-4.0.2/account/models/notify.py
--rw-r--r--   0        0        0     3345 2023-06-23 21:15:35.138374 django_restit-4.0.2/account/models/session.py
--rw-r--r--   0        0        0     2137 2023-06-23 21:15:35.138434 django_restit-4.0.2/account/models/settings.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.138485 django_restit-4.0.2/account/oauth/__init__.py
--rw-r--r--   0        0        0     2078 2023-06-23 21:15:35.138691 django_restit-4.0.2/account/oauth/google.py
--rw-r--r--   0        0        0      578 2023-06-23 21:15:35.138771 django_restit-4.0.2/account/periodic.py
--rw-r--r--   0        0        0      152 2023-06-23 21:15:35.138965 django_restit-4.0.2/account/rpc/__init__.py
--rw-r--r--   0        0        0    12428 2023-06-23 21:15:35.139084 django_restit-4.0.2/account/rpc/auth.py
--rw-r--r--   0        0        0     2104 2022-11-13 00:14:42.000000 django_restit-4.0.2/account/rpc/device.py
--rw-r--r--   0        0        0     3078 2023-06-23 21:15:35.139179 django_restit-4.0.2/account/rpc/group.py
--rw-r--r--   0        0        0     1150 2022-10-30 01:24:30.000000 django_restit-4.0.2/account/rpc/member.py
--rw-r--r--   0        0        0     3344 2022-10-04 17:23:13.000000 django_restit-4.0.2/account/rpc/notify.py
--rw-r--r--   0        0        0     2610 2023-06-23 21:15:35.139259 django_restit-4.0.2/account/rpc/oauth.py
--rw-r--r--   0        0        0      271 2023-06-23 21:15:35.139434 django_restit-4.0.2/account/rpc/settings.py
--rw-r--r--   0        0        0       53 2023-06-23 21:15:35.139504 django_restit-4.0.2/account/settings.py
--rw-r--r--   0        0        0     9709 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/templates/email/base.html
--rw-r--r--   0        0        0    10567 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/templates/email/invite.html
--rw-r--r--   0        0        0    15185 2023-06-23 21:15:35.139631 django_restit-4.0.2/account/templates/email/plain/invite.html
--rw-r--r--   0        0        0    13954 2023-06-23 21:15:35.139720 django_restit-4.0.2/account/templates/email/plain/reset_code.html
--rw-r--r--   0        0        0    10261 2022-07-28 20:16:05.000000 django_restit-4.0.2/account/templates/email/reset_code.html
--rw-r--r--   0        0        0    15163 2023-06-23 21:15:35.139805 django_restit-4.0.2/account/templates/email/simple/invite.html
--rw-r--r--   0        0        0    13944 2023-06-23 21:15:35.139868 django_restit-4.0.2/account/templates/email/simple/reset_code.html
--rw-r--r--   0        0        0      520 2022-07-29 02:52:46.000000 django_restit-4.0.2/auditlog/README
--rw-r--r--   0        0        0        0 2022-07-29 02:52:46.000000 django_restit-4.0.2/auditlog/__init__.py
--rw-r--r--   0        0        0     1006 2022-09-24 03:15:33.000000 django_restit-4.0.2/auditlog/admin.py
--rw-r--r--   0        0        0     6553 2022-09-24 03:15:33.000000 django_restit-4.0.2/auditlog/decorators.py
--rw-r--r--   0        0        0     1329 2023-06-23 21:15:35.139991 django_restit-4.0.2/auditlog/middleware.py
--rw-r--r--   0        0        0     3309 2022-09-24 03:15:33.000000 django_restit-4.0.2/auditlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-07-29 02:52:46.000000 django_restit-4.0.2/auditlog/migrations/__init__.py
--rw-r--r--   0        0        0    16043 2023-06-23 21:15:35.140513 django_restit-4.0.2/auditlog/models.py
--rw-r--r--   0        0        0      264 2023-06-23 21:15:35.140617 django_restit-4.0.2/auditlog/periodic.py
--rw-r--r--   0        0        0     3591 2022-10-03 03:50:26.000000 django_restit-4.0.2/auditlog/rpc.py
--rw-r--r--   0        0        0     2019 2023-06-23 21:15:35.140714 django_restit-4.0.2/auditlog/tq.py
--rw-r--r--   0        0        0      163 2022-07-29 02:52:46.000000 django_restit-4.0.2/auditlog/urls.py
--rw-r--r--   0        0        0     2169 2023-06-23 21:15:35.140811 django_restit-4.0.2/inbox/README.md
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.140833 django_restit-4.0.2/inbox/__init__.py
--rw-r--r--   0        0        0      243 2023-06-23 21:15:35.140908 django_restit-4.0.2/inbox/admin.py
--rw-r--r--   0        0        0     5621 2023-06-23 21:15:35.140972 django_restit-4.0.2/inbox/handlers.py
--rw-r--r--   0        0        0     6429 2023-06-23 21:15:35.141059 django_restit-4.0.2/inbox/migrations/0001_initial.py
--rw-r--r--   0        0        0      380 2023-06-23 21:15:35.141115 django_restit-4.0.2/inbox/migrations/0002_alter_message_cc.py
--rw-r--r--   0        0        0      416 2023-06-23 21:15:35.141178 django_restit-4.0.2/inbox/migrations/0003_attachment_content_type.py
--rw-r--r--   0        0        0     1140 2023-06-23 21:15:35.141236 django_restit-4.0.2/inbox/migrations/0004_mailtemplate.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.141260 django_restit-4.0.2/inbox/migrations/__init__.py
--rw-r--r--   0        0        0      174 2023-06-23 21:15:35.141369 django_restit-4.0.2/inbox/models/__init__.py
--rw-r--r--   0        0        0     2832 2023-06-23 21:15:35.141433 django_restit-4.0.2/inbox/models/bounce.py
--rw-r--r--   0        0        0     2468 2023-06-23 21:15:35.141520 django_restit-4.0.2/inbox/models/complaint.py
--rw-r--r--   0        0        0     2879 2023-06-23 21:15:35.141710 django_restit-4.0.2/inbox/models/message.py
--rw-r--r--   0        0        0     1013 2023-06-23 21:15:35.141770 django_restit-4.0.2/inbox/models/template.py
--rw-r--r--   0        0        0     1534 2023-06-23 21:15:35.141837 django_restit-4.0.2/inbox/rpc.py
--rw-r--r--   0        0        0       89 2023-06-23 21:15:35.141924 django_restit-4.0.2/inbox/utils/__init__.py
--rw-r--r--   0        0        0     4366 2023-06-23 21:15:35.142001 django_restit-4.0.2/inbox/utils/parsing.py
--rw-r--r--   0        0        0     4098 2023-06-23 21:15:35.142066 django_restit-4.0.2/inbox/utils/render.py
--rw-r--r--   0        0        0     2109 2023-06-23 21:15:35.142125 django_restit-4.0.2/inbox/utils/sending.py
--rw-r--r--   0        0        0     1114 2023-06-23 21:15:35.142232 django_restit-4.0.2/incident/README.md
--rw-r--r--   0        0        0      988 2023-06-23 21:15:35.142301 django_restit-4.0.2/incident/__init__.py
--rw-r--r--   0        0        0     9720 2023-06-23 21:15:35.142408 django_restit-4.0.2/incident/migrations/0001_initial.py
--rw-r--r--   0        0        0      595 2023-06-23 21:15:35.142478 django_restit-4.0.2/incident/migrations/0002_event_component_event_component_id.py
--rw-r--r--   0        0        0      425 2023-06-23 21:15:35.142525 django_restit-4.0.2/incident/migrations/0003_rule_action.py
--rw-r--r--   0        0        0      662 2023-06-23 21:15:35.142574 django_restit-4.0.2/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py
--rw-r--r--   0        0        0      698 2023-06-23 21:15:35.142626 django_restit-4.0.2/incident/migrations/0005_incident_component_alter_incident_state.py
--rw-r--r--   0        0        0      324 2023-06-23 21:15:35.142680 django_restit-4.0.2/incident/migrations/0006_delete_eventmetadata.py
--rw-r--r--   0        0        0      414 2023-06-23 21:15:35.142730 django_restit-4.0.2/incident/migrations/0007_event_metadata.py
--rw-r--r--   0        0        0      903 2023-06-23 21:15:35.142784 django_restit-4.0.2/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.142804 django_restit-4.0.2/incident/migrations/__init__.py
--rw-r--r--   0        0        0      167 2023-06-23 21:15:35.142905 django_restit-4.0.2/incident/models/__init__.py
--rw-r--r--   0        0        0     4976 2023-06-23 21:15:35.142969 django_restit-4.0.2/incident/models/event.py
--rw-r--r--   0        0        0    10022 2023-06-23 21:15:35.143045 django_restit-4.0.2/incident/models/incident.py
--rw-r--r--   0        0        0     2187 2023-06-23 21:15:35.143123 django_restit-4.0.2/incident/models/ossec.py
--rw-r--r--   0        0        0     5300 2023-06-23 21:15:35.143181 django_restit-4.0.2/incident/models/rules.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.143230 django_restit-4.0.2/incident/parsers/__init__.py
--rw-r--r--   0        0        0     5289 2023-06-23 21:15:35.143323 django_restit-4.0.2/incident/parsers/ossec.py
--rw-r--r--   0        0        0      723 2023-06-23 21:15:35.143378 django_restit-4.0.2/incident/periodic.py
--rw-r--r--   0        0        0     2831 2023-06-23 21:15:35.143434 django_restit-4.0.2/incident/rpc.py
--rw-r--r--   0        0        0    12732 2023-06-23 21:15:35.143576 django_restit-4.0.2/incident/templates/email/incident_change.html
--rw-r--r--   0        0        0    15173 2023-06-23 21:15:35.143659 django_restit-4.0.2/incident/templates/email/incident_new.html
--rw-r--r--   0        0        0    13208 2023-06-23 21:15:35.143748 django_restit-4.0.2/incident/templates/email/incident_plain.html
--rw-r--r--   0        0        0      796 2023-06-23 21:15:35.143887 django_restit-4.0.2/incident/tq.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.2/location/__init__.py
--rw-r--r--   0        0        0      297 2023-06-23 21:15:35.143952 django_restit-4.0.2/location/admin.py
--rw-r--r--   0        0        0     1694 2023-06-23 21:15:35.144111 django_restit-4.0.2/location/geolocate.py
--rw-r--r--   0        0        0     7000 2022-07-28 20:16:05.000000 django_restit-4.0.2/location/migrations/0001_initial.py
--rw-r--r--   0        0        0      576 2023-06-23 21:15:35.144178 django_restit-4.0.2/location/migrations/0002_geoip_subnet_alter_geoip_ip.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.2/location/migrations/__init__.py
--rw-r--r--   0        0        0      230 2023-06-23 21:15:35.144260 django_restit-4.0.2/location/models/__init__.py
--rw-r--r--   0        0        0     2028 2023-06-23 21:15:35.144322 django_restit-4.0.2/location/models/address.py
--rw-r--r--   0        0        0     3500 2023-06-23 21:15:35.144407 django_restit-4.0.2/location/models/ip.py
--rw-r--r--   0        0        0     1994 2023-06-23 21:15:35.144467 django_restit-4.0.2/location/models/legacy.py
--rw-r--r--   0        0        0     2316 2023-06-23 21:15:35.144520 django_restit-4.0.2/location/models/location.py
--rw-r--r--   0        0        0     1474 2023-06-23 21:15:35.144569 django_restit-4.0.2/location/models/track.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.144628 django_restit-4.0.2/location/providers/__init__.py
--rw-r--r--   0        0        0      730 2023-06-23 21:15:35.144750 django_restit-4.0.2/location/providers/iplookup/__init__.py
--rw-r--r--   0        0        0     2419 2023-06-23 21:15:35.144808 django_restit-4.0.2/location/providers/iplookup/abstractapi.py
--rw-r--r--   0        0        0     1345 2023-06-23 21:15:35.144857 django_restit-4.0.2/location/providers/iplookup/extremeip.py
--rw-r--r--   0        0        0     2121 2023-06-23 21:15:35.144909 django_restit-4.0.2/location/providers/iplookup/geoplugin.py
--rw-r--r--   0        0        0     1797 2023-06-23 21:15:35.144963 django_restit-4.0.2/location/providers/iplookup/ipapi.py
--rw-r--r--   0        0        0     1265 2023-06-23 21:15:35.145020 django_restit-4.0.2/location/providers/iplookup/ipinfo.py
--rw-r--r--   0        0        0      937 2023-06-23 21:15:35.145073 django_restit-4.0.2/location/providers/iplookup/restit.py
--rw-r--r--   0        0        0       42 2023-06-23 21:15:35.145153 django_restit-4.0.2/location/providers/location/__init__.py
--rw-r--r--   0        0        0     2860 2023-06-23 21:15:35.145211 django_restit-4.0.2/location/providers/location/google.py
--rw-r--r--   0        0        0       46 2023-06-23 21:15:35.145290 django_restit-4.0.2/location/providers/timezones/__init__.py
--rw-r--r--   0        0        0      619 2023-06-23 21:15:35.145347 django_restit-4.0.2/location/providers/timezones/google.py
--rw-r--r--   0        0        0     1935 2023-06-23 21:15:35.145739 django_restit-4.0.2/location/providers/zillow.py
--rw-r--r--   0        0        0      123 2023-06-23 21:15:35.145822 django_restit-4.0.2/location/rpc/__init__.py
--rw-r--r--   0        0        0      782 2023-06-23 21:15:35.145877 django_restit-4.0.2/location/rpc/ip.py
--rw-r--r--   0        0        0      779 2023-06-23 21:15:35.145928 django_restit-4.0.2/location/rpc/location.py
--rw-r--r--   0        0        0     3735 2023-06-23 21:15:35.145987 django_restit-4.0.2/location/rpc/track.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:05.000000 django_restit-4.0.2/medialib/__init__.py
--rw-r--r--   0        0        0     2261 2022-07-28 20:16:05.000000 django_restit-4.0.2/medialib/admin.py
--rw-r--r--   0        0        0       27 2022-07-28 20:16:05.000000 django_restit-4.0.2/medialib/cvutil/__init__.py
--rw-r--r--   0        0        0     4269 2022-07-28 20:16:05.000000 django_restit-4.0.2/medialib/cvutil/contours.py
--rw-r--r--   0        0        0    12649 2022-07-28 20:16:05.000000 django_restit-4.0.2/medialib/cvutil/images.py
--rw-r--r--   0        0        0     9586 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/cvutil/misc.py
--rw-r--r--   0        0        0     5824 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/cvutil/text.py
--rw-r--r--   0        0        0    48442 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/fixtures/initial_data.json
--rw-r--r--   0        0        0    31978 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/fixtures/medialib.json
--rw-r--r--   0        0        0    16989 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/fixtures/medialib_test_fixture.json
--rw-r--r--   0        0        0     5442 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/forms.py
--rw-r--r--   0        0        0    20518 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/migrations/__init__.py
--rw-r--r--   0        0        0    52121 2023-06-23 21:15:35.146207 django_restit-4.0.2/medialib/models.py
--rw-r--r--   0        0        0     1189 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/ocr.py
--rw-r--r--   0        0        0     1275 2023-06-23 21:15:35.146396 django_restit-4.0.2/medialib/pdf.py
--rw-r--r--   0        0        0      545 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/qrcode.py
--rw-r--r--   0        0        0    10312 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/__init__.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/__init__.py
--rw-r--r--   0        0        0     3531 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/anigif.py
--rw-r--r--   0        0        0     6881 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/ffmpeg.py
--rw-r--r--   0        0        0      792 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/gifsicle.py
--rw-r--r--   0        0        0     3436 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/hls.py
--rw-r--r--   0        0        0      983 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/mp4box.py
--rw-r--r--   0        0        0      397 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/rtmp/Makefile
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/rtmp/__init__.py
--rw-r--r--   0        0        0     4026 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/rtmp/rtmp.i
--rw-r--r--   0        0        0      699 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/rtmpdump.py
--rw-r--r--   0        0        0     1017 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/rtmpsink.py
--rw-r--r--   0        0        0     3466 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/video_getinfo.py
--rw-r--r--   0        0        0      809 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/engines/websnap.py
--rw-r--r--   0        0        0     2193 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/exceptions.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/__init__.py
--rw-r--r--   0        0        0     4179 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/akamai.py
--rw-r--r--   0        0        0     3284 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/animated_thumbnail.py
--rw-r--r--   0        0        0     4004 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/ffmpeg.py
--rw-r--r--   0        0        0     2087 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/flv.py
--rw-r--r--   0        0        0     6567 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/hls.py
--rw-r--r--   0        0        0     6955 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/image_transcode.py
--rw-r--r--   0        0        0     1094 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/image_validate.py
--rw-r--r--   0        0        0     2423 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/mp4.py
--rw-r--r--   0        0        0     4997 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/video_still.py
--rw-r--r--   0        0        0     3228 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/video_validate.py
--rw-r--r--   0        0        0      863 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/websnap.py
--rw-r--r--   0        0        0     2282 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/presets/youtube.py
--rw-r--r--   0        0        0    16451 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/render_utils.py
--rw-r--r--   0        0        0      370 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/render/schedule.py
--rw-r--r--   0        0        0       82 2022-10-20 05:50:28.000000 django_restit-4.0.2/medialib/rpc/__init__.py
--rw-r--r--   0        0        0    37925 2022-10-20 05:55:31.000000 django_restit-4.0.2/medialib/rpc/legacy.py
--rw-r--r--   0        0        0      617 2022-10-20 06:03:18.000000 django_restit-4.0.2/medialib/rpc/media.py
--rw-r--r--   0        0        0      956 2022-10-20 05:51:56.000000 django_restit-4.0.2/medialib/rpc/tools.py
--rwxr-xr-x   0        0        0     7875 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/scripts/init_config
--rw-r--r--   0        0        0     4499 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/css/base_medialibui.css
--rw-r--r--   0        0        0     3128 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/css/base_widgets.css
--rw-r--r--   0        0        0     3263 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/css/jquery.jcrop.css
--rw-r--r--   0        0        0      193 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/arrow-down-white.png
--rw-r--r--   0        0        0     4589 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/bg-body.gif
--rw-r--r--   0        0        0      441 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/cancel.gif
--rw-r--r--   0        0        0      341 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/icon-generic.gif
--rw-r--r--   0        0        0      355 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/icon-image.gif
--rw-r--r--   0        0        0      359 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/icon-media.gif
--rw-r--r--   0        0        0      355 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/icon-zip.gif
--rw-r--r--   0        0        0     3208 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/loading.gif
--rw-r--r--   0        0        0     2537 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/noimage.gif
--rw-r--r--   0        0        0     1057 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/render_err.gif
--rw-r--r--   0        0        0     6716 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/rendering.gif
--rw-r--r--   0        0        0      292 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/star_off.png
--rw-r--r--   0        0        0      297 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/star_on.png
--rw-r--r--   0        0        0     1130 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/img/unknown.gif
--rwxr-xr-x   0        0        0    74054 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/caman.full.js
--rw-r--r--   0        0        0    17360 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/hammer.min.js
--rwxr-xr-x   0        0        0    42434 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/jquery.Jcrop.js
--rw-r--r--   0        0        0      743 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/jquery.hammer.js
--rw-r--r--   0        0        0    16587 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/load-image.min.js
--rwxr-xr-x   0        0        0   111779 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/swiper.js
--rw-r--r--   0        0        0     1163 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js
--rw-r--r--   0        0        0     1163 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js
--rw-r--r--   0        0        0     5708 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js
--rw-r--r--   0        0        0     3502 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/medialib.html
--rw-r--r--   0        0        0     5876 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/__init__.py
--rw-r--r--   0        0        0      601 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/__init__.py
--rw-r--r--   0        0        0     9852 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/channel.py
--rw-r--r--   0        0        0    35929 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/discovery.py
--rw-r--r--   0        0        0     3516 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/errors.py
--rw-r--r--   0        0        0    52911 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/http.py
--rw-r--r--   0        0        0     6505 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/mimeparse.py
--rw-r--r--   0        0        0    11761 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/model.py
--rw-r--r--   0        0        0     3528 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/sample_tools.py
--rw-r--r--   0        0        0     9293 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/apiclient/schema.py
--rw-r--r--   0        0        0     1592 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/filestore.py
--rw-r--r--   0        0        0    69575 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/httplib2/__init__.py
--rw-r--r--   0        0        0    39670 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/httplib2/cacerts.txt
--rw-r--r--   0        0        0     3821 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/httplib2/iri2uri.py
--rw-r--r--   0        0        0    18452 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/httplib2/socks.py
--rw-r--r--   0        0        0      706 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/httpstore.py
--rw-r--r--   0        0        0      304 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/nullstore.py
--rw-r--r--   0        0        0      213 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/__init__.py
--rw-r--r--   0        0        0     1044 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/anyjson.py
--rw-r--r--   0        0        0    32534 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/appengine.py
--rw-r--r--   0        0        0    44346 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/client.py
--rw-r--r--   0        0        0     4425 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/clientsecrets.py
--rw-r--r--   0        0        0    10239 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/crypt.py
--rw-r--r--   0        0        0     3755 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/django_orm.py
--rw-r--r--   0        0        0     3164 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/file.py
--rw-r--r--   0        0        0     3036 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/gce.py
--rw-r--r--   0        0        0     3229 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/keyring_storage.py
--rw-r--r--   0        0        0    11393 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/locked_file.py
--rw-r--r--   0        0        0    13950 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/multistore_file.py
--rw-r--r--   0        0        0     5588 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/old_run.py
--rw-r--r--   0        0        0     8379 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/tools.py
--rw-r--r--   0        0        0     5706 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/util.py
--rw-r--r--   0        0        0     3367 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/oauth2client/xsrfutil.py
--rw-r--r--   0        0        0      500 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/rtmpstore.py
--rw-r--r--   0        0        0     4583 2023-06-23 21:15:35.146572 django_restit-4.0.2/medialib/stores/s3store.py
--rw-r--r--   0        0        0     4996 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/uritemplate/__init__.py
--rw-r--r--   0        0        0      406 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/stores/youtubestore.py
--rw-r--r--   0        0        0     3691 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/base.html
--rw-r--r--   0        0        0     1277 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/instances.html
--rw-r--r--   0        0        0     1170 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/items.html
--rw-r--r--   0        0        0     8194 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/library.html
--rw-r--r--   0        0        0       65 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_error.subject
--rw-r--r--   0        0        0       49 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_error.to
--rw-r--r--   0        0        0      272 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_error.txt
--rw-r--r--   0        0        0       71 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_ready.subject
--rw-r--r--   0        0        0       49 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_ready.to
--rw-r--r--   0        0        0      298 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_ready.txt
--rw-r--r--   0        0        0       64 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_render_error.subject
--rw-r--r--   0        0        0       48 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_render_error.to
--rw-r--r--   0        0        0      271 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_render_error.txt
--rw-r--r--   0        0        0       68 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_validate_error.subject
--rw-r--r--   0        0        0       48 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_validate_error.to
--rw-r--r--   0        0        0      275 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/notify_validate_error.txt
--rw-r--r--   0        0        0      206 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/smil
--rw-r--r--   0        0        0     1177 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/test.html
--rw-r--r--   0        0        0     1549 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/templates/medialib/testpicker.html
--rw-r--r--   0        0        0     6045 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/tests.py
--rw-r--r--   0        0        0      544 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/tq.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/urls.py
--rw-r--r--   0        0        0     3756 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/utils.py
--rw-r--r--   0        0        0     4321 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/views.py
--rw-r--r--   0        0        0     4303 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/__init__.py
--rw-r--r--   0        0        0      601 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/__init__.py
--rw-r--r--   0        0        0     9886 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/channel.py
--rw-r--r--   0        0        0    35907 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/discovery.py
--rw-r--r--   0        0        0     3550 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/errors.py
--rw-r--r--   0        0        0    52945 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/http.py
--rw-r--r--   0        0        0     6505 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/mimeparse.py
--rw-r--r--   0        0        0    11795 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/model.py
--rw-r--r--   0        0        0     3596 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/sample_tools.py
--rw-r--r--   0        0        0     9327 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/apiclient/schema.py
--rw-r--r--   0        0        0    69581 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/httplib2/__init__.py
--rw-r--r--   0        0        0    39670 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/httplib2/cacerts.txt
--rw-r--r--   0        0        0     3821 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/httplib2/iri2uri.py
--rw-r--r--   0        0        0    18452 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/httplib2/socks.py
--rw-r--r--   0        0        0      213 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/__init__.py
--rw-r--r--   0        0        0     1044 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/anyjson.py
--rw-r--r--   0        0        0    32534 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/appengine.py
--rw-r--r--   0        0        0    44431 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/client.py
--rw-r--r--   0        0        0     4425 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/clientsecrets.py
--rw-r--r--   0        0        0    10239 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/crypt.py
--rw-r--r--   0        0        0     3753 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/django_orm.py
--rw-r--r--   0        0        0     3164 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/file.py
--rw-r--r--   0        0        0     3036 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/gce.py
--rw-r--r--   0        0        0     3229 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/keyring_storage.py
--rw-r--r--   0        0        0    11393 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/locked_file.py
--rw-r--r--   0        0        0    13950 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/multistore_file.py
--rw-r--r--   0        0        0     5588 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/old_run.py
--rw-r--r--   0        0        0     8379 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/tools.py
--rw-r--r--   0        0        0     5706 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/util.py
--rw-r--r--   0        0        0     3367 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/oauth2client/xsrfutil.py
--rw-r--r--   0        0        0     2849 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/upload.py
--rw-r--r--   0        0        0     4996 2022-07-28 20:16:06.000000 django_restit-4.0.2/medialib/youtube/uritemplate/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-23 21:15:35.146800 django_restit-4.0.2/metrics/README.md
--rw-r--r--   0        0        0       90 2023-06-23 21:15:35.146848 django_restit-4.0.2/metrics/__init__.py
--rw-r--r--   0        0        0    23460 2023-06-23 21:15:35.146988 django_restit-4.0.2/metrics/client.py
--rw-r--r--   0        0        0     9182 2023-06-23 21:15:35.147084 django_restit-4.0.2/metrics/eod.py
--rw-r--r--   0        0        0     1664 2023-06-23 21:15:35.147166 django_restit-4.0.2/metrics/examples/eod_example.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.147220 django_restit-4.0.2/metrics/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.147298 django_restit-4.0.2/metrics/management/commands/__init__.py
--rw-r--r--   0        0        0      429 2023-06-23 21:15:35.147527 django_restit-4.0.2/metrics/management/commands/delete_gauge.py
--rw-r--r--   0        0        0      464 2023-06-23 21:15:35.147736 django_restit-4.0.2/metrics/management/commands/delete_metric.py
--rw-r--r--   0        0        0     2801 2023-06-23 21:15:35.147974 django_restit-4.0.2/metrics/management/commands/fix_redis_metrics_keys.py
--rw-r--r--   0        0        0     1928 2023-06-23 21:15:35.148212 django_restit-4.0.2/metrics/management/commands/generate_test_metrics.py
--rw-r--r--   0        0        0     1742 2023-06-23 21:15:35.148371 django_restit-4.0.2/metrics/management/commands/redis_metrics_send_mail.py
--rw-r--r--   0        0        0     1874 2023-06-23 21:15:35.148601 django_restit-4.0.2/metrics/management/commands/reset_weekly_metrics.py
--rw-r--r--   0        0        0     4343 2023-06-23 21:15:35.148742 django_restit-4.0.2/metrics/management/commands/system_metric.py
--rw-r--r--   0        0        0     2399 2023-06-23 21:15:35.148840 django_restit-4.0.2/metrics/migrations/0001_initial.py
--rw-r--r--   0        0        0     1510 2023-06-23 21:15:35.148905 django_restit-4.0.2/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py
--rw-r--r--   0        0        0      453 2023-06-23 21:15:35.148960 django_restit-4.0.2/metrics/migrations/0003_metrics_expires.py
--rw-r--r--   0        0        0     3271 2023-06-23 21:15:35.149017 django_restit-4.0.2/metrics/migrations/0004_eodmetrics.py
--rw-r--r--   0        0        0     2358 2023-06-24 01:15:03.076316 django_restit-4.0.2/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.149043 django_restit-4.0.2/metrics/migrations/__init__.py
--rw-r--r--   0        0        0    10599 2023-06-24 01:15:03.076758 django_restit-4.0.2/metrics/models.py
--rw-r--r--   0        0        0      480 2023-06-23 21:15:35.149225 django_restit-4.0.2/metrics/periodic.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.149281 django_restit-4.0.2/metrics/providers/__init__.py
--rw-r--r--   0        0        0     7335 2023-06-23 21:15:35.149411 django_restit-4.0.2/metrics/providers/aws.py
--rw-r--r--   0        0        0    14826 2023-06-23 21:15:35.149500 django_restit-4.0.2/metrics/rpc.py
--rw-r--r--   0        0        0      132 2023-06-23 21:15:35.149570 django_restit-4.0.2/metrics/settings.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.149594 django_restit-4.0.2/metrics/tq.py
--rw-r--r--   0        0        0    10490 2023-06-23 21:15:35.149712 django_restit-4.0.2/metrics/utils.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/pushit/__init__.py
--rw-r--r--   0        0        0      451 2022-07-28 20:16:06.000000 django_restit-4.0.2/pushit/admin.py
--rw-r--r--   0        0        0     4555 2022-07-28 20:16:06.000000 django_restit-4.0.2/pushit/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/pushit/migrations/__init__.py
--rw-r--r--   0        0        0     5076 2022-07-28 20:16:06.000000 django_restit-4.0.2/pushit/models.py
--rw-r--r--   0        0        0    12431 2023-06-23 21:15:35.150053 django_restit-4.0.2/pushit/rpc.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.150246 django_restit-4.0.2/pushit/static/js/models_pushit.js
--rw-r--r--   0        0        0     1462 2023-06-25 17:36:11.934754 django_restit-4.0.2/pyproject.toml
--rw-r--r--   0        0        0      118 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/.gitignore
--rw-r--r--   0        0        0     5460 2022-10-30 01:29:56.000000 django_restit-4.0.2/rest/README.md
--rw-r--r--   0        0        0       72 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/RemoteEvents.py
--rw-r--r--   0        0        0      120 2022-11-13 00:23:18.000000 django_restit-4.0.2/rest/__init__.py
--rw-r--r--   0        0        0     1967 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/arc4.py
--rw-r--r--   0        0        0       83 2023-06-23 21:15:35.150349 django_restit-4.0.2/rest/cache.py
--rw-r--r--   0        0        0       72 2023-06-23 21:15:35.150496 django_restit-4.0.2/rest/crypto/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-23 21:15:35.150606 django_restit-4.0.2/rest/crypto/aes.py
--rw-r--r--   0        0        0     4082 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/crypto/privpub.py
--rw-r--r--   0        0        0     3955 2022-10-28 22:27:17.000000 django_restit-4.0.2/rest/crypto/util.py
--rw-r--r--   0        0        0     7784 2023-06-23 21:15:35.150736 django_restit-4.0.2/rest/datem.py
--rw-r--r--   0        0        0    15213 2023-06-23 21:15:35.150865 django_restit-4.0.2/rest/decorators.py
--rw-r--r--   0        0        0      788 2023-06-23 21:15:35.150965 django_restit-4.0.2/rest/encryption.py
--rw-r--r--   0        0        0       54 2023-06-23 21:15:35.151052 django_restit-4.0.2/rest/extra/__init__.py
--rw-r--r--   0        0        0     1078 2023-06-23 21:15:35.151114 django_restit-4.0.2/rest/extra/json_metadata.py
--rw-r--r--   0        0        0     9719 2023-06-23 21:15:35.151226 django_restit-4.0.2/rest/fields.py
--rw-r--r--   0        0        0     6316 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/forms.py
--rw-r--r--   0        0        0    23837 2023-06-23 21:15:35.151406 django_restit-4.0.2/rest/helpers.py
--rw-r--r--   0        0        0      260 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/joke.py
--rw-r--r--   0        0        0     2298 2023-06-23 21:15:35.151515 django_restit-4.0.2/rest/jwtoken.py
--rw-r--r--   0        0        0    21139 2023-06-23 21:15:35.151666 django_restit-4.0.2/rest/log.py
--rw-r--r--   0        0        0     7754 2023-06-23 21:15:35.151788 django_restit-4.0.2/rest/mail.py
--rw-r--r--   0        0        0     9174 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/mailman.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/management/__init__.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/management/commands/__init__.py
--rw-r--r--   0        0        0      389 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/management/commands/rpc.py
--rw-r--r--   0        0        0       33 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/middleware/__init__.py
--rw-r--r--   0        0        0     3513 2022-07-30 23:06:28.000000 django_restit-4.0.2/rest/middleware/cors.py
--rw-r--r--   0        0        0     2345 2023-06-23 21:15:35.151948 django_restit-4.0.2/rest/middleware/db_router.py
--rw-r--r--   0        0        0     5395 2023-06-23 21:15:35.152061 django_restit-4.0.2/rest/middleware/jwt.py
--rw-r--r--   0        0        0     4127 2023-06-23 21:15:35.152179 django_restit-4.0.2/rest/middleware/request.py
--rw-r--r--   0        0        0     9015 2023-06-23 21:15:35.152293 django_restit-4.0.2/rest/middleware/session.py
--rw-r--r--   0        0        0     1874 2023-06-23 21:15:35.152353 django_restit-4.0.2/rest/middleware/session_store.py
--rw-r--r--   0        0        0    76845 2023-06-23 21:15:35.152636 django_restit-4.0.2/rest/models.py
--rw-r--r--   0        0        0   149463 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/regexes.yaml
--rw-r--r--   0        0        0    14894 2023-06-23 21:15:35.152738 django_restit-4.0.2/rest/requestex.py
--rw-r--r--   0        0        0     3480 2022-09-29 05:47:59.000000 django_restit-4.0.2/rest/rpc.py
--rw-r--r--   0        0        0     7645 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/search.py
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.152794 django_restit-4.0.2/rest/serializers/__init__.py
--rw-r--r--   0        0        0     1644 2023-06-23 21:15:35.152880 django_restit-4.0.2/rest/serializers/collection.py
--rw-r--r--   0        0        0     2975 2023-06-23 21:15:35.152935 django_restit-4.0.2/rest/serializers/csv.py
--rw-r--r--   0        0        0     1077 2023-06-23 21:15:35.152983 django_restit-4.0.2/rest/serializers/excel.py
--rw-r--r--   0        0        0     1736 2023-06-23 21:15:35.153036 django_restit-4.0.2/rest/serializers/json.py
--rw-r--r--   0        0        0    61738 2023-06-23 21:15:35.153260 django_restit-4.0.2/rest/serializers/legacy.py
--rw-r--r--   0        0        0     4943 2023-06-25 17:36:11.924423 django_restit-4.0.2/rest/serializers/model.py
--rw-r--r--   0        0        0     6162 2023-06-23 21:15:35.153411 django_restit-4.0.2/rest/serializers/response.py
--rw-r--r--   0        0        0     2734 2023-06-23 21:15:35.153507 django_restit-4.0.2/rest/serializers/util.py
--rw-r--r--   0        0        0     1532 2023-06-23 21:15:35.153605 django_restit-4.0.2/rest/settings_helper.py
--rw-r--r--   0        0        0    95786 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/static/lib/jquery.js
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.153689 django_restit-4.0.2/rest/static/rest/app.css
--rw-r--r--   0        0        0        0 2023-06-23 21:15:35.153786 django_restit-4.0.2/rest/static/rest/app.js
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/static/rest/rest.js
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/static/rest/rest.scss
--rw-r--r--   0        0        0      529 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/templates/email/error.html
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/templates/email/error.subject
--rw-r--r--   0        0        0     7148 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/templates/rest_docs.html
--rw-r--r--   0        0        0    10880 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/templates/rest_html.html
--rw-r--r--   0        0        0   185122 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/ua.py
--rw-r--r--   0        0        0    17064 2023-06-23 21:15:35.153956 django_restit-4.0.2/rest/uberdict.py
--rw-r--r--   0        0        0    11881 2022-07-28 20:16:06.000000 django_restit-4.0.2/rest/url_docs.py
--rw-r--r--   0        0        0     1713 2023-06-23 21:15:35.154058 django_restit-4.0.2/rest/urls.py
--rw-r--r--   0        0        0     1056 2023-06-23 21:15:35.154155 django_restit-4.0.2/rest/views.py
--rw-r--r--   0        0        0      118 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/.gitignore
--rw-r--r--   0        0        0       62 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/README.md
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/__init__.py
--rw-r--r--   0        0        0      245 2023-06-23 21:15:35.154256 django_restit-4.0.2/sessionlog/admin.py
--rw-r--r--   0        0        0     1694 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/migrations/__init__.py
--rw-r--r--   0        0        0     3922 2023-06-23 21:15:35.154359 django_restit-4.0.2/sessionlog/models.py
--rw-r--r--   0        0        0      383 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/tests.py
--rw-r--r--   0        0        0       26 2022-07-28 20:16:06.000000 django_restit-4.0.2/sessionlog/views.py
--rw-r--r--   0        0        0     2196 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/README.md
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/__init__.py
--rw-r--r--   0        0        0      208 2023-06-23 21:15:35.154426 django_restit-4.0.2/taskqueue/admin.py
--rw-r--r--   0        0        0     4738 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/migrations/__init__.py
--rw-r--r--   0        0        0    16531 2023-06-23 21:15:35.154590 django_restit-4.0.2/taskqueue/models.py
--rw-r--r--   0        0        0     3072 2023-06-23 21:15:35.154789 django_restit-4.0.2/taskqueue/periodic.py
--rw-r--r--   0        0        0     5326 2023-06-23 21:15:35.154903 django_restit-4.0.2/taskqueue/rpc.py
--rw-r--r--   0        0        0      942 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/tq.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/transports/__init__.py
--rw-r--r--   0        0        0      623 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/transports/email.py
--rw-r--r--   0        0        0     2409 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/transports/http.py
--rw-r--r--   0        0        0     1099 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/transports/s3.py
--rw-r--r--   0        0        0     1891 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/transports/sftp.py
--rw-r--r--   0        0        0      142 2022-07-28 20:16:06.000000 django_restit-4.0.2/taskqueue/transports/sms.py
--rw-r--r--   0        0        0    13660 2023-06-23 21:15:35.155056 django_restit-4.0.2/taskqueue/worker.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/telephony/__init__.py
--rw-r--r--   0        0        0      243 2023-06-23 21:15:35.155115 django_restit-4.0.2/telephony/admin.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/telephony/decorators.py
--rw-r--r--   0        0        0     3030 2022-07-28 20:16:06.000000 django_restit-4.0.2/telephony/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/telephony/migrations/__init__.py
--rw-r--r--   0        0        0     7753 2022-07-28 20:16:06.000000 django_restit-4.0.2/telephony/models.py
--rw-r--r--   0        0        0     2126 2022-07-28 20:16:06.000000 django_restit-4.0.2/telephony/phone_util.py
--rw-r--r--   0        0        0     2659 2022-11-04 18:26:58.000000 django_restit-4.0.2/telephony/rpc.py
--rw-r--r--   0        0        0     3624 2023-06-23 21:15:35.155183 django_restit-4.0.2/ws4redis/README.md
--rwxr-xr-x   0        0        0       46 2022-07-28 20:16:06.000000 django_restit-4.0.2/ws4redis/__init__.py
--rw-r--r--   0        0        0     4942 2023-06-23 21:15:35.155467 django_restit-4.0.2/ws4redis/client.py
--rw-r--r--   0        0        0    13026 2023-06-23 21:15:35.155574 django_restit-4.0.2/ws4redis/connection.py
--rwxr-xr-x   0        0        0      636 2022-07-28 20:16:06.000000 django_restit-4.0.2/ws4redis/exceptions.py
--rw-r--r--   0        0        0     5548 2023-06-23 21:15:35.155756 django_restit-4.0.2/ws4redis/redis.py
--rw-r--r--   0        0        0        0 2022-07-28 20:16:06.000000 django_restit-4.0.2/ws4redis/servers/__init__.py
--rw-r--r--   0        0        0     3747 2023-06-23 21:15:35.155987 django_restit-4.0.2/ws4redis/servers/base.py
--rw-r--r--   0        0        0     4329 2022-07-28 20:16:06.000000 django_restit-4.0.2/ws4redis/servers/django.py
--rw-r--r--   0        0        0     1723 2022-07-28 20:16:06.000000 django_restit-4.0.2/ws4redis/servers/uwsgi.py
--rwxr-xr-x   0        0        0     1411 2023-06-23 21:15:35.156079 django_restit-4.0.2/ws4redis/settings.py
--rwxr-xr-x   0        0        0     5122 2022-07-28 20:16:06.000000 django_restit-4.0.2/ws4redis/utf8validator.py
--rwxr-xr-x   0        0        0    14848 2023-06-23 21:15:35.156205 django_restit-4.0.2/ws4redis/websocket.py
--rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 django_restit-4.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-27 05:37:44.430230 django_restit-4.0.4/LICENSE.md
+-rw-r--r--   0        0        0     6234 2023-06-27 05:37:44.430353 django_restit-4.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.430501 django_restit-4.0.4/account/__init__.py
+-rw-r--r--   0        0        0     1839 2023-06-27 05:37:44.430617 django_restit-4.0.4/account/admin.py
+-rw-r--r--   0        0        0      980 2023-06-27 05:37:44.430754 django_restit-4.0.4/account/fcm/__init__.py
+-rw-r--r--   0        0        0    15894 2023-06-27 05:37:44.430954 django_restit-4.0.4/account/migrations/0001_initial.py
+-rw-r--r--   0        0        0      738 2023-06-27 05:37:44.431054 django_restit-4.0.4/account/migrations/0003_member_phone_number.py
+-rw-r--r--   0        0        0      551 2023-06-27 05:37:44.431131 django_restit-4.0.4/account/migrations/0004_group_modified_alter_group_created.py
+-rw-r--r--   0        0        0      437 2023-06-27 05:37:44.431211 django_restit-4.0.4/account/migrations/0005_member_auth_code_expires.py
+-rw-r--r--   0        0        0      450 2023-06-27 05:37:44.431293 django_restit-4.0.4/account/migrations/0006_member_security_token.py
+-rw-r--r--   0        0        0     1654 2023-06-27 05:37:44.431375 django_restit-4.0.4/account/migrations/0007_authtoken_signature_authsession.py
+-rw-r--r--   0        0        0     2379 2023-06-27 05:37:44.431464 django_restit-4.0.4/account/migrations/0008_memberdevice_memberdevicemetadata.py
+-rw-r--r--   0        0        0      468 2023-06-27 05:37:44.431538 django_restit-4.0.4/account/migrations/0009_alter_member_phone_number.py
+-rw-r--r--   0        0        0      305 2023-06-27 05:37:44.431613 django_restit-4.0.4/account/migrations/0010_delete_authtoken.py
+-rw-r--r--   0        0        0     1062 2023-06-27 05:37:44.431685 django_restit-4.0.4/account/migrations/0011_authtoken.py
+-rw-r--r--   0        0        0     2043 2023-06-27 05:37:44.431755 django_restit-4.0.4/account/migrations/0012_settings_settingsmetadata.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.431784 django_restit-4.0.4/account/migrations/__init__.py
+-rw-r--r--   0        0        0      341 2023-06-27 05:37:44.431899 django_restit-4.0.4/account/models/__init__.py
+-rw-r--r--   0        0        0     3070 2023-06-27 05:37:44.431980 django_restit-4.0.4/account/models/device.py
+-rw-r--r--   0        0        0     1437 2023-06-27 05:37:44.432051 django_restit-4.0.4/account/models/feeds.py
+-rw-r--r--   0        0        0    18161 2023-06-27 05:37:44.432210 django_restit-4.0.4/account/models/group.py
+-rw-r--r--   0        0        0     2720 2023-06-27 05:37:44.432315 django_restit-4.0.4/account/models/legacy.py
+-rw-r--r--   0        0        0    45805 2023-06-27 05:37:44.432566 django_restit-4.0.4/account/models/member.py
+-rw-r--r--   0        0        0     6842 2023-06-27 05:37:44.432689 django_restit-4.0.4/account/models/membership.py
+-rw-r--r--   0        0        0    10739 2023-06-27 05:37:44.432797 django_restit-4.0.4/account/models/notify.py
+-rw-r--r--   0        0        0     3345 2023-06-27 05:37:44.432886 django_restit-4.0.4/account/models/session.py
+-rw-r--r--   0        0        0     2137 2023-06-27 05:37:44.432966 django_restit-4.0.4/account/models/settings.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.433042 django_restit-4.0.4/account/oauth/__init__.py
+-rw-r--r--   0        0        0     2078 2023-06-27 05:37:44.433131 django_restit-4.0.4/account/oauth/google.py
+-rw-r--r--   0        0        0      578 2023-06-27 05:37:44.433195 django_restit-4.0.4/account/periodic.py
+-rw-r--r--   0        0        0      152 2023-06-27 05:37:44.433297 django_restit-4.0.4/account/rpc/__init__.py
+-rw-r--r--   0        0        0    12428 2023-06-27 05:37:44.433416 django_restit-4.0.4/account/rpc/auth.py
+-rw-r--r--   0        0        0     2104 2023-06-27 05:37:44.433497 django_restit-4.0.4/account/rpc/device.py
+-rw-r--r--   0        0        0     3078 2023-06-27 05:37:44.433585 django_restit-4.0.4/account/rpc/group.py
+-rw-r--r--   0        0        0     1150 2023-06-27 05:37:44.433650 django_restit-4.0.4/account/rpc/member.py
+-rw-r--r--   0        0        0     3344 2023-06-27 05:37:44.433726 django_restit-4.0.4/account/rpc/notify.py
+-rw-r--r--   0        0        0     2610 2023-06-27 05:37:44.433805 django_restit-4.0.4/account/rpc/oauth.py
+-rw-r--r--   0        0        0      271 2023-06-27 05:37:44.433874 django_restit-4.0.4/account/rpc/settings.py
+-rw-r--r--   0        0        0       53 2023-06-27 05:37:44.433934 django_restit-4.0.4/account/settings.py
+-rw-r--r--   0        0        0     9709 2023-06-27 05:37:44.434095 django_restit-4.0.4/account/templates/email/base.html
+-rw-r--r--   0        0        0    10567 2023-06-27 05:37:44.434205 django_restit-4.0.4/account/templates/email/invite.html
+-rw-r--r--   0        0        0    15185 2023-06-27 05:37:44.434344 django_restit-4.0.4/account/templates/email/plain/invite.html
+-rw-r--r--   0        0        0    13954 2023-06-27 05:37:44.434450 django_restit-4.0.4/account/templates/email/plain/reset_code.html
+-rw-r--r--   0        0        0    10261 2023-06-27 05:37:44.434528 django_restit-4.0.4/account/templates/email/reset_code.html
+-rw-r--r--   0        0        0    15163 2023-06-27 05:37:44.434627 django_restit-4.0.4/account/templates/email/simple/invite.html
+-rw-r--r--   0        0        0    13944 2023-06-27 05:37:44.434713 django_restit-4.0.4/account/templates/email/simple/reset_code.html
+-rw-r--r--   0        0        0      520 2023-06-27 05:37:44.434828 django_restit-4.0.4/auditlog/README
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.434859 django_restit-4.0.4/auditlog/__init__.py
+-rw-r--r--   0        0        0     1006 2023-06-27 05:37:44.434933 django_restit-4.0.4/auditlog/admin.py
+-rw-r--r--   0        0        0     6553 2023-06-27 05:37:44.435019 django_restit-4.0.4/auditlog/decorators.py
+-rw-r--r--   0        0        0     1329 2023-06-27 05:37:44.435081 django_restit-4.0.4/auditlog/middleware.py
+-rw-r--r--   0        0        0     3309 2023-06-27 05:37:44.435191 django_restit-4.0.4/auditlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435224 django_restit-4.0.4/auditlog/migrations/__init__.py
+-rw-r--r--   0        0        0    16043 2023-06-27 05:37:44.435348 django_restit-4.0.4/auditlog/models.py
+-rw-r--r--   0        0        0      264 2023-06-27 05:37:44.435414 django_restit-4.0.4/auditlog/periodic.py
+-rw-r--r--   0        0        0     3591 2023-06-27 05:37:44.435492 django_restit-4.0.4/auditlog/rpc.py
+-rw-r--r--   0        0        0     2019 2023-06-27 05:37:44.435560 django_restit-4.0.4/auditlog/tq.py
+-rw-r--r--   0        0        0      163 2023-06-27 05:37:44.435623 django_restit-4.0.4/auditlog/urls.py
+-rw-r--r--   0        0        0     2169 2023-06-27 05:37:44.435745 django_restit-4.0.4/inbox/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435775 django_restit-4.0.4/inbox/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-27 05:37:44.435850 django_restit-4.0.4/inbox/admin.py
+-rw-r--r--   0        0        0     5621 2023-06-27 05:37:44.435936 django_restit-4.0.4/inbox/handlers.py
+-rw-r--r--   0        0        0     6429 2023-06-27 05:37:44.436034 django_restit-4.0.4/inbox/migrations/0001_initial.py
+-rw-r--r--   0        0        0      380 2023-06-27 05:37:44.436102 django_restit-4.0.4/inbox/migrations/0002_alter_message_cc.py
+-rw-r--r--   0        0        0      416 2023-06-27 05:37:44.436177 django_restit-4.0.4/inbox/migrations/0003_attachment_content_type.py
+-rw-r--r--   0        0        0     1140 2023-06-27 05:37:44.436249 django_restit-4.0.4/inbox/migrations/0004_mailtemplate.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.436274 django_restit-4.0.4/inbox/migrations/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-27 05:37:44.436383 django_restit-4.0.4/inbox/models/__init__.py
+-rw-r--r--   0        0        0     2832 2023-06-27 05:37:44.436463 django_restit-4.0.4/inbox/models/bounce.py
+-rw-r--r--   0        0        0     2468 2023-06-27 05:37:44.436568 django_restit-4.0.4/inbox/models/complaint.py
+-rw-r--r--   0        0        0     2879 2023-06-27 05:37:44.436797 django_restit-4.0.4/inbox/models/message.py
+-rw-r--r--   0        0        0     1013 2023-06-27 05:37:44.436870 django_restit-4.0.4/inbox/models/template.py
+-rw-r--r--   0        0        0     1534 2023-06-27 05:37:44.436956 django_restit-4.0.4/inbox/rpc.py
+-rw-r--r--   0        0        0       89 2023-06-27 05:37:44.437057 django_restit-4.0.4/inbox/utils/__init__.py
+-rw-r--r--   0        0        0     4366 2023-06-27 05:37:44.437161 django_restit-4.0.4/inbox/utils/parsing.py
+-rw-r--r--   0        0        0     4098 2023-06-27 05:37:44.437260 django_restit-4.0.4/inbox/utils/render.py
+-rw-r--r--   0        0        0     2109 2023-06-27 05:37:44.437361 django_restit-4.0.4/inbox/utils/sending.py
+-rw-r--r--   0        0        0     1114 2023-06-27 05:37:44.437469 django_restit-4.0.4/incident/README.md
+-rw-r--r--   0        0        0      988 2023-06-27 05:37:44.437542 django_restit-4.0.4/incident/__init__.py
+-rw-r--r--   0        0        0     9720 2023-06-27 05:37:44.437670 django_restit-4.0.4/incident/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2023-06-27 05:37:44.437757 django_restit-4.0.4/incident/migrations/0002_event_component_event_component_id.py
+-rw-r--r--   0        0        0      425 2023-06-27 05:37:44.437826 django_restit-4.0.4/incident/migrations/0003_rule_action.py
+-rw-r--r--   0        0        0      662 2023-06-27 05:37:44.437890 django_restit-4.0.4/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py
+-rw-r--r--   0        0        0      698 2023-06-27 05:37:44.437964 django_restit-4.0.4/incident/migrations/0005_incident_component_alter_incident_state.py
+-rw-r--r--   0        0        0      324 2023-06-27 05:37:44.438034 django_restit-4.0.4/incident/migrations/0006_delete_eventmetadata.py
+-rw-r--r--   0        0        0      414 2023-06-27 05:37:44.438100 django_restit-4.0.4/incident/migrations/0007_event_metadata.py
+-rw-r--r--   0        0        0      903 2023-06-27 05:37:44.438184 django_restit-4.0.4/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438214 django_restit-4.0.4/incident/migrations/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-27 05:37:44.438331 django_restit-4.0.4/incident/models/__init__.py
+-rw-r--r--   0        0        0     4976 2023-06-27 05:37:44.438427 django_restit-4.0.4/incident/models/event.py
+-rw-r--r--   0        0        0    10022 2023-06-27 05:37:44.438560 django_restit-4.0.4/incident/models/incident.py
+-rw-r--r--   0        0        0     2187 2023-06-27 05:37:44.438718 django_restit-4.0.4/incident/models/ossec.py
+-rw-r--r--   0        0        0     5300 2023-06-27 05:37:44.438826 django_restit-4.0.4/incident/models/rules.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438911 django_restit-4.0.4/incident/parsers/__init__.py
+-rw-r--r--   0        0        0     5289 2023-06-27 05:37:44.439057 django_restit-4.0.4/incident/parsers/ossec.py
+-rw-r--r--   0        0        0      723 2023-06-27 05:37:44.439158 django_restit-4.0.4/incident/periodic.py
+-rw-r--r--   0        0        0     2831 2023-06-27 05:37:44.439252 django_restit-4.0.4/incident/rpc.py
+-rw-r--r--   0        0        0    12732 2023-06-27 05:37:44.439416 django_restit-4.0.4/incident/templates/email/incident_change.html
+-rw-r--r--   0        0        0    15173 2023-06-27 05:37:44.439515 django_restit-4.0.4/incident/templates/email/incident_new.html
+-rw-r--r--   0        0        0    13208 2023-06-27 05:37:44.439626 django_restit-4.0.4/incident/templates/email/incident_plain.html
+-rw-r--r--   0        0        0      796 2023-06-27 05:37:44.439700 django_restit-4.0.4/incident/tq.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.439791 django_restit-4.0.4/location/__init__.py
+-rw-r--r--   0        0        0      297 2023-06-27 05:37:44.439885 django_restit-4.0.4/location/admin.py
+-rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.440042 django_restit-4.0.4/location/geolocate.py
+-rw-r--r--   0        0        0     7000 2023-06-27 05:37:44.440236 django_restit-4.0.4/location/migrations/0001_initial.py
+-rw-r--r--   0        0        0      576 2023-06-27 05:37:44.440313 django_restit-4.0.4/location/migrations/0002_geoip_subnet_alter_geoip_ip.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440339 django_restit-4.0.4/location/migrations/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-27 05:37:44.440480 django_restit-4.0.4/location/models/__init__.py
+-rw-r--r--   0        0        0     2028 2023-06-27 05:37:44.440559 django_restit-4.0.4/location/models/address.py
+-rw-r--r--   0        0        0     3500 2023-06-27 05:37:44.440656 django_restit-4.0.4/location/models/ip.py
+-rw-r--r--   0        0        0     1994 2023-06-27 05:37:44.440722 django_restit-4.0.4/location/models/legacy.py
+-rw-r--r--   0        0        0     2316 2023-06-27 05:37:44.440785 django_restit-4.0.4/location/models/location.py
+-rw-r--r--   0        0        0     1474 2023-06-27 05:37:44.440843 django_restit-4.0.4/location/models/track.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440920 django_restit-4.0.4/location/providers/__init__.py
+-rw-r--r--   0        0        0      730 2023-06-27 05:37:44.441046 django_restit-4.0.4/location/providers/iplookup/__init__.py
+-rw-r--r--   0        0        0     2419 2023-06-27 05:37:44.441128 django_restit-4.0.4/location/providers/iplookup/abstractapi.py
+-rw-r--r--   0        0        0     1345 2023-06-27 05:37:44.441192 django_restit-4.0.4/location/providers/iplookup/extremeip.py
+-rw-r--r--   0        0        0     2121 2023-06-27 05:37:44.441260 django_restit-4.0.4/location/providers/iplookup/geoplugin.py
+-rw-r--r--   0        0        0     1797 2023-06-27 05:37:44.441325 django_restit-4.0.4/location/providers/iplookup/ipapi.py
+-rw-r--r--   0        0        0     1265 2023-06-27 05:37:44.441395 django_restit-4.0.4/location/providers/iplookup/ipinfo.py
+-rw-r--r--   0        0        0      937 2023-06-27 05:37:44.441463 django_restit-4.0.4/location/providers/iplookup/restit.py
+-rw-r--r--   0        0        0       42 2023-06-27 05:37:44.441569 django_restit-4.0.4/location/providers/location/__init__.py
+-rw-r--r--   0        0        0     2860 2023-06-27 05:37:44.441653 django_restit-4.0.4/location/providers/location/google.py
+-rw-r--r--   0        0        0       46 2023-06-27 05:37:44.441777 django_restit-4.0.4/location/providers/timezones/__init__.py
+-rw-r--r--   0        0        0      619 2023-06-27 05:37:44.441855 django_restit-4.0.4/location/providers/timezones/google.py
+-rw-r--r--   0        0        0     1935 2023-06-27 05:37:44.441924 django_restit-4.0.4/location/providers/zillow.py
+-rw-r--r--   0        0        0      123 2023-06-27 05:37:44.442046 django_restit-4.0.4/location/rpc/__init__.py
+-rw-r--r--   0        0        0      782 2023-06-27 05:37:44.442126 django_restit-4.0.4/location/rpc/ip.py
+-rw-r--r--   0        0        0      779 2023-06-27 05:37:44.442183 django_restit-4.0.4/location/rpc/location.py
+-rw-r--r--   0        0        0     3735 2023-06-27 05:37:44.442254 django_restit-4.0.4/location/rpc/track.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.442312 django_restit-4.0.4/medialib/__init__.py
+-rw-r--r--   0        0        0     2261 2023-06-27 05:37:44.442393 django_restit-4.0.4/medialib/admin.py
+-rw-r--r--   0        0        0       27 2023-06-27 05:37:44.442482 django_restit-4.0.4/medialib/cvutil/__init__.py
+-rw-r--r--   0        0        0     4269 2023-06-27 05:37:44.442556 django_restit-4.0.4/medialib/cvutil/contours.py
+-rw-r--r--   0        0        0    12649 2023-06-27 05:37:44.442653 django_restit-4.0.4/medialib/cvutil/images.py
+-rw-r--r--   0        0        0     9586 2023-06-27 05:37:44.442744 django_restit-4.0.4/medialib/cvutil/misc.py
+-rw-r--r--   0        0        0     5824 2023-06-27 05:37:44.442838 django_restit-4.0.4/medialib/cvutil/text.py
+-rw-r--r--   0        0        0    48442 2023-06-27 05:37:44.443047 django_restit-4.0.4/medialib/fixtures/initial_data.json
+-rw-r--r--   0        0        0    31978 2023-06-27 05:37:44.443182 django_restit-4.0.4/medialib/fixtures/medialib.json
+-rw-r--r--   0        0        0    16989 2023-06-27 05:37:44.443279 django_restit-4.0.4/medialib/fixtures/medialib_test_fixture.json
+-rw-r--r--   0        0        0     5442 2023-06-27 05:37:44.443362 django_restit-4.0.4/medialib/forms.py
+-rw-r--r--   0        0        0    20518 2023-06-27 05:37:44.443459 django_restit-4.0.4/medialib/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.443499 django_restit-4.0.4/medialib/migrations/__init__.py
+-rw-r--r--   0        0        0    52121 2023-06-27 05:37:44.443702 django_restit-4.0.4/medialib/models.py
+-rw-r--r--   0        0        0     1189 2023-06-27 05:37:44.443785 django_restit-4.0.4/medialib/ocr.py
+-rw-r--r--   0        0        0     1275 2023-06-27 05:37:44.443858 django_restit-4.0.4/medialib/pdf.py
+-rw-r--r--   0        0        0      545 2023-06-27 05:37:44.443925 django_restit-4.0.4/medialib/qrcode.py
+-rw-r--r--   0        0        0    10312 2023-06-27 05:37:44.444059 django_restit-4.0.4/medialib/render/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444125 django_restit-4.0.4/medialib/render/engines/__init__.py
+-rw-r--r--   0        0        0     3531 2023-06-27 05:37:44.444213 django_restit-4.0.4/medialib/render/engines/anigif.py
+-rw-r--r--   0        0        0     6881 2023-06-27 05:37:44.444291 django_restit-4.0.4/medialib/render/engines/ffmpeg.py
+-rw-r--r--   0        0        0      792 2023-06-27 05:37:44.444369 django_restit-4.0.4/medialib/render/engines/gifsicle.py
+-rw-r--r--   0        0        0     3436 2023-06-27 05:37:44.444438 django_restit-4.0.4/medialib/render/engines/hls.py
+-rw-r--r--   0        0        0      983 2023-06-27 05:37:44.444498 django_restit-4.0.4/medialib/render/engines/mp4box.py
+-rw-r--r--   0        0        0      397 2023-06-27 05:37:44.444604 django_restit-4.0.4/medialib/render/engines/rtmp/Makefile
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444636 django_restit-4.0.4/medialib/render/engines/rtmp/__init__.py
+-rw-r--r--   0        0        0     4026 2023-06-27 05:37:44.444726 django_restit-4.0.4/medialib/render/engines/rtmp/rtmp.i
+-rw-r--r--   0        0        0      699 2023-06-27 05:37:44.444798 django_restit-4.0.4/medialib/render/engines/rtmpdump.py
+-rw-r--r--   0        0        0     1017 2023-06-27 05:37:44.444865 django_restit-4.0.4/medialib/render/engines/rtmpsink.py
+-rw-r--r--   0        0        0     3466 2023-06-27 05:37:44.444941 django_restit-4.0.4/medialib/render/engines/video_getinfo.py
+-rw-r--r--   0        0        0      809 2023-06-27 05:37:44.445017 django_restit-4.0.4/medialib/render/engines/websnap.py
+-rw-r--r--   0        0        0     2193 2023-06-27 05:37:44.445078 django_restit-4.0.4/medialib/render/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.445133 django_restit-4.0.4/medialib/render/presets/__init__.py
+-rw-r--r--   0        0        0     4179 2023-06-27 05:37:44.445227 django_restit-4.0.4/medialib/render/presets/akamai.py
+-rw-r--r--   0        0        0     3284 2023-06-27 05:37:44.445306 django_restit-4.0.4/medialib/render/presets/animated_thumbnail.py
+-rw-r--r--   0        0        0     4004 2023-06-27 05:37:44.445394 django_restit-4.0.4/medialib/render/presets/ffmpeg.py
+-rw-r--r--   0        0        0     2087 2023-06-27 05:37:44.445469 django_restit-4.0.4/medialib/render/presets/flv.py
+-rw-r--r--   0        0        0     6567 2023-06-27 05:37:44.445567 django_restit-4.0.4/medialib/render/presets/hls.py
+-rw-r--r--   0        0        0     6955 2023-06-27 05:37:44.445668 django_restit-4.0.4/medialib/render/presets/image_transcode.py
+-rw-r--r--   0        0        0     1094 2023-06-27 05:37:44.445750 django_restit-4.0.4/medialib/render/presets/image_validate.py
+-rw-r--r--   0        0        0     2423 2023-06-27 05:37:44.445825 django_restit-4.0.4/medialib/render/presets/mp4.py
+-rw-r--r--   0        0        0     4997 2023-06-27 05:37:44.445908 django_restit-4.0.4/medialib/render/presets/video_still.py
+-rw-r--r--   0        0        0     3228 2023-06-27 05:37:44.445986 django_restit-4.0.4/medialib/render/presets/video_validate.py
+-rw-r--r--   0        0        0      863 2023-06-27 05:37:44.446101 django_restit-4.0.4/medialib/render/presets/websnap.py
+-rw-r--r--   0        0        0     2282 2023-06-27 05:37:44.446183 django_restit-4.0.4/medialib/render/presets/youtube.py
+-rw-r--r--   0        0        0    16451 2023-06-27 05:37:44.446294 django_restit-4.0.4/medialib/render/render_utils.py
+-rw-r--r--   0        0        0      370 2023-06-27 05:37:44.446381 django_restit-4.0.4/medialib/render/schedule.py
+-rw-r--r--   0        0        0       82 2023-06-27 05:37:44.446525 django_restit-4.0.4/medialib/rpc/__init__.py
+-rw-r--r--   0        0        0    37925 2023-06-27 05:37:44.446687 django_restit-4.0.4/medialib/rpc/legacy.py
+-rw-r--r--   0        0        0      617 2023-06-27 05:37:44.446776 django_restit-4.0.4/medialib/rpc/media.py
+-rw-r--r--   0        0        0      956 2023-06-27 05:37:44.446852 django_restit-4.0.4/medialib/rpc/tools.py
+-rwxr-xr-x   0        0        0     7875 2023-06-27 05:37:44.446994 django_restit-4.0.4/medialib/scripts/init_config
+-rw-r--r--   0        0        0     4499 2023-06-27 05:37:44.447158 django_restit-4.0.4/medialib/static/css/base_medialibui.css
+-rw-r--r--   0        0        0     3128 2023-06-27 05:37:44.447238 django_restit-4.0.4/medialib/static/css/base_widgets.css
+-rw-r--r--   0        0        0     3263 2023-06-27 05:37:44.447311 django_restit-4.0.4/medialib/static/css/jquery.jcrop.css
+-rw-r--r--   0        0        0      193 2023-06-27 05:37:44.447412 django_restit-4.0.4/medialib/static/img/arrow-down-white.png
+-rw-r--r--   0        0        0     4589 2023-06-27 05:37:44.447507 django_restit-4.0.4/medialib/static/img/bg-body.gif
+-rw-r--r--   0        0        0      441 2023-06-27 05:37:44.447579 django_restit-4.0.4/medialib/static/img/cancel.gif
+-rw-r--r--   0        0        0      341 2023-06-27 05:37:44.447648 django_restit-4.0.4/medialib/static/img/icon-generic.gif
+-rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447712 django_restit-4.0.4/medialib/static/img/icon-image.gif
+-rw-r--r--   0        0        0      359 2023-06-27 05:37:44.447775 django_restit-4.0.4/medialib/static/img/icon-media.gif
+-rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447850 django_restit-4.0.4/medialib/static/img/icon-zip.gif
+-rw-r--r--   0        0        0     3208 2023-06-27 05:37:44.447934 django_restit-4.0.4/medialib/static/img/loading.gif
+-rw-r--r--   0        0        0     2537 2023-06-27 05:37:44.448000 django_restit-4.0.4/medialib/static/img/noimage.gif
+-rw-r--r--   0        0        0     1057 2023-06-27 05:37:44.448065 django_restit-4.0.4/medialib/static/img/render_err.gif
+-rw-r--r--   0        0        0     6716 2023-06-27 05:37:44.448158 django_restit-4.0.4/medialib/static/img/rendering.gif
+-rw-r--r--   0        0        0      292 2023-06-27 05:37:44.448225 django_restit-4.0.4/medialib/static/img/star_off.png
+-rw-r--r--   0        0        0      297 2023-06-27 05:37:44.448287 django_restit-4.0.4/medialib/static/img/star_on.png
+-rw-r--r--   0        0        0     1130 2023-06-27 05:37:44.448351 django_restit-4.0.4/medialib/static/img/unknown.gif
+-rwxr-xr-x   0        0        0    74054 2023-06-27 05:37:44.448677 django_restit-4.0.4/medialib/static/lib/caman.full.js
+-rw-r--r--   0        0        0    17360 2023-06-27 05:37:44.448823 django_restit-4.0.4/medialib/static/lib/hammer.min.js
+-rwxr-xr-x   0        0        0    42434 2023-06-27 05:37:44.449017 django_restit-4.0.4/medialib/static/lib/jquery.Jcrop.js
+-rw-r--r--   0        0        0      743 2023-06-27 05:37:44.449098 django_restit-4.0.4/medialib/static/lib/jquery.hammer.js
+-rw-r--r--   0        0        0    16587 2023-06-27 05:37:44.449224 django_restit-4.0.4/medialib/static/lib/load-image.min.js
+-rwxr-xr-x   0        0        0   111779 2023-06-27 05:37:44.449542 django_restit-4.0.4/medialib/static/lib/swiper.js
+-rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449771 django_restit-4.0.4/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js
+-rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449850 django_restit-4.0.4/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js
+-rw-r--r--   0        0        0     5708 2023-06-27 05:37:44.449979 django_restit-4.0.4/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js
+-rw-r--r--   0        0        0     3502 2023-06-27 05:37:44.450059 django_restit-4.0.4/medialib/static/lib/tinymce/plugins/medialib/medialib.html
+-rw-r--r--   0        0        0     5876 2023-06-27 05:37:44.450187 django_restit-4.0.4/medialib/stores/__init__.py
+-rw-r--r--   0        0        0      601 2023-06-27 05:37:44.450314 django_restit-4.0.4/medialib/stores/apiclient/__init__.py
+-rw-r--r--   0        0        0     9852 2023-06-27 05:37:44.450415 django_restit-4.0.4/medialib/stores/apiclient/channel.py
+-rw-r--r--   0        0        0    35929 2023-06-27 05:37:44.450591 django_restit-4.0.4/medialib/stores/apiclient/discovery.py
+-rw-r--r--   0        0        0     3516 2023-06-27 05:37:44.450684 django_restit-4.0.4/medialib/stores/apiclient/errors.py
+-rw-r--r--   0        0        0    52911 2023-06-27 05:37:44.450906 django_restit-4.0.4/medialib/stores/apiclient/http.py
+-rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.451002 django_restit-4.0.4/medialib/stores/apiclient/mimeparse.py
+-rw-r--r--   0        0        0    11761 2023-06-27 05:37:44.451111 django_restit-4.0.4/medialib/stores/apiclient/model.py
+-rw-r--r--   0        0        0     3528 2023-06-27 05:37:44.451205 django_restit-4.0.4/medialib/stores/apiclient/sample_tools.py
+-rw-r--r--   0        0        0     9293 2023-06-27 05:37:44.451302 django_restit-4.0.4/medialib/stores/apiclient/schema.py
+-rw-r--r--   0        0        0     1592 2023-06-27 05:37:44.451390 django_restit-4.0.4/medialib/stores/filestore.py
+-rw-r--r--   0        0        0    69575 2023-06-27 05:37:44.451712 django_restit-4.0.4/medialib/stores/httplib2/__init__.py
+-rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.451937 django_restit-4.0.4/medialib/stores/httplib2/cacerts.txt
+-rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.452031 django_restit-4.0.4/medialib/stores/httplib2/iri2uri.py
+-rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.452160 django_restit-4.0.4/medialib/stores/httplib2/socks.py
+-rw-r--r--   0        0        0      706 2023-06-27 05:37:44.452238 django_restit-4.0.4/medialib/stores/httpstore.py
+-rw-r--r--   0        0        0      304 2023-06-27 05:37:44.452325 django_restit-4.0.4/medialib/stores/nullstore.py
+-rw-r--r--   0        0        0      213 2023-06-27 05:37:44.452492 django_restit-4.0.4/medialib/stores/oauth2client/__init__.py
+-rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.452598 django_restit-4.0.4/medialib/stores/oauth2client/anyjson.py
+-rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.452767 django_restit-4.0.4/medialib/stores/oauth2client/appengine.py
+-rw-r--r--   0        0        0    44346 2023-06-27 05:37:44.452995 django_restit-4.0.4/medialib/stores/oauth2client/client.py
+-rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.453091 django_restit-4.0.4/medialib/stores/oauth2client/clientsecrets.py
+-rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.453196 django_restit-4.0.4/medialib/stores/oauth2client/crypt.py
+-rw-r--r--   0        0        0     3755 2023-06-27 05:37:44.453276 django_restit-4.0.4/medialib/stores/oauth2client/django_orm.py
+-rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.453391 django_restit-4.0.4/medialib/stores/oauth2client/file.py
+-rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.453451 django_restit-4.0.4/medialib/stores/oauth2client/gce.py
+-rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.453541 django_restit-4.0.4/medialib/stores/oauth2client/keyring_storage.py
+-rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.453634 django_restit-4.0.4/medialib/stores/oauth2client/locked_file.py
+-rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.453698 django_restit-4.0.4/medialib/stores/oauth2client/multistore_file.py
+-rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.453764 django_restit-4.0.4/medialib/stores/oauth2client/old_run.py
+-rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.453855 django_restit-4.0.4/medialib/stores/oauth2client/tools.py
+-rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.453938 django_restit-4.0.4/medialib/stores/oauth2client/util.py
+-rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.454013 django_restit-4.0.4/medialib/stores/oauth2client/xsrfutil.py
+-rw-r--r--   0        0        0      500 2023-06-27 05:37:44.454077 django_restit-4.0.4/medialib/stores/rtmpstore.py
+-rw-r--r--   0        0        0     4583 2023-06-27 05:37:44.454163 django_restit-4.0.4/medialib/stores/s3store.py
+-rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.454272 django_restit-4.0.4/medialib/stores/uritemplate/__init__.py
+-rw-r--r--   0        0        0      406 2023-06-27 05:37:44.454334 django_restit-4.0.4/medialib/stores/youtubestore.py
+-rw-r--r--   0        0        0     3691 2023-06-27 05:37:44.454500 django_restit-4.0.4/medialib/templates/medialib/base.html
+-rw-r--r--   0        0        0     1277 2023-06-27 05:37:44.454591 django_restit-4.0.4/medialib/templates/medialib/instances.html
+-rw-r--r--   0        0        0     1170 2023-06-27 05:37:44.454657 django_restit-4.0.4/medialib/templates/medialib/items.html
+-rw-r--r--   0        0        0     8194 2023-06-27 05:37:44.454746 django_restit-4.0.4/medialib/templates/medialib/library.html
+-rw-r--r--   0        0        0       65 2023-06-27 05:37:44.454810 django_restit-4.0.4/medialib/templates/medialib/notify_error.subject
+-rw-r--r--   0        0        0       49 2023-06-27 05:37:44.454869 django_restit-4.0.4/medialib/templates/medialib/notify_error.to
+-rw-r--r--   0        0        0      272 2023-06-27 05:37:44.454932 django_restit-4.0.4/medialib/templates/medialib/notify_error.txt
+-rw-r--r--   0        0        0       71 2023-06-27 05:37:44.454996 django_restit-4.0.4/medialib/templates/medialib/notify_ready.subject
+-rw-r--r--   0        0        0       49 2023-06-27 05:37:44.455056 django_restit-4.0.4/medialib/templates/medialib/notify_ready.to
+-rw-r--r--   0        0        0      298 2023-06-27 05:37:44.455113 django_restit-4.0.4/medialib/templates/medialib/notify_ready.txt
+-rw-r--r--   0        0        0       64 2023-06-27 05:37:44.455175 django_restit-4.0.4/medialib/templates/medialib/notify_render_error.subject
+-rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455232 django_restit-4.0.4/medialib/templates/medialib/notify_render_error.to
+-rw-r--r--   0        0        0      271 2023-06-27 05:37:44.455301 django_restit-4.0.4/medialib/templates/medialib/notify_render_error.txt
+-rw-r--r--   0        0        0       68 2023-06-27 05:37:44.455380 django_restit-4.0.4/medialib/templates/medialib/notify_validate_error.subject
+-rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455452 django_restit-4.0.4/medialib/templates/medialib/notify_validate_error.to
+-rw-r--r--   0        0        0      275 2023-06-27 05:37:44.455521 django_restit-4.0.4/medialib/templates/medialib/notify_validate_error.txt
+-rw-r--r--   0        0        0      206 2023-06-27 05:37:44.455593 django_restit-4.0.4/medialib/templates/medialib/smil
+-rw-r--r--   0        0        0     1177 2023-06-27 05:37:44.455665 django_restit-4.0.4/medialib/templates/medialib/test.html
+-rw-r--r--   0        0        0     1549 2023-06-27 05:37:44.455737 django_restit-4.0.4/medialib/templates/medialib/testpicker.html
+-rw-r--r--   0        0        0     6045 2023-06-27 05:37:44.455814 django_restit-4.0.4/medialib/tests.py
+-rw-r--r--   0        0        0      544 2023-06-27 05:37:44.455873 django_restit-4.0.4/medialib/tq.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.455894 django_restit-4.0.4/medialib/urls.py
+-rw-r--r--   0        0        0     3756 2023-06-27 05:37:44.455970 django_restit-4.0.4/medialib/utils.py
+-rw-r--r--   0        0        0     4321 2023-06-27 05:37:44.456050 django_restit-4.0.4/medialib/views.py
+-rw-r--r--   0        0        0     4303 2023-06-27 05:37:44.456166 django_restit-4.0.4/medialib/youtube/__init__.py
+-rw-r--r--   0        0        0      601 2023-06-27 05:37:44.456272 django_restit-4.0.4/medialib/youtube/apiclient/__init__.py
+-rw-r--r--   0        0        0     9886 2023-06-27 05:37:44.456332 django_restit-4.0.4/medialib/youtube/apiclient/channel.py
+-rw-r--r--   0        0        0    35907 2023-06-27 05:37:44.456516 django_restit-4.0.4/medialib/youtube/apiclient/discovery.py
+-rw-r--r--   0        0        0     3550 2023-06-27 05:37:44.456592 django_restit-4.0.4/medialib/youtube/apiclient/errors.py
+-rw-r--r--   0        0        0    52945 2023-06-27 05:37:44.456694 django_restit-4.0.4/medialib/youtube/apiclient/http.py
+-rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.456785 django_restit-4.0.4/medialib/youtube/apiclient/mimeparse.py
+-rw-r--r--   0        0        0    11795 2023-06-27 05:37:44.456835 django_restit-4.0.4/medialib/youtube/apiclient/model.py
+-rw-r--r--   0        0        0     3596 2023-06-27 05:37:44.456895 django_restit-4.0.4/medialib/youtube/apiclient/sample_tools.py
+-rw-r--r--   0        0        0     9327 2023-06-27 05:37:44.456959 django_restit-4.0.4/medialib/youtube/apiclient/schema.py
+-rw-r--r--   0        0        0    69581 2023-06-27 05:37:44.457093 django_restit-4.0.4/medialib/youtube/httplib2/__init__.py
+-rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.457310 django_restit-4.0.4/medialib/youtube/httplib2/cacerts.txt
+-rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.457412 django_restit-4.0.4/medialib/youtube/httplib2/iri2uri.py
+-rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.457533 django_restit-4.0.4/medialib/youtube/httplib2/socks.py
+-rw-r--r--   0        0        0      213 2023-06-27 05:37:44.457629 django_restit-4.0.4/medialib/youtube/oauth2client/__init__.py
+-rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.457687 django_restit-4.0.4/medialib/youtube/oauth2client/anyjson.py
+-rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.457830 django_restit-4.0.4/medialib/youtube/oauth2client/appengine.py
+-rw-r--r--   0        0        0    44431 2023-06-27 05:37:44.457905 django_restit-4.0.4/medialib/youtube/oauth2client/client.py
+-rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.457990 django_restit-4.0.4/medialib/youtube/oauth2client/clientsecrets.py
+-rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.458075 django_restit-4.0.4/medialib/youtube/oauth2client/crypt.py
+-rw-r--r--   0        0        0     3753 2023-06-27 05:37:44.458140 django_restit-4.0.4/medialib/youtube/oauth2client/django_orm.py
+-rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.458204 django_restit-4.0.4/medialib/youtube/oauth2client/file.py
+-rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.458255 django_restit-4.0.4/medialib/youtube/oauth2client/gce.py
+-rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.458323 django_restit-4.0.4/medialib/youtube/oauth2client/keyring_storage.py
+-rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.458399 django_restit-4.0.4/medialib/youtube/oauth2client/locked_file.py
+-rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.458454 django_restit-4.0.4/medialib/youtube/oauth2client/multistore_file.py
+-rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.458510 django_restit-4.0.4/medialib/youtube/oauth2client/old_run.py
+-rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.458604 django_restit-4.0.4/medialib/youtube/oauth2client/tools.py
+-rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.458680 django_restit-4.0.4/medialib/youtube/oauth2client/util.py
+-rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.458745 django_restit-4.0.4/medialib/youtube/oauth2client/xsrfutil.py
+-rw-r--r--   0        0        0     2849 2023-06-27 05:37:44.458806 django_restit-4.0.4/medialib/youtube/upload.py
+-rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.458902 django_restit-4.0.4/medialib/youtube/uritemplate/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-27 05:37:44.459001 django_restit-4.0.4/metrics/README.md
+-rw-r--r--   0        0        0       90 2023-06-27 05:37:44.459061 django_restit-4.0.4/metrics/__init__.py
+-rw-r--r--   0        0        0    23460 2023-06-27 05:37:44.459219 django_restit-4.0.4/metrics/client.py
+-rw-r--r--   0        0        0     9182 2023-06-27 05:37:44.459333 django_restit-4.0.4/metrics/eod.py
+-rw-r--r--   0        0        0     1664 2023-06-27 05:37:44.459430 django_restit-4.0.4/metrics/examples/eod_example.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459493 django_restit-4.0.4/metrics/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459564 django_restit-4.0.4/metrics/management/commands/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-27 05:37:44.459636 django_restit-4.0.4/metrics/management/commands/delete_gauge.py
+-rw-r--r--   0        0        0      464 2023-06-27 05:37:44.459697 django_restit-4.0.4/metrics/management/commands/delete_metric.py
+-rw-r--r--   0        0        0     2801 2023-06-27 05:37:44.459766 django_restit-4.0.4/metrics/management/commands/fix_redis_metrics_keys.py
+-rw-r--r--   0        0        0     1928 2023-06-27 05:37:44.459829 django_restit-4.0.4/metrics/management/commands/generate_test_metrics.py
+-rw-r--r--   0        0        0     1742 2023-06-27 05:37:44.459896 django_restit-4.0.4/metrics/management/commands/redis_metrics_send_mail.py
+-rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.459957 django_restit-4.0.4/metrics/management/commands/reset_weekly_metrics.py
+-rw-r--r--   0        0        0     4343 2023-06-27 05:37:44.460023 django_restit-4.0.4/metrics/management/commands/system_metric.py
+-rw-r--r--   0        0        0     2399 2023-06-27 05:37:44.460109 django_restit-4.0.4/metrics/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1510 2023-06-27 05:37:44.460172 django_restit-4.0.4/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py
+-rw-r--r--   0        0        0      453 2023-06-27 05:37:44.460231 django_restit-4.0.4/metrics/migrations/0003_metrics_expires.py
+-rw-r--r--   0        0        0     3271 2023-06-27 05:37:44.460284 django_restit-4.0.4/metrics/migrations/0004_eodmetrics.py
+-rw-r--r--   0        0        0     2358 2023-06-27 05:37:44.460347 django_restit-4.0.4/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460367 django_restit-4.0.4/metrics/migrations/__init__.py
+-rw-r--r--   0        0        0    10599 2023-06-27 05:37:44.460461 django_restit-4.0.4/metrics/models.py
+-rw-r--r--   0        0        0      480 2023-06-27 05:37:44.460528 django_restit-4.0.4/metrics/periodic.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460587 django_restit-4.0.4/metrics/providers/__init__.py
+-rw-r--r--   0        0        0     7335 2023-06-27 05:37:44.460691 django_restit-4.0.4/metrics/providers/aws.py
+-rw-r--r--   0        0        0    14826 2023-06-27 05:37:44.460783 django_restit-4.0.4/metrics/rpc.py
+-rw-r--r--   0        0        0      132 2023-06-27 05:37:44.460832 django_restit-4.0.4/metrics/settings.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460855 django_restit-4.0.4/metrics/tq.py
+-rw-r--r--   0        0        0    10490 2023-06-27 05:37:44.460959 django_restit-4.0.4/metrics/utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461016 django_restit-4.0.4/pushit/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-27 05:37:44.461079 django_restit-4.0.4/pushit/admin.py
+-rw-r--r--   0        0        0     4555 2023-06-27 05:37:44.461167 django_restit-4.0.4/pushit/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461190 django_restit-4.0.4/pushit/migrations/__init__.py
+-rw-r--r--   0        0        0     5076 2023-06-27 05:37:44.461264 django_restit-4.0.4/pushit/models.py
+-rw-r--r--   0        0        0       88 2023-06-27 05:37:44.461351 django_restit-4.0.4/pushit/rpc/__init__.py
+-rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.461414 django_restit-4.0.4/pushit/rpc/githooks.py
+-rw-r--r--   0        0        0     5028 2023-06-27 05:37:44.461473 django_restit-4.0.4/pushit/rpc/legacy.py
+-rw-r--r--   0        0        0      378 2023-06-27 05:37:44.461520 django_restit-4.0.4/pushit/rpc/products.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461605 django_restit-4.0.4/pushit/static/js/models_pushit.js
+-rw-r--r--   0        0        0      131 2023-06-27 05:37:44.461676 django_restit-4.0.4/pushit/tq.py
+-rw-r--r--   0        0        0     1966 2023-06-27 05:37:44.461734 django_restit-4.0.4/pushit/utils.py
+-rw-r--r--   0        0        0     1401 2023-06-27 15:25:53.138170 django_restit-4.0.4/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-06-27 05:37:44.461884 django_restit-4.0.4/rest/.gitignore
+-rw-r--r--   0        0        0     5460 2023-06-27 05:37:44.461959 django_restit-4.0.4/rest/README.md
+-rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462010 django_restit-4.0.4/rest/RemoteEvents.py
+-rw-r--r--   0        0        0      120 2023-06-27 15:25:53.143859 django_restit-4.0.4/rest/__init__.py
+-rw-r--r--   0        0        0     1967 2023-06-27 05:37:44.462114 django_restit-4.0.4/rest/arc4.py
+-rw-r--r--   0        0        0       83 2023-06-27 05:37:44.462161 django_restit-4.0.4/rest/cache.py
+-rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462295 django_restit-4.0.4/rest/crypto/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-27 05:37:44.462374 django_restit-4.0.4/rest/crypto/aes.py
+-rw-r--r--   0        0        0     4082 2023-06-27 05:37:44.462442 django_restit-4.0.4/rest/crypto/privpub.py
+-rw-r--r--   0        0        0     3955 2023-06-27 05:37:44.462509 django_restit-4.0.4/rest/crypto/util.py
+-rw-r--r--   0        0        0     7784 2023-06-27 05:37:44.462604 django_restit-4.0.4/rest/datem.py
+-rw-r--r--   0        0        0    15597 2023-06-27 05:37:44.462702 django_restit-4.0.4/rest/decorators.py
+-rw-r--r--   0        0        0      788 2023-06-27 05:37:44.462816 django_restit-4.0.4/rest/encryption.py
+-rw-r--r--   0        0        0       54 2023-06-27 05:37:44.462913 django_restit-4.0.4/rest/extra/__init__.py
+-rw-r--r--   0        0        0     1078 2023-06-27 05:37:44.462982 django_restit-4.0.4/rest/extra/json_metadata.py
+-rw-r--r--   0        0        0     9719 2023-06-27 05:37:44.463072 django_restit-4.0.4/rest/fields.py
+-rw-r--r--   0        0        0     6316 2023-06-27 05:37:44.463145 django_restit-4.0.4/rest/forms.py
+-rw-r--r--   0        0        0    23837 2023-06-27 05:37:44.463266 django_restit-4.0.4/rest/helpers.py
+-rw-r--r--   0        0        0      260 2023-06-27 05:37:44.463338 django_restit-4.0.4/rest/joke.py
+-rw-r--r--   0        0        0     2298 2023-06-27 05:37:44.463411 django_restit-4.0.4/rest/jwtoken.py
+-rw-r--r--   0        0        0    20932 2023-06-27 15:25:34.224534 django_restit-4.0.4/rest/log.py
+-rw-r--r--   0        0        0     7754 2023-06-27 05:37:44.463623 django_restit-4.0.4/rest/mail.py
+-rw-r--r--   0        0        0     9174 2023-06-27 05:37:44.463711 django_restit-4.0.4/rest/mailman.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463776 django_restit-4.0.4/rest/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463861 django_restit-4.0.4/rest/management/commands/__init__.py
+-rw-r--r--   0        0        0      389 2023-06-27 05:37:44.463942 django_restit-4.0.4/rest/management/commands/rpc.py
+-rw-r--r--   0        0        0       33 2023-06-27 05:37:44.464028 django_restit-4.0.4/rest/middleware/__init__.py
+-rw-r--r--   0        0        0     3513 2023-06-27 05:37:44.464096 django_restit-4.0.4/rest/middleware/cors.py
+-rw-r--r--   0        0        0     2345 2023-06-27 05:37:44.464159 django_restit-4.0.4/rest/middleware/db_router.py
+-rw-r--r--   0        0        0     5395 2023-06-27 05:37:44.464226 django_restit-4.0.4/rest/middleware/jwt.py
+-rw-r--r--   0        0        0     4127 2023-06-27 05:37:44.464313 django_restit-4.0.4/rest/middleware/request.py
+-rw-r--r--   0        0        0     9015 2023-06-27 05:37:44.464386 django_restit-4.0.4/rest/middleware/session.py
+-rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.464450 django_restit-4.0.4/rest/middleware/session_store.py
+-rw-r--r--   0        0        0    76845 2023-06-27 05:37:44.464712 django_restit-4.0.4/rest/models.py
+-rw-r--r--   0        0        0   149463 2023-06-27 05:37:44.465139 django_restit-4.0.4/rest/regexes.yaml
+-rw-r--r--   0        0        0    14894 2023-06-27 05:37:44.465209 django_restit-4.0.4/rest/requestex.py
+-rw-r--r--   0        0        0     3713 2023-06-27 15:25:34.225162 django_restit-4.0.4/rest/rpc.py
+-rw-r--r--   0        0        0     7645 2023-06-27 05:37:44.465350 django_restit-4.0.4/rest/search.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.465410 django_restit-4.0.4/rest/serializers/__init__.py
+-rw-r--r--   0        0        0     1644 2023-06-27 05:37:44.465494 django_restit-4.0.4/rest/serializers/collection.py
+-rw-r--r--   0        0        0     2975 2023-06-27 05:37:44.465556 django_restit-4.0.4/rest/serializers/csv.py
+-rw-r--r--   0        0        0     1077 2023-06-27 05:37:44.465616 django_restit-4.0.4/rest/serializers/excel.py
+-rw-r--r--   0        0        0     1736 2023-06-27 05:37:44.465675 django_restit-4.0.4/rest/serializers/json.py
+-rw-r--r--   0        0        0    61738 2023-06-27 05:37:44.465903 django_restit-4.0.4/rest/serializers/legacy.py
+-rw-r--r--   0        0        0     4943 2023-06-27 05:37:44.465981 django_restit-4.0.4/rest/serializers/model.py
+-rw-r--r--   0        0        0     6162 2023-06-27 05:37:44.466049 django_restit-4.0.4/rest/serializers/response.py
+-rw-r--r--   0        0        0     2734 2023-06-27 05:37:44.466139 django_restit-4.0.4/rest/serializers/util.py
+-rw-r--r--   0        0        0     1532 2023-06-27 05:37:44.466216 django_restit-4.0.4/rest/settings_helper.py
+-rw-r--r--   0        0        0    95786 2023-06-27 05:37:44.466685 django_restit-4.0.4/rest/static/lib/jquery.js
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466742 django_restit-4.0.4/rest/static/rest/app.css
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466776 django_restit-4.0.4/rest/static/rest/app.js
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466808 django_restit-4.0.4/rest/static/rest/rest.js
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466846 django_restit-4.0.4/rest/static/rest/rest.scss
+-rw-r--r--   0        0        0      529 2023-06-27 05:37:44.466992 django_restit-4.0.4/rest/templates/email/error.html
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.467020 django_restit-4.0.4/rest/templates/email/error.subject
+-rw-r--r--   0        0        0     7148 2023-06-27 05:37:44.467101 django_restit-4.0.4/rest/templates/rest_docs.html
+-rw-r--r--   0        0        0    10880 2023-06-27 05:37:44.467182 django_restit-4.0.4/rest/templates/rest_html.html
+-rw-r--r--   0        0        0   185122 2023-06-27 05:37:44.467607 django_restit-4.0.4/rest/ua.py
+-rw-r--r--   0        0        0    17064 2023-06-27 05:37:44.467734 django_restit-4.0.4/rest/uberdict.py
+-rw-r--r--   0        0        0    11881 2023-06-27 05:37:44.467820 django_restit-4.0.4/rest/url_docs.py
+-rw-r--r--   0        0        0     1787 2023-06-27 05:37:44.467877 django_restit-4.0.4/rest/urls.py
+-rw-r--r--   0        0        0     1056 2023-06-27 05:37:44.467929 django_restit-4.0.4/rest/views.py
+-rw-r--r--   0        0        0      118 2023-06-27 05:37:44.468007 django_restit-4.0.4/sessionlog/.gitignore
+-rw-r--r--   0        0        0       62 2023-06-27 05:37:44.468062 django_restit-4.0.4/sessionlog/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468086 django_restit-4.0.4/sessionlog/__init__.py
+-rw-r--r--   0        0        0      245 2023-06-27 05:37:44.468153 django_restit-4.0.4/sessionlog/admin.py
+-rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.468231 django_restit-4.0.4/sessionlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468261 django_restit-4.0.4/sessionlog/migrations/__init__.py
+-rw-r--r--   0        0        0     3922 2023-06-27 05:37:44.468340 django_restit-4.0.4/sessionlog/models.py
+-rw-r--r--   0        0        0      383 2023-06-27 05:37:44.468400 django_restit-4.0.4/sessionlog/tests.py
+-rw-r--r--   0        0        0       26 2023-06-27 05:37:44.468451 django_restit-4.0.4/sessionlog/views.py
+-rw-r--r--   0        0        0     2196 2023-06-27 05:37:44.468543 django_restit-4.0.4/taskqueue/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468569 django_restit-4.0.4/taskqueue/__init__.py
+-rw-r--r--   0        0        0      208 2023-06-27 05:37:44.468635 django_restit-4.0.4/taskqueue/admin.py
+-rw-r--r--   0        0        0     4738 2023-06-27 05:37:44.468730 django_restit-4.0.4/taskqueue/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468758 django_restit-4.0.4/taskqueue/migrations/__init__.py
+-rw-r--r--   0        0        0    16531 2023-06-27 05:37:44.468876 django_restit-4.0.4/taskqueue/models.py
+-rw-r--r--   0        0        0     3072 2023-06-27 05:37:44.468952 django_restit-4.0.4/taskqueue/periodic.py
+-rw-r--r--   0        0        0     5326 2023-06-27 05:37:44.469019 django_restit-4.0.4/taskqueue/rpc.py
+-rw-r--r--   0        0        0      942 2023-06-27 05:37:44.469073 django_restit-4.0.4/taskqueue/tq.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469126 django_restit-4.0.4/taskqueue/transports/__init__.py
+-rw-r--r--   0        0        0      623 2023-06-27 05:37:44.469185 django_restit-4.0.4/taskqueue/transports/email.py
+-rw-r--r--   0        0        0     2409 2023-06-27 05:37:44.469240 django_restit-4.0.4/taskqueue/transports/http.py
+-rw-r--r--   0        0        0     1099 2023-06-27 05:37:44.469291 django_restit-4.0.4/taskqueue/transports/s3.py
+-rw-r--r--   0        0        0     1891 2023-06-27 05:37:44.469341 django_restit-4.0.4/taskqueue/transports/sftp.py
+-rw-r--r--   0        0        0      142 2023-06-27 05:37:44.469388 django_restit-4.0.4/taskqueue/transports/sms.py
+-rw-r--r--   0        0        0    13660 2023-06-27 05:37:44.469465 django_restit-4.0.4/taskqueue/worker.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469517 django_restit-4.0.4/telephony/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-27 05:37:44.469571 django_restit-4.0.4/telephony/admin.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469591 django_restit-4.0.4/telephony/decorators.py
+-rw-r--r--   0        0        0     3030 2023-06-27 05:37:44.469692 django_restit-4.0.4/telephony/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469714 django_restit-4.0.4/telephony/migrations/__init__.py
+-rw-r--r--   0        0        0     7753 2023-06-27 05:37:44.469796 django_restit-4.0.4/telephony/models.py
+-rw-r--r--   0        0        0     2126 2023-06-27 05:37:44.469861 django_restit-4.0.4/telephony/phone_util.py
+-rw-r--r--   0        0        0     2659 2023-06-27 05:37:44.469923 django_restit-4.0.4/telephony/rpc.py
+-rw-r--r--   0        0        0     3624 2023-06-27 05:37:44.470008 django_restit-4.0.4/ws4redis/README.md
+-rwxr-xr-x   0        0        0       46 2023-06-27 05:37:44.470065 django_restit-4.0.4/ws4redis/__init__.py
+-rw-r--r--   0        0        0     4942 2023-06-27 05:37:44.470133 django_restit-4.0.4/ws4redis/client.py
+-rw-r--r--   0        0        0    13026 2023-06-27 05:37:44.470238 django_restit-4.0.4/ws4redis/connection.py
+-rwxr-xr-x   0        0        0      636 2023-06-27 05:37:44.470295 django_restit-4.0.4/ws4redis/exceptions.py
+-rw-r--r--   0        0        0     5548 2023-06-27 05:37:44.470365 django_restit-4.0.4/ws4redis/redis.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.470422 django_restit-4.0.4/ws4redis/servers/__init__.py
+-rw-r--r--   0        0        0     3747 2023-06-27 05:37:44.470507 django_restit-4.0.4/ws4redis/servers/base.py
+-rw-r--r--   0        0        0     4329 2023-06-27 05:37:44.470582 django_restit-4.0.4/ws4redis/servers/django.py
+-rw-r--r--   0        0        0     1723 2023-06-27 05:37:44.470638 django_restit-4.0.4/ws4redis/servers/uwsgi.py
+-rwxr-xr-x   0        0        0     1411 2023-06-27 05:37:44.470697 django_restit-4.0.4/ws4redis/settings.py
+-rwxr-xr-x   0        0        0     5122 2023-06-27 05:37:44.470772 django_restit-4.0.4/ws4redis/utf8validator.py
+-rwxr-xr-x   0        0        0    14848 2023-06-27 05:37:44.470868 django_restit-4.0.4/ws4redis/websocket.py
+-rw-r--r--   0        0        0     7525 1970-01-01 00:00:00.000000 django_restit-4.0.4/PKG-INFO
```

### Comparing `django_restit-4.0.2/LICENSE.md` & `django_restit-4.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/README.md` & `django_restit-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/admin.py` & `django_restit-4.0.4/account/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/fcm/__init__.py` & `django_restit-4.0.4/account/fcm/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/migrations/0001_initial.py` & `django_restit-4.0.4/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/migrations/0003_member_phone_number.py` & `django_restit-4.0.4/account/migrations/0003_member_phone_number.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/migrations/0004_group_modified_alter_group_created.py` & `django_restit-4.0.4/account/migrations/0004_group_modified_alter_group_created.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/migrations/0007_authtoken_signature_authsession.py` & `django_restit-4.0.4/account/migrations/0007_authtoken_signature_authsession.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/migrations/0008_memberdevice_memberdevicemetadata.py` & `django_restit-4.0.4/account/migrations/0008_memberdevice_memberdevicemetadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/migrations/0011_authtoken.py` & `django_restit-4.0.4/account/migrations/0011_authtoken.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/migrations/0012_settings_settingsmetadata.py` & `django_restit-4.0.4/account/migrations/0012_settings_settingsmetadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/models/device.py` & `django_restit-4.0.4/account/models/device.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/models/feeds.py` & `django_restit-4.0.4/account/models/feeds.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/models/group.py` & `django_restit-4.0.4/account/models/group.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/models/legacy.py` & `django_restit-4.0.4/account/models/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/models/member.py` & `django_restit-4.0.4/account/models/member.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/models/membership.py` & `django_restit-4.0.4/account/models/membership.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/models/notify.py` & `django_restit-4.0.4/account/models/notify.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/models/session.py` & `django_restit-4.0.4/account/models/session.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/models/settings.py` & `django_restit-4.0.4/account/models/settings.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/oauth/google.py` & `django_restit-4.0.4/account/oauth/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/periodic.py` & `django_restit-4.0.4/account/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/rpc/auth.py` & `django_restit-4.0.4/account/rpc/auth.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/rpc/device.py` & `django_restit-4.0.4/account/rpc/device.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/rpc/group.py` & `django_restit-4.0.4/account/rpc/group.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/rpc/member.py` & `django_restit-4.0.4/account/rpc/member.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/rpc/notify.py` & `django_restit-4.0.4/account/rpc/notify.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/rpc/oauth.py` & `django_restit-4.0.4/account/rpc/oauth.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/templates/email/base.html` & `django_restit-4.0.4/account/templates/email/base.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/templates/email/invite.html` & `django_restit-4.0.4/account/templates/email/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/templates/email/plain/invite.html` & `django_restit-4.0.4/account/templates/email/plain/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/templates/email/plain/reset_code.html` & `django_restit-4.0.4/account/templates/email/plain/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/templates/email/reset_code.html` & `django_restit-4.0.4/account/templates/email/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/templates/email/simple/invite.html` & `django_restit-4.0.4/account/templates/email/simple/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/account/templates/email/simple/reset_code.html` & `django_restit-4.0.4/account/templates/email/simple/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/auditlog/README` & `django_restit-4.0.4/auditlog/README`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/auditlog/admin.py` & `django_restit-4.0.4/auditlog/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/auditlog/decorators.py` & `django_restit-4.0.4/auditlog/decorators.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/auditlog/middleware.py` & `django_restit-4.0.4/auditlog/middleware.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/auditlog/migrations/0001_initial.py` & `django_restit-4.0.4/auditlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/auditlog/models.py` & `django_restit-4.0.4/auditlog/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/auditlog/rpc.py` & `django_restit-4.0.4/auditlog/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/auditlog/tq.py` & `django_restit-4.0.4/auditlog/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/inbox/README.md` & `django_restit-4.0.4/inbox/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/inbox/handlers.py` & `django_restit-4.0.4/inbox/handlers.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/inbox/migrations/0001_initial.py` & `django_restit-4.0.4/inbox/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/inbox/migrations/0004_mailtemplate.py` & `django_restit-4.0.4/inbox/migrations/0004_mailtemplate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/inbox/models/bounce.py` & `django_restit-4.0.4/inbox/models/bounce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/inbox/models/complaint.py` & `django_restit-4.0.4/inbox/models/complaint.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/inbox/models/message.py` & `django_restit-4.0.4/inbox/models/message.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/inbox/models/template.py` & `django_restit-4.0.4/inbox/models/template.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/inbox/rpc.py` & `django_restit-4.0.4/inbox/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/inbox/utils/parsing.py` & `django_restit-4.0.4/inbox/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/inbox/utils/render.py` & `django_restit-4.0.4/inbox/utils/render.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/inbox/utils/sending.py` & `django_restit-4.0.4/inbox/utils/sending.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/README.md` & `django_restit-4.0.4/incident/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/__init__.py` & `django_restit-4.0.4/incident/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/migrations/0001_initial.py` & `django_restit-4.0.4/incident/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/migrations/0002_event_component_event_component_id.py` & `django_restit-4.0.4/incident/migrations/0002_event_component_event_component_id.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py` & `django_restit-4.0.4/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/migrations/0005_incident_component_alter_incident_state.py` & `django_restit-4.0.4/incident/migrations/0005_incident_component_alter_incident_state.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py` & `django_restit-4.0.4/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/models/event.py` & `django_restit-4.0.4/incident/models/event.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/models/incident.py` & `django_restit-4.0.4/incident/models/incident.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/models/ossec.py` & `django_restit-4.0.4/incident/models/ossec.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/models/rules.py` & `django_restit-4.0.4/incident/models/rules.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/parsers/ossec.py` & `django_restit-4.0.4/incident/parsers/ossec.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/periodic.py` & `django_restit-4.0.4/incident/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/rpc.py` & `django_restit-4.0.4/incident/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/templates/email/incident_change.html` & `django_restit-4.0.4/incident/templates/email/incident_change.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/templates/email/incident_new.html` & `django_restit-4.0.4/incident/templates/email/incident_new.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/templates/email/incident_plain.html` & `django_restit-4.0.4/incident/templates/email/incident_plain.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/incident/tq.py` & `django_restit-4.0.4/incident/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/geolocate.py` & `django_restit-4.0.4/location/geolocate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/migrations/0001_initial.py` & `django_restit-4.0.4/location/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/migrations/0002_geoip_subnet_alter_geoip_ip.py` & `django_restit-4.0.4/location/migrations/0002_geoip_subnet_alter_geoip_ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/models/address.py` & `django_restit-4.0.4/location/models/address.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/models/ip.py` & `django_restit-4.0.4/location/models/ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/models/legacy.py` & `django_restit-4.0.4/location/models/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/models/location.py` & `django_restit-4.0.4/location/models/location.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/models/track.py` & `django_restit-4.0.4/location/models/track.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/providers/iplookup/__init__.py` & `django_restit-4.0.4/location/providers/iplookup/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/providers/iplookup/abstractapi.py` & `django_restit-4.0.4/location/providers/iplookup/abstractapi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/providers/iplookup/extremeip.py` & `django_restit-4.0.4/location/providers/iplookup/extremeip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/providers/iplookup/geoplugin.py` & `django_restit-4.0.4/location/providers/iplookup/geoplugin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/providers/iplookup/ipapi.py` & `django_restit-4.0.4/location/providers/iplookup/ipapi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/providers/iplookup/ipinfo.py` & `django_restit-4.0.4/location/providers/iplookup/ipinfo.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/providers/iplookup/restit.py` & `django_restit-4.0.4/location/providers/iplookup/restit.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/providers/location/google.py` & `django_restit-4.0.4/location/providers/location/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/providers/timezones/google.py` & `django_restit-4.0.4/location/providers/timezones/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/providers/zillow.py` & `django_restit-4.0.4/location/providers/zillow.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/rpc/ip.py` & `django_restit-4.0.4/location/rpc/ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/rpc/location.py` & `django_restit-4.0.4/location/rpc/location.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/location/rpc/track.py` & `django_restit-4.0.4/location/rpc/track.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/admin.py` & `django_restit-4.0.4/medialib/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/cvutil/contours.py` & `django_restit-4.0.4/medialib/cvutil/contours.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/cvutil/images.py` & `django_restit-4.0.4/medialib/cvutil/images.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/cvutil/misc.py` & `django_restit-4.0.4/medialib/cvutil/misc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/cvutil/text.py` & `django_restit-4.0.4/medialib/cvutil/text.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/fixtures/initial_data.json` & `django_restit-4.0.4/medialib/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/fixtures/medialib.json` & `django_restit-4.0.4/medialib/fixtures/medialib.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/fixtures/medialib_test_fixture.json` & `django_restit-4.0.4/medialib/fixtures/medialib_test_fixture.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/forms.py` & `django_restit-4.0.4/medialib/forms.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/migrations/0001_initial.py` & `django_restit-4.0.4/medialib/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/models.py` & `django_restit-4.0.4/medialib/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/ocr.py` & `django_restit-4.0.4/medialib/ocr.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/pdf.py` & `django_restit-4.0.4/medialib/pdf.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/qrcode.py` & `django_restit-4.0.4/medialib/qrcode.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/__init__.py` & `django_restit-4.0.4/medialib/render/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/engines/anigif.py` & `django_restit-4.0.4/medialib/render/engines/anigif.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/engines/ffmpeg.py` & `django_restit-4.0.4/medialib/render/engines/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/engines/gifsicle.py` & `django_restit-4.0.4/medialib/render/engines/gifsicle.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/engines/hls.py` & `django_restit-4.0.4/medialib/render/engines/hls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/engines/mp4box.py` & `django_restit-4.0.4/medialib/render/engines/mp4box.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/engines/rtmp/rtmp.i` & `django_restit-4.0.4/medialib/render/engines/rtmp/rtmp.i`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/engines/rtmpdump.py` & `django_restit-4.0.4/medialib/render/engines/rtmpdump.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/engines/rtmpsink.py` & `django_restit-4.0.4/medialib/render/engines/rtmpsink.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/engines/video_getinfo.py` & `django_restit-4.0.4/medialib/render/engines/video_getinfo.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/engines/websnap.py` & `django_restit-4.0.4/medialib/render/engines/websnap.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/exceptions.py` & `django_restit-4.0.4/medialib/render/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/presets/akamai.py` & `django_restit-4.0.4/medialib/render/presets/akamai.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/presets/animated_thumbnail.py` & `django_restit-4.0.4/medialib/render/presets/animated_thumbnail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/presets/ffmpeg.py` & `django_restit-4.0.4/medialib/render/presets/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/presets/flv.py` & `django_restit-4.0.4/medialib/render/presets/flv.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/presets/hls.py` & `django_restit-4.0.4/medialib/render/presets/hls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/presets/image_transcode.py` & `django_restit-4.0.4/medialib/render/presets/image_transcode.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/presets/image_validate.py` & `django_restit-4.0.4/medialib/render/presets/image_validate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/presets/mp4.py` & `django_restit-4.0.4/medialib/render/presets/mp4.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/presets/video_still.py` & `django_restit-4.0.4/medialib/render/presets/video_still.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/presets/video_validate.py` & `django_restit-4.0.4/medialib/render/presets/video_validate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/presets/websnap.py` & `django_restit-4.0.4/medialib/render/presets/websnap.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/presets/youtube.py` & `django_restit-4.0.4/medialib/render/presets/youtube.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/render/render_utils.py` & `django_restit-4.0.4/medialib/render/render_utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/rpc/legacy.py` & `django_restit-4.0.4/medialib/rpc/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/rpc/media.py` & `django_restit-4.0.4/medialib/rpc/media.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/rpc/tools.py` & `django_restit-4.0.4/medialib/rpc/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/scripts/init_config` & `django_restit-4.0.4/medialib/scripts/init_config`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/css/base_medialibui.css` & `django_restit-4.0.4/medialib/static/css/base_medialibui.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/css/base_widgets.css` & `django_restit-4.0.4/medialib/static/css/base_widgets.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/css/jquery.jcrop.css` & `django_restit-4.0.4/medialib/static/css/jquery.jcrop.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/img/bg-body.gif` & `django_restit-4.0.4/medialib/static/img/bg-body.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/img/loading.gif` & `django_restit-4.0.4/medialib/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/img/noimage.gif` & `django_restit-4.0.4/medialib/static/img/noimage.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/img/render_err.gif` & `django_restit-4.0.4/medialib/static/img/render_err.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/img/rendering.gif` & `django_restit-4.0.4/medialib/static/img/rendering.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/img/unknown.gif` & `django_restit-4.0.4/medialib/static/img/unknown.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/lib/caman.full.js` & `django_restit-4.0.4/medialib/static/lib/caman.full.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/lib/hammer.min.js` & `django_restit-4.0.4/medialib/static/lib/hammer.min.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/lib/jquery.Jcrop.js` & `django_restit-4.0.4/medialib/static/lib/jquery.Jcrop.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/lib/jquery.hammer.js` & `django_restit-4.0.4/medialib/static/lib/jquery.hammer.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/lib/load-image.min.js` & `django_restit-4.0.4/medialib/static/lib/load-image.min.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/lib/swiper.js` & `django_restit-4.0.4/medialib/static/lib/swiper.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js` & `django_restit-4.0.4/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js` & `django_restit-4.0.4/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js` & `django_restit-4.0.4/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/static/lib/tinymce/plugins/medialib/medialib.html` & `django_restit-4.0.4/medialib/static/lib/tinymce/plugins/medialib/medialib.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/__init__.py` & `django_restit-4.0.4/medialib/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/apiclient/__init__.py` & `django_restit-4.0.4/medialib/stores/apiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/apiclient/channel.py` & `django_restit-4.0.4/medialib/stores/apiclient/channel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/apiclient/discovery.py` & `django_restit-4.0.4/medialib/stores/apiclient/discovery.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/apiclient/errors.py` & `django_restit-4.0.4/medialib/stores/apiclient/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/apiclient/http.py` & `django_restit-4.0.4/medialib/stores/apiclient/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/apiclient/mimeparse.py` & `django_restit-4.0.4/medialib/stores/apiclient/mimeparse.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/apiclient/model.py` & `django_restit-4.0.4/medialib/stores/apiclient/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/apiclient/sample_tools.py` & `django_restit-4.0.4/medialib/stores/apiclient/sample_tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/apiclient/schema.py` & `django_restit-4.0.4/medialib/stores/apiclient/schema.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/filestore.py` & `django_restit-4.0.4/medialib/stores/filestore.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/httplib2/__init__.py` & `django_restit-4.0.4/medialib/stores/httplib2/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/httplib2/cacerts.txt` & `django_restit-4.0.4/medialib/stores/httplib2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/httplib2/iri2uri.py` & `django_restit-4.0.4/medialib/stores/httplib2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/httplib2/socks.py` & `django_restit-4.0.4/medialib/stores/httplib2/socks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/httpstore.py` & `django_restit-4.0.4/medialib/stores/httpstore.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/anyjson.py` & `django_restit-4.0.4/medialib/stores/oauth2client/anyjson.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/appengine.py` & `django_restit-4.0.4/medialib/stores/oauth2client/appengine.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/client.py` & `django_restit-4.0.4/medialib/stores/oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/clientsecrets.py` & `django_restit-4.0.4/medialib/stores/oauth2client/clientsecrets.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/crypt.py` & `django_restit-4.0.4/medialib/stores/oauth2client/crypt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/django_orm.py` & `django_restit-4.0.4/medialib/stores/oauth2client/django_orm.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/file.py` & `django_restit-4.0.4/medialib/stores/oauth2client/file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/gce.py` & `django_restit-4.0.4/medialib/stores/oauth2client/gce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/keyring_storage.py` & `django_restit-4.0.4/medialib/stores/oauth2client/keyring_storage.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/locked_file.py` & `django_restit-4.0.4/medialib/stores/oauth2client/locked_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/multistore_file.py` & `django_restit-4.0.4/medialib/stores/oauth2client/multistore_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/old_run.py` & `django_restit-4.0.4/medialib/stores/oauth2client/old_run.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/tools.py` & `django_restit-4.0.4/medialib/stores/oauth2client/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/util.py` & `django_restit-4.0.4/medialib/stores/oauth2client/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/oauth2client/xsrfutil.py` & `django_restit-4.0.4/medialib/stores/oauth2client/xsrfutil.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/s3store.py` & `django_restit-4.0.4/medialib/stores/s3store.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/stores/uritemplate/__init__.py` & `django_restit-4.0.4/medialib/stores/uritemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/templates/medialib/base.html` & `django_restit-4.0.4/medialib/templates/medialib/base.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/templates/medialib/instances.html` & `django_restit-4.0.4/medialib/templates/medialib/instances.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/templates/medialib/items.html` & `django_restit-4.0.4/medialib/templates/medialib/items.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/templates/medialib/library.html` & `django_restit-4.0.4/medialib/templates/medialib/library.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/templates/medialib/test.html` & `django_restit-4.0.4/medialib/templates/medialib/test.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/templates/medialib/testpicker.html` & `django_restit-4.0.4/medialib/templates/medialib/testpicker.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/tests.py` & `django_restit-4.0.4/medialib/tests.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/tq.py` & `django_restit-4.0.4/medialib/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/utils.py` & `django_restit-4.0.4/medialib/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/views.py` & `django_restit-4.0.4/medialib/views.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/__init__.py` & `django_restit-4.0.4/medialib/youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/apiclient/__init__.py` & `django_restit-4.0.4/medialib/youtube/apiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/apiclient/channel.py` & `django_restit-4.0.4/medialib/youtube/apiclient/channel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/apiclient/discovery.py` & `django_restit-4.0.4/medialib/youtube/apiclient/discovery.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/apiclient/errors.py` & `django_restit-4.0.4/medialib/youtube/apiclient/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/apiclient/http.py` & `django_restit-4.0.4/medialib/youtube/apiclient/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/apiclient/mimeparse.py` & `django_restit-4.0.4/medialib/youtube/apiclient/mimeparse.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/apiclient/model.py` & `django_restit-4.0.4/medialib/youtube/apiclient/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/apiclient/sample_tools.py` & `django_restit-4.0.4/medialib/youtube/apiclient/sample_tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/apiclient/schema.py` & `django_restit-4.0.4/medialib/youtube/apiclient/schema.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/httplib2/__init__.py` & `django_restit-4.0.4/medialib/youtube/httplib2/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/httplib2/cacerts.txt` & `django_restit-4.0.4/medialib/youtube/httplib2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/httplib2/iri2uri.py` & `django_restit-4.0.4/medialib/youtube/httplib2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/httplib2/socks.py` & `django_restit-4.0.4/medialib/youtube/httplib2/socks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/anyjson.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/anyjson.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/appengine.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/appengine.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/client.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/clientsecrets.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/clientsecrets.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/crypt.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/crypt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/django_orm.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/django_orm.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/file.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/gce.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/gce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/keyring_storage.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/keyring_storage.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/locked_file.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/locked_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/multistore_file.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/multistore_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/old_run.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/old_run.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/tools.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/util.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/oauth2client/xsrfutil.py` & `django_restit-4.0.4/medialib/youtube/oauth2client/xsrfutil.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/upload.py` & `django_restit-4.0.4/medialib/youtube/upload.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/medialib/youtube/uritemplate/__init__.py` & `django_restit-4.0.4/medialib/youtube/uritemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/README.md` & `django_restit-4.0.4/metrics/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/client.py` & `django_restit-4.0.4/metrics/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/eod.py` & `django_restit-4.0.4/metrics/eod.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/examples/eod_example.py` & `django_restit-4.0.4/metrics/examples/eod_example.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/management/commands/fix_redis_metrics_keys.py` & `django_restit-4.0.4/metrics/management/commands/fix_redis_metrics_keys.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/management/commands/generate_test_metrics.py` & `django_restit-4.0.4/metrics/management/commands/generate_test_metrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/management/commands/redis_metrics_send_mail.py` & `django_restit-4.0.4/metrics/management/commands/redis_metrics_send_mail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/management/commands/reset_weekly_metrics.py` & `django_restit-4.0.4/metrics/management/commands/reset_weekly_metrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/management/commands/system_metric.py` & `django_restit-4.0.4/metrics/management/commands/system_metric.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/migrations/0001_initial.py` & `django_restit-4.0.4/metrics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py` & `django_restit-4.0.4/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/migrations/0004_eodmetrics.py` & `django_restit-4.0.4/metrics/migrations/0004_eodmetrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py` & `django_restit-4.0.4/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/models.py` & `django_restit-4.0.4/metrics/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/providers/aws.py` & `django_restit-4.0.4/metrics/providers/aws.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/rpc.py` & `django_restit-4.0.4/metrics/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/metrics/utils.py` & `django_restit-4.0.4/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/pushit/migrations/0001_initial.py` & `django_restit-4.0.4/pushit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/pushit/models.py` & `django_restit-4.0.4/pushit/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/pushit/rpc.py` & `django_restit-4.0.4/rest/url_docs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,334 +1,330 @@
-from django.db import models
+import collections
+import inspect
+import re
+import sys
+
+def guess_wrapper(cells):
+    # look through the funciton closure for cells that look
+    # like wrapped functions. for multuple functions,
+    # attempt to guess which is the more likely candidate
+
+    # we add points for
+    # * non-lambda
+    # * 'request' in arg list
+
+    functions = collections.defaultdict(list)
+    for cell in cells:
+        contents = cell.cell_contents
+        if not inspect.isfunction(contents):
+            continue
+
+        score = 0
+        if contents.__name__ != '<lambda>':
+            score += 1
+        if 'request' in inspect.getargspec(contents).args:
+            score += 1
 
+        functions[score].append(contents)
 
-from account.models import Member
+    for score in reversed(sorted(functions.keys())):
+        return functions[score][0]
+    return None
 
-from rest.views import *
-from rest.decorators import *
-from rest import search
-from rest import helpers
-from rest import crypto
-from rest import log
-from rest import settings
 
+def unwrap_and_compare(kwargs_provided, callback, description):
+    # if the callback is decorated, unwrap to find the
+    # original view
+
+    # if we have a decorated function, the "wrapped"
+    # function should b in the closure of the decorator
+    # so we look for functions in the closure, guessing
+    # if neccessary.
+
+    if callback is not None:
+        while callback.__closure__:
+            compare(kwargs_provided, callback, description)
+            cells = callback.__closure__
+            guess = guess_wrapper(cells)
+            if guess:
+                callback = guess
+            else:
+                # nothing in the closure was a function, so give up
+                break
+        compare(kwargs_provided, callback, description)
+        return callback
 
-logger = log.getLogger("pushit", filename="pushit.log")
 
-from objict import objict
 
-from pushit.models import Product, Release
+def compare(kwargs_provided, callback, description):
+    spec = inspect.getargspec(callback)
 
-import json
+    args = spec.args
+    defaults = spec.defaults
+    if defaults:
+        required_args = args[:-len(defaults)]
+    else:
+        required_args = args
 
-import base64
+    missing_kwargs = set(required_args) - kwargs_provided
+    if missing_kwargs:
+        print(("%s: view requires kwargs %s not in the url kwargs" % (
+            description, list(missing_kwargs))))
 
-from datetime import datetime, timedelta
-import time
 
-@urlPOST (r'^product$')
-@urlPOST (r'^product/(?P<product_id>\d+)$')
-@urlPOST (r'^product/uuid/(?P<uuid>\w+)$')
-@login_optional
-def updateProduct(request, product_id=None, uuid=None):
-    if not request.member:
-        return restPermissionDenied(request)
-    product = None
-    if not product_id and not uuid:
-        product = Product.createFromRequest(request, owner=request.member, group=request.group)
-    elif product_id:
-        product = Product.objects.filter(pk=product_id).last()
-    elif uuid:
-        product = Product.objects.filter(oid=uuid).last()
-
-    if not product:
-        return restStatus(request, False, error="unknown product")
-    if product.owner != request.member or (product.group and not request.member.isMemberOf(product.group)):
-        if not request.user.is_staff:
-            return restPermissionDenied(request)
-        product.saveFromRequest(request, owner=request.member)
-    return restGet(request, product, **Product.getGraph("default"))
-
-@urlGET (r'^product/(?P<product_id>\d+)$')
-@urlGET (r'^product/uuid/(?P<uuid>\w+)$')
-@login_optional
-def getProduct(request, product_id=None, uuid=None):
-    product = None
-    if product_id:
-        product = Product.objects.filter(pk=product_id).last()
-    elif uuid:
-        product = Product.objects.filter(oid=uuid).last()
-    else:
-        return restNotFound(request)
+    if spec.keywords:
+        # signature contains **kwargs, so can't do second check
+        return
 
-    if not product:
-        return restStatus(request, False, error="unknown product")
-    if not product.is_public and not request.member:
-        return restPermissionDenied(request, "not logged in")
-    return product.restGet(request)
-
-@urlGET (r'^product$')
-@login_optional
-def listProducts(request):
-    if not request.member:
-        return restPermissionDenied(request)
-    if not request.member.is_staff:
-        return restPermissionDenied(request)
-
-    kind = request.DATA.get("kind")
-    qset = Product.objects.filter(archived=False)
-    if kind:
-        qset = qset.filter(kind=kind)
-
-    return restList(request, qset, **Product.getGraph("default"))
-
-@urlPOST (r'^release$')
-@urlPOST (r'^release/(?P<release_id>\d+)$')
-@login_optional
-def updateRelease(request, release_id=None):
-    if not request.member:
-        return restPermissionDenied(request)
-
-    if not release_id:
-        auto_version = request.DATA.get("auto_version", False)
-        prod_uuid = request.DATA.get(["product", "product_uuid"])
-        product = None
-        if prod_uuid:
-            product = Product.objects.filter(oid=prod_uuid).last()
-        else:
-            prod_id = request.DATA.get("product_id")
-            if prod_id:
-                product = Product.objects.filter(pk=prod_id).last()
-        if not product:
-            return restStatus(request, False, error="product required")
-        version_num = request.DATA.get("version_num", field_type=int)
-        last_release = Release.objects.filter(product=product).order_by("-version_num").first()
-
-        if not version_num:
-            if last_release and auto_version:
-                version_num = last_release.version_num + 1
-            elif auto_version:
-                version_num = 1
-            else:
-                return restStatus(request, False, error="no version info supplied, try auto_version=1")
-        elif last_release and version_num <= last_release.version_num:
-            return restStatus(request, False, error="version is not greater then last")
+    extra_kwargs = kwargs_provided - set(args)
+    if extra_kwargs:
+        print(("%s: url provides kwargs %s not in the view signature" % (
+            description, list(extra_kwargs))))
 
-        release = Release.createFromRequest(request, product=product, owner=request.member, group=request.group, version_num=version_num)
-    else:
-        release = Release.objects.filter(pk=release_id).last()
-        if not release:
-            return restStatus(request, False, error="unknown release")
-        if release.owner != request.member or (release.product.group and not request.member.isMemberOf(release.product.group)):
-            if not request.user.is_staff:
-                return restPermissionDenied(request)
-        release.saveFromRequest(request, owner=request.member)
-    if request.DATA.get("make_current"):
-        release.makeCurrent()
-    elif request.DATA.get("make_beta"):
-        release.makeCurrent()
-    return restGet(request, release, **Release.getGraph("default"))
-
-@urlGET (r'^release/(?P<release_id>\d+)$')
-@login_optional
-def getRelease(request, release_id):
-    release = Release.objects.filter(pk=release_id).last()
-    if not release:
-        return restStatus(request, False, error="unknown release")
-    if not release.product.is_public and not request.member:
-        return restPermissionDenied(request, "not logged in")
-    return restGet(request, release, **Release.getGraph("default"))
-
-def reportRestIssue(subject, message, perm="rest_errors", email_only=False):
-    # notifyWithPermission(perm, subject, message=None, template=None, context=None, email_only=False)
-    # notify email only
-    Member.notifyWithPermission(perm, subject, message, email_only=email_only)
-
-from random import randint
-@rest_async
-def update_code(git_updater, updater_md5=None, branch=None):
-    # randomize the hit so we avoid collisions (gitlabs issues)
-    time.sleep(randint(1, 10))
-    import os
-    import subprocess
-    # check md5sum
-    if updater_md5:
-        cur_md5 = crypto.getFileMD5(git_updater)
-        if cur_md5.lower() != updater_md5.lower():
-            reportRestIssue("md5 check failed", "{}\ncould not be executed, md5 check failed".format(git_updater))
-            return
-
-    # TODO
-    # - check for errors and permissions
-    if settings.PUSHIT_TEST_SUDO:
-        cmd = ["sudo", "-lU", "ec2-user", git_updater, branch]
-        process = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-        out, err = process.communicate()
-        if err.strip():
-            logger.warning("WARNING: cannot run {}, we don't have sudo rights".format(git_updater))
-            logger.warning("WARNING: add {} to your sudo user".format(git_updater))
-            return
-    # - lock it so we kill any updates in progress and start a new one
-    cmd = ["sudo", "-u", "ec2-user", git_updater, branch]
-    logger.info("updating...", cmd)
-    subprocess.Popen(cmd, close_fds=True)
-
-@rest_async
-def new_release(product, tag, url, msg):
-    version_str = tag
-    if tag.startswith("v"):
-        version_str = tag[1:]
-
-    rev = tag.split('.')[-1]
-    if not rev.isdigit():
-        return False
-    token =  product.getProperty("git_token", "XXXXX")
-    release = Release(product=product, version_num=int(rev), version_str=version_str, notes=msg)
-    release.owner = product.owner
-    release_url = "{}/repository/{}/archive.zip?private_token={}".format(url, tag, token)
-    release.save()
-    logger.info(release_url)
-    release.set_media(release_url, True)
-    release.makeCurrent()
-
-def on_git_merge_request(info, request):
-    state = request.DATA.get("object_attributes.state")
-    target_branch = request.DATA.get("object_attributes.target_branch")
-
-    git_branch = info.get("branch")
-    git_updater = info.get("updater")
-    git_updater_md5 = info.get("updater_md5", None)
-
-    if target_branch == git_branch:
-        reportRestIssue(
-            "{} update({}) on: {}".format(info.get("project", "n/a"), settings.get("SERVER_NAME", "unknown"), git_branch),
-            "<pre>{}</pre>".format(helpers.dictToString(request.DATA.asDict(), True)),
-            "git_updates", email_only=True)
-        update_code(git_updater, git_updater_md5, git_branch)
-
-def on_git_push_request(info, hook_request):
-    git_branch = info.get("branch")
-    git_updater = info.get("updater")
-    git_updater_md5 = info.get("updater_md5", None)
-    update_code(git_updater, git_updater_md5, git_branch)
-
-def on_git_new_release(info, request):
-    project = request.DATA.get("project.name")
-    logger.info("NEW RELEASE FOR {}".format(project))
-    product = Product.objects.filter(name=project).last()
-    if not product:
-        logger.info("PRODUCT NOT FOUND")
+
+
+def check_resolver(entry, prefix):
+    effective_regex = re.compile(prefix + entry.regex.pattern)
+
+    # skip the admin
+    if effective_regex.pattern.startswith('^admin/'):
         return
-    tag = request.DATA.get("ref").split('/')[-1]
-    msg = request.DATA.get("message")
-    url = request.DATA.get("project.web_url")
-    if product and msg:
-        new_release(product, tag, url, msg)
-
-
-def parseGitLab(request):
-    info = objict(vendor="gitlab")
-    info.name = request.DATA.get("project.name")
-    info.kind = request.DATA.get("object_kind")
-    if "ref" in request.DATA:
-        info.branch = request.DATA.get("ref").split('/')[-1]
-    if info.kind == "merge_request":
-        info.state = request.DATA.get("object_attributes.state", None)
-        if info.state == "merged":
-            info.kind = "merged"
-    return info
-
-
-def parseGithub(request):
-    info = objict(vendor="github")
-    info.name = request.DATA.get("repository.name")
-    info.kind = request.DATA.getHeader("HTTP_X_GITHUB_EVENT")
-    if "ref" in request.DATA:
-        info.branch = request.DATA.get("ref").split('/')[-1]
-    logger.info("github request", info)
-    return info
-
-
-def getProjectForBranch(proj_info, branch):
-    if proj_info is None:
-        return None
-    if type(proj_info) is list:
-        for pi in proj_info:
-            if pi["branch"] == branch:
-                return pi
-        return None
-    if project_info["branch"] == branch:
-        return proj_info
-    return None
+    #print dir(entry)
+    description = (getattr(entry, 'name', None) or effective_regex.pattern)
 
+    kwargs_provided = set(['request'] + list(getattr(entry, 'default_args', {}).keys()))
+    #print kwargs_provided
+    kwargs_provided.update(list(effective_regex.groupindex.keys()))
+    callback = unwrap_and_compare(kwargs_provided, entry.callback, description)
+
+    url_request = {"url":description, "methods":{}, "args": list(effective_regex.groupindex.keys())}
+    if hasattr(entry, 'default_args'):
+        dargs = getattr(entry, 'default_args', {})
+        if "__MODULE" in dargs:
+            url_request["module"] = dargs["__MODULE"].__name__
+            method_patterns = dargs["__MODULE"].urlpattern_methods
+            if entry.regex.pattern + "__GET" in method_patterns:
+                url_request["methods"]["get"] = {"callback": method_patterns[entry.regex.pattern+ "__GET"]}
+            if entry.regex.pattern + "__POST" in method_patterns:
+                url_request["methods"]["post"] = {"callback": method_patterns[entry.regex.pattern+ "__POST"]}
+            if entry.regex.pattern + "__DELETE" in method_patterns:
+                url_request["methods"]["delete"] = {"callback": method_patterns[entry.regex.pattern+ "__DELETE"]}
+            if entry.regex.pattern + "__PUT" in method_patterns:
+                url_request["methods"]["put"] = {"callback": method_patterns[entry.regex.pattern+ "__PUT"]}
+    if "module" not in url_request and callback:
+        url_request["module"] = callback.__module__
+    url_request["callback"] = callback
+
+
+    #print dir(callback)
+    return url_request
+
+
+def show_urls(urllist, apis, filter=None, prefix=''):
+    for entry in urllist:
+        api = check_resolver(entry, prefix)
+        if api:
+            api["url"] = api["url"].replace("^", "").replace("$", "")
+            if (filter and api["url"].startswith(filter)) or filter is None:
+                if api["callback"].__doc__:
+                    api["doc"] = api["callback"].__doc__
+                else:
+                    api["doc"] = None
+                apis.append(api)
+
+        if hasattr(entry, 'url_patterns'):
+            show_urls(entry.url_patterns, apis, filter, prefix + entry.regex.pattern)
+
+def sanatizeUrl(url):
+    return re.sub(r'\(\?P<(.*?)>.*?\)',r'{\1}',url)
+
+def parseDoc(api, graphs):
+    """
+    did regex, this approached seems to work better
+    """
+    doc = {"params":{}, "graphs":"", "summary":"", "issues":"", "returns":""}
+
+    key = None
+    subkey = None
+
+    for line in api["doc"].split("\n"):
+        linestr = line.strip()
+        if linestr.startswith('|'):
+            linestr = linestr[1:].strip()
+            line = line.strip()[1:]
+        lower_line = linestr.lower()
+        if lower_line.startswith("parameter:") or lower_line.startswith("param:"):
+            name = line[line.find(':')+1:line.find('=')].strip()
+            info = line[line.find('=')+1:]
+            doc["params"][name] = info
+            key = "params"
+            subkey = name
+        elif lower_line.startswith("return:"):
+            doc["returns"] = line[line.find(':')+1:].strip()
+            key = "summary"
+            subkey = None
+        elif lower_line.startswith("issues:"):
+            doc["issues"] = line[line.find(':')+1:].strip()
+            key = "issues"
+            subkey = None
+        elif lower_line.startswith("graphs:"):
+            doc["graphs"] = line[line.find(':')+1:].strip()
+            key = "graphs"
+            subkey = None
+        elif key and subkey:
+            doc[key][subkey] = "{0}\n{1}".format(doc[key][subkey], line.strip())
+        elif key:
+            doc[key] = "{0}\n{1}".format(doc[key], line.strip())
+    doc["summary"] = doc["summary"].strip()
+
+    if False: # doc["graphs"]
+        graph_names = []
+        fields = doc["graphs"].split('=')
+        # print fields
+        key = None
+        value = None
+        while len(fields):
+            val = fields.pop(0)
+            vals = val.strip()
+            if vals.endswith("_graph"):
+                epos = max(val.rfind(' '), val.rfind('\n'))
+                nkey = val[epos:].strip()
+                if epos > 0:
+                    if value:
+                        value = "{0}={1}".format(value, val[:epos].strip())
+                    else:
+                        value = val[:epos].strip()
+
+                if key and value:
+                    if key not in graphs:
+                        graphs[key] = value
+                    graph_names.append(key)
+                key = nkey
+            elif key:
+                value = "{0}={1}".format(value, val)
+        if key and value:
+            if key not in graphs:
+                graphs[key] = value
+            graph_names.append(key)
+
+        if "_graph" in doc["graphs"]:
+            words = doc["graphs"].split()
+            for word in words:
+                if word.strip().endswith("_graph"):
+                    graph_names.append(word.strip())
+        doc["graphs"] = graph_names
+    elif "_graph" in doc["returns"]:
+        if "_graph" in doc["returns"]:
+            graph_names = []
+            words = doc["returns"].split()
+            for word in words:
+                if word.strip().endswith("_graph"):
+                    graph_names.append(word.strip())
+            doc["graphs"] = graph_names
 
-@urlPOST (r'^hooks/git_update$')
-def on_git_hook(request):
-    sec_key = request.DATA.get("token")
-    git_key = settings.get("GIT_KEY", "hookswhat")
-    is_gitlab = True
-    hook_request = None
-    req_key = request.DATA.getHeader("HTTP_X_GITLAB_TOKEN")
-    if req_key is not None:
-        logger.info("GITLAB Detected")
-        hook_request = parseGitLab(request)
-    else:
-        req_key = request.DATA.getHeader("HTTP_X_HUB_SIGNATURE_256")
-        if req_key is not None:
-            is_gitlab = False
-            logger.info("GITHUB Detected")
-            hook_request = parseGithub(request)    
-
-    if sec_key != git_key:
-        if req_key is None:
-            logger.warning("NO TOKEN")
-            logger.warning(request.META)
-            return restPermissionDenied(request)
-
-    git_projects = settings.get("GIT_PROJECTS", None)
-
-    if hook_request.name not in git_projects:
-        return restStatus(request, False, error="no config for project")
-
-    proj_info = getProjectForBranch(git_projects.get(hook_request.name), hook_request.branch)
-    if proj_info is None:
-        logger.info("no branch for project", hook_request)
-        return restStatus(request, False, error="no branch for project")
-
-    if hook_request.kind == "push":
-        on_git_push_request(proj_info, hook_request)
-
-    # kind = request.DATA.get("object_kind")
-    # project = request.DATA.get("project.name")
-
-    # git_projects = settings.get("GIT_PROJECTS", None)
-    # if git_projects and project in git_projects:
-    #     proj_info = git_projects.get(project)
-    #     # now lets handle different kinds
-    #     if kind == "merge_request":
-    #         # now check the state
-    #         state = request.DATA.get("object_attributes.state", None)
-    #         if state != "merged":
-    #             return restStatus(request, True)
-    #         if type(proj_info) is list:
-    #             for info in proj_info:
-    #                 info["project"] = project
-    #                 on_git_merge_request(info, request)
-    #         else:
-    #             on_git_merge_request(proj_info, request)
-    #     elif kind == "push":
-    #         if type(proj_info) is list:
-    #             for info in proj_info:
-    #                 info["project"] = project
-    #                 on_git_push_request(info, request)
-    #         else:
-    #             proj_info["project"] = project
-    #             on_git_push_request(proj_info, request)
-    #     elif kind == "tag_push":
-    #         on_git_new_release(proj_info, request)
-    # elif kind == "tag_push":
-    #     proj_info = git_projects.get(project)
-    #     on_git_new_release(proj_info, request)
-    # else:
-    #     helpers.log_print("No Config for Project {}".format(project))
-    return restStatus(request, True)
+    return doc
+
+import json
+def dumpGraphs(module_name, graphs):
+    if module_name not in sys.modules:
+        print("MODULE NOT LOADED.. loading")
+        return
+    module = sys.modules[module_name]
+    for name in module.__dict__:
+        # if "getMyself" in name:
+        #     print "+++++++++++++++++"
+        #     func = getattr(module, name)
+        #     print func.__doc__
+        #     print dir(func)
+        #     print func.__dict__
+
+        if "_graph" in name:
+            graph = getattr(module, name)
+            # print graph.keys()
+            dc = {}
+            if "fields" in graph:
+                fields = graph["fields"]
+                graph_doc = {}
+                for f in fields:
+                    if type(f) is tuple:
+                        o = f[0]
+                        f = f[1]
+                        if len(f):
+                            if "." in o:
+                                o = o[:o.rfind('.')]
+                                f = "{0}.{1}".format(o, f)
+                    if "." in f:
+                        levels = f.split('.')
+                        current = graph_doc
+                        field = levels[-1]
+                        for o in levels:
+                            if o is field:
+                                continue
+                            if o not in current:
+                                current[o] = {}
+                            elif type(current[o]) is str:
+                                current[o] = {}
+                            current = current[o]
+                        current[field] = ''
+                    else:
+                        graph_doc[f] = ''
+                graphs[name] = json.dumps(graph_doc)
+
+
+def getRestApis(patterns, sanatize_urls=True):
+    apis = []
+    graphs = {}
+    modules = []
+    show_urls(patterns, apis)
+    if sanatize_urls:
+        old_apis = apis
+        apis = []
+        for api in old_apis:
+            if len(api["methods"]):
+                for method in api["methods"]:
+                    a = {"method":method}
+                    m = api["methods"][method]
+                    module_name = m["callback"].__module__
+                    if module_name not in modules:
+                        dumpGraphs(module_name, graphs)
+                        modules.append(module_name)
+
+                    a["url"] = api["url"]
+                    # print a["url"]
+
+                    # # print m["callback"].func_doc
+                    # if not m["callback"].__doc__:
+                    #     print dir(m["callback"].__code__)
+                    #     print m["callback"].__code__.__doc__
+                    if m["callback"].__doc__:
+                        # print "\tyes we have docs"
+                        a["doc"] = m["callback"].__doc__
+                        a["doc"] = parseDoc(a, graphs)
+                        if a["doc"] is None or len(a["doc"]) == 0:
+                            a["doc"] = ""
+                        apis.append({
+                            "module":api["module"].replace(".rpc", ""),
+                            "method":method,
+                            "url":sanatizeUrl(a["url"]),
+                            "doc":a["doc"]
+                        })
+                    else:
+                        apis.append({
+                            "module":api["module"].replace(".rpc", ""),
+                            "method":method,
+                            "url":sanatizeUrl(a["url"]),
+                            "doc":""
+                        })
+                        # print "\tno docs"
+            else:
+                # print api
+                if api["doc"] is None or len(api["doc"]) == 0:
+                    continue
+                api["doc"] = parseDoc(api, graphs)
+                apis.append({
+                    "module":api["module"].replace(".rpc", ""),
+                    "method":"*",
+                    "url":sanatizeUrl(api["url"]),
+                    "doc":api["doc"]
+                    })
+    return apis, graphs
```

### Comparing `django_restit-4.0.2/pyproject.toml` & `django_restit-4.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-restit"
-version = "4.0.2"
+version = "4.0.4"
 description = "A Rest Framework for DJANGO"
 authors = ["Ian Starnes <ians@311labs.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     {include = "account"},
@@ -49,26 +49,23 @@
 redis = "^3.0.1"
 django-redis-cache = "^3.0.1"
 django-redis-sessions = "^0.6.2"
 
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
-bumpver = "^2023.1124"
 
 [tool.bumpver]
-current_version = "4.0.0"
+current_version = "4.0.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = true
 push = true
 
-[tool.bumpver.file_patterns]
-"pyproject.toml" = [
-    'current_version = "{version}"',
-]
+[tool.poetry_bumpversion.file."rest/__init__.py"]
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_restit-4.0.2/rest/README.md` & `django_restit-4.0.4/rest/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/arc4.py` & `django_restit-4.0.4/rest/arc4.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/crypto/aes.py` & `django_restit-4.0.4/rest/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/crypto/privpub.py` & `django_restit-4.0.4/rest/crypto/privpub.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/crypto/util.py` & `django_restit-4.0.4/rest/crypto/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/datem.py` & `django_restit-4.0.4/rest/datem.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/decorators.py` & `django_restit-4.0.4/rest/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 import metrics
 import incident
 
 from datetime import datetime
 from auditlog.models import PersistentLog
 
 import importlib
+import pkgutil
 import threading
 import traceback
 
 REST_METRICS = settings.get("REST_METRICS", False)
 REST_METRICS_BY_ENDPOINT = settings.get("REST_METRICS_BY_ENDPOINT", False)
 REST_METRICS_IGNORE = settings.get("REST_METRICS_IGNORE", [])
+REST_MODULE_NAME = settings.get("REST_MODULE_NAME", "rpc")
 
 
 # background task (no return)
 def rest_async(func):
     """
     Execute the function asynchronously in a separate thread
     """
@@ -126,14 +128,20 @@
     key = pattern + '__' + method
     if key in module.urlpattern_methods:
         return rest_error_catcher(module.urlpattern_methods[key], request, *args, **kwargs)
     # print module.urlpattern_methods
     return restStatus(request, False, error="endpoint not found", error_code=404)
 
 
+def _load_module(mod):
+    if pkgutil.find_loader(mod) is not None:
+        return importlib.import_module(mod)
+    return None
+
+
 def _url_method(pattern, method=None, *args, **kwargs):
     """
     Register a view handler for a specific HTTP method
     """
     caller_filename = sys._getframe(2).f_code.co_filename
     module = None
     for m in list(sys.modules.values()):
@@ -146,21 +154,25 @@
         if module:
             rpc_root_module = module
             if module.__name__.count('.') > 1:
                 # this means we are not in root
                 # print module.__name__
                 root_name = module.__name__.split('.')[0]
                 # print "importing {0}.rpc".format(root_name)
-                rpc_root_module = importlib.import_module(root_name + ".rpc")
+                rmodule = _load_module(f"{root_name}.{REST_MODULE_NAME}")
+                if rmodule is not None:
+                    rpc_root_module = rmodule
             # print "{0}/{1}".format(rpc_root_module.__name__, pattern)
-            elif not module.__name__.endswith(".rpc") and module.__name__.count('.'):
+            elif not module.__name__.endswith(f".{REST_MODULE_NAME}") and module.__name__.count('.'):
                 # print module.__name__
                 root_name = module.__name__.split('.')[0]
                 # print "importing {0}.rpc".format(root_name)
-                rpc_root_module = importlib.import_module(root_name + ".rpc")
+                rmodule = _load_module(f"{root_name}.{REST_MODULE_NAME}")
+                if rmodule is not None:
+                    rpc_root_module = rmodule
             lmethod = method
             if lmethod is None:
                 lmethod = "ALL"
             if 'urlpatterns' not in rpc_root_module.__dict__:
                 rpc_root_module.urlpatterns = []
             if lmethod and 'urlpattern_methods' not in rpc_root_module.__dict__:
                 rpc_root_module.urlpattern_methods = {}
```

### Comparing `django_restit-4.0.2/rest/encryption.py` & `django_restit-4.0.4/rest/encryption.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/extra/json_metadata.py` & `django_restit-4.0.4/rest/extra/json_metadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/fields.py` & `django_restit-4.0.4/rest/fields.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/forms.py` & `django_restit-4.0.4/rest/forms.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/helpers.py` & `django_restit-4.0.4/rest/helpers.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/jwtoken.py` & `django_restit-4.0.4/rest/jwtoken.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/log.py` & `django_restit-4.0.4/rest/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,36 +8,27 @@
 import logging
 import os
 import errno
 import sys
 import threading
 import time
 import traceback
+from .settings_helper import settings
 
+LOG_FOLDER = settings.LOG_FOLDER
+if LOG_FOLDER is None:
+    LOG_FOLDER = os.path.join(settings.BASE_DIR, "var", "logs")
 
 COLOR_LOGS = True
 MAX_LOG_SIZE = 10485760
 
 # number of bytes to leave after rotating/truncating a file
 ROTATE_LEFT_OVER_BYTES = 50000
 LOG_COUNT = 3
 
-REST_FOLDER = os.path.realpath(__file__)
-# now work backwards until we find folder with "django"
-ROOT = None
-CUR_FOLDER = REST_FOLDER
-while ROOT is None:
-    if os.path.exists(os.path.join(CUR_FOLDER, "django")):
-        ROOT = CUR_FOLDER
-    else:
-        CUR_FOLDER = os.path.dirname(CUR_FOLDER)
-
-VAR_FOLDER = os.path.join(ROOT, "var", "logs")
-PATH = VAR_FOLDER
-
 
 class RestLogManager(object):
     def __init__(self):
         self.lock = threading.RLock()
         self.master = None
         self.loggers = {}
         self.streams = {}
@@ -117,16 +108,16 @@
         master = None
         if errors_to_root:
             master = LOG_MANAGER.master
         rest_logger = RestLogger(name, filename, level, master, max_bytes=max_bytes)
         LOG_MANAGER.loggers[name] = rest_logger
         if set_master:
             LOG_MANAGER.master = rest_logger
-        if not os.path.exists(VAR_FOLDER):
-            mkdir(VAR_FOLDER)
+        if not os.path.exists(LOG_FOLDER):
+            mkdir(LOG_FOLDER)
     except Exception as err:
         print((str(err)))
         print((str(traceback.format_exc())))
     LOG_MANAGER.release()
     return rest_logger
 
 
@@ -156,15 +147,15 @@
         if filename:
             if filename not in ["stdout", "stderr"]:
                 self.is_file = True
                 # lets put it in the var path
                 if not os.path.exists(self.filename):
                     path, fname = os.path.split(filename)
                     if not len(path):
-                        self.filename = os.path.join(VAR_FOLDER, filename)
+                        self.filename = os.path.join(LOG_FOLDER, filename)
         self.max_bytes = max_bytes
         self.stream = None
         self.is_stdout = False
         self.is_stderr = False
         self.lock = threading.RLock()
         self.open()
```

### Comparing `django_restit-4.0.2/rest/mail.py` & `django_restit-4.0.4/rest/mail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/mailman.py` & `django_restit-4.0.4/rest/mailman.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/middleware/cors.py` & `django_restit-4.0.4/rest/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/middleware/db_router.py` & `django_restit-4.0.4/rest/middleware/db_router.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/middleware/jwt.py` & `django_restit-4.0.4/rest/middleware/jwt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/middleware/request.py` & `django_restit-4.0.4/rest/middleware/request.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/middleware/session.py` & `django_restit-4.0.4/rest/middleware/session.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/middleware/session_store.py` & `django_restit-4.0.4/rest/middleware/session_store.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/models.py` & `django_restit-4.0.4/rest/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/regexes.yaml` & `django_restit-4.0.4/rest/regexes.yaml`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/requestex.py` & `django_restit-4.0.4/rest/requestex.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/rpc.py` & `django_restit-4.0.4/rest/rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,21 @@
 
 
 @url(r'^version$')
 def on_get_version(request):
     return views.restStatus(request, True, {"data": version.VERSION})
 
 
+@url(r'^versions$')
+def on_get_version(request):
+    from rest import __version__ as restit_version
+    versions = dict(project=version.VERSION, restit=restit_version)
+    return views.restStatus(request, True, {"data": versions})
+
+
 @url(r'^joke$')
 def on_get_joke(request):
     return views.restGet(request, {"joke": joke.getRandomJoke()})
 
 
 def getTcpEstablishedCount():
     return len(getTcpEstablished())
```

### Comparing `django_restit-4.0.2/rest/search.py` & `django_restit-4.0.4/rest/search.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/serializers/collection.py` & `django_restit-4.0.4/rest/serializers/collection.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/serializers/csv.py` & `django_restit-4.0.4/rest/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/serializers/excel.py` & `django_restit-4.0.4/rest/serializers/excel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/serializers/json.py` & `django_restit-4.0.4/rest/serializers/json.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/serializers/legacy.py` & `django_restit-4.0.4/rest/serializers/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/serializers/model.py` & `django_restit-4.0.4/rest/serializers/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/serializers/response.py` & `django_restit-4.0.4/rest/serializers/response.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/serializers/util.py` & `django_restit-4.0.4/rest/serializers/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/settings_helper.py` & `django_restit-4.0.4/rest/settings_helper.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/static/lib/jquery.js` & `django_restit-4.0.4/rest/static/lib/jquery.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/templates/email/error.html` & `django_restit-4.0.4/rest/templates/email/error.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/templates/rest_docs.html` & `django_restit-4.0.4/rest/templates/rest_docs.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/templates/rest_html.html` & `django_restit-4.0.4/rest/templates/rest_html.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/ua.py` & `django_restit-4.0.4/rest/ua.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/uberdict.py` & `django_restit-4.0.4/rest/uberdict.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/rest/urls.py` & `django_restit-4.0.4/rest/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,17 @@
     re_path('offline', views.__offline)
 ]
 
 
 def load_app(app, root_module=None):
     module = None
     try:
-        module = loadModule(app + '.rpc')
+        module = loadModule(f"{app}.rpc")
+        if module is None:
+            module = loadModule(f"{app}.rurl")
     except ImportError as err:
         print("**** failed to load {0}.rpc! ****".format(app))
         print("**** missing dependencies ****")
         print("**** {0} ****".format(err))
     except SyntaxError:
         print("\t{0}: fail".format(app))
         print("Exception in user code:")
```

### Comparing `django_restit-4.0.2/rest/views.py` & `django_restit-4.0.4/rest/views.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/sessionlog/migrations/0001_initial.py` & `django_restit-4.0.4/sessionlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/sessionlog/models.py` & `django_restit-4.0.4/sessionlog/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/taskqueue/README.md` & `django_restit-4.0.4/taskqueue/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/taskqueue/migrations/0001_initial.py` & `django_restit-4.0.4/taskqueue/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/taskqueue/models.py` & `django_restit-4.0.4/taskqueue/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/taskqueue/periodic.py` & `django_restit-4.0.4/taskqueue/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/taskqueue/rpc.py` & `django_restit-4.0.4/taskqueue/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/taskqueue/tq.py` & `django_restit-4.0.4/taskqueue/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/taskqueue/transports/email.py` & `django_restit-4.0.4/taskqueue/transports/email.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/taskqueue/transports/http.py` & `django_restit-4.0.4/taskqueue/transports/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/taskqueue/transports/s3.py` & `django_restit-4.0.4/taskqueue/transports/s3.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/taskqueue/transports/sftp.py` & `django_restit-4.0.4/taskqueue/transports/sftp.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/taskqueue/worker.py` & `django_restit-4.0.4/taskqueue/worker.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/telephony/migrations/0001_initial.py` & `django_restit-4.0.4/telephony/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/telephony/models.py` & `django_restit-4.0.4/telephony/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/telephony/phone_util.py` & `django_restit-4.0.4/telephony/phone_util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/telephony/rpc.py` & `django_restit-4.0.4/telephony/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/ws4redis/README.md` & `django_restit-4.0.4/ws4redis/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/ws4redis/client.py` & `django_restit-4.0.4/ws4redis/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/ws4redis/connection.py` & `django_restit-4.0.4/ws4redis/connection.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/ws4redis/exceptions.py` & `django_restit-4.0.4/ws4redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/ws4redis/redis.py` & `django_restit-4.0.4/ws4redis/redis.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/ws4redis/servers/base.py` & `django_restit-4.0.4/ws4redis/servers/base.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/ws4redis/servers/django.py` & `django_restit-4.0.4/ws4redis/servers/django.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/ws4redis/servers/uwsgi.py` & `django_restit-4.0.4/ws4redis/servers/uwsgi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/ws4redis/settings.py` & `django_restit-4.0.4/ws4redis/settings.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/ws4redis/utf8validator.py` & `django_restit-4.0.4/ws4redis/utf8validator.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/ws4redis/websocket.py` & `django_restit-4.0.4/ws4redis/websocket.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.2/PKG-INFO` & `django_restit-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-restit
-Version: 4.0.2
+Version: 4.0.4
 Summary: A Rest Framework for DJANGO
 License: MIT
 Author: Ian Starnes
 Author-email: ians@311labs.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

