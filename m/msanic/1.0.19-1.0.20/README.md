# Comparing `tmp/msanic-1.0.19-py3-none-any.whl.zip` & `tmp/msanic-1.0.20-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 57060 bytes, number of entries: 42
+Zip file size: 59037 bytes, number of entries: 42
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-19 13:56 msanic/__init__.py
 -rw-rw-rw-  2.0 fat     3462 b- defN 24-Apr-15 07:17 msanic/base_blue.py
 -rw-rw-rw-  2.0 fat     8536 b- defN 24-May-05 02:44 msanic/base_conf.py
 -rw-rw-rw-  2.0 fat     3241 b- defN 24-Mar-25 14:10 msanic/base_server.py
--rw-rw-rw-  2.0 fat     9749 b- defN 24-May-05 02:25 msanic/base_ws.py
+-rw-rw-rw-  2.0 fat     9826 b- defN 24-May-07 10:22 msanic/base_ws.py
 -rw-rw-rw-  2.0 fat     2908 b- defN 24-Apr-28 08:44 msanic/exception.py
 -rw-rw-rw-  2.0 fat     7677 b- defN 24-Apr-15 07:12 msanic/handler_http.py
--rw-rw-rw-  2.0 fat     2724 b- defN 24-May-04 17:16 msanic/handler_ws.py
+-rw-rw-rw-  2.0 fat     2727 b- defN 24-May-07 10:22 msanic/handler_ws.py
 -rw-rw-rw-  2.0 fat      576 b- defN 24-Apr-12 02:20 msanic/middleware.py
 -rw-rw-rw-  2.0 fat    10352 b- defN 24-May-05 02:43 msanic/mult_creator.py
 -rw-rw-rw-  2.0 fat     8531 b- defN 24-Mar-21 14:40 msanic/verify.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-19 13:56 msanic/libs/__init__.py
 -rw-rw-rw-  2.0 fat     7656 b- defN 24-Mar-21 14:40 msanic/libs/base_timed.py
 -rw-rw-rw-  2.0 fat     1276 b- defN 24-Apr-12 09:22 msanic/libs/component.py
 -rw-rw-rw-  2.0 fat     3151 b- defN 24-Apr-28 08:45 msanic/libs/consts.py
@@ -31,14 +31,14 @@
 -rw-rw-rw-  2.0 fat    18726 b- defN 24-Apr-28 08:44 msanic/orm/db_model.py
 -rw-rw-rw-  2.0 fat    11698 b- defN 24-Apr-03 07:45 msanic/orm/mssql_generator.py
 -rw-rw-rw-  2.0 fat    11743 b- defN 24-Apr-28 08:44 msanic/orm/mysql_generator.py
 -rw-rw-rw-  2.0 fat    11720 b- defN 24-Apr-03 07:45 msanic/orm/pgsql_generator.py
 -rw-rw-rw-  2.0 fat     5098 b- defN 24-Apr-12 02:19 msanic/orm/rc_model.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-19 13:56 test/__init__.py
 -rw-rw-rw-  2.0 fat      701 b- defN 24-May-04 15:15 test/test_unit.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-May-05 02:45 msanic-1.0.19.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      878 b- defN 24-May-05 02:45 msanic-1.0.19.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-05 02:45 msanic-1.0.19.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       52 b- defN 24-May-05 02:45 msanic-1.0.19.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       12 b- defN 24-May-05 02:45 msanic-1.0.19.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     3313 b- defN 24-May-05 02:45 msanic-1.0.19.dist-info/RECORD
-42 files, 177758 bytes uncompressed, 51866 bytes compressed:  70.8%
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-May-07 10:22 msanic-1.0.20.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4801 b- defN 24-May-07 10:22 msanic-1.0.20.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-07 10:22 msanic-1.0.20.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       52 b- defN 24-May-07 10:22 msanic-1.0.20.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       12 b- defN 24-May-07 10:22 msanic-1.0.20.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3314 b- defN 24-May-07 10:22 msanic-1.0.20.dist-info/RECORD
+42 files, 181762 bytes uncompressed, 53843 bytes compressed:  70.4%
```

## zipnote {}

```diff
@@ -102,26 +102,26 @@
 
 Filename: test/__init__.py
 Comment: 
 
 Filename: test/test_unit.py
 Comment: 
 
-Filename: msanic-1.0.19.dist-info/LICENSE
+Filename: msanic-1.0.20.dist-info/LICENSE
 Comment: 
 
-Filename: msanic-1.0.19.dist-info/METADATA
+Filename: msanic-1.0.20.dist-info/METADATA
 Comment: 
 
-Filename: msanic-1.0.19.dist-info/WHEEL
+Filename: msanic-1.0.20.dist-info/WHEEL
 Comment: 
 
-Filename: msanic-1.0.19.dist-info/entry_points.txt
+Filename: msanic-1.0.20.dist-info/entry_points.txt
 Comment: 
 
-Filename: msanic-1.0.19.dist-info/top_level.txt
+Filename: msanic-1.0.20.dist-info/top_level.txt
 Comment: 
 
-Filename: msanic-1.0.19.dist-info/RECORD
+Filename: msanic-1.0.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## msanic/base_ws.py

```diff
@@ -12,27 +12,27 @@
 from msanic.libs import tool, tool_ws, tool_dt
 from msanic.libs.manager import WsConnector
 
 
 class RdsWS(ConfDI):
     CMD_MAP = {}
     '''服务命令映射'''
-    conf: BaseConf = None
     ws_manager = WsConnector
 
     dft_type: Union[int, str] = 1
     '''系统默认消息类型'''
     beat_code: Union[int, str] = 1
     '''心跳消息标码'''
     reject_code: Union[int, str] = 2
     '''弹回消息标码'''
     max_history_queue = 100
     '''最大历史消息数量'''
 
     def __init__(self):
+        self.CMD_MAP = {k: v(self.conf, k) for k, v in self.CMD_MAP.items()}
         self.fun_pack_msg: callable = tool_ws.pack_msg
         self.fun_parse_msg: callable = tool_ws.parse_msg
 
     @classmethod
     def init_ws(cls):
         return cls()
 
@@ -92,14 +92,15 @@
 
     async def listen_msg(self, ws, uinfo):
         while 1:
             c_type, c_code, data, extra = self.fun_parse_msg(await ws.recv(), log_fun=self.log.error)
             if c_type and (c_type == self.dft_type) and (c_code == self.beat_code):
                 await ws.send(self.fun_pack_msg(
                     self.dft_type, self.beat_code, data=data, code=self.conf.STA_CODE.PASS, req=extra))
+                continue
             fun = self.CMD_MAP.get(c_type)
             if fun and callable(fun.funapi):
                 msg_arr = None
                 try:
                     msg_arr = await fun.funapi(c_code, uinfo, data)
                     await ws.send(self.fun_pack_msg(c_type, *msg_arr, req=extra))
                 except WebsocketClosed:
```

## msanic/handler_ws.py

```diff
@@ -7,15 +7,15 @@
 from msanic.libs.consts import Code
 
 
 class WsHandler(ConfDI):
     CMD_FUN_MAP = {}
 
     def __init__(self, conf: BaseConf, cmd_type: int):
-        self.__conf = conf
+        self.conf = conf
         self.__cmd_type = cmd_type
 
     @property
     def cmd_type(self):
         return self.__cmd_type
 
     async def funapi(self, cmd, uinfo, data):
@@ -29,15 +29,15 @@
                 return cmd, data, self.sta_code.FAIL, ''
         return cmd, None, self.conf.STA_CODE.FAIL, 'unspecified message.'
 
     async def off_line(self, ukey: Union[int, str]):
         """掉线处理逻辑"""
         pass
 
-    def sendmsg(self, code: Code = None, data: dict or list = None, hint='success'):
+    def sendmsg(self, code: Code = None, data: Union[dict, list] = None, hint='success'):
         if not code:
             code = self.sta_code.PASS
         raise WsRpsMsg(code, data, hint=hint)
 
     def vf_str(self, val, require=False, default='', turn=0, minlen: int = None, maxlen: int = None, p_name=''):
         sta, val_info = verify.vstr(
             val, require=require, default=default, turn=turn, minlen=minlen, maxlen=maxlen, p_name=p_name)
```

## Comparing `msanic-1.0.19.dist-info/LICENSE` & `msanic-1.0.20.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `msanic-1.0.19.dist-info/RECORD` & `msanic-1.0.20.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 msanic/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 msanic/base_blue.py,sha256=ZTQRdgkmmjhcSHMjXHj0gypj3QDu3uKMrZ-LetvkmT4,3462
 msanic/base_conf.py,sha256=6oH0jR4KZWimRoTApIq9LLXyd3tWhfk38BkFELC6-TQ,8536
 msanic/base_server.py,sha256=zqY89X4amLX-xIEr-jZliSTmVnAUH4amWCYwaTmJTSE,3241
-msanic/base_ws.py,sha256=lYo1WzMKQPDQWGJ22sA4kdga6_yoJnezggXgPlZFsf8,9749
+msanic/base_ws.py,sha256=NenWaLhaiycSo9aUuLSmTbHJlzZyvQ5kCi5hXWGVqjg,9826
 msanic/exception.py,sha256=iz1kGBWkcYQ3zwUjreEjojQ9BLFkCabqRTe70ttgBUQ,2908
 msanic/handler_http.py,sha256=MgyJSiwHAPkCP_dVqLZGaDCrVnz86_utqpg7e1-9UGE,7677
-msanic/handler_ws.py,sha256=n31R_rd97bnmsrodRsg3gLzgxBk42Jg3kjDthXt4MmE,2724
+msanic/handler_ws.py,sha256=XWhzv_36FM71Ox8nuhr952b_PjWJeJihm3h8W6pq44M,2727
 msanic/middleware.py,sha256=YCgWTJlELPWWYdMbaHNUIgFFiKHQezMgko3b0g09m-A,576
 msanic/mult_creator.py,sha256=nMIW10dMn9VJvHdVqeCi-YLEN0UMY9y_JcuhxQw-r74,10352
 msanic/verify.py,sha256=JVpivos9g7uBE6a08jI4BfhhsqJMWE-71tdrh2awRwc,8531
 msanic/libs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 msanic/libs/base_timed.py,sha256=IoPAOt_pRxA4_mQKOu_CMd1Mcu7ditijeKERTvzUZ0A,7656
 msanic/libs/component.py,sha256=21DIgD6RU6u36H2kuN0oA1uBdidULpYiZhpMqRX8hxk,1276
 msanic/libs/consts.py,sha256=OHIOgaLY8R8jZRiwDeEDg_3NN7kj-gZ_7HnP6Ccoq4c,3151
@@ -30,13 +30,13 @@
 msanic/orm/db_model.py,sha256=Gd9Zm7DjiEH4xGEqM19Iar-2tTMY5lziRfaBlWOBLZ0,18726
 msanic/orm/mssql_generator.py,sha256=c9q71hljWqBxoNriG0OefwD48w3gVTb62HnFKjreom4,11698
 msanic/orm/mysql_generator.py,sha256=6AMVa9twa7GRCuTlEga5g2zHJvkCD9YocUwGGcvLQ4Q,11743
 msanic/orm/pgsql_generator.py,sha256=BMNDAZ-2X9dPbUOBlhR5UJBfqXWpl23KRgTozleKCCQ,11720
 msanic/orm/rc_model.py,sha256=NcgSVW34eSx_TiMYE9DYrA6Bt_qitTRH5pX3UYqa6ok,5098
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_unit.py,sha256=zIZWr20nXYmLsKZpGZv-dmRuwQTJXyTcAcUDbx3FdF0,701
-msanic-1.0.19.dist-info/LICENSE,sha256=GSAKapQH5ZIGWlpQTA7v5YrfECyaxaohUb1vJX-qepw,1090
-msanic-1.0.19.dist-info/METADATA,sha256=ZxefTvdMCbFRRD8sfZxOc4rPccxvbFFyvKdsj4kgkME,878
-msanic-1.0.19.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-msanic-1.0.19.dist-info/entry_points.txt,sha256=CAoZ_qtmP0HhzVmX9w0oN-KSxoCpdqxjDC4pljoU-l4,52
-msanic-1.0.19.dist-info/top_level.txt,sha256=lT96LXfr87NYrx1PR9GraMGNX9KQ6ImvR88MTHEhBkM,12
-msanic-1.0.19.dist-info/RECORD,,
+msanic-1.0.20.dist-info/LICENSE,sha256=GSAKapQH5ZIGWlpQTA7v5YrfECyaxaohUb1vJX-qepw,1090
+msanic-1.0.20.dist-info/METADATA,sha256=lU_7ylotR3qZuieOaQY8tK3u5jBbzS238SCC6yXqUo4,4801
+msanic-1.0.20.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+msanic-1.0.20.dist-info/entry_points.txt,sha256=CAoZ_qtmP0HhzVmX9w0oN-KSxoCpdqxjDC4pljoU-l4,52
+msanic-1.0.20.dist-info/top_level.txt,sha256=lT96LXfr87NYrx1PR9GraMGNX9KQ6ImvR88MTHEhBkM,12
+msanic-1.0.20.dist-info/RECORD,,
```

