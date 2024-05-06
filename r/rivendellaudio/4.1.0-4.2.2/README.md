# Comparing `tmp/rivendellaudio-4.1.0.tar.gz` & `tmp/rivendellaudio-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fredg/dev/rivendell-v4/apis/pypi/dist/tmp_rtudtck/rivendellaudio-4.1.0.tar", last modified: Fri Aug 11 16:36:51 2023, max compression
+gzip compressed data, was "rivendellaudio-4.2.2.tar", last modified: Mon May  6 23:09:51 2024, max compression
```

## Comparing `rivendellaudio-4.1.0.tar` & `rivendellaudio-4.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2023-08-11 16:36:51.000000 rivendellaudio-4.1.0/
-drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2023-08-11 16:36:51.000000 rivendellaudio-4.1.0/src/
-drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2023-08-11 16:36:51.000000 rivendellaudio-4.1.0/src/rivendellaudio/
--rw-rw-r--   0 fredg     (1000) fredg     (1000)        0 2023-08-11 16:36:44.000000 rivendellaudio-4.1.0/src/rivendellaudio/__init__.py
--rw-rw-r--   0 fredg     (1000) fredg     (1000)    37171 2023-08-11 16:36:44.000000 rivendellaudio-4.1.0/src/rivendellaudio/pypad.py
--rwxrwxr-x   0 fredg     (1000) fredg     (1000)    70798 2023-08-11 16:36:44.000000 rivendellaudio-4.1.0/src/rivendellaudio/rivwebpyapi.py
-drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2023-08-11 16:36:51.000000 rivendellaudio-4.1.0/src/rivendellaudio.egg-info/
--rw-rw-r--   0 fredg     (1000) fredg     (1000)     1290 2023-08-11 16:36:51.000000 rivendellaudio-4.1.0/src/rivendellaudio.egg-info/PKG-INFO
--rw-rw-r--   0 fredg     (1000) fredg     (1000)      334 2023-08-11 16:36:51.000000 rivendellaudio-4.1.0/src/rivendellaudio.egg-info/SOURCES.txt
--rw-rw-r--   0 fredg     (1000) fredg     (1000)        1 2023-08-11 16:36:51.000000 rivendellaudio-4.1.0/src/rivendellaudio.egg-info/dependency_links.txt
--rw-rw-r--   0 fredg     (1000) fredg     (1000)       37 2023-08-11 16:36:51.000000 rivendellaudio-4.1.0/src/rivendellaudio.egg-info/requires.txt
--rw-rw-r--   0 fredg     (1000) fredg     (1000)       15 2023-08-11 16:36:51.000000 rivendellaudio-4.1.0/src/rivendellaudio.egg-info/top_level.txt
--rw-rw-r--   0 fredg     (1000) fredg     (1000)    26530 2023-08-11 16:36:44.000000 rivendellaudio-4.1.0/LICENSE
--rw-rw-r--   0 fredg     (1000) fredg     (1000)       94 2023-08-11 16:36:44.000000 rivendellaudio-4.1.0/pyproject.toml
--rw-rw-r--   0 fredg     (1000) fredg     (1000)     1444 2023-08-11 16:36:51.000000 rivendellaudio-4.1.0/setup.cfg
--rw-rw-r--   0 fredg     (1000) fredg     (1000)     1290 2023-08-11 16:36:51.000000 rivendellaudio-4.1.0/PKG-INFO
+drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2024-05-06 23:09:51.418270 rivendellaudio-4.2.2/
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)    26530 2024-05-06 23:09:47.000000 rivendellaudio-4.2.2/LICENSE
+-rw-r--r--   0 fredg     (1000) fredg     (1000)     1321 2024-05-06 23:09:51.418270 rivendellaudio-4.2.2/PKG-INFO
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)       94 2024-05-06 23:09:47.000000 rivendellaudio-4.2.2/pyproject.toml
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)     1444 2024-05-06 23:09:51.418270 rivendellaudio-4.2.2/setup.cfg
+drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2024-05-06 23:09:51.414270 rivendellaudio-4.2.2/src/
+drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2024-05-06 23:09:51.418270 rivendellaudio-4.2.2/src/rivendellaudio/
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)        0 2024-05-06 23:09:47.000000 rivendellaudio-4.2.2/src/rivendellaudio/__init__.py
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)    38430 2024-05-06 23:09:47.000000 rivendellaudio-4.2.2/src/rivendellaudio/pypad.py
+-rwxrwxr-x   0 fredg     (1000) fredg     (1000)    70798 2024-05-06 23:09:47.000000 rivendellaudio-4.2.2/src/rivendellaudio/rivwebpyapi.py
+drwxrwxr-x   0 fredg     (1000) fredg     (1000)        0 2024-05-06 23:09:51.418270 rivendellaudio-4.2.2/src/rivendellaudio.egg-info/
+-rw-r--r--   0 fredg     (1000) fredg     (1000)     1321 2024-05-06 23:09:51.000000 rivendellaudio-4.2.2/src/rivendellaudio.egg-info/PKG-INFO
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)      334 2024-05-06 23:09:51.000000 rivendellaudio-4.2.2/src/rivendellaudio.egg-info/SOURCES.txt
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)        1 2024-05-06 23:09:51.000000 rivendellaudio-4.2.2/src/rivendellaudio.egg-info/dependency_links.txt
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)       37 2024-05-06 23:09:51.000000 rivendellaudio-4.2.2/src/rivendellaudio.egg-info/requires.txt
+-rw-rw-r--   0 fredg     (1000) fredg     (1000)       15 2024-05-06 23:09:51.000000 rivendellaudio-4.2.2/src/rivendellaudio.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rivendellaudio-4.1.0/src/rivendellaudio/pypad.py` & `rivendellaudio-4.2.2/src/rivendellaudio/pypad.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,16 @@
     def __init__(self,pad_data,config,rd_config):
         self.__fields=pad_data
         self.__config=config
         self.__rd_config=rd_config
 
     def __fromIso8601(self,string):
         try:
+            if len(string)==0:
+                return datetime.datetime()
             return datetime.datetime.strptime(string.strip()[:19],'%Y-%m-%dT%H:%M:%S')
         except AttributeError:
             return ''
 
     def __escapeXml(self,string):
         string=string.replace("&","&amp;")
         string=string.replace("<","&lt;")
@@ -923,49 +925,67 @@
 
         # Open rd.conf(5)
         rd_config=configparser.ConfigParser(interpolation=None)
         rd_config.readfp(open('/etc/rd.conf'))
 
         # Open the syslog
         pypad_name=sys.argv[0].split('/')[-1]
-        syslog.openlog(pypad_name,logoption=syslog.LOG_PID,facility=int(rd_config.get('Identity','SyslogFacility',fallback=syslog.LOG_USER)))
+        syslog.openlog(pypad_name,logoption=syslog.LOG_PID|syslog.LOG_PERROR,facility=int(rd_config.get('Identity','SyslogFacility',fallback=syslog.LOG_USER)))
 
         # Connect to the PAD feed
         sock=socket.socket(socket.AF_INET)
         conn=sock.connect((hostname,port))
         timeout=None
         if self.__timer_interval!=None:
             timeout=self.__timer_interval
             deadline=datetime.datetime.now()+datetime.timedelta(seconds=timeout)
         sel=selectors.DefaultSelector()
         sel.register(sock,selectors.EVENT_READ)
         c=bytes()
-        line=bytes()
-        msg=""
+        msg=bytearray()
 
+        # Process updates
+        bracket_count=0
+        escaped=False
+        quoted=False
         while 1<2:
             if len(sel.select(timeout))==0:
                 now=datetime.datetime.now()
                 if now>=deadline:
                     timeout=self.__timer_interval
                     deadline=now+datetime.timedelta(seconds=timeout)
                     self.__pypad_TimerProcess(self.__config_parser)
                 else:
                     timeout=(deadline-now).total_seconds()
             else:
                 c=sock.recv(1)
-                line+=c
-                if c[0]==10:
-                    linebytes=line.decode('utf-8','replace')
-                    msg+=linebytes
-                    if linebytes=='\r\n':
-                        jdata=json.loads(msg)
-                        if (not self.__active_now_groups and not self.__active_next_groups) or (jdata['padUpdate'] is not None and jdata['padUpdate']['now'] is not None and jdata['padUpdate']['now']['groupName'] in self.__active_now_groups) or (jdata['padUpdate'] is not None and jdata['padUpdate']['next'] is not None and jdata['padUpdate']['next']['groupName'] in self.__active_next_groups):
-                            self.__pypad_Process(Update(jdata,self.__config_parser,rd_config))
-                        msg=""
-                    line=bytes()
-                if self.__timer_interval!=None:
-                    timeout=(deadline-datetime.datetime.now()).total_seconds()
-
+                msg.append(c[0])
+                if (c[0]==92)and(not escaped):   # Matches '\'
+                    escaped=True
+                else:
+                    if (c[0]==34)and(not escaped):   # Matches '"'
+                        quoted=not quoted
+                    else:
+                        if (c[0]==123)and(not quoted):  # Matches '{'
+                            bracket_count+=1
+                        if (c[0]==125)and(not quoted):  # Matches '}'
+                            bracket_count-=1
+                            if bracket_count==0:
+                                ok=False
+                                try:
+                                    jdata=json.loads(msg)
+                                    ok=True
+                                except:
+                                    priority=syslog.LOG_WARNING|(int(rd_config.get('Identity','SyslogFacility',fallback=syslog.LOG_USER))<<3)
+                                    syslog.syslog(priority,'error parsing JSON: "'+msg.decode('utf-8','replace')+'"')
+                                    if rd_config.get('Debugging','KillPypadAfterJsonError',fallback='no').lower()=='yes':
+                                        sys.exit(1)
+                                if ok:
+                                    if (not self.__active_now_groups and not self.__active_next_groups) or (jdata['padUpdate'] is not None and jdata['padUpdate']['now'] is not None and jdata['padUpdate']['now']['groupName'] in self.__active_now_groups) or (jdata['padUpdate'] is not None and jdata['padUpdate']['next'] is not None and jdata['padUpdate']['next']['groupName'] in self.__active_next_groups):
+                                                self.__pypad_Process(Update(jdata,self.__config_parser,rd_config))
+                                msg=bytearray()
+                        if self.__timer_interval!=None:
+                            timeout=(deadline-datetime.datetime.now()).total_seconds()
+                    escaped=False
 
 def SigHandler(signo,stack):
     sys.exit(0)
```

### Comparing `rivendellaudio-4.1.0/src/rivendellaudio/rivwebpyapi.py` & `rivendellaudio-4.2.2/src/rivendellaudio/rivwebpyapi.py`

 * *Files identical despite different names*

### Comparing `rivendellaudio-4.1.0/src/rivendellaudio.egg-info/PKG-INFO` & `rivendellaudio-4.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: rivendellaudio
-Version: 4.1.0
+Version: 4.2.2
 Summary: Python 3 interface to the Rivendell Radio Automation System
 Home-page: https://github.com/ElvishArtisan/rivendell
 Author: Fred Gleason
 Author-email: fredg@paravelsystems.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ElvishArtisan/rivendell/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: mysqlclient>=1.3.12
+Requires-Dist: requests>=2.14.2
 
 This is a Python 3 interface for the Rivendell Radio
 Automation System. It contains the following modules:
 
 - PyPAD. A system for processing Program Associated Data (PAD) generated
 by Rivendell.
 
@@ -33,8 +33,7 @@
 * Logs
 * Podcasts
 * Scheduler Codes
 
 Example scripts for testing and exercising the API can be found in the
 [Rivendell sources](https://github.com/ElvishArtisan/rivendell/tree/qt5)
 in 'apis/rivwebpyapi/tests/'.
-
```

### Comparing `rivendellaudio-4.1.0/LICENSE` & `rivendellaudio-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rivendellaudio-4.1.0/setup.cfg` & `rivendellaudio-4.2.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rivendellaudio
-version = 4.1.0
+version = 4.2.2
 author = Fred Gleason
 author_email = fredg@paravelsystems.com
 description = Python 3 interface to the Rivendell Radio Automation System
 long_description = This is a Python 3 interface for the Rivendell Radio
 	Automation System. It contains the following modules:
 	
 	- PyPAD. A system for processing Program Associated Data (PAD) generated
```

### Comparing `rivendellaudio-4.1.0/PKG-INFO` & `rivendellaudio-4.2.2/src/rivendellaudio.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: rivendellaudio
-Version: 4.1.0
+Version: 4.2.2
 Summary: Python 3 interface to the Rivendell Radio Automation System
 Home-page: https://github.com/ElvishArtisan/rivendell
 Author: Fred Gleason
 Author-email: fredg@paravelsystems.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ElvishArtisan/rivendell/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: mysqlclient>=1.3.12
+Requires-Dist: requests>=2.14.2
 
 This is a Python 3 interface for the Rivendell Radio
 Automation System. It contains the following modules:
 
 - PyPAD. A system for processing Program Associated Data (PAD) generated
 by Rivendell.
 
@@ -33,8 +33,7 @@
 * Logs
 * Podcasts
 * Scheduler Codes
 
 Example scripts for testing and exercising the API can be found in the
 [Rivendell sources](https://github.com/ElvishArtisan/rivendell/tree/qt5)
 in 'apis/rivwebpyapi/tests/'.
-
```

