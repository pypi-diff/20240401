# Comparing `tmp/airbyte_source_surveymonkey-0.2.4.tar.gz` & `tmp/airbyte_source_surveymonkey-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_surveymonkey-0.2.4.tar", max compression
+gzip compressed data, was "airbyte_source_surveymonkey-0.3.0.tar", max compression
```

## Comparing `airbyte_source_surveymonkey-0.2.4.tar` & `airbyte_source_surveymonkey-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     4604 2024-02-12 12:17:44.000000 airbyte_source_surveymonkey-0.2.4/README.md
--rw-r--r--   0        0        0      822 2024-02-12 12:44:25.830383 airbyte_source_surveymonkey-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1146 2024-02-12 12:17:44.000000 airbyte_source_surveymonkey-0.2.4/source_surveymonkey/__init__.py
--rw-r--r--   0        0        0      248 2024-02-12 12:17:44.000000 airbyte_source_surveymonkey-0.2.4/source_surveymonkey/run.py
--rw-r--r--   0        0        0     1869 2024-02-12 12:17:44.000000 airbyte_source_surveymonkey-0.2.4/source_surveymonkey/schemas/collectors.json
--rw-r--r--   0        0        0      352 2024-02-12 12:17:44.000000 airbyte_source_surveymonkey-0.2.4/source_surveymonkey/schemas/survey_collectors.json
--rw-r--r--   0        0        0      320 2024-02-12 12:17:44.000000 airbyte_source_surveymonkey-0.2.4/source_surveymonkey/schemas/survey_ids.json
--rw-r--r--   0        0        0      447 2024-02-12 12:17:44.000000 airbyte_source_surveymonkey-0.2.4/source_surveymonkey/schemas/survey_pages.json
--rw-r--r--   0        0        0     2700 2024-02-12 12:17:44.000000 airbyte_source_surveymonkey-0.2.4/source_surveymonkey/schemas/survey_questions.json
--rw-r--r--   0        0        0     2515 2024-02-12 12:17:44.000000 airbyte_source_surveymonkey-0.2.4/source_surveymonkey/schemas/survey_responses.json
--rw-r--r--   0        0        0     1791 2024-02-12 12:17:44.000000 airbyte_source_surveymonkey-0.2.4/source_surveymonkey/schemas/surveys.json
--rw-r--r--   0        0        0     4139 2024-02-12 12:17:44.000000 airbyte_source_surveymonkey-0.2.4/source_surveymonkey/source.py
--rw-r--r--   0        0        0     4280 2024-02-12 12:17:44.000000 airbyte_source_surveymonkey-0.2.4/source_surveymonkey/spec.json
--rw-r--r--   0        0        0    13532 2024-02-12 12:17:44.000000 airbyte_source_surveymonkey-0.2.4/source_surveymonkey/streams.py
--rw-r--r--   0        0        0     5393 1970-01-01 00:00:00.000000 airbyte_source_surveymonkey-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     4609 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/README.md
+-rw-r--r--   0        0        0      818 2024-04-01 21:13:51.251355 airbyte_source_surveymonkey-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1244 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/__init__.py
+-rw-r--r--   0        0        0     2164 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/components.py
+-rw-r--r--   0        0        0     2620 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/config_migrations.py
+-rw-r--r--   0        0        0    15740 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/manifest.yaml
+-rw-r--r--   0        0        0      347 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/run.py
+-rw-r--r--   0        0        0     1869 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/collectors.json
+-rw-r--r--   0        0        0      352 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/survey_collectors.json
+-rw-r--r--   0        0        0      320 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/survey_ids.json
+-rw-r--r--   0        0        0      447 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/survey_pages.json
+-rw-r--r--   0        0        0     2700 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/survey_questions.json
+-rw-r--r--   0        0        0     2515 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/survey_responses.json
+-rw-r--r--   0        0        0     1791 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/surveys.json
+-rw-r--r--   0        0        0     2344 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/source.py
+-rw-r--r--   0        0        0     8428 2024-04-01 18:40:30.000000 airbyte_source_surveymonkey-0.3.0/source_surveymonkey/streams.py
+-rw-r--r--   0        0        0     5395 1970-01-01 00:00:00.000000 airbyte_source_surveymonkey-0.3.0/PKG-INFO
```

### Comparing `airbyte_source_surveymonkey-0.2.4/README.md` & `airbyte_source_surveymonkey-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-surveymonkey spec
 poetry run source-surveymonkey check --config secrets/config.json
 poetry run source-surveymonkey discover --config secrets/config.json
-poetry run source-surveymonkey read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-surveymonkey read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

### Comparing `airbyte_source_surveymonkey-0.2.4/pyproject.toml` & `airbyte_source_surveymonkey-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.4"
+version = "0.3.0"
 name = "airbyte-source-surveymonkey"
 description = "Source implementation for Surveymonkey."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,18 +18,18 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_surveymonkey" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "==0.51.40"
+airbyte-cdk = "^0"
 vcrpy = "==4.1.1"
 urllib3 = "==1.26.18"
 
 [tool.poetry.scripts]
 source-surveymonkey = "source_surveymonkey.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
-pytest-mock = "^3.6.1"
-pytest = "^6.1"
+pytest-mock = "^3.12.0"
+pytest = "^8.0.0"
```

### Comparing `airbyte_source_surveymonkey-0.2.4/source_surveymonkey/schemas/collectors.json` & `airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/collectors.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.2.4/source_surveymonkey/schemas/survey_questions.json` & `airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/survey_questions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.2.4/source_surveymonkey/schemas/survey_responses.json` & `airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/survey_responses.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.2.4/source_surveymonkey/schemas/surveys.json` & `airbyte_source_surveymonkey-0.3.0/source_surveymonkey/schemas/surveys.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.2.4/source_surveymonkey/streams.py` & `airbyte_source_surveymonkey-0.3.0/source_surveymonkey/streams.py`

 * *Files 24% similar despite different names*

```diff
@@ -72,19 +72,17 @@
                     raise e
 
     def backoff_time(self, response: requests.Response) -> Optional[float]:
         """
         https://developer.surveymonkey.com/api/v3/#headers
         X-Ratelimit-App-Global-Minute-Remaining - Number of remaining requests app has before hitting per minute limit
         X-Ratelimit-App-Global-Minute-Reset     - Number of seconds until the rate limit remaining resets
-
         Limits: https://developer.surveymonkey.com/api/v3/#request-and-response-limits
         Max Requests Per Day - 500
         Max Requests Per Minute - 120
-
         Real limits from API response headers:
         "X-Ratelimit-App-Global-Minute-Limit": "720"
         "X-Ratelimit-App-Global-Day-Limit": "500000"
         """
         # Stop for 60 secs if less than 1 request remains before we hit minute limit
         minute_limit_remaining = response.headers.get("X-Ratelimit-App-Global-Minute-Remaining", "100")
         if int(minute_limit_remaining) <= 1:
@@ -157,24 +155,21 @@
                 yield {"survey_id": survey["id"]}
 
 
 class Surveys(SurveyIDSliceMixin, IncrementalSurveymonkeyStream):
     """
     Docs: https://developer.surveymonkey.com/api/v3/#surveys
     A source for stream slices. It does not contain useful info itself.
-
     The `surveys/id/details` endpoint contains full data about pages and questions. This data is already collected and
     gathered into array [pages] and array of arrays questions, where each inner array contains data about certain page.
     Example [[q1, q2,q3], [q4,q5]] means we have 2 pages, first page contains 3 questions q1, q2, q3, second page contains other.
-
     If we use the "normal" query, we need to query surveys/id/pages for page enumeration,
     then we need to query each page_id in every new request for details (because `pages` doesn't contain full info
     and valid only for enumeration), then for each page need to enumerate questions and get each question_id for details
     (since `/surveys/id/pages/id/questions` without ending /id also doesnt contain full info,
-
     In other words, we need to have triple stream slices, (note that api is very very rate limited
     and we need details for each survey etc), and finally we get a response similar to those we can have from `/id/details`
     endpoint. Also we will need to gather info to array in case of overrequesting, but details is already gathered it for us.
     We just need to apply filtering or small data transformation against array.
     So this way is very much better in terms of API limits.
     """
 
@@ -182,125 +177,7 @@
     cursor_field = "date_modified"
 
     def parse_response(self, response: requests.Response, stream_state: Mapping[str, Any], **kwargs) -> Iterable[Mapping]:
         data = super().parse_response(response=response, stream_state=stream_state, **kwargs)
         for record in data:
             record.pop("pages", None)  # remove pages data
             yield record
-
-
-class SurveyPages(SurveyIDSliceMixin, SurveymonkeyStream):
-    """should be filled from SurveyDetails"""
-
-    data_field = "pages"
-
-    def parse_response(self, response: requests.Response, stream_state: Mapping[str, Any], **kwargs) -> Iterable[Mapping]:
-        data = super().parse_response(response=response, stream_state=stream_state, **kwargs)
-        for record in data:
-            record.pop("questions", None)  # remove question data
-            yield record
-
-
-class SurveyQuestions(SurveyIDSliceMixin, SurveymonkeyStream):
-    """should be filled from SurveyDetails"""
-
-    data_field = "pages"
-
-    def parse_response(self, response: requests.Response, stream_state: Mapping[str, Any], **kwargs) -> Iterable[Mapping]:
-        data = super().parse_response(response=response, stream_state=stream_state, **kwargs)
-        for entry in data:
-            page_id = entry["id"]
-            questions = entry["questions"]
-            for question in questions:
-                question["page_id"] = page_id
-                yield question
-
-
-class SurveyResponses(SurveyIDSliceMixin, IncrementalSurveymonkeyStream):
-    """
-    Docs: https://developer.surveymonkey.com/api/v3/#api-endpoints-survey-responses
-    """
-
-    cursor_field = "date_modified"
-
-    def path(self, stream_slice: Mapping[str, Any] = None, **kwargs) -> str:
-        return f"surveys/{stream_slice['survey_id']}/responses/bulk"
-
-    def get_updated_state(self, current_stream_state: MutableMapping[str, Any], latest_record: Mapping[str, Any]) -> Mapping[str, Any]:
-        """
-        Return the latest state by comparing the survey_id and cursor value in the latest record with the stream's most recent state object
-        and returning an updated state object.
-        """
-        survey_id = latest_record.get("survey_id")
-        if not current_stream_state:
-            current_stream_state = {}
-        survey_state = current_stream_state.get(survey_id, {})
-
-        latest_record_value = latest_record.get(self.cursor_field, "")
-        if latest_record_value:
-            # add 1 second, otherwise next incremental syns return the same record
-            latest_record_value = pendulum.parse(latest_record_value).add(seconds=1).to_iso8601_string()
-
-        state_value = max(
-            latest_record_value,
-            survey_state.get(self.cursor_field, ""),
-        )
-        current_stream_state[survey_id] = {self.cursor_field: state_value}
-        return current_stream_state
-
-    def request_params(
-        self, stream_state: Mapping[str, Any], stream_slice: Mapping[str, Any] = None, next_page_token: Mapping[str, Any] = None
-    ) -> MutableMapping[str, Any]:
-        if next_page_token:
-            return next_page_token
-
-        params = super().request_params(stream_state=stream_state, stream_slice=stream_slice, next_page_token=next_page_token)
-        params["sort_order"] = "ASC"
-        params["sort_by"] = self.cursor_field
-        # Max of 100 allowed per page. We use the highest
-        # possible value to reduce the number of API calls.
-        params["per_page"] = 100
-
-        since_value_surv = stream_state.get(stream_slice["survey_id"])
-        if since_value_surv:
-            since_value = (
-                pendulum.parse(since_value_surv.get(self.cursor_field)) if since_value_surv.get(self.cursor_field) else self._start_date
-            )
-            since_value = max(since_value, self._start_date)
-        else:
-            since_value = self._start_date
-        params["start_modified_at"] = since_value.strftime("%Y-%m-%dT%H:%M:%S")
-        return params
-
-
-class SurveyCollectors(SurveyIDSliceMixin, SurveymonkeyStream):
-    """
-    API Docs: https://www.surveymonkey.com/developer/api/v3/#api-endpoints-get-surveys-id-collectors
-    """
-
-    def path(self, stream_slice: Mapping[str, Any] = None, **kwargs) -> str:
-        return f"surveys/{ stream_slice['survey_id'] }/collectors"
-
-    def parse_response(self, response: requests.Response, stream_state: Mapping[str, Any], **kwargs) -> Iterable[Mapping]:
-        data = super().parse_response(response=response, stream_state=stream_state, **kwargs)
-        for record in data:
-            record["survey_id"] = kwargs.get("stream_slice", {}).get("survey_id")
-            yield record
-
-
-class Collectors(SurveymonkeyStream):
-    """
-    API Docs: https://www.surveymonkey.com/developer/api/v3/#api-endpoints-get-collectors-id-
-    """
-
-    data_field = None
-
-    def path(self, stream_slice: Mapping[str, Any] = None, **kwargs) -> str:
-        return f"collectors/{stream_slice['collector_id']}"
-
-    def stream_slices(self, stream_state: Mapping[str, Any] = None, **kwargs):
-
-        survey_collectors = SurveyCollectors(start_date=self._start_date, survey_ids=self._survey_ids, authenticator=self.authenticator)
-        survey_ids = survey_collectors.stream_slices(stream_state, **kwargs)
-        for slice in survey_ids:
-            for collector in survey_collectors.read_records(sync_mode=SyncMode.full_refresh, stream_state=stream_state, stream_slice=slice):
-                yield {"collector_id": collector["id"]}
```

### Comparing `airbyte_source_surveymonkey-0.2.4/PKG-INFO` & `airbyte_source_surveymonkey-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-surveymonkey
-Version: 0.2.4
+Version: 0.3.0
 Summary: Source implementation for Surveymonkey.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.51.40)
+Requires-Dist: airbyte-cdk (>=0,<1)
 Requires-Dist: urllib3 (==1.26.18)
 Requires-Dist: vcrpy (==4.1.1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/surveymonkey
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Surveymonkey source connector
@@ -47,15 +47,15 @@
 
 
 ### Locally running the connector
 ```
 poetry run source-surveymonkey spec
 poetry run source-surveymonkey check --config secrets/config.json
 poetry run source-surveymonkey discover --config secrets/config.json
-poetry run source-surveymonkey read --config secrets/config.json --catalog sample_files/configured_catalog.json
+poetry run source-surveymonkey read --config secrets/config.json --catalog integration_tests/configured_catalog.json
 ```
 
 ### Running unit tests
 To run unit tests locally, from the connector directory run:
 ```
 poetry run pytest unit_tests
 ```
```

