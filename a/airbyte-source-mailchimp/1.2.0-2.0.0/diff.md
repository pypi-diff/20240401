# Comparing `tmp/airbyte_source_mailchimp-1.2.0.tar.gz` & `tmp/airbyte_source_mailchimp-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_mailchimp-1.2.0.tar", max compression
+gzip compressed data, was "airbyte_source_mailchimp-2.0.0.tar", max compression
```

## Comparing `airbyte_source_mailchimp-1.2.0.tar` & `airbyte_source_mailchimp-2.0.0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
--rw-r--r--   0        0        0     4550 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/README.md
--rw-r--r--   0        0        0      782 2024-03-28 18:30:48.444664 airbyte_source_mailchimp-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       67 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/__init__.py
--rw-r--r--   0        0        0      239 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/run.py
--rw-r--r--   0        0        0     4542 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/automations.json
--rw-r--r--   0        0        0    29465 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/campaigns.json
--rw-r--r--   0        0        0     1987 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/email_activity.json
--rw-r--r--   0        0        0      383 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/interest_categories.json
--rw-r--r--   0        0        0      455 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/interests.json
--rw-r--r--   0        0        0     4162 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/list_members.json
--rw-r--r--   0        0        0    12237 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/lists.json
--rw-r--r--   0        0        0    19375 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/reports.json
--rw-r--r--   0        0        0     2720 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/segment_members.json
--rw-r--r--   0        0        0     1333 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/segments.json
--rw-r--r--   0        0        0      930 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/addressMergeSegment.json
--rw-r--r--   0        0        0     1085 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/addressZipWithinSegment.json
--rw-r--r--   0        0        0     1054 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/aimSegment.json
--rw-r--r--   0        0        0     1113 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/automationSegment.json
--rw-r--r--   0        0        0      883 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/birthdayMergeSegment.json
--rw-r--r--   0        0        0      852 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/campaignPollSegment.json
--rw-r--r--   0        0        0      263 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/campaignStatus.json
--rw-r--r--   0        0        0      396 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/campaignType.json
--rw-r--r--   0        0        0     1070 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/conversationSegment.json
--rw-r--r--   0        0        0     1021 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/countryStateSegment.json
--rw-r--r--   0        0        0      897 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/dateMergeSegment.json
--rw-r--r--   0        0        0     1510 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/dateSegment.json
--rw-r--r--   0        0        0      908 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/dropdownRadioMergeSegment.json
--rw-r--r--   0        0        0     1103 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/ecommCategorySegment.json
--rw-r--r--   0        0        0     1283 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/ecommNumberSegment.json
--rw-r--r--   0        0        0      741 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/ecommPurchasedSegment.json
--rw-r--r--   0        0        0      923 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/ecommSpentSegment.json
--rw-r--r--   0        0        0      856 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/ecommStoreSegment.json
--rw-r--r--   0        0        0      958 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/emailClientSegment.json
--rw-r--r--   0        0        0     1039 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/emailSegment.json
--rw-r--r--   0        0        0      924 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/fuzzySegment.json
--rw-r--r--   0        0        0     1455 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/geoInSegment.json
--rw-r--r--   0        0        0      964 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/goalActivitySegment.json
--rw-r--r--   0        0        0      971 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/goalTimestampSegment.json
--rw-r--r--   0        0        0     1096 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/interestSegment.json
--rw-r--r--   0        0        0     1039 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/ipGeoInZipSegment.json
--rw-r--r--   0        0        0      856 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/languageSegment.json
--rw-r--r--   0        0        0      939 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/memberRatingSegment.json
--rw-r--r--   0        0        0      823 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/newSubscribers.json
--rw-r--r--   0        0        0      874 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/predictedAgeSegment.json
--rw-r--r--   0        0        0      862 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/predictedGenderSegment.json
--rw-r--r--   0        0        0     2773 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/segmentCondition.json
--rw-r--r--   0        0        0      917 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/segmentationOptions.json
--rw-r--r--   0        0        0      840 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/signupSourceSegment.json
--rw-r--r--   0        0        0      922 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/socialAgeSegment.json
--rw-r--r--   0        0        0      941 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/socialGenderSegment.json
--rw-r--r--   0        0        0      988 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/socialInfluenceSegment.json
--rw-r--r--   0        0        0     1023 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/socialNetworkFollowSegment.json
--rw-r--r--   0        0        0     1177 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/socialNetworkSegment.json
--rw-r--r--   0        0        0      894 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/staticSegment.json
--rw-r--r--   0        0        0     1083 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/surveyMonkeySegment.json
--rw-r--r--   0        0        0     1127 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/textOrNumberMergeSegment.json
--rw-r--r--   0        0        0      751 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/unknownSegment.json
--rw-r--r--   0        0        0      639 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/vipSegment.json
--rw-r--r--   0        0        0      896 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/zipSegment.json
--rw-r--r--   0        0        0      265 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/tags.json
--rw-r--r--   0        0        0      782 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/unsubscribes.json
--rw-r--r--   0        0        0     6499 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/source.py
--rw-r--r--   0        0        0     4079 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/spec.json
--rw-r--r--   0        0        0    22036 2024-03-28 12:02:50.000000 airbyte_source_mailchimp-1.2.0/source_mailchimp/streams.py
--rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 airbyte_source_mailchimp-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4550 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/README.md
+-rw-r--r--   0        0        0      781 2024-04-01 13:33:39.205556 airbyte_source_mailchimp-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       67 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/__init__.py
+-rw-r--r--   0        0        0     2528 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/components.py
+-rw-r--r--   0        0        0     3724 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/config_migrations.py
+-rw-r--r--   0        0        0    11660 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/manifest.yaml
+-rw-r--r--   0        0        0      356 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/run.py
+-rw-r--r--   0        0        0     4542 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/automations.json
+-rw-r--r--   0        0        0    29465 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/campaigns.json
+-rw-r--r--   0        0        0     1987 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/email_activity.json
+-rw-r--r--   0        0        0      383 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/interest_categories.json
+-rw-r--r--   0        0        0      455 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/interests.json
+-rw-r--r--   0        0        0     4162 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/list_members.json
+-rw-r--r--   0        0        0    12237 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/lists.json
+-rw-r--r--   0        0        0    19375 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/reports.json
+-rw-r--r--   0        0        0     2720 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/segment_members.json
+-rw-r--r--   0        0        0     1333 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/segments.json
+-rw-r--r--   0        0        0      930 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/addressMergeSegment.json
+-rw-r--r--   0        0        0     1085 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/addressZipWithinSegment.json
+-rw-r--r--   0        0        0     1054 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/aimSegment.json
+-rw-r--r--   0        0        0     1113 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/automationSegment.json
+-rw-r--r--   0        0        0      883 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/birthdayMergeSegment.json
+-rw-r--r--   0        0        0      852 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/campaignPollSegment.json
+-rw-r--r--   0        0        0      263 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/campaignStatus.json
+-rw-r--r--   0        0        0      396 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/campaignType.json
+-rw-r--r--   0        0        0     1070 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/conversationSegment.json
+-rw-r--r--   0        0        0     1021 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/countryStateSegment.json
+-rw-r--r--   0        0        0      897 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/dateMergeSegment.json
+-rw-r--r--   0        0        0     1510 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/dateSegment.json
+-rw-r--r--   0        0        0      908 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/dropdownRadioMergeSegment.json
+-rw-r--r--   0        0        0     1103 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/ecommCategorySegment.json
+-rw-r--r--   0        0        0     1283 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/ecommNumberSegment.json
+-rw-r--r--   0        0        0      741 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/ecommPurchasedSegment.json
+-rw-r--r--   0        0        0      923 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/ecommSpentSegment.json
+-rw-r--r--   0        0        0      856 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/ecommStoreSegment.json
+-rw-r--r--   0        0        0      958 2024-04-01 13:31:06.721465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/emailClientSegment.json
+-rw-r--r--   0        0        0     1039 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/emailSegment.json
+-rw-r--r--   0        0        0      924 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/fuzzySegment.json
+-rw-r--r--   0        0        0     1455 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/geoInSegment.json
+-rw-r--r--   0        0        0      964 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/goalActivitySegment.json
+-rw-r--r--   0        0        0      971 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/goalTimestampSegment.json
+-rw-r--r--   0        0        0     1096 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/interestSegment.json
+-rw-r--r--   0        0        0     1039 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/ipGeoInZipSegment.json
+-rw-r--r--   0        0        0      856 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/languageSegment.json
+-rw-r--r--   0        0        0      939 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/memberRatingSegment.json
+-rw-r--r--   0        0        0      823 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/newSubscribers.json
+-rw-r--r--   0        0        0      874 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/predictedAgeSegment.json
+-rw-r--r--   0        0        0      862 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/predictedGenderSegment.json
+-rw-r--r--   0        0        0     2773 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/segmentCondition.json
+-rw-r--r--   0        0        0      917 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/segmentationOptions.json
+-rw-r--r--   0        0        0      840 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/signupSourceSegment.json
+-rw-r--r--   0        0        0      922 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/socialAgeSegment.json
+-rw-r--r--   0        0        0      941 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/socialGenderSegment.json
+-rw-r--r--   0        0        0      988 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/socialInfluenceSegment.json
+-rw-r--r--   0        0        0     1023 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/socialNetworkFollowSegment.json
+-rw-r--r--   0        0        0     1177 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/socialNetworkSegment.json
+-rw-r--r--   0        0        0      894 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/staticSegment.json
+-rw-r--r--   0        0        0     1083 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/surveyMonkeySegment.json
+-rw-r--r--   0        0        0     1127 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/textOrNumberMergeSegment.json
+-rw-r--r--   0        0        0      751 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/unknownSegment.json
+-rw-r--r--   0        0        0      639 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/vipSegment.json
+-rw-r--r--   0        0        0      896 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/zipSegment.json
+-rw-r--r--   0        0        0      265 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/tags.json
+-rw-r--r--   0        0        0      782 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/unsubscribes.json
+-rw-r--r--   0        0        0      287 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/source.py
+-rw-r--r--   0        0        0     4138 2024-04-01 13:31:06.725465 airbyte_source_mailchimp-2.0.0/source_mailchimp/spec.json
+-rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 airbyte_source_mailchimp-2.0.0/PKG-INFO
```

### Comparing `airbyte_source_mailchimp-1.2.0/README.md` & `airbyte_source_mailchimp-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/pyproject.toml` & `airbyte_source_mailchimp-2.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.2.0"
+version = "2.0.0"
 name = "airbyte-source-mailchimp"
 description = "Source implementation for Mailchimp."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -26,9 +26,9 @@
 pytest = "==6.2.5"
 
 [tool.poetry.scripts]
 source-mailchimp = "source_mailchimp.run:run"
 
 [tool.poetry.group.dev.dependencies]
 pytest-mock = "^3.6.1"
-responses = "^0.19.0"
 requests-mock = "^1.9.3"
+freezegun = "^1.4.0"
```

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/automations.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/automations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/campaigns.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/email_activity.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/email_activity.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/list_members.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/list_members.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/lists.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/lists.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/reports.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/reports.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/segment_members.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/segment_members.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/segments.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/segments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/addressMergeSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/addressMergeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/addressZipWithinSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/addressZipWithinSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/aimSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/aimSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/automationSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/automationSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/birthdayMergeSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/birthdayMergeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/campaignPollSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/campaignPollSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/conversationSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/conversationSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/countryStateSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/countryStateSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/dateMergeSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/dateMergeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/dateSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/dateSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/dropdownRadioMergeSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/dropdownRadioMergeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/ecommCategorySegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/ecommCategorySegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/ecommNumberSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/ecommNumberSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/ecommPurchasedSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/ecommPurchasedSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/ecommSpentSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/ecommSpentSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/ecommStoreSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/ecommStoreSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/emailClientSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/emailClientSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/emailSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/emailSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/fuzzySegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/fuzzySegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/geoInSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/geoInSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/goalActivitySegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/goalActivitySegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/goalTimestampSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/goalTimestampSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/interestSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/interestSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/ipGeoInZipSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/ipGeoInZipSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/languageSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/languageSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/memberRatingSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/memberRatingSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/newSubscribers.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/newSubscribers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/predictedAgeSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/predictedAgeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/predictedGenderSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/predictedGenderSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/segmentCondition.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/segmentCondition.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/segmentationOptions.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/segmentationOptions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/signupSourceSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/signupSourceSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/socialAgeSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/socialAgeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/socialGenderSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/socialGenderSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/socialInfluenceSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/socialInfluenceSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/socialNetworkFollowSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/socialNetworkFollowSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/socialNetworkSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/socialNetworkSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/staticSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/staticSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/surveyMonkeySegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/surveyMonkeySegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/textOrNumberMergeSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/textOrNumberMergeSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/unknownSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/unknownSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/vipSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/vipSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/shared/zipSegment.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/shared/zipSegment.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/schemas/unsubscribes.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/schemas/unsubscribes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_mailchimp-1.2.0/source_mailchimp/spec.json` & `airbyte_source_mailchimp-2.0.0/source_mailchimp/spec.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930555555555557%*

 * *Differences: {"'connectionSpecification'": "{'properties': {'data_center': OrderedDict([('title', "*

 * *                              "'DataCenter'), ('description', 'Technical fields used to identify "*

 * *                              "datacenter to send request to'), ('type', 'string'), "*

 * *                              "('airbyte_hidden', True)]), delete: ['campaign_id']}}"}*

```diff
@@ -54,19 +54,14 @@
         ],
         "predicate_value": "oauth2.0"
     },
     "connectionSpecification": {
         "$schema": "http://json-schema.org/draft-07/schema#",
         "additionalProperties": true,
         "properties": {
-            "campaign_id": {
-                "airbyte_hidden": true,
-                "title": "ID of a campaign to sync email activities",
-                "type": "string"
-            },
             "credentials": {
                 "oneOf": [
                     {
                         "properties": {
                             "access_token": {
                                 "airbyte_secret": true,
                                 "description": "An access token generated using the above client ID and secret.",
@@ -119,14 +114,20 @@
                         "title": "API Key",
                         "type": "object"
                     }
                 ],
                 "title": "Authentication",
                 "type": "object"
             },
+            "data_center": {
+                "airbyte_hidden": true,
+                "description": "Technical fields used to identify datacenter to send request to",
+                "title": "DataCenter",
+                "type": "string"
+            },
             "start_date": {
                 "description": "The date from which you want to start syncing data for Incremental streams. Only records that have been created or modified since this date will be synced. If left blank, all data will by synced.",
                 "examples": [
                     "2020-01-01T00:00:00.000Z"
                 ],
                 "format": "date-time",
                 "pattern": "^[0-9]{4}-[0-9]{2}-[0-9]{2}T[0-9]{2}:[0-9]{2}:[0-9]{2}.[0-9]{3}Z$",
```

### Comparing `airbyte_source_mailchimp-1.2.0/PKG-INFO` & `airbyte_source_mailchimp-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-mailchimp
-Version: 1.2.0
+Version: 2.0.0
 Summary: Source implementation for Mailchimp.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

