# Comparing `tmp/composo-0.1.35.tar.gz` & `tmp/composo-0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composo-0.1.35.tar", last modified: Wed Mar  6 17:54:24 2024, max compression
+gzip compressed data, was "composo-0.1.37.tar", last modified: Tue May  7 09:04:18 2024, max compression
```

## Comparing `composo-0.1.35.tar` & `composo-0.1.37.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 svc       (1000) svc       (1000)        0 2024-03-06 17:54:24.503004 composo-0.1.35/
--rw-r--r--   0 svc       (1000) svc       (1000)     2659 2024-03-01 16:51:39.000000 composo-0.1.35/LICENSE
--rw-r--r--   0 svc       (1000) svc       (1000)      244 2024-03-06 17:54:24.503004 composo-0.1.35/PKG-INFO
--rw-r--r--   0 svc       (1000) svc       (1000)        0 2024-03-01 16:51:39.000000 composo-0.1.35/README.md
-drwxr-xr-x   0 svc       (1000) svc       (1000)        0 2024-03-06 17:54:24.493004 composo-0.1.35/composo/
--rw-r--r--   0 svc       (1000) svc       (1000)    11870 2024-03-06 17:54:24.000000 composo-0.1.35/composo/__init__.py
--rw-r--r--   0 svc       (1000) svc       (1000)     4520 2024-03-01 16:51:39.000000 composo-0.1.35/composo/helpers.py
--rw-r--r--   0 svc       (1000) svc       (1000)     3784 2024-03-01 16:51:39.000000 composo-0.1.35/composo/helpers_test.py
--rw-r--r--   0 svc       (1000) svc       (1000)     6440 2024-03-06 11:19:14.000000 composo-0.1.35/composo/package_primitives.py
-drwxr-xr-x   0 svc       (1000) svc       (1000)        0 2024-03-06 17:54:24.503004 composo-0.1.35/composo.egg-info/
--rw-r--r--   0 svc       (1000) svc       (1000)      244 2024-03-06 17:54:24.000000 composo-0.1.35/composo.egg-info/PKG-INFO
--rw-r--r--   0 svc       (1000) svc       (1000)      273 2024-03-06 17:54:24.000000 composo-0.1.35/composo.egg-info/SOURCES.txt
--rw-r--r--   0 svc       (1000) svc       (1000)        1 2024-03-06 17:54:24.000000 composo-0.1.35/composo.egg-info/dependency_links.txt
--rw-r--r--   0 svc       (1000) svc       (1000)       56 2024-03-06 17:54:24.000000 composo-0.1.35/composo.egg-info/requires.txt
--rw-r--r--   0 svc       (1000) svc       (1000)        8 2024-03-06 17:54:24.000000 composo-0.1.35/composo.egg-info/top_level.txt
--rw-r--r--   0 svc       (1000) svc       (1000)       38 2024-03-06 17:54:24.503004 composo-0.1.35/setup.cfg
--rw-r--r--   0 svc       (1000) svc       (1000)      477 2024-03-06 17:53:29.000000 composo-0.1.35/setup.py
+drwxr-xr-x   0 svc       (1000) svc       (1000)        0 2024-05-07 09:04:18.201907 composo-0.1.37/
+-rw-r--r--   0 svc       (1000) svc       (1000)     2659 2024-04-18 13:19:44.000000 composo-0.1.37/LICENSE
+-rw-r--r--   0 svc       (1000) svc       (1000)      244 2024-05-07 09:04:18.201907 composo-0.1.37/PKG-INFO
+-rw-r--r--   0 svc       (1000) svc       (1000)        0 2024-04-18 13:19:44.000000 composo-0.1.37/README.md
+drwxr-xr-x   0 svc       (1000) svc       (1000)        0 2024-05-07 09:04:18.201907 composo-0.1.37/composo/
+-rw-r--r--   0 svc       (1000) svc       (1000)    12170 2024-05-07 09:04:18.000000 composo-0.1.37/composo/__init__.py
+-rw-r--r--   0 svc       (1000) svc       (1000)     4519 2024-04-18 13:19:44.000000 composo-0.1.37/composo/helpers.py
+-rw-r--r--   0 svc       (1000) svc       (1000)     3784 2024-04-18 13:19:44.000000 composo-0.1.37/composo/helpers_test.py
+-rw-r--r--   0 svc       (1000) svc       (1000)     6440 2024-05-06 14:46:22.000000 composo-0.1.37/composo/package_primitives.py
+drwxr-xr-x   0 svc       (1000) svc       (1000)        0 2024-05-07 09:04:18.201907 composo-0.1.37/composo.egg-info/
+-rw-r--r--   0 svc       (1000) svc       (1000)      244 2024-05-07 09:04:18.000000 composo-0.1.37/composo.egg-info/PKG-INFO
+-rw-r--r--   0 svc       (1000) svc       (1000)      273 2024-05-07 09:04:18.000000 composo-0.1.37/composo.egg-info/SOURCES.txt
+-rw-r--r--   0 svc       (1000) svc       (1000)        1 2024-05-07 09:04:18.000000 composo-0.1.37/composo.egg-info/dependency_links.txt
+-rw-r--r--   0 svc       (1000) svc       (1000)       56 2024-05-07 09:04:18.000000 composo-0.1.37/composo.egg-info/requires.txt
+-rw-r--r--   0 svc       (1000) svc       (1000)        8 2024-05-07 09:04:18.000000 composo-0.1.37/composo.egg-info/top_level.txt
+-rw-r--r--   0 svc       (1000) svc       (1000)       38 2024-05-07 09:04:18.201907 composo-0.1.37/setup.cfg
+-rw-r--r--   0 svc       (1000) svc       (1000)      477 2024-05-07 09:03:21.000000 composo-0.1.37/setup.py
```

### Comparing `composo-0.1.35/LICENSE` & `composo-0.1.37/LICENSE`

 * *Files identical despite different names*

### Comparing `composo-0.1.35/composo/__init__.py` & `composo-0.1.37/composo/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-_F='CustomStreamWrapper'
-_E='Stream'
+_H='CustomStreamWrapper'
+_G='Stream'
+_F=False
+_E='put'
 _D='local'
 _C='prod'
 _B='PACKAGE_ENV'
 _A=None
-__version__='0.1.35'
-import os,inspect,copy,time,math,json
+__version__='0.1.37'
+import datetime,os,inspect,copy,time,math,json
 from typing import List,Union,Any,Literal
+from urllib import response
+from regex import D
 import requests
 from dataclasses import dataclass,asdict
 from composo.package_primitives import*
 from composo.helpers import parse_parameters,generate_api_key,parse_return_type,stream_handler
+from typing import ClassVar,Dict,Protocol,Any
 import logging
 from colorama import init,Fore
 init()
 def conditional_raise(x):
 	'\n    Allow errors to be raised in local\n    '
 	if os.environ.get(_B,_C)==_D:raise x
 def check_is_jsonable(x):
@@ -23,61 +28,60 @@
 class ComposoLogHandler(logging.StreamHandler):
 	def __new__(cls,*args,**kwargs):return super(ComposoLogHandler,cls).__new__(cls)
 	def __init__(self,stream=_A):super().__init__(stream)
 	def emit(self,record):record.msg=f"{Fore.YELLOW}Composo:{Fore.RESET} {record.msg}";super().emit(record)
 packageLogger=logging.getLogger('ComposoLogger')
 if os.environ.get(_B,_C)in[_D,'dev']:print("Using DEBUG logging as you're running locally");packageLogger.setLevel(logging.DEBUG)
 else:packageLogger.setLevel(logging.INFO)
-handler=ComposoLogHandler()
-formatter=logging.Formatter('%(asctime)s - %(message)s',datefmt='%Y-%m-%d %H:%M:%S')
-handler.setFormatter(formatter)
-packageLogger.addHandler(handler)
 if os.environ.get(_B,_C)==_D:packageLogger.info('Connecting to Composo local');BACKEND_URL='http://localhost:8000';FRONTEND_URL='http://localhost:5173'
 elif os.environ.get(_B,_C)=='dev':packageLogger.info('Connecting to Composo dev');BACKEND_URL='https://composo-prod-backend-composo-dev-backend.azurewebsites.net';FRONTEND_URL=BACKEND_URL
 elif os.environ.get(_B,_C)=='test':packageLogger.info('Connecting to Composo test');BACKEND_URL='http://composo-prod-backend-composo-test-backend.azurewebsites.net';FRONTEND_URL=BACKEND_URL
 else:BACKEND_URL='https://app.composo.ai';FRONTEND_URL=BACKEND_URL
+handler=ComposoLogHandler()
+formatter=logging.Formatter('%(asctime)s - %(message)s',datefmt='%Y-%m-%d %H:%M:%S')
+handler.setFormatter(formatter)
+packageLogger.addHandler(handler)
+class IsDataclass(Protocol):__dataclass_fields__:0
+def make_request(method,path,data=_A,timeout=100,max_tries=100):
+	packageLogger.debug(f"Request started path: {path}");headers={'Content-Type':'application/json'};url=BACKEND_URL+path;tries=0
+	while tries<max_tries:
+		try:
+			if method.lower()=='post':json_data=json.dumps(asdict(data),default=str);response=requests.post(url,data=json_data,headers=headers,timeout=timeout)
+			elif method.lower()=='get':response=requests.get(url,headers=headers,timeout=timeout)
+			elif method.lower()==_E:json_data=json.dumps(asdict(data),default=str);response=requests.put(url,data=json_data,headers=headers,timeout=timeout)
+			else:raise ValueError('Invalid method. Available options are "post", "get", and "put".')
+			if tries>0:packageLogger.info('Connection to Composo backend re-established')
+			packageLogger.debug(f"Request finished path: {path}");return response
+		except requests.exceptions.Timeout as e:packageLogger.info(f"Request to Composo timed out. Retry {tries+1} of {max_tries}");time.sleep(max(10*(tries/10)**2,10));tries+=1
+		except requests.exceptions.ConnectionError as e:packageLogger.info(f"Could not connect to Composo. Retry {tries+1} of {max_tries}");time.sleep(max(10*(tries/10)**2,10));tries+=1
+		except Exception as e:raise ComposoDeveloperException(f"There was an unexpected error in make request: {str(e)}")
+	raise ComposoCriticalException(f"Could not connect to Composo backend after {max_tries} tries.")
 class BackendEventGress:
-	def __init__(self,app_registration):self.app_registration=app_registration
-	def make_request(self,method,path,data=_A):
-		packageLogger.debug(f"Request started path: {path}")
-		if not type(data)==dict or data is _A:raise ComposoDeveloperException("Data must be a dict or None. Something's gone wrong.")
-		jsondump=json.dumps(data,default=str);headers={'Content-Type':'application/json'};url=BACKEND_URL+path;tries=0;max_tries=100
-		while tries<max_tries:
-			try:
-				if method.lower()=='post':response=requests.post(url,data=jsondump,headers=headers,timeout=100)
-				elif method.lower()=='get':response=requests.get(url,headers=headers,timeout=100)
-				elif method.lower()=='put':response=requests.put(url,data=jsondump,headers=headers,timeout=100)
-				else:raise ValueError('Invalid method. Available options are "post", "get", and "put".')
-				if tries>0:packageLogger.info('Connection to Composo backend re-established')
-				packageLogger.debug(f"Request finished path: {path}");return response
-			except requests.exceptions.Timeout as e:packageLogger.info(f"Request to Composo timed out. Retry {tries+1} of {max_tries}");time.sleep(max(10*(tries/10)**2,10));tries+=1
-			except requests.exceptions.ConnectionError as e:packageLogger.info(f"Could not connect to Composo. Retry {tries+1} of {max_tries}");time.sleep(max(10*(tries/10)**2,10));tries+=1
-			except Exception as e:raise ComposoDeveloperException(f"There was an unexpected error in backend polling: {str(e)}")
-		raise ComposoCriticalException(f"Could not connect to Composo backend after {max_tries} tries.")
-class LiveEventIngress(BackendEventGress):
-	def event_poll(self):
-		A='message';response=self.make_request(method='post',path='/api/runner',data=asdict(self.app_registration))
+	@staticmethod
+	def update_last_active(runner_id):make_request(_E,path=f"/api/runner/{runner_id}",data=RunnerUpdate(last_active=datetime.datetime.now(datetime.timezone.utc)))
+	def event_poll(self,this_runner_id):
+		A='message';response=make_request(method='get',path=f"/api/runner/package/{this_runner_id}")
 		if response.status_code==200:
 			json_response=response.json()
 			try:
 				parsed_event=PollResponse(**json_response)
 				try:trigger=RunTrigger(**parsed_event.payload);cases=[CaseTrigger(**x)for x in trigger.cases];trigger.cases=cases;parsed_event.payload=trigger;return parsed_event
 				except:pass
 				try:parsed_event.payload=AppDeletionEvent(**parsed_event.payload);return parsed_event
 				except:pass
 				parsed_event.payload=_A;return parsed_event
 			except Exception as e:raise ComposoDeveloperException(f"Could not parse the response from the backend into a known response type: {response}")
 		elif response.status_code==418:packageLogger.error(f"ERROR: {response.json()[A]}")
 		elif response.status_code==501:ComposoDeveloperException(f"POLLING ERROR: {response.json()[A]}")
 		else:raise ComposoDeveloperException(f"The backend is returning an unknown error from polling: {response}")
-class LiveEventEgress(BackendEventGress):
 	def report_run_results(self,run_result,run_id):
-		response=self.make_request('put',path=f"/api/runner/{run_id}",data=asdict(run_result))
+		response=make_request(_E,path=f"/api/runner/package/{run_id}",data=run_result)
 		if response.status_code==200:packageLogger.info('Run completed and results reported')
 		else:raise ComposoDeveloperException(f"The backend is returning a non 200 status code from reporting run results, this should never happen: {response}")
+	def register_runner(self,api_key,adjustable_params,auto_bump,version,docstring):response=make_request('post','/api/runner',data=RunnerCreate(api_key=api_key,parameters=adjustable_params,runner_type='python',package_version=__version__,docstring=docstring,auto_bump=auto_bump,version=version),max_tries=1);return response
 def run_experiment(replacement_vars,all_vars,func):
 	'\n    Takes a dict replacement_vars where both values are json str dump, conversion to the correct type is handled inside\n    ';packageLogger.info('Experiment initiated')
 	if not all(key in[x.name for x in all_vars]for key in replacement_vars.keys()):raise ComposoDeveloperException(f"The user has somehow been allowed to provide args that are not tagged. Provided args: {replacement_vars.keys()}. Tagged args: {[x.name for x in all_vars]} ")
 	working_args=[];working_kwargs={}
 	for arg in copy.deepcopy(all_vars):
 		pushme=lambda x:working_args.append(x)if not arg.is_kwarg else working_kwargs.update({arg.name:x})
 		def typeme(x):
@@ -86,68 +90,66 @@
 		validate_me=lambda x:arg.validate(x)
 		if type(arg)==FixedParameter:pushme(arg.live_working_value)
 		elif arg.name in replacement_vars:typed=typeme(replacement_vars[arg.name]);validate_me(typed);pushme(typed)
 		else:typed=typeme(arg.demo_value);validate_me(typed);pushme(typed)
 	try:ret_val=func(*working_args,**working_kwargs)
 	except Exception as e:raise ComposoUserException(f"The linked function produced an error: {str(e)}")
 	return ret_val
-def experiment_controller(func,demo_args,demo_kwargs,demo_globals,api_key='cp-XXX_FAKE_KEY_FOR_TESTING_XXXX',event_ingress=_A,event_egress=_A,poll_wait_time=3):
-	'\n    Args:\n        event_ingress (_type_): server-side events from polling\n        event_egress (_type_): various backend methods\n\n    ';A='POLL_WAIT_TIME'
-	if os.environ.get(A)is not _A:
-		try:_poll_wait_time=int(os.environ.get(A));assert _poll_wait_time>=1 and _poll_wait_time<10;poll_wait_time=_poll_wait_time
+def experiment_controller(func,demo_args,demo_kwargs,demo_globals,api_key='cp-XXX_FAKE_KEY_FOR_TESTING_XXXX',auto_bump=_F,version=_A,event_gress=_A,poll_wait_time=3):
+	C='########################################';B='POLL_WAIT_TIME';A='id'
+	if os.environ.get(B)is not _A:
+		try:_poll_wait_time=int(os.environ.get(B));assert _poll_wait_time>=1 and _poll_wait_time<10;poll_wait_time=_poll_wait_time
 		except:pass
-	packageLogger.info('Composo Experiment is activated');all_vars=parse_parameters(func,*demo_args,**demo_kwargs);return_type=parse_return_type(func);app_is_streaming=return_type in[_E,_F];adjustable_params=[x for x in all_vars if type(x)in WORKABLE_TYPES.__args__];app_registration=AppRegistration(api_key=api_key,runner_type='python',runner_version=__version__,raw_name=func.__name__,parameters=adjustable_params,docstring=inspect.getdoc(func))
-	if event_ingress is _A or event_egress is _A:
+	if event_gress is _A:
 		packageLogger.info('Initialising live connection to Composo')
 		if api_key is _A:raise ValueError('api_key must be provided')
-		event_ingress=LiveEventIngress(app_registration);event_egress=LiveEventEgress(app_registration)
-	elif event_ingress is _A and event_egress is not _A or event_ingress is not _A and event_egress is _A:raise ValueError('event_ingress and event_egress must both be None or both be not None')
-	previously_noted_app_ids=[];packageLogger.info('Connected and listening.')
+		event_gress=BackendEventGress()
+	packageLogger.info('Composo Experiment is activated');all_vars=parse_parameters(func,*demo_args,**demo_kwargs);return_type=parse_return_type(func);app_is_streaming=return_type in[_G,_H];adjustable_params=[x for x in all_vars if type(x)in WORKABLE_TYPES.__args__];docstring=inspect.getdoc(func);response=event_gress.register_runner(api_key,adjustable_params,auto_bump,version,docstring)
+	if response.status_code!=200:raise ComposoDeveloperException(f"Could not register runner: {response.json()}")
+	this_runner=response.json();packageLogger.info(C);packageLogger.info('# FOLLOW THE LINK TO REGISTER YOUR APP #');packageLogger.info(f"{Fore.CYAN}"+FRONTEND_URL+'/link?api_key='+api_key+f"{Fore.RESET}");packageLogger.info('######### Or use your API key ##########');packageLogger.info('### '+api_key+' ###');packageLogger.info(C);previously_noted_app_ids=[];packageLogger.info('Connected and listening.')
 	while True:
 		try:
-			time.sleep(poll_wait_time);event=event_ingress.event_poll()
+			time.sleep(poll_wait_time);BackendEventGress.update_last_active(this_runner[A]);event=event_gress.event_poll(this_runner[A])
 			if isinstance(event,PollResponse):
 				if isinstance(event.payload,AppDeletionEvent):packageLogger.critical('Composo is shutting down.');packageLogger.critical(event.payload.message);return
 				registered_apps=event.registered_apps
 				for registered_app in registered_apps:
 					if registered_app not in previously_noted_app_ids:packageLogger.info(f"App registered: {registered_app}");previously_noted_app_ids.append(registered_app)
 				if event.payload is not _A:
 					packageLogger.info('New Evaluation Run Triggered')
-					def report_case(case):event_egress.report_run_results(RunResult(run_id=event.payload.run_id,results=[case]),run_id=event.payload.run_id)
+					def report_case(case):event_gress.report_run_results(RunResult(run_id=event.payload.run_id,results=[case]),run_id=event.payload.run_id)
 					packageLogger.info(f"Running {len(event.payload.cases)} cases")
 					for case in event.payload.cases:
-						case_result=_A
+						BackendEventGress.update_last_active(this_runner[A]);case_result=_A
 						try:
 							ret=run_experiment(case.vars,all_vars,func)
 							if app_is_streaming:
 								if not hasattr(ret,'__iter__'):raise ComposoUserException('The linked function is returning a stream but the return type is not iterable.')
 								report_case_intermediate=lambda current_value:report_case(CaseResult(case_id=case.case_id,value=current_value,error=_A,output_stream_incomplete=True));final_result=stream_handler(ret,report_case_intermediate)
 							else:final_result=ret
-							case_result=CaseResult(case_id=case.case_id,value=final_result,error=_A,output_stream_incomplete=False);print('Setting output_stream_incomplete to False');print(case_result);report_case(case_result)
+							case_result=CaseResult(case_id=case.case_id,value=final_result,error=_A,output_stream_incomplete=_F);print('Setting output_stream_incomplete to False');print(case_result);report_case(case_result)
 						except ComposoUserException as e:conditional_raise(e);case_result=CaseResult(case_id=case.case_id,value=_A,error='ERROR: '+str(e));report_case(case_result)
 						except Exception as e:conditional_raise(e);packageLogger.debug(f"Unidentified exception caught with case {case}: {str(e)}");case_result=CaseResult(case_id=case.case_id,value=_A,error='ERROR: The composo package has failed with an unidentified error. Please contact composo support.');report_case(case_result)
 		except ComposoDeveloperException as e:conditional_raise(e);packageLogger.debug(f"Composo Developer Exception caught: {str(e)}");pass
 		except ComposoUserException as e:conditional_raise(e);packageLogger.info(f"Composo User Exception caught: {str(e)}")
 		except ComposoCriticalException as e:conditional_raise(e);raise e
 		except Exception as e:conditional_raise(e);packageLogger.debug(f"Unidentified exception caught: {str(e)}");pass
 class Composo:
 	@classmethod
-	def link(cls,api_key=_A):
-		cls.api_key=api_key
+	def link(cls,api_key=_A,auto_bump=_F,version=_A):
 		def actual_decorator(func):
 			def wrapped_func(*args,**kwargs):
-				B='########################################';A='COMPOSO_APP_API_KEY'
+				A='COMPOSO_APP_API_KEY'
 				if not hasattr(Composo,'activated'):
-					cls.activated=True;packageLogger.info('Composo is activated. Running the function once to check for errors...')
+					cls.api_key=api_key;cls.auto_bump=auto_bump;cls.version=version;cls.activated=True;packageLogger.info('Composo is activated. Running the function once to check for errors...')
 					try:result=func(*args,**kwargs)
 					except Exception as e:raise Exception('The function invocation has errors. Please fix before linking to Composo. Error: '+str(e))
-					permissable_return_types=['int','float','str','dict','list','tuple',_F,_E];result_type=type(result).__name__
+					permissable_return_types=['int','float','str','dict','list','tuple',_H,_G];result_type=type(result).__name__
 					if result_type not in permissable_return_types:raise Exception(f"The linked function returned type: {result_type}. Supported return types are {', '.join(permissable_return_types)}")
 					packageLogger.info('Function test run successful.')
 					if cls.api_key is _A:
-						if A in os.environ:api_key=os.environ[A]
-						else:api_key=generate_api_key()
-					else:api_key=cls.api_key
-					packageLogger.info(B);packageLogger.info('# FOLLOW THE LINK TO REGISTER YOUR APP #');packageLogger.info(f"{Fore.CYAN}"+FRONTEND_URL+'/app_link?api_key='+api_key+f"{Fore.RESET}");packageLogger.info('######### Or use your API key ##########');packageLogger.info('### '+api_key+' ###');packageLogger.info(B);experiment_controller(func,args,kwargs,func.__globals__,api_key=api_key);return result
+						if A in os.environ:cls.api_key=os.environ[A]
+						else:cls.api_key=generate_api_key()
+					experiment_controller(func,args,kwargs,func.__globals__,api_key=cls.api_key,auto_bump=cls.auto_bump,version=cls.version);return result
 				else:result=func(*args,**kwargs)
 			return wrapped_func
 		return actual_decorator
```

### Comparing `composo-0.1.35/composo/helpers.py` & `composo-0.1.37/composo/helpers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -128,8 +128,8 @@
             if time.time() - last_callback_at_time > CALLBACK_PERIOD:
                 callback(built_str)
                 last_callback_at_time = time.time()
 
     callback(built_str)
 
     # Finally return the built string
-    return built_str
+    return built_str
```

### Comparing `composo-0.1.35/composo/helpers_test.py` & `composo-0.1.37/composo/helpers_test.py`

 * *Files identical despite different names*

### Comparing `composo-0.1.35/composo/package_primitives.py` & `composo-0.1.37/composo/package_primitives.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 There are good reasons the package has separate schemas from the rest of the app
 1. We don't necessarily want to expose the underlying schema
 2. The package requires quite different objects - notably all input parameters need to be defined in the app parameter
 """
 
+import datetime
+from sys import version
 from typing import List, Union, Any, Optional, Literal
 import uuid
 import enum
 import json
-from dataclasses import dataclass, asdict
+from dataclasses import dataclass
 
 
 ################################
 # Exceptions
 ################################
 class ComposoException(Exception):
     pass
@@ -144,17 +146,15 @@
 
     def cast(self, item):
         return float(item)
 
 
 @dataclass
 class MultiChoiceStrParam(ParameterBase):
-    param_type: Literal[ParameterType.MULTICHOICESTRING] = (
-        ParameterType.MULTICHOICESTRING
-    )
+    param_type: Literal[ParameterType.MULTICHOICESTRING] = ParameterType.MULTICHOICESTRING
     choices: List[str] = None
 
     def __init__(self, choices: List[str] = None, description=None):
         self.description = description
         self.choices = choices
 
     def validate(self, value):
@@ -168,39 +168,31 @@
 
     def cast(self, item):
         return str(item)
 
 
 @dataclass
 class ConversationHistoryParam(ParameterBase):
-    param_type: Literal[ParameterType.CONVERSATIONHISTORY] = (
-        ParameterType.CONVERSATIONHISTORY
-    )
+    param_type: Literal[ParameterType.CONVERSATIONHISTORY] = ParameterType.CONVERSATIONHISTORY
 
     def __init__(self, description=None):
         self.description = description
 
     def validate(self, value):
         if not isinstance(value, list):
-            raise ComposoUserException(
-                f"ConversationHistoryParam is invalid. Must be a list"
-            )
+            raise ComposoUserException(f"ConversationHistoryParam is invalid. Must be a list")
         if not all(isinstance(item, dict) for item in value):
-            raise ComposoUserException(
-                f"ConversationHistoryParam is invalid. Must be a list of dicts"
-            )
+            raise ComposoUserException(f"ConversationHistoryParam is invalid. Must be a list of dicts")
         return value
 
     def cast(self, item):
         return item
 
 
-WORKABLE_TYPES = Union[
-    StrParam, IntParam, FloatParam, MultiChoiceStrParam, ConversationHistoryParam
-]
+WORKABLE_TYPES = Union[StrParam, IntParam, FloatParam, MultiChoiceStrParam, ConversationHistoryParam]
 
 
 @dataclass
 class CaseTrigger:
     case_id: uuid.UUID
     vars: dict
 
@@ -248,14 +240,19 @@
 class RunResult:
     run_id: uuid.UUID
     results: Optional[List[CaseResult]] = None
     error: Optional[str] = None
 
 
 @dataclass
-class AppRegistration:
+class RunnerCreate:
     api_key: str
-    runner_type: Literal["python", "golang"]
-    runner_version: str
-    raw_name: str
     parameters: List[WORKABLE_TYPES]
-    docstring: Optional[str] = None
+    docstring: str
+    runner_type: Literal["python", "golang"]
+    package_version: str
+    auto_bump: bool
+    version: str
+
+@dataclass
+class RunnerUpdate:
+    last_active: datetime.datetime
```

