# Comparing `tmp/mysql_study_datamaker_cn-0.0.6.tar.gz` & `tmp/mysql_study_datamaker_cn-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql_study_datamaker_cn-0.0.6.tar", last modified: Mon May  6 08:42:54 2024, max compression
+gzip compressed data, was "mysql_study_datamaker_cn-0.1.0.tar", last modified: Tue May  7 10:46:23 2024, max compression
```

## Comparing `mysql_study_datamaker_cn-0.0.6.tar` & `mysql_study_datamaker_cn-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:54.291696 mysql_study_datamaker_cn-0.0.6/
--rw-rw-rw-   0        0        0     1091 2024-04-28 07:59:25.000000 mysql_study_datamaker_cn-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      912 2024-05-06 08:42:54.291696 mysql_study_datamaker_cn-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      495 2024-04-30 06:17:18.000000 mysql_study_datamaker_cn-0.0.6/README.md
--rw-rw-rw-   0        0        0      407 2024-05-06 08:42:06.000000 mysql_study_datamaker_cn-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-06 08:42:54.291696 mysql_study_datamaker_cn-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:54.259017 mysql_study_datamaker_cn-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:54.277227 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/
--rw-rw-rw-   0        0        0      619 2024-05-06 08:41:18.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/__init__.py
--rw-rw-rw-   0        0        0    10385 2024-05-06 08:41:18.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/datamaker.py
--rw-rw-rw-   0        0        0     1501 2024-04-23 04:28:09.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/new_family.txt
--rw-rw-rw-   0        0        0    28630 2024-04-23 04:24:33.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/new_names.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 08:42:54.291696 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN.egg-info/
--rw-rw-rw-   0        0        0      912 2024-05-06 08:42:54.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2024-05-06 08:42:54.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 08:42:54.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-06 08:42:54.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 10:46:23.805477 mysql_study_datamaker_cn-0.1.0/
+-rw-rw-rw-   0        0        0     1091 2024-04-28 07:59:25.000000 mysql_study_datamaker_cn-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      912 2024-05-07 10:46:23.800489 mysql_study_datamaker_cn-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2024-04-30 06:17:18.000000 mysql_study_datamaker_cn-0.1.0/README.md
+-rw-rw-rw-   0        0        0      407 2024-05-07 10:25:44.000000 mysql_study_datamaker_cn-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-07 10:46:23.806017 mysql_study_datamaker_cn-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-07 10:46:23.743461 mysql_study_datamaker_cn-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-07 10:46:23.775618 mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN/
+-rw-rw-rw-   0        0        0       90 2024-05-07 10:45:17.000000 mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN/__init__.py
+-rw-rw-rw-   0        0        0    13030 2024-05-07 10:45:31.000000 mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN/datamaker.py
+-rw-rw-rw-   0        0        0     1501 2024-04-23 04:28:09.000000 mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN/new_family.txt
+-rw-rw-rw-   0        0        0    28630 2024-04-23 04:24:33.000000 mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN/new_names.txt
+drwxrwxrwx   0        0        0        0 2024-05-07 10:46:23.795060 mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN.egg-info/
+-rw-rw-rw-   0        0        0      912 2024-05-07 10:46:23.000000 mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-05-07 10:46:23.000000 mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 10:46:23.000000 mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-07 10:46:23.000000 mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN.egg-info/top_level.txt
```

### Comparing `mysql_study_datamaker_cn-0.0.6/LICENSE` & `mysql_study_datamaker_cn-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql_study_datamaker_cn-0.0.6/PKG-INFO` & `mysql_study_datamaker_cn-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql_study_datamaker_CN
-Version: 0.0.6
+Version: 0.1.0
 Summary: Generate some data and convert it to MySQL language.
 Author-email: Kavin <scratch_test@126.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/datamaker.py` & `mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN/datamaker.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
+import random
 import random as r
 from datetime import datetime
 
 
 class DataMaker:
     """
     这个类的目的是为了在学习 MySQL 语言时，创建表结构后，需要很多插入的数据来进行学习测试；
     DataMaker会根据指定的数量生成指定多的随机项，且支持自定义顺序；
     当前的版本只会生成一个 txt 文本，注意最后一行的","要替换成";"才能够插入数据；
     xxx 是你的 MySQL 表名，需要替换，很傻瓜很简单的一个类
     """
 
-    def __init__(self, N, args=("姓名", "年龄", "性别", "生日", "部门"), left=1950, right=2000,
-                 department=None, gender="int", a=0, b=150, file=None):
+    def __init__(self, N, args=("姓名", "性别", "年龄", "生日", "身份证", "部门", "电话"), left=1950, right=2000,
+                 department=None, gender="int", a=0, b=150, phonehead=130, phone=0, IDCITY=('11000', '310101'),
+                 work_num="员工", work_numwidth=3, work_start=1, file=None):
         """
         __information：数据字典
         N：数据个数
-        args：字段列表，目前只支持：姓名,年龄,部门,生日,性别,分数
+        args：字段列表，目前只支持：姓名,年龄,部门,生日,性别,分数,身份证,手机
         left:出生日期左边界，默认情况下不允许小于 1950 （如有需求可自行修改源代码中的判定）
         right:出生日期有边界，默认情况下不允许小于当前年 （自动判定当前年份，拒绝未来人）
         department：默认给了：‘销售部,技术部,售后部,企划部,咨询部,人事部,财务部’，如果需要重新定义部门，需要写字符串，用','分割；
         gender：
             int：默认是数字类型，0 和 1 代表不同性别，没有严格的去区分哪个数字代表男和女；
             cn：中文的 男 女
             en：英文的 M F
@@ -27,38 +29,52 @@
         a：考试分数的随机，最小值；
         b:考试分数的随机，最大值；
         分数只要识别前两个字符是分数就可以，如果想创建多个分数的学生信息，可以写成：
         ("姓名", "年龄", "性别",  "分数1", "分数2", "分数3")
         考试分数默认是 ； 0~150 分，则 a 就是 0， b：就是 150，做了判定修改，支持 b < a
         file：文件名，写入以 x 格式，所以创建后，再次生成会报文件已存在的错误，建议写入当前日期时间，模式为：None或者'date'，
               如果是None则使用 "_mysql_date.txt" , 如果是 "date" 则以此刻时间为基准，也可以自定义名直接写；
+
+        phonehead(int)：前三位，默认是 '130' 这里只是模拟，不是很准确；
+        phone:手机号从 0 开始
+
+        IDCITY：最好元组格式，没有做限制，身份证城市ID头
+        work_num：工号标头
+        work_numwidth：工号编号，当前只支持数字牌号
         """
         self.__informations = {}
 
         self.__N = N
         self.__args = args
         self.__left = left
         self.__right = right
         self.__department = department
         self.__gender = gender
         self.__a = a
         self.__b = b
+        self.__phonehead = phonehead
+        self.__phone = phone
+        self.__IDCITY = IDCITY
+
+        self.__work_num = work_num
+        self.__work_num_width = work_numwidth
+        self.__work_start = work_start
 
         if file is None:
             self.file = "_mysql_date.txt"
         elif not isinstance(file, str):
             raise TypeError("'file' should be a str")
         elif file.lower() == "date":
             now = datetime.now()
             self.file = f"{now.year}{now.month:>02}{now.day:>02} {now.hour:>02}.{now.minute:>02}.{now.second:>02}.txt"
         else:
             self.file = file
-        self.get_info()
+        self.__get_info()
 
-    def get_name(self):
+    def __get_name(self):
         """
         返回随机生成的姓名系统，总共有 300个姓氏，3579个名字；
         如果超过 1,073,700 个姓名，就一定会有重复的名字出现；
         因为没有做去重处理，所以就算生成 2 个随机姓名也有重复出现的概率！
         :param N: 生成名字的个数；
         :return: 返回一个迭代器；
         """
@@ -66,69 +82,72 @@
             names = f.read().splitlines()
 
         with open(__file__[:__file__.rfind("d")] + 'new_family.txt', encoding="utf-8") as f:
             familys = f.read().splitlines()
 
         return ("'" + r.choice(familys) + r.choice(names) + "'" for _ in range(self.__N))
 
-    def is_leapyear(self, year):
+    def __is_leapyear(self, year):
         if year % 4 == 0 and (year % 100 != 0 or year % 400 == 0):
             return True
         return False
 
-    def get_birthday_age(self, left=1950, right=2000, types="birthday"):
+    def __get_birthday_age_ID(self):
         """
         返回的是一个生成器, 根据types的类型来判断返回什么，默认返回的是生日类型；
         年龄具有时效性！如果是前一年生成的，那么下一年则需要变动；
         随机生成生日的函数，这里做了限定，不能低于 1950 生人；
         如果左右的限定不符合规则（如 年份超出当今年份）都会触发异常；
+        因为每个人的身份证号也包含年龄，所以该方法也可以返回身份证号
         :param N: 数量
         :param left: 1950年起，今年；
         :param right: 同 left
-        :param types: 只能是 'birthday' 或者 'age'
+        :param types: 只能是 'birthday' 或者 'age' 或者 ‘ID’
         :return: 生成器
         """
 
-        if not isinstance(left, int) or not isinstance(right, int):
+        if not isinstance(self.__left, int) or not isinstance(self.__right, int):
             raise TypeError('left or right must be int')
         today = datetime.now()
-        if left < 1950 or left > today.year:
+        if self.__left < 1950 or self.__left > today.year:
             raise ValueError(f"left must be '1950 <= left <= {today.year}.'")
-        if right < 1950 or right > today.year:
+        if self.__right < 1950 or self.__right > today.year:
             raise ValueError(f"right must be '1950 <= right <= {today.year}.'")
-        if types not in ["birthday", "age"]:
-            raise ValueError(f"types must be 'birthday' or 'age'")
-        if left > right:
-            left, right = right, left
+        if self.__left > self.__right:
+            self.__left, self.__right = self.__right, self.__left
 
-        years = [year for year in range(left, right + 1)]
+        years = [year for year in range(self.__left, self.__right + 1)]
         months = [month for month in range(1, 13)]
         days1 = [day for day in range(1, 32)]
         days2 = [day for day in range(1, 31)]
         days3 = [day for day in range(1, 30)]
         days4 = [day for day in range(1, 29)]
 
         for i in range(self.__N):
             year = r.choice(years)
-            if types == "birthday":
-                month = r.choice(months)
-                if month in [1, 3, 5, 7, 8, 10, 12]:
-                    day = r.choice(days1)
-                elif month in [4, 6, 9, 11]:
-                    day = r.choice(days2)
-                else:
-                    if self.is_leapyear(year):
-                        day = r.choice(days3)
-                    else:
-                        day = r.choice(days4)
-                yield f"'{year:>02}-{month:>02}-{day:>02}'"
+            month = r.choice(months)
+            if month in [1, 3, 5, 7, 8, 10, 12]:
+                day = r.choice(days1)
+            elif month in [4, 6, 9, 11]:
+                day = r.choice(days2)
             else:
-                yield str(today.year - year)
+                if self.__is_leapyear(year):
+                    day = r.choice(days3)
+                else:
+                    day = r.choice(days4)
+
+            id_head = random.choice(self.__IDCITY)
+            id_end = "".join([str(random.randint(0, 9)) for i in range(3)]) + random.choice("0123456789X")
 
-    def get_gender(self, types="int"):
+            yield [f"\'{year:>02}-{month:>02}-{day:>02}\'",
+                   str(today.year - year),
+                   f"\'{id_head}{year:>02}{month:>02}{day:>02}{id_end}\'"]
+
+
+    def __get_gender(self, types="int"):
         """
         根据传递的类型不同，可以分别用，英文，中文，整数来表达性别；
         注意，英文如果是全拼的 'english' 返回 'Male' 'Female'；
         如果是 'en' 返回 'M' 'F'
         中文的'chinese' 'cn' 都是 ‘男’  ‘女’
         :param N: 返回的数量
         :param types: english, chinese, int, cn, en
@@ -141,90 +160,131 @@
         elif types == "english":
             return ("'" + r.choice(["Male", "Female"]) + "'" for _ in range(self.__N))
         elif types == "en":
             return ("'" + r.choice("MF") + "'" for _ in range(self.__N))
         else:
             return ("'" + r.choice("男女") + "'" for _ in range(self.__N))
 
-    def get_department(self, department=None):
+    def __get_department(self, department=None):
         """
         部门默认是："销售部,技术部,售后部,企划部,咨询部,人事部,财务部"
         可以自定义传递，传递必须是字符串，且用英文','分割
         :param N: 生成个数
         :param department:默认是None
         :return: 生成器
         """
         if department is None:
             department = "销售部,技术部,售后部,企划部,咨询部,人事部,财务部"
         department = department.split(",")
         return ("'" + r.choice(department) + "'" for _ in range(self.__N))
 
-    def get_score(self, a=0, b=150):
+    def __get_phone(self):
+        """
+        模拟随机的手机号
+        :return: 生成器
+        """
+        for i in range(self.__N):
+            yield f'\'{self.__phonehead}{self.__phone:>08}\''
+            self.__phone += 1
+            if self.__phone == 99999999:
+                self.__phonehead += 1
+                self.__phone = 0
+
+
+
+
+    def __get_score(self, a=0, b=150):
         """
         返回随机分数
         :param N: 个数
         :param a: 最低值
         :param b: 最高值
         :return: 返回生成器
         """
         if a > b:
             a, b = b, a
         return (str(r.randint(a, b)) for _ in range(self.__N))
 
-    def get_info(self):
-        infos = "姓名,年龄,部门,生日,性别,分数".split(",")
+    def __get_worknum(self):
+        return (f"{self.__work_num}{i:0>{self.__work_num_width}}" for i in range(self.__work_start, self.__N + self.__work_start))
+
+    def __get_info(self):
+        infos = "姓名,年龄,部门,生日,性别,分数,手机,身份证,工号".split(",")
         for info in self.__args:
-            if info[:2] not in infos:
-                raise ValueError(f"All must be in {infos}, {info} not in.")
+            if info not in infos:
+                if info[:2] != "分数":
+                    raise ValueError(f"All must be in {infos}, {info} not in.")
 
         for item in self.__args:
             if item == "姓名":
-                self.__informations[item] = self.get_name()
-            elif item == "年龄":
-                self.__informations[item] = self.get_birthday_age(left=self.__left, right=self.__right, types="age")
+                self.__informations[item] = self.__get_name()
+            elif item in ["年龄", "生日", "身份证"]:
+                self.__informations["DATE"] = self.__get_birthday_age_ID()
             elif item == "部门":
-                self.__informations[item] = self.get_department(department=self.__department)
-            elif item == "生日":
-                self.__informations[item] = self.get_birthday_age(self.__left, self.__right, types="birthday")
+                self.__informations[item] = self.__get_department(department=self.__department)
             elif item == "性别":
-                self.__informations[item] = self.get_gender(self.__gender)
+                self.__informations[item] = self.__get_gender(self.__gender)
             elif item[:2] == "分数":
-                self.__informations[item] = self.get_score(self.__a, self.__b)
+                self.__informations[item] = self.__get_score(self.__a, self.__b)
+            elif item == "手机":
+                self.__informations[item] = self.__get_phone()
+            elif item == "工号":
+                self.__informations[item] = self.__get_worknum()
 
     def __iter__(self):
         return self
 
     def __next__(self):
 
         result = ""
-        for v in self.__informations.values():
-            result += next(v) + ","
+        for k, v in self.__informations.items():
+            if k == "DATE":
+                temp = next(v)
+                for item in self.__args:
+                    if item == "生日":
+                        result += temp[0] + ","
+                    elif item == "年龄":
+                        result += temp[1] + ","
+                    elif item == "身份证":
+                        result += temp[2] + ","
+
+            else:
+                result += next(v) + ","
         result = result[:-1]
         if not result:
             raise StopIteration
         return result
 
-    @classmethod
-    def create_insertinto(cls, self):
+    def create_insertinto(self):
         """
         需要先生成一个DataMaker对象，来创建指定数量和字段，再调用该方法，写入到一个txt文本中；
         :param self: 生成的对象
         :param file: txt文件名
         :return: None
         """
         with open("insert_into_" + self.file, "x", encoding="utf-8") as f:
-            f.write("insert into xxx values \n")
+            f.write(f"insert into xxx values {('PRIMARYKEY_ID',) + self.__args} \n")
             id = 1
             for line in self:
                 comment = "(" + str(id) + "," + line + "),\n"
                 id += 1
                 f.write(comment)
+                
+    
+def get_help():
+    content = """--- ver 0.1.0 ---
+    该版本支持‘身份证’，‘手机’，‘工号’，及修复了年龄显示 不正确的 bug，
+    如果要使用身份证，需要输入大写 ‘ID’，构造函数IDCITY参数要传递城市开头代码，这里默认给了北京和上海的，
+    如果需要更多的城市可以自己对该参数进行修改，后四位为随机生成，不符合性别及正规规律，单纯模拟，
+    如果有需要末尾是按照需求的可自行修改代码。"""
+    print(content)
 
 
 if __name__ == '__main__':
     """
     下面是案例，直接运行可以获得测试代码，生成15个随机数据；
     """
-    args = ("姓名", "年龄", "性别")
+    get_help()
+    args = ("姓名", "工号", "年龄", "生日", "身份证", "手机", "分数语文")
     one = DataMaker(15, args, left=2010, gender="cn", file='date')
-    DataMaker.create_insertinto(one)
+    one.create_insertinto()
```

### Comparing `mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/new_family.txt` & `mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN/new_family.txt`

 * *Files identical despite different names*

### Comparing `mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/new_names.txt` & `mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN/new_names.txt`

 * *Files identical despite different names*

### Comparing `mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN.egg-info/PKG-INFO` & `mysql_study_datamaker_cn-0.1.0/src/mysql_study_datamaker_CN.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql_study_datamaker_CN
-Version: 0.0.6
+Version: 0.1.0
 Summary: Generate some data and convert it to MySQL language.
 Author-email: Kavin <scratch_test@126.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

