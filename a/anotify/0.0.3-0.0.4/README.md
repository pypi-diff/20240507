# Comparing `tmp/anotify-0.0.3.tar.gz` & `tmp/anotify-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anotify-0.0.3.tar", last modified: Sun Apr 28 06:23:26 2024, max compression
+gzip compressed data, was "anotify-0.0.4.tar", last modified: Tue May  7 02:30:37 2024, max compression
```

## Comparing `anotify-0.0.3.tar` & `anotify-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 06:23:26.057036 anotify-0.0.3/
-drwxrwxrwx   0        0        0        0 2024-04-28 06:23:26.040988 anotify-0.0.3/ANotify/
--rw-rw-rw-   0        0        0      677 2024-04-26 11:54:00.000000 anotify-0.0.3/ANotify/Nanpush.py
--rw-rw-rw-   0        0        0     2719 2024-04-26 11:56:48.000000 anotify-0.0.3/ANotify/Nemail.py
--rw-rw-rw-   0        0        0      429 2024-04-26 11:57:17.000000 anotify-0.0.3/ANotify/Niyuu.py
--rw-rw-rw-   0        0        0     1610 2024-04-26 11:58:03.000000 anotify-0.0.3/ANotify/Npushplus.py
--rw-rw-rw-   0        0        0      750 2024-04-28 06:22:25.000000 anotify-0.0.3/ANotify/Nserverchan.py
--rw-rw-rw-   0        0        0     6307 2024-04-26 12:01:18.000000 anotify-0.0.3/ANotify/Nwecom.py
--rw-rw-rw-   0        0        0      888 2024-04-26 13:05:21.000000 anotify-0.0.3/ANotify/__init__.py
--rw-rw-rw-   0        0        0     1062 2024-04-26 12:33:33.000000 anotify-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2652 2024-04-28 06:23:26.056035 anotify-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2202 2024-04-26 13:30:03.000000 anotify-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 06:23:26.055036 anotify-0.0.3/anotify.egg-info/
--rw-rw-rw-   0        0        0     2652 2024-04-28 06:23:25.000000 anotify-0.0.3/anotify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      316 2024-04-28 06:23:25.000000 anotify-0.0.3/anotify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 06:23:25.000000 anotify-0.0.3/anotify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-28 06:23:25.000000 anotify-0.0.3/anotify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-28 06:23:25.000000 anotify-0.0.3/anotify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-28 06:23:26.057036 anotify-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      667 2024-04-28 06:23:18.000000 anotify-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:30:37.713216 anotify-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:30:37.713216 anotify-0.0.4/ANotify/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/Nanpush.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/Nemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/Niyuu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/Npushplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/Nserverchan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/Nwecom.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-07 02:30:32.000000 anotify-0.0.4/ANotify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-07 02:30:32.000000 anotify-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-07 02:30:37.713216 anotify-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-07 02:30:32.000000 anotify-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 02:30:37.713216 anotify-0.0.4/anotify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-07 02:30:37.000000 anotify-0.0.4/anotify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-07 02:30:37.000000 anotify-0.0.4/anotify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 02:30:37.000000 anotify-0.0.4/anotify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 02:30:37.000000 anotify-0.0.4/anotify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-07 02:30:37.000000 anotify-0.0.4/anotify.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 02:30:37.713216 anotify-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-07 02:30:32.000000 anotify-0.0.4/setup.py
```

### Comparing `anotify-0.0.3/ANotify/Nemail.py` & `anotify-0.0.4/ANotify/Nemail.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-import smtplib
-from email.mime.text import MIMEText
-from email.mime.multipart import MIMEMultipart
-
-class EmailNotify:
-    def __init__(self, mail_host, mail_user, mail_pass, sender):
-        self.mail_host = mail_host
-        self.mail_user = mail_user
-        self.mail_pass = mail_pass
-        self.sender = sender
-        # 设置email信息
-        self.message = MIMEMultipart()
-        # 发送方信息
-        self.message['From'] = sender
-
-    # 添加附件
-    def add_attachment(self, attachment_filename):
-        attachment = MIMEText(open(attachment_filename,'rb').read(), 'base64', 'utf-8')
-        attachment.add_header("Content-Type","application/octet-stream")
-        attachment.add_header("Content-Disposition", "attachment", filename=attachment_filename)
-        self.message.attach(attachment)
-
-    def send_email(self, subject, text, attachment_filename = None, receiver = '786731256@qq.com'):
-        """发送邮件
-        :subject:               主题
-        :text:                  正文
-        :attachment_filename:   附件文件名
-        :receiver:              收信地址
-        :return:                发送是否成功
-        """
-
-        # 邮件接受方邮箱地址，注意需要[]包裹，这意味着你可以写多个邮件地址群发
-        receivers = [receiver]
-
-        # 正文内容
-        msg = MIMEText(text,'plain','utf-8')
-
-        self.message.attach(msg)
-        # 邮件主题
-        self.message['Subject'] = subject
-
-        # 接受方信息
-        self.message['To'] = receivers[0]
-
-        if attachment_filename is not None:
-            self.add_attachment(attachment_filename)
-
-        # 登录并发送邮件
-        try:
-            smtpObj = smtplib.SMTP()
-            # 连接到服务器
-            smtpObj.connect(self.mail_host,25)
-            # 登录到服务器
-            smtpObj.login(self.mail_user, self.mail_pass)
-            # 发送
-            smtpObj.sendmail(self.sender,receivers,self.message.as_string())
-            # 退出
-            smtpObj.quit()
-            return True
-        except smtplib.SMTPException as e:
-            return False
-
-if __name__ == "__main__":
-    # 邮箱服务器地址
-    MAIL_HOST = ''
-    # 用户名
-    MAIL_USER = ''
-    # 密码(部分邮箱为授权码)
-    MAIL_PASS = ''
-    # 邮件发送方邮箱地址
-    SENDER = ''
-
-    email_notify = EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER)
-    if email_notify.send_email("测试标题", "测试正文", attachment_filename=None, receiver='123@example.com'):
-        print("邮件发送成功√")
-    else:
+import smtplib
+from email.mime.text import MIMEText
+from email.mime.multipart import MIMEMultipart
+
+class EmailNotify:
+    def __init__(self, mail_host, mail_user, mail_pass, sender):
+        self.mail_host = mail_host
+        self.mail_user = mail_user
+        self.mail_pass = mail_pass
+        self.sender = sender
+        # 设置email信息
+        self.message = MIMEMultipart()
+        # 发送方信息
+        self.message['From'] = sender
+
+    # 添加附件
+    def add_attachment(self, attachment_filename):
+        attachment = MIMEText(open(attachment_filename,'rb').read(), 'base64', 'utf-8')
+        attachment.add_header("Content-Type","application/octet-stream")
+        attachment.add_header("Content-Disposition", "attachment", filename=attachment_filename)
+        self.message.attach(attachment)
+
+    def send_email(self, subject, text, attachment_filename = None, receiver = '786731256@qq.com'):
+        """发送邮件
+        :subject:               主题
+        :text:                  正文
+        :attachment_filename:   附件文件名
+        :receiver:              收信地址
+        :return:                发送是否成功
+        """
+
+        # 邮件接受方邮箱地址，注意需要[]包裹，这意味着你可以写多个邮件地址群发
+        receivers = [receiver]
+
+        # 正文内容
+        msg = MIMEText(text,'plain','utf-8')
+
+        self.message.attach(msg)
+        # 邮件主题
+        self.message['Subject'] = subject
+
+        # 接受方信息
+        self.message['To'] = receivers[0]
+
+        if attachment_filename is not None:
+            self.add_attachment(attachment_filename)
+
+        # 登录并发送邮件
+        try:
+            smtpObj = smtplib.SMTP()
+            # 连接到服务器
+            smtpObj.connect(self.mail_host,25)
+            # 登录到服务器
+            smtpObj.login(self.mail_user, self.mail_pass)
+            # 发送
+            smtpObj.sendmail(self.sender,receivers,self.message.as_string())
+            # 退出
+            smtpObj.quit()
+            return True
+        except smtplib.SMTPException as e:
+            return False
+
+if __name__ == "__main__":
+    # 邮箱服务器地址
+    MAIL_HOST = ''
+    # 用户名
+    MAIL_USER = ''
+    # 密码(部分邮箱为授权码)
+    MAIL_PASS = ''
+    # 邮件发送方邮箱地址
+    SENDER = ''
+
+    email_notify = EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER)
+    if email_notify.send_email("测试标题", "测试正文", attachment_filename=None, receiver='123@example.com'):
+        print("邮件发送成功√")
+    else:
         print("邮件发送失败×")
```

### Comparing `anotify-0.0.3/ANotify/Npushplus.py` & `anotify-0.0.4/ANotify/Npushplus.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-import requests
-from enum import Enum
-import json
-
-class TemplateType(Enum):
-    html = 'html'                   # 默认模板，支持html文本
-    txt = 'txt'                     # 纯文本展示，不转义html
-    json = 'json'                   # 内容基于json格式展示
-    markdown = 'markdown'           # 内容基于markdown格式展示
-    cloudMonitor = 'cloudMonitor'   # 阿里云监控报警定制模板
-    jenkins = 'jenkins'             # jenkins插件定制模板
-    route = 'route'                 # 路由器插件定制模板
-    pay = 'pay'                     # 支付成功通知模板
-
-class PushPlusNotify:
-    def __init__(self, token):
-        self.token = token
-        self.base_url = 'http://www.pushplus.plus/send'
-
-    # https://www.pushplus.plus/doc/guide/api.html#%E4%B8%80%E3%80%81%E5%8F%91%E9%80%81%E6%B6%88%E6%81%AF%E6%8E%A5%E5%8F%A3
-    def send_msg(self, msg_title, msg_text, template_type=TemplateType.html):
-        """发送消息
-        :msg_title: 主题
-        :msg_text:  正文
-        :return:    发送是否成功
-        """
-
-        data = {
-            "token": self.token,
-            "title": msg_title,
-            "content": msg_text,
-            "template": template_type.value,
-            "channel": "wechat"
-        }
-
-        response = requests.post(self.base_url, data=json.dumps(data))
-        response.raise_for_status()
-        return response.json()
-
-if __name__ == "__main__":
-    TOKEN = ''
-    print(PushPlusNotify(TOKEN).send_msg("测试标题", "测试正文", TemplateType.txt))
-
+import requests
+from enum import Enum
+import json
+
+class TemplateType(Enum):
+    html = 'html'                   # 默认模板，支持html文本
+    txt = 'txt'                     # 纯文本展示，不转义html
+    json = 'json'                   # 内容基于json格式展示
+    markdown = 'markdown'           # 内容基于markdown格式展示
+    cloudMonitor = 'cloudMonitor'   # 阿里云监控报警定制模板
+    jenkins = 'jenkins'             # jenkins插件定制模板
+    route = 'route'                 # 路由器插件定制模板
+    pay = 'pay'                     # 支付成功通知模板
+
+class PushPlusNotify:
+    def __init__(self, token):
+        self.token = token
+        self.base_url = 'http://www.pushplus.plus/send'
+
+    # https://www.pushplus.plus/doc/guide/api.html#%E4%B8%80%E3%80%81%E5%8F%91%E9%80%81%E6%B6%88%E6%81%AF%E6%8E%A5%E5%8F%A3
+    def send_msg(self, msg_title, msg_text, template_type=TemplateType.html):
+        """发送消息
+        :msg_title: 主题
+        :msg_text:  正文
+        :return:    发送是否成功
+        """
+
+        data = {
+            "token": self.token,
+            "title": msg_title,
+            "content": msg_text,
+            "template": template_type.value,
+            "channel": "wechat"
+        }
+
+        response = requests.post(self.base_url, data=json.dumps(data))
+        response.raise_for_status()
+        return response.json()
+
+if __name__ == "__main__":
+    TOKEN = ''
+    print(PushPlusNotify(TOKEN).send_msg("测试标题", "测试正文", TemplateType.txt))
+
```

### Comparing `anotify-0.0.3/ANotify/__init__.py` & `anotify-0.0.4/ANotify/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-#   __
-#  /__)  _  _     _   _ _/   _
-# / (   (- (/ (/ (- _)  /  _)
-#          /
-
-"""
-Requests HTTP Library
-~~~~~~~~~~~~~~~~~~~~~
-
-Requests is an HTTP library, written in Python, for human beings.
-Basic GET usage:
-
-   >>> import requests
-   >>> r = requests.get('https://www.python.org')
-   >>> r.status_code
-   200
-   >>> b'Python is a programming language' in r.content
-   True
-
-... or POST:
-
-   >>> payload = dict(key1='value1', key2='value2')
-   >>> r = requests.post('https://httpbin.org/post', data=payload)
-   >>> print(r.text)
-   {
-     ...
-     "form": {
-       "key1": "value1",
-       "key2": "value2"
-     },
-     ...
-   }
-
-The other HTTP methods are supported - see `requests.api`. Full documentation
-is at <https://requests.readthedocs.io>.
-
-:copyright: (c) 2017 by Kenneth Reitz.
-:license: Apache 2.0, see LICENSE for more details.
+#   __
+#  /__)  _  _     _   _ _/   _
+# / (   (- (/ (/ (- _)  /  _)
+#          /
+
+"""
+Requests HTTP Library
+~~~~~~~~~~~~~~~~~~~~~
+
+Requests is an HTTP library, written in Python, for human beings.
+Basic GET usage:
+
+   >>> import requests
+   >>> r = requests.get('https://www.python.org')
+   >>> r.status_code
+   200
+   >>> b'Python is a programming language' in r.content
+   True
+
+... or POST:
+
+   >>> payload = dict(key1='value1', key2='value2')
+   >>> r = requests.post('https://httpbin.org/post', data=payload)
+   >>> print(r.text)
+   {
+     ...
+     "form": {
+       "key1": "value1",
+       "key2": "value2"
+     },
+     ...
+   }
+
+The other HTTP methods are supported - see `requests.api`. Full documentation
+is at <https://requests.readthedocs.io>.
+
+:copyright: (c) 2017 by Kenneth Reitz.
+:license: Apache 2.0, see LICENSE for more details.
 """
```

### Comparing `anotify-0.0.3/LICENSE` & `anotify-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `anotify-0.0.3/PKG-INFO` & `anotify-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,98 +1,103 @@
-Metadata-Version: 2.1
-Name: anotify
-Version: 0.0.3
-Summary: Send notifications by multiple channels.
-Home-page: https://github.com/TommyMerlin/ANotify
-Author: 7ommy
-Author-email: tommymerlin0920@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.25.1
-
-![Alt](https://repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg "Repobeats analytics image")
-
-## 安装
-```console
-pip install anotify
-```
-
-## 实例
-### 企业微信
-```python
-from ANotify import Nwecom
-# 企业ID
-CORPID = ''
-# 应用Secret
-CORPSECRET = ''
-# 应用ID
-AgentId = ''
-
-wn = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
-wn.send_msg("test message")
-wn.send_text_card("test title", "test content", "https://www.example.com")
-wn.send_file("./test.txt")
-wn.send_img("./test.png")
-```
-
-### AnPush
-```python
-from ANotify import Nanpush
-TOKEN = ""
-anpush = Nanpush.AnpushNotify(TOKEN)
-anpush.send_msg("title", "content", "channel_id")
-```
-
-### IYUU
-```python
-from ANotify import Niyuu
-TOKEN = ""
-iyuu = Niyuu.IyuuNotify(TOKEN)
-iyuu.send_msg("title", "content")
-```
-
-### PushPlus
-```python
-from ANotify import NPushPlus
-TOKEN = ''
-pushplus = Npushplus.PushPlusNotify(TOKEN)
-pushplus = Npushplus.PushPlusNotify(TOKEN)
-pushplus.send_msg("测试标题", "测试正文", Npushplus.TemplateType.txt)
-msg_json = {
-    "status": 200,
-    "msg": "success"
-}
-pushplus.send_msg("测试标题", msg_json, Npushplus.TemplateType.json)
-pushplus.send_msg("测试标题", "**测试内容**\n- test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)", Npushplus.TemplateType.markdown)
-pushplus.send_msg("测试标题", "测试内容<a href='https://github.com/TommyMerlin/ANotify'>ANotify</a>", Npushplus.TemplateType.html)
-```
-
-### Server酱
-```python
-from ANotify import Nserverchan
-TOKEN = ''
-serverchan = Nserverchan.ServerChanNotify(TOKEN)
-serverchan.send_msg("测试标题", "测试正文")
-```
-
-### Email
-```python
-from ANotify import Nemail
-# 邮箱服务器地址
-MAIL_HOST = ''
-# 用户名
-MAIL_USER = ''
-# 密码(部分邮箱为授权码)
-MAIL_PASS = ''
-# 邮件发送方邮箱地址
-SENDER = ''
-
-email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER)
-if email_notify.send_email("测试标题", "测试正文", attachment_filename=None, receiver='123@example.com'):
-    print("邮件发送成功√")
-else:
-    print("邮件发送失败×")
-```
+Metadata-Version: 2.1
+Name: anotify
+Version: 0.0.4
+Summary: Send notifications by multiple channels.
+Home-page: https://github.com/TommyMerlin/ANotify
+Author: 7ommy
+Author-email: tommymerlin0920@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.15.1
+
+![Alt](https://repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg "Repobeats analytics image")
+
+## 安装
+```console
+pip install anotify
+```
+
+## 实例
+### 企业微信
+[官网](https://work.weixin.qq.com/)
+```python
+from ANotify import Nwecom
+# 企业ID
+CORPID = ''
+# 应用Secret
+CORPSECRET = ''
+# 应用ID
+AgentId = ''
+
+wn = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
+wn.send_msg("test message")
+wn.send_text_card("test title", "test content", "https://www.example.com")
+wn.send_file("./test.txt")
+wn.send_img("./test.png")
+```
+
+### AnPush
+[官网](https://anpush.com/)
+```python
+from ANotify import Nanpush
+TOKEN = ""
+anpush = Nanpush.AnpushNotify(TOKEN)
+anpush.send_msg("title", "content", "channel_id")
+```
+
+### IYUU
+[官网](https://iyuu.cn/)
+```python
+from ANotify import Niyuu
+TOKEN = ""
+iyuu = Niyuu.IyuuNotify(TOKEN)
+iyuu.send_msg("title", "content")
+```
+
+### PushPlus
+[官网](https://www.pushplus.plus/)
+```python
+from ANotify import NPushPlus
+TOKEN = ''
+pushplus = Npushplus.PushPlusNotify(TOKEN)
+pushplus = Npushplus.PushPlusNotify(TOKEN)
+pushplus.send_msg("测试标题", "测试正文", Npushplus.TemplateType.txt)
+msg_json = {
+    "status": 200,
+    "msg": "success"
+}
+pushplus.send_msg("测试标题", msg_json, Npushplus.TemplateType.json)
+pushplus.send_msg("测试标题", "**测试内容**\n- test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)", Npushplus.TemplateType.markdown)
+pushplus.send_msg("测试标题", "测试内容<a href='https://github.com/TommyMerlin/ANotify'>ANotify</a>", Npushplus.TemplateType.html)
+```
+
+### Server酱
+[官网](https://sct.ftqq.com/)
+```python
+from ANotify import Nserverchan
+TOKEN = ''
+serverchan = Nserverchan.ServerChanNotify(TOKEN)
+serverchan.send_msg("测试标题", "测试正文")
+```
+
+### Email
+```python
+from ANotify import Nemail
+# 邮箱服务器地址
+MAIL_HOST = ''
+# 用户名
+MAIL_USER = ''
+# 密码(部分邮箱为授权码)
+MAIL_PASS = ''
+# 邮件发送方邮箱地址
+SENDER = ''
+
+email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER)
+if email_notify.send_email("测试标题", "测试正文", attachment_filename=None, receiver='123@example.com'):
+    print("邮件发送成功√")
+else:
+    print("邮件发送失败×")
+```
```

#### html2text {}

```diff
@@ -1,34 +1,36 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.0.3 Summary: Send notifications
+Metadata-Version: 2.1 Name: anotify Version: 0.0.4 Summary: Send notifications
 by multiple channels. Home-page: https://github.com/TommyMerlin/ANotify Author:
 7ommy Author-email: tommymerlin0920@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: requests>=2.25.1 ![Alt](https://
+File: LICENSE Requires-Dist: requests>=2.15.1 ![Alt](https://
 repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg
 "Repobeats analytics image") ## å®è£ ```console pip install anotify ``` ##
-å®ä¾ ### ä¼ä¸å¾®ä¿¡ ```python from ANotify import Nwecom # ä¼ä¸ID CORPID
-= '' # åºç¨Secret CORPSECRET = '' # åºç¨ID AgentId = '' wn =
-Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
-wn.send_msg("test message") wn.send_text_card("test title", "test content",
-"https://www.example.com") wn.send_file("./test.txt") wn.send_img("./test.png")
-``` ### AnPush ```python from ANotify import Nanpush TOKEN = "" anpush =
+å®ä¾ ### ä¼ä¸å¾®ä¿¡ [å®ç½](https://work.weixin.qq.com/) ```python from
+ANotify import Nwecom # ä¼ä¸ID CORPID = '' # åºç¨Secret CORPSECRET = '' #
+åºç¨ID AgentId = '' wn = Nwecom.WxNotify(corpid=CORPID,
+corpsecret=CORPSECRET, agentid=AgentId) wn.send_msg("test message")
+wn.send_text_card("test title", "test content", "https://www.example.com")
+wn.send_file("./test.txt") wn.send_img("./test.png") ``` ### AnPush [å®ç½]
+(https://anpush.com/) ```python from ANotify import Nanpush TOKEN = "" anpush =
 Nanpush.AnpushNotify(TOKEN) anpush.send_msg("title", "content", "channel_id")
-``` ### IYUU ```python from ANotify import Niyuu TOKEN = "" iyuu =
-Niyuu.IyuuNotify(TOKEN) iyuu.send_msg("title", "content") ``` ### PushPlus
-```python from ANotify import NPushPlus TOKEN = '' pushplus =
-Npushplus.PushPlusNotify(TOKEN) pushplus = Npushplus.PushPlusNotify(TOKEN)
-pushplus.send_msg("æµè¯æ é¢", "æµè¯æ­£æ", Npushplus.TemplateType.txt)
-msg_json = { "status": 200, "msg": "success" } pushplus.send_msg
-("æµè¯æ é¢", msg_json, Npushplus.TemplateType.json) pushplus.send_msg
-("æµè¯æ é¢", "**æµè¯åå®¹**\n- test1\n- [ANotify](https://github.com/
-TommyMerlin/ANotify)", Npushplus.TemplateType.markdown) pushplus.send_msg
-("æµè¯æ é¢", "æµè¯åå®¹_A_N_o_t_i_f_y", Npushplus.TemplateType.html) ``` ###
-Serveré± ```python from ANotify import Nserverchan TOKEN = '' serverchan =
-Nserverchan.ServerChanNotify(TOKEN) serverchan.send_msg("æµè¯æ é¢",
-"æµè¯æ­£æ") ``` ### Email ```python from ANotify import Nemail #
-é®ç®±æå¡å¨å°å MAIL_HOST = '' # ç¨æ·å MAIL_USER = '' # å¯ç 
-(é¨åé®ç®±ä¸ºææç ) MAIL_PASS = '' # é®ä»¶åéæ¹é®ç®±å°å SENDER
-= '' email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER)
-if email_notify.send_email("æµè¯æ é¢", "æµè¯æ­£æ",
+``` ### IYUU [å®ç½](https://iyuu.cn/) ```python from ANotify import Niyuu
+TOKEN = "" iyuu = Niyuu.IyuuNotify(TOKEN) iyuu.send_msg("title", "content") ```
+### PushPlus [å®ç½](https://www.pushplus.plus/) ```python from ANotify import
+NPushPlus TOKEN = '' pushplus = Npushplus.PushPlusNotify(TOKEN) pushplus =
+Npushplus.PushPlusNotify(TOKEN) pushplus.send_msg("æµè¯æ é¢",
+"æµè¯æ­£æ", Npushplus.TemplateType.txt) msg_json = { "status": 200, "msg":
+"success" } pushplus.send_msg("æµè¯æ é¢", msg_json,
+Npushplus.TemplateType.json) pushplus.send_msg("æµè¯æ é¢",
+"**æµè¯åå®¹**\n- test1\n- [ANotify](https://github.com/TommyMerlin/
+ANotify)", Npushplus.TemplateType.markdown) pushplus.send_msg("æµè¯æ é¢",
+"æµè¯åå®¹_A_N_o_t_i_f_y", Npushplus.TemplateType.html) ``` ### Serveré± [å®ç½]
+(https://sct.ftqq.com/) ```python from ANotify import Nserverchan TOKEN = ''
+serverchan = Nserverchan.ServerChanNotify(TOKEN) serverchan.send_msg
+("æµè¯æ é¢", "æµè¯æ­£æ") ``` ### Email ```python from ANotify import
+Nemail # é®ç®±æå¡å¨å°å MAIL_HOST = '' # ç¨æ·å MAIL_USER = '' #
+å¯ç (é¨åé®ç®±ä¸ºææç ) MAIL_PASS = '' # é®ä»¶åéæ¹é®ç®±å°å
+SENDER = '' email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS,
+SENDER) if email_notify.send_email("æµè¯æ é¢", "æµè¯æ­£æ",
 attachment_filename=None, receiver='123@example.com'): print
 ("é®ä»¶åéæåâ") else: print("é®ä»¶åéå¤±è´¥Ã") ```
```

### Comparing `anotify-0.0.3/anotify.egg-info/PKG-INFO` & `anotify-0.0.4/anotify.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,98 +1,103 @@
-Metadata-Version: 2.1
-Name: anotify
-Version: 0.0.3
-Summary: Send notifications by multiple channels.
-Home-page: https://github.com/TommyMerlin/ANotify
-Author: 7ommy
-Author-email: tommymerlin0920@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.25.1
-
-![Alt](https://repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg "Repobeats analytics image")
-
-## 安装
-```console
-pip install anotify
-```
-
-## 实例
-### 企业微信
-```python
-from ANotify import Nwecom
-# 企业ID
-CORPID = ''
-# 应用Secret
-CORPSECRET = ''
-# 应用ID
-AgentId = ''
-
-wn = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
-wn.send_msg("test message")
-wn.send_text_card("test title", "test content", "https://www.example.com")
-wn.send_file("./test.txt")
-wn.send_img("./test.png")
-```
-
-### AnPush
-```python
-from ANotify import Nanpush
-TOKEN = ""
-anpush = Nanpush.AnpushNotify(TOKEN)
-anpush.send_msg("title", "content", "channel_id")
-```
-
-### IYUU
-```python
-from ANotify import Niyuu
-TOKEN = ""
-iyuu = Niyuu.IyuuNotify(TOKEN)
-iyuu.send_msg("title", "content")
-```
-
-### PushPlus
-```python
-from ANotify import NPushPlus
-TOKEN = ''
-pushplus = Npushplus.PushPlusNotify(TOKEN)
-pushplus = Npushplus.PushPlusNotify(TOKEN)
-pushplus.send_msg("测试标题", "测试正文", Npushplus.TemplateType.txt)
-msg_json = {
-    "status": 200,
-    "msg": "success"
-}
-pushplus.send_msg("测试标题", msg_json, Npushplus.TemplateType.json)
-pushplus.send_msg("测试标题", "**测试内容**\n- test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)", Npushplus.TemplateType.markdown)
-pushplus.send_msg("测试标题", "测试内容<a href='https://github.com/TommyMerlin/ANotify'>ANotify</a>", Npushplus.TemplateType.html)
-```
-
-### Server酱
-```python
-from ANotify import Nserverchan
-TOKEN = ''
-serverchan = Nserverchan.ServerChanNotify(TOKEN)
-serverchan.send_msg("测试标题", "测试正文")
-```
-
-### Email
-```python
-from ANotify import Nemail
-# 邮箱服务器地址
-MAIL_HOST = ''
-# 用户名
-MAIL_USER = ''
-# 密码(部分邮箱为授权码)
-MAIL_PASS = ''
-# 邮件发送方邮箱地址
-SENDER = ''
-
-email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER)
-if email_notify.send_email("测试标题", "测试正文", attachment_filename=None, receiver='123@example.com'):
-    print("邮件发送成功√")
-else:
-    print("邮件发送失败×")
-```
+Metadata-Version: 2.1
+Name: anotify
+Version: 0.0.4
+Summary: Send notifications by multiple channels.
+Home-page: https://github.com/TommyMerlin/ANotify
+Author: 7ommy
+Author-email: tommymerlin0920@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.15.1
+
+![Alt](https://repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg "Repobeats analytics image")
+
+## 安装
+```console
+pip install anotify
+```
+
+## 实例
+### 企业微信
+[官网](https://work.weixin.qq.com/)
+```python
+from ANotify import Nwecom
+# 企业ID
+CORPID = ''
+# 应用Secret
+CORPSECRET = ''
+# 应用ID
+AgentId = ''
+
+wn = Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
+wn.send_msg("test message")
+wn.send_text_card("test title", "test content", "https://www.example.com")
+wn.send_file("./test.txt")
+wn.send_img("./test.png")
+```
+
+### AnPush
+[官网](https://anpush.com/)
+```python
+from ANotify import Nanpush
+TOKEN = ""
+anpush = Nanpush.AnpushNotify(TOKEN)
+anpush.send_msg("title", "content", "channel_id")
+```
+
+### IYUU
+[官网](https://iyuu.cn/)
+```python
+from ANotify import Niyuu
+TOKEN = ""
+iyuu = Niyuu.IyuuNotify(TOKEN)
+iyuu.send_msg("title", "content")
+```
+
+### PushPlus
+[官网](https://www.pushplus.plus/)
+```python
+from ANotify import NPushPlus
+TOKEN = ''
+pushplus = Npushplus.PushPlusNotify(TOKEN)
+pushplus = Npushplus.PushPlusNotify(TOKEN)
+pushplus.send_msg("测试标题", "测试正文", Npushplus.TemplateType.txt)
+msg_json = {
+    "status": 200,
+    "msg": "success"
+}
+pushplus.send_msg("测试标题", msg_json, Npushplus.TemplateType.json)
+pushplus.send_msg("测试标题", "**测试内容**\n- test1\n- [ANotify](https://github.com/TommyMerlin/ANotify)", Npushplus.TemplateType.markdown)
+pushplus.send_msg("测试标题", "测试内容<a href='https://github.com/TommyMerlin/ANotify'>ANotify</a>", Npushplus.TemplateType.html)
+```
+
+### Server酱
+[官网](https://sct.ftqq.com/)
+```python
+from ANotify import Nserverchan
+TOKEN = ''
+serverchan = Nserverchan.ServerChanNotify(TOKEN)
+serverchan.send_msg("测试标题", "测试正文")
+```
+
+### Email
+```python
+from ANotify import Nemail
+# 邮箱服务器地址
+MAIL_HOST = ''
+# 用户名
+MAIL_USER = ''
+# 密码(部分邮箱为授权码)
+MAIL_PASS = ''
+# 邮件发送方邮箱地址
+SENDER = ''
+
+email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER)
+if email_notify.send_email("测试标题", "测试正文", attachment_filename=None, receiver='123@example.com'):
+    print("邮件发送成功√")
+else:
+    print("邮件发送失败×")
+```
```

#### html2text {}

```diff
@@ -1,34 +1,36 @@
-Metadata-Version: 2.1 Name: anotify Version: 0.0.3 Summary: Send notifications
+Metadata-Version: 2.1 Name: anotify Version: 0.0.4 Summary: Send notifications
 by multiple channels. Home-page: https://github.com/TommyMerlin/ANotify Author:
 7ommy Author-email: tommymerlin0920@gmail.com License: MIT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Requires-Python: >=3.6 Description-Content-Type: text/markdown License-
-File: LICENSE Requires-Dist: requests>=2.25.1 ![Alt](https://
+File: LICENSE Requires-Dist: requests>=2.15.1 ![Alt](https://
 repobeats.axiom.co/api/embed/e1ca45165d69b8370c78d60260a6474b49621fac.svg
 "Repobeats analytics image") ## å®è£ ```console pip install anotify ``` ##
-å®ä¾ ### ä¼ä¸å¾®ä¿¡ ```python from ANotify import Nwecom # ä¼ä¸ID CORPID
-= '' # åºç¨Secret CORPSECRET = '' # åºç¨ID AgentId = '' wn =
-Nwecom.WxNotify(corpid=CORPID, corpsecret=CORPSECRET, agentid=AgentId)
-wn.send_msg("test message") wn.send_text_card("test title", "test content",
-"https://www.example.com") wn.send_file("./test.txt") wn.send_img("./test.png")
-``` ### AnPush ```python from ANotify import Nanpush TOKEN = "" anpush =
+å®ä¾ ### ä¼ä¸å¾®ä¿¡ [å®ç½](https://work.weixin.qq.com/) ```python from
+ANotify import Nwecom # ä¼ä¸ID CORPID = '' # åºç¨Secret CORPSECRET = '' #
+åºç¨ID AgentId = '' wn = Nwecom.WxNotify(corpid=CORPID,
+corpsecret=CORPSECRET, agentid=AgentId) wn.send_msg("test message")
+wn.send_text_card("test title", "test content", "https://www.example.com")
+wn.send_file("./test.txt") wn.send_img("./test.png") ``` ### AnPush [å®ç½]
+(https://anpush.com/) ```python from ANotify import Nanpush TOKEN = "" anpush =
 Nanpush.AnpushNotify(TOKEN) anpush.send_msg("title", "content", "channel_id")
-``` ### IYUU ```python from ANotify import Niyuu TOKEN = "" iyuu =
-Niyuu.IyuuNotify(TOKEN) iyuu.send_msg("title", "content") ``` ### PushPlus
-```python from ANotify import NPushPlus TOKEN = '' pushplus =
-Npushplus.PushPlusNotify(TOKEN) pushplus = Npushplus.PushPlusNotify(TOKEN)
-pushplus.send_msg("æµè¯æ é¢", "æµè¯æ­£æ", Npushplus.TemplateType.txt)
-msg_json = { "status": 200, "msg": "success" } pushplus.send_msg
-("æµè¯æ é¢", msg_json, Npushplus.TemplateType.json) pushplus.send_msg
-("æµè¯æ é¢", "**æµè¯åå®¹**\n- test1\n- [ANotify](https://github.com/
-TommyMerlin/ANotify)", Npushplus.TemplateType.markdown) pushplus.send_msg
-("æµè¯æ é¢", "æµè¯åå®¹_A_N_o_t_i_f_y", Npushplus.TemplateType.html) ``` ###
-Serveré± ```python from ANotify import Nserverchan TOKEN = '' serverchan =
-Nserverchan.ServerChanNotify(TOKEN) serverchan.send_msg("æµè¯æ é¢",
-"æµè¯æ­£æ") ``` ### Email ```python from ANotify import Nemail #
-é®ç®±æå¡å¨å°å MAIL_HOST = '' # ç¨æ·å MAIL_USER = '' # å¯ç 
-(é¨åé®ç®±ä¸ºææç ) MAIL_PASS = '' # é®ä»¶åéæ¹é®ç®±å°å SENDER
-= '' email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS, SENDER)
-if email_notify.send_email("æµè¯æ é¢", "æµè¯æ­£æ",
+``` ### IYUU [å®ç½](https://iyuu.cn/) ```python from ANotify import Niyuu
+TOKEN = "" iyuu = Niyuu.IyuuNotify(TOKEN) iyuu.send_msg("title", "content") ```
+### PushPlus [å®ç½](https://www.pushplus.plus/) ```python from ANotify import
+NPushPlus TOKEN = '' pushplus = Npushplus.PushPlusNotify(TOKEN) pushplus =
+Npushplus.PushPlusNotify(TOKEN) pushplus.send_msg("æµè¯æ é¢",
+"æµè¯æ­£æ", Npushplus.TemplateType.txt) msg_json = { "status": 200, "msg":
+"success" } pushplus.send_msg("æµè¯æ é¢", msg_json,
+Npushplus.TemplateType.json) pushplus.send_msg("æµè¯æ é¢",
+"**æµè¯åå®¹**\n- test1\n- [ANotify](https://github.com/TommyMerlin/
+ANotify)", Npushplus.TemplateType.markdown) pushplus.send_msg("æµè¯æ é¢",
+"æµè¯åå®¹_A_N_o_t_i_f_y", Npushplus.TemplateType.html) ``` ### Serveré± [å®ç½]
+(https://sct.ftqq.com/) ```python from ANotify import Nserverchan TOKEN = ''
+serverchan = Nserverchan.ServerChanNotify(TOKEN) serverchan.send_msg
+("æµè¯æ é¢", "æµè¯æ­£æ") ``` ### Email ```python from ANotify import
+Nemail # é®ç®±æå¡å¨å°å MAIL_HOST = '' # ç¨æ·å MAIL_USER = '' #
+å¯ç (é¨åé®ç®±ä¸ºææç ) MAIL_PASS = '' # é®ä»¶åéæ¹é®ç®±å°å
+SENDER = '' email_notify = Nemail.EmailNotify(MAIL_HOST, MAIL_USER, MAIL_PASS,
+SENDER) if email_notify.send_email("æµè¯æ é¢", "æµè¯æ­£æ",
 attachment_filename=None, receiver='123@example.com'): print
 ("é®ä»¶åéæåâ") else: print("é®ä»¶åéå¤±è´¥Ã") ```
```

