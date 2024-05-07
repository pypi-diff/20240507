# Comparing `tmp/dmarc-1.0.5.tar.gz` & `tmp/dmarc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmarc-1.0.5.tar", last modified: Sun Apr  7 16:31:26 2024, max compression
+gzip compressed data, was "dmarc-1.1.0.tar", last modified: Tue May  7 11:43:18 2024, max compression
```

## Comparing `dmarc-1.0.5.tar` & `dmarc-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,35 @@
-drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-04-07 16:31:26.864894 dmarc-1.0.5/
--rw-r--r--   0 dusan      (501) staff       (20)     1091 2023-12-23 04:27:57.000000 dmarc-1.0.5/LICENSE
--rw-r--r--   0 dusan      (501) staff       (20)     3274 2024-04-07 16:31:26.863559 dmarc-1.0.5/PKG-INFO
--rw-r--r--   0 dusan      (501) staff       (20)     2250 2024-04-06 17:40:27.000000 dmarc-1.0.5/README.md
-drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-04-07 16:31:26.842983 dmarc-1.0.5/dmarc/
--rw-r--r--   0 dusan      (501) staff       (20)    21966 2024-04-07 16:09:53.000000 dmarc-1.0.5/dmarc/__init__.py
--rw-r--r--   0 dusan      (501) staff       (20)     1306 2024-03-23 19:44:51.000000 dmarc-1.0.5/dmarc/ar.py
--rw-r--r--   0 dusan      (501) staff       (20)      983 2024-03-22 18:33:19.000000 dmarc-1.0.5/dmarc/asyncresolver.py
--rw-r--r--   0 dusan      (501) staff       (20)      271 2024-03-23 21:26:06.000000 dmarc-1.0.5/dmarc/psl.py
--rw-r--r--   0 dusan      (501) staff       (20)     1259 2024-03-21 21:48:07.000000 dmarc-1.0.5/dmarc/resolver.py
-drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-04-07 16:31:26.856776 dmarc-1.0.5/dmarc/tests/
--rw-r--r--   0 dusan      (501) staff       (20)        0 2024-04-04 14:53:57.000000 dmarc-1.0.5/dmarc/tests/__init__.py
--rw-r--r--   0 dusan      (501) staff       (20)     1045 2024-04-04 16:02:36.000000 dmarc-1.0.5/dmarc/tests/test_ar.py
--rw-r--r--   0 dusan      (501) staff       (20)      516 2024-04-04 15:56:02.000000 dmarc-1.0.5/dmarc/tests/test_asyncresolver.py
--rw-r--r--   0 dusan      (501) staff       (20)     7317 2024-04-07 15:39:42.000000 dmarc-1.0.5/dmarc/tests/test_dmarc.py
--rw-r--r--   0 dusan      (501) staff       (20)      441 2024-04-04 18:59:04.000000 dmarc-1.0.5/dmarc/tests/test_psl.py
--rw-r--r--   0 dusan      (501) staff       (20)      472 2024-04-04 15:59:24.000000 dmarc-1.0.5/dmarc/tests/test_resolver.py
-drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-04-07 16:31:26.860629 dmarc-1.0.5/dmarc.egg-info/
--rw-r--r--   0 dusan      (501) staff       (20)     3274 2024-04-07 16:31:26.000000 dmarc-1.0.5/dmarc.egg-info/PKG-INFO
--rw-r--r--   0 dusan      (501) staff       (20)      414 2024-04-07 16:31:26.000000 dmarc-1.0.5/dmarc.egg-info/SOURCES.txt
--rw-r--r--   0 dusan      (501) staff       (20)        1 2024-04-07 16:31:26.000000 dmarc-1.0.5/dmarc.egg-info/dependency_links.txt
--rw-r--r--   0 dusan      (501) staff       (20)       57 2024-04-07 16:31:26.000000 dmarc-1.0.5/dmarc.egg-info/requires.txt
--rw-r--r--   0 dusan      (501) staff       (20)        6 2024-04-07 16:31:26.000000 dmarc-1.0.5/dmarc.egg-info/top_level.txt
--rw-r--r--   0 dusan      (501) staff       (20)       38 2024-04-07 16:31:26.865174 dmarc-1.0.5/setup.cfg
--rw-r--r--   0 dusan      (501) staff       (20)     1205 2024-04-07 16:00:27.000000 dmarc-1.0.5/setup.py
+drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-05-07 11:43:18.427288 dmarc-1.1.0/
+-rw-r--r--   0 dusan      (501) staff       (20)     1091 2023-12-23 04:27:57.000000 dmarc-1.1.0/LICENSE
+-rw-r--r--   0 dusan      (501) staff       (20)     3295 2024-05-07 11:43:18.426547 dmarc-1.1.0/PKG-INFO
+-rw-r--r--   0 dusan      (501) staff       (20)     2268 2024-05-07 11:34:53.000000 dmarc-1.1.0/README.md
+drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-05-07 11:43:18.401920 dmarc-1.1.0/dmarc/
+-rw-r--r--   0 dusan      (501) staff       (20)    20332 2024-05-07 11:34:53.000000 dmarc-1.1.0/dmarc/__init__.py
+-rw-r--r--   0 dusan      (501) staff       (20)     1165 2024-05-07 11:34:53.000000 dmarc-1.1.0/dmarc/ar.py
+-rw-r--r--   0 dusan      (501) staff       (20)     1007 2024-05-07 11:34:53.000000 dmarc-1.1.0/dmarc/asyncresolver.py
+-rw-r--r--   0 dusan      (501) staff       (20)      351 2024-05-07 11:34:53.000000 dmarc-1.1.0/dmarc/psl.py
+drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-05-07 11:43:18.408239 dmarc-1.1.0/dmarc/report/
+-rw-r--r--   0 dusan      (501) staff       (20)     5772 2024-05-07 11:34:53.000000 dmarc-1.1.0/dmarc/report/__init__.py
+drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-05-07 11:43:18.410551 dmarc-1.1.0/dmarc/report/schemas/
+-rw-r--r--   0 dusan      (501) staff       (20)     9256 2024-05-07 11:34:53.000000 dmarc-1.1.0/dmarc/report/schemas/dmarc-relaxed.xsd
+-rw-r--r--   0 dusan      (501) staff       (20)     9067 2024-05-07 11:34:53.000000 dmarc-1.1.0/dmarc/report/schemas/dmarc.xsd
+-rw-r--r--   0 dusan      (501) staff       (20)     1294 2024-05-07 11:34:53.000000 dmarc-1.1.0/dmarc/resolver.py
+drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-05-07 11:43:18.420710 dmarc-1.1.0/dmarc/tests/
+-rw-r--r--   0 dusan      (501) staff       (20)        0 2024-04-04 14:53:57.000000 dmarc-1.1.0/dmarc/tests/__init__.py
+drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-05-07 11:43:18.422570 dmarc-1.1.0/dmarc/tests/report/
+-rw-r--r--   0 dusan      (501) staff       (20)        0 2024-05-07 11:34:53.000000 dmarc-1.1.0/dmarc/tests/report/__init__.py
+drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-05-07 11:43:18.423933 dmarc-1.1.0/dmarc/tests/report/data/
+-rw-r--r--   0 dusan      (501) staff       (20)     1838 2024-05-07 11:34:53.000000 dmarc-1.1.0/dmarc/tests/report/data/samplereport.xml
+-rw-r--r--   0 dusan      (501) staff       (20)     4705 2024-05-07 11:34:53.000000 dmarc-1.1.0/dmarc/tests/report/test_report.py
+-rw-r--r--   0 dusan      (501) staff       (20)     1045 2024-04-04 16:02:36.000000 dmarc-1.1.0/dmarc/tests/test_ar.py
+-rw-r--r--   0 dusan      (501) staff       (20)      516 2024-04-04 15:56:02.000000 dmarc-1.1.0/dmarc/tests/test_asyncresolver.py
+-rw-r--r--   0 dusan      (501) staff       (20)     7317 2024-04-07 15:39:42.000000 dmarc-1.1.0/dmarc/tests/test_dmarc.py
+-rw-r--r--   0 dusan      (501) staff       (20)      441 2024-04-04 18:59:04.000000 dmarc-1.1.0/dmarc/tests/test_psl.py
+-rw-r--r--   0 dusan      (501) staff       (20)      472 2024-04-04 15:59:24.000000 dmarc-1.1.0/dmarc/tests/test_resolver.py
+drwxr-xr-x   0 dusan      (501) staff       (20)        0 2024-05-07 11:43:18.425022 dmarc-1.1.0/dmarc.egg-info/
+-rw-r--r--   0 dusan      (501) staff       (20)     3295 2024-05-07 11:43:18.000000 dmarc-1.1.0/dmarc.egg-info/PKG-INFO
+-rw-r--r--   0 dusan      (501) staff       (20)      615 2024-05-07 11:43:18.000000 dmarc-1.1.0/dmarc.egg-info/SOURCES.txt
+-rw-r--r--   0 dusan      (501) staff       (20)        1 2024-05-07 11:43:18.000000 dmarc-1.1.0/dmarc.egg-info/dependency_links.txt
+-rw-r--r--   0 dusan      (501) staff       (20)       77 2024-05-07 11:43:18.000000 dmarc-1.1.0/dmarc.egg-info/requires.txt
+-rw-r--r--   0 dusan      (501) staff       (20)        6 2024-05-07 11:43:18.000000 dmarc-1.1.0/dmarc.egg-info/top_level.txt
+-rw-r--r--   0 dusan      (501) staff       (20)       38 2024-05-07 11:43:18.427472 dmarc-1.1.0/setup.cfg
+-rw-r--r--   0 dusan      (501) staff       (20)     1250 2024-05-07 11:34:53.000000 dmarc-1.1.0/setup.py
```

### Comparing `dmarc-1.0.5/LICENSE` & `dmarc-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dmarc-1.0.5/PKG-INFO` & `dmarc-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: dmarc
-Version: 1.0.5
+Version: 1.1.0
 Summary: Parse and evaluate DMARC email authentication policy
 Home-page: https://gitlab.com/duobradovic/pydmarc
 Author: Dusan Obradovic
 Author-email: dusan@euracks.net
 License: MIT
-Keywords: dkim,spf,dmarc,email,authentication,rfc5451,rfc7001,rfc7601,rfc8601
+Keywords: dkim,spf,dmarc,email,authentication,rfc7489,rfc8601
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Communications :: Email :: Mail Transport Agents
 Classifier: Topic :: Communications :: Email :: Filters
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=2.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: resolver
 Requires-Dist: dnspython; extra == "resolver"
 Provides-Extra: ar
 Requires-Dist: authres; extra == "ar"
 Provides-Extra: psl
 Requires-Dist: publicsuffix2; extra == "psl"
+Provides-Extra: report
+Requires-Dist: xmlschema; extra == "report"
 
 # DMARC (Domain-based Message Authentication, Reporting & Conformance)
 
 DMARC email authentication module implemented in Python.
 
 ## Installation
 
@@ -39,24 +40,24 @@
 
 ## Usage
 
 ```python
 >>> import dmarc
 >>>
 >>> # Represent verified SPF and DKIM status
->>> aspf = dmarc.SPF(domain='news.example.com', result=dmarc.SPF_PASS)
+>>> aspf = dmarc.SPF(domain='news.example.com', result=dmarc.SPFResult.PASS)
 >>> #aspf = dmarc.SPF.from_authres(SPFAuthenticationResult(result='pass', smtp_mailfrom='email@news.example.com'))
 >>> 
->>> adkim = dmarc.DKIM(domain='example.com', result=dmarc.DKIM_PASS)
+>>> adkim = dmarc.DKIM(domain='example.com', result=dmarc.DKIMResult.PASS)
 >>> #adkim = dmarc.DKIM.from_authres(DKIMAuthenticationResult(result='pass', header_d='example.com'))
 >>>
 >>> try:
 ...     admarc = dmarc.DMARCPolicy(record='v=DMARC1; p=reject;', domain='example.com')
 ...     admarc.verify(spf=aspf, dkim=adkim)
-...     #admarc.verify(auth_results=[aspf, adkim, dmarc.DKIM('news.example.com', dmarc.DKIM_FAIL)])
+...     #admarc.verify(auth_results=[aspf, adkim, dmarc.DKIM('news.example.com', dmarc.DKIMResult.FAIL)])
 ...     adict = admarc.result.as_dict() # dict repr
 ... except dmarc.PolicyNoneError:
 ...     pass
 ... except dmarc.PolicyQuarantineError:
 ...     raise
 ... except dmarc.PolicyRejectError:
 ...     raise
```

### Comparing `dmarc-1.0.5/README.md` & `dmarc-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 
 ## Usage
 
 ```python
 >>> import dmarc
 >>>
 >>> # Represent verified SPF and DKIM status
->>> aspf = dmarc.SPF(domain='news.example.com', result=dmarc.SPF_PASS)
+>>> aspf = dmarc.SPF(domain='news.example.com', result=dmarc.SPFResult.PASS)
 >>> #aspf = dmarc.SPF.from_authres(SPFAuthenticationResult(result='pass', smtp_mailfrom='email@news.example.com'))
 >>> 
->>> adkim = dmarc.DKIM(domain='example.com', result=dmarc.DKIM_PASS)
+>>> adkim = dmarc.DKIM(domain='example.com', result=dmarc.DKIMResult.PASS)
 >>> #adkim = dmarc.DKIM.from_authres(DKIMAuthenticationResult(result='pass', header_d='example.com'))
 >>>
 >>> try:
 ...     admarc = dmarc.DMARCPolicy(record='v=DMARC1; p=reject;', domain='example.com')
 ...     admarc.verify(spf=aspf, dkim=adkim)
-...     #admarc.verify(auth_results=[aspf, adkim, dmarc.DKIM('news.example.com', dmarc.DKIM_FAIL)])
+...     #admarc.verify(auth_results=[aspf, adkim, dmarc.DKIM('news.example.com', dmarc.DKIMResult.FAIL)])
 ...     adict = admarc.result.as_dict() # dict repr
 ... except dmarc.PolicyNoneError:
 ...     pass
 ... except dmarc.PolicyQuarantineError:
 ...     raise
 ... except dmarc.PolicyRejectError:
 ...     raise
```

### Comparing `dmarc-1.0.5/dmarc/ar.py` & `dmarc-1.1.0/dmarc/ar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 from authres import AuthenticationResultsHeader, AuthenticationResultProperty, SPFAuthenticationResult, DKIMAuthenticationResult, AuthResError
 from authres.dmarc import DMARCAuthenticationResult
-from . import POLICY_PASS, POLICY_FAIL
 
-def authres(result=None, **kwargs):
+def authres(result=None, **kwargs) -> DMARCAuthenticationResult:
     """This is a convenience factory function that uses the dmarc.Result object
     to make the DMARCAuthenticationResult object.
     
     Args:
         result: dmarc.Result object
     
     Returns:
         DMARCAuthenticationResult object
     """
     kwargs['result'] = 'none'
     if result:
+        kwargs['result'] = result.result.value
         adict = result.as_dict()
         policy_published = adict['policy_published']
         policy_evaluated = adict['record']['row']['policy_evaluated']
-        
-        if result.result == POLICY_PASS:
-            kwargs['result'] = 'pass'
-        elif result.result == POLICY_FAIL:
-            kwargs['result'] = 'fail'
-        
         kwargs['result_comment'] = ' '.join('{0}=%({1})s'.format(key,key) for key in policy_published) % policy_published
         kwargs['header_from'] = result.policy.domain
         kwargs['policy'] = policy_evaluated['disposition']
         kwargs['policy_comment'] = ' '.join('{0}=%({1})s'.format(key,key) for key in policy_evaluated) % policy_evaluated
     
     return DMARCAuthenticationResult(**kwargs)
```

### Comparing `dmarc-1.0.5/dmarc/asyncresolver.py` & `dmarc-1.1.0/dmarc/asyncresolver.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,19 +10,27 @@
     ... except RecordMultiFoundError:
     ...     raise # permerror
     ... except RecordResolverError:
     ...     raise # temperror
     ... 
 """
 
-from dns.asyncresolver import resolve as resolver, NXDOMAIN, NoAnswer
-from dns.exception import DNSException
-from .resolver import response, RecordResolverError, RecordNotFoundError, RecordNoDataError, RecordMultiFoundError
+from dns.asyncresolver import resolve as resolver
+from .resolver import (
+    response,
+    DNSException,
+    NXDOMAIN,
+    NoAnswer,
+    RecordResolverError,
+    RecordNotFoundError,
+    RecordNoDataError,
+    RecordMultiFoundError,
+)
 
-async def resolve(domain):
+async def resolve(domain: str) -> str:
     try:
         answers = await resolver('_dmarc.{0}'.format(domain), 'TXT')
         return response(answers)
     except NXDOMAIN as err:
         raise RecordNotFoundError(err)
     except NoAnswer as err:
         raise RecordNoDataError(err)
```

### Comparing `dmarc-1.0.5/dmarc/resolver.py` & `dmarc-1.1.0/dmarc/resolver.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     ... except RecordMultiFoundError:
     ...     raise # permerror
     ... except RecordResolverError:
     ...     raise # temperror
     ... 
 """
 
-from dns.resolver import resolve as resolver, NXDOMAIN, NoAnswer
+from dns.resolver import resolve as resolver, NXDOMAIN, NoAnswer, Answer
 from dns.exception import DNSException
 from . import Error
 
 class RecordResolverError(Error):
     pass
 
 class RecordNotFoundError(RecordResolverError):
@@ -26,23 +26,23 @@
 
 class RecordMultiFoundError(RecordResolverError):
     pass
 
 class RecordNoDataError(RecordNotFoundError):
     pass
 
-def resolve(domain):
+def resolve(domain: str) -> str:
     try:
         answers = resolver('_dmarc.{0}'.format(domain), 'TXT')
         return response(answers)
     except NXDOMAIN as err:
         raise RecordNotFoundError(err)
     except NoAnswer as err:
         raise RecordNoDataError(err)
     except DNSException as err:
         raise RecordResolverError(err)
 
-def response(answers):
+def response(answers: Answer) -> str:
     if len(answers) > 1:
         raise RecordMultiFoundError('A domain can only have one DMARC record.')
     return b''.join(answers[0].strings).decode()
```

### Comparing `dmarc-1.0.5/dmarc/tests/test_ar.py` & `dmarc-1.1.0/dmarc/tests/test_ar.py`

 * *Files identical despite different names*

### Comparing `dmarc-1.0.5/dmarc/tests/test_asyncresolver.py` & `dmarc-1.1.0/dmarc/tests/test_asyncresolver.py`

 * *Files identical despite different names*

### Comparing `dmarc-1.0.5/dmarc/tests/test_dmarc.py` & `dmarc-1.1.0/dmarc/tests/test_dmarc.py`

 * *Files identical despite different names*

### Comparing `dmarc-1.0.5/dmarc.egg-info/PKG-INFO` & `dmarc-1.1.0/dmarc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: dmarc
-Version: 1.0.5
+Version: 1.1.0
 Summary: Parse and evaluate DMARC email authentication policy
 Home-page: https://gitlab.com/duobradovic/pydmarc
 Author: Dusan Obradovic
 Author-email: dusan@euracks.net
 License: MIT
-Keywords: dkim,spf,dmarc,email,authentication,rfc5451,rfc7001,rfc7601,rfc8601
+Keywords: dkim,spf,dmarc,email,authentication,rfc7489,rfc8601
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Communications :: Email :: Mail Transport Agents
 Classifier: Topic :: Communications :: Email :: Filters
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=2.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: resolver
 Requires-Dist: dnspython; extra == "resolver"
 Provides-Extra: ar
 Requires-Dist: authres; extra == "ar"
 Provides-Extra: psl
 Requires-Dist: publicsuffix2; extra == "psl"
+Provides-Extra: report
+Requires-Dist: xmlschema; extra == "report"
 
 # DMARC (Domain-based Message Authentication, Reporting & Conformance)
 
 DMARC email authentication module implemented in Python.
 
 ## Installation
 
@@ -39,24 +40,24 @@
 
 ## Usage
 
 ```python
 >>> import dmarc
 >>>
 >>> # Represent verified SPF and DKIM status
->>> aspf = dmarc.SPF(domain='news.example.com', result=dmarc.SPF_PASS)
+>>> aspf = dmarc.SPF(domain='news.example.com', result=dmarc.SPFResult.PASS)
 >>> #aspf = dmarc.SPF.from_authres(SPFAuthenticationResult(result='pass', smtp_mailfrom='email@news.example.com'))
 >>> 
->>> adkim = dmarc.DKIM(domain='example.com', result=dmarc.DKIM_PASS)
+>>> adkim = dmarc.DKIM(domain='example.com', result=dmarc.DKIMResult.PASS)
 >>> #adkim = dmarc.DKIM.from_authres(DKIMAuthenticationResult(result='pass', header_d='example.com'))
 >>>
 >>> try:
 ...     admarc = dmarc.DMARCPolicy(record='v=DMARC1; p=reject;', domain='example.com')
 ...     admarc.verify(spf=aspf, dkim=adkim)
-...     #admarc.verify(auth_results=[aspf, adkim, dmarc.DKIM('news.example.com', dmarc.DKIM_FAIL)])
+...     #admarc.verify(auth_results=[aspf, adkim, dmarc.DKIM('news.example.com', dmarc.DKIMResult.FAIL)])
 ...     adict = admarc.result.as_dict() # dict repr
 ... except dmarc.PolicyNoneError:
 ...     pass
 ... except dmarc.PolicyQuarantineError:
 ...     raise
 ... except dmarc.PolicyRejectError:
 ...     raise
```

### Comparing `dmarc-1.0.5/setup.py` & `dmarc-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dmarc",
-    version="1.0.5",
+    version="1.1.0",
     author="Dusan Obradovic",
     author_email="dusan@euracks.net",
     description="Parse and evaluate DMARC email authentication policy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     url="https://gitlab.com/duobradovic/pydmarc",
     packages=setuptools.find_packages(),
-    keywords = ['dkim', 'spf', 'dmarc', 'email', 'authentication', 'rfc5451', 'rfc7001', 'rfc7601', 'rfc8601'],
+    package_data={"dmarc": ["report/schemas/*.xsd", "tests/report/data/*.xml"]},
+    keywords = ['dkim', 'spf', 'dmarc', 'email', 'authentication', 'rfc7489', 'rfc8601'],
     classifiers=[
         "Intended Audience :: Developers",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Communications :: Email :: Mail Transport Agents",
         "Topic :: Communications :: Email :: Filters",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
-    python_requires='>=2.7',
+    python_requires='>=3.9',
     extras_require={
         "resolver": ['dnspython'],
         "ar": ['authres'],
         "psl": ['publicsuffix2'],
+        "report": ['xmlschema'],
     },
 )
```

