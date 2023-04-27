# Comparing `tmp/tom_hermes-0.1.7.tar.gz` & `tmp/tom_hermes-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tom_hermes-0.1.7.tar", max compression
+gzip compressed data, was "tom_hermes-0.1.8.tar", max compression
```

## Comparing `tom_hermes-0.1.7.tar` & `tom_hermes-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-04-24 23:51:22.907679 tom_hermes-0.1.7/LICENSE
--rw-r--r--   0        0        0     1363 2023-04-24 23:51:22.907679 tom_hermes-0.1.7/README.md
--rw-r--r--   0        0        0     1265 2023-04-24 23:51:51.655861 tom_hermes-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       96 2023-04-24 23:51:51.655861 tom_hermes-0.1.7/tom_hermes/__init__.py
--rw-r--r--   0        0        0    11280 2023-04-24 23:51:22.907679 tom_hermes-0.1.7/tom_hermes/hermes.py
--rw-r--r--   0        0        0     2828 2023-04-24 23:51:22.907679 tom_hermes-0.1.7/tom_hermes/templates/tom_hermes/query_result.html
--rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 tom_hermes-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-27 20:08:14.861194 tom_hermes-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1594 2023-04-27 20:08:14.861194 tom_hermes-0.1.8/README.md
+-rw-r--r--   0        0        0     1265 2023-04-27 20:08:37.061579 tom_hermes-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-04-27 20:08:37.061579 tom_hermes-0.1.8/tom_hermes/__init__.py
+-rw-r--r--   0        0        0    11038 2023-04-27 20:08:14.861194 tom_hermes-0.1.8/tom_hermes/hermes.py
+-rw-r--r--   0        0        0     2836 2023-04-27 20:08:14.861194 tom_hermes-0.1.8/tom_hermes/templates/tom_hermes/query_result.html
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 tom_hermes-0.1.8/PKG-INFO
```

### Comparing `tom_hermes-0.1.7/LICENSE` & `tom_hermes-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tom_hermes-0.1.7/README.md` & `tom_hermes-0.1.8/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -27,8 +27,11 @@
         'django.contrib.admin',
         'django.contrib.auth',
         ...
         'tom_hermes'
     ]
 ```
 
+Add `HERMES_API_URL` to your `settings.py` if you want to point to a hermes instance other than `https://hermes.lco.global`.
+This is the same settings variable that `tom_nonlocalizedevents` uses to make queries to hermes as well.
+
 `Hermes` is now available as a Broker from the TOM Toolkit Alerts page. You may configure and execute your queries as you would any Broker.
```

### Comparing `tom_hermes-0.1.7/pyproject.toml` & `tom_hermes-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "tom-hermes"
 # this version is a placeholder: version supplied by poetry-dynamic-versioning
-version = "0.1.7"
+version = "0.1.8"
 description = "A TOM Toolkit Broker module for querying the Hermes Alert API"
 authors = ["Lindy Lindstrom <llindstrom@lco.global>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 packages = [{include = "tom_hermes"}]
```

### Comparing `tom_hermes-0.1.7/tom_hermes/hermes.py` & `tom_hermes-0.1.8/tom_hermes/hermes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 import logging
 import os
 import requests
+from dateutil.parser import parse
 
 from crispy_forms.layout import Column, Fieldset, Layout, Row
 
 from django import forms
 from django.apps import apps
 from django.conf import settings
 
@@ -20,67 +21,60 @@
 
 from tom_alerts.alerts import GenericBroker, GenericQueryForm
 from tom_targets.models import Target
 
 logger = logging.getLogger(__name__)
 #logger.setLevel(logging.DEBUG)
 
-HERMES_URL = os.getenv('HERMES_BASE_URL', 'http://hermes.lco.global')
+HERMES_URL = settings.HERMES_API_URL if hasattr(settings, 'HERMES_API_URL') else os.getenv('HERMES_BASE_URL', 'https://hermes.lco.global')
 HERMES_API_VERSION = 0
 HERMES_API_URL = f'{HERMES_URL}/api/v{HERMES_API_VERSION}'
 
 
 class HermesQueryForm(GenericQueryForm):
-    topic = forms.MultipleChoiceField(choices=[], required=False, label='Topic')
-    timestamp_after = forms.DateTimeField(required=False, label='Datetime lower',
-        #widget=forms.TextInput(attrs={'type': 'date'})
-        )
-    timestamp_before = forms.DateTimeField(required=False, label='Datetime upper',
-        #widget=forms.TextInput(attrs={'type': 'date'})
-        )
+    published_after = forms.CharField(required=False, label='Published after',
+        widget=forms.TextInput(attrs={'type': 'date'})
+    )
+    published_before = forms.CharField(required=False, label='Published before',
+        widget=forms.TextInput(attrs={'type': 'date'})
+    )
 
     event_id = forms.CharField(required=False, label='Hermes Event ID')
 
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        self.fields['topic'].choices = self.get_topic_choices()
-
         self.helper.layout = Layout(
             self.common_layout,
             Fieldset(
                 'Time Filters',
                 Row(
-                    Column('timestamp_after'),
-                    Column('timestamp_before')
+                    Column('published_after'),
+                    Column('published_before')
                 )
             ),
             'event_id',
 
         )
 
+    def clean_published_after(self):
+        published_after = self.cleaned_data['published_after']
+        return parse(published_after).isoformat()
+
+    def clean_published_before(self):
+        published_before = self.cleaned_data['published_before']
+        return parse(published_before).isoformat()
+
     def clean(self):
         cleaned_data = super().clean()
         # TODO: do we need to extend this method from the super?
 
         return cleaned_data
 
-    @staticmethod
-    def get_topic_choices():
-        """The Hermes api/v0/topics endpoint return JSON of the form:
-        {'topics': [<list of topic strings]}
-
-        This method should return a list of tuples suitable for choices property
-        of a forms.MultipleChoiceField.
-        """
-        response = requests.get(f'{HERMES_API_URL}/topics')
-        response.raise_for_status()
-        return [(topic_name, topic_name) for topic_name in response.json()['topics']]
-
 
 # TODO: Sort out "upstream" submission to Hopskotch functionality
 #class SCIMMAUpstreamSubmissionForm(GenericUpstreamSubmissionForm):
 #    topic = forms.CharField(required=False, max_length=100, widget=forms.HiddenInput())
 #
 
 @dataclass
@@ -88,17 +82,17 @@
     """Represent a Hermes NonlocalizedEvent for display as query result.
 
     HermesBroker._to_generic_alert does the translation
     """
     id: int # used for cache identification and retrieval 
     event_id: str
     nonlocalizedevent_id: int # PK of tom_nonlocalizedevent.model.NonLocalizedEvent (if exists)
-    title: str
     sequence_type: str
     sequence_number: int
+    published: str
     hermes_url: str
     gracedb_url: str
     far: float # False Alarm Rate
 
 
 class HermesBroker(GenericBroker):
     """
@@ -121,40 +115,38 @@
         This method is called by RunQueryView.get_context_data with the alerts from
         the broker.fetch_alerts method below. (The `alerts` passed in here is the iterable
         returned from fetch_alerts).
         """
         # Report whether `tom_nonlocalizedevents` is installed.
 
         broker_context_for_view = {
-            'salutation': 'All your Events are Belong to Us!',  # this was just for testing puposes
             'tom_nonlocalizedevents_installed': apps.is_installed('tom_nonlocalizedevents'),
             'version': __version__, # from tom_hermes/__init__.py
         }
 
         return broker_context_for_view
 
     def _request_messages(self, parameters):
         logger.debug(f'HermesBroker._request_messages()  parameters: {parameters}')
         response = requests.get(f'{HERMES_API_URL}/nonlocalizedevents/',
-                                params={**parameters},
-                                headers=settings.BROKERS['HERMES'])
+                                params={**parameters})
         logger.debug(f'HermesBroker._request_messages() response.url: {response.url}')
         response.raise_for_status()
         return response.json()
 
     def fetch_alerts(self, parameters):
         logger.debug(f'HermesBroker.fetch_alerts()  parameters: {parameters}')
         parameters['page_size'] = 20
         result = self._request_messages(parameters)
         return iter(result['results'])
 
     def fetch_message(self, message_id):
         logger.debug(f'HermesBroker.fetch_message()  message_id: {message_id}')
         url = f'{HERMES_API_URL}/messages/{message_id}'
-        response = requests.get(url, headers=settings.BROKERS['HERMES'])
+        response = requests.get(url)
         response.raise_for_status()
         json_data = response.json()
         return json_data
 
     def to_generic_alert(self, nonlocalizedevent):
         """Map the Hermes Nonlocalized fields into GenericAlert fields.
         Rather than tom_alerts.GenericAlert, tom_hermes uses the HermesNonLocalizedEventAlert
@@ -168,22 +160,27 @@
         event_id = nonlocalizedevent['event_id']
         url = f'{HERMES_URL}/nonlocalizedevent/{event_id}'
         # Use the last message in the sequence to get values
         message = nonlocalizedevent['sequences'][-1]['message'] # index -1 gives last in sequence
         sequence_type = nonlocalizedevent['sequences'][-1]['sequence_type']
         sequence_number = nonlocalizedevent['sequences'][-1]['sequence_number']
         try:
-            gracedb_url = message['data']['eventpage_url'],
+            gracedb_url = message['data'].get('urls', {}).get('gracedb', '')
         except KeyError:
             # a RETRACTION does not have an eventpage_url so use the previous alert in the sequence
-            gracedb_url = nonlocalizedevent['sequences'][-2]['message']['data']['eventpage_url'],
+            gracedb_url = nonlocalizedevent['sequences'][-2]['message']['data'].get('urls', {}).get('gracedb', '')
 
         # set score for this event as it's False Alarm Rate (far)
         # Retractions won't have FAR, so provide default
-        far = float(message['data'].get('far', "1").split()[0])
+        if message['data'].get('event', {}):
+            far = float(message['data'].get('event', {}).get('far', 1))
+        else:
+            far = 1
+
+        published = parse(message['published'])
 
         # if tom_nonlocalizedevents is installed, then check if there is a
         # tom_nonlocalizedevents.models.NonLocalizedEvent instance for this event_id.
         # if so, return it's PK (for linking) as the id of the alert.
         nle_id = None # if event is not found
         if apps.is_installed('tom_nonlocalizedevents'):
             # yes, it's unorthodox to import here
@@ -192,15 +189,15 @@
             if nonlocalized_event is not None:
                 nle_id = nonlocalized_event.id
         
         hermes_alert = HermesNonLocalizedEventAlert(
             id=event_id,
             event_id=event_id,
             nonlocalizedevent_id=nle_id,
-            title=message['data']['title'],
+            published=published.strftime('%d/%m/%Y %H:%M:%S'),
             sequence_type=sequence_type,
             sequence_number=sequence_number,
             hermes_url=url,
             gracedb_url=gracedb_url,
             far = far)
 
         return hermes_alert
```

### Comparing `tom_hermes-0.1.7/tom_hermes/templates/tom_hermes/query_result.html` & `tom_hermes-0.1.8/tom_hermes/templates/tom_hermes/query_result.html`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     <p><em>Note: Event creation can take time as sky maps are retreived from GraceDb.</em></p>
   </div>
   <table class="table table-striped">
     <thead>
       <tr>
         <th></th>
         <th>Event ID</th>
-        <th>Title</th>
+        <th>Published</th>
         <th>Sequence Type (Number)</th>
         <th>Hermes</th>
         <th>GraceDB</th>
         <th><span title="{{ score_description }}">FAR</span></th>
       </tr>
     </thead>
     <tbody>
@@ -47,15 +47,15 @@
         <td>{{ event.event_id }}</td>
         {% endif %}
         {% else %}
         <!-- tom_nonlocalizedevents not installed-->
         <td></td>
         <td>{{ event.event_id }}</td>
         {% endif %}
-        <td>{{ event.title }}</td>
+        <td>{{ event.published }}</td>
         <td>{{ event.sequence_type }} ({{ event.sequence_number }})</td>
         <td><a href="{{ event.hermes_url }}" target="_blank" title="Hermes Alert">Hermes</a></td>
         <td><a href="{{ event.gracedb_url }}" target="_blank" title="GraceDB View">GraceDB</a></td>
         <td>{{ event.far|stringformat:"e" }}</td>
       </tr>
       {% endfor %}
     </tbody>
```

#### html2text {}

```diff
@@ -5,22 +5,22 @@
 {% csrf_token %}
   [Create Events]
 {% else %}
 NOTE: tom_nonlocalizedevents is not intalled. Event creation functions
 disabled.
 {% endif %}
 Note: Event creation can take time as sky maps are retreived from GraceDb.
- Event ID       Title Sequence Type  Hermes GraceDB        FAR
-                      (Number)
-                                                                       {
- {                    {                     {              {           { event.sequence_type                {
- {              ⁰   {                     {              {           }} ({                 Hermes GraceDB {
- event.event_id       event.event_id        event.event_id event.title {                                    event.far|stringformat:
- }}                   }}                    }}             }}          event.sequence_number                "e" }}
-                                                                       }})
+ Event ID       Published Sequence Type  Hermes GraceDB        FAR
+                          (Number)
+                                                                               {
+ {                        {                     {              {               { event.sequence_type                {
+ {              ⁰       {                     {              {               }} ({                 Hermes GraceDB {
+ event.event_id           event.event_id        event.event_id event.published {                                    event.far|stringformat:
+ }}                       }}                    }}             }}              event.sequence_number                "e" }}
+                                                                               }})
  {% if tom_nonlocalizedevents_installed %}
 {% else %}
 {% endif %} {% if broker_feedback %}
 {{broker_feedback}}
 {% endif %}
 tom_hermes version {{ version }}
  {% endblock %}
```

### Comparing `tom_hermes-0.1.7/PKG-INFO` & `tom_hermes-0.1.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tom-hermes
-Version: 0.1.7
+Version: 0.1.8
 Summary: A TOM Toolkit Broker module for querying the Hermes Alert API
 License: GPL-3.0-or-later
 Author: Lindy Lindstrom
 Author-email: llindstrom@lco.global
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -44,9 +44,12 @@
         'django.contrib.admin',
         'django.contrib.auth',
         ...
         'tom_hermes'
     ]
 ```
 
+Add `HERMES_API_URL` to your `settings.py` if you want to point to a hermes instance other than `https://hermes.lco.global`.
+This is the same settings variable that `tom_nonlocalizedevents` uses to make queries to hermes as well.
+
 `Hermes` is now available as a Broker from the TOM Toolkit Alerts page. You may configure and execute your queries as you would any Broker.
```

