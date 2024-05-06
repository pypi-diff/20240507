# Comparing `tmp/tom_swift-0.2.0a3.tar.gz` & `tmp/tom_swift-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tom_swift-0.2.0a3.tar", max compression
+gzip compressed data, was "tom_swift-0.2.1.tar", max compression
```

## Comparing `tom_swift-0.2.0a3.tar` & `tom_swift-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-10-17 23:53:50.988352 tom_swift-0.2.0a3/LICENSE
--rw-r--r--   0        0        0     2249 2023-10-17 23:53:50.988352 tom_swift-0.2.0a3/README.md
--rw-r--r--   0        0        0     1290 2023-10-17 23:54:14.864628 tom_swift-0.2.0a3/pyproject.toml
--rw-r--r--   0        0        0       99 2023-10-17 23:54:14.864628 tom_swift-0.2.0a3/tom_swift/__init__.py
--rw-r--r--   0        0        0    31828 2023-10-17 23:53:50.988352 tom_swift-0.2.0a3/tom_swift/swift.py
--rw-r--r--   0        0        0     5451 2023-10-17 23:53:50.988352 tom_swift-0.2.0a3/tom_swift/swift_api.py
--rw-r--r--   0        0        0     8927 2023-10-17 23:53:50.988352 tom_swift-0.2.0a3/tom_swift/templates/tom_swift/observation_form.html
--rw-r--r--   0        0        0     2954 1970-01-01 00:00:00.000000 tom_swift-0.2.0a3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-06 22:56:01.039283 tom_swift-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2331 2024-05-06 22:56:01.039283 tom_swift-0.2.1/README.md
+-rw-r--r--   0        0        0     1348 2024-05-06 22:56:14.115418 tom_swift-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       97 2024-05-06 22:56:14.115418 tom_swift-0.2.1/tom_swift/__init__.py
+-rw-r--r--   0        0        0    35475 2024-05-06 22:56:01.039283 tom_swift-0.2.1/tom_swift/swift.py
+-rw-r--r--   0        0        0     7170 2024-05-06 22:56:01.039283 tom_swift-0.2.1/tom_swift/swift_api.py
+-rw-r--r--   0        0        0    11283 2024-05-06 22:56:01.039283 tom_swift-0.2.1/tom_swift/templates/tom_swift/observation_form.html
+-rw-r--r--   0        0        0      231 2024-05-06 22:56:01.039283 tom_swift-0.2.1/tom_swift/test_swift.py
+-rw-r--r--   0        0        0     2972 1970-01-01 00:00:00.000000 tom_swift-0.2.1/PKG-INFO
```

### Comparing `tom_swift-0.2.0a3/LICENSE` & `tom_swift-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tom_swift-0.2.0a3/README.md` & `tom_swift-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # tom_swift
-_Note: This repository is under active development. It is a not-yet-functional, work in progress._
-
 [Neil Gehrels Swift Observatory](https://swift.gsfc.nasa.gov/index.html) facility module for TOM Toolkit. This module uses the
 [Swift TOO API](https://www.swift.psu.edu/too_api/) for all its interactions with the _Swift_ Observatory. When installed and
 configured, your TOM can query target visibility, submit TOO observation requests to Swift, and check TOO observation status.
 
 ## Swift TOO Prerequisites
 In order to submit TOO requests to Swift, you must [register with the Swift TOO system](https://www.swift.psu.edu/toop/too_newuser.php).
 Once you are registered and have logged in, you can [get your shared secret](https://www.swift.psu.edu/toop/change_secret.php), which you
@@ -14,23 +12,32 @@
 
 Install the module into your TOM environment:
 
 ```shell
 pip install tom-swift
 ```
 
-Add `tom_swift.swift.SwiftFacility` to the `TOM_FACILITY_CLASSES` in your TOM's
+1. In your project `settings.py`, add `tom_swift` to your `INSTALLED_APPS` setting:
+
+    ```python
+    INSTALLED_APPS = [
+        ...
+        'tom_swift',
+    ]
+    ```
+
+2. Add `tom_swift.swift.SwiftFacility` to the `TOM_FACILITY_CLASSES` in your TOM's
 `settings.py`:
-```python
+   ```python
     TOM_FACILITY_CLASSES = [
         'tom_observations.facilities.lco.LCOFacility',
         ...
         'tom_swift.swift.SwiftFacility',
     ]
-```
+   ```   
 
 ## Configuration
 
 Include the following settings inside the `FACILITIES` dictionary inside `settings.py`:
 
 ```python
     FACILITIES = {
```

### Comparing `tom_swift-0.2.0a3/pyproject.toml` & `tom_swift-0.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [tool.poetry]
 name = "tom-swift"
 # this version is a placeholder: version supplied by poetry-dynamic-versioning
-version = "0.2.0a3"
+version = "0.2.1"
 description = "TOM Toolkit Facility module for the Neil Gehrels Swift Observatory"
 authors = ["Lindy Lindstrom <llindstrom@lco.global>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "tom_swift"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
-tomtoolkit = "^2.14"
-BatAnalysis = "^1.0"
+python = ">=3.8.1,<3.12"
+tomtoolkit = ">=2.15"
+swifttools = "<4"
 
+[tool.poetry.group.lint.dependencies]
+flake8 = ">=6.0,<7.1"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 # the default pattern regex makes the 'v' manditory
 # this pattern modifies the default regex in order to make the 'v' optional
```

### Comparing `tom_swift-0.2.0a3/tom_swift/swift.py` & `tom_swift-0.2.1/tom_swift/swift.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import logging
 
-from crispy_forms.layout import Layout, Div, Field, Row, HTML
+from crispy_forms.layout import Layout, Div, Field
 from crispy_forms.bootstrap import Accordion, AccordionGroup
 from django import forms
-from django.conf import settings
-from django.contrib import messages # not sure if we can do this outside of a View
 from django.utils.safestring import mark_safe
 
 from tom_observations.facility import BaseObservationForm, BaseObservationFacility, get_service_class
 from tom_targets.models import Target
 
 from tom_swift import __version__
 from tom_swift.swift_api import (SwiftAPI,
                                  SWIFT_INSTRUMENT_CHOICES,
+                                 SWIFT_OTHER_CHOICE,
                                  SWIFT_TARGET_CLASSIFICATION_CHOICES,
                                  SWIFT_URGENCY_CHOICES,
                                  SWIFT_XRT_MODE_CHOICES,
+                                 SWIFT_UVOT_FILTER_MODE_CHOICES,
+                                 get_grb_detector_choices,
                                  get_observation_type_choices,
                                  get_monitoring_unit_choices,)
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 #  TODO: re-consider (or remove?) assumption that all Layout instances have a group property
@@ -43,15 +44,15 @@
 
     #
     # Source name, type, location, position_error
     #
     # source_name, ra, dec are not part of the form
 
     # see tom_swift/templates/tom_swift/observation_form.html for javascript
-    # that displays/hides the target_classification ChoiceField if "Other (please specify)""
+    # that displays/hides the target_classification ChoiceField if "Other (please specify)"
     # is chosen in the target_classification_choices drop-down menu widget.
     target_classification_choices = forms.ChoiceField(
         required=True,
         label='Target Type or Classification',
         choices=SWIFT_TARGET_CLASSIFICATION_CHOICES,
         initial=SWIFT_TARGET_CLASSIFICATION_CHOICES[0]
     )
@@ -80,90 +81,113 @@
     urgency = forms.ChoiceField(
         required=True,
         label='Urgency',
         choices=SWIFT_URGENCY_CHOICES,
         initial=SWIFT_URGENCY_CHOICES[2])
 
     #
-    # Observation Type ('Specroscopy', 'Light Curve', 'Position', 'Timing')
+    # Observation Type ('Spectroscopy', 'Light Curve', 'Position', 'Timing')
     #
     obs_type = forms.ChoiceField(
         required=True,
         label='Observation Type',
         choices=get_observation_type_choices(),
         help_text='What is driving the exposure time?')
 
     #
     # Description of the source brightness for various instruments
     #
     # TODO: validation - answer at least one of these questions
-    optical_magnitude = forms.FloatField(required=False, label='Optical Magnitude')
-    optical_filter = forms.CharField(required=False, help_text='What filter was the optical magnitude measured in?', initial='u')
+    optical_magnitude = forms.FloatField(
+        required=False,
+        label='Optical Magnitude')
+    optical_filter = forms.CharField(
+        required=False,
+        label='Optical Filter',
+        help_text='What filter was the optical magnitude measured in?',
+        initial='u')
     xrt_countrate = forms.FloatField(required=False, label='XRT Count Rate [counts/second]')
     bat_countrate = forms.FloatField(required=False, label='BAT Count Rate [counts/second]')
     other_brightness = forms.CharField(
-        required=False, label='Other Brightness',
-        widget=forms.TextInput(attrs={'placeholder': 'Any other brightness information.'})
+        required=False, label='Additional Brightness Information',
+        widget=forms.Textarea(attrs={
+            'rows': 2,
+            'placeholder': 'Any other brightness information.',
+        })
     )
 
     #
     # GRB stuff
     #
-    grb_detector = forms.CharField(
+    grb_detector_choices = forms.ChoiceField(
         required=False,
         label='GRB Detector',
-        widget=forms.TextInput(attrs={'placeholder': 'Should be "Mission/Detection" (e.g. Swift/BAT, Fermi/LAT)'})
+        choices=get_grb_detector_choices(),
+    )
+
+    grb_detector = forms.CharField(
+        required=False,
+        label='Other GRB Detector',
+        widget=forms.TextInput(attrs={'placeholder': 'Specify other "Mission/Detection"'})
     )
 
     grb_triggertime = forms.DateTimeField(
         required=False,
-        label='GRB Trigger Date/Time',
-        widget=forms.DateTimeInput) # TODO: finish this
-    # TODO: validate: required if target_classification is GRB
-    # TODO: make the widget nice
+        label='GRB Trigger Date/Time [UTC]',
+        # see https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/datetime-local
+        widget=forms.TextInput(attrs={'class': 'ml-2', 'type': 'datetime-local'}))
 
     #
     # Science Justification
     #
     immediate_objective = forms.CharField(
         required=False, label='Immediate Objective',
         widget=forms.Textarea(attrs={
             'rows': 2,
-            'placeholder' : 'One sentence explanation of this TOO request.'})
-        )
+            'placeholder': 'One sentence explanation of this TOO request.'
+        })
+    )
 
     science_just = forms.CharField(
         required=False, label='Science Justification',
         widget=forms.Textarea(attrs={
             'rows': 8,
-            'placeholder' : 'A pursuasive paragraph or two explaining why this object requires rapid observation.'})
-        )
+            'placeholder': 'Two or three persuasive paragraphs explaining why this object requires rapid observation.'
+        })
+    )
 
     #
     # Exposure requested time (total)
     #
-    exposure = forms.FloatField(required=False, label='Exposure time requested [s]',initial=500)
+    exposure = forms.FloatField(
+        required=True,
+        label='Total exposure time requested [s]')
     exp_time_just = forms.CharField(
-        required=False, label='Exposure Time Justification',
+        required=True,
+        label='Exposure time justification',
         widget=forms.Textarea(attrs={
             'rows': 2,
             'placeholder': 'Briefly justify the exposure time requested.'}),
     )
 
     #
     # Monitoring requests
     #
-    exp_time_per_visit = forms.FloatField(required=False, label='Exposure time per visit(s) [s]')
-    num_of_visits= forms.IntegerField(
+    exp_time_per_visit = forms.FloatField(required=False, label='Exposure time per visit [s]')
+    num_of_visits = forms.IntegerField(
         required=False,
         label='Number of visits [integer]',
         help_text=('If number of visits is more than one, then complete exposure'
                    ' time per visit and monitoring frequency.'),
         initial=1)
-    monitoring_freq = forms.IntegerField(required=False, label='Monitoring Frequency', initial=1)
+    monitoring_freq = forms.IntegerField(
+        required=False,
+        label='Monitoring frequency',
+        help_text=('One visit every N monitoring units.'),
+        initial=1)
     monitoring_units = forms.ChoiceField(
         required=False,
         choices=get_monitoring_unit_choices(),
     )
 
     #
     # Swift Guest Investigator program parameters
@@ -176,29 +200,37 @@
     proposal_pi = forms.CharField(required=False, label='Proposal PI name')
 
     #
     # Instrument mode
     #
     xrt_mode = forms.TypedChoiceField(
         required=False,
-        label='XRT mode',
+        label='XRT Mode',
         choices=SWIFT_XRT_MODE_CHOICES,
-        coerce=int, # convert the string '6' to int 6
-        initial=6) # Windowed Timing (WT))
+        coerce=int,  # convert the string '6' to int 6
+        initial=6)  # Windowed Timing (WT))
+
+    uvot_mode_choices = forms.ChoiceField(
+        required=False,
+        label='UVOT Filter Mode',
+        initial=SWIFT_UVOT_FILTER_MODE_CHOICES[-2],
+        choices=SWIFT_UVOT_FILTER_MODE_CHOICES,
+        help_text=mark_safe((f'These are some common UVOT Filter modes.'
+                             f' See <a target=_blank'
+                             f' href=https://www.swift.psu.edu/operations/mode_lookup.php>'
+                             f'UVOT Mode Lookup Tool</a>.'
+                             f' Select "{SWIFT_OTHER_CHOICE}" to specify your own filter mode'
+                             f' or give written instructions.'
+                             )),
+    )
 
     uvot_mode = forms.CharField(
         required=False,
-        label='UVOT filter mode',
-        initial='0x9999',
-        help_text=mark_safe(('Supply a specific UVOT Filter mode or written instructions.'
-                             ' See <a target=_blank'
-                             ' href=https://www.swift.psu.edu/operations/mode_lookup.php>'
-                             'UVOT Mode Lookup Tool</a>'
-                            )),
-    ) # 0x9999 is the "Filter of the Day" and does not require justification
+        label='Other UVOT Filter Mode',
+    )  # 0x9999 is the "Filter of the Day" and does not require justification
 
     # required unless uvot_mode is 0x9999 (Filter of the Day)
     uvot_just = forms.CharField(
         required=False,
         label='UVOT Mode Justification',
         widget=forms.Textarea(attrs={
             'rows': 3,
@@ -246,130 +278,142 @@
         help_text='Text description of why tiling is justified.',
         widget=forms.Textarea(attrs={
             'rows': 4,
             'placeholder': 'Please describe why tiling is justified.'
         }),
     )
 
-
     #
     # Debug parameter
     #
     debug = forms.BooleanField(required=False, label='Debug', initial=True)
 
-
-
     def layout(self):
         layout = Layout(
             'urgency',
             Accordion(
                 AccordionGroup('Target Information',
-                'target_classification_choices',
-                'target_classification',
-                'grb_detector',
-                'grb_triggertime',
-                'poserr',
-                ),
+                               'target_classification_choices',
+                               'target_classification',
+                               Div(
+                                   Div(Field('grb_detector_choices'), css_class='col-md-5',),
+                                   Div(Field('grb_triggertime'), css_class='col-md-7',),
+                                   css_class='row',
+                                ),
+                               'grb_detector',
+                               'poserr',
+                               ),
                 AccordionGroup('Science Justification',
-                    Div(
-                        'immediate_objective',
-                        'science_just',
-                    )
-                ),
+                               Div(
+                                   'immediate_objective',
+                                   'science_just',
+                               )
+                               ),
                 AccordionGroup('Instrument Information',
-                    Div(
-                        Div(# this div is to put instrument drop-down and slew_in_place checkbox
-                            # side-by-side in the same row
-                            Div(Field('instrument'), css_class='col-md-6',),
-                            Div(Field('slew_in_place'), css_class='col-md-6',),
-                            css_class='row',
-                        ),
-                        'xrt_mode',
-                        'uvot_mode',
-                        'uvot_just',
-                    ),
-                ),
+                               Div(
+                                   Div(  # this div is to put instrument drop-down and slew_in_place checkbox
+                                         # side-by-side in the same row
+                                       Div(Field('instrument'), css_class='col-md-7',),
+                                       Div(Field('slew_in_place'), css_class='col-md-5',),
+                                       css_class='row',
+                                   ),
+                                   'xrt_mode',
+                                   'uvot_mode_choices',
+                                   'uvot_mode',
+                                   'uvot_just',
+                               ),
+                               ),
                 AccordionGroup('Source Brightness',
-                    Div(
-                        'obs_type',
-                        'optical_magnitude',
-                        'optical_filter',
-                        'xrt_countrate',
-                        'bat_countrate',
-                        'other_brightness',
-                    ),
-                ),
-                AccordionGroup('Exposure Information',
-                    Div(
-                        'exposure',
-                        'exp_time_just',
-                    ),
-                    Div(
-                        'num_of_visits',
-                        'exp_time_per_visit',
-                        Div(
-                            Div(Field('monitoring_freq'), css_class='col-md-6',),
-                            Div(Field('monitoring_units'), css_class='col-md-6',),
-                            css_class='row',
-                        ),
-                    )
-                ),
+                               Div(
+                                   'obs_type',
+                                   Div(
+                                       Div(Field('optical_magnitude'), css_class='col-md-6'),
+                                       Div(Field('optical_filter'), css_class='col-md-6',),
+                                       css_class='row',
+                                   ),
+                                   Div(
+                                       Div(Field('xrt_countrate'), css_class='col-md-6'),
+                                       Div(Field('bat_countrate'), css_class='col-md-6',),
+                                       css_class='row',
+                                   ),
+                                   'other_brightness',
+                               ),
+                               ),
+                AccordionGroup('Exposure & Visit Information',
+                               Div(
+                                   'exposure',
+                                   'exp_time_just',
+                               ),
+                               Div(
+                                   'num_of_visits',
+                                   'exp_time_per_visit',
+                                   Div(  # put these fields side-by-side in the same row
+                                       Div(Field('monitoring_freq'), css_class='col-md-6',),
+                                       Div(Field('monitoring_units'), css_class='col-md-6',),
+                                       css_class='row',
+                                   ),
+                               )
+                               ),
                 AccordionGroup('Tiling',
-                    Div(
-                        'tiling',
-                        'number_of_tiles',
-                        'exposure_time_per_tile',
-                        'tiling_justification',
-                    )
-                ),
+                               Div(
+                                   Div(  # make the tiling Boolean widget a switch
+                                       Field('tiling', css_class="custom-control-input"),
+                                       css_class="custom-control custom-switch"),
+                                   'number_of_tiles',
+                                   'exposure_time_per_tile',
+                                   'tiling_justification',
+                               )
+                               ),
                 AccordionGroup('Swift Guest Investigator',
-                    Div(
-                        'proposal',
-                        'proposal_id',
-                        'proposal_pi',
-                        'proposal_trigger_just',
-                    )
-                ),
+                               Div(
+                                   Div(  # make the proposal Boolean widget a switch
+                                       Field('proposal', css_class="custom-control-input"),
+                                       css_class="custom-control custom-switch"),
+                                   'proposal_id',
+                                   'proposal_pi',
+                                   'proposal_trigger_just',
+                               )
+                               ),
             ),
             'debug'
-        ) # end layout
+        )  # end layout
 
         return layout
 
     def is_valid(self):
         """Validate the form
 
         This method is called by the view's form_valid() method.
         """
         # TODO: check validity of doc-string
-        super().is_valid() # this adds cleaned_data to the form instance
+        super().is_valid()  # this adds cleaned_data to the form instance
         logger.debug(f'SwiftObservationForm.is_valid -- cleaned_data: {self.cleaned_data}')
 
         observation_payload = self.observation_payload()
         logger.debug(f'SwiftObservationForm.is_valid -- observation_payload: {observation_payload}')
 
         # BaseObservationForm.is_valid() says to make this call the Facility.validate_observation() method
         observation_module = get_service_class(self.cleaned_data['facility'])
 
         # validate_observation needs to return a list of (field, error) tuples
         # if the list is empty, then the observation is valid
         #
-        # in order to call self.add_error(field, error), the field given must match the
-        # a field declared on the Form, Thus, the form field names must match the properties
-        # of the swifttoolkit.Swift_TOO object (unless we want to maintain a a mapping between
+        # in order to call self.add_error(field, error), the field given must match a
+        # field declared on the Form, thus the form field names must match the properties
+        # of the swifttoolkit.Swift_TOO object (unless we want to maintain a mapping between
         # the two). NB: field can be None.
         #
         errors: [] = observation_module().validate_observation(observation_payload)
 
         if errors:
             self.add_error(None, errors)
             logger.debug(f'SwiftObservationForm.is_valid -- errors: {errors}')
 
         if self._errors:
-            logger.warn(f'Facility submission has errors {self._errors.as_data()}')
+            logger.warning(f'Facility submission has errors {self._errors.as_data()}')
 
         # if add_error has not been called, then a success message will be displayed in the template
         return not self._errors
 
     def observation_payload(self):
         """Transform the form.cleaned_data into a payload dictionary that can be:
            A. validated (see) SwiftFacility.validate_observation(); and
@@ -379,17 +423,17 @@
         into something that can be more directly submitted to the facility's API
         (via the Facility's validate_observation() and submit_observation() methods).
 
         For Swift, since we're configuring a Swift_TOO object, the form.cleaned_data
         plus the target information should be sufficient. See _configure_too() for how
         the observation_payload is used to configure the TOO attributes.
         """
-        # At the moment it's unclear why the obeervation_payload needs to differ from
+        # At the moment it's unclear why the observation_payload needs to differ from
         # the form.cleaned_data...
-        payload = self.cleaned_data.copy() # copy() just to be safe
+        payload = self.cleaned_data.copy()  # copy() just to be safe
 
         # ...but we need to add the target information because only the target_id is
         # in the form via get_initial().
         target = Target.objects.get(pk=self.cleaned_data['target_id'])
         payload['source_name'] = target.name
         payload['ra'] = target.ra
         payload['dec'] = target.dec
@@ -425,15 +469,15 @@
         # get the username from the SwiftAPI for the context
         username = self.swift_api.get_credentials()[0]  # returns (username, shared_secret)
         new_context_data = {
             'version': __version__,  # from tom_swift/__init__.py
             'username': username,
         }
 
-        # get the resovled target info from the SwiftAPI
+        # get the resolved target info from the SwiftAPI
         target = kwargs['target']
         resolved_target = self.swift_api.resolve_target(target)
         if resolved_target:
             new_context_data['resolver'] = resolved_target.resolver
             new_context_data['resolved_target_name'] = resolved_target.name
             new_context_data['resolved_target_ra'] = resolved_target.ra
             new_context_data['resolved_target_dec'] = resolved_target.dec
@@ -447,15 +491,15 @@
     def get_form(self, observation_type):
         return SwiftObservationForm
 
     def all_data_products(self, observation_record):
         data_products = super().all_data_products(observation_record)
         logger.debug(f'all_data_products: {data_products}')
         # TODO: right now we just extend this to log a debug message. So remove this
-        # and just let the super class method handle it, when we're finished developing.
+        #  and just let the super class method handle it, when we're finished developing.
         return data_products
 
     def data_products(self, observation_id, product_id=None):
         logger.debug('data_products')
         # TODO: how do we get data products from Swift?
         return []
 
@@ -467,15 +511,15 @@
         """
         """
         logger.debug('get_observation_url')
         return 'SwiftFacility.get_observation_url()'
 
     def get_observing_sites(self):
         """Normally this would return an iterable dictionary of site LAT,LON,ELV values
-        to be used for target visibiliy window calculations. See, for example,
+        to be used for target visibility window calculations. See, for example,
         tom_base/tom_observations/facilities/ocs.py::OCSSettings.get_sites()
 
         Swift is entirely different. Just return and empty dict for now.
         """
         logger.debug('get_observing_sites')
         return {}
 
@@ -486,16 +530,14 @@
         # TODO: this just a made-up list of states. Find out what the real states are.
         terminal_states = ['Completed', 'Failed', 'Canceled']
 
         logger.warning(f'get_terminal_observing_states - (FAKE!) terminal_states: {terminal_states}')
 
         return terminal_states
 
-
-
     def _configure_too(self, observation_payload):
         """In preparation for calls to self.swift_api.too.validate() and self.swift_api.too.submit(),
         both validate_observation() and submit_observation() call this method to
         configure the Swift_TOO object (self.too) from the observation_payload.
 
         For this Facility, the observation_payload is the serialized form.cleaned_data
         plus the target information (which doesn't come from the form).
@@ -518,15 +560,15 @@
         self.swift_api.too.source_name = observation_payload['source_name']
         self.swift_api.too.ra = observation_payload['ra']
         self.swift_api.too.dec = observation_payload['dec']
         self.swift_api.too.poserr = observation_payload['poserr']
 
         # Get the source_type from target_classification_choices or target_classification
         # depending on if they selected "Other (please specify)" in the drop-down menu
-        if observation_payload['target_classification_choices'] == 'Other (please specify)':
+        if observation_payload['target_classification_choices'] == SWIFT_OTHER_CHOICE:
             # they specified a custom target classification. So, use that.
             self.swift_api.too.source_type = observation_payload['target_classification']
         else:
             # use the value from the drop-down menu
             self.swift_api.too.source_type = observation_payload['target_classification_choices']
 
         #
@@ -550,15 +592,26 @@
         self.swift_api.too.bat_countrate = observation_payload['bat_countrate']  # counts/second
         self.swift_api.too.other_brightness = observation_payload['other_brightness']
         # TODO: validation - answer at least one of these questions
 
         #
         # GRB stuff
         #
-        # TODO: GRB stuff
+        # If they specified GRB for the target_classification,
+        #     then set the grb_detector and grb_triggertime.
+        # And, if they specified SWIFT_OTHER_CHOICE for the GRB detector,
+        #     then set grb_detector from their text.
+        #
+        if observation_payload['target_classification_choices'] == 'GRB':
+            self.swift_api.too.grb_triggertime = observation_payload['grb_triggertime']
+            if observation_payload['grb_detector_choices'] == SWIFT_OTHER_CHOICE:
+                # they specified a custom GRB detector. So, use that.
+                self.swift_api.too.grb_detector = observation_payload['grb_detector']
+            else:
+                self.swift_api.too.grb_detector = observation_payload['grb_detector_choices']
 
         #
         # Science Justification
         #
         self.swift_api.too.immediate_objective = observation_payload['immediate_objective']
         self.swift_api.too.science_just = observation_payload['science_just']
 
@@ -567,19 +620,20 @@
         #
         self.swift_api.too.exposure = observation_payload['exposure']
         self.swift_api.too.exp_time_just = observation_payload['exp_time_just']
 
         #
         # Monitoring requests
         #
-        self.swift_api.too.num_of_visits = observation_payload['num_of_visits'] # use assignment expression?
+        self.swift_api.too.num_of_visits = observation_payload['num_of_visits']  # use assignment expression?
         if self.swift_api.too.num_of_visits > 1:
             self.swift_api.too.exp_time_per_visit = observation_payload['exp_time_per_visit']
             # construct monitoring_freq from monitoring_freq and monitoring_units e.g '1 hour'
-            self.swift_api.too.monitoring_freq = f"{observation_payload['monitoring_freq']} {observation_payload['monitoring_units']}"
+            self.swift_api.too.monitoring_freq = f"{observation_payload['monitoring_freq']} " \
+                                                 f"{observation_payload['monitoring_units']}"
         else:
             self.swift_api.too.exp_time_per_visit = None
             self.swift_api.too.monitoring_freq = None
 
         #
         # Swift Guest Investigator program parameters
         #
@@ -592,15 +646,15 @@
         if observation_payload['proposal']:
             # this is a Swift Guest Investigator request, so set it's too attributes
             self.swift_api.too.proposal = observation_payload['proposal']
             self.swift_api.too.proposal_id = observation_payload['proposal_id']
             self.swift_api.too.proposal_pi = observation_payload['proposal_pi']
             self.swift_api.too.proposal_trigger_just = observation_payload['proposal_trigger_just']
         else:
-            # just in case there are previously set attributes lingering in the too, reset them
+            # just in case there are previously set attributes lingering in the TOO, reset them
             self.swift_api.too.proposal = False
             self.swift_api.too.proposal_id = None
             self.swift_api.too.proposal_pi = None
             self.swift_api.too.proposal_trigger_just = None
 
         #
         # Instrument mode
@@ -609,156 +663,157 @@
         # Set and unset too.attributes according to the instrument selected.
         if self.swift_api.too.instrument == 'BAT':
             # not sure what to do here!  TODO: find out
             self.swift_api.too.xrt_mode = None
             self.swift_api.too.uvot_mode = None
             self.swift_api.too.uvot_just = None
         elif self.swift_api.too.instrument == 'UVOT':
-            self.swift_api.too.uvot_mode = observation_payload['uvot_mode']
             self.swift_api.too.uvot_just = observation_payload['uvot_just']
             self.swift_api.too.xrt_mode = None
+            if observation_payload['uvot_mode_choices'] == SWIFT_OTHER_CHOICE:
+                # use the value from the uvot_mode text field
+                self.swift_api.too.uvot_mode = observation_payload['uvot_mode']
+            else:
+                # use the value from the drop-down menu
+                self.swift_api.too.uvot_mode = observation_payload['uvot_mode_choices']
         else:
             # XRT mode
             self.swift_api.too.xrt_mode = observation_payload['xrt_mode']
             self.swift_api.too.uvot_mode = None
             self.swift_api.too.uvot_just = None
-        self.swift_api.too.slew_in_place = observation_payload['slew_in_place']
+
+        # WARNING: Setting too.slew_in_place to False causes a timeout error in too.server_validate() !!!
+        if observation_payload['slew_in_place']:
+            self.swift_api.too.slew_in_place = observation_payload['slew_in_place']
+        else:
+            self.swift_api.too.slew_in_place = None  # do NOT slew_in_place to False!!!
 
         #
         # Tiling request
         #
         if observation_payload['tiling']:
             # this is a tiling request to set tiling too attributes
             self.swift_api.too.tiling = observation_payload['tiling']
             self.swift_api.too.number_of_tiles = observation_payload['number_of_tiles']
             self.swift_api.too.exposure_time_per_tile = observation_payload['exposure_time_per_tile']
             # TODO: validation, if exposure_time_per_tile is unset, position_error should be set
             self.swift_api.too.tiling_justification = observation_payload['tiling_justification']
         else:
-            # just in case there are previously set attributes lingering in the too, reset them
+            # just in case there are previously set attributes lingering in the TOO, reset them
             self.swift_api.too.tiling = False
             self.swift_api.too.number_of_tiles = None
             self.swift_api.too.exposure_time_per_tile = None
             self.swift_api.too.tiling_justification = None
 
         #
         # Debug parameter
         #
         self.swift_api.too.debug = observation_payload['debug']
 
         logger.info(f'SwiftFacility._configure_too - configured too:\n{self.swift_api.too}')
 
-
     def validate_observation(self, observation_payload) -> []:
         """Perform a dry-run of submitting the observation.
 
         See submit_observation() for details.
 
         The super class method is absract. No need to call it.
         """
         self._configure_too(observation_payload)
 
         validation_errors = []
         # first, validate the too locally
+        logger.debug(f'validate_observation - calling too.validate():\n{self.swift_api.too}')
         too_is_valid = self.swift_api.too.validate()
         logger.debug(f'validate_observation response: {too_is_valid}')
 
         if too_is_valid:
-            # if the too was internally valid, now validate with the server
-            logger.debug(f'validate_observation - calling too.server_validate()')
+            # if the TOO was internally valid, now validate with the server
+            logger.debug('validate_observation - calling too.server_validate()')
             too_is_server_valid = self.swift_api.too.server_validate()
 
-        #logger.debug(f'validate_observation - too.status: {self.swift_api.too.status}')
-        ##logger.debug(f'validate_observation - dir(too.status): {dir(self.swift_api.too.status)}')
-        #too_status_properties_removed = [
-        #    'clear', 'submit', 'jwt', 'queue',
-        #    'error', 'warning', 'validate',
-        #]
-        #too_status_properties = ['api_data', 'api_name', 'api_version', 'began',
-        #                         'complete', 'completed', 'errors', 'fetchresult',
-        #                         'ignorekeys', 'jobnumber', 'result', 'shared_secret',
-        #                         'status', 'submit_url', 'timeout', 'timestamp',
-        #                         'too_api_dict', 'too_id', 'username', 'warnings']
-        #
-        #for property in too_status_properties:
-        #    logger.debug(f'validate_observation - too.status.{property}: {getattr(self.swift_api.too.status, property)}')
-
         if not (too_is_valid and too_is_server_valid):
             logger.debug(f'validate_observation - too.status.status: {self.swift_api.too.status.status}')
             logger.debug(f'validate_observation - too.status.errors: {self.swift_api.too.status.errors}')
             logger.debug(f'validate_observation - type(too.status.errors): {type(self.swift_api.too.status.errors)}')
-            
+
             validation_errors = self.swift_api.too.status.errors
 
         return validation_errors
 
     def submit_observation(self, observation_payload) -> [()]:
         """Submit the observation to the Swift ToO API
 
         `observation_payload` is the serialized form.cleaned_data
 
-        For the SwiftFacility, sumbitting (or validating) an observation request means
-        instanciating a Swift_TOO object, setting it properties from the observation_payload,
+        For the SwiftFacility, submitting (or validating) an observation request means
+        instantiating a Swift_TOO object, setting it properties from the observation_payload,
         and calling its submit() (or validate()) method. self.too is the Swift_TOO object, whose
-        proerties we need to set.
+        properties we need to set.
 
         returns a list of (field, error) tuples if the observation is invalid
 
-        See https://www.swift.psu.edu/too_api/ for documentation. 
+        See https://www.swift.psu.edu/too_api/ for documentation.
 
         The super class method is absract. No need to call it.
          """
         self._configure_too(observation_payload)
 
         # TODO: remove this for production
         if not self.swift_api.too.debug:
             # while in development, exit early if we're not in debug mode. (i.e. don't submit).
             logger.warning(f'submit_observation - Skipping ACTUAL submission!!! too.debug: {self.swift_api.too.debug}'
                            f' Even though, in the form, Debug is {self.swift_api.too.debug}, it is being reset'
                            f' to True before we call too.submit()')
             self.swift_api.too.debug = True
 
-        logger.debug(f'calling too.submit()')
+        logger.debug('calling too.submit()')
         self.swift_api.too.submit()
-        logger.debug(f'too.submit() returned')
+        logger.debug('too.submit() returned')
 
         logger.info(f'submit_observation - too.status.status: {self.swift_api.too.status.status}')
         logger.info(f'submit_observation - too.status.errors: {self.swift_api.too.status.errors}')
 
         logger.debug(f'submit_observation - too.status: {self.swift_api.too.status}')
 
-        #too_status_properties_removed = [
+        #  too_status_properties_removed = [
         #    'clear', 'submit', 'jwt', 'queue',
         #    'error', 'warning', 'validate',
-        #]
-        #too_status_properties = ['api_data', 'api_name', 'api_version', 'began',
+        #  ]
+        #  too_status_properties = ['api_data', 'api_name', 'api_version', 'began',
         #                         'complete', 'completed', 'errors', 'fetchresult',
         #                         'ignorekeys', 'jobnumber', 'result', 'shared_secret',
         #                         'status', 'submit_url', 'timeout', 'timestamp',
         #                         'too_api_dict', 'too_id', 'username', 'warnings']
         #
-        #for property in too_status_properties:
+        #  for property in too_status_properties:
         #    logger.debug(f'submit_observation - too.status.{property}: {getattr(self.swift_api.too.status, property)}')
 
         too_id = None
         if self.swift_api.too.status.status == 'Accepted':
             too_id = self.swift_api.too.status.too_id
             # this was a successful submission
             logger.info(f'submit_observation - too.status.status: {self.swift_api.too.status.status}')
             logger.info(f'submit_observation - too_id: {too_id}')
 
-            # lets examine the TOO created
+            # let's examine the TOO created
             # see https://www.swift.psu.edu/too_api/index.php?md=Swift TOO Request Example Notebook.ipynb
 
             if self.swift_api.too.debug:
                 # this was a debug submission and thus, no TOO was made and
-                # the too_id returned in the too.status is points to nothing.
-                logger.warning((f'submit_observation - DEBUG submission - too_id: {too_id} is not real.'))
+                # the too_id returned in the too.status points to nothing.
+                logger.warning(f'submit_observation - DEBUG submission - too_id: {too_id} is not real.')
         else:
             logger.error(f'submit_observation - too.status.status: {self.swift_api.too.status.status}')
 
         # TODO: remove this -- it is only for debugging/development
-        #self.swift_api.too.status.too_id = 19529 # an actual NCG1566 TOO
+        #  self.swift_api.too.status.too_id = 19529 #  an actual NCG1566 TOO
 
         return [too_id]
 
-
+    def update_all_observation_statuses(self, target):
+        """This would normaly be implemented by BaseRoboticObservationFacility, but that's
+        not one of our super classes. So, for now, we have a stub implementation here.
+        """
+        failed_records = []
+        logger.warning(f'Swift Facility - update_all_observation_statuses not implemented yet. target: {target}')
+        return failed_records
```

### Comparing `tom_swift-0.2.0a3/tom_swift/swift_api.py` & `tom_swift-0.2.1/tom_swift/swift_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,52 +9,51 @@
   - more notes
 """
 import logging
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 
-from astropy.coordinates import SkyCoord
 from requests.exceptions import ConnectionError
 
 from swifttools.swift_too import TOO, TOORequests, Resolve
 from swifttools.swift_too.api_resolve import Swift_Resolve
 
 from tom_targets.models import Target
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
+
 class SwiftAPI:
     """This is the interface between the SwiftFacility and the swifttools.swift_too classes.
 
-    This keeps the SwiftFacility class focued on implementing it's super class methods and separates
+    This keeps the SwiftFacility class focused on implementing its superclass methods and separates
     the SwiftFacility from the swifttools.swift_too classes.
     """
     def __init__(self, debug=True):
         self.too = TOO()
         self.too_request = TOORequests()
 
-
     def get_credentials(self) -> (str, str):
         """returns username and password from settings.py
 
         Use username and password to set the too.username and too.shared_secret respectively.
         """
         try:
             username = settings.FACILITIES['SWIFT'].get('SWIFT_USERNAME', 'SWIFT_USERNAME not configured')
-            shared_secret = settings.FACILITIES['SWIFT'].get('SWIFT_SHARED_SECRET', 'SWIFT_SHARED_SECRET not configured')
+            shared_secret = settings.FACILITIES['SWIFT'].get('SWIFT_SHARED_SECRET',
+                                                             'SWIFT_SHARED_SECRET not configured')
 
             logger.info(f'swift username: {username}')
-        except KeyError as ex:
-            logger.error(f"'SWIFT' configuration dictionary not defined in settings.FACILITIES")
+        except KeyError:
+            logger.error("'SWIFT' configuration dictionary not defined in settings.FACILITIES")
             raise ImproperlyConfigured
         return username, shared_secret
 
-
     def resolve_target(self, target: Target):
         """
         """
         logger.info(f'resolve_target: {target.name}')
 
         try:
             resolved_target: Swift_Resolve = Resolve(target.name)  # this calls the API
@@ -69,106 +68,156 @@
         if resolved_target is not None:
             for key, value in resolved_target.__dict__.items():
                 logger.debug(f'resolved_target.{key}): {value}')
 
         return resolved_target
 
 
+# define OTHER_CHOICE so it can be used consistently and tested against
+SWIFT_OTHER_CHOICE = 'Other (please specify)'
+
 #
 # Urgency
 #
 SWIFT_URGENCY_CHOICES = [
     (1, 'Within 4 hours (Wakes up the Swift Observatory Duty Scientist).'),
     (2, 'Within 24 hours'),
-    (3, 'Days to a week'), # default
+    (3, 'Days to a week'),  # default
     (4, 'Week to a month'),
 ]
 
 SWIFT_TARGET_CLASSIFICATION_CHOICES = [
     ('AGN', 'AGN'),
     ('Be Binary System', 'Be Binary System'),
-    ('Comet or Asteroid','Comet or Asteroid'),
+    ('Comet or Asteroid', 'Comet or Asteroid'),
     ('Dwarf Nova', 'Dwarf Nova'),
     ('GRB', 'GRB'),
     ('Nova', 'Nova'),
     ('Pulsar', 'Pulsar'),
     ('Supernova', 'Supernova'),
     ('Tidal Disruption Event', 'Tidal Disruption Event'),
     ('X-Ray Transient', 'X-Ray Transient'),
-    ('Other (please specify)', 'Other (please specify)'),
+    (SWIFT_OTHER_CHOICE, SWIFT_OTHER_CHOICE),
 ]
 
+
 #
 # Observation Types
 #
 # Note that:
 # >>> TOO().obs_types
 # ['Spectroscopy', 'Light Curve', 'Position', 'Timing']
-
+#
 def get_observation_type_choices():
     """Returns a list of tuples for the observation type choices.
 
-    Since the TOO() object has propperty describing the valid observation types,
-    use that to create the choices list of tuples (e.g. [('Spectroscopy', 'Spectroscopy'), ('Light Curve', 'Light Curve'), ...]).
+    Since the TOO() object has property describing the valid observation types,
+    use that to create the choices list of tuples (e.g. [('Spectroscopy', 'Spectroscopy'), ('Light Curve',
+    'Light Curve'), ...]).
     """
     observation_type_choices = []
     for obs_type in TOO().obs_types:
         observation_type_choices.append((obs_type, obs_type))
     return observation_type_choices
 
+
 #
 # Instruments
 #
+# could also use TOO().instruments, which is [ 'XRT', 'BAT', 'UVOT']
+# but that doesn't include the full names
 SWIFT_INSTRUMENT_CHOICES = [
     ('UVOT', 'UV/Optical Telescope (UVOT)'),
     ('XRT', 'X-ray Telescope (XRT)'),
     ('BAT', 'Burst Alert Telescope (BAT)'),
 ]
 
+#
+# GRB Detectors
+#
+
+
+def get_grb_detector_choices():
+    """Returns a list of tuples for the GRB detector choices.
+
+    Since the TOO() object has property describing the valid GRB detectors,
+    use that to create the choices list of tuples (e.g. [('Swift/BAT', 'Swift/BAT'), ('Fermi/LAT',
+    'Fermi/LAT'), ...]).
+    """
+    grb_detector_choices = []
+    for mission in TOO().mission_names:
+        if mission != 'ANTARES':
+            grb_detector_choices.append((mission, mission))
+
+    # add the SWIFT_OTHER_CHOICE
+    grb_detector_choices.append((SWIFT_OTHER_CHOICE, SWIFT_OTHER_CHOICE))
+    return grb_detector_choices
+
 
 #
 # XRT Modes
 #
 # XRT modes are converted to numbers. So,
 #    too.xrt_mode = 6
-# and 
+# and
 #    too.xrt_mode = 'WT'
 # are equivalent.
 #
 SWIFT_XRT_MODE_CHOICES = [
-    (0, "Auto"), # picks a mode based on brightness, but if brightness is known, best to pick yourself
-    #(1, "Null"),
-    #(2, "ShortIM"),
-    #(3, "LongIM"),
-    #(4, "PUPD"),
-    #(5, "LRPD"),
+    (0, "Auto"),  # picks a mode based on brightness, but if brightness is known, best to pick yourself
+    # (1, "Null"),
+    # (2, "ShortIM"),
+    # (3, "LongIM"),
+    # (4, "PUPD"),
+    # (5, "LRPD"),
     (6, "Windowed Timing (WT)"),
     (7, "Photon Counting (PC)"),
-    #(8, "Raw"),
-    #(9, "Bias"),
+    # (8, "Raw"),
+    # (9, "Bias"),
 ]
 
 #
 # UVOT Modes
 #
 
-# >>> too.uvot_mode = 0x01AB  # Assign too.uvot_mode as a Hexidecimal number:
+# >>> too.uvot_mode = 0x01AB  # Assign too.uvot_mode as a Hexadecimal number:
 # >>> too.uvot_mode  # It's reported as a Hex string:
 # '0x01ab'
 # >>> type(too.uvot_mode)
 # <class 'str'>
 # Any string will validate:
 # >>> too.uvot_mode = "I think I want all UV filters for this, whatever the UVOT team recommends."
 
+SWIFT_UVOT_FILTER_MODE_CHOICES = [
+    (0x015a, 'uvm2 (0x015a)'),
+    (0x011e, 'uvw2 (0x011e)'),
+    (0x01aa, 'u (0x01aa)'),
+    (0x018c, 'uvw1 (0x018c)'),
+    (0x2016, 'B (0x2016)'),
+    (0x2005, 'V (0x2005)'),
+    (0x2019, 'white (0x2019)'),
+    (0x209a, 'three optical filters (0x209a)'),
+    (0x308f, 'three NUV filters (0x308f)'),
+    (0x30d5, 'four UV/NUV filters (0x30d5)'),
+    (0x30ed, 'standard six-filter blue-weighted mode (0x30ed)'),
+    (0x223f, 'heavily weighted six-filter mode; for supernovae and very red objects (0x223f)'),
+    (0x2241, 'all seven optical/UV filters (0x2241)'),
+    (0x0270, ('unscaled six-filter mode to get 6 broadband filters in AT observations with'
+              ' snapshot lengths > 1000s (0x0270)')),
+    (0x9999, 'Filter of the Day (0x9999)'),
+    (SWIFT_OTHER_CHOICE, SWIFT_OTHER_CHOICE),
+]
+
+
 #
 # Monitoring
 #
 def get_monitoring_unit_choices():
     """Returns a list of tuples for the monitoring frequency unit choices.
 
-    Since the TOO() object has propperty describing the valid monitoring frequency units,
+    Since the TOO() object has property describing the valid monitoring frequency units,
     use that to create the choices list of tuples (e.g. [('day', 'day'), ('week', 'week'), ...]).
     """
     monitoring_unit_choices = []
     for unit in TOO().monitoring_units:
-        monitoring_unit_choices.append((unit, unit))
-    return monitoring_unit_choices
+        monitoring_unit_choices.append((unit, f'{unit}(s)'))
+    return monitoring_unit_choices
```

### Comparing `tom_swift-0.2.0a3/tom_swift/templates/tom_swift/observation_form.html` & `tom_swift-0.2.1/tom_swift/templates/tom_swift/observation_form.html`

 * *Files 20% similar despite different names*

```diff
@@ -7,31 +7,43 @@
 {% endblock %}
 {% block content %}
 
 <script>
 function showHideTargetClassificationFields() {
     const target_classification = document.getElementById('id_target_classification_choices').options[document.getElementById('id_target_classification_choices').selectedIndex].value;
     switch (target_classification) {
-        case 'Other (please specify)':
+        case 'Other (please specify)': // define as SWIFT_OTHER_CHOICE in swift_api.py
             // in this case show the target_classification CharField
             document.getElementById('div_id_target_classification').style.display = '';
             // and hide the grb_detector and grb_triggertime fields
+            document.getElementById('div_id_grb_detector_choices').style.display = 'none';
             document.getElementById('div_id_grb_detector').style.display = 'none';
             document.getElementById('div_id_grb_triggertime').style.display = 'none';
             break;
         case 'GRB':
             // in this case show the grb_detector and grb_triggertime fields
-            document.getElementById('div_id_grb_detector').style.display = '';
+            document.getElementById('div_id_grb_detector_choices').style.display = '';
+            // we do the other-please-specify dance if they want an Other GRB Detector
+            const grb_detector_choice = document.getElementById('id_grb_detector_choices').options[document.getElementById('id_grb_detector_choices').selectedIndex].value;
+            if (grb_detector_choice == 'Other (please specify)') {
+                // in this case show the grb_detector CharField
+                document.getElementById('div_id_grb_detector').style.display = '';
+            } else {
+                // in this case hide the grb_detector CharField
+                document.getElementById('div_id_grb_detector').style.display = 'none';
+            }
+
             document.getElementById('div_id_grb_triggertime').style.display = '';
             // and hide the target_classification CharField
             document.getElementById('div_id_target_classification').style.display = 'none';
             break;
         default:
             // in this case hide all the extra fields
             document.getElementById('div_id_target_classification').style.display = 'none';
+            document.getElementById('div_id_grb_detector_choices').style.display = 'none';
             document.getElementById('div_id_grb_detector').style.display = 'none';
             document.getElementById('div_id_grb_triggertime').style.display = 'none';
             break;
     }
 };
 
 function showHideMonitoringFields() {
@@ -53,28 +65,36 @@
     const inst = document.getElementById('id_instrument').options[document.getElementById('id_instrument').selectedIndex].value;
     switch (inst) {
         case 'XRT':
             console.log('XRT instrument selected');
             // show the xrt_mode field; hide the UVOT fields
             document.getElementById('div_id_xrt_mode').style.display = '';
             document.getElementById('div_id_uvot_mode').style.display = 'none';
+            document.getElementById('div_id_uvot_mode_choices').style.display = 'none';
             document.getElementById('div_id_uvot_just').style.display = 'none';
             break;
         case 'UVOT':
             console.log('UVOT instrument selected');
             // show the uvot_mode and uvot_just fields; hide the xrt_mode fields
-            document.getElementById('div_id_uvot_mode').style.display = '';
+            const uvot_mode = document.getElementById('id_uvot_mode_choices').options[document.getElementById('id_uvot_mode_choices').selectedIndex].value;
+            if (uvot_mode == 'Other (please specify)') {
+                document.getElementById('div_id_uvot_mode').style.display = '';
+            } else {
+                document.getElementById('div_id_uvot_mode').style.display = 'none';
+            }
+            document.getElementById('div_id_uvot_mode_choices').style.display = '';
             document.getElementById('div_id_uvot_just').style.display = '';
             document.getElementById('div_id_xrt_mode').style.display = 'none';
             break;
         case 'BAT':
             console.log('BAT instrument selected');
             // not sure what to show or hide here (hide everything?)
             document.getElementById('div_id_xrt_mode').style.display = 'none';
             document.getElementById('div_id_uvot_mode').style.display = 'none';
+            document.getElementById('div_id_uvot_mode_choices').style.display = 'none';
             document.getElementById('div_id_uvot_just').style.display = 'none';
             break;
     }
 };
 
 function showHideTilingFields() {
     if (document.getElementById('id_tiling').checked) {
@@ -104,27 +124,31 @@
         // hide the proposal fields
         document.getElementById('div_id_proposal_id').style.display = 'none';
         document.getElementById('div_id_proposal_pi').style.display = 'none';
         document.getElementById('div_id_proposal_trigger_just').style.display = 'none';
     }
 };
 
+function showExposureAccordianOnError() {
+    const exposureAccordion = document.getElementById('exposure-visit-information');
+    exposureAccordion.classList.add('show');
+}
 </script>
 
 <script type="text/javascript">
     window.addEventListener("load", showHideTargetClassificationFields);
     window.addEventListener("load", showHideMonitoringFields);
     window.addEventListener("load", showHideInstrumentModeFields);
     window.addEventListener("load", showHideTilingFields);
     window.addEventListener("load", showHideSwiftGIProposalFields);
 </script>
 <!-- see also script element at end of file -->
 
 {{ form|as_crispy_errors }}
-<h1>Submit Request to Neil Gehrels Swift Observatory</h1>
+<h1>Submit Request to Neil Gehrels Swift Observatory for <a href="{% url 'targets:detail' pk=target.id %}">{{target.name}}</a></h1>
 
 
 {% if target.type == 'SIDEREAL' %}
 <div class="row">
     <div class="col">
         <p>This is where we might put some visibility windows.</p>
     </div>
@@ -145,16 +169,16 @@
             <dd class="col-sm-6">{{ resolved_target_name }}</dd>
             <dt class="col-sm-6">Right Ascension</dt>
             <dd class="col-sm-6">{{ resolved_target_ra|floatformat:4 }}</dd>
             <dt class="col-sm-6">Declination</dt>
             <dd class="col-sm-6">{{ resolved_target_dec|floatformat:4 }}</dd>
         </dl>
         <hr>
-        <!-- display tom_swift Facility verison -->
-        <p><em>TOM Toolit Facility (<a href="https://github.com/TOMToolkit/tom_swift">tom_swift</a>) version {{ version }}</em></p>
+        <!-- display tom_swift Facility version -->
+        <p><em>TOM Toolkit Facility (<a target="_blank" href="https://github.com/TOMToolkit/tom_swift">tom_swift</a>) version {{ version }}</em></p>
     </div>
     <!-- Column 2 -->
     <div class="col-md-6">
         <!-- Nav tabs -->
         <ul class="nav nav-tabs" id="tabs">
         {% for observation_type, observation_form in observation_type_choices %}
             <li class="nav-item">
@@ -176,23 +200,36 @@
 </div>
 
 <!-- this must at the end or else the elements can't be found and then the eventListener
      can't be added
  -->
 <script type="text/javascript">
     var el1 = document.getElementById("div_id_target_classification_choices");
-    el1.addEventListener("click", showHideTargetClassificationFields);
+    el1.addEventListener("change", showHideTargetClassificationFields);
 
     var el2 = document.getElementById("div_id_instrument");
-    el2.addEventListener("click", showHideInstrumentModeFields);
+    el2.addEventListener("change", showHideInstrumentModeFields);
+
+    var el7 = document.getElementById("div_id_uvot_mode_choices");
+    el7.addEventListener("change", showHideInstrumentModeFields);
 
     var el3 = document.getElementById("div_id_num_of_visits");
-    el3.addEventListener("click", showHideMonitoringFields);
+    el3.addEventListener("change", showHideMonitoringFields);
 
     var el4 = document.getElementById("div_id_tiling");
-    el4.addEventListener("click", showHideTilingFields);
+    el4.addEventListener("change", showHideTilingFields);
 
     var el5 = document.getElementById("div_id_proposal");
-    el5.addEventListener("click", showHideSwiftGIProposalFields);
+    el5.addEventListener("change", showHideSwiftGIProposalFields);
+
+    var el6 = document.getElementById("div_id_grb_detector_choices");
+    //el6.addEventListener("click", showHideGRBDetectionFields);
+    el6.addEventListener("change", showHideTargetClassificationFields);
+
+    var el7 = document.getElementById("id_exposure");
+    el7.addEventListener("invalid", showExposureAccordianOnError);
+
+    var el8 = document.getElementById("id_exp_time_just");
+    el8.addEventListener("invalid", showExposureAccordianOnError);
 </script>
 
-{% endblock %}
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 {% extends 'tom_common/base.html' %} {% load bootstrap4 static
 crispy_forms_tags observation_extras targets_extras %} {% block title %}Submit
 Observation{% endblock %} {% block additional_css %}
 {% endblock %} {% block content %}
 {{ form|as_crispy_errors }}
-************ SSuubbmmiitt RReeqquueesstt ttoo NNeeiill GGeehhrreellss SSwwiifftt OObbsseerrvvaattoorryy ************
+************ SSuubbmmiitt RReeqquueesstt ttoo NNeeiill GGeehhrreellss SSwwiifftt OObbsseerrvvaattoorryy ffoorr _{{_{{_tt_aa_rr_gg_ee_tt_.._nn_aa_mm_ee_}}_}}
+************
 {% if target.type == 'SIDEREAL' %}
 This is where we might put some visibility windows.
 {% endif %}
 SSuubbmmiittttiinngg ccrreeddeennttiiaall:: {{{{ uusseerrnnaammee }}}}
 ===============================================================================
 ****** TTaarrggeett IInnffoorrmmaattiioonn ******
 {% target_data target %}
@@ -16,15 +17,15 @@
   Resolved Name
       {{ resolved_target_name }}
   Right Ascension
       {{ resolved_target_ra|floatformat:4 }}
   Declination
       {{ resolved_target_dec|floatformat:4 }}
 ===============================================================================
-TTOOMM TToooolliitt FFaacciilliittyy ((_tt_oo_mm____ss_ww_ii_ff_tt)) vveerrssiioonn {{{{ vveerrssiioonn }}}}
+TTOOMM TToooollkkiitt FFaacciilliittyy ((_tt_oo_mm____ss_ww_ii_ff_tt)) vveerrssiioonn {{{{ vveerrssiioonn }}}}
     * {% for observation_type, observation_form in observation_type_choices %}
     * {{ observation_type }}
     * {% endfor %}
 {% for observation_type, observation_form in observation_type_choices %}
 {% crispy observation_form %}
 {% endfor %}
 {% endblock %}
```

### Comparing `tom_swift-0.2.0a3/PKG-INFO` & `tom_swift-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: tom-swift
-Version: 0.2.0a3
+Version: 0.2.1
 Summary: TOM Toolkit Facility module for the Neil Gehrels Swift Observatory
 License: GPL-3.0-or-later
 Author: Lindy Lindstrom
 Author-email: llindstrom@lco.global
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: BatAnalysis (>=1.0,<2.0)
-Requires-Dist: tomtoolkit (>=2.14,<3.0)
+Requires-Dist: swifttools (<4)
+Requires-Dist: tomtoolkit (>=2.15)
 Description-Content-Type: text/markdown
 
 # tom_swift
-_Note: This repository is under active development. It is a not-yet-functional, work in progress._
-
 [Neil Gehrels Swift Observatory](https://swift.gsfc.nasa.gov/index.html) facility module for TOM Toolkit. This module uses the
 [Swift TOO API](https://www.swift.psu.edu/too_api/) for all its interactions with the _Swift_ Observatory. When installed and
 configured, your TOM can query target visibility, submit TOO observation requests to Swift, and check TOO observation status.
 
 ## Swift TOO Prerequisites
 In order to submit TOO requests to Swift, you must [register with the Swift TOO system](https://www.swift.psu.edu/toop/too_newuser.php).
 Once you are registered and have logged in, you can [get your shared secret](https://www.swift.psu.edu/toop/change_secret.php), which you
@@ -32,23 +29,32 @@
 
 Install the module into your TOM environment:
 
 ```shell
 pip install tom-swift
 ```
 
-Add `tom_swift.swift.SwiftFacility` to the `TOM_FACILITY_CLASSES` in your TOM's
+1. In your project `settings.py`, add `tom_swift` to your `INSTALLED_APPS` setting:
+
+    ```python
+    INSTALLED_APPS = [
+        ...
+        'tom_swift',
+    ]
+    ```
+
+2. Add `tom_swift.swift.SwiftFacility` to the `TOM_FACILITY_CLASSES` in your TOM's
 `settings.py`:
-```python
+   ```python
     TOM_FACILITY_CLASSES = [
         'tom_observations.facilities.lco.LCOFacility',
         ...
         'tom_swift.swift.SwiftFacility',
     ]
-```
+   ```   
 
 ## Configuration
 
 Include the following settings inside the `FACILITIES` dictionary inside `settings.py`:
 
 ```python
     FACILITIES = {
```

